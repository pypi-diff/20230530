# Comparing `tmp/brainweb-dl-0.0.0.tar.gz` & `tmp/brainweb-dl-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainweb-dl-0.0.0.tar", last modified: Mon May 29 12:53:03 2023, max compression
+gzip compressed data, was "brainweb-dl-0.0.1.tar", last modified: Tue May 30 08:15:16 2023, max compression
```

## Comparing `brainweb-dl-0.0.0.tar` & `brainweb-dl-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:53:03.546316 brainweb-dl-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/src/brainweb_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/src/brainweb_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/src/brainweb_dl/_brainweb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/src/brainweb_dl/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/src/brainweb_dl/data/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/src/brainweb_dl/data/brainweb1_tissues.csv
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/src/brainweb_dl/data/brainweb20_tissues.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-29 12:52:39.000000 brainweb-dl-0.0.0/src/brainweb_dl/mri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:53:03.542316 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-29 12:53:03.000000 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 12:53:03.000000 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:53:03.000000 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 12:53:03.000000 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-29 12:53:03.000000 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 12:53:03.000000 brainweb-dl-0.0.0/src/brainweb_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.902856 brainweb-dl-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.898856 brainweb-dl-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.898856 brainweb-dl-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-30 08:15:16.902856 brainweb-dl-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:15:16.902856 brainweb-dl-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.898856 brainweb-dl-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.902856 brainweb-dl-0.0.1/src/brainweb_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/src/brainweb_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/src/brainweb_dl/_brainweb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/src/brainweb_dl/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.902856 brainweb-dl-0.0.1/src/brainweb_dl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/src/brainweb_dl/data/brainweb1_tissues.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/src/brainweb_dl/data/brainweb20_tissues.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-30 08:14:55.000000 brainweb-dl-0.0.1/src/brainweb_dl/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:15:16.902856 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 08:15:16.000000 brainweb-dl-0.0.1/src/brainweb_dl.egg-info/top_level.txt
```

### Comparing `brainweb-dl-0.0.0/.github/workflows/master-cd.yml` & `brainweb-dl-0.0.1/.github/workflows/master-cd.yml`

 * *Files 22% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 permissions:
   id-token: write
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to TestPyPI
     runs-on: ubuntu-latest
+    environment: test-pypi
     steps:
     - name: Checkout
       uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python 3.10
       uses: actions/setup-python@v4
       with:
         python-version: "3.10"
 
     - name: Install pypa/build
       run: |
-        python -m pip install build twine
+        python -m pip install build
         python -m pip install .
 
     - name: Build a binary wheel and a source tarball
       run: |
         python -m build --sdist --wheel --outdir dist/ .
 
-    - name: Check Dist
-      run: |
-        python -m twine check dist/*
-    - name: Upload to Test PyPI
-      run: |
-        python -m twine upload -r testpypi -u __token__ -p ${{ secrets.TEST_PYPI_API }} dist/*
+    - name: Publish distribution 📦 to  Test PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
+      with:
+        repository-url: https://test.pypi.org/legacy/
```

### Comparing `brainweb-dl-0.0.0/.github/workflows/tags-release.yml` & `brainweb-dl-0.0.1/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.0/LICENSE` & `brainweb-dl-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.0/PKG-INFO` & `brainweb-dl-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainweb-dl
-Version: 0.0.0
+Version: 0.0.1
 Summary: Download BrainWeb MRI data
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 
 Welcome to Brainweb-DL, a powerful Python toolkit for downloading and converting the Brainweb dataset. 
 
 <p align="center">
 <img src=https://img.shields.io/github/license/paquiteau/brainweb-dl a=https://github.com/paquiteau/brainweb-dl/blob/main/LICENSE>
 <img src=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge a=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl>
 <img src=https://img.shields.io/badge/style-black-black a=https://github.com/psf/black>
-
+<img src=https://img.shields.io/pypi/v/brainweb-dl a=https://pypi.org/project/brainweb-dl/>
 </p>
 
 ## Features
 
 - **Effortless Dataset Management:** Automatically download, cache, and format the Brainweb dataset with ease. Convert it to the convenient nifti format or numpy array hassle-free.
 
 - **Multiple Image Generation:** Generate high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset. Perfect for testing purposes, although keep in mind that the values provided are approximate.
```

### Comparing `brainweb-dl-0.0.0/README.md` & `brainweb-dl-0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Welcome to Brainweb-DL, a powerful Python toolkit for downloading and converting the Brainweb dataset. 
 
 <p align="center">
 <img src=https://img.shields.io/github/license/paquiteau/brainweb-dl a=https://github.com/paquiteau/brainweb-dl/blob/main/LICENSE>
 <img src=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge a=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl>
 <img src=https://img.shields.io/badge/style-black-black a=https://github.com/psf/black>
-
+<img src=https://img.shields.io/pypi/v/brainweb-dl a=https://pypi.org/project/brainweb-dl/>
 </p>
 
 ## Features
 
 - **Effortless Dataset Management:** Automatically download, cache, and format the Brainweb dataset with ease. Convert it to the convenient nifti format or numpy array hassle-free.
 
 - **Multiple Image Generation:** Generate high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset. Perfect for testing purposes, although keep in mind that the values provided are approximate.
```

### Comparing `brainweb-dl-0.0.0/pyproject.toml` & `brainweb-dl-0.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -64,29 +64,39 @@
 "Bug Reports" = "https://github.com/paquiteau/brainweb-dl/issues"
 "Source" = "https://github.com/paquiteau/brainweb-dl"
 
 [project.scripts]  # Optional
 # "my-script = my_package.some_module:main"
 brainweb-dl = "brainweb_dl.cli:main"
 
+[tool.setuptools.packages.find]
+where=["src"]
+
+
+[tool.setuptools_scm]
+write_to = "src/brainweb_dl/_version.py"
+version_scheme = "python-simplified-semver"
+local_scheme="no-local-version"
+
+
 # Formatting using black.
 [tool.black]
 
 [tool.isort]
 profile="black"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = [
-    "--cov=simfmri",
+    "--cov=brainweb_dl",
     "--cov-report=term-missing",
     "--cov-report=xml"
 ]
 
-
+# linting using ruff.
 [tool.ruff]
 src = ["src", "tests"]
 select = ["E", "F", "B", "Q", "D", "UP", "ANN"]
 
 ignore = [
     "ANN101", # missing type annotation for self
     "ANN102", # missing type annotation for cls in classmethod.
```

### Comparing `brainweb-dl-0.0.0/src/brainweb_dl/_brainweb.py` & `brainweb-dl-0.0.1/src/brainweb_dl/_brainweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,19 @@
     brainweb_dir = get_brainweb_dir(brainweb_dir)
     path = brainweb_dir / f"brainweb_s{s:02d}_{segmentation}.{extension}"
     if path.exists() and not force:
         return path
 
     if segmentation == "crisp":
         download_command = f"subject{s:02d}_{segmentation}"
-        _request_get_brainweb(download_command, path, shape=BIG_RES, dtype=np.uint16)
+        data = _request_get_brainweb(
+            download_command, path, shape=BIG_RES, dtype=np.uint16, obj_mode=True
+        )
+        data = data >> 4
+        data = data.astype(np.uint8)
     elif segmentation == "fuzzy":
         # Download all the fuzzy segmentation and create a 4D volume.
         path = Path(brainweb_dir) / f"brainweb_s{s:02d}_fuzzy.{extension}"
         # The case of fuzzy segmentation is a bit special.
         # We download all the fuzzy segmentation and create a 4D volume.
         # The 4th dimension is the segmentation type.
         if path.exists() and not force:
@@ -177,19 +181,17 @@
                 obj_mode=True,
             )
 
         Parallel(n_jobs=-1, backend="threading")(
             delayed(_download_fuzzy)(i, tissue["ID"], data)
             for i, tissue in enumerate(tissue_map)
         )
-        return save_array(data, path)
-
     else:
         raise ValueError("segmentation must be 'crisp' or 'fuzzy'")
-    return path
+    return save_array(data, path)
 
 
 def get_brainweb1(
     type: Literal["T1", "T2", "PD", "crisp", "fuzzy"] = "T2",
     res: int = 1,
     noise: int = 0,
     field_value: int = 0,
```

### Comparing `brainweb-dl-0.0.0/src/brainweb_dl/cli.py` & `brainweb-dl-0.0.1/src/brainweb_dl/cli.py`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.0/src/brainweb_dl/mri.py` & `brainweb-dl-0.0.1/src/brainweb_dl/mri.py`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.0/src/brainweb_dl.egg-info/PKG-INFO` & `brainweb-dl-0.0.1/src/brainweb_dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainweb-dl
-Version: 0.0.0
+Version: 0.0.1
 Summary: Download BrainWeb MRI data
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 
 Welcome to Brainweb-DL, a powerful Python toolkit for downloading and converting the Brainweb dataset. 
 
 <p align="center">
 <img src=https://img.shields.io/github/license/paquiteau/brainweb-dl a=https://github.com/paquiteau/brainweb-dl/blob/main/LICENSE>
 <img src=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge a=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl>
 <img src=https://img.shields.io/badge/style-black-black a=https://github.com/psf/black>
-
+<img src=https://img.shields.io/pypi/v/brainweb-dl a=https://pypi.org/project/brainweb-dl/>
 </p>
 
 ## Features
 
 - **Effortless Dataset Management:** Automatically download, cache, and format the Brainweb dataset with ease. Convert it to the convenient nifti format or numpy array hassle-free.
 
 - **Multiple Image Generation:** Generate high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset. Perfect for testing purposes, although keep in mind that the values provided are approximate.
```

### Comparing `brainweb-dl-0.0.0/src/brainweb_dl.egg-info/SOURCES.txt` & `brainweb-dl-0.0.1/src/brainweb_dl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/master-cd.yml
 .github/workflows/tags-release.yml
 src/brainweb_dl/__init__.py
 src/brainweb_dl/_brainweb.py
+src/brainweb_dl/_version.py
 src/brainweb_dl/cli.py
 src/brainweb_dl/mri.py
 src/brainweb_dl.egg-info/PKG-INFO
 src/brainweb_dl.egg-info/SOURCES.txt
 src/brainweb_dl.egg-info/dependency_links.txt
 src/brainweb_dl.egg-info/entry_points.txt
 src/brainweb_dl.egg-info/requires.txt
```

