# Comparing `tmp/scalib-0.5.4.tar.gz` & `tmp/scalib-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalib-0.5.4.tar", last modified: Wed Apr 26 15:01:45 2023, max compression
+gzip compressed data, was "scalib-0.5.5.tar", last modified: Tue May 30 11:22:27 2023, max compression
```

## Comparing `scalib-0.5.4.tar` & `scalib-0.5.5.tar`

### file list

```diff
@@ -1,573 +1,575 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 15:01:30.000000 scalib-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 15:01:30.000000 scalib-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-26 15:01:30.000000 scalib-0.5.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 15:01:30.000000 scalib-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 15:01:30.000000 scalib-0.5.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-26 15:01:30.000000 scalib-0.5.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-26 15:01:30.000000 scalib-0.5.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-26 15:01:30.000000 scalib-0.5.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-26 15:01:30.000000 scalib-0.5.4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-26 15:01:30.000000 scalib-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-26 15:01:30.000000 scalib-0.5.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 15:01:45.173366 scalib-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-26 15:01:30.000000 scalib-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/copyright.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/aes_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/paper/
--rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-04-26 15:01:30.000000 scalib-0.5.4/paper/build_paper.sh
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-26 15:01:30.000000 scalib-0.5.4/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-26 15:01:30.000000 scalib-0.5.4/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-26 15:01:30.000000 scalib-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-26 15:01:45.177367 scalib-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 15:01:30.000000 scalib-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/attacks/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/attacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/attacks/factor_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/attacks/sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib/build_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/config/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/metrics/snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/metrics/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/modeling/ldaclassifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/postprocessing/rankestimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-04-26 15:01:45.000000 scalib-0.5.4/src/scalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    45960 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib_ext/geigen/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib_ext/geigen/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.105365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.093365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.105365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.109365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.125365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.129366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.129366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.149366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.157366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.157366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.157366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/Version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/geigen.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/geigen/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/src/geigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/src/geigen.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/ranklib/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/ranklib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/aes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/aes.h
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.h
--rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_execute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_execute.h
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.h
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.h
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/histogram.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/main_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/rank.rs
--rw-r--r--   0 runner    (1001) docker     (123)   274225 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/score_example_data.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.h
--rw-r--r--   0 runner    (1001) docker     (123)   224884 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/top.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/get_snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/mttest.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/snr_update.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/src/scalib_ext/scalib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/matrixmul.rs
--rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/mttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/
--rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/bp_compute.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_build.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_parser.rs
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/ttest.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/src/scalib_ext/scalib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/tests/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/tests/multivarcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/tests/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib-py/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/ranking.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/thread_pool.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/mttest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_factorgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_lda.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-26 15:01:30.000000 scalib-0.5.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.982273 scalib-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-30 11:22:17.000000 scalib-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-30 11:22:17.000000 scalib-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-30 11:22:17.000000 scalib-0.5.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-30 11:22:17.000000 scalib-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 11:22:17.000000 scalib-0.5.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-30 11:22:17.000000 scalib-0.5.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-30 11:22:17.000000 scalib-0.5.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-30 11:22:17.000000 scalib-0.5.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-30 11:22:17.000000 scalib-0.5.5/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 11:22:17.000000 scalib-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-30 11:22:17.000000 scalib-0.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-30 11:22:27.046273 scalib-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-30 11:22:17.000000 scalib-0.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.982273 scalib-0.5.5/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/copyright.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/aes_attack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/aes_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/aes_tvla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/paper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-05-30 11:22:17.000000 scalib-0.5.5/paper/build_paper.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-30 11:22:17.000000 scalib-0.5.5/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-05-30 11:22:17.000000 scalib-0.5.5/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 11:22:17.000000 scalib-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-30 11:22:27.046273 scalib-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 11:22:17.000000 scalib-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.986273 scalib-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/attacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/attacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/attacks/factor_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24799 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/attacks/sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib/build_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/config/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/metrics/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/metrics/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/modeling/ldaclassifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/postprocessing/rankestimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27051 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    45960 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/geigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/geigen/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.986273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.002273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.002273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.986273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.014273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.014273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.026273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.034273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.034273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.034273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/Version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/geigen.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/src/geigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/src/geigen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/ranklib/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/ranklib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/aes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/aes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_execute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_execute.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/histogram.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/main_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/rank.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   274225 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/score_example_data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)   224884 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/top.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/get_snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/mttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/snr_update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/src/scalib_ext/scalib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/matrixmul.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/mttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/
+-rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/bp_compute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_parser.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/ttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/src/scalib_ext/scalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/tests/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/tests/multivarcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/tests/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/ranking.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/thread_pool.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/mttest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_factorgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_lda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-30 11:22:17.000000 scalib-0.5.5/tox.ini
```

### Comparing `scalib-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md` & `scalib-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md` & `scalib-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/.github/workflows/ci.yml` & `scalib-0.5.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/CHANGELOG.rst` & `scalib-0.5.5/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 =========
 Changelog
 =========
 
 Not released
 ------------
 
+v0.5.5 (2023/05/30)
+-------------------
+
+* Fix ``Distribution`` size bug in belief propagation computation (#102).
+* Do not include debug symbols in release builds (makes wheel much smaller).
+* ``Ttest``: do not crash on non-contiguous/fortran-order arrays
+* Improve examples and README
+
 v0.5.4 (2023/04/26)
 -------------------
 
 * Run CI on Mac Os and build wheels (x86_64 and arm64, but we test only x86_64). No AVX2 due to old runner in github CI.
 * Add ``scalib.tools.ContextExecutor``, as a solution to ``LookupError`` in
   ``get_config()``.
 * Fix numerical underflow in ``BPState`` when multiple traces are used.
```

### Comparing `scalib-0.5.4/CONTRIBUTING.rst` & `scalib-0.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/COPYING` & `scalib-0.5.5/COPYING`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/COPYRIGHT` & `scalib-0.5.5/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/MANIFEST.in` & `scalib-0.5.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/Makefile` & `scalib-0.5.5/Makefile`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/PKG-INFO` & `scalib-0.5.5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,43 @@
-Metadata-Version: 2.1
-Name: scalib
-Version: 0.5.4
-Summary: Side-Channel Analysis Library
-Home-page: https://github.com/simple-crypto/scalib
-Author: Olivier Bronchain, Gaëtan Cassiers
-Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
-License: GNU AGPL v3+
-Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: COPYING
-
-Welcome to SCALib
-=================
+======
+SCALib
+======
 
 .. image:: https://badge.fury.io/py/scalib.svg
     :target: https://pypi.org/project/scalib/
     :alt: PyPI
 .. image:: https://readthedocs.org/projects/scalib/badge/?version=stable
     :target: https://scalib.readthedocs.io/en/stable/
     :alt: Documentation Status
 .. image:: https://img.shields.io/matrix/scalib:matrix.org
     :target: https://matrix.to/#/#scalib:matrix.org
     :alt: Matrix room
 
-The Side-Channel Analysis Library (SCALib) is a Python package that
-contains state-of-the-art tools for side-channel security evaluation. It focuses on
+The Side-Channel Analysis Library (SCALib) is a Python library that
+contains state-of-the-art tools for side-channel security evaluation.
+
+- **Documentation**: https://scalib.readthedocs.io/
+- **Examples**: `examples/ <examples/>`_
+- **Chat**: `https://matrix.to/#/#scalib:matrix.org`
+- **Source code**: https://github.com/simple-crypto/SCALib
+- **Bug reports/feature requests**: https://github.com/simple-crypto/SCALib/issues/new/choose
+- **Contributing**: https://scalib.readthedocs.io/en/stable/source/contributing.html
+
+
+SCALib focuses on
 
 - simple interface,
 - state-of-the art algorithms,
 - excellent performance (see `benchmarks <https://github.com/cassiersg/SCABench>`_).
 
 SCALib should be useful for any side-channel practitioner who wants to
 evaluate, but not necessarily attack, protected or non-protected
 implementations.
-
 See the documentation_ for the list of implemented tools.
 
-We have a `matrix chat <https://matrix.to/#/#scalib:matrix.org>`_ for
-announcements, questions, community support and discussions.
-
 .. _documentation: https://scalib.readthedocs.io/en/stable
 
 Install
 =======
 
 SCALib is on PyPi! Simple install:
 
@@ -105,18 +99,21 @@
 Contributions and Issues
 ========================
 
 Contributions welcome !
 
 Please file a **bug report** for any issue you encounter (even bad documentation is
 a bug !), and let us know your **suggestions** (open a `github issue
-<https://github.com/simple-crypto/SCALib/issues/new/choose>`_, email works too).
+<https://github.com/simple-crypto/SCALib/issues/new/choose>`_, `chat
+<https://matrix.to/#/#scalib:matrix.org>`_ and `email
+<mailto:gaetan.cassiers@uclouvain.be>`_ work too).
 We also welcome code contributions, see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_.
+You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_
+(announcements, questions, community support, open discussion, etc.).
 
 All code contributions are subject to the Contributor License Agreement (`CLA
 <https://www.simple-crypto.dev/organization>`_) of SIMPLE-Crypto, which ensures
 a thriving future for open-source hardware security.
 
 License
 =======
```

### Comparing `scalib-0.5.4/README.rst` & `scalib-0.5.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,56 @@
-Welcome to SCALib
-=================
+Metadata-Version: 2.1
+Name: scalib
+Version: 0.5.5
+Summary: Side-Channel Analysis Library
+Home-page: https://github.com/simple-crypto/scalib
+Author: Olivier Bronchain, Gaëtan Cassiers
+Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
+License: GNU AGPL v3+
+Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: COPYING
+
+======
+SCALib
+======
 
 .. image:: https://badge.fury.io/py/scalib.svg
     :target: https://pypi.org/project/scalib/
     :alt: PyPI
 .. image:: https://readthedocs.org/projects/scalib/badge/?version=stable
     :target: https://scalib.readthedocs.io/en/stable/
     :alt: Documentation Status
 .. image:: https://img.shields.io/matrix/scalib:matrix.org
     :target: https://matrix.to/#/#scalib:matrix.org
     :alt: Matrix room
 
-The Side-Channel Analysis Library (SCALib) is a Python package that
-contains state-of-the-art tools for side-channel security evaluation. It focuses on
+The Side-Channel Analysis Library (SCALib) is a Python library that
+contains state-of-the-art tools for side-channel security evaluation.
+
+- **Documentation**: https://scalib.readthedocs.io/
+- **Examples**: `examples/ <examples/>`_
+- **Chat**: `https://matrix.to/#/#scalib:matrix.org`
+- **Source code**: https://github.com/simple-crypto/SCALib
+- **Bug reports/feature requests**: https://github.com/simple-crypto/SCALib/issues/new/choose
+- **Contributing**: https://scalib.readthedocs.io/en/stable/source/contributing.html
+
+
+SCALib focuses on
 
 - simple interface,
 - state-of-the art algorithms,
 - excellent performance (see `benchmarks <https://github.com/cassiersg/SCABench>`_).
 
 SCALib should be useful for any side-channel practitioner who wants to
 evaluate, but not necessarily attack, protected or non-protected
 implementations.
-
 See the documentation_ for the list of implemented tools.
 
-We have a `matrix chat <https://matrix.to/#/#scalib:matrix.org>`_ for
-announcements, questions, community support and discussions.
-
 .. _documentation: https://scalib.readthedocs.io/en/stable
 
 Install
 =======
 
 SCALib is on PyPi! Simple install:
 
@@ -92,18 +112,21 @@
 Contributions and Issues
 ========================
 
 Contributions welcome !
 
 Please file a **bug report** for any issue you encounter (even bad documentation is
 a bug !), and let us know your **suggestions** (open a `github issue
-<https://github.com/simple-crypto/SCALib/issues/new/choose>`_, email works too).
+<https://github.com/simple-crypto/SCALib/issues/new/choose>`_, `chat
+<https://matrix.to/#/#scalib:matrix.org>`_ and `email
+<mailto:gaetan.cassiers@uclouvain.be>`_ work too).
 We also welcome code contributions, see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_.
+You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_
+(announcements, questions, community support, open discussion, etc.).
 
 All code contributions are subject to the Contributor License Agreement (`CLA
 <https://www.simple-crypto.dev/organization>`_) of SIMPLE-Crypto, which ensures
 a thriving future for open-source hardware security.
 
 License
 =======
```

### Comparing `scalib-0.5.4/docs/Makefile` & `scalib-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/docs/_templates/autosummary/class.rst` & `scalib-0.5.5/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/docs/_templates/autosummary/module.rst` & `scalib-0.5.5/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/docs/conf.py` & `scalib-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/docs/index.rst` & `scalib-0.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/docs/make.bat` & `scalib-0.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/examples/aes_simulation.py` & `scalib-0.5.5/examples/aes_attack.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,140 @@
-from scalib.metrics import SNR
+from scalib.metrics import SNR, Ttest
 from scalib.modeling import LDAClassifier
-from scalib.attacks import SASCAGraph
+from scalib.attacks import FactorGraph, BPState
 from scalib.postprocessing import rank_accuracy
 
 from utils import sbox, gen_traces
 import numpy as np
 
 
 def main():
     nc = 256
     npoi = 2
 
     # Parameters
-    std = 1
-    ntraces_a = 1000
+    std = 2
+    ntraces_a = 40
     ntraces_p = 20000
 
-    print("1. Generate simulated traces with parameters:")
+    print(
+        "1. Generate simulated traces (Hamming weight + Gaussian noise) with parameters:"
+    )
     print(f"    ntraces for profiling: {ntraces_p}")
     print(f"    ntraces for attack:    {ntraces_a}")
     print(f"    noise std:             {std}")
-    traces_p, labels_p = gen_traces(ntraces_p, std, random_key=1)
-    traces_a, labels_a = gen_traces(ntraces_a, std, random_key=0)
+    traces_p, labels_p = gen_traces(
+        ntraces_p, std, random_key=True, random_plaintext=True
+    )
+    traces_a, labels_a = gen_traces(
+        ntraces_a, std, random_key=False, random_plaintext=True
+    )
 
     _, ns = traces_p.shape
-    print("2. Profiling")
-    # For each of the 16 variables at the output of the Sbox (xi)
-    # we build a model that store in the dictonnary models.
-    #
-    # The profiling is done in 3 phases
-    # 1. Compute SNR for all xi
-    # 2. Select the Point-of-Interest based on the SNR
-    # 3. Fit an LDA model for each of the xi
 
-    models = {}
-    for i in range(16):
-        models[f"x{i}"] = {}
-
-    print("    2.1 Compute snr for 16 Sbox outputs xi")
+    print("2. POI selection with SNR")
+    print("    2.1 Compute SNR for 16 Sbox outputs xi")
     # y array with xi values
     x = np.zeros((ntraces_p, 16), dtype=np.uint16)
     for i in range(16):
         x[:, i] = labels_p[f"x{i}"]
 
     # estimate SNR
-    snr = SNR(nc=256, ns=ns, np=16)
+    snr = SNR(nc=nc, ns=ns, np=16)
     snr.fit_u(traces_p, x)
     snr_val = snr.get_snr()
 
-    print(f"    2.2 Keep {npoi} POIs for each xi")
-    # POI are the npoi indexes with the largest SNR
-    for i in range(16):
-        models[f"x{i}"]["poi"] = np.argsort(snr_val[i])[-npoi:]
+    print("    2.2 Select POIs with highest SNR.")
+    pois = [np.argsort(snr_val[i])[-npoi:] for i in range(16)]
 
-    print("    2.3 Build LDAClassifier for each xi")
+    print("3. Profiling")
+    # We build a LDA model (pooled Gaussian templates) for each of the 16
+    # Sboxes (xi).
+
+    print("    3.1 Build LDAClassifier for each xi")
+    models = []
     for i in range(16):
-        model = models[f"x{i}"]
-        lda = LDAClassifier(nc=256, ns=npoi, p=1)
-        lda.fit_u(l=traces_p[:, model["poi"]], x=labels_p[f"x{i}"].astype(np.uint16))
+        lda = LDAClassifier(nc=nc, ns=npoi, p=1)
+        lda.fit_u(l=traces_p[:, pois[i]], x=labels_p[f"x{i}"].astype(np.uint16))
         lda.solve()
-        model["lda"] = lda
+        models.append(lda)
+
+    print("    3.2 Get xi distributions from attack traces")
+    probas = [models[i].predict_proba(traces_a[:, pois[i]]) for i in range(16)]
 
-    print("3. Attack")
-    print("    3.1 Create the SASCA Graph")
+    print("4. Attack")
+    print("    4.1 Create the SASCA Graph")
     graph_desc = f"""
                 NC {nc}
                 TABLE sbox   # The Sbox
                 """
 
     for i in range(16):
         graph_desc += f"""
                 VAR SINGLE k{i} # The key
-                VAR MULTI p{i}  # The plaintext
+                PUB MULTI p{i}  # The plaintext
                 VAR MULTI x{i}  # Sbox output
                 VAR MULTI y{i}  # Sbox input
                 PROPERTY y{i} = k{i} ^ p{i} # Key addition
                 PROPERTY x{i} = sbox[y{i}]  # Sbox lookup
                 """
 
-    # Init SASCAGraph with graph_desc and the number of attack traces
-    sasca = SASCAGraph(graph_desc, n=ntraces_a)
+    # Initialize FactorGraph with the graph description and the required tables
+    factor_graph = FactorGraph(graph_desc, {"sbox": sbox})
 
-    print("    3.2 Add public information in the SASCAGraph")
-    sasca.set_table("sbox", sbox)
-    for i in range(16):
-        sasca.set_public(f"p{i}", labels_a[f"p{i}"].astype(np.uint32))
+    print("    4.2 Create belief propagation state.")
+    # We have to give the number of attack traces and the values for the public variables.
+    bp = BPState(
+        factor_graph,
+        ntraces_a,
+        {f"p{i}": labels_a[f"p{i}"].astype(np.uint32) for i in range(16)},
+    )
 
-    print("    3.3 Add xi distributions in the graph")
     for i in range(16):
-        model = models[f"x{i}"]
-        sasca.set_init_distribution(
-            f"x{i}", model["lda"].predict_proba(traces_a[:, model["poi"]])
-        )
+        bp.set_evidence(f"x{i}", probas[i])
 
-    print("    3.4 Run belief propagation")
-    print("")
-    sasca.run_bp(it=3)
-    print("")
+    print("    4.3 Run belief propagation")
+    for i in range(16):
+        bp.bp_acyclic(f"k{i}")
 
-    print("4. Attack evaluation")
-    print("    4.1 Byte-wise attack")
+    print("5. Attack evaluation")
+    print("    5.1 Byte-wise attack")
 
     # correct secret key
     secret_key = []
     # distribution for each of the key bytes
     key_distribution = []
     # the best key guess of the adversary
     guess_key = []
     # rank for all the key bytes
     ranks = []
 
     for i in range(16):
         sk = labels_a[f"k{i}"][0]  # secret key byte
-        distribution = sasca.get_distribution(f"k{i}")[0, :]
+        distribution = bp.get_distribution(f"k{i}")
 
         guess_key.append(np.argmax(distribution))
         ranks.append(256 - np.where(np.argsort(distribution) == sk)[0])
 
         secret_key.append(sk)
         key_distribution.append(distribution)
 
     print("")
     print("        secret key (hex):", " ".join(["%3x" % (x) for x in secret_key]))
     print("        best key   (hex):", " ".join(["%3x" % (x) for x in guess_key]))
     print("        key byte ranks  :", " ".join(["%3d" % (x) for x in ranks]))
     print("")
 
-    print(f"    4.2 Estimate full log2 key rank:")
+    print(f"   5.2 Estimate full log2 key rank:")
     key_distribution = np.array(key_distribution)
 
-    rmin, r, rmax = rank_accuracy(-np.log10(key_distribution), secret_key, 1)
+    # Scores are negative log-likelihoods.
+    # Put a lower-bound on the probabilities, oterwise we might get NaNs.
+    scores = -np.log2(np.maximum(key_distribution, 2**-128))
+    rmin, r, rmax = rank_accuracy(scores, secret_key, 1)
 
     lrmin, lr, lrmax = (np.log2(rmin), np.log2(r), np.log2(rmax))
     print("")
     print(f"        {lrmin} < {lr} < {lrmax}")
     print("")
```

### Comparing `scalib-0.5.4/examples/utils.py` & `scalib-0.5.5/examples/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,21 +19,25 @@
         0x70, 0x3e, 0xb5, 0x66, 0x48, 0x03, 0xf6, 0x0e, 0x61, 0x35, 0x57, 0xb9, 0x86, 0xc1, 0x1d, 0x9e,
         0xe1, 0xf8, 0x98, 0x11, 0x69, 0xd9, 0x8e, 0x94, 0x9b, 0x1e, 0x87, 0xe9, 0xce, 0x55, 0x28, 0xdf,
         0x8c, 0xa1, 0x89, 0x0d, 0xbf, 0xe6, 0x42, 0x68, 0x41, 0x99, 0x2d, 0x0f, 0xb0, 0x54, 0xbb, 0x16
         ],dtype=np.uint32)
 # fmt: on
 
 
-def gen_traces(ntraces, std, random_key):
-    if not random_key:
-        k = np.random.randint(0, 256, (1, 16), dtype=np.uint8)
-    else:
+def gen_traces(ntraces, std, random_key, random_plaintext):
+    if random_key:
         k = np.random.randint(0, 256, (ntraces, 16), dtype=np.uint8)
+    else:
+        k = np.random.randint(0, 256, (1, 16), dtype=np.uint8)
 
-    p = np.random.randint(0, 256, (ntraces, 16), dtype=np.uint8)
+    if random_plaintext:
+        p = np.random.randint(0, 256, (ntraces, 16), dtype=np.uint8)
+    else:
+        p = np.random.randint(0, 256, (16,), dtype=np.uint8)
+        p = np.vstack(ntraces * [p])
 
     # generate sensible data.
     # Input and output of the Sbox
     y = p ^ k
     x = sbox[y]
     data = np.concatenate((x, y), axis=1).astype(np.uint8)
```

### Comparing `scalib-0.5.4/paper/paper.bib` & `scalib-0.5.5/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/paper/paper.md` & `scalib-0.5.5/paper/paper.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,20 @@
     orcid: 0000-0001-7595-718X
     equal-contrib: true
     affiliation: 1
   - name: Gaëtan Cassiers
     orcid: 0000-0001-5426-9345
     equal-contrib: true
     corresponding: true
-    affiliation: "1, 2, 3"
+    affiliation: "1, 2"
 affiliations:
  - name: UCLouvain, Belgium
    index: 1
  - name: Graz University of Technology, Austria
    index: 2
- - name: Lamarr Security Research, Austria
-   index: 3
 date: 16 February 2023
 bibliography: paper.bib
 
 ---
 
 # Summary
 
@@ -41,101 +39,102 @@
 Then, a statistical processing is applied to this leakage in order to infer the
 internal behavior of the device (typically, an intermediate state of the
 cryptographic algorithm). Finally, the cryptographic key is recovered from the
 known behavior [@DBLP:conf/eurocrypt/StandaertMY09].
 
 For the statistical processing, we distinguish between two classes of attacks,
 based on the use of a profiling dataset.
-Such a dataset consists in leakage measurements on a device running the
+Such a dataset consists of leakage measurements on a device running the
 cryptographic algorithm with the known key.
 Profiled attacks use this data to fit a statistical model (or train a
 machine-learning model) of the device, while non-profiled attacks have to rely
 on *a priori* models and are therefore less powerful [@DBLP:conf/ches/ChariRR02].
 
-There are two main approaches to evaluating security of devices against side-channel attacks.
+There are two main approaches for evaluating the security of devices against side-channel attacks.
 First, attack-based evaluations try to attack the device and report their success or failure.
 In case of success, the main figure of merit is the number of traces (i.e.,
 number of executions of a cryptographic algorithm for which the leakage is
 measured).
 Second, detection-based evaluations try to detect the presence of key-dependent
 leakage and sometimes quantify it.
 These two types of methods can be complementary in the evaluation of a device.
 
 Side-channel evaluations are used in various research contexts, such as
 analyzing the effectiveness of a newly proposed countermeasure or analyzing a
 widely deployed device.
 In `SCALib`, we implement algorithms for commonly used metrics and methods in
 side-channel security evaluations, attack-based and evaluation-based.
-We however focus on the requirements of evaluations, and do not implement
+We focus on the requirements of evaluations and do not implement
 complete attacks when they are not needed to evaluate the security of a device.
 
 `SCALib` is distributed as a Python package and uses 16-bit integer `numpy` [@numpy] arrays
 for leakage traces.
-For the sake of efficiency, most algorithms are however implemented in Rust,
+For the sake of efficiency, most algorithms are implemented in Rust,
 allowing fine control of the memory accesses and enabling efficient
 parallelization.
 
 
 # Statement of need
 
 Many of the algorithms used in side-channel security evaluations are well-known
 statistical techniques.
 For instance, the widely used TVLA methodology is based on the Welch t-test for
 the difference of means [@DBLP:conf/ches/SchneiderM15].
-Also when modeling the leakage, techniques such as Linear Discriminant Analysis
+Also, when modeling the leakage, techniques such as Linear Discriminant Analysis
 (LDA) [@DBLP:conf/ches/StandaertA08] can be used.
 While implementations of these algorithms are fairly easy to find, our use-case
 has a few particularities that motivate dedicated implementations.
-For example, the number of traces used in a evaluation can be very large,
+For example, the number of traces used in an evaluation can be very large,
 amounting to terabytes of data, hence incremental single-pass algorithms (that
 avoid the need to store and/or load multiple times the dataset) are highly
 desirable.
-Moreover, while the leakage samples are acquired at relatively low-resolution
+Moreover, while the leakage samples are acquired at a fairly low-resolution
 (8-bit to 16-bit integers), detection of very small effect sizes is
 needed, as they can potentially be exploited to mount an attack.
 Besides this requirement, leakage traces contain many points (typically
-thousands) and many metrics have to be computed for each of these points,
+thousands), and many metrics have to be computed for each of these points,
 providing parallelization opportunities.
 As a result of these characteristics, dedicated implementations can achieve
 much better accuracy and performance than generic or naive (e.g., pure `numpy`)
 ones.
 
 On the other hand, security-specific algorithms are also used, such as key rank
-estimation (which allows to know the computational cost of the last part of a
+estimation (which allows us to know the computational cost of the last part of a
 side-channel attack without actually running it) [@DBLP:conf/ches/PoussierSG16].
 
-While there exists multiple open-source side-channel attack and evaluation
-libraries, most of them offer a very limited feature set and are unmaintained.
+While multiple open-source side-channel attack and evaluation
+libraries exist, most of them offer a very limited feature set and are unmaintained.
 The most comprehensive libraries are `lascar` [@lascar] and `SCAred` [@scared], which offer
 implementations of some evaluation metrics and non-profiled attacks.
 
 `SCALib` complements and improves over these libraries by providing better
 implementations for the computation of two common evaluation metrics, by
-providing algorithms for profiled side-channel attacks and by including a key
+providing algorithms for profiled side-channel attacks and including a key
 rank enumeration algorithm as a final evaluation step.
 More precisely, for leakage metrics, we implement the Welch t-test and the
 computation of the signal-to-noise ratio, and our implementations are significantly
 faster than the ones of `lascar` and `SCAred` [@scabench].
 Moreover, our t-test implementation includes so-called higher-order and
 multivariate evaluations [@DBLP:conf/ches/SchneiderM15].
 Regarding profiled attacks, `SCALib` includes an implementation of
 LDA with a dimensionality reduction step (this
 provides a regularization and improves classification performance) [@DBLP:conf/ches/StandaertA08].
 We also implement the soft analytical side-channel attack (SASCA), which is a
 variant of the belief propagation algorithm [@DBLP:conf/asiacrypt/Veyrat-CharvillonGS14].
-Finally, our key-rank estimation implementation relies an efficient histogram-based algorithm [@DBLP:conf/ches/PoussierSG16].
+Finally, our key-rank estimation implementation relies on an efficient
+histogram-based algorithm [@DBLP:conf/ches/PoussierSG16].
 
 `SCALib` has been used in many recent papers as a tool to validate new protected
 designs [@DBLP:journals/tches/NagpalGPM22], to publish new attacks on public
 implementations [@DBLP:journals/iacr/BronchainCS21], and also as a basis
 to develop new attack and evaluation methodologies [@DBLP:journals/tches/BronchainS21].
 
 
 # Acknowledgments
 
 This work has been funded in part by the Belgian Fund for Scientific Research
 (F.R.S.-FNRS) through the Equipment Project SCALAB, by the European Union (EU)
 and the Walloon Region through the FEDER project USERMedia (convention number
-501907-379156), and by the European Union (EU) through the ERC project 724725
-(acronym SWORD).
+501907-379156), by the European Union (EU) through the ERC project 724725
+(acronym SWORD), and by SGS.
 
 # References
```

### Comparing `scalib-0.5.4/pyproject.toml` & `scalib-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/setup.cfg` & `scalib-0.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/setup.py` & `scalib-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/__init__.py` & `scalib-0.5.5/src/scalib/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/attacks/factor_graph.py` & `scalib-0.5.5/src/scalib/attacks/factor_graph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/attacks/sascagraph.py` & `scalib-0.5.5/src/scalib/attacks/sascagraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,21 +140,18 @@
         The number of independent traces to process for the `VAR MULTI`
         variables.
     """
 
     def __init__(self, graph, n):
         import warnings
 
-        warnings.simplefilter("once", DeprecationWarning)  # turn off filter
         warnings.warn(
             "SASCAGraph is deprecated and will be removed in a next release. Use FactorGraph instead.",
             category=DeprecationWarning,
-            stacklevel=2,
         )
-        warnings.simplefilter("default", DeprecationWarning)  # reset filter
 
         self.n_ = n
         self.solved_ = False
 
         self.graph = SASCAGraphParser(graph)
         self.nc_ = self.graph.nc
         self.tables_ = {table: None for table in self.graph.tables}
```

### Comparing `scalib-0.5.4/src/scalib/config/__init__.py` & `scalib-0.5.5/src/scalib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/config/threading.py` & `scalib-0.5.5/src/scalib/config/threading.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/metrics/snr.py` & `scalib-0.5.5/src/scalib/metrics/snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/metrics/ttest.py` & `scalib-0.5.5/src/scalib/metrics/ttest.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,18 +145,23 @@
             be of dimension `(n, ns)` and its type must be `np.int16`.
         x : array_like, np.uint16
             Set in which each trace belongs. Must be of shape `(n,)`, must be
             `np.uint16` and must contain only `0` and `1`.
         """
         nl, nsl = l.shape
         nx = x.shape[0]
-        if not (nx == nl):
+        if nx != nl:
             raise ValueError(f"Expected x with shape ({nl},)")
-        if not (nsl == self._ns):
-            raise Exception(f"Expected second dim of l to have size {self._ns}.")
+        if nsl != self._ns:
+            raise ValueError(f"Expected second dim of l to have size {self._ns}.")
+        if not l.flags["C_CONTIGUOUS"]:
+            raise ValueError(
+                "Expected l to be a contiguous (C memory order) array. "
+                "Use np.ascontiguous to change memory representation."
+            )
 
         with scalib.utils.interruptible():
             self._ttest.update(l, x, get_config())
 
     def get_ttest(self):
         r"""Return the current Ttest estimation with an array of shape `(d,ns)`."""
         with scalib.utils.interruptible():
@@ -185,25 +190,28 @@
     Especially, :math:`\bar{l}` denotes the estimated mean of `l` and
     :math:`\sigma_l` its standard deviation. `pois` defines the points in the
     traces for which the (normalized) product will be tested.
 
     Parameters
     ----------
     d : int
-        Maximal statistical order of the :math:`t`-test.
+        Number of variables of the :math:`t`-test.
     pois : array_like, uint32
-        Array of share `(d,n_pois)`. Each column in `pois` will result in a
-        :math:`t`-test of the product of the traces at these $d$ indexes.
+        Array of shape ``(d,n_pois)``. Each column in `pois` will result in a
+        :math:`t`-test of the product of the traces at these :math:`d` indexes.
+        If an index is repeated in a column, the corresponding test uses a
+        higher-order moment for the corresponding point in the trace.
 
     Examples
     --------
     >>> from scalib.metrics import MTtest
     >>> import numpy as np
     >>> traces = np.random.randint(0,256,(100,200),dtype=np.int16)
-    >>> pois = np.random.randint(0,200,(2,5000),dtype=np.uint32)
+    >>> # Take as POIs each point in the trace combined with any of the 10 following samples.
+    >>> pois = np.array([[x, x+d] for x in range(200) for d in range(10) if x + d < 200], dtype=np.uint32).T
     >>> X = np.random.randint(0,2,100,dtype=np.uint16)
     >>> mttest = MTtest(d=2,pois=pois)
     >>> mttest.fit_u(traces,X)
     >>> t = mttest.get_ttest()
 
     """
```

### Comparing `scalib-0.5.4/src/scalib/modeling/__init__.py` & `scalib-0.5.5/src/scalib/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/modeling/ldaclassifier.py` & `scalib-0.5.5/src/scalib/modeling/ldaclassifier.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/postprocessing/rankestimation.py` & `scalib-0.5.5/src/scalib/postprocessing/rankestimation.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/tools.py` & `scalib-0.5.5/src/scalib/tools.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib/utils.py` & `scalib-0.5.5/src/scalib/utils.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib.egg-info/PKG-INFO` & `scalib-0.5.5/src/scalib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 Metadata-Version: 2.1
 Name: scalib
-Version: 0.5.4
+Version: 0.5.5
 Summary: Side-Channel Analysis Library
 Home-page: https://github.com/simple-crypto/scalib
 Author: Olivier Bronchain, Gaëtan Cassiers
 Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 License: GNU AGPL v3+
 Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
-Welcome to SCALib
-=================
+======
+SCALib
+======
 
 .. image:: https://badge.fury.io/py/scalib.svg
     :target: https://pypi.org/project/scalib/
     :alt: PyPI
 .. image:: https://readthedocs.org/projects/scalib/badge/?version=stable
     :target: https://scalib.readthedocs.io/en/stable/
     :alt: Documentation Status
 .. image:: https://img.shields.io/matrix/scalib:matrix.org
     :target: https://matrix.to/#/#scalib:matrix.org
     :alt: Matrix room
 
-The Side-Channel Analysis Library (SCALib) is a Python package that
-contains state-of-the-art tools for side-channel security evaluation. It focuses on
+The Side-Channel Analysis Library (SCALib) is a Python library that
+contains state-of-the-art tools for side-channel security evaluation.
+
+- **Documentation**: https://scalib.readthedocs.io/
+- **Examples**: `examples/ <examples/>`_
+- **Chat**: `https://matrix.to/#/#scalib:matrix.org`
+- **Source code**: https://github.com/simple-crypto/SCALib
+- **Bug reports/feature requests**: https://github.com/simple-crypto/SCALib/issues/new/choose
+- **Contributing**: https://scalib.readthedocs.io/en/stable/source/contributing.html
+
+
+SCALib focuses on
 
 - simple interface,
 - state-of-the art algorithms,
 - excellent performance (see `benchmarks <https://github.com/cassiersg/SCABench>`_).
 
 SCALib should be useful for any side-channel practitioner who wants to
 evaluate, but not necessarily attack, protected or non-protected
 implementations.
-
 See the documentation_ for the list of implemented tools.
 
-We have a `matrix chat <https://matrix.to/#/#scalib:matrix.org>`_ for
-announcements, questions, community support and discussions.
-
 .. _documentation: https://scalib.readthedocs.io/en/stable
 
 Install
 =======
 
 SCALib is on PyPi! Simple install:
 
@@ -105,18 +112,21 @@
 Contributions and Issues
 ========================
 
 Contributions welcome !
 
 Please file a **bug report** for any issue you encounter (even bad documentation is
 a bug !), and let us know your **suggestions** (open a `github issue
-<https://github.com/simple-crypto/SCALib/issues/new/choose>`_, email works too).
+<https://github.com/simple-crypto/SCALib/issues/new/choose>`_, `chat
+<https://matrix.to/#/#scalib:matrix.org>`_ and `email
+<mailto:gaetan.cassiers@uclouvain.be>`_ work too).
 We also welcome code contributions, see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_.
+You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_
+(announcements, questions, community support, open discussion, etc.).
 
 All code contributions are subject to the Contributor License Agreement (`CLA
 <https://www.simple-crypto.dev/organization>`_) of SIMPLE-Crypto, which ensures
 a thriving future for open-source hardware security.
 
 License
 =======
```

### Comparing `scalib-0.5.4/src/scalib.egg-info/SOURCES.txt` & `scalib-0.5.5/src/scalib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/source/api_ref.rst
 docs/source/changelog.rst
 docs/source/contributing.rst
 docs/source/copyright.rst
 examples/README.rst
-examples/aes_simulation.py
+examples/aes_attack.py
+examples/aes_info.py
+examples/aes_tvla.py
 examples/test_examples.py
 examples/utils.py
 paper/build_paper.sh
 paper/paper.bib
 paper/paper.md
 src/scalib/__init__.py
 src/scalib/build_config.py
```

### Comparing `scalib-0.5.4/src/scalib_ext/.gitignore` & `scalib-0.5.5/src/scalib_ext/.gitignore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/Cargo.lock` & `scalib-0.5.5/src/scalib_ext/Cargo.lock`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/build.rs` & `scalib-0.5.5/src/scalib_ext/geigen/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Cholesky` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CholmodSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Core` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Eigenvalues` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Geometry` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Householder` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Jacobi` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/LU` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/MetisSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/OrderingMethods` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PaStiXSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PardisoSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QR` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SPQRSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SVD` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Sparse` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCholesky` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCore` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseLU` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseQR` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdDeque` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdList` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdVector` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SuperLUSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/UmfPackSupport` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/Version.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/Version.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/include/geigen.h` & `scalib-0.5.5/src/scalib_ext/geigen/include/geigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/src/geigen.cpp` & `scalib-0.5.5/src/scalib_ext/geigen/src/geigen.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/src/geigen.rs` & `scalib-0.5.5/src/scalib_ext/geigen/src/geigen.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/geigen/src/lib.rs` & `scalib-0.5.5/src/scalib_ext/geigen/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/build.rs` & `scalib-0.5.5/src/scalib_ext/ranklib/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/fuzz/Cargo.toml` & `scalib-0.5.5/src/scalib_ext/ranklib/fuzz/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs` & `scalib-0.5.5/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/aes.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/aes.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_execute.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_execute.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_struct.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_struct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/histogram.rs` & `scalib-0.5.5/src/scalib_ext/ranklib/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/lib.rs` & `scalib-0.5.5/src/scalib_ext/ranklib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/main_example.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/main_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/rank.rs` & `scalib-0.5.5/src/scalib_ext/ranklib/src/rank.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/score_example_data.rs` & `scalib-0.5.5/src/scalib_ext/ranklib/src/score_example_data.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.h` & `scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example_data.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example_data.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/ranklib/src/top.cpp` & `scalib-0.5.5/src/scalib_ext/ranklib/src/top.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/Cargo.toml` & `scalib-0.5.5/src/scalib_ext/scalib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/benches/belief_propagation.rs` & `scalib-0.5.5/src/scalib_ext/scalib/benches/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/benches/get_snr.rs` & `scalib-0.5.5/src/scalib_ext/scalib/benches/get_snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/benches/mttest.rs` & `scalib-0.5.5/src/scalib_ext/scalib/benches/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/benches/snr_update.rs` & `scalib-0.5.5/src/scalib_ext/scalib/benches/snr_update.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/benches/ttest.rs` & `scalib-0.5.5/src/scalib_ext/scalib/benches/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/belief_propagation.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/lda.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/lib.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/matrixmul.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/matrixmul.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/mttest.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/belief_propagation.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/bp_compute.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/bp_compute.rs`

 * *Files 0% similar despite different names*

```diff
@@ -223,20 +223,17 @@
                 return res;
             }
             (DistrRepr::Uniform, DistrRepr::Full(v)) => (&one, v),
             (DistrRepr::Full(v), DistrRepr::Uniform) => (v, &one),
             (DistrRepr::Full(vst), DistrRepr::Full(vdiv)) => (vst, vdiv),
         };
         res.value = DistrRepr::Full(
-            Zip::from(
-                vst.broadcast((std::cmp::max(vst.dim().0, vdiv.dim().0), vst.dim().1))
-                    .unwrap(),
-            )
-            .and_broadcast(vdiv)
-            .map_collect(|vst, vdiv| *vst / (*vdiv + MIN_PROBA)),
+            Zip::from(vst.broadcast((res.shape.0, vst.dim().1)).unwrap())
+                .and_broadcast(vdiv)
+                .map_collect(|vst, vdiv| *vst / (*vdiv + MIN_PROBA)),
         );
         return res;
     }
     pub fn dividing_full(&mut self, other: &Distribution) {
         match (&mut self.value, &other.value) {
             (DistrRepr::Full(div), DistrRepr::Full(st)) => {
                 ndarray::azip!(div, st).for_each(|div, st| *div = *st / *div);
```

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/factor_graph.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/factor_graph.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_build.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_parser.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_parser.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/mod.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/mod.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/snr.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/ttest.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/src/utils.rs` & `scalib-0.5.5/src/scalib_ext/scalib/src/utils.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/tests/lda.rs` & `scalib-0.5.5/src/scalib_ext/scalib/tests/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/tests/multivarcs.rs` & `scalib-0.5.5/src/scalib_ext/scalib/tests/multivarcs.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib/tests/ttest.rs` & `scalib-0.5.5/src/scalib_ext/scalib/tests/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/Cargo.toml` & `scalib-0.5.5/src/scalib_ext/scalib-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/belief_propagation.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/factor_graph.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/factor_graph.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/lda.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/lib.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/ranking.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/ranking.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/snr.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/thread_pool.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/thread_pool.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/src/scalib_ext/scalib-py/src/ttest.rs` & `scalib-0.5.5/src/scalib_ext/scalib-py/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/tests/mttest_test.py` & `scalib-0.5.5/tests/mttest_test.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/tests/test_factorgraph.py` & `scalib-0.5.5/tests/test_factorgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -932,7 +932,63 @@
 
     distri_y_ref = np.log2(distri_x).sum(axis=0, keepdims=True)
     distri_y_ref = distri_y_ref - np.max(distri_y_ref[0, :])
     distri_y_ref = 2**distri_y_ref
     distri_y_ref = distri_y_ref / distri_y_ref.sum(axis=1, keepdims=True)
 
     assert np.allclose(distri_y_ref, distri_y, rtol=1e-5, atol=1e-19)
+
+
+def test_mix_single_multi():
+    graph_desc = """
+    NC 2
+    TABLE t
+    VAR SINGLE s
+
+    VAR MULTI a
+    VAR MULTI b
+
+    PROPERTY TABLE: a = t[s]
+    PROPERTY XOR: b = a ^ s
+    """
+
+    graph_desc2 = """
+    NC 2
+    TABLE t
+    VAR SINGLE s
+
+    VAR SINGLE a0
+    VAR SINGLE b0
+
+    PROPERTY a0 = t[s]
+    PROPERTY b0 = a0 ^ s
+
+    VAR SINGLE a1
+    VAR SINGLE b1
+
+    PROPERTY a1 = t[s]
+    PROPERTY b1 = a1 ^ s
+    """
+
+    graph = FactorGraph(graph_desc, {"t": np.arange(2, dtype=np.uint32)})
+    graph2 = FactorGraph(graph_desc2, {"t": np.arange(2, dtype=np.uint32)})
+
+    sasca = BPState(graph, 2)
+    sasca.bp_loopy(4, initialize_states=True)  # check no crash
+
+    sasca = BPState(graph, 2)
+    sasca2 = BPState(graph2, 1)
+
+    for _ in range(10):
+        sasca.bp_loopy(1, initialize_states=False)
+        sasca2.bp_loopy(1, initialize_states=False)
+        for v in ("a", "b"):
+            d = sasca.get_distribution(v)
+            d0 = sasca2.get_distribution(f"{v}0")
+            d1 = sasca2.get_distribution(f"{v}0")
+            if d is not None:
+                assert np.allclose(d[0, :], d0, rtol=1e-5, atol=1e-19)
+                assert np.allclose(d[1, :], d1, rtol=1e-5, atol=1e-19)
+        d = sasca.get_distribution("s")
+        d2 = sasca2.get_distribution("s")
+        if d is not None:
+            assert np.allclose(d, d2, rtol=1e-5, atol=1e-19)
```

### Comparing `scalib-0.5.4/tests/test_lda.py` & `scalib-0.5.5/tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/tests/test_sascagraph.py` & `scalib-0.5.5/tests/test_sascagraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import pytest
 from scalib.attacks import SASCAGraph
 import numpy as np
 import os
 
+pytestmark = pytest.mark.filterwarnings(
+    "ignore:.*:DeprecationWarning:scalib.attacks.sacagraph"
+)
+
 
 def test_table():
     """
     Test Table lookup
     """
     nc = 16
     n = 100
```

### Comparing `scalib-0.5.4/tests/test_snr.py` & `scalib-0.5.5/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/tests/test_tools.py` & `scalib-0.5.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.4/tests/test_ttest.py` & `scalib-0.5.5/tests/test_ttest.py`

 * *Files 11% similar despite different names*

```diff
@@ -108,7 +108,24 @@
     traces += m[labels]
 
     t_ref = reference(traces, labels, d)
     ttest = Ttest(ns, d)
     ttest.fit_u(traces, labels)
     t = ttest.get_ttest()
     assert np.allclose(t_ref, t, rtol=1e-3)
+
+
+def test_ttest_data_transpose():
+    ns = 100
+    d = 1
+    nc = 2
+    n = 200
+
+    m = np.random.randint(0, 2, (nc, ns))
+    traces = np.asfortranarray(np.random.randint(0, 10, (n, ns), dtype=np.int16))
+    labels = np.random.randint(0, nc, n, dtype=np.uint16)
+    traces += m[labels]
+
+    t_ref = reference(traces, labels, d)
+    ttest = Ttest(ns, 1)
+    with pytest.raises(ValueError):
+        ttest.fit_u(traces, labels)
```

### Comparing `scalib-0.5.4/tox.ini` & `scalib-0.5.5/tox.ini`

 * *Files identical despite different names*

