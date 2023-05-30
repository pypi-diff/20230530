# Comparing `tmp/PyCosmo-2.1.0.tar.gz` & `tmp/PyCosmo-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCosmo-2.1.0.tar", last modified: Fri Oct 28 11:08:26 2022, max compression
+gzip compressed data, was "PyCosmo-2.1.1.tar", last modified: Tue May 30 13:00:09 2023, max compression
```

## Comparing `PyCosmo-2.1.0.tar` & `PyCosmo-2.1.1.tar`

### file list

```diff
@@ -1,90 +1,109 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.539135 PyCosmo-2.1.0/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      471 2022-06-03 08:24:13.000000 PyCosmo-2.1.0/AUTHORS.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      728 2022-06-03 08:24:13.000000 PyCosmo-2.1.0/LICENSE
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1810 2022-10-28 11:08:26.539276 PyCosmo-2.1.0/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      808 2022-06-03 08:24:13.000000 PyCosmo-2.1.0/README.rst
--rw-r--r--   0 uweschmitt   (501) staff       (20)      764 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/pyproject.toml
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1429 2022-10-28 11:08:26.539757 PyCosmo-2.1.0/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      603 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/setup.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.514986 PyCosmo-2.1.0/src/
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.525883 PyCosmo-2.1.0/src/PyCosmo/
--rw-r--r--   0 uweschmitt   (501) staff       (20)    13867 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/Background.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.528043 PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3622 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/Fields.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    17516 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/LinearPerturbationBoltzmann.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4129 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/LsodaSolver.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3841 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/ScipySolver.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)      811 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    27585 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/Cosmo.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    18706 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    26965 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9963 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu_rsa.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    28586 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu_wcdm.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    10545 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu_wcdm_rsa.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6522 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_rsa.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    20528 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_wcdm.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7161 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_wcdm_rsa.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    28245 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/LinearPerturbationApprox.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4639 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/LinearPerturbationBase.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6658 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/LinearPerturbationTable.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    18999 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/NonLinearPerturbationHaloFit.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    28624 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/NonLinearPerturbationMead.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6225 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/NonLinearPerturbationTable.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    35035 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/Obs.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    33894 2022-10-24 12:16:44.000000 PyCosmo-2.1.0/src/PyCosmo/Obs_old.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2941 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/PerturbationBase.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7617 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/PerturbationTable.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    14698 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/Projection.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     7658 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/TheoryPredTables.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     8214 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_Cosmics.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5961 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_Recombination.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2907 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_RecombinationClass.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3098 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_RecombinationCosmics.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)    12606 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_Tables.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_Util.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1333 2022-10-28 10:26:23.000000 PyCosmo-2.1.0/src/PyCosmo/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1483 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/_scipy_utils.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2189 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/build.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.533957 PyCosmo-2.1.0/src/PyCosmo/config/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      916 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1567 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_lcdm.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1646 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_lcdm_rsa.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1616 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_mnulcdm.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1666 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_mnulcdm_rsa.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1630 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_mnuwcdm.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1680 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_mnuwcdm_rsa.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1613 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_wcdm.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1663 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/default_wcdm_rsa.ini
--rw-r--r--   0 uweschmitt   (501) staff       (20)    11251 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/config/load_parameters_ini.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3911 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/core_file_handling.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.538974 PyCosmo-2.1.0/src/PyCosmo/cython/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      855 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/__init__.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9558 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/const.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      660 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/constf.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)   967846 2022-10-28 11:07:50.000000 PyCosmo-2.1.0/src/PyCosmo/cython/halo_integral.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     9569 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/halo_integral.pyx
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2210 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/logf.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      172 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/main.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     4693 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/mconf.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2369 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/mtherr.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1605 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/polevl.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1841 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/polevlf.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6173 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/protos.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)    15940 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/sici.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)       72 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/sici.h
--rw-r--r--   0 uweschmitt   (501) staff       (20)    15914 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/sici32.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5715 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/sicif.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5206 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/cython/sinf.c
--rw-r--r--   0 uweschmitt   (501) staff       (20)      378 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/disable_multithreading.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     3977 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/ini_handling.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6026 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/model_config.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2099 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/optimize_nq.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)      960 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/patches.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5025 2022-10-28 10:25:19.000000 PyCosmo-2.1.0/src/PyCosmo/predefined_k_grids.py
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2022-10-28 11:08:26.526916 PyCosmo-2.1.0/src/PyCosmo.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)     1810 2022-10-28 11:08:26.000000 PyCosmo-2.1.0/src/PyCosmo.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)     2586 2022-10-28 11:08:26.000000 PyCosmo-2.1.0/src/PyCosmo.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2022-10-28 11:08:26.000000 PyCosmo-2.1.0/src/PyCosmo.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2022-10-24 11:55:57.000000 PyCosmo-2.1.0/src/PyCosmo.egg-info/not-zip-safe
--rw-r--r--   0 uweschmitt   (501) staff       (20)      270 2022-10-28 11:08:26.000000 PyCosmo-2.1.0/src/PyCosmo.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        8 2022-10-28 11:08:26.000000 PyCosmo-2.1.0/src/PyCosmo.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.856346 PyCosmo-2.1.1/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      471 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/AUTHORS.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      728 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/LICENSE
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1810 2023-05-30 13:00:09.856440 PyCosmo-2.1.1/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      808 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/README.rst
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      774 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/pyproject.toml
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1468 2023-05-30 13:00:09.856819 PyCosmo-2.1.1/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      601 2023-05-30 12:59:31.000000 PyCosmo-2.1.1/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.835255 PyCosmo-2.1.1/src/
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.844056 PyCosmo-2.1.1/src/PyCosmo/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    14017 2023-05-23 14:23:55.000000 PyCosmo-2.1.1/src/PyCosmo/Background.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.846597 PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3622 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/Fields.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    20738 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/LinearPerturbationBoltzmann.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4023 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/LsodaSolver.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10035 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/ScipySolver.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      811 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    28714 2023-05-09 12:37:21.000000 PyCosmo-2.1.1/src/PyCosmo/Cosmo.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    18908 2023-05-23 14:40:50.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    26965 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10064 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu_rsa.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    28586 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu_wcdm.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    10655 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu_wcdm_rsa.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6631 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_rsa.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    20528 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_wcdm.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7270 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_wcdm_rsa.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    28248 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/src/PyCosmo/LinearPerturbationApprox.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4639 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/LinearPerturbationBase.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6658 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/LinearPerturbationTable.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    18899 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/NonLinearPerturbationHaloFit.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    28789 2023-05-05 15:41:07.000000 PyCosmo-2.1.1/src/PyCosmo/NonLinearPerturbationMead.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6225 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/NonLinearPerturbationTable.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    35417 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/src/PyCosmo/Obs.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2949 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/src/PyCosmo/PerturbationBase.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7561 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/PerturbationTable.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    14680 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/Projection.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7658 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/TheoryPredTables.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     8214 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_Cosmics.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5961 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_Recombination.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2907 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_RecombinationClass.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3098 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_RecombinationCosmics.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    12606 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_Tables.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1683 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_Util.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1333 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1483 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/_scipy_utils.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2189 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/build.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.848290 PyCosmo-2.1.1/src/PyCosmo/config/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      916 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1586 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_lcdm.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1665 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_lcdm_rsa.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1635 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_mnulcdm.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1685 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_mnulcdm_rsa.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1649 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_mnuwcdm.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1699 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_mnuwcdm_rsa.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1632 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_wcdm.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1682 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/default_wcdm_rsa.ini
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    11420 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/config/load_parameters_ini.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4087 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/core_file_handling.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.852445 PyCosmo-2.1.1/src/PyCosmo/cython/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      855 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/__init__.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9558 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/const.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      660 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/constf.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)   984884 2023-05-09 14:37:59.000000 PyCosmo-2.1.1/src/PyCosmo/cython/halo_integral.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     9569 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/halo_integral.pyx
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2210 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/logf.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      172 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/main.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4693 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/mconf.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2369 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/mtherr.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1605 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/polevl.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1841 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/polevlf.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6173 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/protos.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    15940 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/sici.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       72 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/sici.h
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    15914 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/sici32.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5715 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/sicif.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5206 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/cython/sinf.c
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      378 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/disable_multithreading.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3977 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/ini_handling.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6026 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/model_config.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2099 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/optimize_nq.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      960 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/patches.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5025 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/src/PyCosmo/predefined_k_grids.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.845165 PyCosmo-2.1.1/src/PyCosmo.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1810 2023-05-30 13:00:09.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3119 2023-05-30 13:00:09.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-05-30 13:00:09.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       63 2023-05-30 13:00:09.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/entry_points.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2022-10-24 11:55:57.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/not-zip-safe
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      265 2023-05-30 13:00:09.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        8 2023-05-30 13:00:09.000000 PyCosmo-2.1.1/src/PyCosmo.egg-info/top_level.txt
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-05-30 13:00:09.856187 PyCosmo-2.1.1/tests/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    13792 2023-05-23 14:38:26.000000 PyCosmo-2.1.1/tests/test_background.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    23705 2023-05-30 09:58:32.000000 PyCosmo-2.1.1/tests/test_boltzmann_solver.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6837 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/tests/test_class.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1778 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_core_files_imports.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1574 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_cosmo.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1845 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/tests/test_cython_extensions.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1267 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_ini_handling.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     7500 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_linear_perturbation_approx.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     5287 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_massive_neutrinos.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     4508 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_nonlinear_perturbation_halofit.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6305 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_nonlinear_perturbation_mead.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)    24028 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/tests/test_obs.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2375 2023-05-03 10:35:11.000000 PyCosmo-2.1.1/tests/test_perturbation_table.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      978 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_pickling.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     3563 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_pycosmo.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      432 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_recombination.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     2256 2023-05-30 09:58:54.000000 PyCosmo-2.1.1/tests/test_scipy_solver.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     1415 2023-05-03 10:30:43.000000 PyCosmo-2.1.1/tests/test_util.py
```

### Comparing `PyCosmo-2.1.0/LICENSE` & `PyCosmo-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/PKG-INFO` & `PyCosmo-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCosmo
-Version: 2.1.0
+Version: 2.1.1
 Summary: A multi-purpose cosmology calculation tool
 Author: Uwe Schmitt et al
 Author-email: uwe.schmitt@id.ethz.ch
 License: GPLv3
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/PyCosmo
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `PyCosmo-2.1.0/README.rst` & `PyCosmo-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/pyproject.toml` & `PyCosmo-2.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,22 @@
 testpaths = ["tests"]
 filterwarnings = ["ignore:invalid"]
 
 [tool.tox]
 legacy_tox_ini = '''
 [tox]
 isolated_build = true
-envlist = py38,py39,py10
+envlist = py39,py310,py311
+package = sdist
 setenv =
     PIP_EXTRA_INDEX_URL=https://cosmo-pypi.phys.ethz.ch/simple
     HTTP_PROXY=http://proxy.ethz.ch:3128
     HTTPS_PROXY=http://proxy.ethz.ch:3128
 
 [testenv]
 skip_install = false
 passenv = *
+allowlist_externals = pytest
 extras = dev
-allowlist_exernals = pytest
 commands =
-    pytest -x -v -ra --color=yes --runslow
+    pytest --runslow -v -ra tests
 '''
```

### Comparing `PyCosmo-2.1.0/setup.cfg` & `PyCosmo-2.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyCosmo
-version = 2.1.0
+version = 2.1.1
 license = GPLv3
 description = A multi-purpose cosmology calculation tool
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 author = Uwe Schmitt et al
 author_email = uwe.schmitt@id.ethz.ch
 classifiers = 
@@ -22,21 +22,21 @@
 	Topic :: Scientific/Engineering :: Astronomy
 project_urls = 
 	Source = https://cosmo-docs.phys.ethz.ch/PyCosmo
 
 [options]
 install_requires = 
 	numpy
-	scipy>=0.14
 	recfast4py>=0.2.3
 	dill
 	matplotlib
-	numba
-	sympy2c>=2
+	numba>=0.57.0rc1
+	sympy2c>=2.2.2
 	numexpr
+	scipy
 packages = find:
 package_dir = 
 	=src
 zip_safe = False
 python_requires = >=3.8
 
 [options.packages.find]
@@ -45,27 +45,33 @@
 [options.package_data]
 * = 
 	*.pyx
 	*.c
 	*.h
 	config/*.ini
 
+[options.entry_points]
+console_scripts = 
+	recompile = PyCosmo:Cosmo.recompile_from_cli
+
 [options.extras_require]
 dev = 
+	Cython
 	twine
-	pytest
+	pytest<7.2.0
 	pytest-cov
 	pytest-regtest
 	tox
 	flake8
-	black @ git+https://github.com/psf/black   # binary wheels are broken on some machines
+	black
 	isort
 	sphinx
 	sphinx-pynpoint-theme
 	myst-parser
+	memray
 docs = 
 	sphinx
 	sphinx-pynpoint-theme
 	myst-parser
 
 [egg_info]
 tag_build =
```

### Comparing `PyCosmo-2.1.0/setup.py` & `PyCosmo-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
-
-from setuptools import Extension, setup
-from Cython.Build import cythonize
-
 import numpy
+from Cython.Build import cythonize
+from setuptools import Extension, setup
 
 files = [
     "const.c",
     "main.c",
     "halo_integral.c",
     "polevl.c",
     "sici.c",
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/Background.py` & `PyCosmo-2.1.1/src/PyCosmo/Background.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     if a is None:
         return getattr(wrapper, function)()
     elif isinstance(a, (float, int)):
         return getattr(wrapper, function)(a)
     elif isinstance(a, list):
         a = np.array(a)
     assert isinstance(a, np.ndarray)
-    a = a.astype(float)
-    return getattr(wrapper, function)(a)
+    return getattr(wrapper, function)(a.astype(float))
 
 
 class Background(object):
     """
     The background calculations are based on a
     Friedmann-Robertson-Walker model for which the evolution is governed by
     the Friedmann equation.
@@ -76,20 +75,19 @@
         """
         self._cosmo.reset_wrapper_globals()
         return _call(self._wrapper, "H", a)
 
     _hubble = H
 
     def _H2_H02_a(self, a=1.0):
-        return (
-            self._H2_H02_Omegar_a(a=a)
-            + self._H2_H02_Omegam_a(a=a)
-            + self._H2_H02_Omegak_a(a=a)
-            + self._H2_H02_Omegal_a(a=a)
-        )
+        result = self._H2_H02_Omegar_a(a=a)
+        result += self._H2_H02_Omegam_a(a=a)
+        result += self._H2_H02_Omegak_a(a=a)
+        result += self._H2_H02_Omegal_a(a=a)
+        return result
 
     def _H2_H02_Omegar_a(self, a=1.0):
         return self._params.omega_r / a**4
 
     def _H2_H02_Omegam_a(self, a=1.0):
         self._cosmo.reset_wrapper_globals()
         return (
@@ -290,15 +288,20 @@
 
         .. code-block:: python
 
             cosmo.background.tau(a)
         """
         a = np.atleast_1d(a)
         return np.array(
-            [integrate.quadrature(self._tau_intgd, np.log(aa), 0.0)[0] for aa in a]
+            [
+                integrate.quadrature(
+                    self._tau_intgd, np.log(aa), 0.0, rtol=1e-6, maxiter=100
+                )[0]
+                for aa in a
+            ]
         )
 
     def _tau_intgd(self, lna):
         a = np.exp(lna)
         return -self.taudot(a=a) / (a * self.H(a=a) / self._params.H0 / self._params.rh)
 
     def tau_b(self, a=1.0):
@@ -431,15 +434,17 @@
 
     def _omega_l_a(self, a=1.0):
         """
         Calculates the dark energy density for a given scale factor
         input: a - scale factor [1]
         output: [1]
         """
-        return self._H2_H02_Omegal_a(a=a) / self._H2_H02_a(a=a)
+        result = self._H2_H02_Omegal_a(a=a)
+        result /= self._H2_H02_a(a=a)
+        return result
 
     def _omega_nu_m_a(self, a=1.0):
         """
         Calculates the massive neutrinos density for a given scale factor
         input: a - scale factor [1]
         output: [1]
         """
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/Fields.py` & `PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/Fields.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/LinearPerturbationBoltzmann.py` & `PyCosmo-2.1.1/src/PyCosmo/NonLinearPerturbationHaloFit.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,493 +10,505 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with this
 # program.  If not, see <http://www.gnu.org/licenses/>.
 
-import itertools
-import warnings
-from functools import lru_cache
-
+import numexpr as ne
 import numpy as np
+import scipy
 
-from ..LinearPerturbationBase import LinearPerturbationBase
-from .Fields import Fields
-from .LsodaSolver import LsodaSolver
-
+from PyCosmo.PerturbationBase import NonLinearPerturbationBase
 
-# use decorator to print messages only once per model:
-@lru_cache(maxsize=1)
-def print_new_traces(cache_file):
-    print()
-    print("new traces detected! you might want to run")
-    print("recompile {}".format(cache_file))
-    print()
 
+class NonLinearPerturbationHaloFit(NonLinearPerturbationBase):
 
-class LinearPerturbationBoltzmann(LinearPerturbationBase):
     """
-    Class for computing linear perturbations by solving the Einstein-Boltzmann ODE
-    system.
-
-     The Boltzmann solver is selected using the *set function*:
-
-        .. code-block:: python
-
-            cosmo.set(pk_type = "boltz")
+    The class computes the non-linear matter power spectrum, :math:`P_{nl}(k)`,
+    with a choice of analytic fitting funtions.
 
+    .. Warning ::
+        NonLinearPerturbationHalofit not supported by the Boltzmann solver yet.
+        Calling any function from this module while using the Boltzmann solver
+        (pk_type = 'boltz') will return
+        **AttributeError: 'NoneType' object has no attribute 'function'**
     """
 
-    def __init__(self, cosmology):
-        self._cosmo = cosmology
-        self._params = cosmology.params
-        self._background = cosmology.background
-        self._solver = LsodaSolver(
-            True,
-            self._params.boltzmann_rtol,
-            self._params.boltzmann_atol,
-            self._params.boltzmann_max_bdf_order,
-            self._params.boltzmann_max_iter,
-            self._cosmo,
-            self._params.fast_solver,
-        )
-        self._wrapper = self._background._wrapper
-        self._background = cosmology.background
-        self._enrich_params()
-
-    def _enrich_params(self):
-        if self._params.pk_norm_type == "A_s":
-            self._params.As_norm = self._params.pk_norm
-        else:
-            self._params.As_norm = None
+    def __init__(self, cosmo):
+        self._params = cosmo.params
+        self._background = cosmo.background
+        self._lin_pert = cosmo.lin_pert
+
+    def k_nl(self, a):
+        r"""Computes the non-linear wave number :math:`k_{nl}` as a function of the
+        scale factor a.
 
-    def _setup_norm(self):
-        if self._params.As_norm is None and self._params.pk_norm_type == "sigma8":
-            self._params.sigma8 = self._params.pk_norm
-            self._params.As_norm = 2.0e-9  # arbitrary temporary value
-            sigma8_temp = self.sigma8()
-            self._params.As_norm = (
-                self._params.As_norm * (self._params.sigma8 / sigma8_temp) ** 2
-            )
+        :param a: scale factor [1]
+        :return: k_nl: non-linear wave number [:math:`\mathrm{Mpc}^{-1}`]
+        """
+        logk_ran = [-3.0, 2.0]
+        k = np.logspace(logk_ran[0], logk_ran[1], num=1000)
+        aa = np.atleast_1d(a)
+        k_nl = np.zeros(len(aa))
+        for i in range(len(aa)):
+            # Delta^2=k ** 3*P(k)/(2 pi ** 2)
+            del2 = self._lin_pert.powerspec_a_k(aa[i], k)[0] * k**3 / 2.0 / np.pi**2
+            # k_nl defined such that Delta^2(k_nl)=1
+            k_nl[i] = np.interp(1.0, del2, k)
+            if k_nl[i] < 10 ** logk_ran[0] or k_nl[i] > 10 ** logk_ran[1]:
+                print("k_nl: warning: k_nl outside of search k range")
+        return k_nl
 
     def max_redshift(self, k):
         """computes max redshift for which this model is applicable.
-        uses the implemented initial conditions to determine this.
 
-        :param k: wavenumber k [:math:`h Mpc^{-1}`]
+        :param k: wavenumber k, might be needed for some underlying linear perturbation
+                  models.  [:math:`h Mpc^{-1}`]
         :returns: redshift
         """
-        return 1 / (self.min_a(k) + 1.0)
+        return np.array([5.0]).repeat(len(k))
 
     def min_a(self, k):
-        return np.array([self._solver.initial_conditions(ki)[0] for ki in k])
+        return 1 / (1 + self.max_redshift(k))
 
     def powerspec_a_k(self, a=1.0, k=0.1, diag_only=False):
         """
-        Returns the linear total matter power spectrum computed from the Boltzmann
-        solver, this includes cold dark matter, baryons and massive neutrinos for an
-        array of a and k values.
-
-        :param a: scale factor [1] (default:a=1)
-        :param k: wavenumber used to compute the power spectrum
-                  (default:k=1 Mpc^1) [Mpc^-1]
-        :param diag_only: if set to True: compute powerspectrum for pairs
-                          :math:`a_i, k_i`, else consider all combinations
-                          :math:`a_i, k_j`
-
-        .. Warning ::
-            If pk_norm_type = 'A_s' this will compute the total matter power spectrum
-            following the general relativistic treatment (using delta_m_tot). If
-            pk_norm_type = 'deltah' the Poisson equation will be assumed and the
-            evolution will be split in growth factor and transfer function. We recommend
-            the use of A_s or sigma8 normalizations.
+        Returns the nonlinear matter power spectrum using a choice of fitting functions.
+        Currently both the *Halofit* fitting function and its revision by
+        `Takahashi et al., 2012 <https://arxiv.org/abs/1208.2701>`_ are supported.
+        Those can be selected using the *set function*:
 
-        :return: P(a,k): total matter power spectrum [:math:`Mpc^3`]
-        """
-        a = np.atleast_1d(a)
-        k = np.atleast_1d(k)
+        .. code-block:: python
 
-        min_a = self.min_a(k)
+            cosmo.set(pk_nonlin_type = option)
 
-        if diag_only:
-            assert len(a) == len(k)
-            if any(ai < miai for (ai, miai) in zip(a, min_a)):
-                warnings.warn(
-                    f"some a values are below a={min_a:e} resp log_a={np.log(min_a):e}"
-                    " for given k. invalid a values will be removed."
-                )
-            k = np.array([ki for (ki, ai, miai) in zip(k, a, min_a) if ai >= miai])
+        where *option* can be one the following keywords:
 
-        else:
-            min_a = np.max(min_a)
-            if any(a < min_a):
-                warnings.warn(
-                    f"some a values are below a={min_a:e} resp log_a={np.log(min_a):e}"
-                    " for given k. invalid a values will be removed."
-                )
+        - ``halofit`` (default) for
+          `Smith et al., 2003, MNRAS, 341, 1311 <https://arxiv.org/abs/astro-ph/0207664>`_
+        - ``rev_halofit`` for revision by
+          `Takahashi et al., 2012, ApJ, 761, 152 <https://arxiv.org/abs/1208.2701>`_
 
-            # we need log to be compliant with the grid used internally
-            a = a[np.log(a) > np.log(min_a)]
+        After selecting the fitting function, the non-linear matter power spectrum,
+        :math:`P_{nl}(k)`, can be computed as follows:
 
-        if self._params.pk_norm_type == "deltah":
-            warnings.warn(
-                (
-                    "We discourage the use of deltah normalization with the Boltzmann"
-                    " solver!"
-                ),
-                UserWarning,
-            )
-            T_k = self.transfer_k(k=k)
-            growth = self.growth_a(a, k=1)
+        .. code-block:: python
 
-            # using equation in section 2.4 of notes
-            norm = (
-                2.0
-                * np.pi ** 2
-                * self._params.pk_norm ** 2
-                * (self._params.c / self._params.H0) ** (3.0 + self._params.n)
-            )
+            cosmo.nonlin_pert.powerspec_a_k(a,k)
 
-            if diag_only:
-                pk = norm * growth ** 2 * k ** self._params.n * T_k ** 2
-            else:
-                # pk = norm * np.outer(growth.T ** 2, k ** self._params.n * T_k ** 2).T
-                pk = (
-                    norm * growth ** 2 * (k ** self._params.n * T_k ** 2).reshape(-1, 1)
-                )
+        :param a: scale factor [1]
+        :param k: wavenumber :math:`[Mpc^{-1}]`
+        :return: Nonlinear matter power spectrum, :math:`P_{nl}(k)`, in :math:`[Mpc^3]`.
+        """
 
-        if (self._params.pk_norm_type == "A_s") or (
-            self._params.pk_norm_type == "sigma8"
-        ):
-            self._setup_norm()  # renormalization, links sigma8 and A_s
-            pk = self._a_s_powerspec(a, k, diag_only)
-            if diag_only:
-                return pk.flatten()
-
-        return pk
-
-    def _a_s_powerspec(self, a, k, diag_only):
-        norm = (
-            2.0
-            * np.pi ** 2
-            * self._params.As_norm
-            / self._params.k_pivot ** (self._params.n - 1)
+        if self._params.pk_nonlin_type in ("halofit", "rev_halofit"):
+            return self._powerspec_nonlin_halofit_a_k(
+                a, k, self._params.pk_nonlin_type, diag_only
+            )
+        raise NotImplementedError(
+            "{} not implemented yet".format(self._params.pk_nonlin_type)
         )
 
-        kk = k / self._params.h
-        src_m = np.zeros((len(a), len(k)))
-
-        src_m = []
-
-        if self._cosmo._pool is None:
-            if diag_only:
-                for ai, ki in zip(a, kk):
-                    src_m.append(src_m_column_j((self, ai, ki)))
-            else:
-                for ki in kk:
-                    src_m.append(src_m_column_j((self, a, ki)))
-        else:
-            kk = np.array(kk)
-            perm = np.argsort(kk)
-            kk = kk[perm]
-            src_m = [None] * len(kk)
-            if diag_only:
-                args = [(self, ai, ki) for ai, ki in zip(a, kk)]
-            else:
-                args = [(self, a, ki) for ki in kk]
-
-            src_m_cols = list(self._cosmo._pool.map(src_m_column_j, args))
-            for i, pi in enumerate(perm):
-                src_m[pi] = src_m_cols[i]
-
-        src_m = np.vstack(src_m).T
-        return norm * src_m.T ** 2 * k[:, None] ** (self._params.n - 4.0)
-
-    def powerspec_cb_a_k(self, a=1.0, k=0.1, diag_only=False):
+    def _interp_k_sig(self, a):
+        """Creates an interpolant to the k_sig-redshift relation in order to speed up
+        the calculation of the nonlinear matter power spectrum.
+        : param a: scale factor [1]
+        : return: nonlinear scale k_sig(a) needed to compute nonlinear matter
+                  power spectrum [:math:`Mpc^{-1}`]
         """
-        Returns the linear matter power spectrum of cold dark matter and baryons
-        computed from the Boltzmann solver for an array of a and k values.
 
+        a = np.atleast_1d(a)
 
-        :param a: scale factor [1] (default:a=1)
-        :param k: wavenumber used to compute the power spectrum
-                  (default:k=1 :math:`Mpc^{-1}`) [:math:`Mpc^{-1}`]
-        :param diag_only: if set to True: compute powerspectrum for pairs
-                        :math:`a_i, k_i`, else consider all combinations
-                        :math:`a_i, k_j`
+        if not hasattr(self, "halofit_params_interp"):
+            # restrict to valid a values for approximate lin pert models:
 
-        :return: P_cb(a,k): power spectrum of CDM+baryons [:math:`Mpc^3`]
-        """
-        a = np.atleast_1d(a)
-        k = np.atleast_1d(k)
-        if diag_only:
-            assert len(a) == len(k)
+            # Need to precompute ksig with a fine k grid for each input scale
+            # factor a
+            k_temp = np.logspace(-4, 4, 1000)
+            a_limit = np.max(self.min_a(k_temp))
+            a_temp = np.logspace(np.log10(a_limit), 0, 1000)
+
+            pklin_temp = self._lin_pert.powerspec_a_k(a=a_temp, k=k_temp)
+            Dlin_temp = self._pk_to_D(
+                pklin_temp, np.reshape(k_temp, (k_temp.shape[0], 1))
+            )
 
-        if self._params.pk_norm_type == "deltah":
-            raise ValueError("powerspec_cb_a_k is not supported for deltah normization")
+            k_sig_interp = np.zeros_like(a_temp)
+            np3_interp = np.zeros_like(a_temp)
+            C_interp = np.zeros_like(a_temp)
+            for i, ai in enumerate(a_temp):
+                k_sig_interp[i], np3_interp[i], C_interp[i] = self._k_sig(
+                    Dlin_temp[:, i], ai, k_temp
+                )
 
-        self._setup_norm()  # renormalization, links sigma8 and A_s
+            self.halofit_params_interp = (a_temp, k_sig_interp, np3_interp, C_interp)
 
-        norm = (
-            2.0
-            * np.pi ** 2
-            * self._params.pk_norm
-            / self._params.k_pivot ** (self._params.n - 1)
+        k_sig = np.interp(
+            a,
+            self.halofit_params_interp[0],
+            self.halofit_params_interp[1],
+            left=np.nan,
+            right=np.nan,
+        )
+        np3 = np.interp(
+            a,
+            self.halofit_params_interp[0],
+            self.halofit_params_interp[2],
+            left=np.nan,
+            right=np.nan,
+        )
+        C = np.interp(
+            a,
+            self.halofit_params_interp[0],
+            self.halofit_params_interp[3],
+            left=np.nan,
+            right=np.nan,
         )
 
-        tk = np.zeros((len(a), len(k)))
-        kk = k / self._params.h
-        for j, onek in enumerate(kk):
-            grid, y, meta, keep_lna0 = self._compute_fields(onek, grid=np.log(a))
-            delta = y[:, 1]
-            theta = y[:, 2] * onek
-            delta_b = y[:, 3]
-            theta_b = y[:, 4] * onek
-            H = self._background.H(a) / (self._params.H0 * self._params.rh)
-            delta_m_tot = self._params.omega_dm * delta + self._params.omega_b * delta_b
-            theta_m_tot = self._params.omega_dm * theta + self._params.omega_b * theta_b
-
-            tk[:, j] = (
-                delta_m_tot + (3 * a * H / onek ** 2) * theta_m_tot
-            ) / self._params.omega_m
+        return k_sig, np3, C
 
-        pk = norm * tk.T ** 2 * k[:, None] ** (self._params.n - 4.0)
+    def _powerspec_nonlin_halofit_a_k(self, a, k, model, diag_only):
+        """Returns the halofit nonlinear matter power spectrum per k as defined in
+        Smith et al., 2003, MNRAS, 341, 1311."""
 
-        if diag_only:
-            return np.diag(pk)
+        a = np.atleast_1d(a)
+        k = np.atleast_1d(k)
+        lenk = k.shape[0]
+        lena = a.shape[0]
 
-        return pk
+        if diag_only:
+            assert lenk == lena
+            pklin_temp = self._lin_pert.powerspec_a_k(a=a, k=k, diag_only=True)
+            Dlin_temp = self._pk_to_D(pklin_temp, k)
+            k_sig, np3, C = self._interp_k_sig(a)
+            D_halofit = self._D_nonlin_halofit(Dlin_temp, k, k_sig, np3, C, a, model)
+            pk_halofit = self._D_to_pk(D_halofit, k)
+            return pk_halofit
+
+        # TODO Need to decide how the nonlinear power spectrum should be
+        # computed
+
+        pklin_temp = self._lin_pert.powerspec_a_k(a=a, k=k)
+        Dlin_temp = self._pk_to_D(pklin_temp, k[:, None])
+        k_sig, np3, C = self._interp_k_sig(a)
+        k_arr = np.tile(k, lena)
+        k_arr = k_arr.reshape((-1, lenk)).T
+        D_halofit = self._D_nonlin_halofit(Dlin_temp, k_arr, k_sig, np3, C, a, model)
 
-    def growth_a(self, a=1.0, k=None):
-        """
-        Returns the linear growth factor computed from the Boltzmann solver at a given k
-        value.
+        pk_halofit = self._D_to_pk(D_halofit, np.reshape(k, (lenk, 1)))
 
-        :param a: scale factor [1]
-        :param k: wavenumber used to compute the growth factor
-                  (default:k=1 :math:`Mpc^{-1}`) [:math:`Mpc^{-1}`]
+        if diag_only:
+            return np.diag(pk_halofit)
+        return pk_halofit
 
-        :return: D(a): growth factor normalised to 1 at a=1 [1]
-        """
-        assert (
-            k is not None
-        ), "growth factor of Einstein-Boltzmann model requires a k value"
-        # TODO: add option where D is normalised to a in matter dominated era
-        grid = np.log(np.atleast_1d(a))
-        if grid[-1] != 0.0:
-            grid = np.append(grid, [0.0])
-
-        grid, y, meta, keep_lna0 = self._compute_fields(k, grid=grid)
-        delta = y[:, 1]
-        growth = delta / delta[-1]
-
-        # if a is a scalar, return a scalar
-        if np.isscalar(a):
-            return growth[0]
-        # if a=1 is contained in a, return all values
-        elif a[-1] == 1.0:
-            return growth
-        # remove the first value, since we added a=1
+    def _pk_to_D(self, pk, k):
+        """Returns the matter power spectrum per unit lnk from an
+        input matter power spectrum per unit k."""
+
+        return k**3 * pk / (2 * np.pi**2)
+
+    def _D_to_pk(self, D, k):
+        """Returns the matter power spectrum per unit k from an
+        input matter power spectrum per unit lnk."""
+
+        return (2 * np.pi**2) * D / k**3
+
+    def _k_sig(self, Dlin, a, k):
+        """Computes the scale k_sig which satisfies sig^2(1/ksig) = 1 where
+        sig^2(R) = int dlnk Dlin Wgauss(kR) ** 2 as defined in Eq. 54 of
+        Smith et al., 2003, MNRAS, 341, 1311"""
+
+        if a > 0.3:
+            if self._params.pk_norm >= 0.65 and self._params.pk_norm <= 1.2:
+                logkmin = -1
+                logkmax = 2
+                nk = 300
+            elif self._params.pk_norm < 0.65:
+                logkmin = -1
+                logkmax = 6
+                nk = 200
+            else:
+                logkmin = -2
+                logkmax = 4
+                nk = 110
+        # 2nd case: redshift larger than 2.3
         else:
-            return growth[:-1]
-
-    def _transfer_k(self, args):
-        try:
-            i, k = args
-            kk = np.atleast_1d(k) / self._params.h
-            transfer = np.empty_like(kk)
-            for index, onek in enumerate(kk):
-                grid, y, meta, keep_lna0 = self._compute_fields(
-                    onek, [0], keep_lna0=True
-                )
-                Phi = y[:, 0]
-                transfer[index] = Phi[-1] / Phi[0]
-
-            if np.isscalar(k):
-                return transfer[0]
+            # Redshift smaller than five
+            if a > 0.166:
+                if self._params.pk_norm >= 0.6:
+                    logkmin = -1.0
+                    logkmax = 4
+                    nk = 600
+                else:
+                    logkmin = 0.0
+                    logkmax = 7
+                    nk = 1000
+            elif a <= 0.166 and a > 0.125:
+                logkmin = -1
+                logkmax = 7
+                nk = 600
             else:
-                return transfer
-        except Exception:
-            import traceback
+                logkmin = -1
+                logkmax = 7
+                nk = 200
 
-            traceback.print_exc()
-            raise
+        kseek = np.logspace(logkmin, logkmax, nk)
 
-    def transfer_k(self, k):
-        """
-        Computes the linear matter transfer function using the Boltzmann solver
-        assuming the Poisson equation.
+        sig2gauss = np.trapz(
+            np.exp(-np.outer(1 / kseek, k) ** 2) * Dlin / k, x=k, axis=1
+        )
 
-        :param k:  wavenumber :math:`[ Mpc^{-1} ]`
+        ksig = np.interp(1.0, sig2gauss, kseek)
 
-        :return: Transfer function :math:`[ Mpc^{3/2} ]`
-        """
-        a_matter = np.sqrt(self._params.a_eq * self._params.a_eq2)
-        corr_fac = self.growth_a(a_matter, k=1.0) / a_matter * 10.0 / 9.0
+        # If the ksig determination goes out of bounds or sig^2(ksig^-1) is not strictly
+        # increasing # we return ksig = nan
+        if any([ksig == kseek[-1], ksig == kseek[0], np.any(np.diff(sig2gauss) <= 0)]):
+            ksig = np.nan
+
+        # assert np.abs(sig-1.0) <= 10 ** (-6), \
+        # 'The determination of k_sig failed to reach the required accuracy of 10^-6.\
+        # sig-1.0 = %d' %(np.abs(sig-1.0))
+
+        y = k / ksig
+        # Effective index, equation (C7)
+        # n = -3 - dlnsig^2/dlnR
+        #   = -3 + 2 int dlnk Dlin (k/ksig)^2 Wgauss(k/ksig) ** 2
+        np3 = 2.0 * np.trapz(y**2 * np.exp(-(y**2)) * Dlin / k, x=k)
+        # Spectral curvature, equation (C8)
+        # C = - d^2lnsig^2/dlnR^2
+        #   = 2(n+3) + (n+3)^2 - 4 int dlnk Dlin (k/ksig)^4 Wgauss(k/ksig) ** 2
+        C = (
+            (np3 + 1.0) ** 2
+            - 1.0
+            - 4.0 * np.trapz(y**4 * np.exp(-(y**2)) * Dlin / k, x=k)
+        )
 
-        if self._cosmo._pool is None or np.isscalar(k):
-            return self._transfer_k((0, k)) * corr_fac
+        return ksig, np3, C
 
-        pool = self._cosmo._pool
+    def _D_nonlin_halofit(self, Dlin, k, ksig, np3, C, a=1.0, model="halofit"):
+        """Returns the halofit nonlinear matter power spectrum per lnk
+        starting from the desired linear matter power spectrum.
+        If model == 0 it returns the nonlinear matter power spectrum as defined in
+        Smith et al., 2003, MNRAS, 341, 1311.
+        Note: all equations are defined in Appendix C of Smith et al.,
+        2003, MNRAS, 341, 1311
+        If model == 1 it returns the nonlinear matter power spectrum as defined in
+        Takahashi et al., 2012, ApJ, 761, 152
+        Note: all equations are defined in the Appendix of Takahashi et al.,
+        2012, ApJ, 761, 152"""
+
+        # Determine the fractional matter density at the redshift of interest
+        omega_m_z = self._background._omega_m_a(a=a)
+
+        # Dimensionless wavenumber, below Eq. (C2)
+        y = k / ksig
+        # Effective index, equation (C7)
+        # n = -3 - dlnsig^2/dlnR
+        #   = -3 + 2 int dlnk Dlin (k/ksig)^2 Wgauss(k/ksig) ** 2
+        # np3 = 2*np.trapz(ysq*np.exp(-ysq)*Dlin/k,x=k)
+        n = np3 - 3.0
+        # Spectral curvature, equation (C8)
+        # C = - d^2lnsig^2/dlnR^2
+        #   = 2(n+3) + (n+3)^2 - 4 int dlnk Dlin (k/ksig)^4 Wgauss(k/ksig) ** 2
+        # C = (np3+1) ** 2 - 1 - 4*np.trapz(ysq ** 2*np.exp(-ysq)*Dlin/k,x=k)
+
+        # omega_m_z dependent functions
+        # 1st case: Matter dominated universe
+        if self._params.omega_m == 1.0:
+            f1 = 1.0
+            f2 = 1.0
+            f3 = 1.0
+        # 2nd case: universe is not matter dominated, interpolate linearily between
+        # dark energy w and curvature with w_eff = -1/3
+        else:
+            w_z = self._background._w_a(a=a)
 
-        k = np.array(k)
-        n_chunks = min(len(k), pool._max_workers)
+            frac1 = self._params.omega_l / (self._params.omega_l + self._params.omega_k)
+            we = frac1 * w_z + 1.0 / 3.0 * (1.0 - frac1)
+            frac2 = -1.0 * ((3.0 * we) + 1.0) / 2.0
+
+            f1 = frac2 * omega_m_z**-0.0307 + (1 - frac2) * omega_m_z**-0.0732
+            f2 = frac2 * omega_m_z**-0.0585 + (1 - frac2) * omega_m_z**-0.1423
+            f3 = frac2 * omega_m_z**0.0743 + (1 - frac2) * omega_m_z**0.0725
+
+        # Coefficients used in the fitting function - this is the only difference
+        # between # Smith et al, 2003 and Takahashi et al., 2012
+        # Parameters from Smith et al, 2003 (model='halofit') or Takahashi et al. 2012
+        # (model='takahashi')
+        # Equations (C9) - (C16) of Smith et al., 2003
+        if model == "halofit":
+            a_hf = np.power(
+                10,
+                1.4861
+                + 1.8369 * n
+                + 1.6762 * n**2
+                + 0.7940 * n**3
+                + 0.1670 * n**4
+                - 0.6206 * C,
+            )
+            b = np.power(10, 0.9463 + 0.9466 * n + 0.3084 * n**2 - 0.9400 * C)
+            c = np.power(10, -0.2807 + 0.6669 * n + 0.3214 * n**2 - 0.0793 * C)
+            alpha = 1.3884 + 0.3700 * n - 0.1452 * n**2
+            beta = 0.8291 + 0.9854 * n + 0.3401 * n**2
+            gamma = 0.8649 + 0.2989 * n + 0.1631 * C
+            mu = 10 ** (-3.5442 + 0.1908 * n)
+            nu = np.power(10.0, 0.9589 + 1.2857 * n)
+        elif model == "rev_halofit":
+            # Equations (A6) - (A13) of Takahashi et al., 2012
+            omega_l_z = self._background._omega_l_a(a=a)  # noqa
+            gamma = 0.1971 - 0.0843 * n + 0.8460 * C
+
+            # The quasi-linear term
+            # Equation (C2)
+            DQ_plus_DH = ne.evaluate(
+                """(
+                Dlin
+                * exp(-0.25 * y - 0.125 * y ** 2)
+                * (1 + Dlin)
+                ** (
+                    2.0379
+                    - 0.7354 * n
+                    + 0.3157 * n**2
+                    + 1.2490 * n**3
+                    + 0.3980 * n**4
+                    - 0.1682 * C
+                )
+                / (1 + abs(6.0835 + 1.3373 * n - 0.1959 * n**2 - 5.5274 * C) * Dlin)
+            )"""
+            )
 
-        perm = np.argsort(k)
-        k = k[perm]
-        args = [(i, k[i::n_chunks]) for i in range(n_chunks)]
+            # The halo term
+            # Equations (C3) - (C4)
+            w0 = self._params.w0  # noqa
+            DQ_plus_DH += ne.evaluate(
+                """(
+                10 ** (
+                    1.5222
+                    + 2.8553 * n
+                    + 2.3706 * n**2
+                    + 0.9903 * n**3
+                    + 0.2250 * n**4
+                    - 0.6038 * C
+                    + 0.1749 * omega_l_z * (1 + w0)
+                )
+                * y ** (2 + 3 * f1)
+                / (y ** 2 + 10 ** (5.2105 + 3.6902 * n))
+                / (
+                    1
+                    + 10 ** (
+                        -0.5642
+                        + 0.5864 * n
+                        + 0.5716 * n**2
+                        - 1.5474 * C
+                        + 0.2279 * omega_l_z * (1 + w0)
+                    )
+                    * y ** f2
+                    + (
+                        10 ** (0.3698 + 2.0404 * n + 0.8161 * n**2 + 0.5869 * C)
+                        * f3
+                        * y
+                    )
+                    ** (3 - gamma)
+                  )
+                )"""
+            )
+            return DQ_plus_DH
+        else:
+            raise NotImplementedError(
+                "non linear model {} not implemented".format(model)
+            )
 
-        results = pool.map(self._transfer_k, args)
-        # trick to revert chunking:
-        unchunked = np.array(
-            [ti for t in itertools.zip_longest(*results) for ti in t if ti is not None]
+        # The quasi-linear term
+        # Equation (C2)
+        DQ_plus_DH = (
+            Dlin
+            * np.exp(-0.25 * y - 0.125 * y**2)
+            * (1 + Dlin) ** beta
+            / (1 + alpha * Dlin)
         )
-        inverse_perm = np.arange(len(perm))[perm]
-        return corr_fac * unchunked[inverse_perm]
 
-    def fields(
-        self,
-        k,
-        grid,
-        sec_factor=5,
-        keep_lna0=False,
-        initial_conditions=None,
-        enable_fast_solver=True,
-        enable_sparse_lu_solver=True,
-    ):
-        """
-        Solves the Einstein-Boltzmann ODE system for the evolution
-        of the linear order perturbation of the fields.
-
-        :param k: wavenumber :math:`[h/Mpc]`
-        :param grid: ln(a) values at which to output fields [1]
-        :param sec_factor: relaxes row permutation criterium in optimized LUP solver
-        :param keep_lna0: if True includes the fields at initial time a_0
-        :param initial_conditions: can pass a_0, y_0 (vector of initial conditions)
-        :param enable_fast_solver: if set to False always use standard LUP solver for
-                                   full matrix
-        :param enable_sparse_lu_solver: if set to True: avoid iterating over known
-                                        zero-entries in fallback LUP solver
-
-        :return: Linear order perturbations, accessed with fields.a, fields.Phi etc.
-        """
-        grid, solver_result, meta, keep_lna_0 = self._compute_fields(
-            k,
-            grid,
-            sec_factor,
-            keep_lna0,
-            initial_conditions,
-            enable_fast_solver,
-            enable_sparse_lu_solver,
+        # The halo term
+        # Equations (C3) - (C4)
+        DQ_plus_DH += (
+            a_hf
+            * y ** (2 + 3 * f1)
+            / (y**2 + mu * y + nu)
+            / (1 + b * y**f2 + (c * f3 * y) ** (3 - gamma))
         )
-        fields = Fields(self._cosmo)
-        fields.set_results(grid, solver_result)
-        fields.meta = meta
-        return fields
-
-    def _sigma_k_grid(self):
-        c = self._cosmo
-        k_wiggles = np.pi / (c.background.r_s() / c.params.h)
-        k_first = 10 ** np.linspace(-5, np.log10(k_wiggles), 10)
-
-        h = np.pi / 5
-        n = 22
-        k_middle = k_wiggles * np.arange(1, n / h) * h
-
-        k_last = 10 ** np.linspace(np.log10(k_middle[-1]), 2, 10)
-
-        k_grid = np.hstack((k_first, k_middle, k_last))
-        # remove duplicates in log values:
-        return sorted({np.log(k): k for k in k_grid}.values())
-
-    def _compute_fields(
-        self,
-        k,
-        grid,
-        sec_factor=3,
-        keep_lna0=False,
-        initial_conditions=None,
-        enable_fast_solver=True,
-        enable_sparse_lu_solver=True,
-    ):
-
-        grid = np.atleast_1d(grid)
-        grid, solver_result, meta = self._solver.solve(
-            k,
-            grid,
-            sec_factor,
-            initial_conditions,
-            enable_fast_solver,
-            enable_sparse_lu_solver,
-            keep_lna0,
-        )
-        new_traces = meta["new_traces"]
-        if (isinstance(new_traces, dict) and new_traces) or (
-            isinstance(new_traces, list) and any(new_traces)
-        ):
-            print_new_traces(self._cosmo._cache_file)
-        return grid, solver_result, meta, keep_lna0
-
-    def P_R_k(self, k):
-        """
-        Computes the primordial power spectrum of gauge invariant curvature
-        perturbations (R)
-
-        :param k: wavenumber :math:`[1/Mpc]`
-        :return: P_R(k), primordial power spectrum of R
-        """
-        if self._params.pk_norm_type == "A_s":
-            norm = self._params.As_norm / self._params.k_pivot ** (self._params.n - 1)
-        elif self._params.pk_norm_type == "sigma8":
-            if self._params.As_norm is None:
-                self._setup_norm()
-
-            norm = self._params.As_norm / self._params.k_pivot ** (self._params.n - 1)
-        else:
-            raise ValueError("Need A_s or sigma8 normalization for P_R(k)")
-
-        return norm * k ** (self._params.n - 1)
 
+        return DQ_plus_DH
 
-def src_m_column_j(arg):
-    self, a, onek = arg
-    a = np.atleast_1d(a)
-    grid, y, meta, keep_lna0 = self._compute_fields(onek, grid=np.log(a))
-
-    n_grid = len(grid)
-    a = a[-n_grid:]
-    delta = y[:, 1]
-    theta = y[:, 2] * onek
-    delta_b = y[:, 3]
-    theta_b = y[:, 4] * onek
-    H = self._background.H(a) / (self._params.H0 * self._params.rh)
-    omega_nu_m = 0.0
-    P_nu_m = 0.0
-    omega_m_tot = self._params.omega_m
-    omega_plus_p_m_tot = self._params.omega_m
-    # include massive neutrinos in the total matter term
-    src_col = np.zeros((n_grid,))
-    if self._params.N_massive_nu != 0:
-        omega_nu_m = self._wrapper.omega_nu_m_ufunc(a)
-        P_nu_m = self._wrapper.P_nu_m_ufunc(a)
-        omega_m_tot += omega_nu_m / a
-        omega_plus_p_m_tot += (omega_nu_m + P_nu_m) / a
-        delta_nu_m = self._wrapper.delta_nu_m_ufunc(a, y[1:])
-        theta_nu_m = onek * self._wrapper.u_nu_m_ufunc(a, y[1:])
-        src_col += (
-            delta_nu_m * omega_nu_m / a / omega_m_tot
-            + (3 * a * H / onek ** 2)
-            * theta_nu_m
-            * (omega_nu_m + P_nu_m)
-            / a
-            / omega_plus_p_m_tot
-        )
+    # The set of fucntions useful to comupte the One-Halo and Two-Halo terms
+    # in Mead follow here
 
-    delta_m_tot = self._params.omega_dm * delta + self._params.omega_b * delta_b
-    theta_m_tot = self._params.omega_dm * theta + self._params.omega_b * theta_b
+    def _sigma_v(self, k, Dlin):
+        """
+        :param a: scale factor
+        :param k: wavenumber [Mpc^-1]
+        :param Dlin: P(k) linear-theory matter power spectrum P(k) [Mpc^3]
+        :return: 1D linear displacement variance, as defined in eq.4 in Mead et al, 2015
+        """
+        integr = 1.0 / 3 * np.trapz(Dlin / (k**3), x=k, axis=1)
+        sigmav = np.sqrt(integr)
+        return np.sqrt(sigmav)
 
-    src_col += (
-        delta_m_tot / omega_m_tot
-        + (3 * a * H / onek ** 2) * theta_m_tot / omega_plus_p_m_tot
-    )
-    return src_col
+    def _sigma_d_100(self, k, Dlin):
+        """
+        :param a: scale factor
+        :param k: wavenumber [Mpc^-1]
+        :param Dlin: P(k) linear-theory matter power spectrum P(k) [Mpc^3]
+        :return: 1D linear displacement variance, as defined in eq.4 in Mead et al, 2016
+        """
+        k = np.atleast_1d(k)
+        R = 100.0 / self._params.h
+        T = 3 / ((k * R) ** 3) * (np.sin(k * R) - np.cos(k * R))
+        # T = self.T(k * R)
+        integr = 1.0 / 3 * np.trapz((Dlin / (k**3)) * (T**2), x=k, axis=1)
+        sigma_d100 = np.sqrt(integr)
+        return sigma_d100
+
+    def _sigma8(self, a, k, Dlin):
+        """
+        Compute sigma8, the rms density contrast fluctuation smoothed with a top hat of
+        radius 8 h^-1 Mpc at redshift z.
+        :param a: scale factor
+        :param k: wavenumber [Mpc^-1]
+        :param Dlin: P(k) linear-theory matter power spectrum P(k) [Mpc^3]
+        :return sig8z: sigma8 at the desired redshift [1]
+        """
+        R = 8.0 / self._params.h  # smoothing radius [Mpc]
+        lnk = np.log(k)
+        w = (
+            3 / ((k * R) ** 3) * (np.sin(k * R) - np.cos(k * R))
+        )  # top hat window function
+        res = np.trapz(k**3 * Dlin[0] * w**2, lnk)
+        sig8z = np.sqrt(1.0 / (2.0 * np.pi**2) * res)
+
+        return sig8z
+
+    def _windowf(self, k, r_v, c):
+        """
+        :param r_v: virial radius
+        :param c: concentration parameter
+        :return: Fourier Transform of the halo density profile
+        """
+        k = np.atleast_1d(k)
+        # Normalised mass of a halo of concentration c
+        f_c = np.log(1 + c) - c / (1 + c)
+        k_s = k * r_v / c
+
+        Si1, Ci1 = scipy.special.sici(k_s * (1 + c))
+        Si2, Ci2 = scipy.special.sici(k_s)
+        W = (
+            (Ci1 - Ci2) * np.cos(k_s)
+            + (Si1 - Si2) * np.sin(k_s)
+            - np.sin(c * k_s) / (k_s * (1 + c))
+        ) / f_c
+        return W
+
+    def _rho_critic(self):
+        # Newton's gravitational constant as in Mo, Bosch & White "Galaxy
+        # Formation and Evolution" (2010)
+        G = 4.299e-9
+        rho = 3 * self._params.H0**2 / (8 * np.pi * G)
+        return rho
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/LsodaSolver.py` & `PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/LsodaSolver.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,42 +29,44 @@
     def __init__(
         self,
         verbose,
         rtol,
         atol,
         max_bdf_order,
         max_iter,
+        h0,
         cosmology,
         fast_solver,
         **extra_args_for_solver,
     ):
         self.verbose = verbose
         self.rtol = rtol
         self.atol = atol
         self.max_bdf_order = max_bdf_order
         self.max_iter = max_iter
+        self.h0 = h0
         self.extra_args_for_solver = extra_args_for_solver
 
         self.params = cosmology.params
-        self.cosmology = cosmology
-        self.background = cosmology.background
-        self.fast_solver = fast_solver
-
+        # self.background = cosmology.background
         self.wrapper = cosmology._wrapper
 
+        assert fast_solver, "slow solver not supported anymore"
+        self.fast_solver = fast_solver
+
     def initial_conditions(self, k):
         self.wrapper.set_globals(k=k)
 
         initial_conditions = getattr(
             self.wrapper, "initial_values_" + self.params.initial_conditions, None
         )
         if initial_conditions is None:
             raise ValueError(
-                "initial conditions '{}' not implemented.".format(
-                    self.params.initial_conditions
+                "{}: initial conditions '{}' not implemented.".format(
+                    self.wrapper, self.params.initial_conditions
                 )
             )
 
         return initial_conditions()
 
     def _setup_globals(self, k):
         parameters = {"k": k}
@@ -104,34 +106,27 @@
             warnings.warn(
                 "grid starts before initial a0= {:e} resp lna0 = {:e}, removed"
                 " therefore gridpoints".format(a_0, lna0)
             )
         grid = grid[grid > lna0]
         grid = np.concatenate(([lna0], grid))
 
-        atol = self.atol
-        rtol = self.rtol
-        max_order = self.max_bdf_order
-        max_iter = self.max_iter
-
-        if self.fast_solver:
-            solver = getattr(self.wrapper, "solve_fast_" + self.SOLVER_ID)
-        else:
-            solver = getattr(self.wrapper, "solve_" + self.SOLVER_ID)
+        solver = getattr(self.wrapper, "solve_fast_" + self.SOLVER_ID)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             y, meta = solver(
                 y_0,
                 grid,
-                rtol,
-                atol,
-                max_order=max_order,
-                max_iter=max_iter,
+                self.rtol,
+                self.atol,
+                max_order=self.max_bdf_order,
+                max_iter=self.max_iter,
                 enable_fast_solver=enable_fast_solver,
                 enable_sparse_lu_solver=enable_sparse_lu_solver,
+                h0=self.h0,
             )
         if meta["istate"] <= 0:
             raise RuntimeError(f"solving ode failed for k = {k}, meta={meta}")
 
         start_idx = 0 if keep_lna0 else 1
         return grid[start_idx:], y[start_idx:], meta
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/BoltzmannSolver/__init__.py` & `PyCosmo-2.1.1/src/PyCosmo/BoltzmannSolver/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/Cosmo.py` & `PyCosmo-2.1.1/src/PyCosmo/Cosmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,41 +18,66 @@
 import functools
 import hashlib
 import os
 import sys
 import textwrap
 import types
 from concurrent.futures import ProcessPoolExecutor
+from datetime import datetime
 from multiprocessing import current_process
 
 import dill
 import numpy as np
 from sympy2c import __version__ as sympy2c_version
 from sympy2c.compiler import base_cache_folder, load_module
+from sympy2c.utils import get_platform
 
-from PyCosmo import core_file_handling
 from PyCosmo.Background import Background, _call
-from PyCosmo.BoltzmannSolver.LinearPerturbationBoltzmann import (
-    LinearPerturbationBoltzmann,
-)
 from PyCosmo.LinearPerturbationApprox import LinearPerturbationApprox
-from PyCosmo.PerturbationTable import PerturbationTable
 
 from ._Util import get_active_branch_name
 from .config import INFO, check_flattened, load_parameters_ini
 from .disable_multithreading import disable_multithreading
 from .ini_handling import Bunch
-from .NonLinearPerturbationHaloFit import NonLinearPerturbationHaloFit
-from .NonLinearPerturbationMead import NonLinearPerturbationMead
 from .Projection import Projection
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 disable_multithreading()
 
+proc_name = current_process().name
+
+
+def trace_call(frame, event, arg):
+    if event in ("line",):
+        return trace_call
+    fname = frame.f_code.co_filename
+    if any(
+        n in fname
+        for n in (
+            "pprint",
+            "dill",
+            "pickle",
+            "numba",
+            "logging",
+            "ini_handling",
+            "traceback",
+            "weakref",
+            "llvmlite",
+        )
+    ):
+        return trace_call
+    print(datetime.now(), end=" ")
+    fr = frame
+    print(proc_name, event, end="")
+    while (fr := fr.f_back) is not None:
+        print("  ", end="")
+    print(fname, frame.f_code.co_name, frame.f_lineno, flush=True)
+    return trace_call
+
 
 def make_pickable(checks):
     detached_checks = [
         types.FunctionType(check.__code__, __builtins__) for check in checks
     ]
     return detached_checks
 
@@ -109,43 +134,50 @@
     def _load_wrapper(self):
 
         from . import version
 
         branch = get_active_branch_name() or ""
 
         folder = os.path.join(
-            base_cache_folder(), "PyCosmo", branch, version.replace(".", "_")
+            base_cache_folder(),
+            "PyCosmo",
+            get_platform(),
+            branch,
+            version.replace(".", "_"),
         )
         if not os.path.exists(folder):
             try:
                 os.makedirs(folder)
             except IOError:
                 # might be triggered due to race condition when run in parallel
                 assert os.path.exists(folder), "this must not happen"
 
         cache_file = os.path.join(folder, self._cache_file_name)
 
         wrapper_loaded = False
         if os.path.exists(cache_file):
             print("cache hit at", cache_file)
 
-            data = dill.load(open(cache_file, "rb"))
+            with open(cache_file, "rb") as fh:
+                data = dill.load(fh)
 
             folder = data["folder"]
             checks = data["checks"]
             enrich_params = data["enrich_params"]
 
             try:
                 print("load wrapper from", folder)
                 wrapper = load_module(folder)
                 wrapper_loaded = True
             except ImportError:
                 wrapper = None
 
         if not wrapper_loaded:
+            from PyCosmo import core_file_handling
+
             module, checks, enrich_params = core_file_handling.load_core_files(
                 self.core_equations_files, self.model_config
             )
             compilation_flags = self.model_config.main.compilation_flags.split(" ")
             wrapper = module.compile_and_load(compilation_flags=compilation_flags)
 
             data = {
@@ -165,21 +197,23 @@
         self._cache_file = cache_file
 
     @staticmethod
     def recompile_from_cli():
         assert len(sys.argv) == 2, "need name to pkl file"
         cache_file = sys.argv[1]
         try:
-            data = dill.load(open(cache_file, "rb"))
+            with open(cache_file, "rb") as fh:
+                data = dill.load(fh)
         except Exception as e:
             print("could not read {}: {}".format(cache_file, e))
             sys.exit(1)
 
         model_config = data["model_config"]
         compilation_flags = model_config.main.compilation_flags.split(" ")
+        from PyCosmo import core_file_handling
 
         module, _, _ = core_file_handling.load_core_files(
             model_config["main"]["core_equations_files"], model_config
         )
         wrapper = module.recompile_and_load(
             compilation_flags=compilation_flags, force=True
         )
@@ -252,23 +286,30 @@
             self.print_params(inc_derived=False)
             print("")
         else:
             print("Parameters updated")
 
     def __getstate__(self):
         dd = self.__dict__.copy()
+
+        dd["model_config"] = dill.dumps(dd["model_config"])
         dd["model_parameter_checks"] = dill.dumps(dd["model_parameter_checks"])
         dd["model_enrich_params"] = dill.dumps(dd["model_enrich_params"])
         dd["_pool"] = None
+        del dd["background"]
+        del dd["projection"]
+        del dd["lin_pert"]
+        del dd["nonlin_pert"]
+        del dd["rec"]
+        # sys.settrace(trace_call)
+
         return dd
 
     def __setstate__(self, dd):
-        # preload notebooks, required for first compilation in parallel mode
-        core_equations_files = dd["model_config"]["main"]["core_equations_files"]
-        core_file_handling.load_core_files(core_equations_files, dd["model_config"])
+        dd["model_config"] = dill.loads(dd["model_config"])
         dd["model_parameter_checks"] = dill.loads(dd["model_parameter_checks"])
         dd["model_enrich_params"] = dill.loads(dd["model_enrich_params"])
         self.__dict__.update(dd)
         self._reset()
 
     def _reset(self):
         """
@@ -328,17 +369,18 @@
 
             if self._pool is None:
                 if params.n_cores > 1:
                     self._pool = ProcessPoolExecutor(params.n_cores)
             else:
                 if self._pool._max_workers != params.n_cores:
                     self._pool.shutdown()
-                    self._pool = None
-                if params.n_cores > 1:
-                    self._pool = ProcessPoolExecutor(params.n_cores)
+                    if params.n_cores == 1:
+                        self._pool = None
+                    else:
+                        self._pool = ProcessPoolExecutor(params.n_cores)
 
         recomb = params.recomb
         if recomb == "recfast++":
             from PyCosmo._Recombination import Recombination
 
             self.rec = Recombination(params)
         elif recomb == "class":
@@ -366,42 +408,52 @@
         if params.pk_type in ("EH", "BBKS", "BBKS_CCL"):
             if params.pk_norm == "A_s":
                 raise ValueError(
                     "A_s normalization not available for fitting functions"
                 )
             self.lin_pert = LinearPerturbationApprox(self)
         elif params.pk_type == "boltz":
+            from PyCosmo.BoltzmannSolver.LinearPerturbationBoltzmann import (
+                LinearPerturbationBoltzmann,
+            )
+
             self.lin_pert = LinearPerturbationBoltzmann(self)
             if params.pk_nonlin_type is not None:
                 params.pk_nonlin_type = None
         else:
             # Todo raise an error
             raise ValueError("unknown pk_type value {} used".format(params.pk_type))
 
         if params.pk_nonlin_type == "halofit" or params.pk_nonlin_type == "rev_halofit":
             assert (
                 params.pk_type != "boltz"
             ), "Halofit model not supported by the Boltzmann solver yet!"
+            from .NonLinearPerturbationHaloFit import NonLinearPerturbationHaloFit
+
             self.nonlin_pert = NonLinearPerturbationHaloFit(self)
 
         elif params.pk_nonlin_type == "mead":
             assert (
                 params.pk_type != "boltz"
             ), "Mead model not supported by the Boltzmann solver yet!"
+            from .NonLinearPerturbationMead import NonLinearPerturbationMead
+
             self.nonlin_pert = NonLinearPerturbationMead(self)
 
         elif params.pk_nonlin_type is None:
             self.nonlin_pert = None
 
         else:
             raise ValueError(
                 'unknown pk_nonlin_type "{}"'.format(params.pk_nonlin_type)
             )
 
         if params.tabulation != "off":
+            from PyCosmo.PerturbationTable import PerturbationTable
+
             self.lin_pert = PerturbationTable(self, self.lin_pert)
             if self.nonlin_pert is not None:
                 self.nonlin_pert = PerturbationTable(self, self.nonlin_pert)
 
         if self.nonlin_pert is None:
             self.projection = FakeProjection()
             return
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     k,
 )
 
 
 h = H0 / 100
 neq = 5 + 3 * (l_max + 1)
 
+
 # check functions used to impose conditions
 # on the parameters
 def check_wa(params):
     if "wa" not in params:
         return "wa not set"
     wa = params.wa
     if wa != 0:
@@ -474,14 +475,16 @@
     + (3 * a * H_Mpc / k)
     * (
         (omega_dm * u + omega_b * u_b) / a**3
         + 4 * (omega_gamma * Theta[1] + omega_neu * N[1]) / a**4
     )
 ) / ((omega_dm + omega_b) / a**3 + (omega_gamma + omega_neu) / a**4)
 
+Psi = -Phi - 12 * (H0_Mpc / (k * a)) ** 2 * (omega_gamma * Theta[2] + omega_neu * N[2])
+
 
 def rhs(H=H_Mpc, H0=H0_Mpc, R=R, l_max=l_max):
     """
     rhs of the ODE system containing the equations
     in d(lna), order needs to be the same as in lhs
     """
 
@@ -594,14 +597,15 @@
     "linear_perturbation", lna, lhs(), rhs(), splits=splits, reorder=reorder
 )
 ode = Ode("linear_perturbation", lna, lhs(), rhs())
 
 
 y = Alias("y", *lhs())
 fun_econ = Function("econ", econ, a, y)  # export econ as a function
+fun_Psi = Function("Psi", Psi, a, y)  # export econ as a function
 
 # jacobian, can be used for scipy ODE solvers, currently not implemented
 ddy = sp.Matrix(rhs()).jacobian(lhs())
 fun_linear_perturbation_jac = Function(
     "linear_perturbation_jac", ddy.reshape(1, ddy.rows * ddy.cols), lna, y
 )
 
@@ -636,11 +640,12 @@
     l_max = cosmology.model_config.equation_parameters.l_max
     for i in range(l_max + 1):
         lhs.append(f"Theta[{i}]")
         lhs.append(f"Theta_P[{i}]")
         lhs.append(f"N[{i}]")
     fields = dict(zip(lhs, y.T))
     fields["econ"] = econ_ufunc(np.exp(lna), y)
+    fields["Psi"] = Psi_ufunc(np.exp(lna), y)
     return fields
 
 
 fields = PythonFunction(fields)
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu_rsa.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu_rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,76 +90,76 @@
     Theta_interp[0] = Phi + u_b * taudot_interp(a) / k
     Psi = -Phi - 12 * (H0 / (k * a)) ** 2 * (
         omega_gamma * Theta_interp[2] + omega_neu * N_interp[2] + C_nu * sum_M2
     )
     Pi = Theta_interp[2] + Theta_P_interp[0] + Theta_P_interp[2]
     dPhi_dlan = (
         Psi
-        - k_H ** 2 / 3 * Phi
+        - k_H**2 / 3 * Phi
         + (H0 / H) ** 2
         / 2
         * (
-            (omega_dm * delta + omega_b * delta_b) * a ** -3
+            (omega_dm * delta + omega_b * delta_b) * a**-3
             + 4
             * (omega_gamma * Theta_interp[0] + omega_neu * N_interp[0] + C_nu * sum_M0)
-            * a ** -4
+            * a**-4
         )
     )
 
     # Boltzmann equations for the various components
     # N_interp[1] = -2 * a * H / k * dPhi_dlan
-    Theta_interp[1] = -2 * a * H / k * dPhi_dlan + a * H * taudot_interp(a) / k ** 2 * (
+    Theta_interp[1] = -2 * a * H / k * dPhi_dlan + a * H * taudot_interp(a) / k**2 * (
         u_b - k_H * c_s_interp(a) ** 2 * delta_b + k_H * Phi
     )  # Theta_1 RSA
     ddelta_dlan = -k_H * u - 3 * dPhi_dlan  # dark matter density
     du_dlan = -u + k_H * Psi  # dark matter velocity
     ddelta_b_dlan = -k_H * u_b - 3 * dPhi_dlan  # baryonic matter density
     du_b_dlan = (
         -u_b
         + k_H * Psi
         + taudot_interp(a) / (R * a * H) * (u_b - 3 * Theta_interp[1])
         + k_H * c_s_interp(a) ** 2 * delta_b
     )  # baryonic matter velocity
 
     for j in range(nq):
         # Massive neutrinos: the first nq values of the array are the 0th multipole
-        dM_dlan[j] = -qq[j] * k_H / sp.sqrt(amnu ** 2 + qq[j] ** 2) * M[
+        dM_dlan[j] = -qq[j] * k_H / sp.sqrt(amnu**2 + qq[j] ** 2) * M[
             nq + j
         ] - dPhi_dlan * qq[j] / (sp.exp(-qq[j]) + 1)
         # Massive neutrinos: the second nq values of the array are the 1st multipole
         dM_dlan[nq + j] = (
             1
             / (a * H)
             * (
                 qq[j]
                 * k
-                / (3 * sp.sqrt(amnu ** 2 + qq[j] ** 2))
+                / (3 * sp.sqrt(amnu**2 + qq[j] ** 2))
                 * (M[j] - 2 * M[2 * nq + j])
-                + sp.sqrt(amnu ** 2 + qq[j] ** 2) * k / 3 * Psi / (sp.exp(-qq[j]) + 1)
+                + sp.sqrt(amnu**2 + qq[j] ** 2) * k / 3 * Psi / (sp.exp(-qq[j]) + 1)
             )
         )
     # lth multipoles massive neutrinos
     for m in range(2, l_max_mnu):
         for j in range(nq):
 
             dM_dlan[m * nq + j] = (
                 qq[j]
                 * k
-                / (a * H * sp.sqrt(amnu ** 2 + qq[j] ** 2) * (2 * m + 1))
+                / (a * H * sp.sqrt(amnu**2 + qq[j] ** 2) * (2 * m + 1))
                 * (m * M[(m - 1) * nq + j] - (m + 1) * M[(m + 1) * nq + j])
             )
     # hierarchy truncation massive neutrinos
     for j in range(nq):
         dM_dlan[l_max_mnu * nq + j] = (
             1
             / (a * H)
             * (
                 qq[j]
                 * k
-                / sp.sqrt(amnu ** 2 + qq[j] ** 2)
+                / sp.sqrt(amnu**2 + qq[j] ** 2)
                 * M[(l_max_mnu - 1) * nq + j]
                 - (l_max_mnu + 1) / eta_interp(a) * M[l_max_mnu * nq + j]
             )
         )
 
     # returns the rhs in the right order
     ret = [dPhi_dlan, ddelta_dlan, du_dlan, ddelta_b_dlan, du_b_dlan]
@@ -168,15 +168,19 @@
     return ret
 
 
 def switch_time(wrapper, lna):  # pragma: no cover
     # use trigger parameters to determine a
     # at which RSA kicks in (as a function of k)
     a = np.logspace(-3, 0, 50)
-    eta_ = wrapper.eta(a)
+    print(wrapper)
+    y, _ = wrapper.solve_fast_eta(
+        np.array((0.0,)), np.concatenate(([1e-100], a)), 1e-8, 1e-8
+    )
+    eta_ = y.flatten()[1:]
     a_tau = np.where(
         (-1 / (taudot_interp_ufunc(a) * eta_) > wrapper.globals.rsa_trigger_taudot_eta),
         a,
         1.0,
     )
     lim = wrapper.globals.k * eta_ > wrapper.globals.rsa_trigger_k_eta
     a_keta = np.where(lim, a, 1.0)
@@ -225,17 +229,17 @@
     a = np.exp(t_1)
 
     # and derived params
     T_0 = Tcmb * T_mnu
     amnu = a * massive_nu_total_mass / (N_massive_nu * kb * T_0)
     rho_ev = (
         3
-        * H0 ** 2
+        * H0**2
         * (hbar) ** 3
-        * c_ms ** 3
+        * c_ms**3
         / (8 * np.pi * G)
         / evc2
         / (mpc / 1000) ** 2
     ) / (kb * T_0) ** 4
     C_nu = N_massive_nu / (2 * np.pi) ** 2 / rho_ev
 
     Phi = y_1[:, 0]
@@ -285,25 +289,25 @@
     Psi = -Phi - 12 * (1 / (rh * k * a)) ** 2 * (C_nu * sum_M2)
     dPhi_dlan = (
         Psi
         - (k / (a * H_Mpc)) ** 2 / 3 * Phi
         + (1 / (rh * H_Mpc)) ** 2
         / 2
         * (
-            (omega_dm * delta + omega_b * delta_b) * a ** -3
+            (omega_dm * delta + omega_b * delta_b) * a**-3
             + 4
             * (omega_gamma * Theta0_interp + omega_neu * N0_interp + C_nu * sum_M0)
-            * a ** -4
+            * a**-4
         )
     )
 
     N1_interp = -2 * a * H_Mpc / k * dPhi_dlan
     Theta1_interp = -2 * a * H_Mpc / k * dPhi_dlan + a * H_Mpc * taudot_interp_ufunc(
         a
-    ) / k ** 2 * (
+    ) / k**2 * (
         u_b
         - k / (a * H_Mpc) * c_s_interp_ufunc(a) ** 2 * delta_b
         + k / (a * H_Mpc) * Phi
     )
 
     # reshape and stack perturbations
     N0_interp = np.reshape(N0_interp, (len(y_1[:, 0]), 1))
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu_wcdm.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu_wcdm.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_massivenu_wcdm_rsa.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_massivenu_wcdm_rsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,15 +193,18 @@
     return ret
 
 
 def switch_time(wrapper, lna):  # pragma: no cover
     # use trigger parameters to determine a
     # at which RSA kicks in (as a function of k)
     a = np.logspace(-3, 0, 50)
-    eta_ = wrapper.eta(a)
+    y, _ = wrapper.solve_fast_eta(
+        np.array((0.0,)), np.concatenate(([1e-100], a)), 1e-8, 1e-8
+    )
+    eta_ = y.flatten()[1:]
     a_tau = np.where(
         (-1 / (taudot_interp_ufunc(a) * eta_) > wrapper.globals.rsa_trigger_taudot_eta),
         a,
         1.0,
     )
     lim = wrapper.globals.k * eta_ > wrapper.globals.rsa_trigger_k_eta
     a_keta = np.where(lim, a, 1.0)
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_rsa.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,30 +114,32 @@
     return ret
 
 
 def switch_time(wrapper, lna):  # pragma: no cover
     # use trigger parameters to determine a
     # at which RSA kicks in (as a function of k)
     a = np.logspace(-3, 0, 50)
-    eta_ = wrapper.eta(a)
+    y, _ = wrapper.solve_fast_eta(
+        np.array((0.0,)), np.concatenate(([1e-100], a)), 1e-8, 1e-8
+    )
+    eta_ = y.flatten()[1:]
     a_tau = np.where(
         (
             -1 / (taudot_interp_ufunc(a) * eta_)
             > get_globals()["rsa_trigger_taudot_eta"]
         ),
         a,
         1.0,
     )
     lim = get_globals()["k"] * eta_ > get_globals()["rsa_trigger_k_eta"]
     a_keta = np.where(lim, a, 1.0)
     lna_cut = np.log(max(min(a_keta), min(a_tau)))
     return lna_cut
 
 
-
 def switch(wrapper, t, y):  # pragma: no cover
     # initial conditions for RSA ODE system
     return y[-1, :5]
 
 
 def merge(wrapper, t_0, t_switch, t_1, y_0, y_1):  # pragma: no cover
     """
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_wcdm.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_wcdm.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/CosmologyCore_wcdm_rsa.py` & `PyCosmo-2.1.1/src/PyCosmo/CosmologyCore_wcdm_rsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,30 +135,32 @@
     return ret
 
 
 def switch_time(wrapper, lna):  # pragma: no cover
     # use trigger parameters to determine a
     # at which RSA kicks in (as a function of k)
     a = np.logspace(-3, 0, 50)
-    eta_ = wrapper.eta(a)
+    y, _ = wrapper.solve_fast_eta(
+        np.array((0.0,)), np.concatenate(([1e-100], a)), 1e-8, 1e-8
+    )
+    eta_ = y.flatten()[1:]
     a_tau = np.where(
         (
             -1 / (taudot_interp_ufunc(a) * eta_)
             > get_globals()["rsa_trigger_taudot_eta"]
         ),
         a,
         1.0,
     )
     lim = get_globals()["k"] * eta_ > get_globals()["rsa_trigger_k_eta"]
     a_keta = np.where(lim, a, 1.0)
     lna_cut = np.log(max(min(a_keta), min(a_tau)))
     return lna_cut
 
 
-
 def switch(wrapper, t, y):  # pragma: no cover
     # initial conditions for RSA ODE system
     return y[-1, :7]
 
 
 def merge(wrapper, t_0, t_switch, t_1, y_0, y_1):  # pragma: no cover
     """
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/LinearPerturbationApprox.py` & `PyCosmo-2.1.1/src/PyCosmo/LinearPerturbationApprox.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         !!!NEED TO INCLUDE REFERENCE!!!
         """
         a_temp = np.exp(
             np.array(x)
         )  # ; x=ln(a) #; compute derivatives of y1=G and y2=dG/dlna
         f1 = y[1]  # f1=dy1/dx=y2=dG/dlna
 
-        _dlnh_dlna = self._background._dlnh_dlna(a=a_temp)
+        _dlnh_dlna = self._background._dlnh_dlna(a=a_temp)[0]
 
         f2 = (
             -(4.0 + _dlnh_dlna) * y[1]
             - (3.0 + _dlnh_dlna - 1.5 * self._background._omega_m_a(a=a_temp)) * y[0]
         )
         return [f1, f2]
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/LinearPerturbationBase.py` & `PyCosmo-2.1.1/src/PyCosmo/LinearPerturbationBase.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/LinearPerturbationTable.py` & `PyCosmo-2.1.1/src/PyCosmo/LinearPerturbationTable.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/NonLinearPerturbationMead.py` & `PyCosmo-2.1.1/src/PyCosmo/NonLinearPerturbationMead.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with this
 # program.  If not, see <http://www.gnu.org/licenses/>.
 
 
-import numba
 import numpy as np
-from scipy import special
 
 from PyCosmo.cython.halo_integral import _integral_halo as cython_integral_halo
 from PyCosmo.PerturbationBase import NonLinearPerturbationBase
 from PyCosmo.TheoryPredTables import TheoryPredTables
 
 from ._scipy_utils import interp1d
 
@@ -283,14 +281,43 @@
         r"""
         Computes the Fourier Transform of a 3D spherical top-hat function.
 
         :param x: dimensionless parameter (usually equal to :math:`kr`) [1]
         :return: Fourier Transform of a 3D spherical top-hat function.
         """
 
+        import numba
+
+        @numba.njit(numba.float64[:](numba.float64[:]))
+        def fft_top_hat(x):  # pragma: no cover
+            """
+            Fourier transform of 3D spherical top hat.
+
+            :param x: dimensionless parameter (usually k r)
+            :return t: Fourier transform of a 3D spherical top hat.
+            """
+
+            cutoff = 1e-8
+            # x values below thresh will yield a result abs smaller than cutoff:
+            thresh = np.sqrt(6 / cutoff)
+
+            t = np.zeros(len(x))
+
+            for i, y in enumerate(x):
+
+                if y > thresh:
+                    continue
+
+                elif y > 1e-2:
+                    t[i] = 3.0 * (np.sin(y) - y * np.cos(y)) / y**3.0
+                else:
+                    t[i] = 1.0 - y**2.0 / 10.0 + y**4.0 / 280.0
+
+            return t
+
         orig_shape = x.shape
         x_flat = np.ravel(x)
         t = fft_top_hat(x_flat)
         t = t.reshape(orig_shape)
 
         return t
 
@@ -758,52 +785,25 @@
         pk[:, mask_invalid] = np.nan
         if diag_only:
             return np.diag(pk)
         else:
             return pk
 
 
-@numba.jit(numba.float64[:](numba.float64[:]))
-def fft_top_hat(x):  # pragma: no cover
-    """
-    Fourier transform of 3D spherical top hat.
-
-    :param x: dimensionless parameter (usually k r)
-    :return t: Fourier transform of a 3D spherical top hat.
-    """
-
-    cutoff = 1e-8
-    # x values below thresh will yield a result abs smaller than cutoff:
-    thresh = np.sqrt(6 / cutoff)
-
-    t = np.zeros(len(x))
-
-    for i, y in enumerate(x):
-
-        if y > thresh:
-            continue
-
-        elif y > 1e-2:
-            t[i] = 3.0 * (np.sin(y) - y * np.cos(y)) / y**3.0
-        else:
-            t[i] = 1.0 - y**2.0 / 10.0 + y**4.0 / 280.0
-
-    return t
-
-
 def _u_km_slow(k, a, c, rv_mpc, nu_range, eta):
     """
     Fourier transform u(k,M) of the NFW profile, normed such that the integrated mass
     equals one.
 
     :param k: wavenumber [Mpc^-1]
     :param m_msun: halo mass in solar masses [Msun]
     :param a: scale factor
     :return ukm: Fourier Transform u(k,M) of the NFW profile [1]
     """
+    from scipy import special
 
     k = k[None, :, None] * nu_range[:, None, None] ** eta[None, None, :]
     nm, nk, __ = k.shape
     na = len(a)
 
     c = np.atleast_2d(c).T[:, None, :]
     rv_mpc = np.atleast_2d(rv_mpc).T[:, None, :]
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/NonLinearPerturbationTable.py` & `PyCosmo-2.1.1/src/PyCosmo/NonLinearPerturbationTable.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/Obs.py` & `PyCosmo-2.1.1/src/PyCosmo/Obs.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,25 +144,28 @@
         ]
 
     def nz(self, obsparams, nzmode=None, path2zdist=None):
         """
         Computes and normalises the redshift selection-function of a survey.
 
         :param obsparams: dictionary containing specifications for the observables
-        :param nzmode: string tag in [``smail``, ``cfhtlens``, ``custom``]
+        :param nzmode: string tag in [``smail``, ``cfhtlens``, ``custom``,
+                       ``custom_array``]
         :param path2zdist: if :math:`n(z)` comes from a file, then this is the path to
-                           the file
+                           the file (`nzmode` = ``custom``)
+                           if :math:`n(z)` comes from an array, this is the array
+                           (`nzmode` = ``custom_array``)
         :param z: redshift grid
         :return: Corresponding normalised redshift selection-function,
                  :math:`P(z)_{|norm}`.
         """
 
         # Todo need to think about default of a (like the Cosmo Class) or z?
 
-        distribution_type = ["smail", "cfhtlens", "custom"]
+        distribution_type = ["smail", "cfhtlens", "custom", "custom_array"]
 
         assert nzmode.lower() in distribution_type, (
             "The redshift distribution type in input parameters is not recognised."
             " Use one of the following: \n %s " % distribution_type
         )
 
         if nzmode.lower() == "smail":
@@ -187,14 +190,20 @@
 
         elif nzmode.lower() == "custom":
             datafile = np.genfromtxt(path2zdist)
 
             z = datafile[:, 0]
             pz = datafile[:, 1]
 
+        elif nzmode.lower() == "custom_array":
+            datafile = path2zdist
+
+            z = datafile[:, 0]
+            pz = datafile[:, 1]
+
         else:
             z = None
             pz = None
 
         if z is not None:
             norm = np.trapz(pz, z)
 
@@ -226,15 +235,15 @@
             nzmode = obsparams["nz"][i]
             if nzmode is not None:
                 print(
                     "Setting up galaxy selection function for {}.".format(
                         obsparams["probes"][i]
                     )
                 )
-                if nzmode in ["cfhtlens", "custom"]:
+                if nzmode in ["cfhtlens", "custom", "custom_array"]:
                     path2zdist = obsparams["path2zdist"][i]
                     z, selec = self.nz(obsparams, nzmode, path2zdist)
                 else:
                     z, selec = self.nz(obsparams, nzmode)
                 self.n[i] = interp1d(z, selec, bounds_error=False, fill_value=0.0)
             else:
                 self.n[i] = None
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/PerturbationBase.py` & `PyCosmo-2.1.1/src/PyCosmo/PerturbationBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     for name, method in clz._prototypes.items():
         if name not in clz.__dict__:
             raise RuntimeError(
                 "class {} implements no method for prototype {}.".format(clz, name)
             )
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            spec_tobe = inspect.getargspec(method)
-            spec_is = inspect.getargspec(clz.__dict__[name])
+            spec_tobe = inspect.getfullargspec(method)
+            spec_is = inspect.getfullargspec(clz.__dict__[name])
             if spec_tobe != spec_is:
                 # fix when decorated with @profile:
                 closure = clz.__dict__[name].__closure__
                 if closure:
                     for cell in closure:
                         if isinstance(cell.cell_contents, types.FunctionType):
                             spec_is = inspect.getargspec(cell.cell_contents)
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/PerturbationTable.py` & `PyCosmo-2.1.1/src/PyCosmo/PerturbationTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,14 @@
 
         lnk_grid = np.log(self._k_grid)
 
         min_a = np.max(self._perturbation.min_a(self._k_grid))
 
         valid_a = self._a_grid[self._a_grid > min_a]
 
-        # valid_a = np.concatenate(([min_a], valid_a))
-
         self._a_limits = (np.min(valid_a), np.max(valid_a))
         values = self._perturbation.powerspec_a_k(valid_a, self._k_grid)
         self._interpolator = RectBivariateSpline(
             np.log(valid_a),
             lnk_grid,
             np.log(values.T),
         )
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/Projection.py` & `PyCosmo-2.1.1/src/PyCosmo/Projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,16 @@
         :return: Integrand at :math:`\ell` for the values of a.
         """
 
         r = self.background.dist_trans_a(a=a)
         weightfunc = (
             weight_function1(a, self)
             * weight_function2(a, self)
-            / r ** 2
-            / a ** 2
+            / r**2
+            / a**2
             / self.background.H(a)
             * self.params.c
         )
 
         avec = np.tile(a, len(ells))
         weightvec = np.tile(weightfunc, len(ells))
         kvec = np.outer(ells, 1 / r).flatten()
@@ -191,19 +191,19 @@
         )
         # cl = np.trapz(intg_vec,a_vec)
         cls = np.trapz(intg_vec, a_vec, axis=1)
 
         cls *= (
             3.0
             * self.params.omega_m
-            * self.params.H0 ** 2
+            * self.params.H0**2
             * self.params.Tcmb
-            / self.params.c ** 2
+            / self.params.c**2
             * 1.0
-            / ell ** 2
+            / ell**2
         )
 
         return cls
 
     def cl_limber_ISW_int(
         self, a, ells, weight_function1, weight_function2, growth_ISW, perturb="linear"
     ):
@@ -294,16 +294,16 @@
         r = self.background.dist_trans_a(a=a)
         # For the second redshift selection functions, we need to transform a to z
         z = 1.0 / a - 1.0
         weightfunc = (
             weight_function1(a, self)
             * weight_function2(z)
             * F(a, self)
-            / r ** 2
-            / a ** 2
+            / r**2
+            / a**2
         )
 
         avec = np.tile(a, len(ells))
         weightvec = np.tile(weightfunc, len(ells))
         kvec = np.outer(ells, 1.0 / r).flatten()
 
         if IAmodel == "NLA":
@@ -365,16 +365,16 @@
         z = 1.0 / a - 1.0
         weightfunc = (
             self.background.H(a=a)
             / self.params.c
             * weight_function1(z)
             * weight_function2(z)
             * F(a, self) ** 2
-            / r ** 2
-            / a ** 2
+            / r**2
+            / a**2
         )
 
         avec = np.tile(a, len(ells))
         weightvec = np.tile(weightfunc, len(ells))
         kvec = np.outer(ells, 1.0 / r).flatten()
 
         if IAmodel == "NLA":
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/TheoryPredTables.py` & `PyCosmo-2.1.1/src/PyCosmo/TheoryPredTables.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_Cosmics.py` & `PyCosmo-2.1.1/src/PyCosmo/_Cosmics.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_Recombination.py` & `PyCosmo-2.1.1/src/PyCosmo/_Recombination.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_RecombinationClass.py` & `PyCosmo-2.1.1/src/PyCosmo/_RecombinationClass.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_RecombinationCosmics.py` & `PyCosmo-2.1.1/src/PyCosmo/_RecombinationCosmics.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_Tables.py` & `PyCosmo-2.1.1/src/PyCosmo/_Tables.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_Util.py` & `PyCosmo-2.1.1/src/PyCosmo/_Util.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/__init__.py` & `PyCosmo-2.1.1/src/PyCosmo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/_scipy_utils.py` & `PyCosmo-2.1.1/src/PyCosmo/_scipy_utils.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/build.py` & `PyCosmo-2.1.1/src/PyCosmo/build.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/__init__.py` & `PyCosmo-2.1.1/src/PyCosmo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_lcdm.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_mnulcdm.ini`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 omega_b = 0.06
 omega_m = 0.3
 omega_l =
 flat_universe = True
 n = 1.0
 Tcmb = 2.725
 Yp = 0.24
-N_massless_nu = 3.044
-N_massive_nu = 0
-massive_nu_total_mass = 0.0
+N_massless_nu = 0.00441
+N_massive_nu = 3.
+massive_nu_total_mass = 0.06
 wa = 0.0
 w0 = -1.0
 
 [computations]
 n_cores = 1
 
+[model_specific_parameters]
+T_mnu = 0.71611
+
 [recombination]
 recomb = recfast++
 recomb_dir =
 recomb_filename =
 F = 1.14
 fDM = 0.0
 
@@ -58,14 +61,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_lcdm_rsa.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_lcdm_rsa.ini`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_mnulcdm.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_mnulcdm_rsa.ini`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 w0 = -1.0
 
 [computations]
 n_cores = 1
 
 [model_specific_parameters]
 T_mnu = 0.71611
+rsa_trigger_taudot_eta = 5
+rsa_trigger_k_eta = 45
 
 [recombination]
 recomb = recfast++
 recomb_dir =
 recomb_filename =
 F = 1.14
 fDM = 0.0
@@ -61,14 +63,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_mnulcdm_rsa.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_mnuwcdm_rsa.ini`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 n = 1.0
 Tcmb = 2.725
 Yp = 0.24
 N_massless_nu = 0.00441
 N_massive_nu = 3.
 massive_nu_total_mass = 0.06
 wa = 0.0
-w0 = -1.0
+w0 = -0.95
 
 [computations]
 n_cores = 1
 
 [model_specific_parameters]
 T_mnu = 0.71611
+cs_de2 = 1.0
 rsa_trigger_taudot_eta = 5
 rsa_trigger_k_eta = 45
 
 [recombination]
 recomb = recfast++
 recomb_dir =
 recomb_filename =
@@ -63,14 +64,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_mnuwcdm.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_wcdm.ini`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 omega_b = 0.06
 omega_m = 0.3
 omega_l =
 flat_universe = True
 n = 1.0
 Tcmb = 2.725
 Yp = 0.24
-N_massless_nu = 0.00441
-N_massive_nu = 3.
-massive_nu_total_mass = 0.06
+N_massless_nu = 3.044
+N_massive_nu = 0.
+massive_nu_total_mass = 0.0
 wa = 0.0
 w0 = -0.95
 
 [computations]
 n_cores = 1
 
 [model_specific_parameters]
-T_mnu = 0.71611
 cs_de2 = 1.0
 
 [recombination]
 recomb = recfast++
 recomb_dir =
 recomb_filename =
 F = 1.14
@@ -62,14 +61,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
@@ -77,15 +77,15 @@
 [internal:comparison_modifications]
 omega_suppress = False
 suppress_rad = False
 cosmo_nudge = [1., 1., 1.]
 
 [internal:physical_constants]
 c = 299792.458  # [km/s]
-kb = 8.6173303e-5  # [eV/K]
+kb = 8.617333262e-5  # [eV/K]
 evc2 = 1.782661907e-36  # [kg] - eV/c^2
 G = 6.67408e-11  # [m^3/kg/s^2]
 hbar = 6.582119514e-16  # eV s
 mpc = 3.085677581491367e22  # [m]
 mp = 938.2720813  # [MeV/c**2]
 msun = 1.98848e30  # [kg]
 sigmat = 6.6524587158e-29  # [m**2]
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_mnuwcdm_rsa.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_wcdm_rsa.ini`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 omega_b = 0.06
 omega_m = 0.3
 omega_l =
 flat_universe = True
 n = 1.0
 Tcmb = 2.725
 Yp = 0.24
-N_massless_nu = 0.00441
-N_massive_nu = 3.
-massive_nu_total_mass = 0.06
+N_massless_nu = 3.044
+N_massive_nu = 0.
+massive_nu_total_mass = 0.0
 wa = 0.0
 w0 = -0.95
 
 [computations]
 n_cores = 1
 
 [model_specific_parameters]
-T_mnu = 0.71611
 cs_de2 = 1.0
 rsa_trigger_taudot_eta = 5
 rsa_trigger_k_eta = 45
 
 [recombination]
 recomb = recfast++
 recomb_dir =
@@ -64,14 +63,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
@@ -79,15 +79,15 @@
 [internal:comparison_modifications]
 omega_suppress = False
 suppress_rad = False
 cosmo_nudge = [1., 1., 1.]
 
 [internal:physical_constants]
 c = 299792.458  # [km/s]
-kb = 8.6173303e-5  # [eV/K]
+kb = 8.617333262e-5  # [eV/K]
 evc2 = 1.782661907e-36  # [kg] - eV/c^2
 G = 6.67408e-11  # [m^3/kg/s^2]
 hbar = 6.582119514e-16  # eV s
 mpc = 3.085677581491367e22  # [m]
 mp = 938.2720813  # [MeV/c**2]
 msun = 1.98848e30  # [kg]
 sigmat = 6.6524587158e-29  # [m**2]
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_wcdm.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_lcdm.ini`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 omega_m = 0.3
 omega_l =
 flat_universe = True
 n = 1.0
 Tcmb = 2.725
 Yp = 0.24
 N_massless_nu = 3.044
-N_massive_nu = 0.
+N_massive_nu = 0
 massive_nu_total_mass = 0.0
 wa = 0.0
-w0 = -0.95
+w0 = -1.0
 
 [computations]
 n_cores = 1
 
-[model_specific_parameters]
-cs_de2 = 1.0
-
 [recombination]
 recomb = recfast++
 recomb_dir =
 recomb_filename =
 F = 1.14
 fDM = 0.0
 
@@ -61,14 +58,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
@@ -76,15 +74,15 @@
 [internal:comparison_modifications]
 omega_suppress = False
 suppress_rad = False
 cosmo_nudge = [1., 1., 1.]
 
 [internal:physical_constants]
 c = 299792.458  # [km/s]
-kb = 8.617333262e-5  # [eV/K]
+kb = 8.6173303e-5  # [eV/K]
 evc2 = 1.782661907e-36  # [kg] - eV/c^2
 G = 6.67408e-11  # [m^3/kg/s^2]
 hbar = 6.582119514e-16  # eV s
 mpc = 3.085677581491367e22  # [m]
 mp = 938.2720813  # [MeV/c**2]
 msun = 1.98848e30  # [kg]
 sigmat = 6.6524587158e-29  # [m**2]
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/default_wcdm_rsa.ini` & `PyCosmo-2.1.1/src/PyCosmo/config/default_mnuwcdm.ini`

 * *Files 21% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 omega_b = 0.06
 omega_m = 0.3
 omega_l =
 flat_universe = True
 n = 1.0
 Tcmb = 2.725
 Yp = 0.24
-N_massless_nu = 3.044
-N_massive_nu = 0.
-massive_nu_total_mass = 0.0
+N_massless_nu = 0.00441
+N_massive_nu = 3.
+massive_nu_total_mass = 0.06
 wa = 0.0
 w0 = -0.95
 
 [computations]
 n_cores = 1
 
 [model_specific_parameters]
+T_mnu = 0.71611
 cs_de2 = 1.0
-rsa_trigger_taudot_eta = 5
-rsa_trigger_k_eta = 45
 
 [recombination]
 recomb = recfast++
 recomb_dir =
 recomb_filename =
 F = 1.14
 fDM = 0.0
@@ -63,14 +62,15 @@
 initial_conditions = class
 dt_0 = 1.5e-2
 sec_factor = 10.0
 boltzmann_rtol = 1e-5
 boltzmann_atol = 1e-5
 boltzmann_max_bdf_order = 5
 boltzmann_max_iter = 2000000
+boltzmann_h0 = 0.0
 fast_solver = True
 
 [internal:linear_perturbation_approx_growth_factor]
 ainit_growth=5e-2
 rtol_growth=1.49012e-8
 atol_growth=1.49012e-8
 h0_growth=0.0
@@ -78,15 +78,15 @@
 [internal:comparison_modifications]
 omega_suppress = False
 suppress_rad = False
 cosmo_nudge = [1., 1., 1.]
 
 [internal:physical_constants]
 c = 299792.458  # [km/s]
-kb = 8.617333262e-5  # [eV/K]
+kb = 8.6173303e-5  # [eV/K]
 evc2 = 1.782661907e-36  # [kg] - eV/c^2
 G = 6.67408e-11  # [m^3/kg/s^2]
 hbar = 6.582119514e-16  # eV s
 mpc = 3.085677581491367e22  # [m]
 mp = 938.2720813  # [MeV/c**2]
 msun = 1.98848e30  # [kg]
 sigmat = 6.6524587158e-29  # [m**2]
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/config/load_parameters_ini.py` & `PyCosmo-2.1.1/src/PyCosmo/config/load_parameters_ini.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU General Public License along with this
 # program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 from types import FunctionType
 
-import numpy as np
+from numpy import ndarray
 
 from ..ini_handling import Bunch, load_ini
 
 PYCOSMO_ROOT = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 
 INFO = {
@@ -69,14 +69,15 @@
         "initial_conditions": "Initical conditions",
         "dt_0": "User defined initial steps size",
         "sec_factor": "Security factor for LU permutations",
         "boltzmann_atol": "Boltzmann solver atol",
         "boltzmann_rtol": "Boltzmann solver rtol",
         "boltzmann_max_bdf_order": "LSODA max bdf order",
         "boltzmann_max_iter": "LSODA max iter",
+        "boltzmann_h0": "LSODA inital step size",
         "fast_solver": "Use fast LSODA solver",
     },
     "nonlinear_perturbations:mead": {
         "baryons": "",
         "multiplicity_fnct": "Multiplicity Function",
         "npoints_k": "Number of points for k grid",
         "A_mead": "",
@@ -137,15 +138,15 @@
         "recomb_dir": (None, str),
         "recomb_filename": (None, str),
         "F": float,
         "fDM": float,
     },
     "tabulation": {
         "tabulation": ["off", "bao", "manual", "default_precise", "default_fast"],
-        "tabulation_k_grid": (None, np.ndarray),
+        "tabulation_k_grid": (None, ndarray),
         "tabulation_max_k": (None, float),
         "tabulation_min_k": (None, float),
     },
     "linear_perturbations": {
         "pk_type": ["EH", "BBKS", "BBKS_CCL", "boltz"],
         "pk_norm_type": ["sigma8", "deltah", "A_s"],
         "pk_norm": float,
@@ -162,25 +163,29 @@
         "eta0_mead_equation": bool,
         "eta0_mead_equation_version": [1],
         "eta0_mead": float,
     },
     "internal:boltzmann_solver": {
         "table_size": int,
         "lna_0": (None, float),
-        "y_0": (None, np.ndarray),
+        "y_0": (None, ndarray),
         "initial_conditions": ["class", "cosmics", "camb"],
         "dt_0": (None, float),
         "sec_factor": lambda v: (
             isinstance(v, float) and v >= 1.0,
             "must be float >= 1.0",
         ),
-        "boltzmann_atol": (float, np.ndarray),
-        "boltzmann_rtol": (float, np.ndarray),
+        "boltzmann_atol": (float, ndarray),
+        "boltzmann_rtol": (float, ndarray),
         "boltzmann_max_bdf_order": (1, 2, 3, 4, 5),
         "boltzmann_max_iter": int,
+        "boltzmann_h0": lambda v: (
+            isinstance(v, float) and v >= 0.0,
+            "must be float >= 0.0",
+        ),
         "fast_solver": bool,
     },
     "internal:observables": {"k_size": int, "a_size": int},
     "internal:linear_perturbation_approx_growth_factor": {
         "ainit_growth": float,
         "rtol_growth": float,
         "atol_growth": float,
@@ -265,29 +270,29 @@
         return
 
     if isinstance(spec, (tuple, list)):
         for si in spec:
             if si is None:
                 if value is None:
                     return
-            elif si in (float, int, str, bool, np.ndarray):
+            elif si in (float, int, str, bool, ndarray):
                 if isinstance(value, si):
                     return
             elif si == value:
                 return
         raise ValueError(
             "{} has invalid value {}, allowed are {}.".format(key, value, spec)
         )
     elif spec is float:
         if not isinstance(value, (int, float)):
             raise ValueError(
                 "{} has invalid value {}, expected {}.".format(key, value, spec)
             )
 
-    elif spec in (int, str, bool, np.ndarray, list):
+    elif spec in (int, str, bool, ndarray, list):
         if not isinstance(value, spec):
             raise ValueError(
                 "{} has invalid value {}, expected {}.".format(key, value, spec)
             )
 
     elif isinstance(spec, FunctionType):
         ok, msg = spec(value)
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/core_file_handling.py` & `PyCosmo-2.1.1/src/PyCosmo/core_file_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,23 @@
 # program.  If not, see <http://www.gnu.org/licenses/>.
 
 import importlib
 import inspect
 import json
 import os
 import sys
+import types
 
 from sympy2c import Module
 
 
+def remove_globals(f):
+    return types.FunctionType(f.__code__, {}, argdefs=f.__defaults__)
+
+
 def load_core_files(paths, cosmology_config):
 
     if paths[0].endswith(".ipynb"):
         return extract_code_from_nb(paths, cosmology_config)
     elif paths[0].endswith(".py"):
         return extract_code_from_py(paths, cosmology_config)
     else:
@@ -94,14 +99,15 @@
     enrich_params = None
     for name, value in module.__dict__.items():
         if isinstance(
             value, (Function, Ode, OdeFast, OdeCombined, Globals, PythonFunction)
         ):
             m.add(value)
         if name.startswith("check"):
+            value = remove_globals(value)  # avoids pickling issues
             checks.append(value)
         if name == "enrich_params":
             enrich_params = value
 
     return m, checks, enrich_params
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/__init__.py` & `PyCosmo-2.1.1/src/PyCosmo/cython/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/const.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/const.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/constf.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/constf.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/halo_integral.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/halo_integral.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/PyCosmo/cython/sici.h"
         ],
@@ -23,16 +23,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -63,14 +63,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -99,18 +100,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -140,18 +145,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -163,15 +217,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -193,31 +247,34 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -509,35 +566,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -661,16 +718,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -943,17 +1002,17 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
   "src/PyCosmo/cython/halo_integral.pyx",
-  "venv/lib/python3.9/site-packages/numpy/__init__.pxd",
+  "__init__.pxd",
   "stringsource",
-  "venv/lib/python3.9/site-packages/Cython/Includes/cpython/type.pxd",
+  "type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
@@ -999,51 +1058,47 @@
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* Atomics.proto */
 #include <pythread.h>
 #ifndef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 1
 #endif
+#define __PYX_CYTHON_ATOMICS_ENABLED() CYTHON_ATOMICS
 #define __pyx_atomic_int_type int
-#if CYTHON_ATOMICS && __GNUC__ >= 4 && (__GNUC_MINOR__ > 1 ||\
-                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL >= 2)) &&\
-                    !defined(__i386__)
-    #define __pyx_atomic_incr_aligned(value, lock) __sync_fetch_and_add(value, 1)
-    #define __pyx_atomic_decr_aligned(value, lock) __sync_fetch_and_sub(value, 1)
+#if CYTHON_ATOMICS && (__GNUC__ >= 5 || (__GNUC__ == 4 &&\
+                    (__GNUC_MINOR__ > 1 ||\
+                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL__ >= 2))))
+    #define __pyx_atomic_incr_aligned(value) __sync_fetch_and_add(value, 1)
+    #define __pyx_atomic_decr_aligned(value) __sync_fetch_and_sub(value, 1)
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
-#elif CYTHON_ATOMICS && defined(_MSC_VER) && 0
-    #include <Windows.h>
+#elif CYTHON_ATOMICS && defined(_MSC_VER) && CYTHON_COMPILING_IN_NOGIL
+    #include <intrin.h>
     #undef __pyx_atomic_int_type
-    #define __pyx_atomic_int_type LONG
-    #define __pyx_atomic_incr_aligned(value, lock) InterlockedIncrement(value)
-    #define __pyx_atomic_decr_aligned(value, lock) InterlockedDecrement(value)
+    #define __pyx_atomic_int_type long
+    #pragma intrinsic (_InterlockedExchangeAdd)
+    #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
+    #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
-#elif CYTHON_ATOMICS && (defined(__ICC) || defined(__INTEL_COMPILER)) && 0
-    #define __pyx_atomic_incr_aligned(value, lock) _InterlockedIncrement(value)
-    #define __pyx_atomic_decr_aligned(value, lock) _InterlockedDecrement(value)
-    #ifdef __PYX_DEBUG_ATOMICS
-        #warning "Using Intel atomics"
-    #endif
 #else
     #undef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 0
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Not using atomics"
     #endif
 #endif
 typedef volatile __pyx_atomic_int_type __pyx_atomic_int;
 #if CYTHON_ATOMICS
     #define __pyx_add_acquisition_count(memview)\
-             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
+             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview))
     #define __pyx_sub_acquisition_count(memview)\
-            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
+            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview))
 #else
     #define __pyx_add_acquisition_count(memview)\
             __pyx_add_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
     #define __pyx_sub_acquisition_count(memview)\
             __pyx_sub_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
 #endif
 
@@ -1056,195 +1111,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1275,42 +1330,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1333,15 +1388,15 @@
   double *c_ptr;
   double *k_ptr;
   double *integrand;
   double *m_msun_ptr;
   double *rv_mpc_ptr;
 };
 
-/* "View.MemoryView":105
+/* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 struct __pyx_array_obj {
@@ -1358,28 +1413,28 @@
   PyObject *_format;
   void (*callback_free_data)(void *);
   int free_data;
   int dtype_is_object;
 };
 
 
-/* "View.MemoryView":279
+/* "View.MemoryView":280
  * 
  * @cname('__pyx_MemviewEnum')
  * cdef class Enum(object):             # <<<<<<<<<<<<<<
  *     cdef object name
  *     def __init__(self, name):
  */
 struct __pyx_MemviewEnum_obj {
   PyObject_HEAD
   PyObject *name;
 };
 
 
-/* "View.MemoryView":330
+/* "View.MemoryView":331
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 struct __pyx_memoryview_obj {
@@ -1394,15 +1449,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":967
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1411,29 +1466,29 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "View.MemoryView":105
+/* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 
 struct __pyx_vtabstruct_array {
   PyObject *(*get_memview)(struct __pyx_array_obj *);
 };
 static struct __pyx_vtabstruct_array *__pyx_vtabptr_array;
 
 
-/* "View.MemoryView":330
+/* "View.MemoryView":331
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 
@@ -1445,15 +1500,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":967
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -1581,26 +1636,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1624,14 +1679,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1946,14 +2007,20 @@
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyObject_GenericGetAttrNoDict.proto */
@@ -1978,20 +2045,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -2413,15 +2488,15 @@
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
@@ -2431,15 +2506,15 @@
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
@@ -2574,14 +2649,16 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
+static PyObject *__pyx_int_112105877;
+static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
@@ -2602,15 +2679,16 @@
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
 /* "PyCosmo/cython/halo_integral.pyx":23
  * @cython.wraparound(False)   # turn off negative index wrapping for entire function
  * @cython.cdivision(True)
  * cdef double trapez(double *x, double *y, size_t n) nogil:             # <<<<<<<<<<<<<<
  *     cdef double integral = 0.0
@@ -5391,15 +5469,15 @@
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5408,29 +5486,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5441,15 +5519,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5458,29 +5536,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5491,15 +5569,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5508,29 +5586,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5541,15 +5619,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5558,29 +5636,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5591,15 +5669,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5608,29 +5686,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5641,212 +5719,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5862,15 +5940,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5878,84 +5956,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5970,15 +6048,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5994,15 +6072,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6010,84 +6088,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6102,15 +6180,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6126,15 +6204,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6142,84 +6220,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6234,189 +6312,189 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":967
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":979
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":967
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":982
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":994
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":982
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":997
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":997
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1007
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1014
+/* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":122
+/* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -6460,21 +6538,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_itemsize)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(2, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(2, 123, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(2, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(2, 123, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -6482,15 +6560,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_allocate_buffer);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 122, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 123, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -6498,46 +6576,46 @@
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_shape = ((PyObject*)values[0]);
-    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 122, __pyx_L3_error)
+    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 123, __pyx_L3_error)
     __pyx_v_format = values[2];
     __pyx_v_mode = values[3];
     if (values[4]) {
-      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 123, __pyx_L3_error)
+      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 124, __pyx_L3_error)
     } else {
 
-      /* "View.MemoryView":123
+      /* "View.MemoryView":124
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 122, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 123, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.array.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(2, 122, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(2, 123, __pyx_L1_error)
   if (unlikely(((PyObject *)__pyx_v_format) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(2, 122, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(2, 123, __pyx_L1_error)
   }
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(((struct __pyx_array_obj *)__pyx_v_self), __pyx_v_shape, __pyx_v_itemsize, __pyx_v_format, __pyx_v_mode, __pyx_v_allocate_buffer);
 
-  /* "View.MemoryView":122
+  /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -6571,579 +6649,579 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_format);
 
-  /* "View.MemoryView":129
+  /* "View.MemoryView":130
  *         cdef PyObject **p
  * 
  *         self.ndim = <int> len(shape)             # <<<<<<<<<<<<<<
  *         self.itemsize = itemsize
  * 
  */
   if (unlikely(__pyx_v_shape == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(2, 129, __pyx_L1_error)
+    __PYX_ERR(2, 130, __pyx_L1_error)
   }
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 129, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 130, __pyx_L1_error)
   __pyx_v_self->ndim = ((int)__pyx_t_1);
 
-  /* "View.MemoryView":130
+  /* "View.MemoryView":131
  * 
  *         self.ndim = <int> len(shape)
  *         self.itemsize = itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not self.ndim:
  */
   __pyx_v_self->itemsize = __pyx_v_itemsize;
 
-  /* "View.MemoryView":132
+  /* "View.MemoryView":133
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_self->ndim != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":133
+    /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 133, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 133, __pyx_L1_error)
+    __PYX_ERR(2, 134, __pyx_L1_error)
 
-    /* "View.MemoryView":132
+    /* "View.MemoryView":133
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":135
+  /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   __pyx_t_2 = ((__pyx_v_itemsize <= 0) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":136
+    /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 136, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 136, __pyx_L1_error)
+    __PYX_ERR(2, 137, __pyx_L1_error)
 
-    /* "View.MemoryView":135
+    /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":138
+  /* "View.MemoryView":139
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_format); 
   __pyx_t_4 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":139
+    /* "View.MemoryView":140
  * 
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')             # <<<<<<<<<<<<<<
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 139, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_n_s_ASCII) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_ASCII);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 139, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_format, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":138
+    /* "View.MemoryView":139
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   }
 
-  /* "View.MemoryView":140
+  /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 140, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":141
+  /* "View.MemoryView":142
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format             # <<<<<<<<<<<<<<
  * 
  * 
  */
   if (unlikely(__pyx_v_self->_format == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(2, 141, __pyx_L1_error)
+    __PYX_ERR(2, 142, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(2, 141, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(2, 142, __pyx_L1_error)
   __pyx_v_self->format = __pyx_t_7;
 
-  /* "View.MemoryView":144
+  /* "View.MemoryView":145
  * 
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)             # <<<<<<<<<<<<<<
  *         self._strides = self._shape + self.ndim
  * 
  */
   __pyx_v_self->_shape = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * __pyx_v_self->ndim) * 2)));
 
-  /* "View.MemoryView":145
+  /* "View.MemoryView":146
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)
  *         self._strides = self._shape + self.ndim             # <<<<<<<<<<<<<<
  * 
  *         if not self._shape:
  */
   __pyx_v_self->_strides = (__pyx_v_self->_shape + __pyx_v_self->ndim);
 
-  /* "View.MemoryView":147
+  /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   __pyx_t_4 = ((!(__pyx_v_self->_shape != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "View.MemoryView":148
+    /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 148, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 148, __pyx_L1_error)
+    __PYX_ERR(2, 149, __pyx_L1_error)
 
-    /* "View.MemoryView":147
+    /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   }
 
-  /* "View.MemoryView":151
+  /* "View.MemoryView":152
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
   __pyx_t_8 = 0;
   __pyx_t_3 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
   for (;;) {
     if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(2, 151, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(2, 152, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 151, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 151, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 152, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_8;
     __pyx_t_8 = (__pyx_t_8 + 1);
 
-    /* "View.MemoryView":152
+    /* "View.MemoryView":153
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     __pyx_t_4 = ((__pyx_v_dim <= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":153
+      /* "View.MemoryView":154
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))             # <<<<<<<<<<<<<<
  *             self._shape[idx] = dim
  * 
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_6);
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 153, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(2, 153, __pyx_L1_error)
+      __PYX_ERR(2, 154, __pyx_L1_error)
 
-      /* "View.MemoryView":152
+      /* "View.MemoryView":153
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     }
 
-    /* "View.MemoryView":154
+    /* "View.MemoryView":155
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim             # <<<<<<<<<<<<<<
  * 
  *         cdef char order
  */
     (__pyx_v_self->_shape[__pyx_v_idx]) = __pyx_v_dim;
 
-    /* "View.MemoryView":151
+    /* "View.MemoryView":152
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":157
+  /* "View.MemoryView":158
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 157, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 158, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":158
+    /* "View.MemoryView":159
  *         cdef char order
  *         if mode == 'fortran':
  *             order = b'F'             # <<<<<<<<<<<<<<
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  */
     __pyx_v_order = 'F';
 
-    /* "View.MemoryView":159
+    /* "View.MemoryView":160
  *         if mode == 'fortran':
  *             order = b'F'
  *             self.mode = u'fortran'             # <<<<<<<<<<<<<<
  *         elif mode == 'c':
  *             order = b'C'
  */
     __Pyx_INCREF(__pyx_n_u_fortran);
     __Pyx_GIVEREF(__pyx_n_u_fortran);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_fortran;
 
-    /* "View.MemoryView":157
+    /* "View.MemoryView":158
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":160
+  /* "View.MemoryView":161
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 160, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 161, __pyx_L1_error)
   if (likely(__pyx_t_4)) {
 
-    /* "View.MemoryView":161
+    /* "View.MemoryView":162
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  *             order = b'C'             # <<<<<<<<<<<<<<
  *             self.mode = u'c'
  *         else:
  */
     __pyx_v_order = 'C';
 
-    /* "View.MemoryView":162
+    /* "View.MemoryView":163
  *         elif mode == 'c':
  *             order = b'C'
  *             self.mode = u'c'             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  */
     __Pyx_INCREF(__pyx_n_u_c);
     __Pyx_GIVEREF(__pyx_n_u_c);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_c;
 
-    /* "View.MemoryView":160
+    /* "View.MemoryView":161
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":164
+  /* "View.MemoryView":165
  *             self.mode = u'c'
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)             # <<<<<<<<<<<<<<
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 164, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 164, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_10, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __PYX_ERR(2, 164, __pyx_L1_error)
+    __PYX_ERR(2, 165, __pyx_L1_error)
   }
   __pyx_L10:;
 
-  /* "View.MemoryView":166
+  /* "View.MemoryView":167
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,             # <<<<<<<<<<<<<<
  *                                              itemsize, self.ndim, order)
  * 
  */
   __pyx_v_self->len = __pyx_fill_contig_strides_array(__pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_itemsize, __pyx_v_self->ndim, __pyx_v_order);
 
-  /* "View.MemoryView":169
+  /* "View.MemoryView":170
  *                                              itemsize, self.ndim, order)
  * 
  *         self.free_data = allocate_buffer             # <<<<<<<<<<<<<<
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:
  */
   __pyx_v_self->free_data = __pyx_v_allocate_buffer;
 
-  /* "View.MemoryView":170
+  /* "View.MemoryView":171
  * 
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'             # <<<<<<<<<<<<<<
  *         if allocate_buffer:
  * 
  */
-  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 170, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 170, __pyx_L1_error)
+  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 171, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_self->dtype_is_object = __pyx_t_4;
 
-  /* "View.MemoryView":171
+  /* "View.MemoryView":172
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = (__pyx_v_allocate_buffer != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":174
+    /* "View.MemoryView":175
  * 
  * 
  *             self.data = <char *>malloc(self.len)             # <<<<<<<<<<<<<<
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")
  */
     __pyx_v_self->data = ((char *)malloc(__pyx_v_self->len));
 
-    /* "View.MemoryView":175
+    /* "View.MemoryView":176
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     __pyx_t_4 = ((!(__pyx_v_self->data != 0)) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":176
+      /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 176, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(2, 176, __pyx_L1_error)
+      __PYX_ERR(2, 177, __pyx_L1_error)
 
-      /* "View.MemoryView":175
+      /* "View.MemoryView":176
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     }
 
-    /* "View.MemoryView":178
+    /* "View.MemoryView":179
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     __pyx_t_4 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":179
+      /* "View.MemoryView":180
  * 
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data             # <<<<<<<<<<<<<<
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  */
       __pyx_v_p = ((PyObject **)__pyx_v_self->data);
 
-      /* "View.MemoryView":180
+      /* "View.MemoryView":181
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):             # <<<<<<<<<<<<<<
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)
  */
       if (unlikely(__pyx_v_itemsize == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-        __PYX_ERR(2, 180, __pyx_L1_error)
+        __PYX_ERR(2, 181, __pyx_L1_error)
       }
       else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_self->len))) {
         PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-        __PYX_ERR(2, 180, __pyx_L1_error)
+        __PYX_ERR(2, 181, __pyx_L1_error)
       }
       __pyx_t_1 = __Pyx_div_Py_ssize_t(__pyx_v_self->len, __pyx_v_itemsize);
       __pyx_t_9 = __pyx_t_1;
       for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_9; __pyx_t_11+=1) {
         __pyx_v_i = __pyx_t_11;
 
-        /* "View.MemoryView":181
+        /* "View.MemoryView":182
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None             # <<<<<<<<<<<<<<
  *                     Py_INCREF(Py_None)
  * 
  */
         (__pyx_v_p[__pyx_v_i]) = Py_None;
 
-        /* "View.MemoryView":182
+        /* "View.MemoryView":183
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
         Py_INCREF(Py_None);
       }
 
-      /* "View.MemoryView":178
+      /* "View.MemoryView":179
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     }
 
-    /* "View.MemoryView":171
+    /* "View.MemoryView":172
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":122
+  /* "View.MemoryView":123
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -7159,15 +7237,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_format);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":185
+/* "View.MemoryView":186
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -7202,249 +7280,249 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":186
+  /* "View.MemoryView":187
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1             # <<<<<<<<<<<<<<
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
   __pyx_v_bufmode = -1;
 
-  /* "View.MemoryView":187
+  /* "View.MemoryView":188
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 187, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 188, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":188
+    /* "View.MemoryView":189
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
     __pyx_v_bufmode = (PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":187
+    /* "View.MemoryView":188
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":189
+  /* "View.MemoryView":190
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 189, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 190, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":190
+    /* "View.MemoryView":191
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  */
     __pyx_v_bufmode = (PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":189
+    /* "View.MemoryView":190
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":191
+  /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   __pyx_t_1 = ((!((__pyx_v_flags & __pyx_v_bufmode) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":192
+    /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 192, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 192, __pyx_L1_error)
+    __PYX_ERR(2, 193, __pyx_L1_error)
 
-    /* "View.MemoryView":191
+    /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   }
 
-  /* "View.MemoryView":193
+  /* "View.MemoryView":194
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data             # <<<<<<<<<<<<<<
  *         info.len = self.len
  *         info.ndim = self.ndim
  */
   __pyx_t_4 = __pyx_v_self->data;
   __pyx_v_info->buf = __pyx_t_4;
 
-  /* "View.MemoryView":194
+  /* "View.MemoryView":195
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  *         info.len = self.len             # <<<<<<<<<<<<<<
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  */
   __pyx_t_5 = __pyx_v_self->len;
   __pyx_v_info->len = __pyx_t_5;
 
-  /* "View.MemoryView":195
+  /* "View.MemoryView":196
  *         info.buf = self.data
  *         info.len = self.len
  *         info.ndim = self.ndim             # <<<<<<<<<<<<<<
  *         info.shape = self._shape
  *         info.strides = self._strides
  */
   __pyx_t_6 = __pyx_v_self->ndim;
   __pyx_v_info->ndim = __pyx_t_6;
 
-  /* "View.MemoryView":196
+  /* "View.MemoryView":197
  *         info.len = self.len
  *         info.ndim = self.ndim
  *         info.shape = self._shape             # <<<<<<<<<<<<<<
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  */
   __pyx_t_7 = __pyx_v_self->_shape;
   __pyx_v_info->shape = __pyx_t_7;
 
-  /* "View.MemoryView":197
+  /* "View.MemoryView":198
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  *         info.strides = self._strides             # <<<<<<<<<<<<<<
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  */
   __pyx_t_7 = __pyx_v_self->_strides;
   __pyx_v_info->strides = __pyx_t_7;
 
-  /* "View.MemoryView":198
+  /* "View.MemoryView":199
  *         info.shape = self._shape
  *         info.strides = self._strides
  *         info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *         info.itemsize = self.itemsize
  *         info.readonly = 0
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "View.MemoryView":199
+  /* "View.MemoryView":200
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize             # <<<<<<<<<<<<<<
  *         info.readonly = 0
  * 
  */
   __pyx_t_5 = __pyx_v_self->itemsize;
   __pyx_v_info->itemsize = __pyx_t_5;
 
-  /* "View.MemoryView":200
+  /* "View.MemoryView":201
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  *         info.readonly = 0             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   __pyx_v_info->readonly = 0;
 
-  /* "View.MemoryView":202
+  /* "View.MemoryView":203
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":203
+    /* "View.MemoryView":204
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_4 = __pyx_v_self->format;
     __pyx_v_info->format = __pyx_t_4;
 
-    /* "View.MemoryView":202
+    /* "View.MemoryView":203
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
     goto __pyx_L5;
   }
 
-  /* "View.MemoryView":205
+  /* "View.MemoryView":206
  *             info.format = self.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.obj = self
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L5:;
 
-  /* "View.MemoryView":207
+  /* "View.MemoryView":208
  *             info.format = NULL
  * 
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":185
+  /* "View.MemoryView":186
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -7466,15 +7544,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":211
+/* "View.MemoryView":212
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
@@ -7490,122 +7568,122 @@
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":212
+  /* "View.MemoryView":213
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
   __pyx_t_1 = ((__pyx_v_self->callback_free_data != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":213
+    /* "View.MemoryView":214
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)             # <<<<<<<<<<<<<<
  *         elif self.free_data:
  *             if self.dtype_is_object:
  */
     __pyx_v_self->callback_free_data(__pyx_v_self->data);
 
-    /* "View.MemoryView":212
+    /* "View.MemoryView":213
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":214
+  /* "View.MemoryView":215
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   __pyx_t_1 = (__pyx_v_self->free_data != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":215
+    /* "View.MemoryView":216
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":216
+      /* "View.MemoryView":217
  *         elif self.free_data:
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,             # <<<<<<<<<<<<<<
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_self->data, __pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_self->ndim, 0);
 
-      /* "View.MemoryView":215
+      /* "View.MemoryView":216
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     }
 
-    /* "View.MemoryView":218
+    /* "View.MemoryView":219
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  *             free(self.data)             # <<<<<<<<<<<<<<
  *         PyObject_Free(self._shape)
  * 
  */
     free(__pyx_v_self->data);
 
-    /* "View.MemoryView":214
+    /* "View.MemoryView":215
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":219
+  /* "View.MemoryView":220
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  *         PyObject_Free(self._shape)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   PyObject_Free(__pyx_v_self->_shape);
 
-  /* "View.MemoryView":211
+  /* "View.MemoryView":212
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":222
+/* "View.MemoryView":223
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -7627,29 +7705,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":223
+  /* "View.MemoryView":224
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 223, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":222
+  /* "View.MemoryView":223
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -7660,15 +7738,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":226
+/* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -7680,54 +7758,54 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_memview", 0);
 
-  /* "View.MemoryView":227
+  /* "View.MemoryView":228
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  */
   __pyx_v_flags = ((PyBUF_ANY_CONTIGUOUS | PyBUF_FORMAT) | PyBUF_WRITABLE);
 
-  /* "View.MemoryView":228
+  /* "View.MemoryView":229
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":226
+  /* "View.MemoryView":227
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -7740,15 +7818,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":230
+/* "View.MemoryView":231
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
@@ -7766,39 +7844,39 @@
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":231
+  /* "View.MemoryView":232
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
  */
   __pyx_r = (__pyx_v_self->_shape[0]);
   goto __pyx_L0;
 
-  /* "View.MemoryView":230
+  /* "View.MemoryView":231
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":233
+/* "View.MemoryView":234
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -7821,32 +7899,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 0);
 
-  /* "View.MemoryView":234
+  /* "View.MemoryView":235
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 234, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 234, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 235, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":233
+  /* "View.MemoryView":234
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -7858,15 +7936,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":236
+/* "View.MemoryView":237
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -7889,32 +7967,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":237
+  /* "View.MemoryView":238
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 237, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 237, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":236
+  /* "View.MemoryView":237
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -7926,15 +8004,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":239
+/* "View.MemoryView":240
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -7956,27 +8034,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
 
-  /* "View.MemoryView":240
+  /* "View.MemoryView":241
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 240, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(2, 240, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(2, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":239
+  /* "View.MemoryView":240
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -8101,15 +8179,15 @@
   __Pyx_AddTraceback("View.MemoryView.array.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":244
+/* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -8123,145 +8201,145 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("array_cwrapper", 0);
 
-  /* "View.MemoryView":248
+  /* "View.MemoryView":249
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_buf == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":249
+    /* "View.MemoryView":250
  * 
  *     if buf == NULL:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))             # <<<<<<<<<<<<<<
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_4);
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 249, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":248
+    /* "View.MemoryView":249
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":251
+  /* "View.MemoryView":252
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
   /*else*/ {
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":252
+    /* "View.MemoryView":253
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)             # <<<<<<<<<<<<<<
  *         result.data = buf
  * 
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 253, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(2, 252, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(2, 253, __pyx_L1_error)
 
-    /* "View.MemoryView":251
+    /* "View.MemoryView":252
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 251, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "View.MemoryView":253
+    /* "View.MemoryView":254
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)
  *         result.data = buf             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
     __pyx_v_result->data = __pyx_v_buf;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":255
+  /* "View.MemoryView":256
  *         result.data = buf
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":244
+  /* "View.MemoryView":245
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -8276,15 +8354,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":281
+/* "View.MemoryView":282
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
@@ -8313,26 +8391,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(2, 281, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(2, 282, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 281, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 282, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.Enum.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), __pyx_v_name);
 
@@ -8342,42 +8420,42 @@
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "View.MemoryView":282
+  /* "View.MemoryView":283
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
  */
   __Pyx_INCREF(__pyx_v_name);
   __Pyx_GIVEREF(__pyx_v_name);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = __pyx_v_name;
 
-  /* "View.MemoryView":281
+  /* "View.MemoryView":282
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":283
+/* "View.MemoryView":284
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -8395,27 +8473,27 @@
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":284
+  /* "View.MemoryView":285
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "View.MemoryView":283
+  /* "View.MemoryView":284
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -8690,15 +8768,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -8715,98 +8793,98 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":298
+/* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
 static void *__pyx_align_pointer(void *__pyx_v_memory, size_t __pyx_v_alignment) {
   Py_intptr_t __pyx_v_aligned_p;
   size_t __pyx_v_offset;
   void *__pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":300
+  /* "View.MemoryView":301
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory             # <<<<<<<<<<<<<<
  *     cdef size_t offset
  * 
  */
   __pyx_v_aligned_p = ((Py_intptr_t)__pyx_v_memory);
 
-  /* "View.MemoryView":304
+  /* "View.MemoryView":305
  * 
  *     with cython.cdivision(True):
  *         offset = aligned_p % alignment             # <<<<<<<<<<<<<<
  * 
  *     if offset > 0:
  */
   __pyx_v_offset = (__pyx_v_aligned_p % __pyx_v_alignment);
 
-  /* "View.MemoryView":306
+  /* "View.MemoryView":307
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   __pyx_t_1 = ((__pyx_v_offset > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":307
+    /* "View.MemoryView":308
  * 
  *     if offset > 0:
  *         aligned_p += alignment - offset             # <<<<<<<<<<<<<<
  * 
  *     return <void *> aligned_p
  */
     __pyx_v_aligned_p = (__pyx_v_aligned_p + (__pyx_v_alignment - __pyx_v_offset));
 
-    /* "View.MemoryView":306
+    /* "View.MemoryView":307
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   }
 
-  /* "View.MemoryView":309
+  /* "View.MemoryView":310
  *         aligned_p += alignment - offset
  * 
  *     return <void *> aligned_p             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((void *)__pyx_v_aligned_p);
   goto __pyx_L0;
 
-  /* "View.MemoryView":298
+  /* "View.MemoryView":299
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":345
+/* "View.MemoryView":346
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -8843,47 +8921,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(2, 345, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(2, 346, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype_is_object);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 345, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 346, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_obj = values[0];
-    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 345, __pyx_L3_error)
+    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 346, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 345, __pyx_L3_error)
+      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 346, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 345, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 346, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_obj, __pyx_v_flags, __pyx_v_dtype_is_object);
 
@@ -8900,37 +8978,37 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "View.MemoryView":346
+  /* "View.MemoryView":347
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  */
   __Pyx_INCREF(__pyx_v_obj);
   __Pyx_GIVEREF(__pyx_v_obj);
   __Pyx_GOTREF(__pyx_v_self->obj);
   __Pyx_DECREF(__pyx_v_self->obj);
   __pyx_v_self->obj = __pyx_v_obj;
 
-  /* "View.MemoryView":347
+  /* "View.MemoryView":348
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj
  *         self.flags = flags             # <<<<<<<<<<<<<<
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  */
   __pyx_v_self->flags = __pyx_v_flags;
 
-  /* "View.MemoryView":348
+  /* "View.MemoryView":349
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   __pyx_t_2 = (((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))) == ((PyObject *)__pyx_memoryview_type));
@@ -8942,231 +9020,250 @@
   }
   __pyx_t_3 = (__pyx_v_obj != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":349
+    /* "View.MemoryView":350
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)             # <<<<<<<<<<<<<<
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  */
-    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 349, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 350, __pyx_L1_error)
 
-    /* "View.MemoryView":350
+    /* "View.MemoryView":351
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     __pyx_t_1 = ((((PyObject *)__pyx_v_self->view.obj) == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":351
+      /* "View.MemoryView":352
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None             # <<<<<<<<<<<<<<
  *                 Py_INCREF(Py_None)
  * 
  */
       ((Py_buffer *)(&__pyx_v_self->view))->obj = Py_None;
 
-      /* "View.MemoryView":352
+      /* "View.MemoryView":353
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
- *         global __pyx_memoryview_thread_locks_used
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
  */
       Py_INCREF(Py_None);
 
-      /* "View.MemoryView":350
+      /* "View.MemoryView":351
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     }
 
-    /* "View.MemoryView":348
+    /* "View.MemoryView":349
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   }
 
   /* "View.MemoryView":355
+ *                 Py_INCREF(Py_None)
  * 
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
  */
-  __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
+  __pyx_t_1 = ((!(__PYX_CYTHON_ATOMICS_ENABLED() != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":356
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:
- */
-    __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
-
     /* "View.MemoryView":357
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  */
-    __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
+    __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
+    if (__pyx_t_1) {
 
-    /* "View.MemoryView":355
- * 
- *         global __pyx_memoryview_thread_locks_used
- *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
+      /* "View.MemoryView":358
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
+ *                 __pyx_memoryview_thread_locks_used += 1
+ *             if self.lock is NULL:
  */
-  }
+      __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
 
-  /* "View.MemoryView":358
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:             # <<<<<<<<<<<<<<
- *             self.lock = PyThread_allocate_lock()
+      /* "View.MemoryView":359
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
  *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
  */
-  __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-  if (__pyx_t_1) {
+      __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
 
-    /* "View.MemoryView":359
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
- *             if self.lock is NULL:
- *                 raise MemoryError
+      /* "View.MemoryView":357
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  */
-    __pyx_v_self->lock = PyThread_allocate_lock();
+    }
 
     /* "View.MemoryView":360
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 raise MemoryError
- * 
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
  */
     __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-    if (unlikely(__pyx_t_1)) {
+    if (__pyx_t_1) {
 
       /* "View.MemoryView":361
- *             self.lock = PyThread_allocate_lock()
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:
- *                 raise MemoryError             # <<<<<<<<<<<<<<
+ *                 self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
+ *                 if self.lock is NULL:
+ *                     raise MemoryError
+ */
+      __pyx_v_self->lock = PyThread_allocate_lock();
+
+      /* "View.MemoryView":362
+ *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *                     raise MemoryError
+ * 
+ */
+      __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
+      if (unlikely(__pyx_t_1)) {
+
+        /* "View.MemoryView":363
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
+ *                     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
-      PyErr_NoMemory(); __PYX_ERR(2, 361, __pyx_L1_error)
+        PyErr_NoMemory(); __PYX_ERR(2, 363, __pyx_L1_error)
+
+        /* "View.MemoryView":362
+ *             if self.lock is NULL:
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *                     raise MemoryError
+ * 
+ */
+      }
 
       /* "View.MemoryView":360
- *         if self.lock is NULL:
- *             self.lock = PyThread_allocate_lock()
+ *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *                 __pyx_memoryview_thread_locks_used += 1
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 raise MemoryError
- * 
+ *                 self.lock = PyThread_allocate_lock()
+ *                 if self.lock is NULL:
  */
     }
 
-    /* "View.MemoryView":358
- *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *             __pyx_memoryview_thread_locks_used += 1
- *         if self.lock is NULL:             # <<<<<<<<<<<<<<
- *             self.lock = PyThread_allocate_lock()
- *             if self.lock is NULL:
+    /* "View.MemoryView":355
+ *                 Py_INCREF(Py_None)
+ * 
+ *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
+ *             global __pyx_memoryview_thread_locks_used
+ *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
  */
   }
 
-  /* "View.MemoryView":363
- *                 raise MemoryError
+  /* "View.MemoryView":365
+ *                     raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":364
+    /* "View.MemoryView":366
  * 
  *         if flags & PyBUF_FORMAT:
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')             # <<<<<<<<<<<<<<
  *         else:
  *             self.dtype_is_object = dtype_is_object
  */
     __pyx_t_2 = (((__pyx_v_self->view.format[0]) == 'O') != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L11_bool_binop_done;
+      goto __pyx_L12_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_self->view.format[1]) == '\x00') != 0);
     __pyx_t_1 = __pyx_t_2;
-    __pyx_L11_bool_binop_done:;
+    __pyx_L12_bool_binop_done:;
     __pyx_v_self->dtype_is_object = __pyx_t_1;
 
-    /* "View.MemoryView":363
- *                 raise MemoryError
+    /* "View.MemoryView":365
+ *                     raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
-    goto __pyx_L10;
+    goto __pyx_L11;
   }
 
-  /* "View.MemoryView":366
+  /* "View.MemoryView":368
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  *             self.dtype_is_object = dtype_is_object             # <<<<<<<<<<<<<<
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  */
   /*else*/ {
     __pyx_v_self->dtype_is_object = __pyx_v_dtype_is_object;
   }
-  __pyx_L10:;
+  __pyx_L11:;
 
-  /* "View.MemoryView":368
+  /* "View.MemoryView":370
  *             self.dtype_is_object = dtype_is_object
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(             # <<<<<<<<<<<<<<
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL
  */
   __pyx_v_self->acquisition_count_aligned_p = ((__pyx_atomic_int *)__pyx_align_pointer(((void *)(&(__pyx_v_self->acquisition_count[0]))), (sizeof(__pyx_atomic_int))));
 
-  /* "View.MemoryView":370
+  /* "View.MemoryView":372
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(memoryview self):
  */
   __pyx_v_self->typeinfo = NULL;
 
-  /* "View.MemoryView":345
+  /* "View.MemoryView":346
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -9177,15 +9274,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":372
+/* "View.MemoryView":374
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
@@ -9208,215 +9305,215 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
   PyThread_type_lock __pyx_t_7;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":373
+  /* "View.MemoryView":375
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":374
+    /* "View.MemoryView":376
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  */
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
-    /* "View.MemoryView":373
+    /* "View.MemoryView":375
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":375
+  /* "View.MemoryView":377
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":377
+    /* "View.MemoryView":379
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
  *             Py_DECREF(Py_None)
  * 
  */
     ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
 
-    /* "View.MemoryView":378
+    /* "View.MemoryView":380
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *         cdef int i
  */
     Py_DECREF(Py_None);
 
-    /* "View.MemoryView":375
+    /* "View.MemoryView":377
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":382
+  /* "View.MemoryView":384
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":383
+    /* "View.MemoryView":385
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":384
+      /* "View.MemoryView":386
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":385
+        /* "View.MemoryView":387
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":388
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":390
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":387
+          /* "View.MemoryView":389
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":386
+          /* "View.MemoryView":388
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":389
+        /* "View.MemoryView":391
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":384
+        /* "View.MemoryView":386
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":391
+      /* "View.MemoryView":393
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":382
+    /* "View.MemoryView":384
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
 
-  /* "View.MemoryView":372
+  /* "View.MemoryView":374
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":393
+/* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -9434,107 +9531,107 @@
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":397
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":399
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 397, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 397, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 399, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 399, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 399, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 399, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 397, __pyx_L1_error)
+          else __PYX_ERR(2, 399, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":398
+    /* "View.MemoryView":400
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 398, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(2, 398, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 400, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(2, 400, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":397
+    /* "View.MemoryView":399
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":400
+  /* "View.MemoryView":402
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":395
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -9546,15 +9643,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":403
+/* "View.MemoryView":405
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -9584,143 +9681,143 @@
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":404
+  /* "View.MemoryView":406
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":405
+    /* "View.MemoryView":407
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":404
+    /* "View.MemoryView":406
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":407
+  /* "View.MemoryView":409
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 407, __pyx_L1_error)
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(2, 407, __pyx_L1_error)
+      __PYX_ERR(2, 409, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 407, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 407, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 407, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 409, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":410
+  /* "View.MemoryView":412
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 412, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":411
+    /* "View.MemoryView":413
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 411, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":410
+    /* "View.MemoryView":412
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":413
+  /* "View.MemoryView":415
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(2, 413, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(2, 415, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":414
+    /* "View.MemoryView":416
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 414, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":403
+  /* "View.MemoryView":405
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -9735,15 +9832,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":416
+/* "View.MemoryView":418
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -9771,182 +9868,182 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":417
+  /* "View.MemoryView":419
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":418
+    /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 418, __pyx_L1_error)
+    __PYX_ERR(2, 420, __pyx_L1_error)
 
-    /* "View.MemoryView":417
+    /* "View.MemoryView":419
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":422
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(2, 420, __pyx_L1_error)
+      __PYX_ERR(2, 422, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 420, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 422, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":424
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 422, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 424, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":423
+    /* "View.MemoryView":425
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 423, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":426
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 424, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 426, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":425
+      /* "View.MemoryView":427
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 425, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":424
+      /* "View.MemoryView":426
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":427
+    /* "View.MemoryView":429
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(2, 427, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 427, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(2, 429, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":422
+    /* "View.MemoryView":424
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":429
+  /* "View.MemoryView":431
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 429, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 431, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":416
+  /* "View.MemoryView":418
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -9963,15 +10060,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":431
+/* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -9989,26 +10086,26 @@
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":432
+  /* "View.MemoryView":434
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":433
+    /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
     {
@@ -10016,59 +10113,59 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":436
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 434, __pyx_L4_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":437
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 435, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 437, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":436
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 434, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 434, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 436, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":433
+        /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -10077,30 +10174,30 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":436
+      /* "View.MemoryView":438
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(2, 436, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(2, 438, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":439
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
         __Pyx_XDECREF(__pyx_r);
@@ -10109,15 +10206,15 @@
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":433
+      /* "View.MemoryView":435
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -10130,36 +10227,36 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":432
+    /* "View.MemoryView":434
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":439
+  /* "View.MemoryView":441
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":433
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -10173,15 +10270,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":441
+/* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -10197,60 +10294,60 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":447
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(2, 445, __pyx_L1_error)
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 445, __pyx_L1_error)
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 447, __pyx_L1_error)
 
-  /* "View.MemoryView":446
+  /* "View.MemoryView":448
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(2, 446, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 446, __pyx_L1_error)
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(2, 448, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 448, __pyx_L1_error)
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":449
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":447
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 445, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 447, __pyx_L1_error)
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":443
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -10263,15 +10360,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":449
+/* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -10296,204 +10393,204 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":453
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":456
+  /* "View.MemoryView":458
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 456, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 458, __pyx_L1_error)
   __pyx_v_dst_slice = __pyx_t_1;
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":460
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
   __pyx_t_2 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":459
+    /* "View.MemoryView":461
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":462
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     __pyx_t_2 = ((__pyx_v_tmp == NULL) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":461
+      /* "View.MemoryView":463
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      PyErr_NoMemory(); __PYX_ERR(2, 461, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(2, 463, __pyx_L1_error)
 
-      /* "View.MemoryView":460
+      /* "View.MemoryView":462
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":464
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":458
+    /* "View.MemoryView":460
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":464
+  /* "View.MemoryView":466
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":468
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
   /*try:*/ {
 
-    /* "View.MemoryView":467
+    /* "View.MemoryView":469
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
     __pyx_t_2 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":468
+      /* "View.MemoryView":470
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":467
+      /* "View.MemoryView":469
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":470
+    /* "View.MemoryView":472
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 470, __pyx_L6_error)
+      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 472, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":474
+    /* "View.MemoryView":476
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     __pyx_t_2 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":475
+      /* "View.MemoryView":477
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 475, __pyx_L6_error)
+      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 477, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "View.MemoryView":474
+      /* "View.MemoryView":476
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":478
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":479
+  /* "View.MemoryView":481
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
   /*finally:*/ {
@@ -10532,15 +10629,15 @@
       __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_6;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":451
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -10553,15 +10650,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":481
+/* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -10572,36 +10669,36 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
-  /* "View.MemoryView":482
+  /* "View.MemoryView":484
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(2, 482, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(2, 484, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":485
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 483, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":483
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -10614,15 +10711,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":485
+/* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10644,39 +10741,39 @@
   size_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":488
+  /* "View.MemoryView":490
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 488, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":491
+  /* "View.MemoryView":493
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 491, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":492
+  /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
   {
@@ -10684,24 +10781,24 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":493
+      /* "View.MemoryView":495
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 493, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 495, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 493, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -10710,94 +10807,94 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":492
+      /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":497
+    /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":498
+        /* "View.MemoryView":500
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 498, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 500, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":497
+        /* "View.MemoryView":499
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":499
+      /* "View.MemoryView":501
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -10808,52 +10905,52 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":496
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 494, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 496, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(2, 494, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(2, 496, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(2, 495, __pyx_L5_except_error)
+      __PYX_ERR(2, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":492
+    /* "View.MemoryView":494
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -10865,15 +10962,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":487
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10891,15 +10988,15 @@
   __Pyx_XDECREF(__pyx_v_bytesitem);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":501
+/* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -10925,88 +11022,88 @@
   char *__pyx_t_13;
   char *__pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":504
+  /* "View.MemoryView":506
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 504, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":509
+  /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":510
+    /* "View.MemoryView":512
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 510, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":509
+    /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":512
+  /* "View.MemoryView":514
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -11015,102 +11112,102 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(2, 514, __pyx_L1_error)
+    __PYX_ERR(2, 516, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":517
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":514
+    /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":517
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":503
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -11130,15 +11227,15 @@
   __Pyx_XDECREF(__pyx_v_struct);
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":518
+/* "View.MemoryView":520
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -11173,15 +11270,15 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":519
+  /* "View.MemoryView":521
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
@@ -11191,268 +11288,268 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":520
+    /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 520, __pyx_L1_error)
+    __PYX_ERR(2, 522, __pyx_L1_error)
 
-    /* "View.MemoryView":519
+    /* "View.MemoryView":521
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":524
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":523
+    /* "View.MemoryView":525
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":524
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":525
+  /* "View.MemoryView":527
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":529
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":528
+    /* "View.MemoryView":530
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":527
+    /* "View.MemoryView":529
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":530
+  /* "View.MemoryView":532
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":534
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":533
+    /* "View.MemoryView":535
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":532
+    /* "View.MemoryView":534
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":535
+  /* "View.MemoryView":537
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":539
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":538
+    /* "View.MemoryView":540
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":537
+    /* "View.MemoryView":539
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":540
+  /* "View.MemoryView":542
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":544
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":543
+  /* "View.MemoryView":545
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":546
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":547
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":548
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":549
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":518
+  /* "View.MemoryView":520
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -11474,15 +11571,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":553
+/* "View.MemoryView":555
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -11506,49 +11603,49 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":554
+  /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 554, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(2, 554, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(2, 556, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":557
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 555, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 557, __pyx_L1_error)
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":558
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":553
+  /* "View.MemoryView":555
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -11560,15 +11657,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":559
+/* "View.MemoryView":561
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -11586,42 +11683,42 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":560
+  /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":559
+  /* "View.MemoryView":561
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":563
+/* "View.MemoryView":565
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -11648,41 +11745,41 @@
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":564
+  /* "View.MemoryView":566
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 564, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 564, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 564, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 566, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 564, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":563
+  /* "View.MemoryView":565
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -11694,15 +11791,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":567
+/* "View.MemoryView":569
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -11730,73 +11827,73 @@
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":568
+  /* "View.MemoryView":570
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 570, __pyx_L1_error)
+    __PYX_ERR(2, 572, __pyx_L1_error)
 
-    /* "View.MemoryView":568
+    /* "View.MemoryView":570
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":574
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(2, 572, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(2, 574, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":567
+  /* "View.MemoryView":569
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -11808,15 +11905,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":575
+/* "View.MemoryView":577
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -11844,77 +11941,77 @@
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":576
+  /* "View.MemoryView":578
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":577
+    /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":576
+    /* "View.MemoryView":578
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":581
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 581, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(2, 579, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(2, 581, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":575
+  /* "View.MemoryView":577
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -11926,15 +12023,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":582
+/* "View.MemoryView":584
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -11956,29 +12053,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":583
+  /* "View.MemoryView":585
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 583, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":582
+  /* "View.MemoryView":584
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -11989,15 +12086,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":586
+/* "View.MemoryView":588
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -12019,29 +12116,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":587
+  /* "View.MemoryView":589
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 587, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":586
+  /* "View.MemoryView":588
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -12052,15 +12149,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":590
+/* "View.MemoryView":592
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -12084,35 +12181,35 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":591
+  /* "View.MemoryView":593
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 591, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 591, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":590
+  /* "View.MemoryView":592
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -12125,15 +12222,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":594
+/* "View.MemoryView":596
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -12162,98 +12259,98 @@
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":595
+  /* "View.MemoryView":597
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":596
+    /* "View.MemoryView":598
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":600
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 598, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 600, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":599
+      /* "View.MemoryView":601
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 599, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 601, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":601
+    /* "View.MemoryView":603
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":595
+    /* "View.MemoryView":597
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":603
+  /* "View.MemoryView":605
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":594
+  /* "View.MemoryView":596
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -12266,15 +12363,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":605
+/* "View.MemoryView":607
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -12293,68 +12390,68 @@
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":606
+  /* "View.MemoryView":608
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":607
+    /* "View.MemoryView":609
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":606
+    /* "View.MemoryView":608
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":609
+  /* "View.MemoryView":611
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":607
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":611
+/* "View.MemoryView":613
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -12378,64 +12475,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":614
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":615
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 613, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":614
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":613
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -12448,15 +12545,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":615
+/* "View.MemoryView":617
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -12479,43 +12576,43 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "View.MemoryView":616
+  /* "View.MemoryView":618
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":617
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -12527,15 +12624,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":619
+/* "View.MemoryView":621
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12560,39 +12657,39 @@
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
-  /* "View.MemoryView":622
+  /* "View.MemoryView":624
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 622, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 624, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":623
+  /* "View.MemoryView":625
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 623, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":619
+  /* "View.MemoryView":621
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12603,15 +12700,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":625
+/* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12636,39 +12733,39 @@
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
-  /* "View.MemoryView":628
+  /* "View.MemoryView":630
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 628, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 630, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":629
+  /* "View.MemoryView":631
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 629, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -12679,15 +12776,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":631
+/* "View.MemoryView":633
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -12712,57 +12809,57 @@
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":635
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":637
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":636
+  /* "View.MemoryView":638
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 636, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 638, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":641
+  /* "View.MemoryView":643
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 641, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":633
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -12773,15 +12870,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":643
+/* "View.MemoryView":645
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -12807,57 +12904,57 @@
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":647
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":649
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":648
+  /* "View.MemoryView":650
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 648, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 650, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":653
+  /* "View.MemoryView":655
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 653, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":645
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -12981,15 +13078,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":657
+/* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -13001,64 +13098,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
-  /* "View.MemoryView":658
+  /* "View.MemoryView":660
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":661
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":662
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -13072,54 +13169,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":663
+/* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
 
-  /* "View.MemoryView":664
+  /* "View.MemoryView":666
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":665
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":666
+/* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -13145,243 +13242,243 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
-  /* "View.MemoryView":671
+  /* "View.MemoryView":673
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":672
+    /* "View.MemoryView":674
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 672, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 674, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":671
+    /* "View.MemoryView":673
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":674
+  /* "View.MemoryView":676
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":678
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 676, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":677
+  /* "View.MemoryView":679
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":680
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":681
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 679, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 679, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 681, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 681, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 681, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 679, __pyx_L1_error)
+          else __PYX_ERR(2, 681, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":680
+    /* "View.MemoryView":682
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":681
+      /* "View.MemoryView":683
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":682
+        /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 682, __pyx_L1_error)
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__17);
             __Pyx_GIVEREF(__pyx_slice__17);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__17);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":685
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":681
+        /* "View.MemoryView":683
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":685
+      /* "View.MemoryView":687
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":686
+      /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":680
+      /* "View.MemoryView":682
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":688
+    /* "View.MemoryView":690
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
     /*else*/ {
@@ -13393,40 +13490,40 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":689
+        /* "View.MemoryView":691
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 689, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 691, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 689, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 691, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(2, 689, __pyx_L1_error)
+        __PYX_ERR(2, 691, __pyx_L1_error)
 
-        /* "View.MemoryView":688
+        /* "View.MemoryView":690
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":691
+      /* "View.MemoryView":693
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
       __pyx_t_10 = (__pyx_v_have_slices != 0);
@@ -13437,120 +13534,120 @@
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":692
+      /* "View.MemoryView":694
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 692, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 694, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":679
+    /* "View.MemoryView":681
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":694
+  /* "View.MemoryView":696
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(2, 694, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":695
+  /* "View.MemoryView":697
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":696
+    /* "View.MemoryView":698
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 696, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__17);
         __Pyx_GIVEREF(__pyx_slice__17);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__17);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":695
+    /* "View.MemoryView":697
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":698
+  /* "View.MemoryView":700
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 698, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":668
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -13568,15 +13665,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":700
+/* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -13590,60 +13687,60 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
-  /* "View.MemoryView":701
+  /* "View.MemoryView":703
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":702
+    /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":703
+      /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(2, 703, __pyx_L1_error)
+      __PYX_ERR(2, 705, __pyx_L1_error)
 
-      /* "View.MemoryView":702
+      /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":702
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -13656,15 +13753,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":710
+/* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -13700,529 +13797,529 @@
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
-  /* "View.MemoryView":711
+  /* "View.MemoryView":713
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":718
+  /* "View.MemoryView":720
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":722
+  /* "View.MemoryView":724
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(2, 722, __pyx_L1_error)
+      __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":726
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":725
+    /* "View.MemoryView":727
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 725, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 727, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":728
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":724
+    /* "View.MemoryView":726
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":728
+  /* "View.MemoryView":730
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":729
+    /* "View.MemoryView":731
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":735
+  /* "View.MemoryView":737
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":736
+  /* "View.MemoryView":738
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":741
+  /* "View.MemoryView":743
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":742
+  /* "View.MemoryView":744
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":746
+  /* "View.MemoryView":748
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 746, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 746, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 748, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 748, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 748, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 748, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 748, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 746, __pyx_L1_error)
+          else __PYX_ERR(2, 748, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":747
+    /* "View.MemoryView":749
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":751
+      /* "View.MemoryView":753
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 751, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 753, __pyx_L1_error)
 
-      /* "View.MemoryView":748
+      /* "View.MemoryView":750
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 748, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 750, __pyx_L1_error)
 
-      /* "View.MemoryView":747
+      /* "View.MemoryView":749
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":754
+    /* "View.MemoryView":756
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":755
+      /* "View.MemoryView":757
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":758
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":759
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":760
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":754
+      /* "View.MemoryView":756
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":760
+    /* "View.MemoryView":762
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 760, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 760, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 762, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 760, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 762, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":761
+      /* "View.MemoryView":763
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 761, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 763, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 763, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 761, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 763, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":762
+      /* "View.MemoryView":764
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 762, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 764, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 764, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 764, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":766
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 764, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 766, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":765
+      /* "View.MemoryView":767
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 765, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 767, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":768
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 766, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 768, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":770
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 768, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 770, __pyx_L1_error)
 
-      /* "View.MemoryView":774
+      /* "View.MemoryView":776
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":746
+    /* "View.MemoryView":748
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":776
+  /* "View.MemoryView":778
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":779
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":780
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 778, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 780, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":781
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 779, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 781, __pyx_L1_error) }
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":779
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 777, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 777, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 779, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":776
+    /* "View.MemoryView":778
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":782
+  /* "View.MemoryView":784
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":783
+    /* "View.MemoryView":785
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 782, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":782
+    /* "View.MemoryView":784
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 782, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 784, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":712
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -14236,15 +14333,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_memviewsliceobj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":807
+/* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -14255,95 +14352,95 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":827
+  /* "View.MemoryView":829
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":831
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":830
+      /* "View.MemoryView":832
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":829
+      /* "View.MemoryView":831
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":833
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":834
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 832, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 834, __pyx_L1_error)
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":833
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":827
+    /* "View.MemoryView":829
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":835
+  /* "View.MemoryView":837
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
   /*else*/ {
@@ -14354,15 +14451,15 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":837
+    /* "View.MemoryView":839
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     __pyx_t_1 = (__pyx_v_have_step != 0);
@@ -14372,639 +14469,639 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":838
+      /* "View.MemoryView":840
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 838, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 840, __pyx_L1_error)
 
-      /* "View.MemoryView":837
+      /* "View.MemoryView":839
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":841
+    /* "View.MemoryView":843
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":842
+      /* "View.MemoryView":844
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":843
+        /* "View.MemoryView":845
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":846
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":845
+          /* "View.MemoryView":847
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":844
+          /* "View.MemoryView":846
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":842
+        /* "View.MemoryView":844
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":846
+      /* "View.MemoryView":848
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":847
+        /* "View.MemoryView":849
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":848
+          /* "View.MemoryView":850
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":849
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":850
+        /* "View.MemoryView":852
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":848
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":841
+      /* "View.MemoryView":843
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":852
+    /* "View.MemoryView":854
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":853
+        /* "View.MemoryView":855
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":854
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":855
+      /* "View.MemoryView":857
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":857
+    /* "View.MemoryView":859
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":858
+      /* "View.MemoryView":860
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":859
+        /* "View.MemoryView":861
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":862
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":861
+          /* "View.MemoryView":863
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":860
+          /* "View.MemoryView":862
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":858
+        /* "View.MemoryView":860
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":862
+      /* "View.MemoryView":864
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":863
+        /* "View.MemoryView":865
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":864
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":859
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":865
+    /* "View.MemoryView":867
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":866
+        /* "View.MemoryView":868
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":867
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":868
+      /* "View.MemoryView":870
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":870
+    /* "View.MemoryView":872
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":871
+      /* "View.MemoryView":873
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":872
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":875
+    /* "View.MemoryView":877
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":879
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":878
+      /* "View.MemoryView":880
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":877
+      /* "View.MemoryView":879
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":880
+    /* "View.MemoryView":882
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":881
+      /* "View.MemoryView":883
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":882
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":884
+    /* "View.MemoryView":886
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":885
+    /* "View.MemoryView":887
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":888
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":889
+  /* "View.MemoryView":891
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":890
+    /* "View.MemoryView":892
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":889
+    /* "View.MemoryView":891
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":892
+  /* "View.MemoryView":894
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":896
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":895
+    /* "View.MemoryView":897
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":896
+      /* "View.MemoryView":898
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":897
+        /* "View.MemoryView":899
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":896
+        /* "View.MemoryView":898
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":899
+      /* "View.MemoryView":901
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
       /*else*/ {
 
-        /* "View.MemoryView":900
+        /* "View.MemoryView":902
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 899, __pyx_L1_error)
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 901, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":895
+      /* "View.MemoryView":897
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":902
+    /* "View.MemoryView":904
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":894
+    /* "View.MemoryView":896
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":904
+  /* "View.MemoryView":906
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":809
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -15020,15 +15117,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":910
+/* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -15045,280 +15142,280 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":914
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":913
+  /* "View.MemoryView":915
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":916
+  /* "View.MemoryView":918
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":917
+    /* "View.MemoryView":919
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(2, 917, __pyx_L1_error)
+      __PYX_ERR(2, 919, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(2, 917, __pyx_L1_error)
+      __PYX_ERR(2, 919, __pyx_L1_error)
     }
     __pyx_v_shape = __Pyx_div_Py_ssize_t(__pyx_v_view->len, __pyx_v_itemsize);
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":920
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":916
+    /* "View.MemoryView":918
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":920
+  /* "View.MemoryView":922
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":921
+    /* "View.MemoryView":923
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":922
+    /* "View.MemoryView":924
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":923
+      /* "View.MemoryView":925
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":922
+      /* "View.MemoryView":924
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":925
+  /* "View.MemoryView":927
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":926
+    /* "View.MemoryView":928
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":929
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":928
+      /* "View.MemoryView":930
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 928, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 928, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 928, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 930, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 928, __pyx_L1_error)
+      __PYX_ERR(2, 930, __pyx_L1_error)
 
-      /* "View.MemoryView":927
+      /* "View.MemoryView":929
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":925
+    /* "View.MemoryView":927
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":930
+  /* "View.MemoryView":932
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":931
+    /* "View.MemoryView":933
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 931, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 931, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 931, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 933, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 931, __pyx_L1_error)
+    __PYX_ERR(2, 933, __pyx_L1_error)
 
-    /* "View.MemoryView":930
+    /* "View.MemoryView":932
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":933
+  /* "View.MemoryView":935
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":934
+  /* "View.MemoryView":936
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":935
+    /* "View.MemoryView":937
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":934
+    /* "View.MemoryView":936
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":937
+  /* "View.MemoryView":939
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":912
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -15329,15 +15426,15 @@
   __Pyx_AddTraceback("View.MemoryView.pybuffer_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":943
+/* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -15357,90 +15454,90 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":944
+  /* "View.MemoryView":946
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":948
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":947
+  /* "View.MemoryView":949
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":951
+  /* "View.MemoryView":953
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
   __pyx_t_3 = __Pyx_div_long(__pyx_v_ndim, 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":952
+    /* "View.MemoryView":954
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":953
+    /* "View.MemoryView":955
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":956
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":958
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
@@ -15450,44 +15547,44 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":957
+      /* "View.MemoryView":959
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 957, __pyx_L1_error)
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 959, __pyx_L1_error)
 
-      /* "View.MemoryView":956
+      /* "View.MemoryView":958
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":959
+  /* "View.MemoryView":961
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":945
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -15503,15 +15600,15 @@
     #endif
   }
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":976
+/* "View.MemoryView":978
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -15526,36 +15623,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":977
+  /* "View.MemoryView":979
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":976
+  /* "View.MemoryView":978
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":979
+/* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -15565,64 +15662,64 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":980
+  /* "View.MemoryView":982
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":981
+    /* "View.MemoryView":983
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 981, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 983, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":980
+    /* "View.MemoryView":982
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":983
+  /* "View.MemoryView":985
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 985, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":981
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -15633,15 +15730,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":985
+/* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -15652,58 +15749,58 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":986
+  /* "View.MemoryView":988
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":987
+    /* "View.MemoryView":989
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 987, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 989, __pyx_L1_error)
 
-    /* "View.MemoryView":986
+    /* "View.MemoryView":988
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":989
+  /* "View.MemoryView":991
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 989, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 991, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":987
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -15716,15 +15813,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":992
+/* "View.MemoryView":994
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -15742,27 +15839,27 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":993
+  /* "View.MemoryView":995
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":992
+  /* "View.MemoryView":994
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -15882,15 +15979,15 @@
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":999
+/* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -15910,351 +16007,351 @@
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
-  /* "View.MemoryView":1007
+  /* "View.MemoryView":1009
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1008
+    /* "View.MemoryView":1010
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1007
+    /* "View.MemoryView":1009
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1013
+  /* "View.MemoryView":1015
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1013, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1015, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1017
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1016
+  /* "View.MemoryView":1018
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1020
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1018, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1020, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1019
+  /* "View.MemoryView":1021
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1023
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1022
+  /* "View.MemoryView":1024
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1025
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1026
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1027
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1029
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1028
+    /* "View.MemoryView":1030
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1027
+    /* "View.MemoryView":1029
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1030
+  /* "View.MemoryView":1032
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1034
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1033
+  /* "View.MemoryView":1035
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1036
+  /* "View.MemoryView":1038
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1037
+  /* "View.MemoryView":1039
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1038
+    /* "View.MemoryView":1040
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1039
+      /* "View.MemoryView":1041
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1042
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1038
+      /* "View.MemoryView":1040
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1042
+  /* "View.MemoryView":1044
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1043
+  /* "View.MemoryView":1045
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1043, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1045, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1044
+    /* "View.MemoryView":1046
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1044, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1046, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1044, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1046, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 1044, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 1046, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1046
+  /* "View.MemoryView":1048
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1047
+  /* "View.MemoryView":1049
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1051
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":1001
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -16268,15 +16365,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1052
+/* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -16288,79 +16385,79 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
-  /* "View.MemoryView":1055
+  /* "View.MemoryView":1057
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1056
+    /* "View.MemoryView":1058
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 1056, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 1058, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1059
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1055
+    /* "View.MemoryView":1057
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1059
+  /* "View.MemoryView":1061
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1060
+    /* "View.MemoryView":1062
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1054
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -16371,15 +16468,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1063
+/* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -16392,120 +16489,120 @@
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   __Pyx_RefNannySetupContext("slice_copy", 0);
 
-  /* "View.MemoryView":1067
+  /* "View.MemoryView":1069
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1068
+  /* "View.MemoryView":1070
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1071
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1073
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1072
+  /* "View.MemoryView":1074
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1076
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1075
+    /* "View.MemoryView":1077
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1076
+    /* "View.MemoryView":1078
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1079
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1065
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1080
+/* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -16515,38 +16612,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
-  /* "View.MemoryView":1083
+  /* "View.MemoryView":1085
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1084
+  /* "View.MemoryView":1086
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1084, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1086, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1082
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -16557,15 +16654,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1087
+/* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -16580,99 +16677,99 @@
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
-  /* "View.MemoryView":1094
+  /* "View.MemoryView":1096
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1095
+    /* "View.MemoryView":1097
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1098
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1094
+    /* "View.MemoryView":1096
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1098
+  /* "View.MemoryView":1100
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1099
+    /* "View.MemoryView":1101
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1101
+  /* "View.MemoryView":1103
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1105
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1101, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1089
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -16683,81 +16780,81 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1109
+/* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":1110
+  /* "View.MemoryView":1112
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1111
+    /* "View.MemoryView":1113
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1110
+    /* "View.MemoryView":1112
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1113
+  /* "View.MemoryView":1115
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1111
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1116
+/* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -16767,187 +16864,187 @@
   Py_ssize_t __pyx_v_f_stride;
   char __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1121
+  /* "View.MemoryView":1123
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1122
+  /* "View.MemoryView":1124
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1126
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1125
+    /* "View.MemoryView":1127
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1126
+      /* "View.MemoryView":1128
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1129
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1125
+      /* "View.MemoryView":1127
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1129
+  /* "View.MemoryView":1131
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1130
+    /* "View.MemoryView":1132
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1131
+      /* "View.MemoryView":1133
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1134
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1130
+      /* "View.MemoryView":1132
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1134
+  /* "View.MemoryView":1136
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1135
+    /* "View.MemoryView":1137
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1134
+    /* "View.MemoryView":1136
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1137
+  /* "View.MemoryView":1139
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1118
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1140
+/* "View.MemoryView":1142
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -16960,61 +17057,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1147
+  /* "View.MemoryView":1149
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1148
+  /* "View.MemoryView":1150
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1151
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1152
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1154
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -17026,195 +17123,195 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1156
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1157
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1153
+      /* "View.MemoryView":1155
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1157
+    /* "View.MemoryView":1159
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1158
+        /* "View.MemoryView":1160
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1159
+        /* "View.MemoryView":1161
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1162
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1152
+    /* "View.MemoryView":1154
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1162
+  /* "View.MemoryView":1164
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1163
+      /* "View.MemoryView":1165
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1167
+      /* "View.MemoryView":1169
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1168
+      /* "View.MemoryView":1170
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1140
+  /* "View.MemoryView":1142
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1170
+/* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
 
-  /* "View.MemoryView":1173
+  /* "View.MemoryView":1175
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1172
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1177
+/* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
@@ -17223,70 +17320,70 @@
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
 
-  /* "View.MemoryView":1179
+  /* "View.MemoryView":1181
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     for shape in src.shape[:ndim]:
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1181
+  /* "View.MemoryView":1183
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  * 
  *     for shape in src.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         size *= shape
  * 
  */
   __pyx_t_3 = (__pyx_v_src->shape + __pyx_v_ndim);
   for (__pyx_t_4 = __pyx_v_src->shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_shape = (__pyx_t_2[0]);
 
-    /* "View.MemoryView":1182
+    /* "View.MemoryView":1184
  * 
  *     for shape in src.shape[:ndim]:
  *         size *= shape             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
     __pyx_v_size = (__pyx_v_size * __pyx_v_shape);
   }
 
-  /* "View.MemoryView":1184
+  /* "View.MemoryView":1186
  *         size *= shape
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1179
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1187
+/* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -17294,121 +17391,121 @@
   int __pyx_v_idx;
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1196
+  /* "View.MemoryView":1198
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1197
+    /* "View.MemoryView":1199
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1198
+      /* "View.MemoryView":1200
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  *     else:
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1199
+      /* "View.MemoryView":1201
  *         for idx in range(ndim):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1196
+    /* "View.MemoryView":1198
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1201
+  /* "View.MemoryView":1203
  *             stride *= shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1202
+      /* "View.MemoryView":1204
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  * 
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1203
+      /* "View.MemoryView":1205
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1205
+  /* "View.MemoryView":1207
  *             stride *= shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1187
+  /* "View.MemoryView":1189
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1208
+/* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -17424,222 +17521,222 @@
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":1219
+  /* "View.MemoryView":1221
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1220
+  /* "View.MemoryView":1222
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1222
+  /* "View.MemoryView":1224
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1223
+  /* "View.MemoryView":1225
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1224
+    /* "View.MemoryView":1226
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 1224, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 1226, __pyx_L1_error)
 
-    /* "View.MemoryView":1223
+    /* "View.MemoryView":1225
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1227
+  /* "View.MemoryView":1229
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1228
+  /* "View.MemoryView":1230
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1231
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1230
+    /* "View.MemoryView":1232
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1231
+    /* "View.MemoryView":1233
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1233
+  /* "View.MemoryView":1235
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1237
+  /* "View.MemoryView":1239
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1238
+    /* "View.MemoryView":1240
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1239
+      /* "View.MemoryView":1241
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1238
+      /* "View.MemoryView":1240
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1241
+  /* "View.MemoryView":1243
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1242
+    /* "View.MemoryView":1244
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1241
+    /* "View.MemoryView":1243
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1244
+  /* "View.MemoryView":1246
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1246
+  /* "View.MemoryView":1248
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1208
+  /* "View.MemoryView":1210
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -17655,15 +17752,15 @@
     #endif
   }
   __pyx_r = NULL;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1251
+/* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -17678,57 +17775,57 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
-  /* "View.MemoryView":1254
+  /* "View.MemoryView":1256
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1254, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1253
+  /* "View.MemoryView":1255
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1253, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1253, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(2, 1253, __pyx_L1_error)
+  __PYX_ERR(2, 1255, __pyx_L1_error)
 
-  /* "View.MemoryView":1251
+  /* "View.MemoryView":1253
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -17743,15 +17840,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1257
+/* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -17767,26 +17864,26 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1258
+  /* "View.MemoryView":1260
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -17796,22 +17893,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(2, 1258, __pyx_L1_error)
+  __PYX_ERR(2, 1260, __pyx_L1_error)
 
-  /* "View.MemoryView":1257
+  /* "View.MemoryView":1259
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -17827,15 +17924,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1261
+/* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -17852,32 +17949,32 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1262
+  /* "View.MemoryView":1264
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1263
+    /* "View.MemoryView":1265
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1263, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -17885,43 +17982,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1263, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 1263, __pyx_L1_error)
+    __PYX_ERR(2, 1265, __pyx_L1_error)
 
-    /* "View.MemoryView":1262
+    /* "View.MemoryView":1264
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1265
+  /* "View.MemoryView":1267
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(2, 1265, __pyx_L1_error)
+    __PYX_ERR(2, 1267, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1261
+  /* "View.MemoryView":1263
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -17937,15 +18034,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1268
+/* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -17967,119 +18064,119 @@
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":1276
+  /* "View.MemoryView":1278
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1277
+  /* "View.MemoryView":1279
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1279
+  /* "View.MemoryView":1281
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1280
+  /* "View.MemoryView":1282
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1283
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1284
+  /* "View.MemoryView":1286
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1285
+    /* "View.MemoryView":1287
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1284
+    /* "View.MemoryView":1286
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1286
+  /* "View.MemoryView":1288
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1289
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1288
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1289
+  /* "View.MemoryView":1291
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
@@ -18087,420 +18184,420 @@
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1291
+  /* "View.MemoryView":1293
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1292
+    /* "View.MemoryView":1294
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1293
+      /* "View.MemoryView":1295
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1294
+        /* "View.MemoryView":1296
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1297
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1293
+        /* "View.MemoryView":1295
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1297
+      /* "View.MemoryView":1299
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1297, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1299, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1292
+      /* "View.MemoryView":1294
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1299
+    /* "View.MemoryView":1301
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1300
+      /* "View.MemoryView":1302
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1300, __pyx_L1_error)
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1302, __pyx_L1_error)
 
-      /* "View.MemoryView":1299
+      /* "View.MemoryView":1301
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1302
+  /* "View.MemoryView":1304
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1304
+    /* "View.MemoryView":1306
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1305
+      /* "View.MemoryView":1307
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1304
+      /* "View.MemoryView":1306
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1307
+    /* "View.MemoryView":1309
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(2, 1307, __pyx_L1_error)
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(2, 1309, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1308
+    /* "View.MemoryView":1310
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1302
+    /* "View.MemoryView":1304
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1310
+  /* "View.MemoryView":1312
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1313
+    /* "View.MemoryView":1315
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1314
+      /* "View.MemoryView":1316
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1313
+      /* "View.MemoryView":1315
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1315
+    /* "View.MemoryView":1317
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1318
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1317
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1318
+    /* "View.MemoryView":1320
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1320
+      /* "View.MemoryView":1322
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1321
+      /* "View.MemoryView":1323
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1324
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1325
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1326
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1318
+      /* "View.MemoryView":1320
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1310
+    /* "View.MemoryView":1312
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1326
+  /* "View.MemoryView":1328
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1329
+    /* "View.MemoryView":1331
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1329, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1331, __pyx_L1_error)
 
-    /* "View.MemoryView":1330
+    /* "View.MemoryView":1332
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1330, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1332, __pyx_L1_error)
 
-    /* "View.MemoryView":1326
+    /* "View.MemoryView":1328
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1332
+  /* "View.MemoryView":1334
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1333
+  /* "View.MemoryView":1335
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1336
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1336
+  /* "View.MemoryView":1338
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1337
+  /* "View.MemoryView":1339
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1268
+  /* "View.MemoryView":1270
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -18516,217 +18613,217 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1340
+/* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *__pyx_v_mslice, int __pyx_v_ndim, int __pyx_v_ndim_other) {
   int __pyx_v_i;
   int __pyx_v_offset;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":1344
+  /* "View.MemoryView":1346
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1346
+  /* "View.MemoryView":1348
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1347
+    /* "View.MemoryView":1349
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1348
+    /* "View.MemoryView":1350
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1351
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1351
+  /* "View.MemoryView":1353
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1352
+    /* "View.MemoryView":1354
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1353
+    /* "View.MemoryView":1355
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1356
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1340
+  /* "View.MemoryView":1342
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1362
+/* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   int __pyx_t_1;
 
-  /* "View.MemoryView":1366
+  /* "View.MemoryView":1368
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1367
+    /* "View.MemoryView":1369
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1366
+    /* "View.MemoryView":1368
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1362
+  /* "View.MemoryView":1364
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1371
+/* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
-  /* "View.MemoryView":1374
+  /* "View.MemoryView":1376
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1371
+  /* "View.MemoryView":1373
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1377
+/* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -18735,178 +18832,178 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
-  /* "View.MemoryView":1381
+  /* "View.MemoryView":1383
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1382
+    /* "View.MemoryView":1384
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1383
+      /* "View.MemoryView":1385
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1384
+        /* "View.MemoryView":1386
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1383
+        /* "View.MemoryView":1385
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1386
+      /* "View.MemoryView":1388
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1382
+      /* "View.MemoryView":1384
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1388
+    /* "View.MemoryView":1390
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
     /*else*/ {
 
-      /* "View.MemoryView":1389
+      /* "View.MemoryView":1391
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1391
+    /* "View.MemoryView":1393
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1377
+  /* "View.MemoryView":1379
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1397
+/* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
 
-  /* "View.MemoryView":1400
+  /* "View.MemoryView":1402
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1401
+  /* "View.MemoryView":1403
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1403
+  /* "View.MemoryView":1405
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1397
+  /* "View.MemoryView":1399
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1407
+/* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -18915,118 +19012,118 @@
   Py_ssize_t __pyx_v_stride;
   Py_ssize_t __pyx_v_extent;
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
 
-  /* "View.MemoryView":1411
+  /* "View.MemoryView":1413
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1412
+  /* "View.MemoryView":1414
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1414
+  /* "View.MemoryView":1416
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1415
+    /* "View.MemoryView":1417
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1416
+      /* "View.MemoryView":1418
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1417
+      /* "View.MemoryView":1419
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1414
+    /* "View.MemoryView":1416
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1419
+  /* "View.MemoryView":1421
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1420
+      /* "View.MemoryView":1422
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1422
+      /* "View.MemoryView":1424
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1407
+  /* "View.MemoryView":1409
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -19116,151 +19213,155 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb068931) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__21, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb068931:
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xb068931:
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -19280,18 +19381,18 @@
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -20209,15 +20310,15 @@
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_k_Incompatible_checksums_s_vs_0xb0, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
@@ -20307,105 +20408,105 @@
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 26, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "venv/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "../../../../private/var/folders/k8/zfp7dvcs1m326gz1brql1tv80000gn/T/pip-build-env-g_faq8wx/overlay/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "View.MemoryView":133
+  /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 133, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "View.MemoryView":136
+  /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 136, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "View.MemoryView":148
+  /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 148, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "View.MemoryView":176
+  /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 176, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "View.MemoryView":192
+  /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 192, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -20420,66 +20521,66 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 418, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "View.MemoryView":495
+  /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 495, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 520, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 570, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 577, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   PyTuple_SET_ITEM(__pyx_tuple__14, 0, __pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
@@ -20497,33 +20598,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "View.MemoryView":682
+  /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 682, __pyx_L1_error)
+  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__17);
   __Pyx_GIVEREF(__pyx_slice__17);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 703, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 705, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -20537,90 +20638,95 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "View.MemoryView":286
+  /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "View.MemoryView":291
+  /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -20666,62 +20772,62 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
-  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
-  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
   __pyx_array_type = &__pyx_type___pyx_array;
-  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 279, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 280, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_MemviewEnum.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_MemviewEnum.tp_dictoffset && __pyx_type___pyx_MemviewEnum.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_MemviewEnum.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 279, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 280, __pyx_L1_error)
   __pyx_MemviewEnum_type = &__pyx_type___pyx_MemviewEnum;
   __pyx_vtabptr_memoryview = &__pyx_vtable_memoryview;
   __pyx_vtable_memoryview.get_item_pointer = (char *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_get_item_pointer;
   __pyx_vtable_memoryview.is_slice = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_is_slice;
   __pyx_vtable_memoryview.setitem_slice_assignment = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_slice_assignment;
   __pyx_vtable_memoryview.setitem_slice_assign_scalar = (PyObject *(*)(struct __pyx_memoryview_obj *, struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_setitem_slice_assign_scalar;
   __pyx_vtable_memoryview.setitem_indexed = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_indexed;
   __pyx_vtable_memoryview.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryview_convert_item_to_object;
   __pyx_vtable_memoryview.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryview_assign_item_from_object;
-  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryview.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryview.tp_dictoffset && __pyx_type___pyx_memoryview.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryview.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -20734,53 +20840,68 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20965,15 +21086,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_PyCosmo__cython__halo_integral) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -21021,107 +21142,107 @@
  * from libc.math cimport cos, isnan, log, sin
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":209
+  /* "View.MemoryView":210
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 209, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 209, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
-  /* "View.MemoryView":286
+  /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 286, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":291
+  /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":316
+  /* "View.MemoryView":317
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
  */
   __pyx_memoryview_thread_locks_used = 0;
 
-  /* "View.MemoryView":317
+  /* "View.MemoryView":318
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
   __pyx_t_2[0] = PyThread_allocate_lock();
@@ -21130,37 +21251,37 @@
   __pyx_t_2[3] = PyThread_allocate_lock();
   __pyx_t_2[4] = PyThread_allocate_lock();
   __pyx_t_2[5] = PyThread_allocate_lock();
   __pyx_t_2[6] = PyThread_allocate_lock();
   __pyx_t_2[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_2, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":551
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 549, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 549, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 551, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":997
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 995, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 995, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 997, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -22191,15 +22312,15 @@
 }
 #ifndef Py_NO_RETURN
 #define Py_NO_RETURN
 #endif
 static void __pyx_fatalerror(const char *fmt, ...) Py_NO_RETURN {
     va_list vargs;
     char msg[200];
-#ifdef HAVE_STDARG_PROTOTYPES
+#if PY_VERSION_HEX >= 0x030A0000 || defined(HAVE_STDARG_PROTOTYPES)
     va_start(vargs, fmt);
 #else
     va_start(vargs);
 #endif
     vsnprintf(msg, 200, fmt, vargs);
     va_end(vargs);
     Py_FatalError(msg);
@@ -22746,28 +22867,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22788,15 +22909,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -23028,15 +23149,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
   #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -23599,25 +23720,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -23654,57 +23793,77 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -23726,15 +23885,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -23850,14 +24009,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -23913,22 +24078,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -24426,15 +24601,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -24580,15 +24755,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -25572,19 +25747,41 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/halo_integral.pyx` & `PyCosmo-2.1.1/src/PyCosmo/cython/halo_integral.pyx`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/logf.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/logf.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/mconf.h` & `PyCosmo-2.1.1/src/PyCosmo/cython/mconf.h`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/mtherr.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/mtherr.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/polevl.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/polevl.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/polevlf.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/polevlf.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/protos.h` & `PyCosmo-2.1.1/src/PyCosmo/cython/protos.h`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/sici.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/sici.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/sici32.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/sici32.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/sicif.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/sicif.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/cython/sinf.c` & `PyCosmo-2.1.1/src/PyCosmo/cython/sinf.c`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/ini_handling.py` & `PyCosmo-2.1.1/src/PyCosmo/ini_handling.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/model_config.py` & `PyCosmo-2.1.1/src/PyCosmo/model_config.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/optimize_nq.py` & `PyCosmo-2.1.1/src/PyCosmo/optimize_nq.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/patches.py` & `PyCosmo-2.1.1/src/PyCosmo/patches.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo/predefined_k_grids.py` & `PyCosmo-2.1.1/src/PyCosmo/predefined_k_grids.py`

 * *Files identical despite different names*

### Comparing `PyCosmo-2.1.0/src/PyCosmo.egg-info/PKG-INFO` & `PyCosmo-2.1.1/src/PyCosmo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCosmo
-Version: 2.1.0
+Version: 2.1.1
 Summary: A multi-purpose cosmology calculation tool
 Author: Uwe Schmitt et al
 Author-email: uwe.schmitt@id.ethz.ch
 License: GPLv3
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/PyCosmo
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

