# Comparing `tmp/pymc-5.4.0.tar.gz` & `tmp/pymc-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.4.0.tar", last modified: Tue May 23 08:47:51 2023, max compression
+gzip compressed data, was "dist/pymc-5.4.1.tar", last modified: Tue May 30 09:46:27 2023, max compression
```

## Comparing `pymc-5.4.0.tar` & `pymc-5.4.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-23 08:47:43.000000 pymc-5.4.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-23 08:47:43.000000 pymc-5.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-23 08:47:43.000000 pymc-5.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-05-23 08:47:43.000000 pymc-5.4.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-05-23 08:47:43.000000 pymc-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 08:47:43.000000 pymc-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-23 08:47:51.000000 pymc-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-23 08:47:43.000000 pymc-5.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-23 08:47:43.000000 pymc-5.4.0/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   116464 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    42225 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    36499 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    90135 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 08:47:43.000000 pymc-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-23 08:47:43.000000 pymc-5.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-05-23 08:47:43.000000 pymc-5.4.0/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-05-23 08:47:43.000000 pymc-5.4.0/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 08:47:51.000000 pymc-5.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-05-23 08:47:43.000000 pymc-5.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-05-23 08:47:43.000000 pymc-5.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-30 09:46:19.000000 pymc-5.4.1/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-30 09:46:19.000000 pymc-5.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-30 09:46:19.000000 pymc-5.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-05-30 09:46:19.000000 pymc-5.4.1/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-05-30 09:46:19.000000 pymc-5.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 09:46:19.000000 pymc-5.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-30 09:46:27.000000 pymc-5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-30 09:46:19.000000 pymc-5.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-30 09:46:19.000000 pymc-5.4.1/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116464 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42225 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36499 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90135 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50490 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 09:46:19.000000 pymc-5.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 09:46:19.000000 pymc-5.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-05-30 09:46:19.000000 pymc-5.4.1/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-05-30 09:46:19.000000 pymc-5.4.1/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 09:46:27.000000 pymc-5.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-05-30 09:46:19.000000 pymc-5.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-05-30 09:46:19.000000 pymc-5.4.1/versioneer.py
```

### Comparing `pymc-5.4.0/ARCHITECTURE.md` & `pymc-5.4.1/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/CODE_OF_CONDUCT.md` & `pymc-5.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/CONTRIBUTING.md` & `pymc-5.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/GOVERNANCE.md` & `pymc-5.4.1/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/LICENSE` & `pymc-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/PKG-INFO` & `pymc-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.4.0
+Version: 5.4.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.4.0/README.rst` & `pymc-5.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/RELEASE-NOTES.md` & `pymc-5.4.1/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/__init__.py` & `pymc-5.4.1/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/backends/__init__.py` & `pymc-5.4.1/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/backends/arviz.py` & `pymc-5.4.1/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/backends/base.py` & `pymc-5.4.1/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/backends/mcbackend.py` & `pymc-5.4.1/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/backends/ndarray.py` & `pymc-5.4.1/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/backends/report.py` & `pymc-5.4.1/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/blocking.py` & `pymc-5.4.1/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/data.py` & `pymc-5.4.1/pymc/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from pytensor.tensor.random.basic import IntegersRV
 from pytensor.tensor.subtensor import AdvancedSubtensor
 from pytensor.tensor.type import TensorType
 from pytensor.tensor.var import TensorConstant, TensorVariable
 
 import pymc as pm
 
+from pymc.logprob.abstract import _get_measurable_outputs
 from pymc.pytensorf import convert_observed_data
 
 __all__ = [
     "get_data",
     "GeneratorAdapter",
     "Minibatch",
     "Data",
@@ -130,14 +131,19 @@
     # Work-around for https://github.com/pymc-devs/pytensor/issues/97
     def make_node(self, rng, *args, **kwargs):
         if rng is None:
             rng = pytensor.shared(np.random.default_rng())
         return super().make_node(rng, *args, **kwargs)
 
 
+@_get_measurable_outputs.register(MinibatchIndexRV)
+def minibatch_index_rv_measuarable_outputs(op, node):
+    return []
+
+
 minibatch_index = MinibatchIndexRV()
 
 
 def is_minibatch(v: TensorVariable) -> bool:
     return (
         isinstance(v.owner.op, AdvancedSubtensor)
         and isinstance(v.owner.inputs[1].owner.op, MinibatchIndexRV)
@@ -160,35 +166,36 @@
 
 def assert_all_scalars_equal(scalar, *scalars):
     if len(scalars) == 0:
         return scalar
     else:
         return Assert(
             "All variables shape[0] in Minibatch should be equal, check your Minibatch(data1, data2, ...) code"
-        )(scalar, pt.all([scalar == s for s in scalars]))
+        )(scalar, pt.all([pt.eq(scalar, s) for s in scalars]))
 
 
 def Minibatch(variable: TensorVariable, *variables: TensorVariable, batch_size: int):
-    """
-    Get random slices from variables from the leading dimension.
-
+    """Get random slices from variables from the leading dimension.
 
     Parameters
     ----------
     variable: TensorVariable
     variables: TensorVariable
     batch_size: int
 
     Examples
     --------
     >>> data1 = np.random.randn(100, 10)
     >>> data2 = np.random.randn(100, 20)
     >>> mdata1, mdata2 = Minibatch(data1, data2, batch_size=10)
     """
 
+    if not isinstance(batch_size, int):
+        raise TypeError("batch_size must be an integer")
+
     tensor, *tensors = tuple(map(pt.as_tensor, (variable, *variables)))
     upper = assert_all_scalars_equal(*[t.shape[0] for t in (tensor, *tensors)])
     slc = minibatch_index(0, upper, size=batch_size)
     for i, v in enumerate((tensor, *tensors)):
         if not valid_for_minibatch(v):
             raise ValueError(
                 f"{i}: {v} is not valid for Minibatch, only constants or constants.astype(dtype) are allowed"
```

### Comparing `pymc-5.4.0/pymc/distributions/__init__.py` & `pymc-5.4.1/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/bound.py` & `pymc-5.4.1/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/censored.py` & `pymc-5.4.1/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/continuous.py` & `pymc-5.4.1/pymc/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/discrete.py` & `pymc-5.4.1/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/dist_math.py` & `pymc-5.4.1/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/distribution.py` & `pymc-5.4.1/pymc/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/mixture.py` & `pymc-5.4.1/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/multivariate.py` & `pymc-5.4.1/pymc/distributions/multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/shape_utils.py` & `pymc-5.4.1/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/simulator.py` & `pymc-5.4.1/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/timeseries.py` & `pymc-5.4.1/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/transforms.py` & `pymc-5.4.1/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/distributions/truncated.py` & `pymc-5.4.1/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/exceptions.py` & `pymc-5.4.1/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/func_utils.py` & `pymc-5.4.1/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/gp/__init__.py` & `pymc-5.4.1/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/gp/cov.py` & `pymc-5.4.1/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/gp/gp.py` & `pymc-5.4.1/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/gp/hsgp_approx.py` & `pymc-5.4.1/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/gp/mean.py` & `pymc-5.4.1/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/gp/util.py` & `pymc-5.4.1/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/initial_point.py` & `pymc-5.4.1/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/__init__.py` & `pymc-5.4.1/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/abstract.py` & `pymc-5.4.1/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/basic.py` & `pymc-5.4.1/pymc/logprob/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,29 +40,35 @@
 from typing import Dict, List, Optional, Sequence, Union
 
 import numpy as np
 import pytensor
 import pytensor.tensor as pt
 
 from pytensor import config
-from pytensor.graph.basic import Variable, graph_inputs, io_toposort
+from pytensor.graph.basic import (
+    Constant,
+    Variable,
+    ancestors,
+    graph_inputs,
+    io_toposort,
+)
 from pytensor.graph.op import compute_test_value
 from pytensor.graph.rewriting.basic import GraphRewriter, NodeRewriter
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.var import TensorVariable
 from typing_extensions import TypeAlias
 
 from pymc.logprob.abstract import (
     _icdf_helper,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
     get_measurable_outputs,
 )
-from pymc.logprob.rewriting import construct_ir_fgraph
+from pymc.logprob.rewriting import cleanup_ir, construct_ir_fgraph
 from pymc.logprob.transforms import RVTransform, TransformValuesRewrite
 from pymc.logprob.utils import rvs_to_value_vars
 
 TensorLike: TypeAlias = Union[Variable, float, np.ndarray]
 
 
 def _warn_rvs_in_inferred_graph(graph: Sequence[TensorVariable]):
@@ -97,14 +103,15 @@
     value = pt.as_tensor_variable(value, dtype=rv.dtype)
     try:
         return _logprob_helper(rv, value, **kwargs)
     except NotImplementedError:
         fgraph, _, _ = construct_ir_fgraph({rv: value})
         [(ir_rv, ir_value)] = fgraph.preserve_rv_mappings.rv_values.items()
         expr = _logprob_helper(ir_rv, ir_value, **kwargs)
+        cleanup_ir([expr])
         if warn_missing_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
 def logcdf(
     rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
@@ -114,14 +121,15 @@
     try:
         return _logcdf_helper(rv, value, **kwargs)
     except NotImplementedError:
         # Try to rewrite rv
         fgraph, rv_values, _ = construct_ir_fgraph({rv: value})
         [ir_rv] = fgraph.outputs
         expr = _logcdf_helper(ir_rv, value, **kwargs)
+        cleanup_ir([expr])
         if warn_missing_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
 def icdf(
     rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
@@ -131,14 +139,15 @@
     try:
         return _icdf_helper(rv, value, **kwargs)
     except NotImplementedError:
         # Try to rewrite rv
         fgraph, rv_values, _ = construct_ir_fgraph({rv: value})
         [ir_rv] = fgraph.outputs
         expr = _icdf_helper(ir_rv, value, **kwargs)
+        cleanup_ir([expr])
         if warn_missing_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
 def factorized_joint_logprob(
     rv_values: Dict[TensorVariable, TensorVariable],
@@ -227,18 +236,24 @@
     # cumulatively maintains remappings for all the variables/nodes that needed
     # to be recreated after replacing `MeasurableVariable`s with their
     # value-variables.  Since these replacements work in topological order, all
     # the necessary value-variable replacements should be present for each
     # node.
     replacements = updated_rv_values.copy()
 
-    # To avoid cloning the value variables, we map them to themselves in the
-    # `replacements` `dict` (i.e. entries already existing in `replacements`
-    # aren't cloned)
-    replacements.update({v: v for v in rv_values.values()})
+    # To avoid cloning the value variables (or ancestors of value variables),
+    # we map them to themselves in the `replacements` `dict`
+    # (i.e. entries already existing in `replacements` aren't cloned)
+    replacements.update(
+        {
+            v: v
+            for v in ancestors(rv_values.values())
+            if (not isinstance(v, Constant) and v not in replacements)
+        }
+    )
 
     # Walk the graph from its inputs to its outputs and construct the
     # log-probability
     q = deque(fgraph.toposort())
 
     logprob_vars = {}
 
@@ -305,14 +320,16 @@
 
     missing_value_terms = set(original_values.values()) - set(logprob_vars.keys())
     if missing_value_terms:
         raise RuntimeError(
             f"The logprob terms of the following value variables could not be derived: {missing_value_terms}"
         )
 
+    cleanup_ir(logprob_vars.values())
+
     return logprob_vars
 
 
 def _check_no_rvs(logp_terms: Sequence[TensorVariable]):
     # Raise if there are unexpected RandomVariables in the logp graph
     # Only SimulatorRVs MinibatchIndexRVs are allowed
     from pymc.data import MinibatchIndexRV
```

### Comparing `pymc-5.4.0/pymc/logprob/binary.py` & `pymc-5.4.1/pymc/logprob/binary.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/censoring.py` & `pymc-5.4.1/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/checks.py` & `pymc-5.4.1/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/cumsum.py` & `pymc-5.4.1/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/mixture.py` & `pymc-5.4.1/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/rewriting.py` & `pymc-5.4.1/pymc/logprob/rewriting.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,28 +30,34 @@
 #   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
 
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Sequence, Tuple
 
 import pytensor.tensor as pt
 
 from pytensor.compile.mode import optdb
-from pytensor.graph.basic import Variable
+from pytensor.graph.basic import Constant, Variable, ancestors
 from pytensor.graph.features import Feature
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.rewriting.basic import GraphRewriter, node_rewriter
-from pytensor.graph.rewriting.db import EquilibriumDB, RewriteDatabaseQuery, SequenceDB
+from pytensor.graph.rewriting.db import (
+    EquilibriumDB,
+    LocalGroupDB,
+    RewriteDatabaseQuery,
+    SequenceDB,
+    TopoDB,
+)
 from pytensor.tensor.elemwise import DimShuffle, Elemwise
 from pytensor.tensor.extra_ops import BroadcastTo
 from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
-from pytensor.tensor.rewriting.basic import register_canonicalize, register_useless
+from pytensor.tensor.rewriting.basic import register_canonicalize
 from pytensor.tensor.rewriting.shape import ShapeFeature
 from pytensor.tensor.subtensor import (
     AdvancedIncSubtensor,
     AdvancedIncSubtensor1,
     AdvancedSubtensor,
     AdvancedSubtensor1,
     IncSubtensor,
@@ -187,17 +193,16 @@
     dd_val = dd_inp.owner.inputs[0]
 
     new_value_node = node.op.make_node(dd_val, *node.inputs[1:])
     new_node = dd_inp.owner.op.make_node(new_value_node.outputs[0])
     return new_node.outputs
 
 
-@register_useless
-@node_rewriter((DiracDelta,))
-def local_remove_DiracDelta(fgraph, node):
+@node_rewriter([DiracDelta])
+def remove_DiracDelta(fgraph, node):
     r"""Remove `DiracDelta`\s."""
     dd_val = node.inputs[0]
     return [dd_val]
 
 
 @node_rewriter(inc_subtensor_ops)
 def incsubtensor_rv_replace(fgraph, node):
@@ -266,14 +271,25 @@
 # (or eventually) the graph outputs.  Often this is done by lifting other `Op`s
 # "up" through the random/measurable variables and into their inputs.
 measurable_ir_rewrites_db.register("subtensor_lift", local_subtensor_rv_lift, "basic")
 measurable_ir_rewrites_db.register("incsubtensor_lift", incsubtensor_rv_replace, "basic")
 
 logprob_rewrites_db.register("post-canonicalize", optdb.query("+canonicalize"), "basic")
 
+# Rewrites that remove IR Ops
+cleanup_ir_rewrites_db = LocalGroupDB()
+cleanup_ir_rewrites_db.name = "cleanup_ir_rewrites_db"
+logprob_rewrites_db.register(
+    "cleanup_ir_rewrites",
+    TopoDB(cleanup_ir_rewrites_db, order="out_to_in", ignore_newtrees=True, failure_callback=None),
+    "cleanup",
+)
+
+cleanup_ir_rewrites_db.register("remove_DiracDelta", remove_DiracDelta, "cleanup")
+
 
 def construct_ir_fgraph(
     rv_values: Dict[Variable, Variable],
     ir_rewriter: Optional[GraphRewriter] = None,
 ) -> Tuple[FunctionGraph, Dict[Variable, Variable], Dict[Variable, Variable]]:
     r"""Construct a `FunctionGraph` in measurable IR form for the keys in `rv_values`.
 
@@ -312,16 +328,16 @@
     `FunctionGraph`.
     """
 
     # Since we're going to clone the entire graph, we need to keep a map from
     # the old nodes to the new ones; otherwise, we won't be able to use
     # `rv_values`.
     # We start the `dict` with mappings from the value variables to themselves,
-    # to prevent them from being cloned.
-    memo = {v: v for v in rv_values.values()}
+    # to prevent them from being cloned. This also includes ancestors
+    memo = {v: v for v in ancestors(rv_values.values()) if not isinstance(v, Constant)}
 
     # We add `ShapeFeature` because it will get rid of references to the old
     # `RandomVariable`s that have been lifted; otherwise, it will be difficult
     # to give good warnings when an unaccounted for `RandomVariable` is
     # encountered
     fgraph = FunctionGraph(
         outputs=list(rv_values.keys()),
@@ -343,11 +359,17 @@
 
     if ir_rewriter is None:
         ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))
     ir_rewriter.rewrite(fgraph)
 
     if rv_remapper.measurable_conversions:
         # Undo un-valued measurable IR rewrites
-        new_to_old = tuple((v, k) for k, v in rv_remapper.measurable_conversions.items())
+        new_to_old = tuple((v, k) for k, v in reversed(rv_remapper.measurable_conversions.items()))
         fgraph.replace_all(new_to_old)
 
     return fgraph, rv_values, memo
+
+
+def cleanup_ir(vars: Sequence[Variable]) -> None:
+    fgraph = FunctionGraph(outputs=vars, clone=False)
+    ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["cleanup"]))
+    ir_rewriter.rewrite(fgraph)
```

### Comparing `pymc-5.4.0/pymc/logprob/scan.py` & `pymc-5.4.1/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/tensor.py` & `pymc-5.4.1/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/logprob/transforms.py` & `pymc-5.4.1/pymc/logprob/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,33 +84,32 @@
     sinh,
     sqr,
     sqrt,
     sub,
     tanh,
     true_div,
 )
-from pytensor.tensor.rewriting.basic import (
-    register_specialize,
-    register_stabilize,
-    register_useless,
-)
 from pytensor.tensor.var import TensorVariable
 
 from pymc.logprob.abstract import (
     MeasurableElemwise,
     MeasurableVariable,
     _get_measurable_outputs,
     _icdf,
     _icdf_helper,
     _logcdf,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
 )
-from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
+from pymc.logprob.rewriting import (
+    PreserveRVMappings,
+    cleanup_ir_rewrites_db,
+    measurable_ir_rewrites_db,
+)
 from pymc.logprob.utils import check_potential_measurability, ignore_logprob
 
 
 class TransformedVariable(Op):
     """A no-op that identifies a transform and its un-transformed input."""
 
     view_map = {0: [0]}
@@ -130,23 +129,28 @@
     def grad(self, args, g_outs):
         return g_outs[0], DisconnectedType()()
 
 
 transformed_variable = TransformedVariable()
 
 
-@register_specialize
-@register_stabilize
-@register_useless
 @node_rewriter([TransformedVariable])
 def remove_TransformedVariables(fgraph, node):
     if isinstance(node.op, TransformedVariable):
         return [node.inputs[0]]
 
 
+cleanup_ir_rewrites_db.register(
+    "remove_TransformedVariables",
+    remove_TransformedVariables,
+    "cleanup",
+    "transform",
+)
+
+
 class RVTransform(abc.ABC):
     ndim_supp = None
 
     @abc.abstractmethod
     def forward(self, value: TensorVariable, *inputs: Variable) -> TensorVariable:
         """Apply the transformation."""
```

### Comparing `pymc-5.4.0/pymc/logprob/utils.py` & `pymc-5.4.1/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/math.py` & `pymc-5.4.1/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/model.py` & `pymc-5.4.1/pymc/model.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/model_graph.py` & `pymc-5.4.1/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/ode/__init__.py` & `pymc-5.4.1/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/ode/ode.py` & `pymc-5.4.1/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/ode/utils.py` & `pymc-5.4.1/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/plots/__init__.py` & `pymc-5.4.1/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/printing.py` & `pymc-5.4.1/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/pytensorf.py` & `pymc-5.4.1/pymc/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/sampling/__init__.py` & `pymc-5.4.1/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/sampling/forward.py` & `pymc-5.4.1/pymc/sampling/forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,16 @@
 
 def get_vars_in_point_list(trace, model):
     """Get the list of Variable instances in the model that have values stored in the trace."""
     if not isinstance(trace, MultiTrace):
         names_in_trace = list(trace[0])
     else:
         names_in_trace = trace.varnames
-    vars_in_trace = [model[v] for v in names_in_trace if v in model]
+    traceable_varnames = {var.name for var in (model.free_RVs + model.deterministics)}
+    vars_in_trace = [model[v] for v in names_in_trace if v in traceable_varnames]
     return vars_in_trace
 
 
 def compile_forward_sampling_function(
     outputs: List[Variable],
     vars_in_trace: List[Variable],
     basic_rvs: Optional[List[Variable]] = None,
```

### Comparing `pymc-5.4.0/pymc/sampling/jax.py` & `pymc-5.4.1/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/sampling/mcmc.py` & `pymc-5.4.1/pymc/sampling/mcmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
     init: str = "auto",
     jitter_max_retries: int = 10,
     n_init: int = 200_000,
     trace: Optional[TraceOrBackend] = None,
     discard_tuned_samples: bool = True,
     compute_convergence_checks: bool = True,
     keep_warning_stat: bool = False,
-    return_inferencedata: Literal[True],
+    return_inferencedata: Literal[True] = True,
     idata_kwargs: Optional[Dict[str, Any]] = None,
     nuts_sampler_kwargs: Optional[Dict[str, Any]] = None,
     callback=None,
     mp_ctx=None,
     **kwargs,
 ) -> InferenceData:
     ...
```

### Comparing `pymc-5.4.0/pymc/sampling/parallel.py` & `pymc-5.4.1/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/sampling/population.py` & `pymc-5.4.1/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/sampling_jax.py` & `pymc-5.4.1/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/smc/__init__.py` & `pymc-5.4.1/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/smc/kernels.py` & `pymc-5.4.1/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/smc/sampling.py` & `pymc-5.4.1/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/stats/__init__.py` & `pymc-5.4.1/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/stats/convergence.py` & `pymc-5.4.1/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/stats/log_likelihood.py` & `pymc-5.4.1/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/__init__.py` & `pymc-5.4.1/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/arraystep.py` & `pymc-5.4.1/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/compound.py` & `pymc-5.4.1/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/hmc/__init__.py` & `pymc-5.4.1/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.4.1/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/hmc/hmc.py` & `pymc-5.4.1/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/hmc/integration.py` & `pymc-5.4.1/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/hmc/nuts.py` & `pymc-5.4.1/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.4.1/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/metropolis.py` & `pymc-5.4.1/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/slicer.py` & `pymc-5.4.1/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/step_methods/step_sizes.py` & `pymc-5.4.1/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/testing.py` & `pymc-5.4.1/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/tuning/__init__.py` & `pymc-5.4.1/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/tuning/scaling.py` & `pymc-5.4.1/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/tuning/starting.py` & `pymc-5.4.1/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/util.py` & `pymc-5.4.1/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/__init__.py` & `pymc-5.4.1/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/approximations.py` & `pymc-5.4.1/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/callbacks.py` & `pymc-5.4.1/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/inference.py` & `pymc-5.4.1/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/minibatch_rv.py` & `pymc-5.4.1/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/operators.py` & `pymc-5.4.1/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/opvi.py` & `pymc-5.4.1/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/stein.py` & `pymc-5.4.1/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/test_functions.py` & `pymc-5.4.1/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/variational/updates.py` & `pymc-5.4.1/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc/vartypes.py` & `pymc-5.4.1/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/pymc.egg-info/PKG-INFO` & `pymc-5.4.1/pymc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.4.0
+Version: 5.4.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.4.0/pymc.egg-info/SOURCES.txt` & `pymc-5.4.1/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/scripts/docker_container.sh` & `pymc-5.4.1/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/setup.py` & `pymc-5.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.0/versioneer.py` & `pymc-5.4.1/versioneer.py`

 * *Files identical despite different names*

