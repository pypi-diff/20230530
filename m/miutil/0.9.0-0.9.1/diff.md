# Comparing `tmp/miutil-0.9.0.tar.gz` & `tmp/miutil-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miutil-0.9.0.tar", last modified: Fri Sep 10 00:40:21 2021, max compression
+gzip compressed data, was "miutil-0.9.1.tar", last modified: Sat Oct 30 00:38:37 2021, max compression
```

## Comparing `miutil-0.9.0.tar` & `miutil-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.980688 miutil-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.976688 miutil-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.976688 miutil-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2021-09-10 00:40:12.000000 miutil-0.9.0/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2021-09-10 00:40:12.000000 miutil-0.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-09-10 00:40:12.000000 miutil-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-09-10 00:40:12.000000 miutil-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-09-10 00:40:12.000000 miutil-0.9.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-10 00:40:12.000000 miutil-0.9.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-09-10 00:40:21.980688 miutil-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-09-10 00:40:12.000000 miutil-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.976688 miutil-0.9.0/miutil/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil/_dist_ver.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2850 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/cuinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/fdio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.980688 miutil-0.9.0/miutil/imio/
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/imio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11292 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/imio/nii.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.980688 miutil-0.9.0/miutil/mlab/
--rw-r--r--   0 runner    (1001) docker     (121)     8467 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/mlab/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1531 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/mlab/beautify.py
--rw-r--r--   0 runner    (1001) docker     (121)     6285 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-09-10 00:40:12.000000 miutil-0.9.0/miutil/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.980688 miutil-0.9.0/miutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-10 00:40:21.000000 miutil-0.9.0/miutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-09-10 00:40:12.000000 miutil-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2021-09-10 00:40:21.980688 miutil-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-10 00:40:12.000000 miutil-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:21.980688 miutil-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-10 00:40:12.000000 miutil-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-09-10 00:40:12.000000 miutil-0.9.0/tests/test_cuinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-09-10 00:40:12.000000 miutil-0.9.0/tests/test_fdio.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2021-09-10 00:40:12.000000 miutil-0.9.0/tests/test_imio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-09-10 00:40:12.000000 miutil-0.9.0/tests/test_mlab.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-09-10 00:40:12.000000 miutil-0.9.0/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.496734 miutil-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.492734 miutil-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.492734 miutil-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2021-10-30 00:38:30.000000 miutil-0.9.1/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3728 2021-10-30 00:38:30.000000 miutil-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-30 00:38:30.000000 miutil-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-10-30 00:38:30.000000 miutil-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-10-30 00:38:30.000000 miutil-0.9.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-10-30 00:38:30.000000 miutil-0.9.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4041 2021-10-30 00:38:37.496734 miutil-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-10-30 00:38:30.000000 miutil-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.492734 miutil-0.9.1/miutil/
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil/_dist_ver.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2801 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/cuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/fdio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.496734 miutil-0.9.1/miutil/imio/
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/imio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11286 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/imio/nii.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.496734 miutil-0.9.1/miutil/mlab/
+-rw-r--r--   0 runner    (1001) docker     (121)     7762 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/mlab/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1530 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/mlab/beautify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3402 2021-10-30 00:38:30.000000 miutil-0.9.1/miutil/web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.496734 miutil-0.9.1/miutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4041 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-30 00:38:37.000000 miutil-0.9.1/miutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-10-30 00:38:30.000000 miutil-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2021-10-30 00:38:37.496734 miutil-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-10-30 00:38:30.000000 miutil-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:37.496734 miutil-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 00:38:30.000000 miutil-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-10-30 00:38:30.000000 miutil-0.9.1/tests/test_cuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2021-10-30 00:38:30.000000 miutil-0.9.1/tests/test_fdio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2021-10-30 00:38:30.000000 miutil-0.9.1/tests/test_imio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-10-30 00:38:30.000000 miutil-0.9.1/tests/test_mlab.py
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2021-10-30 00:38:30.000000 miutil-0.9.1/tests/test_web.py
```

### Comparing `miutil-0.9.0/.github/workflows/comment-bot.yml` & `miutil-0.9.1/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/.github/workflows/test.yml` & `miutil-0.9.1/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 name: Test
-on: [push, pull_request]
+on:
+  push:
+  pull_request:
+  schedule:
+  - cron: '15 23 * * 6'  # M H d m w (Sat at 23:15)
 jobs:
   check:
-    if: github.event_name != 'pull_request' || github.head_ref != 'devel'
+    if: github.event_name != 'pull_request' || github.repository_owner != 'AMYPAD'
     runs-on: ubuntu-latest
-    name: Check
     steps:
     - uses: actions/checkout@v2
-      with:
-        fetch-depth: 0
     - uses: actions/setup-python@v2
     - name: set PYSHA
       run: echo "PYSHA=$(python -VV | sha256sum | cut -d' ' -f1)" >> $GITHUB_ENV
     - uses: actions/cache@v1
       with:
         path: ~/.cache/pre-commit
         key: pre-commit|${{ env.PYSHA }}|${{ hashFiles('.pre-commit-config.yaml') }}
     - name: dependencies
       run: pip install -U pre-commit
     - uses: reviewdog/action-setup@v1
-    - if: github.event_name != 'schedule'
+    - if: github.event_name == 'push' || github.event_name == 'pull_request'
       name: comment
       run: |
         if [[ $EVENT == pull_request ]]; then
           REPORTER=github-pr-review
         else
           REPORTER=github-check
         fi
         pre-commit run -a todo | reviewdog -efm="%f:%l: %m" -name=TODO -tee -reporter=$REPORTER -filter-mode nofilter
         pre-commit run -a flake8 | reviewdog -f=pep8 -name=flake8 -tee -reporter=$REPORTER -filter-mode nofilter
       env:
         REVIEWDOG_GITHUB_API_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         EVENT: ${{ github.event_name }}
     - run: pre-commit run -a --show-diff-on-failure
   test:
-    if: github.event_name != 'pull_request' || github.head_ref != 'devel'
+    if: github.event_name != 'pull_request' || github.repository_owner != 'AMYPAD'
+    name: py${{ matrix.python }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: [2.7, 3.6, 3.9]
-    name: Test py${{ matrix.python }}
     steps:
     - uses: actions/checkout@v2
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python }}
     - run: pip install -U .[dev,nii,web]
     - if: startsWith(matrix.python, '3')
       run: pytest --durations-min=1
     - if: startsWith(matrix.python, '2')
       run: pytest
-    - run: codecov
+    - uses: codecov/codecov-action@v1
   cuda_matlab:
-    if: github.event_name != 'pull_request' || github.head_ref != 'devel'
+    if: github.event_name != 'pull_request' || github.repository_owner != 'AMYPAD'
+    name: CUDA MATLAB py${{ matrix.python }}
     runs-on: [self-hosted, python, cuda, matlab]
-    name: Test cuda & matlab
+    strategy:
+      matrix:
+        python: [3.7, 3.9]
     steps:
     - uses: actions/checkout@v2
       with:
         fetch-depth: 0
     - name: Run setup-python
-      run: setup-python -p3.7
+      run: setup-python -p${{ matrix.python }}
     - run: pip install -U .[dev,nii,cuda,web,mbeautify]
     - run: pytest --durations-min=1
-    - run: codecov
+    - uses: codecov/codecov-action@v1
     - name: Post Run setup-python
-      run: setup-python -p3.7 -Dr
+      run: setup-python -p${{ matrix.python }} -Dr
       if: ${{ always() }}
   deploy:
     needs: [check, test, cuda_matlab]
     name: PyPI Deploy
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v2
```

### Comparing `miutil-0.9.0/.pre-commit-config.yaml` & `miutil-0.9.1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -31,15 +31,16 @@
   - id: flake8
     args: [-j8]
     additional_dependencies:
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-debugger
     - flake8-string-format
-- repo: https://github.com/psf/black
-  rev: 21.8b0
+- repo: https://github.com/google/yapf
+  rev: v0.31.0
   hooks:
-  - id: black
+  - id: yapf
+    args: [-i]
 - repo: https://github.com/PyCQA/isort
   rev: 5.9.3
   hooks:
   - id: isort
```

### Comparing `miutil-0.9.0/LICENCE.md` & `miutil-0.9.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/PKG-INFO` & `miutil-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,17 @@
 Metadata-Version: 2.1
 Name: miutil
-Version: 0.9.0
+Version: 0.9.1
 Summary: Medical imaging utilities for the AMYPAD and NiftyPET projects
 Home-page: https://github.com/AMYPAD/miutil
 Maintainer: Casper da Costa-Luis
 Maintainer-email: casper.dcl@physics.org
 License: Apache-2.0
 Project-URL: Changelog, https://github.com/AMYPAD/miutil/releases
 Project-URL: Documentation, https://github.com/AMYPAD/miutil/#miutil
-Description: miutil
-        ======
-        
-        Medical imaging utilities.
-        
-        |Version| |Py-Versions| |Conda| |Tests| |Coverage| |DOI| |LICENCE|
-        
-        Basic functionality needed for `AMYPAD <https://github.com/AMYPAD/AMYPAD>`_
-        and `NiftyPET <https://github.com/NiftyPET/NiftyPET>`_.
-        
-        
-        Install
-        -------
-        
-        Intended for inclusion in requirements for other packages.
-        The package name is ``miutil``. Extra install options include:
-        
-        - cuda
-        
-          - provides `miutil.cuinfo <https://github.com/AMYPAD/miutil/blob/master/miutil/cuinfo.py>`_
-        
-        - mbeautify
-        
-          - provides `miutil.mlab.beautify <https://github.com/AMYPAD/miutil/blob/master/miutil/mlab/beautify.py>`_
-        
-        - nii
-        
-          - provides `miutil.imio.nii <https://github.com/AMYPAD/miutil/blob/master/miutil/imio/nii.py>`_
-        
-        - plot
-        
-          - provides `miutil.plot <https://github.com/AMYPAD/miutil/blob/master/miutil/plot.py>`_
-        
-            - includes a useful 3D multi-volume ``imscroll`` function which depends only on ``matplotlib``
-        
-        - web
-        
-          - provides `miutil.web <https://github.com/AMYPAD/miutil/blob/master/miutil/web.py>`_
-        
-        
-        To install extras and their dependencies,
-        use the package name ``miutil[option1,option2]``.
-        
-        
-        .. |Tests| image:: https://img.shields.io/github/workflow/status/AMYPAD/miutil/Test?logo=GitHub
-           :target: https://github.com/AMYPAD/miutil/actions
-        .. |Coverage| image:: https://codecov.io/gh/AMYPAD/miutil/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/AMYPAD/miutil
-        .. |Version| image:: https://img.shields.io/pypi/v/miutil.svg?logo=python&logoColor=white
-           :target: https://github.com/AMYPAD/miutil/releases
-        .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/miutil.svg?logo=python&logoColor=white
-           :target: https://pypi.org/project/miutil
-        .. |Conda| image:: https://img.shields.io/conda/v/conda-forge/miutil.svg?label=conda&logo=conda-forge
-           :target: https://anaconda.org/conda-forge/miutil
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4281542.svg
-           :target: https://doi.org/10.5281/zenodo.4281542
-        .. |LICENCE| image:: https://img.shields.io/pypi/l/miutil.svg
-           :target: https://raw.githubusercontent.com/AMYPAD/miutil/master/LICENCE.md
-        
 Keywords: fMRI,PET,SPECT,EEG,MEG
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Education
@@ -98,7 +39,69 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: nii
 Provides-Extra: plot
 Provides-Extra: cuda
 Provides-Extra: web
 Provides-Extra: mbeautify
+License-File: LICENCE.md
+
+miutil
+======
+
+Medical imaging utilities.
+
+|Version| |Py-Versions| |Conda| |Tests| |Coverage| |DOI| |LICENCE|
+
+Basic functionality needed for `AMYPAD <https://github.com/AMYPAD/AMYPAD>`_
+and `NiftyPET <https://github.com/NiftyPET/NiftyPET>`_.
+
+
+Install
+-------
+
+Intended for inclusion in requirements for other packages.
+The package name is ``miutil``. Extra install options include:
+
+- cuda
+
+  - provides `miutil.cuinfo <https://github.com/AMYPAD/miutil/blob/master/miutil/cuinfo.py>`_
+
+- mbeautify
+
+  - provides `miutil.mlab.beautify <https://github.com/AMYPAD/miutil/blob/master/miutil/mlab/beautify.py>`_
+
+- nii
+
+  - provides `miutil.imio.nii <https://github.com/AMYPAD/miutil/blob/master/miutil/imio/nii.py>`_
+
+- plot
+
+  - provides `miutil.plot <https://github.com/AMYPAD/miutil/blob/master/miutil/plot.py>`_
+
+    - includes a useful 3D multi-volume ``imscroll`` function which depends only on ``matplotlib``
+
+- web
+
+  - provides `miutil.web <https://github.com/AMYPAD/miutil/blob/master/miutil/web.py>`_
+
+
+To install extras and their dependencies,
+use the package name ``miutil[option1,option2]``.
+
+
+.. |Tests| image:: https://img.shields.io/github/workflow/status/AMYPAD/miutil/Test?logo=GitHub
+   :target: https://github.com/AMYPAD/miutil/actions
+.. |Coverage| image:: https://codecov.io/gh/AMYPAD/miutil/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/AMYPAD/miutil
+.. |Version| image:: https://img.shields.io/pypi/v/miutil.svg?logo=python&logoColor=white
+   :target: https://github.com/AMYPAD/miutil/releases
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/miutil.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/miutil
+.. |Conda| image:: https://img.shields.io/conda/v/conda-forge/miutil.svg?label=conda&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/miutil
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4281542.svg
+   :target: https://doi.org/10.5281/zenodo.4281542
+.. |LICENCE| image:: https://img.shields.io/pypi/l/miutil.svg
+   :target: https://raw.githubusercontent.com/AMYPAD/miutil/master/LICENCE.md
+
+
```

### Comparing `miutil-0.9.0/README.rst` & `miutil-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/miutil/cuinfo.py` & `miutil-0.9.1/miutil/cuinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 __all__ = ["num_devices", "compute_capability", "memory", "name", "nvcc_flags"]
 
 
 def nvmlDeviceGetCudaComputeCapability(handle):
     major = pynvml.c_int()
     minor = pynvml.c_int()
-    try:  # pynvml>=11
+    try:      # pynvml>=11
         get_fn = pynvml.nvml._nvmlGetFunctionPointer
     except AttributeError:
         get_fn = pynvml.get_func_pointer
     fn = get_fn("nvmlDeviceGetCudaComputeCapability")
     ret = fn(handle, pynvml.byref(major), pynvml.byref(minor))
-    try:  # pynvml>=11
+    try:      # pynvml>=11
         check_ret = pynvml.nvml._nvmlCheckReturn
     except AttributeError:
         check_ret = pynvml.check_return
     check_ret(ret)
     return [major.value, minor.value]
 
 
@@ -62,16 +62,15 @@
 def name(dev_id=-1):
     """returns device name"""
     return pynvml.nvmlDeviceGetName(get_handle(dev_id)).decode("U8")
 
 
 def nvcc_flags(dev_id=-1):
     return "-gencode=arch=compute_{0:d}{1:d},code=compute_{0:d}{1:d}".format(
-        *compute_capability(dev_id)
-    )
+        *compute_capability(dev_id))
 
 
 def main(*args, **kwargs):
     args = argopt(__doc__).parse_args(*args, **kwargs)
     noargs = True
     devices = range(num_devices()) if args.dev_id is None else [args.dev_id]
 
@@ -82,16 +81,13 @@
         print(" ".join(sorted(set(map(nvcc_flags, devices)))[::-1]))
         noargs = False
     if args.compute:
         print(" ".join(sorted({"%d%d" % compute_capability(i) for i in devices})[::-1]))
         noargs = False
     if noargs:
         for dev_id in devices:
-            print(
-                "Device {:2d}:{}:compute capability:{:d}.{:d}".format(
-                    dev_id, name(dev_id), *compute_capability(dev_id)
-                )
-            )
+            print("Device {:2d}:{}:compute capability:{:d}.{:d}".format(
+                dev_id, name(dev_id), *compute_capability(dev_id)))
 
 
-if __name__ == "__main__":  # pragma: no cover
+if __name__ == "__main__": # pragma: no cover
     main()
```

### Comparing `miutil-0.9.0/miutil/fdio.py` & `miutil-0.9.1/miutil/fdio.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,35 +53,34 @@
     rmtree(d)
 
 
 def extractall(fzip, dest, desc="Extracting"):
     """zipfile.Zipfile(fzip).extractall(dest) with progress"""
     dest = Path(dest).expanduser()
     with ZipFile(fzip) as zipf, tqdm(
-        desc=desc,
-        unit="B",
-        unit_scale=True,
-        unit_divisor=1024,
-        total=sum(getattr(i, "file_size", 0) for i in zipf.infolist()),
+            desc=desc,
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+            total=sum(getattr(i, "file_size", 0) for i in zipf.infolist()),
     ) as pbar:
         for i in zipf.infolist():
-            if not getattr(i, "file_size", 0):  # directory
+            if not getattr(i, "file_size", 0): # directory
                 zipf.extract(i, fspath(dest))
             else:
                 (dest / i.filename).parent.mkdir(parents=True, exist_ok=True)
                 with zipf.open(i) as fi, (dest / i.filename).open(mode="wb") as fo:
                     copyfileobj(CallbackIOWrapper(pbar.update, fi), fo)
                 mode = (i.external_attr >> 16) & 0o777
                 if mode:
                     (dest / i.filename).chmod(mode)
                     log.debug(oct((i.external_attr >> 16) & 0o777))
 
 
 def nsort(fnames):
     """Sort a file list, automatically detecting embedded numbers"""
-
     def path2parts(fname):
         parts = re.split(r"([0-9][0-9.]*e[-+][0-9]+|[0-9]+\.[0-9]+|[0-9]+)", fname)
         parts[1::2] = map(float, parts[1::2])
         return parts
 
     return sorted(fnames, key=path2parts)
```

### Comparing `miutil-0.9.0/miutil/imio/__init__.py` & `miutil-0.9.1/miutil/imio/__init__.py`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/miutil/imio/nii.py` & `miutil-0.9.1/miutil/imio/nii.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """NIfTI I/O"""
 import gzip
 import logging
 import numbers
 import os.path
 import re
+import sys
 
 import nibabel as nib
 import numpy as np
-from six import string_types
 
 from ..fdio import create_dir, fspath, hasext
 from . import RE_NII_GZ
 
 RE_GZ = re.compile(r"^(.+)(\.gz)$", flags=re.I)
 log = logging.getLogger(__name__)
+if sys.version_info[0] < 3:
+    string_types = basestring, # NOQA: F821
+else:
+    string_types = str,
 
 
 def file_parts(fname, regex=RE_NII_GZ):
     """/path/file.nii.gz -> /path, file, .nii.gz"""
     fname = fspath(fname)
     base = os.path.basename(fname)
     root, ext = regex.search(base).groups()
@@ -82,50 +86,39 @@
 
         # > get orientations from the affine
         ornt = nib.io_orientation(nim.affine)
         trnsp = tuple(2 - np.int8(ornt[:, 0]))
         flip = tuple(np.int8(ornt[:, 1]))
 
         # > voxel size
-        voxsize = nim.header.get("pixdim")[1 : nim.header.get("dim")[0] + 1]
+        voxsize = nim.header.get("pixdim")[1:nim.header.get("dim")[0] + 1]
         # > rearrange voxel size according to the orientation
         voxsize = voxsize[np.array(trnsp)]
 
         # > dimensions
-        dims = dim[1 : nim.header.get("dim")[0] + 1]
+        dims = dim[1:nim.header.get("dim")[0] + 1]
         dims = dims[np.array(trnsp)]
 
         # > flip y-axis and z-axis and then transpose.
         # Depends if dynamic (4 dimensions) or static (3 dimensions)
         if dimno == 4:
-            imr = np.transpose(
-                imr[:: -flip[0], :: -flip[1], :: -flip[2], :], (3,) + trnsp
-            )
+            imr = np.transpose(imr[::-flip[0], ::-flip[1], ::-flip[2], :], (3,) + trnsp)
         elif dimno == 3:
-            imr = np.transpose(imr[:: -flip[0], :: -flip[1], :: -flip[2]], trnsp)
+            imr = np.transpose(imr[::-flip[0], ::-flip[1], ::-flip[2]], trnsp)
 
     if output == "affine" or output == "all":
         # A = nim.get_sform()
         # if not A[:3,:3].any():
         #     A = nim.get_qform()
         A = nim.affine
 
     if output == "all":
         out = {
-            "im": imr,
-            "affine": A,
-            "fim": fim,
-            "dtype": nim.get_data_dtype(),
-            "shape": imr.shape,
-            "hdr": nim.header,
-            "voxsize": voxsize,
-            "dims": dims,
-            "transpose": trnsp,
-            "flip": flip,
-        }
+            "im": imr, "affine": A, "fim": fim, "dtype": nim.get_data_dtype(), "shape": imr.shape,
+            "hdr": nim.header, "voxsize": voxsize, "dims": dims, "transpose": trnsp, "flip": flip}
     elif output == "image":
         out = imr
     elif output == "affine":
         out = A
     else:
         raise NameError("Unrecognised output request!")
 
@@ -157,19 +150,15 @@
 
     # ---------------------------------------------------------------------------
     # > TRANSLATIONS and FLIPS
     # > get the same geometry as the input NIfTI file in the form of dictionary,
     # >>as obtained from getnii(..., output='all')
 
     # > permute the axis order in the image array
-    if (
-        isinstance(storage_as, dict)
-        and "transpose" in storage_as
-        and "flip" in storage_as
-    ):
+    if (isinstance(storage_as, dict) and "transpose" in storage_as and "flip" in storage_as):
 
         trnsp = (
             storage_as["transpose"].index(0),
             storage_as["transpose"].index(1),
             storage_as["transpose"].index(2),
         )
 
@@ -182,20 +171,20 @@
         trnsp = tuple([t + 1 for t in trnsp] + [0])
         im = im.transpose(trnsp)
     else:
         im = im.transpose(trnsp)
 
     # > perform flip of x,y,z axes after transposition into proper NIfTI order
     if len(flip) == 3:
-        im = im[:: -flip[0], :: -flip[1], :: -flip[2], ...]
+        im = im[::-flip[0], ::-flip[1], ::-flip[2], ...]
 
     res = nib.Nifti1Image(im, A)
     hdr = res.header
     hdr.set_sform(None, code="scanner")
-    hdr["cal_max"] = np.max(im)  # np.percentile(im, 90) #
+    hdr["cal_max"] = np.max(im) # np.percentile(im, 90) #
     hdr["cal_min"] = np.min(im)
     hdr["descrip"] = descrip
     nib.save(res, fspath(fnii))
 
 
 def niisort(fims, memlim=True):
     """
@@ -262,20 +251,16 @@
     if _nii and datype.count(_nii.get_data_dtype()) != len(datype):
         raise TypeError("Input images are of different data types.")
     # image shape must be 3D
     if _nii and len(_nii.shape) != 3:
         raise ValueError("Input image(s) must be 3D.")
 
     out = {
-        "shape": _nii.shape[::-1],
-        "files": _fims,
-        "sortlist": sortlist,
-        "dtype": _nii.get_data_dtype(),
-        "N": Nim,
-    }
+        "shape": _nii.shape[::-1], "files": _fims, "sortlist": sortlist,
+        "dtype": _nii.get_data_dtype(), "N": Nim}
 
     if memlim and Nfrm > 50:
         imdic = getnii(_fims[0], output="all")
         affine = imdic["affine"]
     else:
         # get the images into an array
         _imin = np.zeros((Nfrm,) + _nii.shape[::-1], dtype=_nii.get_data_dtype())
@@ -324,20 +309,19 @@
             fcomment = "_nimpa-modified"
         fout = file_parts(fnii)[1] + fcomment + ".nii.gz"
     else:
         fout = os.path.splitext(fimout)[0] + ".nii.gz"
     log.debug("output floating and affine file names:%s", fout)
     fout = os.path.join(opth, fout)
 
-    if len(voxel_range) == 1:  # set max value
+    if len(voxel_range) == 1:                                               # set max value
         im = voxel_range[0] * dctnii["im"] / np.max(dctnii["im"])
-    elif len(voxel_range) == 2:  # set range
-        im = (dctnii["im"] - np.min(dctnii["im"])) * (
-            np.ptp(voxel_range) / np.ptp(dctnii["im"])
-        ) + voxel_range[0]
+    elif len(voxel_range) == 2:                                             # set range
+        im = (dctnii["im"] - np.min(dctnii["im"])) * (np.ptp(voxel_range) /
+                                                      np.ptp(dctnii["im"])) + voxel_range[0]
     else:
         return None
 
     # > output file name for the extra reference image
     array2nii(
         im,
         dctnii["affine"],
```

### Comparing `miutil-0.9.0/miutil/mlab/__init__.py` & `miutil-0.9.1/miutil/mlab/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,45 +13,37 @@
 except ImportError:
     from backports.functools_lru_cache import lru_cache
 try:
     FileNotFoundError
 except NameError:
     FileNotFoundError = OSError
 
-
 from ..fdio import Path, extractall, fspath, tmpdir
 
 __all__ = ["get_engine"]
 IS_WIN = any(sys.platform.startswith(i) for i in ["win32", "cygwin"])
 MATLAB_RUN = "matlab -nodesktop -nosplash -nojvm".split()
 if IS_WIN:
     MATLAB_RUN += ["-wait", "-log"]
 log = logging.getLogger(__name__)
 _MCR_URL = {
-    99: (
-        "https://ssd.mathworks.com/supportfiles/downloads/R2020b/Release/4"
-        "/deployment_files/installer/complete/"
-    ),
-    713: "https://www.fil.ion.ucl.ac.uk/spm/download/restricted/utopia/MCR/",
-}
+    99: ("https://ssd.mathworks.com/supportfiles/downloads/R2020b/Release/4"
+         "/deployment_files/installer/complete/"),
+    713: "https://www.fil.ion.ucl.ac.uk/spm/download/restricted/utopia/MCR/"}
 MCR_ARCH = {"Windows": "win64", "Linux": "glnxa64", "Darwin": "maci64"}[system()]
 MCR_URL = {
     "Windows": {
         99: _MCR_URL[99] + "win64/MATLAB_Runtime_R2020b_Update_4_win64.zip",
-        713: _MCR_URL[713] + "win64/MCRInstaller.exe",
-    },
+        713: _MCR_URL[713] + "win64/MCRInstaller.exe"},
     "Linux": {
         99: _MCR_URL[99] + "glnxa64/MATLAB_Runtime_R2020b_Update_4_glnxa64.zip",
-        713: _MCR_URL[713] + "glnxa64/MCRInstaller.bin",
-    },
+        713: _MCR_URL[713] + "glnxa64/MCRInstaller.bin"},
     "Darwin": {
         99: _MCR_URL[99] + "maci64/MATLAB_Runtime_R2020b_Update_4_maci64.dmg.zip",
-        713: _MCR_URL[713] + "maci64/MCRInstaller.dmg",
-    },
-}[system()]
+        713: _MCR_URL[713] + "maci64/MCRInstaller.dmg"}}[system()] # yapf: disable
 
 
 class VersionError(ValueError):
     pass
 
 
 def check_output_u8(*args, **kwargs):
@@ -68,27 +60,23 @@
 @lru_cache()
 def get_engine(name=None):
     try:
         from matlab import engine
     except ImportError:
         try:
             log.warning(
-                dedent(
-                    """\
+                dedent("""\
                 Python could not find the MATLAB engine.
-                Attempting to install automatically."""
-                )
-            )
+                Attempting to install automatically."""))
             log.debug(_install_engine())
             log.info("installed MATLAB engine for Python")
             from matlab import engine
         except CalledProcessError:
             raise ImportError(
-                dedent(
-                    """\
+                dedent("""\
                 Please install MATLAB and its Python module.
                 See https://www.mathworks.com/help/matlab/matlab_external/\
 install-the-matlab-engine-for-python.html
                 or
                 https://www.mathworks.com/help/matlab/matlab_external/\
 install-matlab-engine-api-for-python-in-nondefault-locations.html
                 It's likely you need to do:
@@ -98,36 +86,31 @@
 
                 - Fill in any temporary directory name for BUILDDIR
                   (e.g. /tmp/builddir).
                 - If installation fails due to write permissions, try appending `--user`
                   to the above command.
 
                 Alternatively, use `get_runtime()` instead of `get_engine()`.
-                """
-                ).format(
-                    matlabroot=matlabroot(default="matlabroot"), exe=sys.executable
-                )
-            )
+                """).format(matlabroot=matlabroot(default="matlabroot"), exe=sys.executable))
     started = engine.find_matlab()
     notify = False
     if not started or (name and name not in started):
         notify = True
         log.debug("Starting MATLAB")
     eng = engine.connect_matlab(name=name or getenv("SPM12_MATLAB_ENGINE", None))
     if notify:
         log.debug("MATLAB started")
     return eng
 
 
 def _matlab_run(command, jvm=False, auto_exit=True):
     if auto_exit and not command.endswith("exit"):
         command = command + ", exit"
-    return check_output_u8(
-        MATLAB_RUN + ([] if jvm else ["-nojvm"]) + ["-r", command], stderr=STDOUT
-    )
+    return check_output_u8(MATLAB_RUN + ([] if jvm else ["-nojvm"]) + ["-r", command],
+                           stderr=STDOUT)
 
 
 def matlabroot(default=None):
     if IS_WIN:
         try:
             res = _matlab_run("display(matlabroot);")
         except (CalledProcessError, FileNotFoundError):
@@ -143,107 +126,81 @@
             return default
         raise
     return re.search(r"MATLAB\s+=\s+(\S+)\s*$", res, flags=re.M).group(1)
 
 
 def _install_engine():
     src = path.join(matlabroot(), "extern", "engines", "python")
-    with open(path.join(src, "setup.py")) as fd:  # check version support
+    with open(path.join(src, "setup.py")) as fd: # check version support
         supported = literal_eval(
-            re.search(r"supported_version.*?=\s*(.*?)$", fd.read(), flags=re.M).group(1)
-        )
+            re.search(r"supported_version.*?=\s*(.*?)$", fd.read(), flags=re.M).group(1))
         if ".".join(map(str, sys.version_info[:2])) not in map(str, supported):
             raise VersionError(
-                dedent(
-                    """\
+                dedent("""\
                 Python version is {info[0]}.{info[1]},
                 but the installed MATLAB only supports Python versions: [{supported}]
-                """.format(
-                        info=sys.version_info[:2], supported=", ".join(supported)
-                    )
-                )
-            )
+                """.format(info=sys.version_info[:2], supported=", ".join(supported))))
     with tmpdir() as td:
         cmd = [sys.executable, "setup.py", "build", "--build-base", td, "install"]
         try:
             return check_output_u8(cmd, cwd=src)
         except CalledProcessError:
             log.warning("Normal install failed. Attempting `--user` install.")
             return check_output_u8(cmd + ["--user"], cwd=src)
 
 
 @lru_cache()
 def get_runtime(cache="~/.mcr", version=99):
     cache = Path(cache).expanduser()
     mcr_root = cache
-    i = mcr_root / ("v%d" % version)
+    i = mcr_root / ("v%d"%version)
     if i.is_dir():
         mcr_root = i
     else:
         from miutil.web import urlopen_cached
 
         log.info("Downloading to %s", cache)
         with tmpdir() as td:
             with urlopen_cached(MCR_URL[version], cache) as fd:
                 if MCR_URL[version].endswith(".zip"):
                     extractall(fd, td)
             log.info("Installing ... (may take a few min)")
             if version == 99:
-                check_output_u8(
-                    [
-                        fspath(
-                            Path(td) / ("setup" if system() == "Windows" else "install")
-                        ),
-                        "-mode",
-                        "silent",
-                        "-agreeToLicense",
-                        "yes",
-                        "-destinationFolder",
-                        fspath(mcr_root),
-                    ]
-                )
+                check_output_u8([
+                    fspath(Path(td) / ("setup" if system() == "Windows" else "install")), "-mode",
+                    "silent", "-agreeToLicense", "yes", "-destinationFolder",
+                    fspath(mcr_root)])
             elif version == 713:
                 install = cache / MCR_URL[version].rsplit("/", 1)[-1]
                 if system() == "Linux":
                     install.chmod(0o755)
-                    check_output_u8(
-                        [
-                            fspath(install),
-                            "-P",
-                            'bean421.installLocation="%s"' % fspath(cache),
-                            "-silent",
-                        ]
-                    )
+                    check_output_u8([
+                        fspath(install), "-P",
+                        'bean421.installLocation="%s"' % fspath(cache), "-silent"])
                 else:
                     raise NotImplementedError(
-                        dedent(
-                            """\
+                        dedent("""\
                         Don't yet know how to handle
                         {}
                         for {!r}.
-                        """
-                        ).format(fspath(install), system())
-                    )
+                        """).format(fspath(install), system()))
             else:
                 raise IndexError(version)
             mcr_root /= "v%d" % version
             log.info("Installed")
 
     # bin
     if (mcr_root / "bin" / MCR_ARCH).is_dir():
         env_prefix("PATH", mcr_root / "bin" / MCR_ARCH)
     else:
         log.warning("Cannot find MCR bin")
 
     # libs
-    env_var = {
-        "Linux": "LD_LIBRARY_PATH",
-        "Windows": "PATH",
-        "Darwin": "DYLD_LIBRARY_PATH",
-    }[system()]
+    env_var = {"Linux": "LD_LIBRARY_PATH", "Windows": "PATH",
+               "Darwin": "DYLD_LIBRARY_PATH"}[system()]
     if (mcr_root / "runtime" / MCR_ARCH).is_dir():
         env_prefix(env_var, mcr_root / "runtime" / MCR_ARCH)
     else:
         log.warning("Cannot find MCR libs")
 
     # python module
     pydist = mcr_root / "extern" / "engines" / "python" / "dist"
```

### Comparing `miutil-0.9.0/miutil/mlab/beautify.py` & `miutil-0.9.1/miutil/mlab/beautify.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from argopt import argopt
 from tqdm.contrib import tmap
 
 from ..web import get_file
 from . import get_engine, lru_cache
 
 log = logging.getLogger(__name__)
-MBEAUTIFIER_REV = "1a57849e44662f56271dc0eefa746855698a719a"
+MBEAUTIFIER_REV = "6005eeb8b17be8a40be32cea73005cf0d36de4e9"
 
 
 @lru_cache()
 @wraps(get_engine)
 def ensure_mbeautifier(*args, **kwargs):
     eng = get_engine(*args, **kwargs)
     fn = get_file(
@@ -48,9 +48,9 @@
         log.debug("file:%s", fn)
         try:
             formatter(fn, fn, nargout=0)
         except Exception as exc:
             log.error("file:%s:\n%s", fn, exc)
 
 
-if __name__ == "__main__":  # pragma: no cover
+if __name__ == "__main__": # pragma: no cover
     main()
```

### Comparing `miutil-0.9.0/miutil/plot.py` & `miutil-0.9.1/miutil/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import cm
 
 from .imio import imread
 
-show = plt.show  # convenience: for use after `imscroll`
+show = plt.show    # convenience: for use after `imscroll`
 
 
 def apply_cmap(**kwargs):
     """Apply different cmaps to inputs an average the results.
 
     Args:
       **kwargs: map named cmap to ndarray
@@ -66,26 +66,21 @@
             if titles is None:
                 titles = keys
         ndim = vol[0].ndim + 1
         if ndim == 3:
             vol = [vol]
         elif ndim not in [4, 5]:
             raise IndexError(
-                dedent(
-                    """\
+                dedent("""\
                 Expected vol.ndim in
                     3: single volume
                     4: multiple volumes
                     5: multiple RGB volumes
                 but got {}
-                """.format(
-                        ndim
-                    )
-                )
-            )
+                """.format(ndim)))
 
         view = view.lower()
         if view in ["c", "coronal", "y"]:
             vol = [i.transpose(1, 0, 2) for i in vol]
         elif view in ["s", "saggital", "x"]:
             vol = [i.transpose(2, 0, 1) for i in vol]
 
@@ -108,15 +103,15 @@
         self._annotes = []
         # event callbacks
         self.key = {i: False for i in self._SUPPORTED_KEYS}
         self.fig.canvas.mpl_connect("scroll_event", self._scroll)
         self.fig.canvas.mpl_connect("key_press_event", self._on_key)
         self.fig.canvas.mpl_connect("key_release_event", self._off_key)
         self.fig.canvas.mpl_connect("button_press_event", self._on_click)
-        imscroll._instances.append(self)  # prevents gc
+        imscroll._instances.append(self) # prevents gc
 
     @classmethod
     def clear(cls, self):
         cls._instances.clear()
 
     def _on_key(self, event):
         key = {"ctrl": "control"}.get(event.key, event.key)
@@ -158,21 +153,17 @@
         if arr.ndim == 3:
             z = [
                 ndi.map_coordinates(
                     arr,
                     np.vstack((x, y, np.ones_like(x) * i)),
                     order=self.order,
                     mode="nearest",
-                )
-                for i in range(event.inaxes.images[0].get_array().shape[-1])
-            ]
+                ) for i in range(event.inaxes.images[0].get_array().shape[-1])]
         else:
-            z = ndi.map_coordinates(
-                arr, np.vstack((x, y)), order=self.order, mode="nearest"
-            )
+            z = ndi.map_coordinates(arr, np.vstack((x, y)), order=self.order, mode="nearest")
         self.picked = []
         self.key["control"] = False
 
         self._annotes.append(event.inaxes.plot([x0, x1], [y0, y1], "r-")[0])
         plt.figure()
         if arr.ndim == 3:
             for channel, colour in zip(z, "rgbcmyk"):
```

### Comparing `miutil-0.9.0/miutil/web.py` & `miutil-0.9.1/miutil/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from os import W_OK, access, path, remove
 from shutil import copyfileobj
 
 try:
     from urllib.request import urlopen
-except ImportError:  # py27
+except ImportError: # py27
     from urllib import urlopen
 try:
     from urllib.parse import urlparse
-except ImportError:  # py27
+except ImportError: # py27
     from urlparse import urlparse
 
 import requests
 from tqdm.auto import tqdm
 
 from .fdio import Path, create_dir, fspath
 
@@ -50,20 +50,20 @@
     fpath = path.join(cache_dir, fname)
 
     if not path.exists(fpath):
         log.debug("Downloading %s from %s" % (fpath, origin))
         try:
             d = requests.get(origin, stream=True)
             with tqdm(
-                total=float(d.headers.get("Content-length") or 0),
-                desc=fname,
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1024,
-                leave=False,
+                    total=float(d.headers.get("Content-length") or 0),
+                    desc=fname,
+                    unit="B",
+                    unit_scale=True,
+                    unit_divisor=1024,
+                    leave=False,
             ) as fprog:
                 with open(fpath, "wb") as fo:
                     for chunk in d.iter_content(chunk_size=chunk_size):
                         fo.write(chunk)
                         fprog.update(len(chunk))
                 fprog.total = fprog.n
                 fprog.refresh()
```

### Comparing `miutil-0.9.0/miutil.egg-info/PKG-INFO` & `miutil-0.9.1/miutil.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,17 @@
 Metadata-Version: 2.1
 Name: miutil
-Version: 0.9.0
+Version: 0.9.1
 Summary: Medical imaging utilities for the AMYPAD and NiftyPET projects
 Home-page: https://github.com/AMYPAD/miutil
 Maintainer: Casper da Costa-Luis
 Maintainer-email: casper.dcl@physics.org
 License: Apache-2.0
 Project-URL: Changelog, https://github.com/AMYPAD/miutil/releases
 Project-URL: Documentation, https://github.com/AMYPAD/miutil/#miutil
-Description: miutil
-        ======
-        
-        Medical imaging utilities.
-        
-        |Version| |Py-Versions| |Conda| |Tests| |Coverage| |DOI| |LICENCE|
-        
-        Basic functionality needed for `AMYPAD <https://github.com/AMYPAD/AMYPAD>`_
-        and `NiftyPET <https://github.com/NiftyPET/NiftyPET>`_.
-        
-        
-        Install
-        -------
-        
-        Intended for inclusion in requirements for other packages.
-        The package name is ``miutil``. Extra install options include:
-        
-        - cuda
-        
-          - provides `miutil.cuinfo <https://github.com/AMYPAD/miutil/blob/master/miutil/cuinfo.py>`_
-        
-        - mbeautify
-        
-          - provides `miutil.mlab.beautify <https://github.com/AMYPAD/miutil/blob/master/miutil/mlab/beautify.py>`_
-        
-        - nii
-        
-          - provides `miutil.imio.nii <https://github.com/AMYPAD/miutil/blob/master/miutil/imio/nii.py>`_
-        
-        - plot
-        
-          - provides `miutil.plot <https://github.com/AMYPAD/miutil/blob/master/miutil/plot.py>`_
-        
-            - includes a useful 3D multi-volume ``imscroll`` function which depends only on ``matplotlib``
-        
-        - web
-        
-          - provides `miutil.web <https://github.com/AMYPAD/miutil/blob/master/miutil/web.py>`_
-        
-        
-        To install extras and their dependencies,
-        use the package name ``miutil[option1,option2]``.
-        
-        
-        .. |Tests| image:: https://img.shields.io/github/workflow/status/AMYPAD/miutil/Test?logo=GitHub
-           :target: https://github.com/AMYPAD/miutil/actions
-        .. |Coverage| image:: https://codecov.io/gh/AMYPAD/miutil/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/AMYPAD/miutil
-        .. |Version| image:: https://img.shields.io/pypi/v/miutil.svg?logo=python&logoColor=white
-           :target: https://github.com/AMYPAD/miutil/releases
-        .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/miutil.svg?logo=python&logoColor=white
-           :target: https://pypi.org/project/miutil
-        .. |Conda| image:: https://img.shields.io/conda/v/conda-forge/miutil.svg?label=conda&logo=conda-forge
-           :target: https://anaconda.org/conda-forge/miutil
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4281542.svg
-           :target: https://doi.org/10.5281/zenodo.4281542
-        .. |LICENCE| image:: https://img.shields.io/pypi/l/miutil.svg
-           :target: https://raw.githubusercontent.com/AMYPAD/miutil/master/LICENCE.md
-        
 Keywords: fMRI,PET,SPECT,EEG,MEG
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Education
@@ -98,7 +39,69 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: nii
 Provides-Extra: plot
 Provides-Extra: cuda
 Provides-Extra: web
 Provides-Extra: mbeautify
+License-File: LICENCE.md
+
+miutil
+======
+
+Medical imaging utilities.
+
+|Version| |Py-Versions| |Conda| |Tests| |Coverage| |DOI| |LICENCE|
+
+Basic functionality needed for `AMYPAD <https://github.com/AMYPAD/AMYPAD>`_
+and `NiftyPET <https://github.com/NiftyPET/NiftyPET>`_.
+
+
+Install
+-------
+
+Intended for inclusion in requirements for other packages.
+The package name is ``miutil``. Extra install options include:
+
+- cuda
+
+  - provides `miutil.cuinfo <https://github.com/AMYPAD/miutil/blob/master/miutil/cuinfo.py>`_
+
+- mbeautify
+
+  - provides `miutil.mlab.beautify <https://github.com/AMYPAD/miutil/blob/master/miutil/mlab/beautify.py>`_
+
+- nii
+
+  - provides `miutil.imio.nii <https://github.com/AMYPAD/miutil/blob/master/miutil/imio/nii.py>`_
+
+- plot
+
+  - provides `miutil.plot <https://github.com/AMYPAD/miutil/blob/master/miutil/plot.py>`_
+
+    - includes a useful 3D multi-volume ``imscroll`` function which depends only on ``matplotlib``
+
+- web
+
+  - provides `miutil.web <https://github.com/AMYPAD/miutil/blob/master/miutil/web.py>`_
+
+
+To install extras and their dependencies,
+use the package name ``miutil[option1,option2]``.
+
+
+.. |Tests| image:: https://img.shields.io/github/workflow/status/AMYPAD/miutil/Test?logo=GitHub
+   :target: https://github.com/AMYPAD/miutil/actions
+.. |Coverage| image:: https://codecov.io/gh/AMYPAD/miutil/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/AMYPAD/miutil
+.. |Version| image:: https://img.shields.io/pypi/v/miutil.svg?logo=python&logoColor=white
+   :target: https://github.com/AMYPAD/miutil/releases
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/miutil.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/miutil
+.. |Conda| image:: https://img.shields.io/conda/v/conda-forge/miutil.svg?label=conda&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/miutil
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4281542.svg
+   :target: https://doi.org/10.5281/zenodo.4281542
+.. |LICENCE| image:: https://img.shields.io/pypi/l/miutil.svg
+   :target: https://raw.githubusercontent.com/AMYPAD/miutil/master/LICENCE.md
+
+
```

### Comparing `miutil-0.9.0/miutil.egg-info/SOURCES.txt` & `miutil-0.9.1/miutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/setup.cfg` & `miutil-0.9.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 [options.extras_require]
 dev = 
 	pre-commit
 	pytest
 	pytest-cov
 	pytest-timeout
 	pytest-xdist
-	codecov
 nii = nibabel; numpy
 plot = matplotlib; numpy; scipy
 cuda = argopt; pynvml
 web = requests
 mbeautify = argopt; tqdm>=4.42.0; %(web)s
 
 [options.entry_points]
@@ -70,20 +69,32 @@
 [options.packages.find]
 exclude = tests
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
-max_line_length = 88
-extend-ignore = E203,P1
+max_line_length = 99
+extend-ignore = E228,E261,P1
 exclude = .git,__pycache__,build,dist,.eggs
 
+[yapf]
+spaces_before_comment = 15, 20
+arithmetic_precedence_indication = true
+allow_split_before_dict_value = false
+coalesce_brackets = True
+column_limit = 99
+each_dict_entry_on_separate_line = False
+space_between_ending_comma_and_closing_bracket = False
+split_before_named_assigns = False
+split_before_closing_bracket = False
+
 [isort]
 profile = black
+line_length = 99
 known_first_party = miutil,tests
 
 [tool:pytest]
 timeout = 15
 addopts = -v --tb=short -rxs -W=error --log-level=debug -n=auto --durations=0 --cov=miutil --cov-report=term-missing --cov-report=xml
 
 [egg_info]
```

### Comparing `miutil-0.9.0/tests/test_cuinfo.py` & `miutil-0.9.1/tests/test_cuinfo.py`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/tests/test_fdio.py` & `miutil-0.9.1/tests/test_fdio.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,28 +21,19 @@
         fdio.create_dir(tmpdir)
         assert "cannot create" in caplog.text
 
     assert tmpdir.exists()
 
 
 def test_hasext():
-    for fname, ext in [
-        (".baz", ".baz"),
-        ("foo.bar", ".bar"),
-        ("foo.bar", "bar"),
-        ("foo.bar.baz", "bar.baz"),
-        ("foo/bar.baz", "baz"),
-        ("foo.bar.baz", "baz"),
-    ]:
+    for fname, ext in [(".baz", ".baz"), ("foo.bar", ".bar"), ("foo.bar", "bar"),
+                       ("foo.bar.baz", "bar.baz"), ("foo/bar.baz", "baz"), ("foo.bar.baz", "baz")]:
         assert fdio.hasext(fname, ext)
 
-    for fname, ext in [
-        ("foo.bar", "baz"),
-        ("foo", "foo"),
-    ]:
+    for fname, ext in [("foo.bar", "baz"), ("foo", "foo")]:
         assert not fdio.hasext(fname, ext)
 
 
 def test_tmpdir():
     with fdio.tmpdir() as tmpdir:
         assert path.exists(tmpdir)
         res = tmpdir
@@ -54,18 +45,15 @@
     tmpdir = tmp_path / "extractall"
     assert not tmpdir.exists()
     url = "https://github.com/AMYPAD/miutil/archive/v0.6.0.zip"
     with web.urlopen_cached(url, tmpdir) as fd:
         fdio.extractall(fd, tmpdir)
 
     assert (tmpdir / "miutil-0.6.0" / "README.rst").is_file()
-    assert (
-        "Medical imaging utilities."
-        in (tmpdir / "miutil-0.6.0" / "README.rst").read_text()
-    )
+    assert ("Medical imaging utilities." in (tmpdir / "miutil-0.6.0" / "README.rst").read_text())
 
 
 def test_nsort():
     fnames = ["foo1_bar_21.nii.gz", "foo1_bar_1.2.nii.gz", "foo1_bar_1.nii.gz"]
     assert fdio.nsort(fnames) == fnames[::-1]
     fnames = [i[9:] for i in fnames]
     assert fdio.nsort(fnames) == fnames[::-1]
```

### Comparing `miutil-0.9.0/tests/test_imio.py` & `miutil-0.9.1/tests/test_imio.py`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/tests/test_mlab.py` & `miutil-0.9.1/tests/test_mlab.py`

 * *Files identical despite different names*

### Comparing `miutil-0.9.0/tests/test_web.py` & `miutil-0.9.1/tests/test_web.py`

 * *Files identical despite different names*

