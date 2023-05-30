# Comparing `tmp/xopt-1.4.0.tar.gz` & `tmp/xopt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-p569cmsx/xopt-1.4.0.tar", last modified: Wed May  3 22:33:53 2023, max compression
+gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-9u62j70t/xopt-1.4.1.tar", last modified: Tue May 30 06:03:17 2023, max compression
```

## Comparing `xopt-1.4.0.tar` & `xopt-1.4.1.tar`

### file list

```diff
@@ -1,117 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 22:33:42.000000 xopt-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 22:33:42.000000 xopt-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-03 22:33:53.000000 xopt-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-03 22:33:42.000000 xopt-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 22:33:42.000000 xopt-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 22:33:53.000000 xopt-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 22:33:42.000000 xopt-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/tests/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_bayesian_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_bayesian_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_mobo.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_model_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_time_dependent_bo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_extremum_seeking.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_generator_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_rcds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_vocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_xopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-05-03 22:33:42.000000 xopt-1.4.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/bayesian_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/bayesian/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/prior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/trainable_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/transformed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/es/extremumseeking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/ga/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/cnsga.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/deap_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/deap_fitness_with_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/fitness_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/rcds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/rcds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/rcds/rcds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/scipy/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/mpi/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/resources/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/ackley_20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/modified_tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/sinusoid_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/sphere_20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/vocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 06:03:09.000000 xopt-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 06:03:09.000000 xopt-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-30 06:03:17.000000 xopt-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-30 06:03:09.000000 xopt-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 06:03:09.000000 xopt-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-30 06:03:17.000000 xopt-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-30 06:03:09.000000 xopt-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/tests/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_bax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_bayesian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_bayesian_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_mobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_model_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_time_dependent_bo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/bayesian/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/test_extremum_seeking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/test_generator_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/generators/test_rcds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/test_vocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-30 06:03:09.000000 xopt-1.4.1/tests/test_xopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-05-30 06:03:09.000000 xopt-1.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/bayesian/bax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/bax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/bax/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/bax/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/bax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/bayesian_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/bayesian/custom_botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/custom_botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/custom_botorch/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/custom_botorch/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/bayesian/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/prior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/trainable_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/transformed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/bayesian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/es/extremumseeking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/ga/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/ga/cnsga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/ga/deap_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/ga/deap_fitness_with_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/ga/fitness_with_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/rcds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/rcds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/rcds/rcds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/generators/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/generators/scipy/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/mpi/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt/resources/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/ackley_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/modified_tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/sinusoid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/sphere_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/test_functions/tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/resources/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-30 06:03:09.000000 xopt-1.4.1/xopt/vocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 06:03:17.000000 xopt-1.4.1/xopt.egg-info/top_level.txt
```

### Comparing `xopt-1.4.0/LICENSE` & `xopt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/PKG-INFO` & `xopt-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.4.0
+Version: 1.4.1
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.4.0/README.md` & `xopt-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/setup.py` & `xopt-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_bayesian_exploration.py` & `xopt-1.4.1/tests/generators/bayesian/test_bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_bayesian_generator.py` & `xopt-1.4.1/tests/generators/bayesian/test_bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_bayesian_options.py` & `xopt-1.4.1/tests/generators/bayesian/test_bayesian_options.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_custom_model.py` & `xopt-1.4.1/tests/generators/bayesian/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_expected_improvement.py` & `xopt-1.4.1/tests/generators/bayesian/test_expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_high_level.py` & `xopt-1.4.1/tests/generators/bayesian/test_high_level.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_mggpo.py` & `xopt-1.4.1/tests/generators/bayesian/test_mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_mobo.py` & `xopt-1.4.1/tests/generators/bayesian/test_mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_model_constructor.py` & `xopt-1.4.1/tests/generators/bayesian/test_model_constructor.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_multi_fidelity.py` & `xopt-1.4.1/tests/generators/bayesian/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_time_dependent_bo.py` & `xopt-1.4.1/tests/generators/bayesian/test_time_dependent_bo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_turbo.py` & `xopt-1.4.1/tests/generators/bayesian/test_turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_upper_confidence_bound.py` & `xopt-1.4.1/tests/generators/bayesian/test_upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/bayesian/test_utils.py` & `xopt-1.4.1/tests/generators/bayesian/test_utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/test_extremum_seeking.py` & `xopt-1.4.1/tests/generators/test_extremum_seeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/generators/test_rcds.py` & `xopt-1.4.1/tests/generators/test_rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/test_evaluator.py` & `xopt-1.4.1/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/test_io.py` & `xopt-1.4.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/test_pydantic.py` & `xopt-1.4.1/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/test_vocs.py` & `xopt-1.4.1/tests/test_vocs.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/tests/test_xopt.py` & `xopt-1.4.1/tests/test_xopt.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/versioneer.py` & `xopt-1.4.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/base.py` & `xopt-1.4.1/xopt/base.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/evaluator.py` & `xopt-1.4.1/xopt/evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generator.py` & `xopt-1.4.1/xopt/generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/__init__.py` & `xopt-1.4.1/xopt/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/__init__.py` & `xopt-1.4.1/xopt/generators/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/base_model.py` & `xopt-1.4.1/xopt/generators/bayesian/base_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/bayesian_exploration.py` & `xopt-1.4.1/xopt/generators/bayesian/bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/bayesian_generator.py` & `xopt-1.4.1/xopt/generators/bayesian/bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py` & `xopt-1.4.1/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/identity.py` & `xopt-1.4.1/xopt/generators/bayesian/custom_botorch/identity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py` & `xopt-1.4.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/proximal.py` & `xopt-1.4.1/xopt/generators/bayesian/custom_botorch/proximal.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/expected_improvement.py` & `xopt-1.4.1/xopt/generators/bayesian/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/mggpo.py` & `xopt-1.4.1/xopt/generators/bayesian/mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/mobo.py` & `xopt-1.4.1/xopt/generators/bayesian/mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/models/prior_mean.py` & `xopt-1.4.1/xopt/generators/bayesian/models/prior_mean.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/models/standard.py` & `xopt-1.4.1/xopt/generators/bayesian/models/standard.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/models/time_dependent.py` & `xopt-1.4.1/xopt/generators/bayesian/models/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/models/trainable_mean.py` & `xopt-1.4.1/xopt/generators/bayesian/models/trainable_mean.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/models/transformed_model.py` & `xopt-1.4.1/xopt/generators/bayesian/models/transformed_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/models/utils.py` & `xopt-1.4.1/xopt/generators/bayesian/models/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/multi_fidelity.py` & `xopt-1.4.1/xopt/generators/bayesian/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/objectives.py` & `xopt-1.4.1/xopt/generators/bayesian/objectives.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/options.py` & `xopt-1.4.1/xopt/generators/bayesian/options.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/time_dependent.py` & `xopt-1.4.1/xopt/generators/bayesian/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/turbo.py` & `xopt-1.4.1/xopt/generators/bayesian/turbo.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 
     # get bounds width
     bound_widths = bounds[1] - bounds[0]
 
     # get location of best point so far
     variable_data = vocs.variable_data(data, "")
     objective_data = vocs.objective_data(data, "")
+    dim = vocs.n_variables
 
     # note that the trust region will be around the minimum point since Xopt
     # assumes minimization
     best_idx = objective_data.idxmin()
     best_x = torch.tensor(
         variable_data.loc[best_idx][vocs.variable_names].to_numpy(), **tkwargs
     )
 
     # Scale the TR to be proportional to the lengthscales of the objective model
     x_center = best_x.clone()
     lengthscales = model.models[0].covar_module.base_kernel.lengthscale.detach()
 
     # calculate the ratios of lengthscales for each axis
-    weights = lengthscales / torch.prod(lengthscales.pow(1.0 / len(lengthscales)))
+    weights = lengthscales / torch.prod(lengthscales)**(1/dim)
 
     # calculate the tr bounding box
     tr_lb = torch.clamp(
         x_center - weights * turbo_state.length * bound_widths / 2.0, *bounds
     )
     tr_ub = torch.clamp(
         x_center + weights * turbo_state.length * bound_widths / 2.0, *bounds
```

### Comparing `xopt-1.4.0/xopt/generators/bayesian/upper_confidence_bound.py` & `xopt-1.4.1/xopt/generators/bayesian/upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/bayesian/utils.py` & `xopt-1.4.1/xopt/generators/bayesian/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/es/extremumseeking.py` & `xopt-1.4.1/xopt/generators/es/extremumseeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/ga/cnsga.py` & `xopt-1.4.1/xopt/generators/ga/cnsga.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/ga/deap_creator.py` & `xopt-1.4.1/xopt/generators/ga/deap_creator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/ga/deap_fitness_with_constraints.py` & `xopt-1.4.1/xopt/generators/ga/deap_fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/ga/fitness_with_constraints.py` & `xopt-1.4.1/xopt/generators/ga/fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/random.py` & `xopt-1.4.1/xopt/generators/random.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/rcds/rcds.py` & `xopt-1.4.1/xopt/generators/rcds/rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/generators/scipy/neldermead.py` & `xopt-1.4.1/xopt/generators/scipy/neldermead.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/log.py` & `xopt-1.4.1/xopt/log.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/mpi/run.py` & `xopt-1.4.1/xopt/mpi/run.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/pydantic.py` & `xopt-1.4.1/xopt/pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/resources/test_functions/modified_tnk.py` & `xopt-1.4.1/xopt/resources/test_functions/modified_tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/resources/test_functions/rosenbrock.py` & `xopt-1.4.1/xopt/resources/test_functions/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/resources/test_functions/tnk.py` & `xopt-1.4.1/xopt/resources/test_functions/tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/resources/testing.py` & `xopt-1.4.1/xopt/resources/testing.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/utils.py` & `xopt-1.4.1/xopt/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt/vocs.py` & `xopt-1.4.1/xopt/vocs.py`

 * *Files identical despite different names*

### Comparing `xopt-1.4.0/xopt.egg-info/PKG-INFO` & `xopt-1.4.1/xopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.4.0
+Version: 1.4.1
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.4.0/xopt.egg-info/SOURCES.txt` & `xopt-1.4.1/xopt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 tests/test_xopt.py
 tests/generators/__init__.py
 tests/generators/test_extremum_seeking.py
 tests/generators/test_generator_options.py
 tests/generators/test_random.py
 tests/generators/test_rcds.py
 tests/generators/bayesian/__init__.py
+tests/generators/bayesian/test_bax.py
 tests/generators/bayesian/test_bayesian_exploration.py
 tests/generators/bayesian/test_bayesian_generator.py
 tests/generators/bayesian/test_bayesian_options.py
 tests/generators/bayesian/test_custom_model.py
 tests/generators/bayesian/test_expected_improvement.py
 tests/generators/bayesian/test_high_level.py
 tests/generators/bayesian/test_mggpo.py
@@ -47,26 +48,30 @@
 xopt.egg-info/dependency_links.txt
 xopt.egg-info/requires.txt
 xopt.egg-info/top_level.txt
 xopt/generators/__init__.py
 xopt/generators/random.py
 xopt/generators/bayesian/__init__.py
 xopt/generators/bayesian/base_model.py
+xopt/generators/bayesian/bax_generator.py
 xopt/generators/bayesian/bayesian_exploration.py
 xopt/generators/bayesian/bayesian_generator.py
 xopt/generators/bayesian/expected_improvement.py
 xopt/generators/bayesian/mggpo.py
 xopt/generators/bayesian/mobo.py
 xopt/generators/bayesian/multi_fidelity.py
 xopt/generators/bayesian/objectives.py
 xopt/generators/bayesian/options.py
 xopt/generators/bayesian/time_dependent.py
 xopt/generators/bayesian/turbo.py
 xopt/generators/bayesian/upper_confidence_bound.py
 xopt/generators/bayesian/utils.py
+xopt/generators/bayesian/bax/__init__.py
+xopt/generators/bayesian/bax/acquisition.py
+xopt/generators/bayesian/bax/algorithms.py
 xopt/generators/bayesian/custom_botorch/__init__.py
 xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
 xopt/generators/bayesian/custom_botorch/identity.py
 xopt/generators/bayesian/custom_botorch/multi_fidelity.py
 xopt/generators/bayesian/custom_botorch/proximal.py
 xopt/generators/bayesian/models/__init__.py
 xopt/generators/bayesian/models/prior_mean.py
```

