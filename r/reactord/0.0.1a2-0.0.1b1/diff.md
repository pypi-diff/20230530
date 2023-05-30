# Comparing `tmp/reactord-0.0.1a2.tar.gz` & `tmp/reactord-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactord-0.0.1a2.tar", last modified: Fri Jan 20 14:32:13 2023, max compression
+gzip compressed data, was "reactord-0.0.1b1.tar", last modified: Tue May 30 14:13:03 2023, max compression
```

## Comparing `reactord-0.0.1a2.tar` & `reactord-0.0.1b1.tar`

### file list

```diff
@@ -1,25 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 14:32:13.430785 reactord-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-20 14:32:02.000000 reactord-0.0.1a2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-01-20 14:32:13.430785 reactord-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-01-20 14:32:02.000000 reactord-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 14:32:13.426785 reactord-0.0.1a2/reactord/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 14:32:13.426785 reactord-0.0.1a2/reactord/idealreactor/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/idealreactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53934 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/idealreactor/stationary_pfr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 14:32:13.430785 reactord-0.0.1a2/reactord/mix/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/mix/abstract_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/mix/ideal_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/mix/ideal_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/reactorbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/substance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-20 14:32:02.000000 reactord-0.0.1a2/reactord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 14:32:13.426785 reactord-0.0.1a2/reactord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-01-20 14:32:13.000000 reactord-0.0.1a2/reactord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-20 14:32:13.000000 reactord-0.0.1a2/reactord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 14:32:13.000000 reactord-0.0.1a2/reactord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-20 14:32:13.000000 reactord-0.0.1a2/reactord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-20 14:32:13.000000 reactord-0.0.1a2/reactord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 14:32:13.430785 reactord-0.0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.082556 reactord-0.0.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 14:12:48.000000 reactord-0.0.1b1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-30 14:13:03.082556 reactord-0.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-30 14:12:48.000000 reactord-0.0.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.074556 reactord-0.0.1b1/reactord/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.074556 reactord-0.0.1b1/reactord/flowreactors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/energy_balances/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/energy_balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/energy_balances/adiabatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/energy_balances/isothermic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/energy_balances/noisothermic_all_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/energy_balances/noisothermic_u_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/mass_balances/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/mass_balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/mass_balances/molarflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/pfr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/pressure_balances/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/pressure_balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/pressure_balances/ergun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/flowreactors/stationary_1d/pfr/pressure_balances/isobaric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/kinetic/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/kinetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/kinetic/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/kinetic/kinetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/kinetic/matrix_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/kinetic/reaction_enthalpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20422 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/abstract_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/ideal_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/ideal_solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.078556 reactord-0.0.1b1/reactord/mix/viscosity_mixing_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/viscosity_mixing_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/viscosity_mixing_rules/grunbergnissan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/viscosity_mixing_rules/herningzipperer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/mix/viscosity_mixing_rules/linearmix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.082556 reactord-0.0.1b1/reactord/substance/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/substance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24985 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/substance/substance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/substance/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-30 14:12:48.000000 reactord-0.0.1b1/reactord/substance/thermo_substance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:13:03.074556 reactord-0.0.1b1/reactord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-30 14:13:03.000000 reactord-0.0.1b1/reactord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-30 14:13:03.000000 reactord-0.0.1b1/reactord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:13:03.000000 reactord-0.0.1b1/reactord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 14:13:03.000000 reactord-0.0.1b1/reactord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 14:13:03.000000 reactord-0.0.1b1/reactord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:13:03.082556 reactord-0.0.1b1/setup.cfg
```

### Comparing `reactord-0.0.1a2/LICENCE` & `reactord-0.0.1b1/LICENCE`

 * *Files identical despite different names*

### Comparing `reactord-0.0.1a2/PKG-INFO` & `reactord-0.0.1b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: reactord
-Version: 0.0.1a2
+Version: 0.0.1b1
 Summary: Package for the simulation and design of chemical reactors
 Author-email: "Brandolín, Salvador Eduardo" <salvadorebrandolin@mi.unc.edu.ar>, "Parodi, Adrián" <adrian.parodi@mi.unc.edu.ar>, "Rovezzi, Juan Pablo" <juan.rovezzi@mi.unc.edu.ar>, "Santos, Maricel Del Valle" <maricel.santos@mi.unc.edu.ar>, "Scilipoti, José Antonio" <jscilipoti@unc.edu.ar>
 License: The MIT License
 Project-URL: Homepage, https://github.com/SalvadorBrandolin/reactord
 Keywords: chemical reactor,reactor design,reactor simulation,chemical engineering
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
@@ -32,48 +32,49 @@
 <a href='https://pypi.org/project/reactord/'>
 <img src='https://img.shields.io/pypi/v/reactord'>
 </a>
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)
 ![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)
 [![codecov](https://codecov.io/gh/SalvadorBrandolin/ReactorD/branch/main/graph/badge.svg?token=6E0U0F9AYU)](https://codecov.io/gh/SalvadorBrandolin/ReactorD)
 
-ReactorD (Reactor Design) is a python package whose proposal is to simulate and design reactors for multiple-reaction systems. The intention is to solve the following reactor types in stationary or not-stationary conditions: Plug flow (PFR) and Stirred tank (STR) 
-
-According to requirements, the operation settings can change as follows; 
-
-- Mass Balance:
-	- Homogeneous
-    - Heterogeneous
-    - Continuous
-    - Discontinuous
-    
-- Energy Balance:
-	- Isothermic
-    - Non-isothermic
-    - Adiabatic
-
-- Pressure Balance:
-	- Isobaric
-    - Non-isobaric
-      - Packed bed reactor
-      - Gas phase reaction
-
-
-## Available in version 0.0.1a2
-- Stationary PFR Isothermic - Isobaric Operation
-- Stationary PFR Isothermic - Non-isobaric packed bed reactor Operation
-- Stationary PFR Adiabatic  - Isobaric Operation
-- Stationary PFR Adiabatic  - Non-isobaric packed bed reactor Operation
+ReactorD (Reactor Design) is a `Python` package whose proposal is to simulate 
+and design reactors for multiple-reaction systems. The intention is to solve 
+the following reactor types in stationary or not-stationary conditions: Plug 
+flow (PFR) and Stirred tank (STR) 
+
+## Available in version 0.0.1b1
+- PFR (Border and initial value problems)
+    - Mass Balances
+        - MolarFlow
+    - Energy Balances
+        - Isothermic
+        - Adiabatic
+        - No isothermic (constant U coefficient and refrigerant temperature)
+        - No isothermic (constant U coefficient)
+    - Pressure Balances
+        - Isobaric
+        - Ergun
 
 
 ## Motivation
-Chemical reaction engineering has as its main objective the study and optimization of reactive processes, usually, with a chemical reactor as the protagonist equipment. To design a chemical reactor, it is necessary to consider several physical and chemical phenomena simultaneously, such as the inlet and outlet molar flow of chemical substances, mass transfer, heat transfer, and reaction kinetics. All these contributions to the system's complexity, commonly lead to coupled non-linear algebraic problems, coupled differential equations, or either both coupled algebraic-differential equations that must be solved by numeric algorithms. ReactorD provides an interphase to configure the necessary information for the simulation of the chemical reactors. Also, ReactorD implements the mathematical representations of mass and energy balances of specific reactors for a numerical resolution.
+Chemical reaction engineering has as its main objective the study and 
+optimization of reactive processes, usually, with a chemical reactor as the 
+protagonist equipment. To design a chemical reactor, it is necessary to 
+consider several physical and chemical phenomena simultaneously, such as the 
+inlet and outlet molar flow of chemical substances, mass transfer, heat 
+transfer, and reaction kinetics. All these contributions to the system's 
+complexity, commonly lead to coupled non-linear algebraic problems, coupled 
+differential equations, or either both coupled algebraic-differential 
+equations that must be solved by numeric algorithms. ReactorD provides an 
+interphase to configure the necessary information for the simulation of the 
+chemical reactors. Also, ReactorD implements the mathematical representations 
+of mass and energy balances of specific reactors for a numerical resolution.
 
 ## Requirements
-You need Python 3.7+ to run ReactorD.
+You need Python 3.8+ to run ReactorD.
 
 ## Instalation
 For installing _ReactorD_ you just need to:
 
 ```sh
 pip install reactord
 ```
@@ -85,21 +86,7 @@
 (<a href=adrian.parodi@mi.unc.edu.ar>adrian.parodi@mi.unc.edu.ar</a>)
 Rovezzi, Juan Pablo
 (<a href=juan.rovezzi@mi.unc.edu.ar>juan.rovezzi@mi.unc.edu.ar</a>)
 Santos, Maricel Del Valle
 (<a href=maricel.santos@mi.unc.edu.ar>maricel.santos@mi.unc.edu.ar</a>)
 Scilipoti, José Antonio
 (<a href=jscilipoti@mi.unc.edu.ar>jscilipoti@mi.unc.edu.ar</a>)
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: reactord Version: 0.0.1a2 Summary: Package for the
+Metadata-Version: 2.1 Name: reactord Version: 0.0.1b1 Summary: Package for the
 simulation and design of chemical reactors Author-email: "BrandolÃ­n, Salvador
 Eduardo"
 mi.unc.edu.ar>, "Parodi, AdriÃ¡n"
 parodi@mi.unc.edu.ar>, "Rovezzi, Juan Pablo"
 rovezzi@mi.unc.edu.ar>, "Santos, Maricel Del Valle"
 santos@mi.unc.edu.ar>, "Scilipoti, JosÃ© Antonio"
 unc.edu.ar> License: The MIT License Project-URL: Homepage, https://github.com/
 SalvadorBrandolin/reactord Keywords: chemical reactor,reactor design,reactor
-simulation,chemical engineering Classifier: Development Status :: 2 - Pre-Alpha
+simulation,chemical engineering Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering Description-Content-Type: text/markdown License-File:
 LICENCE # ReactorD ![logo](https://raw.githubusercontent.com/SalvadorBrandolin/
 ReactorD/main/logo.png) [![Binder](https://mybinder.org/badge_logo.svg)](https:
@@ -22,37 +22,33 @@
 69644832889fa9dfcdb974614129be2fda8e4591989fd713a983a21e7fd8d1ad/
 68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4469536f6674436f6d7043692d46414d41462d666664613030]
 [https://img.shields.io/pypi/v/reactord] [![License](https://img.shields.io/
 badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license) !
 [Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg) [![codecov]
 (https://codecov.io/gh/SalvadorBrandolin/ReactorD/branch/main/graph/
 badge.svg?token=6E0U0F9AYU)](https://codecov.io/gh/SalvadorBrandolin/ReactorD)
-ReactorD (Reactor Design) is a python package whose proposal is to simulate and
-design reactors for multiple-reaction systems. The intention is to solve the
-following reactor types in stationary or not-stationary conditions: Plug flow
-(PFR) and Stirred tank (STR) According to requirements, the operation settings
-can change as follows; - Mass Balance: - Homogeneous - Heterogeneous -
-Continuous - Discontinuous - Energy Balance: - Isothermic - Non-isothermic -
-Adiabatic - Pressure Balance: - Isobaric - Non-isobaric - Packed bed reactor -
-Gas phase reaction ## Available in version 0.0.1a2 - Stationary PFR Isothermic
-- Isobaric Operation - Stationary PFR Isothermic - Non-isobaric packed bed
-reactor Operation - Stationary PFR Adiabatic - Isobaric Operation - Stationary
-PFR Adiabatic - Non-isobaric packed bed reactor Operation ## Motivation
-Chemical reaction engineering has as its main objective the study and
-optimization of reactive processes, usually, with a chemical reactor as the
-protagonist equipment. To design a chemical reactor, it is necessary to
-consider several physical and chemical phenomena simultaneously, such as the
-inlet and outlet molar flow of chemical substances, mass transfer, heat
-transfer, and reaction kinetics. All these contributions to the system's
-complexity, commonly lead to coupled non-linear algebraic problems, coupled
-differential equations, or either both coupled algebraic-differential equations
-that must be solved by numeric algorithms. ReactorD provides an interphase to
-configure the necessary information for the simulation of the chemical
-reactors. Also, ReactorD implements the mathematical representations of mass
-and energy balances of specific reactors for a numerical resolution. ##
-Requirements You need Python 3.7+ to run ReactorD. ## Instalation For
-installing _ReactorD_ you just need to: ```sh pip install reactord ``` ##
-Authors BrandolÃ­n, Salvador Eduardo (salvadorebrandolin@mi.unc.edu.ar) Parodi,
-AdriÃ¡n (adrian.parodi@mi.unc.edu.ar) Rovezzi, Juan Pablo
-(juan.rovezzi@mi.unc.edu.ar) Santos, Maricel Del Valle
-(maricel.santos@mi.unc.edu.ar) Scilipoti, JosÃ© Antonio
-(jscilipoti@mi.unc.edu.ar)
+ReactorD (Reactor Design) is a `Python` package whose proposal is to simulate
+and design reactors for multiple-reaction systems. The intention is to solve
+the following reactor types in stationary or not-stationary conditions: Plug
+flow (PFR) and Stirred tank (STR) ## Available in version 0.0.1b1 - PFR (Border
+and initial value problems) - Mass Balances - MolarFlow - Energy Balances -
+Isothermic - Adiabatic - No isothermic (constant U coefficient and refrigerant
+temperature) - No isothermic (constant U coefficient) - Pressure Balances -
+Isobaric - Ergun ## Motivation Chemical reaction engineering has as its main
+objective the study and optimization of reactive processes, usually, with a
+chemical reactor as the protagonist equipment. To design a chemical reactor, it
+is necessary to consider several physical and chemical phenomena
+simultaneously, such as the inlet and outlet molar flow of chemical substances,
+mass transfer, heat transfer, and reaction kinetics. All these contributions to
+the system's complexity, commonly lead to coupled non-linear algebraic
+problems, coupled differential equations, or either both coupled algebraic-
+differential equations that must be solved by numeric algorithms. ReactorD
+provides an interphase to configure the necessary information for the
+simulation of the chemical reactors. Also, ReactorD implements the mathematical
+representations of mass and energy balances of specific reactors for a
+numerical resolution. ## Requirements You need Python 3.8+ to run ReactorD. ##
+Instalation For installing _ReactorD_ you just need to: ```sh pip install
+reactord ``` ## Authors BrandolÃ­n, Salvador Eduardo
+(salvadorebrandolin@mi.unc.edu.ar) Parodi, AdriÃ¡n
+(adrian.parodi@mi.unc.edu.ar) Rovezzi, Juan Pablo (juan.rovezzi@mi.unc.edu.ar)
+Santos, Maricel Del Valle (maricel.santos@mi.unc.edu.ar) Scilipoti, JosÃ©
+Antonio (jscilipoti@mi.unc.edu.ar)
```

### Comparing `reactord-0.0.1a2/README.md` & `reactord-0.0.1b1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,48 +13,49 @@
 <a href='https://pypi.org/project/reactord/'>
 <img src='https://img.shields.io/pypi/v/reactord'>
 </a>
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)
 ![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)
 [![codecov](https://codecov.io/gh/SalvadorBrandolin/ReactorD/branch/main/graph/badge.svg?token=6E0U0F9AYU)](https://codecov.io/gh/SalvadorBrandolin/ReactorD)
 
-ReactorD (Reactor Design) is a python package whose proposal is to simulate and design reactors for multiple-reaction systems. The intention is to solve the following reactor types in stationary or not-stationary conditions: Plug flow (PFR) and Stirred tank (STR) 
-
-According to requirements, the operation settings can change as follows; 
-
-- Mass Balance:
-	- Homogeneous
-    - Heterogeneous
-    - Continuous
-    - Discontinuous
-    
-- Energy Balance:
-	- Isothermic
-    - Non-isothermic
-    - Adiabatic
-
-- Pressure Balance:
-	- Isobaric
-    - Non-isobaric
-      - Packed bed reactor
-      - Gas phase reaction
-
-
-## Available in version 0.0.1a2
-- Stationary PFR Isothermic - Isobaric Operation
-- Stationary PFR Isothermic - Non-isobaric packed bed reactor Operation
-- Stationary PFR Adiabatic  - Isobaric Operation
-- Stationary PFR Adiabatic  - Non-isobaric packed bed reactor Operation
+ReactorD (Reactor Design) is a `Python` package whose proposal is to simulate 
+and design reactors for multiple-reaction systems. The intention is to solve 
+the following reactor types in stationary or not-stationary conditions: Plug 
+flow (PFR) and Stirred tank (STR) 
+
+## Available in version 0.0.1b1
+- PFR (Border and initial value problems)
+    - Mass Balances
+        - MolarFlow
+    - Energy Balances
+        - Isothermic
+        - Adiabatic
+        - No isothermic (constant U coefficient and refrigerant temperature)
+        - No isothermic (constant U coefficient)
+    - Pressure Balances
+        - Isobaric
+        - Ergun
 
 
 ## Motivation
-Chemical reaction engineering has as its main objective the study and optimization of reactive processes, usually, with a chemical reactor as the protagonist equipment. To design a chemical reactor, it is necessary to consider several physical and chemical phenomena simultaneously, such as the inlet and outlet molar flow of chemical substances, mass transfer, heat transfer, and reaction kinetics. All these contributions to the system's complexity, commonly lead to coupled non-linear algebraic problems, coupled differential equations, or either both coupled algebraic-differential equations that must be solved by numeric algorithms. ReactorD provides an interphase to configure the necessary information for the simulation of the chemical reactors. Also, ReactorD implements the mathematical representations of mass and energy balances of specific reactors for a numerical resolution.
+Chemical reaction engineering has as its main objective the study and 
+optimization of reactive processes, usually, with a chemical reactor as the 
+protagonist equipment. To design a chemical reactor, it is necessary to 
+consider several physical and chemical phenomena simultaneously, such as the 
+inlet and outlet molar flow of chemical substances, mass transfer, heat 
+transfer, and reaction kinetics. All these contributions to the system's 
+complexity, commonly lead to coupled non-linear algebraic problems, coupled 
+differential equations, or either both coupled algebraic-differential 
+equations that must be solved by numeric algorithms. ReactorD provides an 
+interphase to configure the necessary information for the simulation of the 
+chemical reactors. Also, ReactorD implements the mathematical representations 
+of mass and energy balances of specific reactors for a numerical resolution.
 
 ## Requirements
-You need Python 3.7+ to run ReactorD.
+You need Python 3.8+ to run ReactorD.
 
 ## Instalation
 For installing _ReactorD_ you just need to:
 
 ```sh
 pip install reactord
 ```
@@ -66,21 +67,7 @@
 (<a href=adrian.parodi@mi.unc.edu.ar>adrian.parodi@mi.unc.edu.ar</a>)
 Rovezzi, Juan Pablo
 (<a href=juan.rovezzi@mi.unc.edu.ar>juan.rovezzi@mi.unc.edu.ar</a>)
 Santos, Maricel Del Valle
 (<a href=maricel.santos@mi.unc.edu.ar>maricel.santos@mi.unc.edu.ar</a>)
 Scilipoti, José Antonio
 (<a href=jscilipoti@mi.unc.edu.ar>jscilipoti@mi.unc.edu.ar</a>)
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

#### html2text {}

```diff
@@ -7,37 +7,33 @@
 69644832889fa9dfcdb974614129be2fda8e4591989fd713a983a21e7fd8d1ad/
 68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4469536f6674436f6d7043692d46414d41462d666664613030]
 [https://img.shields.io/pypi/v/reactord] [![License](https://img.shields.io/
 badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license) !
 [Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg) [![codecov]
 (https://codecov.io/gh/SalvadorBrandolin/ReactorD/branch/main/graph/
 badge.svg?token=6E0U0F9AYU)](https://codecov.io/gh/SalvadorBrandolin/ReactorD)
-ReactorD (Reactor Design) is a python package whose proposal is to simulate and
-design reactors for multiple-reaction systems. The intention is to solve the
-following reactor types in stationary or not-stationary conditions: Plug flow
-(PFR) and Stirred tank (STR) According to requirements, the operation settings
-can change as follows; - Mass Balance: - Homogeneous - Heterogeneous -
-Continuous - Discontinuous - Energy Balance: - Isothermic - Non-isothermic -
-Adiabatic - Pressure Balance: - Isobaric - Non-isobaric - Packed bed reactor -
-Gas phase reaction ## Available in version 0.0.1a2 - Stationary PFR Isothermic
-- Isobaric Operation - Stationary PFR Isothermic - Non-isobaric packed bed
-reactor Operation - Stationary PFR Adiabatic - Isobaric Operation - Stationary
-PFR Adiabatic - Non-isobaric packed bed reactor Operation ## Motivation
-Chemical reaction engineering has as its main objective the study and
-optimization of reactive processes, usually, with a chemical reactor as the
-protagonist equipment. To design a chemical reactor, it is necessary to
-consider several physical and chemical phenomena simultaneously, such as the
-inlet and outlet molar flow of chemical substances, mass transfer, heat
-transfer, and reaction kinetics. All these contributions to the system's
-complexity, commonly lead to coupled non-linear algebraic problems, coupled
-differential equations, or either both coupled algebraic-differential equations
-that must be solved by numeric algorithms. ReactorD provides an interphase to
-configure the necessary information for the simulation of the chemical
-reactors. Also, ReactorD implements the mathematical representations of mass
-and energy balances of specific reactors for a numerical resolution. ##
-Requirements You need Python 3.7+ to run ReactorD. ## Instalation For
-installing _ReactorD_ you just need to: ```sh pip install reactord ``` ##
-Authors BrandolÃ­n, Salvador Eduardo (salvadorebrandolin@mi.unc.edu.ar) Parodi,
-AdriÃ¡n (adrian.parodi@mi.unc.edu.ar) Rovezzi, Juan Pablo
-(juan.rovezzi@mi.unc.edu.ar) Santos, Maricel Del Valle
-(maricel.santos@mi.unc.edu.ar) Scilipoti, JosÃ© Antonio
-(jscilipoti@mi.unc.edu.ar)
+ReactorD (Reactor Design) is a `Python` package whose proposal is to simulate
+and design reactors for multiple-reaction systems. The intention is to solve
+the following reactor types in stationary or not-stationary conditions: Plug
+flow (PFR) and Stirred tank (STR) ## Available in version 0.0.1b1 - PFR (Border
+and initial value problems) - Mass Balances - MolarFlow - Energy Balances -
+Isothermic - Adiabatic - No isothermic (constant U coefficient and refrigerant
+temperature) - No isothermic (constant U coefficient) - Pressure Balances -
+Isobaric - Ergun ## Motivation Chemical reaction engineering has as its main
+objective the study and optimization of reactive processes, usually, with a
+chemical reactor as the protagonist equipment. To design a chemical reactor, it
+is necessary to consider several physical and chemical phenomena
+simultaneously, such as the inlet and outlet molar flow of chemical substances,
+mass transfer, heat transfer, and reaction kinetics. All these contributions to
+the system's complexity, commonly lead to coupled non-linear algebraic
+problems, coupled differential equations, or either both coupled algebraic-
+differential equations that must be solved by numeric algorithms. ReactorD
+provides an interphase to configure the necessary information for the
+simulation of the chemical reactors. Also, ReactorD implements the mathematical
+representations of mass and energy balances of specific reactors for a
+numerical resolution. ## Requirements You need Python 3.8+ to run ReactorD. ##
+Instalation For installing _ReactorD_ you just need to: ```sh pip install
+reactord ``` ## Authors BrandolÃ­n, Salvador Eduardo
+(salvadorebrandolin@mi.unc.edu.ar) Parodi, AdriÃ¡n
+(adrian.parodi@mi.unc.edu.ar) Rovezzi, Juan Pablo (juan.rovezzi@mi.unc.edu.ar)
+Santos, Maricel Del Valle (maricel.santos@mi.unc.edu.ar) Scilipoti, JosÃ©
+Antonio (jscilipoti@mi.unc.edu.ar)
```

### Comparing `reactord-0.0.1a2/reactord/mix/ideal_gas.py` & `reactord-0.0.1b1/reactord/mix/ideal_solution.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,200 +1,212 @@
-"""Ideal gas Module."""
-from typing import List
-
-import chemicals
+"""Ideal solution Module."""
+from typing import List, Union
 
 import numpy as np
+from numpy.typing import NDArray
 
-from reactord.mix.abstract_mix import AbstractMix
 from reactord.substance import Substance
 
+from .abstract_mix import AbstractMix
+
 
-class IdealGas(AbstractMix):
-    """IdealGas object class.
+class IdealSolution(AbstractMix):
+    """IdealSolution object class.
 
-    This class should be used when the mixture is considered an ideal gas.
+    This class should be used when the mixture is considered an ideal solution.
 
     Parameters
     ----------
     substance_list : list [float]
         list of substance objects
+    viscosity_mixing_rule : str, optional
+        Viscosity mixing rule method. Options available: "linear",
+        "grunberg_nissan", "herning_zipperer"., by default "grunberg_nissan"
 
     Attributes
     ----------
-    substances : list [float]
-        list of substance objects
+    phase_nature : str
+        liquid.
+    substances : List [Substance]
+        List of substances.
+    viscosity_mixing_rule : str
+        Viscosity mixing rule method.
     """
 
-    def __init__(self, **substance_dict) -> None:
-
-        substance_list = [
-            value
-            if isinstance(value, Substance)
-            else Substance.from_thermo_database(value)
-            for value in substance_dict.values()
-        ]
-        self.substances = substance_list
-
-    def concentrations(
-        self, moles: List[float], temperature: float, pressure: float
-    ) -> List[float]:
-        """Calculate concentrations of the mixture.
-
-        Parameters
-        ----------
-        moles : ndarray or list [float]
-            Moles of each substance
-        temperature : float
-            System temperature [K]
-        pressure : float
-            System pressure [Pa]
-
-        Returns
-        -------
-        ndarray or list [float]
-            Concentration of each substance [mol/m³]
-        """
-        mol_fractions = self.mol_fractions(moles)
-
-        r = 8.31446261815324  # m³⋅Pa/K/mol
-        density = pressure / (r * temperature)
-        return np.multiply(mol_fractions, density)
+    def __init__(
+        self,
+        substance_list: List[Substance],
+        viscosity_mixing_rule: str = "grunberg_nissan",
+    ) -> None:
+        super().__init__(
+            substance_list=substance_list,
+            phase_nature="liquid",
+            viscosity_mixing_rule=viscosity_mixing_rule,
+        )
 
     def volume(
-        self, moles: List[float], temperature: float, pressure: float
+        self,
+        mole_fractions: List[float],
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
     ) -> float:
-        """Calculate the volume of the mixture.
+        r"""Return the molar volume of the mixture.
+
+        Multiple mixture compositions can be specified by a moles matrix. Each
+        column of the matrix represents each mixture and each row represents
+        each substance's mole fractions. Also with temperature and pressure
+        vectors following de NumPy broadcasting rules.
+
+        .. math::
+            v = \sum z_i {v_i}_{(T,P)}
+
+        | :math:`v`: mix's molar volume.
+        | :math:`z_i`: mole fraction of the mix's :math:`i`-th substance.
+        | :math:`{v_i}_{(T,P)`: liquid molar volume of the mix's :math:`i`-th
+          substance.
+        | :math:`T`: temperature.
+        | :math:`P`: pressure.
 
         Parameters
         ----------
-        moles : ndarray or list[float]
-            Moles of each substance
-        temperature : float
-            System temperature [K]
-        pressure : float
-            System pressure [Pa]
+        mole_fractions : np.Union[float, NDArray[np.float64]]
+            mole fractions of each substance specified in the same order as the
+            mix's substances order.
+        temperature: Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure: Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
         float
-            Volume of the mixture [m³]
+            Mixture's molar volume. [m³/mol]
+
+
+        Requires
+        --------
+            volume_liquid defined on each mix's Substance.
         """
-        total_moles = np.sum(moles)
+        pure_volumes = np.array(
+            [
+                substance.volume_liquid(temperature, pressure)
+                for substance in self.substances
+            ]
+        )
+
+        mix_volumes = np.multiply(pure_volumes, mole_fractions).sum(axis=0)
 
-        r = 8.31446261815324  # m3⋅Pa/K/mol
-        volume = total_moles * r * temperature / pressure
-        return volume
+        return mix_volumes
 
     def mix_heat_capacity(
-        self, moles: List[float], temperature: float, pressure: float
-    ) -> float:
-        """Calculate heat capacity of th mixture.
+        self,
+        mole_fractions: List[float],
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ):
+        r"""Calculate the mixture's heat capacity [J/mol].
+
+        Multiple mixture compositions can be specified by a moles matrix. Each
+        column of the matrix represents each mixture and each row represents
+        each substance's mole fractions. Also with temperature and pressure
+        vectors following de NumPy broadcasting rules.
+
+        .. math::
+            C_{p_{mix}} = \sum_{i=0}^{N} z_i C_{p_i}
+
+        | :math:`C_{p_{mix}}`: mix's heat capacity.
+        | :math:`N`: total number of substances in the mixture.
+        | :math:`C_{p_i}`: ideal gas heat capacity of the mix's
+          :math:`i`-th substance.
+        | :math:`z_i`: mole fraction of the mix's :math:`i`-th substance.
 
         Parameters
         ----------
-        moles : ndarray or list [float]
-            Moles of each substance
-        temperature : float
-            System temperature [K]
+        mole_fractions : np.Union[float, NDArray[np.float64]]
+            mole fractions of each substance specified in the same order as the
+            mix's substances order.
+        temperature: Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure: Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
         float
-            Heat capacity of the mixture [J/K]
-        """
-        mol_fractions = self.mol_fractions(moles)
+            Mixture's heat capacity. [J/mol]
+
 
+        Requires
+        --------
+            heat_capacity_liquid defined on each mix's Substance.
+        """
         pure_cp = np.array(
             [
-                substance.heat_capacity_gas(temperature, pressure)
+                substance.heat_capacity_liquid(temperature, pressure)
                 for substance in self.substances
             ]
         )
-        mix_cp = np.dot(mol_fractions, pure_cp)
-        return mix_cp
-
-    def _formation_enthalpies_set(self):
-        """Return the ideal gas formation enthalpies in a ordered ndarray.
-
-        Method that read the ideal gas formation enthalpies of the mix
-        class and returns them in a ordered ndarray.
-
-        Returns
-        -------
-        ndarray [float]
-            Ideal gas formation enthalpies of each substance [J/mol/K]
-        """
-        enthalpies = np.array([])
 
-        for substance in self.substances:
-            enthalpies = np.append(enthalpies, substance.formation_enthalpy_ig)
-
-        return enthalpies
+        # The next line is equal to a column-wise dot product of the two arrays
+        mix_cp = np.multiply(mole_fractions, pure_cp).sum(axis=0)
+        return mix_cp
 
     def formation_enthalpies_correction(
-        self, temperature: float, pressure: float
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
     ):
         """Calculate the correction term for the formation enthalpy.
 
         Method that calculates the correction term for the formation
         enthalpies of the pure substances from 298.15 K and 101325 Pa to
         the given temperature and pressure using Kirchhoff's equation.
+        If the substance is a solid at a temperature > 298.15 K, this
+        method also takes it into account.
 
         Parameters
         ----------
-        temperature : float
+        temperature : Union[float, NDArray[np.float64]]
             Temperature at which formation enthalpies are to be calculated. [K]
-        pressure : float
+        pressure : Union[float, NDArray[np.float64]]
             Pressure at which formation enthalpies are to be calculated. [Pa]
 
         Returns
         -------
-        correction_enthalpies : ndarray [float]
-            Formation enthalpies of each substance (J/mol/K)
+        correction_enthalpies : Union[float, NDArray[np.float64]]
+            Formation enthalpies correction for each substance (J/mol/K)
         """
         correction_enthalpies = np.array([])
-
         for substance in self.substances:
-            correction_enthalpies = np.append(
-                correction_enthalpies,
-                substance.heat_capacity_gas_dt_integral(
-                    298.15, temperature, pressure
-                ),
-            )
-
+            if substance.normal_melting_point > 298.15:
+                dhs = substance.heat_capacity_solid_dt_integral(
+                    298.15, substance.normal_melting_point, pressure
+                )
+                dhf = substance.fusion_enthalpy(substance.normal_melting_point)
+                dhl = substance.heat_capacity_liquid_dt_integral(
+                    substance.normal_melting_point, temperature, pressure
+                )
+
+                correction_enthalpies = np.append(
+                    correction_enthalpies, dhs + dhf + dhl
+                )
+            else:
+                correction_enthalpies = np.append(
+                    correction_enthalpies,
+                    substance.heat_capacity_liquid_dt_integral(
+                        298.15, temperature, pressure
+                    ),
+                )
         return correction_enthalpies
 
-    def mixture_viscosity(
-        self,
-        moles: List[float],
-        temperature: float,
-        pressure: float,
-    ) -> float:
-        """
-        Evaluate the viscosity of the mixture.
+    def get_formation_enthalpies(self):
+        """Return the formation enthalpies in a ordered ndarray.
+
+        Method that read the formation enthalpies of mix and returns
+        them in a ordered ndarray.
 
-        Parameters
-        ----------
-        temperature : float
-            Temperature at which formation enthalpies are to be calculated. [K]
-        pressure : float
-            Pressure at which formation enthalpies are to be calculated. [Pa]
-        moles: list
-        |   List of moles substance in the mixture
         Returns
         -------
-         mixture_viscosity: float
-            Viscosity of the mixture
+        Union[float, NDArray[np.float64]]
+            Formation enthalpies of each substance
         """
-        mol_fractions = self.mol_fractions(moles)
-        viscosity_pure = []
-        molecular_weight = []
-        for substance in self.substances:
-            viscosity_pure.append(
-                substance.viscosity_gas(temperature, pressure)
-            )
-            molecular_weight.append(substance.molecular_weight)
-
-        return chemicals.viscosity.Herning_Zipperer(
-            mol_fractions, viscosity_pure, molecular_weight
-        )
+        return self.formation_enthalpies
```

### Comparing `reactord-0.0.1a2/reactord/substance.py` & `reactord-0.0.1b1/reactord/substance/substance.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,685 +1,690 @@
 """Substance module.
 
 Class to define a substance for ReactorD library.
 """
-from typing import Callable
+
+from typing import Callable, Union
 
 from dill import dumps, loads
 
 import numpy as np
+from numpy.typing import NDArray
 
-from scipy.integrate import quad
 
-from thermo import ChemicalConstantsPackage
+from .symbolic import Symbolic
+from .thermo_substance import thermo_substance_constructor
 
 
-class Substance:
+class Substance(Symbolic):
     """Substance object class.
 
     Class to define a substance object. Specific attributes definition will be
     required for the reactors, described in each reactor documentation. For
     example, an adiabatic reactor will require that substances define a heat
-    capacity function, on the other hand, when using isothermic reactors this
-    won't be necessary. Substance has the .from_thermo_data_base alternative
-    construction method.
-    E.g:
-
-    water = Substance.from_thermo_data_base('water')
+    capacity function for the substances, on the other hand, when using
+    isothermic reactors this won't be necessary. Substance has the
+    from_thermo_data_base alternative construction method. Substances objects
+    can be saved as pickle files with the method to_pickle. substances can be
+    loaded from a pickle file with the method from_pickle.
+
+    Example:
+
+    >>> water = Substance.from_thermo_data_base('water')
+    >>> water.to_pickle('my_water_file')
+    >>> water_pickle = water.from_pickle('my_water_file)
 
     Parameters
     ----------
-    name : str, optional
-       Name of the substance, by default None
+    name : str
+       Name of the substance.
     molecular_weight : float, optional
-        The molecular weight of the substance [g/mol], by default None
+        The molecular weight of the substance [g/mol], by default None.
     normal_boiling_point : float, optional
-        The normal boiling point of the substance [K], by default None
+        The normal boiling point of the substance [K], by default None.
     normal_melting_point : float, optional
-        The normal melting point of the substance [K], by default None
+        The normal melting point of the substance [K], by default None.
     critical_temperature : float, optional
-        The critical temperature of the substance [K], by default None
+        The critical temperature of the substance [K], by default None.
     critical_pressure : float, optional
-        The critical pressure of the substance [Pa], by default None
+        The critical pressure of the substance [Pa], by default None.
     acentric_factor : float, optional
-        The acentric factor of the substance, by default None
+        The acentric factor of the substance, by default None.
     formation_enthalpy : float, optional
-        Standard state molar enthalpy of formation [J/mol], by default None
+        Standard state molar enthalpy of formation [J/mol], by default None.
     formation_enthalpy_ig : float, optional
-        Ideal-gas molar enthalpy of formation [J/mol], by default None
-    formation_gibbs_ig : float, optional
-        Ideal-gas molar change of Gibbs energy of formation [J/mol], by default
-        None
+        Ideal-gas molar enthalpy of formation [J/mol], by default None.
     vaporization_enthalpy : Callable, optional
         A function that receives a temperature and returns the vaporization
-        enthalpy at that temperature [J/mol], by default None
+        enthalpy at temperature [J/mol], by default None.
     sublimation_enthalpy : Callable, optional
-        A function that receives a temperature and returns the sublimation
-        enthalpy at that temperature [J/mol], by default None
+        A function that receives temperature and returns the sublimation
+        enthalpy at temperature [J/mol], by default None.
     volume_solid : Callable, optional
-        A function that receives a temperature and returns the molar volume of
-        the solid at that temperature [m³/mol], by default None
+        A function that receives temperature and pressure, and returns the
+        molar volume of the solid at temperature [m³/mol], by default None.
     volume_liquid : Callable, optional
-        A function that receives a temperature and pressure, and returns the
-        molar volume of liquid at that temperature and pressure [m³/mol], by
-        default None
-    volume_gas : Callable, optional
-        A function that receives a temperature and pressure, and returns the
-        molar volume of the gas at that temperature and pressure [m³/mol],
-        by default None
+        A function that receives temperature and pressure, and returns the
+        molar volume of liquid at temperature and pressure [m³/mol], by default
+        None.
     heat_capacity_solid : Callable, optional
-        A function that receives a temperature and pressure, and returns the
-        heat capacity of the solid at that temperature and pressure [J/mol/K],
-        by default None
+        A function that receives temperature and pressure, and returns the
+        heat capacity of the solid at temperature and pressure [J/mol/K], by
+        default None.
     heat_capacity_liquid : Callable, optional
-        A function that receives a temperature and returns the heat capacity of
-        the liquid at that temperature [J/mol/K], by default None
+        A function that receives temperature and pressure, and returns the
+        heat capacity of the liquid at temperature and pressure [J/mol/K], by
+        default None.
     heat_capacity_gas : Callable, optional
-        A function that receives a temperature and returns the heat capacity of
-        the gas at that temperature [J/mol/K], by default None
+        A function that receives temperature and pressure, and returns the
+        ideal gas heat capacity at temperature and pressure [J/mol/K], by
+        default None.
     thermal_conductivity_liquid : Callable, optional
-        A function that receives a temperature and pressure, and returns the
-        thermal conductivity of the liquid at that temperature and pressure
-        [W/m/K], by default None
+        A function that receives temperature and pressure, and returns the
+        thermal conductivity of the liquid at temperature and pressure [W/m/K],
+        by default None.
     thermal_conductivity_gas : Callable, optional
-        A function that receives a temperature and pressure, and returns the
-        thermal conductivity of the gas at that temperature and pressure
-        [W/m/K], by default None
+        A function that receives temperature and pressure, and returns the
+        thermal conductivity of the gas at temperature and pressure [W/m/K], by
+        default None.
     viscosity_liquid : Callable, optional
-        A function that receives a temperature and pressure, and returns the
-        viscosity of thr liquid at that temperature and pressure [Pa*s], by
-        default None
+        A function that receives temperature and pressure, and returns the
+        viscosity of the liquid at temperature and pressure [Pa*s], by default
+        None.
     viscosity_gas : Callable, optional
         A function that receives temperature and pressure, and returns the
-        viscosity of gas at temperature and pressure [Pa*s], by default None
+        viscosity of gas at temperature and pressure [Pa*s], by default None.
+    heat_capacity_solid_dt_integral: Callable, optional
+        A function that receives temperature1, temperature2 and pressure, and
+        returns the integral of the solid heat capacity over temperature1 and
+        temperature2 at pressure, by default None.
+    heat_capacity_liquid_dt_integral: Callable, optional
+        A function that receives temperature1, temperature2 and pressure, and
+        returns the integral of the liquid heat capacity over temperature1 and
+        temperature2 at pressure, by default None.
+    heat_capacity_gas_dt_integral: Callable, optional
+        A function that receives temperature1, temperature2 and pressure, and
+        returns the integral of the gas heat capacity over temperature1 and
+        temperature2 at pressure, by default None.
+    vectorize_functions: bool, optional
+        When True, numpy.vectorize() is applied to the temperature and pressure
+        Substance Callable paramaters on Substance object init, by default
+        False.
 
     Attributes
     ----------
-    name : str, optional
-       Name of the substance, by default None
-    molecular_weight : float, optional
-        The molecular weight of the substance [g/mol], by default None
-    normal_boiling_point : float, optional
-        The normal boiling point of the substance [K], by default None
-    normal_melting_point : float, optional
-        The normal melting point of the substance [K], by default None
-    critical_temperature : float, optional
-        The critical temperature of the substance [K], by default None
-    critical_pressure : float, optional
-        The critical pressure of the substance [Pa], by default None
-    acentric_factor : float, optional
-        The acentric factor of the substance, by default None
-    formation_enthalpy : float, optional
-        Standard state molar enthalpy of formation [J/mol], by default None
-    formation_enthalpy_ig : float, optional
-        Ideal-gas molar enthalpy of formation [J/mol], by default None
-    formation_gibbs_ig : float, optional
-        Ideal-gas molar change of Gibbs energy of formation [J/mol], by default
-        None
+    name : str
+       Name of the substance, by default None.
+    molecular_weight : float
+        The molecular weight of the substance [g/mol], by default None.
+    normal_boiling_point : float
+        The normal boiling point of the substance [K], by default None.
+    normal_melting_point : float
+        The normal melting point of the substance [K], by default None.
+    critical_temperature : float
+        The critical temperature of the substance [K], by default None.
+    critical_pressure : float
+        The critical pressure of the substance [Pa], by default None.
+    acentric_factor : float
+        The acentric factor of the substance, by default None.
+    formation_enthalpy : float
+        Standard state molar enthalpy of formation [J/mol], by default None.
+    formation_enthalpy_ig : float
+        Ideal-gas molar enthalpy of formation [J/mol], by default None.
+    vectorize_functions: bool
+        When True, numpy.vectorize() is applied to the temperature and pressure
+        Substance functions on Substance object init, by default False.
     """
 
     def __init__(
         self,
-        name: str = None,
+        name: str,
         molecular_weight: float = None,
         normal_boiling_point: float = None,
         normal_melting_point: float = None,
         critical_temperature: float = None,
         critical_pressure: float = None,
         acentric_factor: float = None,
         formation_enthalpy: float = None,
         formation_enthalpy_ig: float = None,
-        formation_gibbs_ig: float = None,
         vaporization_enthalpy: Callable = None,
         sublimation_enthalpy: Callable = None,
         volume_solid: Callable = None,
         volume_liquid: Callable = None,
-        volume_gas: Callable = None,
         heat_capacity_solid: Callable = None,
         heat_capacity_liquid: Callable = None,
         heat_capacity_gas: Callable = None,
         thermal_conductivity_liquid: Callable = None,
         thermal_conductivity_gas: Callable = None,
         viscosity_liquid: Callable = None,
         viscosity_gas: Callable = None,
+        heat_capacity_solid_dt_integral: Callable = None,
+        heat_capacity_liquid_dt_integral: Callable = None,
+        heat_capacity_gas_dt_integral: Callable = None,
+        vectorize_functions: bool = False,
     ) -> None:
+        # Symbolic init
+        super().__init__(names=name)
 
         # Pure compound properties:
         self.name = name
         self.molecular_weight = molecular_weight
         self.normal_boiling_point = normal_boiling_point
         self.normal_melting_point = normal_melting_point
         self.critical_temperature = critical_temperature
         self.critical_pressure = critical_pressure
         self.acentric_factor = acentric_factor
         self.formation_enthalpy = formation_enthalpy
         self.formation_enthalpy_ig = formation_enthalpy_ig
-        self.formation_gibbs_ig = formation_gibbs_ig
 
-        # Temperature-dependent properties calculation functions:
-        self._vaporization_enthalpy = np.vectorize(
-            vaporization_enthalpy, signature="()->()"
-        )
-        self._sublimation_enthalpy = np.vectorize(
-            sublimation_enthalpy, signature="()->()"
-        )
-        self._volume_solid = np.vectorize(volume_solid, signature="(),()->()")
-        self._volume_liquid = np.vectorize(
-            volume_liquid, signature="(),()->()"
-        )
-        self._volume_gas = np.vectorize(volume_gas, signature="(),()->()")
-        self._heat_capacity_solid = np.vectorize(
-            heat_capacity_solid, signature="(),()->()"
-        )
-        self._heat_capacity_liquid = np.vectorize(
-            heat_capacity_liquid, signature="(),()->()"
-        )
-        self._heat_capacity_gas = np.vectorize(
-            heat_capacity_gas, signature="(),()->()"
-        )
-        self._thermal_conductivity_liquid = np.vectorize(
-            thermal_conductivity_liquid, signature="(),()->()"
-        )
-        self._thermal_conductivity_gas = np.vectorize(
-            thermal_conductivity_gas, signature="(),()->()"
-        )
-        self._viscosity_liquid = np.vectorize(
-            viscosity_liquid, signature="(),()->()"
-        )
-        self._viscosity_gas = np.vectorize(
-            viscosity_gas, signature="(),()->()"
-        )
+        # Vectorize option
+        self.vectorize_functions = vectorize_functions
+
+        # Temperature and pressure-dependent properties calculation functions:
+        # numpy vectorization is not made by default
+        if self.vectorize_functions:
+            self._vaporization_enthalpy = np.vectorize(
+                vaporization_enthalpy, signature="()->()"
+            )
+
+            self._sublimation_enthalpy = np.vectorize(
+                sublimation_enthalpy, signature="()->()"
+            )
+
+            self._volume_solid = np.vectorize(
+                volume_solid, signature="(),()->()"
+            )
+
+            self._volume_liquid = np.vectorize(
+                volume_liquid, signature="(),()->()"
+            )
+
+            self._heat_capacity_solid = np.vectorize(
+                heat_capacity_solid, signature="(),()->()"
+            )
+
+            self._heat_capacity_liquid = np.vectorize(
+                heat_capacity_liquid, signature="(),()->()"
+            )
+
+            self._heat_capacity_gas = np.vectorize(
+                heat_capacity_gas, signature="(),()->()"
+            )
+
+            self._thermal_conductivity_liquid = np.vectorize(
+                thermal_conductivity_liquid, signature="(),()->()"
+            )
+
+            self._thermal_conductivity_gas = np.vectorize(
+                thermal_conductivity_gas, signature="(),()->()"
+            )
+
+            self._viscosity_liquid = np.vectorize(
+                viscosity_liquid, signature="(),()->()"
+            )
+
+            self._viscosity_gas = np.vectorize(
+                viscosity_gas, signature="(),()->()"
+            )
+
+            self._heat_capacity_solid_dt_integral = np.vectorize(
+                heat_capacity_solid_dt_integral, signature="(),(),()->()"
+            )
+
+            self._heat_capacity_liquid_dt_integral = np.vectorize(
+                heat_capacity_liquid_dt_integral, signature="(),(),()->()"
+            )
+
+            self._heat_capacity_gas_dt_integral = np.vectorize(
+                heat_capacity_gas_dt_integral, signature="(),(),()->()"
+            )
+
+        else:
+            # No numpy vectorization if the user guaranties compatibility with
+            # vectors as arguments.
+            self._vaporization_enthalpy = vaporization_enthalpy
+            self._sublimation_enthalpy = sublimation_enthalpy
+            self._volume_solid = volume_solid
+            self._volume_liquid = volume_liquid
+            self._heat_capacity_solid = heat_capacity_solid
+            self._heat_capacity_liquid = heat_capacity_liquid
+            self._heat_capacity_gas = heat_capacity_gas
+            self._thermal_conductivity_liquid = thermal_conductivity_liquid
+            self._thermal_conductivity_gas = thermal_conductivity_gas
+            self._viscosity_liquid = viscosity_liquid
+            self._viscosity_gas = viscosity_gas
+            self._heat_capacity_solid_dt_integral = (
+                heat_capacity_solid_dt_integral
+            )
+            self._heat_capacity_liquid_dt_integral = (
+                heat_capacity_liquid_dt_integral
+            )
+            self._heat_capacity_gas_dt_integral = heat_capacity_gas_dt_integral
 
     @classmethod
-    def from_thermo_database(cls, identification: str):
+    def from_thermo_database(
+        cls, name: str, thermo_identification: str
+    ) -> "Substance":
         """Substance instance from Bell Caleb's thermo library.
 
-        Method that uses Bell Caleb's Thermo library to construct the
-        Substance object.
+        Method that uses Bell Caleb's Thermo library to construct the Substance
+        object.
 
         Cite:
-
-        Caleb Bell and Contributors (2016-2021). Thermo: Chemical
-        properties component of Chemical Engineering Design
-        Library (ChEDL) https://github.com/CalebBell/thermo.
+        Caleb Bell and Contributors (2016-2021). Thermo: Chemical properties
+        component of Chemical Engineering Design Library (ChEDL)
+        https://github.com/CalebBell/thermo.
 
         Parameters
         ----------
-        identification : string
-            Name or CAS number of the substance
+        name : str
+            Name that will be assigned to the Substance object.
+        thermo_identification : str
+            Name or CAS number of the substance that would be used to search in
+            the Thermo library.
 
         Returns
         -------
         Substance
             Instantiated Substance object from thermo database.
         """
-        corr = ChemicalConstantsPackage.correlations_from_IDs([identification])
-
-        # Temperature functions
-        def vaporization_enthalpy(temperature: float) -> float:
-            enthalpy = corr.EnthalpyVaporizations[0].T_dependent_property(
-                temperature
-            )
-            return enthalpy
-
-        def sublimation_enthalpy(temperature: float) -> float:
-            enthalpy = corr.EnthalpySublimations[0].T_dependent_property(
-                temperature
-            )
-            return enthalpy
-
-        # Temperature and pressure dependent functions
-        def volume_solid(temperature: float, pressure: float) -> float:
-            volume = corr.VolumeSolids[0].T_dependent_property(temperature)
-            return volume
-
-        def volume_liquid(temperature: float, pressure: float) -> float:
-            volume = corr.VolumeLiquids[0].T_dependent_property(temperature)
-            return volume
-
-        def volume_gas(temperature: float, pressure: float) -> float:
-            method = corr.VolumeGases[0].method_P
-            volume = corr.VolumeGases[0].calculate_P(
-                temperature, pressure, method
-            )
-            return volume
-
-        def heat_capacity_solid(temperature: float, pressure: float) -> float:
-            heat_cap = corr.HeatCapacitySolids[0].T_dependent_property(
-                temperature
-            )
-            return heat_cap
-
-        def heat_capacity_liquid(temperature: float, pressure: float) -> float:
-            heat_cap = corr.HeatCapacityLiquids[0].T_dependent_property(
-                temperature
-            )
-            return heat_cap
-
-        def heat_capacity_gas(temperature: float, pressure: float) -> float:
-            heat_cap = corr.HeatCapacityGases[0].T_dependent_property(
-                temperature
-            )
-            return heat_cap
-
-        def thermal_conductivity_liquid(
-            temperature: float, pressure: float
-        ) -> float:
-            thermal_cond = corr.ThermalConductivityLiquids[
-                0
-            ].T_dependent_property(temperature)
-            return thermal_cond
-
-        def thermal_conductivity_gas(
-            temperature: float, pressure: float
-        ) -> float:
-            thermal_cond = corr.ThermalConductivityGases[
-                0
-            ].T_dependent_property(temperature)
-            return thermal_cond
-
-        def viscosity_liquid(temperature: float, pressure: float) -> float:
-            thermal_cond = corr.ViscosityLiquids[0].T_dependent_property(
-                temperature
-            )
-            return thermal_cond
-
-        def viscosity_gas(temperature: float, pressure: float) -> float:
-            thermal_cond = corr.ViscosityGases[0].T_dependent_property(
-                temperature
-            )
-            return thermal_cond
-
-        substance_object = cls(
-            name=corr.constants.names[0],
-            molecular_weight=corr.constants.MWs[0],
-            normal_boiling_point=corr.constants.Tbs[0],
-            normal_melting_point=corr.constants.Tms[0],
-            critical_temperature=corr.constants.Tcs[0],
-            critical_pressure=corr.constants.Pcs[0],
-            acentric_factor=corr.constants.omegas[0],
-            formation_enthalpy=corr.constants.Hf_STPs[0],
-            formation_enthalpy_ig=corr.constants.Hfgs[0],
-            formation_gibbs_ig=corr.constants.Gfgs[0],
-            vaporization_enthalpy=vaporization_enthalpy,
-            sublimation_enthalpy=sublimation_enthalpy,
-            volume_solid=volume_solid,
-            volume_liquid=volume_liquid,
-            volume_gas=volume_gas,
-            heat_capacity_solid=heat_capacity_solid,
-            heat_capacity_liquid=heat_capacity_liquid,
-            heat_capacity_gas=heat_capacity_gas,
-            thermal_conductivity_liquid=thermal_conductivity_liquid,
-            thermal_conductivity_gas=thermal_conductivity_gas,
-            viscosity_liquid=viscosity_liquid,
-            viscosity_gas=viscosity_gas,
-        )
-        return substance_object
+        return thermo_substance_constructor(cls, name, thermo_identification)
 
     @classmethod
     def from_pickle(cls, name_file: str) -> "Substance":
         """Read a dill Substance file and return the Substance object.
 
-        Cite:
-        https://github.com/uqfoundation/dill
-
         Parameters
         ----------
         name_file : str
-            Name of the file.
+            path/to/file.
 
         Returns
         -------
         Substance : Substance
             Substance object.
         """
         with open(name_file, "rb") as f:
             return loads(f.read())
 
     def to_pickle(self, name_file: str) -> __file__:
         """Serialize an substance object with dill library.
 
         This method save an object substance as a file.
 
-        Cite:
-        https://github.com/uqfoundation/dill
-
         Parameters
         ----------
         name_file : str
             Name of file to save the substance object.
 
         Returns
         -------
         _file_
             A binary file with substance predefine object.
         """
         with open(name_file, "wb") as f:
             f.write(dumps(self))
 
-    def vaporization_enthalpy(self, temperature: float) -> float:
+    def vaporization_enthalpy(
+        self, temperature: Union[float, NDArray[np.float64]]
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the vaporization enthalpy at a given temperature.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
 
         Returns
         -------
-        float
-            Vaporization enthalpy in Joule per mol [J/mol]
+        Union[float, NDArray[np.float64]]
+            Vaporization enthalpy. [J/mol]
         """
         return self._vaporization_enthalpy(temperature)
 
-    def sublimation_enthalpy(self, temperature: float) -> float:
+    def sublimation_enthalpy(
+        self, temperature: Union[float, NDArray[np.float64]]
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the sublimation enthalpy at a given temperature.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
 
         Returns
         -------
-        float
-            Sublimation enthalpy in Joule per mol [J/mol]
+        Union[float, NDArray[np.float64]]
+            Sublimation enthalpy. [J/mol]
         """
         return self._sublimation_enthalpy(temperature)
 
-    def fusion_enthalpy(self, temperature: float) -> float:
+    def fusion_enthalpy(
+        self, temperature: Union[float, NDArray[np.float64]]
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the fusion enthalpy at a given temperature.
 
-        Uses the sublimation and vaporization enthalpy functions for the
-        fusion enthalpy calculations at a given temperature, by
-        calculating the sublimation and vaporization enthalpy difference.
+        Uses the sublimation and vaporization enthalpy functions for the fusion
+        enthalpy calculations at a given temperature, by calculating the
+        sublimation and vaporization enthalpy difference.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
 
         Returns
         -------
-        float
-            Fusion enthalpy in Joule per mol [J/mol]
+        Union[float, NDArray[np.float64]]
+            Fusion enthalpy. [J/mol]
         """
         fusion_h = self._sublimation_enthalpy(
             temperature
         ) - self._vaporization_enthalpy(temperature)
         return fusion_h
 
-    def volume_solid(self, temperature: float, pressure: float) -> float:
-        """Return the solid molar volume at a given temperature.
+    def volume_solid(
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
+        """Return the solid molar volume at a given temperature and pressure.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Solid molar volume in cubic meters per mol [m³/mol]
+        Union[float, NDArray[np.float64]]
+            Solid molar volume. [m³/mol]
         """
         return self._volume_solid(temperature, pressure)
 
-    def volume_liquid(self, temperature: float, pressure: float) -> float:
+    def volume_liquid(
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the liquid molar volume at a given temperature and pressure.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
-        pressure : float
-            Pressure in pascal [Pa]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Liquid molar volume in cubic meters per mol [m³/mol]
+        Union[float, NDArray[np.float64]]
+            Liquid molar volume. [m³/mol]
         """
         return self._volume_liquid(temperature, pressure)
 
-    def volume_gas(self, temperature: float, pressure: float) -> float:
-        """Return the gas molar volume at a given temperature and pressure.
-
-        Parameters
-        ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
-        pressure : float
-            Pressure in Pascal [Pa]
-
-        Returns
-        -------
-        float
-            Liquid molar volume in cubic meters per mol [m³/mol]
-        """
-        return self._volume_gas(temperature, pressure)
-
     def heat_capacity_solid(
-        self, temperature: float, pressure: float
-    ) -> float:
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the pure solid heat capacity at a given temperature.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Pure solid heat capacity in Joule per mol per Kelvin [J/mol/K]
+        Union[float, NDArray[np.float64]]
+            Solid heat capacity. [J/mol/K]
         """
         return self._heat_capacity_solid(temperature, pressure)
 
     def heat_capacity_liquid(
-        self, temperature: float, pressure: float
-    ) -> float:
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the pure liquid heat capacity at a given temperature.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Pure liquid heat capacity in Joule per mol per Kelvin
-            [J/mol/K]
+        Union[float, NDArray[np.float64]]
+            Liquid heat capacity. [J/mol/K]
         """
         return self._heat_capacity_liquid(temperature, pressure)
 
-    def heat_capacity_gas(self, temperature: float, pressure: float) -> float:
-        """Return the pure gas heat capacity at a given temperature.
+    def heat_capacity_gas(
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
+        """Return the ideal gas heat capacity at a given temperature.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Pure gas heat capacity in Joule per mol per Kelvin [J/mol/K]
+        Union[float, NDArray[np.float64]]
+            Ideal gas heat capacity. [J/mol/K]
         """
         return self._heat_capacity_gas(temperature, pressure)
 
     def thermal_conductivity_liquid(
-        self, temperature: float, pressure: float
-    ) -> float:
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the liquid thermal conductivity.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
-        pressure : float
-            Pressure in Pascal [Pa]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Liquid thermal conductivity in Watts per meter per Kelvin
-            [W/m/K]
+        Union[float, NDArray[np.float64]]
+            Liquid thermal conductivity. [W/m/K]
         """
         return self._thermal_conductivity_liquid(temperature, pressure)
 
     def thermal_conductivity_gas(
-        self, temperature: float, pressure: float
-    ) -> float:
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the gas thermal conductivity.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
-        pressure : float
-            Pressure in Pascal [Pa]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Gas thermal conductivity in Watts per meter per Kelvin
-            [W/m/K]
+        Union[float, NDArray[np.float64]]
+            Gas thermal conductivity. [W/m/K]
         """
         return self._thermal_conductivity_gas(temperature, pressure)
 
-    def viscosity_liquid(self, temperature: float, pressure: float) -> float:
+    def viscosity_liquid(
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the pure liquid viscosity.
 
         Pure liquid viscosity at a given temperature and pressure.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
-        pressure : float
-            Pressure in Pascal [Pa]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Pure liquid viscosity in [Pa*s]
+        Union[float, NDArray[np.float64]]
+            Liquid viscosity. [Pa s]
         """
         return self._viscosity_liquid(temperature, pressure)
 
-    def viscosity_gas(self, temperature: float, pressure: float) -> float:
+    def viscosity_gas(
+        self,
+        temperature: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         """Return the pure gas viscosity.
 
          Pure gas viscosity at a given temperature and pressure.
 
         Parameters
         ----------
-        temperature : float
-            Temperature in Kelvin degrees [K]
-        pressure : float
-            Pressure in Pascal [Pa]
+        temperature : Union[float, NDArray[np.float64]]
+            Temperature. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Pure gas viscosity in [Pa*s]
+        Union[float, NDArray[np.float64]]
+            Gas viscosity. [Pa s]
         """
         return self._viscosity_gas(temperature, pressure)
 
     def heat_capacity_solid_dt_integral(
-        self, temperature1: float, temperature2: float, pressure: float
-    ) -> float:
+        self,
+        temperature1: Union[float, NDArray[np.float64]],
+        temperature2: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         r"""Return the integral of solid heat capacity.
 
         Calculate the integral of solid heat capacity between temperature1
         and temperature2
 
         .. math::
-            \int_{T_1}^{T_2} {C_{p_{solid}} (T)} \mathrm{d}T
+            \int_{T_1}^{T_2} {C_{p_{solid}} (T, P)} \mathrm{d}T
+
+        | :math:`T_1`: temperature1.
+        | :math:`T_2`: temperature2.
+        | :math:`C_{p_{solid}} (T, P)`: solid heat capacity.
 
         Parameters
         ----------
-        temperature1 : float
-            Lower temperature integral bound in Kelvin degrees [K]
-        temperature2 : float
-            Upper temperature integral bound in Kelvin degrees [K]
+        temperature1 : Union[float, NDArray[np.float64]]
+            Lower temperature integral bound. [K]
+        temperature2 : Union[float, NDArray[np.float64]]
+            Upper temperature integral bound. [K]
+        pressure: Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
+        Union[float, NDArray[np.float64]]
             Integral of solid heat capacity between temperature1 and
-            temperature2 in Joule per mol per Kelvin [J/mol/K]
+            temperature2. [J/mol]
         """
-        integral, err = quad(
-            self.heat_capacity_solid,
-            a=temperature1,
-            b=temperature2,
-            args=(pressure,),
+        integral = self._heat_capacity_solid_dt_integral(
+            temperature1, temperature2, pressure
         )
-
         return integral
 
     def heat_capacity_liquid_dt_integral(
-        self, temperature1: float, temperature2: float, pressure: float
-    ) -> float:
+        self,
+        temperature1: Union[float, NDArray[np.float64]],
+        temperature2: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         r"""Return the integral of liquid heat capacity.
 
         Calculate the definite integral of liquid heat capacity between
         temperature1 and temperature2
 
         .. math::
-            \int_{T_1}^{T_2} {C_{p_{liquid}} (T)} \mathrm{d}T
+            \int_{T_1}^{T_2} {C_{p_{liquid}} (T, P)} \mathrm{d}T
+
+        | :math:`T_1`: temperature1.
+        | :math:`T_2`: temperature2.
+        | :math:`C_{p_{liquid}} (T, P)`: liquid heat capacity.
 
         Parameters
         ----------
-        temperature1 : float
-            Lower temperature integral bound in Kelvin degrees [K]
-        temperature2 : float
-            Upper temperature integral bound in Kelvin degrees [K]
+        temperature1 : Union[float, NDArray[np.float64]]
+            Lower temperature integral bound. [K]
+        temperature2 : Union[float, NDArray[np.float64]]
+            Upper temperature integral bound. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
+        Union[float, NDArray[np.float64]]
             Definite integral of liquid heat capacity between temperature1
-            and temperature2 in Joule per mol per Kelvin [J/mol/K]
+            and temperature2. [J/mol]
         """
-        integral, err = quad(
-            self.heat_capacity_liquid,
-            a=temperature1,
-            b=temperature2,
-            args=(pressure,),
+        integral = self._heat_capacity_liquid_dt_integral(
+            temperature1, temperature2, pressure
         )
-
         return integral
 
     def heat_capacity_gas_dt_integral(
-        self, temperature1: float, temperature2: float, pressure: float
-    ) -> float:
+        self,
+        temperature1: Union[float, NDArray[np.float64]],
+        temperature2: Union[float, NDArray[np.float64]],
+        pressure: Union[float, NDArray[np.float64]],
+    ) -> Union[float, NDArray[np.float64]]:
         r"""Return the integral of gas heat capacity.
 
         Calculate the definite integral of gas heat capacity between
-        temperature1 and temperature2
+        temperature1 and temperature2.
 
         .. math::
-            \int_{T_1}^{T_2} {C_{p_{gas}} (T)} \mathrm{d}T
+            \int_{T_1}^{T_2} {C_{p_{gas}} (T, P)} \mathrm{d}T
+
+        | :math:`T_1`: temperature1.
+        | :math:`T_2`: temperature2.
+        | :math:`C_{p_{gas}} (T, P)`: ideal gas heat capacity.
 
         Parameters
         ----------
-        temperature1 : float
-            Lower temperature integral bound in Kelvin degrees [K]
-        temperature2 : float
-            Upper temperature integral bound in Kelvin degrees [K]
+        temperature1 : Union[float, NDArray[np.float64]]
+            Lower temperature integral bound. [K]
+        temperature2 : Union[float, NDArray[np.float64]]
+            Upper temperature integral bound. [K]
+        pressure : Union[float, NDArray[np.float64]]
+            Pressure. [Pa]
 
         Returns
         -------
-        float
-            Definite integral of gas heat capacity between temperature1
-            and temperature2 in Joule per mol per Kelvin [J/mol/K]
+        Union[float, NDArray[np.float64]]
+            Definite integral of gas heat capacity between temperature1 and
+            temperature2. [J/mol]
         """
-        integral, err = quad(
-            self.heat_capacity_gas,
-            a=temperature1,
-            b=temperature2,
-            args=(pressure,),
+        integral = self._heat_capacity_gas_dt_integral(
+            temperature1, temperature2, pressure
         )
-
         return integral
```

### Comparing `reactord-0.0.1a2/reactord.egg-info/PKG-INFO` & `reactord-0.0.1b1/reactord.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: reactord
-Version: 0.0.1a2
+Version: 0.0.1b1
 Summary: Package for the simulation and design of chemical reactors
 Author-email: "Brandolín, Salvador Eduardo" <salvadorebrandolin@mi.unc.edu.ar>, "Parodi, Adrián" <adrian.parodi@mi.unc.edu.ar>, "Rovezzi, Juan Pablo" <juan.rovezzi@mi.unc.edu.ar>, "Santos, Maricel Del Valle" <maricel.santos@mi.unc.edu.ar>, "Scilipoti, José Antonio" <jscilipoti@unc.edu.ar>
 License: The MIT License
 Project-URL: Homepage, https://github.com/SalvadorBrandolin/reactord
 Keywords: chemical reactor,reactor design,reactor simulation,chemical engineering
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
@@ -32,48 +32,49 @@
 <a href='https://pypi.org/project/reactord/'>
 <img src='https://img.shields.io/pypi/v/reactord'>
 </a>
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)
 ![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)
 [![codecov](https://codecov.io/gh/SalvadorBrandolin/ReactorD/branch/main/graph/badge.svg?token=6E0U0F9AYU)](https://codecov.io/gh/SalvadorBrandolin/ReactorD)
 
-ReactorD (Reactor Design) is a python package whose proposal is to simulate and design reactors for multiple-reaction systems. The intention is to solve the following reactor types in stationary or not-stationary conditions: Plug flow (PFR) and Stirred tank (STR) 
-
-According to requirements, the operation settings can change as follows; 
-
-- Mass Balance:
-	- Homogeneous
-    - Heterogeneous
-    - Continuous
-    - Discontinuous
-    
-- Energy Balance:
-	- Isothermic
-    - Non-isothermic
-    - Adiabatic
-
-- Pressure Balance:
-	- Isobaric
-    - Non-isobaric
-      - Packed bed reactor
-      - Gas phase reaction
-
-
-## Available in version 0.0.1a2
-- Stationary PFR Isothermic - Isobaric Operation
-- Stationary PFR Isothermic - Non-isobaric packed bed reactor Operation
-- Stationary PFR Adiabatic  - Isobaric Operation
-- Stationary PFR Adiabatic  - Non-isobaric packed bed reactor Operation
+ReactorD (Reactor Design) is a `Python` package whose proposal is to simulate 
+and design reactors for multiple-reaction systems. The intention is to solve 
+the following reactor types in stationary or not-stationary conditions: Plug 
+flow (PFR) and Stirred tank (STR) 
+
+## Available in version 0.0.1b1
+- PFR (Border and initial value problems)
+    - Mass Balances
+        - MolarFlow
+    - Energy Balances
+        - Isothermic
+        - Adiabatic
+        - No isothermic (constant U coefficient and refrigerant temperature)
+        - No isothermic (constant U coefficient)
+    - Pressure Balances
+        - Isobaric
+        - Ergun
 
 
 ## Motivation
-Chemical reaction engineering has as its main objective the study and optimization of reactive processes, usually, with a chemical reactor as the protagonist equipment. To design a chemical reactor, it is necessary to consider several physical and chemical phenomena simultaneously, such as the inlet and outlet molar flow of chemical substances, mass transfer, heat transfer, and reaction kinetics. All these contributions to the system's complexity, commonly lead to coupled non-linear algebraic problems, coupled differential equations, or either both coupled algebraic-differential equations that must be solved by numeric algorithms. ReactorD provides an interphase to configure the necessary information for the simulation of the chemical reactors. Also, ReactorD implements the mathematical representations of mass and energy balances of specific reactors for a numerical resolution.
+Chemical reaction engineering has as its main objective the study and 
+optimization of reactive processes, usually, with a chemical reactor as the 
+protagonist equipment. To design a chemical reactor, it is necessary to 
+consider several physical and chemical phenomena simultaneously, such as the 
+inlet and outlet molar flow of chemical substances, mass transfer, heat 
+transfer, and reaction kinetics. All these contributions to the system's 
+complexity, commonly lead to coupled non-linear algebraic problems, coupled 
+differential equations, or either both coupled algebraic-differential 
+equations that must be solved by numeric algorithms. ReactorD provides an 
+interphase to configure the necessary information for the simulation of the 
+chemical reactors. Also, ReactorD implements the mathematical representations 
+of mass and energy balances of specific reactors for a numerical resolution.
 
 ## Requirements
-You need Python 3.7+ to run ReactorD.
+You need Python 3.8+ to run ReactorD.
 
 ## Instalation
 For installing _ReactorD_ you just need to:
 
 ```sh
 pip install reactord
 ```
@@ -85,21 +86,7 @@
 (<a href=adrian.parodi@mi.unc.edu.ar>adrian.parodi@mi.unc.edu.ar</a>)
 Rovezzi, Juan Pablo
 (<a href=juan.rovezzi@mi.unc.edu.ar>juan.rovezzi@mi.unc.edu.ar</a>)
 Santos, Maricel Del Valle
 (<a href=maricel.santos@mi.unc.edu.ar>maricel.santos@mi.unc.edu.ar</a>)
 Scilipoti, José Antonio
 (<a href=jscilipoti@mi.unc.edu.ar>jscilipoti@mi.unc.edu.ar</a>)
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: reactord Version: 0.0.1a2 Summary: Package for the
+Metadata-Version: 2.1 Name: reactord Version: 0.0.1b1 Summary: Package for the
 simulation and design of chemical reactors Author-email: "BrandolÃ­n, Salvador
 Eduardo"
 mi.unc.edu.ar>, "Parodi, AdriÃ¡n"
 parodi@mi.unc.edu.ar>, "Rovezzi, Juan Pablo"
 rovezzi@mi.unc.edu.ar>, "Santos, Maricel Del Valle"
 santos@mi.unc.edu.ar>, "Scilipoti, JosÃ© Antonio"
 unc.edu.ar> License: The MIT License Project-URL: Homepage, https://github.com/
 SalvadorBrandolin/reactord Keywords: chemical reactor,reactor design,reactor
-simulation,chemical engineering Classifier: Development Status :: 2 - Pre-Alpha
+simulation,chemical engineering Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering Description-Content-Type: text/markdown License-File:
 LICENCE # ReactorD ![logo](https://raw.githubusercontent.com/SalvadorBrandolin/
 ReactorD/main/logo.png) [![Binder](https://mybinder.org/badge_logo.svg)](https:
@@ -22,37 +22,33 @@
 69644832889fa9dfcdb974614129be2fda8e4591989fd713a983a21e7fd8d1ad/
 68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4469536f6674436f6d7043692d46414d41462d666664613030]
 [https://img.shields.io/pypi/v/reactord] [![License](https://img.shields.io/
 badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license) !
 [Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg) [![codecov]
 (https://codecov.io/gh/SalvadorBrandolin/ReactorD/branch/main/graph/
 badge.svg?token=6E0U0F9AYU)](https://codecov.io/gh/SalvadorBrandolin/ReactorD)
-ReactorD (Reactor Design) is a python package whose proposal is to simulate and
-design reactors for multiple-reaction systems. The intention is to solve the
-following reactor types in stationary or not-stationary conditions: Plug flow
-(PFR) and Stirred tank (STR) According to requirements, the operation settings
-can change as follows; - Mass Balance: - Homogeneous - Heterogeneous -
-Continuous - Discontinuous - Energy Balance: - Isothermic - Non-isothermic -
-Adiabatic - Pressure Balance: - Isobaric - Non-isobaric - Packed bed reactor -
-Gas phase reaction ## Available in version 0.0.1a2 - Stationary PFR Isothermic
-- Isobaric Operation - Stationary PFR Isothermic - Non-isobaric packed bed
-reactor Operation - Stationary PFR Adiabatic - Isobaric Operation - Stationary
-PFR Adiabatic - Non-isobaric packed bed reactor Operation ## Motivation
-Chemical reaction engineering has as its main objective the study and
-optimization of reactive processes, usually, with a chemical reactor as the
-protagonist equipment. To design a chemical reactor, it is necessary to
-consider several physical and chemical phenomena simultaneously, such as the
-inlet and outlet molar flow of chemical substances, mass transfer, heat
-transfer, and reaction kinetics. All these contributions to the system's
-complexity, commonly lead to coupled non-linear algebraic problems, coupled
-differential equations, or either both coupled algebraic-differential equations
-that must be solved by numeric algorithms. ReactorD provides an interphase to
-configure the necessary information for the simulation of the chemical
-reactors. Also, ReactorD implements the mathematical representations of mass
-and energy balances of specific reactors for a numerical resolution. ##
-Requirements You need Python 3.7+ to run ReactorD. ## Instalation For
-installing _ReactorD_ you just need to: ```sh pip install reactord ``` ##
-Authors BrandolÃ­n, Salvador Eduardo (salvadorebrandolin@mi.unc.edu.ar) Parodi,
-AdriÃ¡n (adrian.parodi@mi.unc.edu.ar) Rovezzi, Juan Pablo
-(juan.rovezzi@mi.unc.edu.ar) Santos, Maricel Del Valle
-(maricel.santos@mi.unc.edu.ar) Scilipoti, JosÃ© Antonio
-(jscilipoti@mi.unc.edu.ar)
+ReactorD (Reactor Design) is a `Python` package whose proposal is to simulate
+and design reactors for multiple-reaction systems. The intention is to solve
+the following reactor types in stationary or not-stationary conditions: Plug
+flow (PFR) and Stirred tank (STR) ## Available in version 0.0.1b1 - PFR (Border
+and initial value problems) - Mass Balances - MolarFlow - Energy Balances -
+Isothermic - Adiabatic - No isothermic (constant U coefficient and refrigerant
+temperature) - No isothermic (constant U coefficient) - Pressure Balances -
+Isobaric - Ergun ## Motivation Chemical reaction engineering has as its main
+objective the study and optimization of reactive processes, usually, with a
+chemical reactor as the protagonist equipment. To design a chemical reactor, it
+is necessary to consider several physical and chemical phenomena
+simultaneously, such as the inlet and outlet molar flow of chemical substances,
+mass transfer, heat transfer, and reaction kinetics. All these contributions to
+the system's complexity, commonly lead to coupled non-linear algebraic
+problems, coupled differential equations, or either both coupled algebraic-
+differential equations that must be solved by numeric algorithms. ReactorD
+provides an interphase to configure the necessary information for the
+simulation of the chemical reactors. Also, ReactorD implements the mathematical
+representations of mass and energy balances of specific reactors for a
+numerical resolution. ## Requirements You need Python 3.8+ to run ReactorD. ##
+Instalation For installing _ReactorD_ you just need to: ```sh pip install
+reactord ``` ## Authors BrandolÃ­n, Salvador Eduardo
+(salvadorebrandolin@mi.unc.edu.ar) Parodi, AdriÃ¡n
+(adrian.parodi@mi.unc.edu.ar) Rovezzi, Juan Pablo (juan.rovezzi@mi.unc.edu.ar)
+Santos, Maricel Del Valle (maricel.santos@mi.unc.edu.ar) Scilipoti, JosÃ©
+Antonio (jscilipoti@mi.unc.edu.ar)
```

