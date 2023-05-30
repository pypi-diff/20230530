# Comparing `tmp/lyscripts-0.6.7.tar.gz` & `tmp/lyscripts-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyscripts-0.6.7.tar", last modified: Tue May 23 10:12:21 2023, max compression
+gzip compressed data, was "lyscripts-0.6.8.tar", last modified: Tue May 30 08:43:50 2023, max compression
```

## Comparing `lyscripts-0.6.7.tar` & `lyscripts-0.6.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.927064 lyscripts-0.6.7/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.927064 lyscripts-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.927064 lyscripts-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-05-23 10:12:04.000000 lyscripts-0.6.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 10:12:04.000000 lyscripts-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-23 10:12:21.935064 lyscripts-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-23 10:12:04.000000 lyscripts-0.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-23 10:12:04.000000 lyscripts-0.6.7/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-05-23 10:12:04.000000 lyscripts-0.6.7/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/app/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/app/prevalence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/enhance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/join.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/lyproxify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/corner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/thermo_int.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/lyscripts/predict/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/prevalences.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/risks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/temp_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 10:12:04.000000 lyscripts-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:12:21.935064 lyscripts-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:12:04.000000 lyscripts-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/plot/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/sine.png
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/sine.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/sine_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/test_draw.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/plot/data/
--rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/data/beta_samples.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/plot_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/predict/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/predict/predict_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/predict/prevalences_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/run_doctests.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/test_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.431637 lyscripts-0.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-30 08:43:34.000000 lyscripts-0.6.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 08:43:34.000000 lyscripts-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 08:43:50.439637 lyscripts-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-30 08:43:34.000000 lyscripts-0.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-30 08:43:34.000000 lyscripts-0.6.8/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-05-30 08:43:34.000000 lyscripts-0.6.8/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/app/prevalence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/lyproxify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/lyscripts/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/corner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/thermo_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/lyscripts/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/prevalences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/risks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/temp_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 08:43:34.000000 lyscripts-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:43:50.439637 lyscripts-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:43:34.000000 lyscripts-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/plot/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/sine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/sine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/sine_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/test_draw.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/plot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/data/beta_samples.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/plot_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/predict/predict_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/predict/prevalences_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/run_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/test_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/utils_test.py
```

### Comparing `lyscripts-0.6.7/.chglog/CHANGELOG.tpl.md` & `lyscripts-0.6.8/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/.chglog/config.yml` & `lyscripts-0.6.8/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/.github/workflows/build.yml` & `lyscripts-0.6.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/.github/workflows/docs.yml` & `lyscripts-0.6.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/.github/workflows/tests.yml` & `lyscripts-0.6.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/.gitignore` & `lyscripts-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/.pre-commit-config.yaml` & `lyscripts-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/CHANGELOG.md` & `lyscripts-0.6.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+<a name="0.6.8"></a>
+## [0.6.8] - 2023-05-30
+
+### Bug Fixes
+- flattening error in `lyproxify`
+- more robust lyproxify working again
+
+### Documentation
+- add detail to docstring of `lyproxify` func
+
+### Features
+- add func to generate md docs from column map
+- add two new dict modifying functions
+
+
 <a name="0.6.7"></a>
 ## [0.6.7] - 2023-05-23
 
 ### Bug Fixes
 - make flatten/unflatten funcs more consistent
 - add `max_depth` option for `flatten` function
 - bump isort version to avoid error
@@ -238,15 +253,16 @@
 - set up git-chglog for creating changelogs
 - add pre-commit hook to check commit msg
 
 
 <a name="0.5.3"></a>
 ## [0.5.3] - 2022-08-22
 
-[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.6.7...HEAD
+[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.6.8...HEAD
+[0.6.8]: https://github.com/rmnldwg/lyscripts/compare/0.6.7...0.6.8
 [0.6.7]: https://github.com/rmnldwg/lyscripts/compare/0.6.6...0.6.7
 [0.6.6]: https://github.com/rmnldwg/lyscripts/compare/0.6.5...0.6.6
 [0.6.5]: https://github.com/rmnldwg/lyscripts/compare/0.6.4...0.6.5
 [0.6.4]: https://github.com/rmnldwg/lyscripts/compare/0.6.3...0.6.4
 [0.6.3]: https://github.com/rmnldwg/lyscripts/compare/0.6.2...0.6.3
 [0.6.2]: https://github.com/rmnldwg/lyscripts/compare/0.6.1...0.6.2
 [0.6.1]: https://github.com/rmnldwg/lyscripts/compare/0.6.0...0.6.1
```

### Comparing `lyscripts-0.6.7/LICENSE` & `lyscripts-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/PKG-INFO` & `lyscripts-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.6.7
+Version: 0.6.8
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lyscripts-0.6.7/README.md` & `lyscripts-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/favicon.png` & `lyscripts-0.6.8/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/github-social-card.png` & `lyscripts-0.6.8/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/__init__.py` & `lyscripts-0.6.8/lyscripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/app/__init__.py` & `lyscripts-0.6.8/lyscripts/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/app/prevalence.py` & `lyscripts-0.6.8/lyscripts/app/prevalence.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/__init__.py` & `lyscripts-0.6.8/lyscripts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/__main__.py` & `lyscripts-0.6.8/lyscripts/data/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/clean.py` & `lyscripts-0.6.8/lyscripts/data/clean.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/enhance.py` & `lyscripts-0.6.8/lyscripts/data/enhance.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/generate.py` & `lyscripts-0.6.8/lyscripts/data/generate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/join.py` & `lyscripts-0.6.8/lyscripts/data/join.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/lyproxify.py` & `lyscripts-0.6.8/lyscripts/data/lyproxify.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """
-Consumes raw data and transforms it into a CSV of the format that
-LyProX can understand.
+Consumes raw data and transforms it into a CSV of the format that [LyProX] understands.
 
 To do so, it needs a dictionary that defines a mapping from raw columns to the LyProX
 style data format. See the documentation of the `transform_to_lyprox` function for
 more information.
+
+[LyProX]: https://lyprox.org
 """
 import argparse
 import importlib.util
 import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 import pandas as pd
 
 from lyscripts.data.utils import load_csv_table, save_table_to_csv
-from lyscripts.utils import raise_if_args_none, report, report_state
+from lyscripts.utils import (
+    delete_private_keys,
+    flatten,
+    raise_if_args_none,
+    report,
+    report_state,
+)
 
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 
 def _add_parser(
     subparsers: argparse._SubParsersAction,
     help_formatter,
@@ -94,77 +101,170 @@
             table.rename(
                 columns={f"Unnamed: {col}_level_{row}": f"{col}_lvl_{row}"},
                 inplace=True,
             )
     return table
 
 
+def get_instruction_depth(nested_column_map: Dict[Tuple, Dict[str, Any]]) -> int:
+    """
+    Get the depth at which the column mapping instructions are nested.
+
+    Instructions are a dictionary that contains either a 'func' or 'default' key.
+
+    Example:
+    >>> nested_column_map = {"patient": {"age": {"func": int}}}
+    >>> get_instruction_depth(nested_column_map)
+    2
+    >>> flat_column_map = flatten(nested_column_map, max_depth=2)
+    >>> get_instruction_depth(flat_column_map)
+    1
+    >>> nested_column_map = {"patient": {"__doc__": "some patient info", "age": 61}}
+    >>> get_instruction_depth(nested_column_map)
+    Traceback (most recent call last):
+        ...
+    ValueError: Leaf of column map must be a dictionary with 'func' or 'default' key.
+    """
+    for _, value in nested_column_map.items():
+        if isinstance(value, dict):
+            if "func" in value or "default" in value:
+                return 1
+
+            return 1 + get_instruction_depth(value)
+
+        raise ValueError(
+            "Leaf of column map must be a dictionary with 'func' or 'default' key."
+        )
+
+
+def generate_markdown_docs(
+    nested_column_map: Dict[Tuple, Dict[str, Any]],
+    depth: int = 0,
+) -> str:
+    """
+    Generate a markdown nested, ordered list as documentation for the column map.
+
+    A key in the doctionary is supposed to be documented, when its value is a dictionary
+    containing a `"__doc__"` key.
+
+    Example:
+    >>> nested_column_map = {
+    ...     "patient": {
+    ...         "__doc__": "some patient info",
+    ...         "age": {
+    ...             "__doc__": "age of the patient",
+    ...             "func": int,
+    ...             "columns": ["age"],
+    ...         },
+    ...     },
+    ... }
+    >>> generate_markdown_docs(nested_column_map)
+    '1. **`patient`**: some patient info\\n   1. **`age`**: age of the patient\\n'
+    """
+    md_docs = ""
+    i = 1
+    for key, value in nested_column_map.items():
+        if isinstance(value, dict):
+            if "__doc__" in value:
+                md_docs += f"{'   ' * depth}{i}. **`{key}`**: {value['__doc__']}\n"
+                i += 1
+
+            md_docs += generate_markdown_docs(value, depth + 1)
+
+    return md_docs
+
+
 @report_state(
     status_msg="Transform raw data to LyProX style table...",
     success_msg="Transformed raw data to LyProX style table.",
     stop_on_exc=True
 )
 @raise_if_args_none(
     message="Must provide raw data and mapping instruction module",
     level="warning",
 )
 def transform_to_lyprox(
     raw: pd.DataFrame,
     column_map: Dict[Tuple, Dict[str, Any]]
 ) -> pd.DataFrame:
     """
-    Transform any `raw` data frame into a table that can be uploaded directly to
-    [LyProX](https://lyprox.org). To do so, it uses instructions in the `colum_map`
-    dictionary, that needs to have a particular structure:
+    Transform `raw` data frame into table that can be uploaded directly to [LyProX].
+
+    To do so, it uses instructions in the `colum_map` dictionary, that needs to have
+    a particular structure:
 
     For each column in the final 'lyproxified' `pd.DataFrame`, one entry must exist in
     the `column_map` dctionary. E.g., for the column corresponding to a patient's age,
-    the dictionary should contain a key-value pari of this shape:
+    the dictionary should contain a key-value pair of this shape:
 
     ```python
     column_map = {
         ("patient", "#", "age"): {
             "func": compute_age_from_raw,
             "kwargs": {"randomize": False},
             "columns": ["birthday", "date of diagnosis"]
         },
     }
     ```
+
+    In this example, the function `compute_age_from_raw` is called with the values of
+    the columns `birthday` and `date of diagnosis` as positional arguments, and the
+    keyword argument `randomize` is set to `False`. The function then returns the
+    patient's age, which is subsequently stored in the column `("patient", "#", "age")`.
+
+    Note that the `column_map` dictionary must have either a `default` key or `func`
+    along with `columns` and `kwargs`, depending on the function definition. If the
+    function does not take any arguments, `columns` can be omitted. If it also does
+    not take any keyword arguments, `kwargs` can be omitted, too.
+
+    [LyProX]: https://lyprox.org
     """
+    column_map = delete_private_keys(column_map)
+
+    if (instruction_depth := get_instruction_depth(column_map)) > 1:
+        column_map = flatten(column_map, max_depth=instruction_depth)
+
     multi_idx = pd.MultiIndex.from_tuples(column_map.keys())
     processed = pd.DataFrame(columns=multi_idx)
 
     for multi_idx_col, instruction in column_map.items():
         if instruction != "":
             if "default" in instruction:
                 processed[multi_idx_col] = [instruction["default"]] * len(raw)
-            else:
+            elif "func" in instruction:
                 cols = instruction.get("columns", [])
                 kwargs = instruction.get("kwargs", {})
-                func = instruction.get("func", lambda x, *_a, **_kw: x)
+                func = instruction["func"]
 
                 try:
                     processed[multi_idx_col] = [
                         func(*vals, **kwargs) for vals in raw[cols].values
                     ]
                 except Exception as exc:
                     raise ParsingError(
                         f"Exception encountered while parsing column {multi_idx_col}"
                     ) from exc
+            else:
+                raise ParsingError(
+                    f"Column {multi_idx_col} has neither a `default` value nor `func` "
+                    "describing how to fill this column."
+                )
     return processed
 
 
 @report_state(
     status_msg="Transform absolute side reporting to tumor-relative...",
     success_msg="Transformed absolute side reporting to tumor-relative.",
     stop_on_exc=True,
 )
 @raise_if_args_none(message="Missing data table", level="warning")
 def leftright_to_ipsicontra(data: pd.DataFrame):
     """
+    Change absolute side reporting to tumor-relative.
+
     Transform reporting of LNL involvement by absolute side (right & left) to a
     reporting relative to the tumor (ipsi- & contralateral). The table `data` should
     already be in the format LyProX requires, except for the side-reporting of LNL
     involvement.
     """
     len_before = len(data)
     left_data = data.loc[
@@ -266,20 +366,20 @@
 
     with report.status("Import mapping instructions..."):
         spec = importlib.util.spec_from_file_location("map_module", args.mapping)
         mapping = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(mapping)
         report.success(f"Imported mapping instructions from {args.mapping}")
 
-    reduced = exclude_patients(trimmed, mapping.exclude)
+    reduced = exclude_patients(trimmed, mapping.EXCLUDE)
 
     if args.add_index:
         with report.status("Add index column to data..."):
             reduced.insert(0, ("patient", "#", "id"), list(range(len(reduced))))
             report.success("Added index column to data.")
 
-    processed = transform_to_lyprox(reduced, mapping.column_map)
+    processed = transform_to_lyprox(reduced, mapping.COLUMN_MAP)
 
     if ("tumor", "1", "side") in processed.columns:
         processed = leftright_to_ipsicontra(processed)
 
     save_table_to_csv(args.output, processed)
```

### Comparing `lyscripts-0.6.7/lyscripts/data/split.py` & `lyscripts-0.6.8/lyscripts/data/split.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/data/utils.py` & `lyscripts-0.6.8/lyscripts/data/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/evaluate.py` & `lyscripts-0.6.8/lyscripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/plot/__init__.py` & `lyscripts-0.6.8/lyscripts/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/plot/__main__.py` & `lyscripts-0.6.8/lyscripts/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/plot/corner.py` & `lyscripts-0.6.8/lyscripts/plot/corner.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/plot/histograms.py` & `lyscripts-0.6.8/lyscripts/plot/histograms.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/plot/thermo_int.py` & `lyscripts-0.6.8/lyscripts/plot/thermo_int.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/plot/utils.py` & `lyscripts-0.6.8/lyscripts/plot/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/predict/__init__.py` & `lyscripts-0.6.8/lyscripts/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/predict/__main__.py` & `lyscripts-0.6.8/lyscripts/predict/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/predict/prevalences.py` & `lyscripts-0.6.8/lyscripts/predict/prevalences.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/predict/risks.py` & `lyscripts-0.6.8/lyscripts/predict/risks.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/predict/utils.py` & `lyscripts-0.6.8/lyscripts/predict/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/sample.py` & `lyscripts-0.6.8/lyscripts/sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/temp_schedule.py` & `lyscripts-0.6.8/lyscripts/temp_schedule.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/lyscripts/utils.py` & `lyscripts-0.6.8/lyscripts/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,14 +450,58 @@
         return [lnl.name for lnl in model.ipsi.lnls]
     if isinstance(model, lymph.MidlineBilateral):
         return [lnl.name for lnl in model.ext.ipsi.lnls]
 
     raise TypeError(f"Model cannot be of type {type(model)}")
 
 
+def get_dict_depth(nested: dict) -> int:
+    """
+    Get the depth of a nested dictionary.
+
+    For example:
+    >>> get_dict_depth({"a": {"b": 1}})
+    2
+    >>> varying_depth = {"a": {"b": 1}, "c": {"d": {"e": 2}}}
+    >>> get_dict_depth(varying_depth)
+    3
+    """
+    if isinstance(nested, dict):
+        max_depth = None
+        for _, value in nested.items():
+            value_depth = get_dict_depth(value)
+            max_depth = max(max_depth or value_depth, value_depth)
+
+        return 1 + (max_depth or 0)
+
+    return 0
+
+
+def delete_private_keys(nested: dict) -> dict:
+    """
+    Delete private keys from a nested dictionary.
+
+    A 'private' key is a key whose name starts with an underscore. For example:
+    >>> delete_private_keys({"patient": {"__doc__": "some patient info", "age": 61}})
+    {'patient': {'age': 61}}
+    >>> delete_private_keys({"patient": {"age": 61}})
+    {'patient': {'age': 61}}
+    """
+    cleaned = {}
+
+    if isinstance(nested, dict):
+        for key, value in nested.items():
+            if not (isinstance(key, str) and key.startswith("_")):
+                cleaned[key] = delete_private_keys(value)
+    else:
+        cleaned = nested
+
+    return cleaned
+
+
 def flatten(
     nested: dict,
     prev_key: tuple = (),
     max_depth: Optional[int] = None,
 ) -> dict:
     """
     Flatten a `nested` dictionary by creating key tuples for each value at `max_depth`.
@@ -465,14 +509,16 @@
     For example:
     >>> nested = {"tumor": {"1": {"t_stage": 1, "size": 12.3}}}
     >>> flatten(nested)
     {('tumor', '1', 't_stage'): 1, ('tumor', '1', 'size'): 12.3}
     >>> mapping = {"patient": {"#": {"age": {"func": int, "columns": ["age"]}}}}
     >>> flatten(mapping, max_depth=3)
     {('patient', '#', 'age'): {'func': <class 'int'>, 'columns': ['age']}}
+
+    Note that flattening an already flat dictionary will yield some weird results.
     """
     result = {}
 
     for key, value in nested.items():
         is_dict = isinstance(value, dict)
         has_reached_max_depth = max_depth is not None and len(prev_key) >= max_depth - 1
```

### Comparing `lyscripts-0.6.7/lyscripts.egg-info/PKG-INFO` & `lyscripts-0.6.8/lyscripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.6.7
+Version: 0.6.8
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lyscripts-0.6.7/lyscripts.egg-info/SOURCES.txt` & `lyscripts-0.6.8/lyscripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/pyproject.toml` & `lyscripts-0.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/_sample.py` & `lyscripts-0.6.8/tests/_sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/plot/baseline/sine.png` & `lyscripts-0.6.8/tests/plot/baseline/sine.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/plot/baseline/sine.svg` & `lyscripts-0.6.8/tests/plot/baseline/sine.svg`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/plot/baseline/sine_svg.png` & `lyscripts-0.6.8/tests/plot/baseline/sine_svg.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/plot/baseline/test_draw.png` & `lyscripts-0.6.8/tests/plot/baseline/test_draw.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/plot/data/beta_samples.hdf5` & `lyscripts-0.6.8/tests/plot/data/beta_samples.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/plot/plot_utils_test.py` & `lyscripts-0.6.8/tests/plot/plot_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/predict/predict_utils_test.py` & `lyscripts-0.6.8/tests/predict/predict_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/predict/prevalences_test.py` & `lyscripts-0.6.8/tests/predict/prevalences_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/test_params.yaml` & `lyscripts-0.6.8/tests/test_params.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.7/tests/utils_test.py` & `lyscripts-0.6.8/tests/utils_test.py`

 * *Files identical despite different names*

