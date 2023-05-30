# Comparing `tmp/quantecon-0.7.0.tar.gz` & `tmp/quantecon-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantecon-0.7.0.tar", last modified: Mon Apr 24 09:24:58 2023, max compression
+gzip compressed data, was "quantecon-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quantecon-0.7.0.tar` & `quantecon-0.7.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0    24921 2023-04-24 09:24:51.390751 quantecon-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1540 2023-04-24 09:24:51.390751 quantecon-0.7.0/LICENSE
--rw-r--r--   0        0        0       79 2023-04-24 09:24:51.390751 quantecon-0.7.0/MANIFEST.in
--rw-r--r--   0        0        0     2667 2023-04-24 09:24:51.390751 quantecon-0.7.0/README.md
--rw-r--r--   0        0        0     1485 2023-04-24 09:24:51.390751 quantecon-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       81 2023-04-24 09:24:51.390751 quantecon-0.7.0/pytest.ini
--rw-r--r--   0        0        0     1865 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/__init__.py
--rw-r--r--   0        0        0     8070 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_arma.py
--rw-r--r--   0        0        0     3142 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_ce_util.py
--rw-r--r--   0        0        0    11894 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_compute_fp.py
--rw-r--r--   0        0        0     1940 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_discrete_rv.py
--rw-r--r--   0        0        0    13901 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_dle.py
--rw-r--r--   0        0        0     1121 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_ecdf.py
--rw-r--r--   0        0        0     4820 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_estspec.py
--rw-r--r--   0        0        0     1682 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_filter.py
--rw-r--r--   0        0        0    13594 2023-04-24 09:24:51.390751 quantecon-0.7.0/quantecon/_graph_tools.py
--rw-r--r--   0        0        0    10926 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_gridtools.py
--rw-r--r--   0        0        0     3701 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_inequality.py
--rw-r--r--   0        0        0     8993 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_ivp.py
--rw-r--r--   0        0        0     9604 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_kalman.py
--rw-r--r--   0        0        0     2066 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lae.py
--rw-r--r--   0        0        0    21811 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lqcontrol.py
--rw-r--r--   0        0        0     5224 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lqnash.py
--rw-r--r--   0        0        0    15079 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_lss.py
--rw-r--r--   0        0        0    10492 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_matrix_eqn.py
--rw-r--r--   0        0        0     2802 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_quadsums.py
--rw-r--r--   0        0        0     2965 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_rank_nullspace.py
--rw-r--r--   0        0        0    12504 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/_robustlq.py
--rw-r--r--   0        0        0      743 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/arma.py
--rw-r--r--   0        0        0      236 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/bld.bat
--rw-r--r--   0        0        0      219 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/build.sh
--rw-r--r--   0        0        0      808 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/ce_util.py
--rw-r--r--   0        0        0      822 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/compute_fp.py
--rw-r--r--   0        0        0      817 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/discrete_rv.py
--rw-r--r--   0        0        0     3164 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/distributions.py
--rw-r--r--   0        0        0      757 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/dle.py
--rw-r--r--   0        0        0      762 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/ecdf.py
--rw-r--r--   0        0        0      809 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/estspec.py
--rw-r--r--   0        0        0      781 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/filter.py
--rw-r--r--   0        0        0      881 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/__init__.py
--rw-r--r--   0        0        0     7676 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/brd.py
--rw-r--r--   0        0        0     7225 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/fictplay.py
--rw-r--r--   0        0        0       87 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/__init__.py
--rw-r--r--   0        0        0    23553 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/bimatrix_generators.py
--rw-r--r--   0        0        0        0 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/tests/__init__.py
--rw-r--r--   0        0        0     5706 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py
--rw-r--r--   0        0        0    15486 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/lemke_howson.py
--rw-r--r--   0        0        0     7502 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/localint.py
--rw-r--r--   0        0        0     5214 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/logitdyn.py
--rw-r--r--   0        0        0     9194 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/mclennan_tourky.py
--rw-r--r--   0        0        0    32142 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/normal_form_game.py
--rw-r--r--   0        0        0     1740 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/pure_nash.py
--rw-r--r--   0        0        0     6000 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/random.py
--rw-r--r--   0        0        0    14180 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/repeated_game.py
--rw-r--r--   0        0        0     5561 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/support_enumeration.py
--rw-r--r--   0        0        0        0 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_brd.py
--rw-r--r--   0        0        0     3819 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_fictplay.py
--rw-r--r--   0        0        0     4625 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_lemke_howson.py
--rw-r--r--   0        0        0     1995 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_localint.py
--rw-r--r--   0        0        0     1854 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_logitdyn.py
--rw-r--r--   0        0        0     4993 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_mclennan_tourky.py
--rw-r--r--   0        0        0    18048 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_normal_form_game.py
--rw-r--r--   0        0        0     2231 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_pure_nash.py
--rw-r--r--   0        0        0     2890 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_random.py
--rw-r--r--   0        0        0     1829 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_repeated_game.py
--rw-r--r--   0        0        0     2403 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_support_enumeration.py
--rw-r--r--   0        0        0     1292 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_utilities.py
--rw-r--r--   0        0        0     4751 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/tests/test_vertex_enumeration.py
--rw-r--r--   0        0        0     2148 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/utilities.py
--rw-r--r--   0        0        0    11232 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/game_theory/vertex_enumeration.py
--rw-r--r--   0        0        0      837 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/graph_tools.py
--rw-r--r--   0        0        0      914 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/gridtools.py
--rw-r--r--   0        0        0      845 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/inequality.py
--rw-r--r--   0        0        0      756 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/ivp.py
--rw-r--r--   0        0        0      771 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/kalman.py
--rw-r--r--   0        0        0      756 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lae.py
--rw-r--r--   0        0        0      792 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lqcontrol.py
--rw-r--r--   0        0        0      770 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lqnash.py
--rw-r--r--   0        0        0      794 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/lss.py
--rw-r--r--   0        0        0      483 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/__init__.py
--rw-r--r--   0        0        0     5267 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/_ddp_linprog_simplex.py
--rw-r--r--   0        0        0    14449 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/approximation.py
--rw-r--r--   0        0        0    25355 2023-04-24 09:24:51.394751 quantecon-0.7.0/quantecon/markov/core.py
--rw-r--r--   0        0        0    35365 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/ddp.py
--rw-r--r--   0        0        0     3315 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/estimate.py
--rw-r--r--   0        0        0     4312 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/gth_solve.py
--rw-r--r--   0        0        0     6660 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/random.py
--rw-r--r--   0        0        0        0 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/__init__.py
--rw-r--r--   0        0        0     8533 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_approximation.py
--rw-r--r--   0        0        0    19897 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_core.py
--rw-r--r--   0        0        0    11341 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_ddp.py
--rw-r--r--   0        0        0     3333 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_estimate.py
--rw-r--r--   0        0        0     5792 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_gth_solve.py
--rw-r--r--   0        0        0     4804 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_random.py
--rw-r--r--   0        0        0      471 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/tests/test_utilities.py
--rw-r--r--   0        0        0     3553 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/markov/utilities.py
--rw-r--r--   0        0        0      874 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/matrix_eqn.py
--rw-r--r--   0        0        0     1438 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/meta.yaml
--rw-r--r--   0        0        0      378 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/__init__.py
--rw-r--r--   0        0        0     7357 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/lcp_lemke.py
--rw-r--r--   0        0        0    14318 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/linprog_simplex.py
--rw-r--r--   0        0        0     2591 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/minmax.py
--rw-r--r--   0        0        0    14379 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/nelder_mead.py
--rw-r--r--   0        0        0     4892 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/pivoting.py
--rw-r--r--   0        0        0    15046 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/root_finding.py
--rw-r--r--   0        0        0     4066 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/scalar_maximization.py
--rw-r--r--   0        0        0        0 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/__init__.py
--rw-r--r--   0        0        0     3218 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_lcp_lemke.py
--rw-r--r--   0        0        0    10405 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_linprog_simplex.py
--rw-r--r--   0        0        0     1082 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_minmax.py
--rw-r--r--   0        0        0     9891 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_nelder_mead.py
--rw-r--r--   0        0        0     2763 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_root_finding.py
--rw-r--r--   0        0        0     1263 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/optimize/tests/test_scalar_max.py
--rw-r--r--   0        0        0    31716 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/quad.py
--rw-r--r--   0        0        0      809 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/quadsums.py
--rw-r--r--   0        0        0      298 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/tests/__init__.py
--rw-r--r--   0        0        0     2876 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/tests/test_utilities.py
--rw-r--r--   0        0        0     6368 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/random/utilities.py
--rw-r--r--   0        0        0      814 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/rank_nullspace.py
--rw-r--r--   0        0        0      777 2023-04-24 09:24:51.398751 quantecon-0.7.0/quantecon/robustlq.py
--rw-r--r--   0        0        0      228 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/array.py
--rw-r--r--   0        0        0     2723 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/combinatorics.py
--rw-r--r--   0        0        0      481 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/common_messages.py
--rw-r--r--   0        0        0     3849 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/notebooks.py
--rw-r--r--   0        0        0     2883 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/numba.py
--rw-r--r--   0        0        0     1257 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/random.py
--rw-r--r--   0        0        0     5239 2023-04-24 09:24:51.402752 quantecon-0.7.0/quantecon/util/timing.py
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 quantecon-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    25267 2023-05-30 07:01:41.141751 quantecon-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1540 2023-05-30 07:01:41.141751 quantecon-0.7.1/LICENSE
+-rw-r--r--   0        0        0       79 2023-05-30 07:01:41.141751 quantecon-0.7.1/MANIFEST.in
+-rw-r--r--   0        0        0     2667 2023-05-30 07:01:41.141751 quantecon-0.7.1/README.md
+-rw-r--r--   0        0        0     1485 2023-05-30 07:01:41.145751 quantecon-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-05-30 07:01:41.145751 quantecon-0.7.1/pytest.ini
+-rw-r--r--   0        0        0     1865 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/__init__.py
+-rw-r--r--   0        0        0     8070 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_arma.py
+-rw-r--r--   0        0        0     3142 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_ce_util.py
+-rw-r--r--   0        0        0    11894 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_compute_fp.py
+-rw-r--r--   0        0        0     1940 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_discrete_rv.py
+-rw-r--r--   0        0        0    13901 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_dle.py
+-rw-r--r--   0        0        0     1121 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_ecdf.py
+-rw-r--r--   0        0        0     4820 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_estspec.py
+-rw-r--r--   0        0        0     1682 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_filter.py
+-rw-r--r--   0        0        0    13594 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_graph_tools.py
+-rw-r--r--   0        0        0    10926 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_gridtools.py
+-rw-r--r--   0        0        0     3711 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_inequality.py
+-rw-r--r--   0        0        0     8993 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_ivp.py
+-rw-r--r--   0        0        0     9607 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_kalman.py
+-rw-r--r--   0        0        0     2065 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_lae.py
+-rw-r--r--   0        0        0    21811 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_lqcontrol.py
+-rw-r--r--   0        0        0     5224 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_lqnash.py
+-rw-r--r--   0        0        0    15079 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_lss.py
+-rw-r--r--   0        0        0    10492 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_matrix_eqn.py
+-rw-r--r--   0        0        0     2802 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_quadsums.py
+-rw-r--r--   0        0        0     2965 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_rank_nullspace.py
+-rw-r--r--   0        0        0    12504 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/_robustlq.py
+-rw-r--r--   0        0        0      743 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/arma.py
+-rw-r--r--   0        0        0      279 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/bld.bat
+-rw-r--r--   0        0        0       91 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/build.sh
+-rw-r--r--   0        0        0      808 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/ce_util.py
+-rw-r--r--   0        0        0      822 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/compute_fp.py
+-rw-r--r--   0        0        0      817 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/discrete_rv.py
+-rw-r--r--   0        0        0     3164 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/distributions.py
+-rw-r--r--   0        0        0      757 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/dle.py
+-rw-r--r--   0        0        0      762 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/ecdf.py
+-rw-r--r--   0        0        0      809 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/estspec.py
+-rw-r--r--   0        0        0      781 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/filter.py
+-rw-r--r--   0        0        0      881 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/__init__.py
+-rw-r--r--   0        0        0     7676 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/brd.py
+-rw-r--r--   0        0        0     7225 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/fictplay.py
+-rw-r--r--   0        0        0       87 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/game_generators/__init__.py
+-rw-r--r--   0        0        0    23553 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/game_generators/bimatrix_generators.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/game_generators/tests/__init__.py
+-rw-r--r--   0        0        0     5706 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py
+-rw-r--r--   0        0        0    15486 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/lemke_howson.py
+-rw-r--r--   0        0        0     7502 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/localint.py
+-rw-r--r--   0        0        0     5214 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/logitdyn.py
+-rw-r--r--   0        0        0     9194 2023-05-30 07:01:41.145751 quantecon-0.7.1/quantecon/game_theory/mclennan_tourky.py
+-rw-r--r--   0        0        0    32142 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/normal_form_game.py
+-rw-r--r--   0        0        0     1740 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/pure_nash.py
+-rw-r--r--   0        0        0     6000 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/random.py
+-rw-r--r--   0        0        0    14180 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/repeated_game.py
+-rw-r--r--   0        0        0     5561 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/support_enumeration.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/__init__.py
+-rw-r--r--   0        0        0     2072 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_brd.py
+-rw-r--r--   0        0        0     3819 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_fictplay.py
+-rw-r--r--   0        0        0     4625 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_lemke_howson.py
+-rw-r--r--   0        0        0     1995 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_localint.py
+-rw-r--r--   0        0        0     1854 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_logitdyn.py
+-rw-r--r--   0        0        0     4993 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_mclennan_tourky.py
+-rw-r--r--   0        0        0    18048 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_normal_form_game.py
+-rw-r--r--   0        0        0     2231 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_pure_nash.py
+-rw-r--r--   0        0        0     2890 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_random.py
+-rw-r--r--   0        0        0     1829 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_repeated_game.py
+-rw-r--r--   0        0        0     2403 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_support_enumeration.py
+-rw-r--r--   0        0        0     1292 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_utilities.py
+-rw-r--r--   0        0        0     4751 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/tests/test_vertex_enumeration.py
+-rw-r--r--   0        0        0     2148 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/utilities.py
+-rw-r--r--   0        0        0    11232 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/game_theory/vertex_enumeration.py
+-rw-r--r--   0        0        0      837 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/graph_tools.py
+-rw-r--r--   0        0        0      914 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/gridtools.py
+-rw-r--r--   0        0        0      845 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/inequality.py
+-rw-r--r--   0        0        0      756 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/ivp.py
+-rw-r--r--   0        0        0      771 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/kalman.py
+-rw-r--r--   0        0        0      756 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/lae.py
+-rw-r--r--   0        0        0      792 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/lqcontrol.py
+-rw-r--r--   0        0        0      770 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/lqnash.py
+-rw-r--r--   0        0        0      794 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/lss.py
+-rw-r--r--   0        0        0      483 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/__init__.py
+-rw-r--r--   0        0        0     5267 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/_ddp_linprog_simplex.py
+-rw-r--r--   0        0        0    14449 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/approximation.py
+-rw-r--r--   0        0        0    25355 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/core.py
+-rw-r--r--   0        0        0    35365 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/ddp.py
+-rw-r--r--   0        0        0     3315 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/estimate.py
+-rw-r--r--   0        0        0     4312 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/gth_solve.py
+-rw-r--r--   0        0        0     6660 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/random.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/__init__.py
+-rw-r--r--   0        0        0     8533 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_approximation.py
+-rw-r--r--   0        0        0    19897 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_core.py
+-rw-r--r--   0        0        0    11341 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_ddp.py
+-rw-r--r--   0        0        0     3333 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_estimate.py
+-rw-r--r--   0        0        0     5792 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_gth_solve.py
+-rw-r--r--   0        0        0     4804 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_random.py
+-rw-r--r--   0        0        0      471 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/tests/test_utilities.py
+-rw-r--r--   0        0        0     3553 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/markov/utilities.py
+-rw-r--r--   0        0        0      874 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/matrix_eqn.py
+-rw-r--r--   0        0        0     1482 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/meta.yaml
+-rw-r--r--   0        0        0      378 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/__init__.py
+-rw-r--r--   0        0        0     7357 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/lcp_lemke.py
+-rw-r--r--   0        0        0    14318 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/linprog_simplex.py
+-rw-r--r--   0        0        0     2591 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/minmax.py
+-rw-r--r--   0        0        0    14379 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/nelder_mead.py
+-rw-r--r--   0        0        0     4892 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/pivoting.py
+-rw-r--r--   0        0        0    15046 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/root_finding.py
+-rw-r--r--   0        0        0     4066 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/scalar_maximization.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/__init__.py
+-rw-r--r--   0        0        0     3218 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/test_lcp_lemke.py
+-rw-r--r--   0        0        0    10405 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/test_linprog_simplex.py
+-rw-r--r--   0        0        0     1082 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/test_minmax.py
+-rw-r--r--   0        0        0     9891 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/test_nelder_mead.py
+-rw-r--r--   0        0        0     2763 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/test_root_finding.py
+-rw-r--r--   0        0        0     1263 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/optimize/tests/test_scalar_max.py
+-rw-r--r--   0        0        0    31716 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/quad.py
+-rw-r--r--   0        0        0      809 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/quadsums.py
+-rw-r--r--   0        0        0      298 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/random/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/random/tests/__init__.py
+-rw-r--r--   0        0        0     3061 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/random/tests/test_utilities.py
+-rw-r--r--   0        0        0     6383 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/random/utilities.py
+-rw-r--r--   0        0        0      814 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/rank_nullspace.py
+-rw-r--r--   0        0        0      777 2023-05-30 07:01:41.149751 quantecon-0.7.1/quantecon/robustlq.py
+-rw-r--r--   0        0        0      228 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/__init__.py
+-rw-r--r--   0        0        0     1223 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/array.py
+-rw-r--r--   0        0        0     2723 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/combinatorics.py
+-rw-r--r--   0        0        0      481 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/common_messages.py
+-rw-r--r--   0        0        0     3849 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/notebooks.py
+-rw-r--r--   0        0        0     2883 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/numba.py
+-rw-r--r--   0        0        0     1257 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/random.py
+-rw-r--r--   0        0        0     5239 2023-05-30 07:01:41.153751 quantecon-0.7.1/quantecon/util/timing.py
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 quantecon-0.7.1/PKG-INFO
```

### Comparing `quantecon-0.7.0/CHANGELOG.md` & `quantecon-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # Changelog
 
-## Ver 0.7.0 (24-February-2023)
+## Ver 0.7.1 (29-May-2023)
+
+This is a minor release with bug fixes and improvements to documentation. 
+
+### Fix
+
+1. [Fix for #704](https://github.com/QuantEcon/QuantEcon.py/commit/beec748020bace3834bff9afa83067f668357a24)
+
+Thank you to [oyamad](https://github.com/oyamad), [HengchengZhang](https://github.com/HengchengZhang) for your
+contributions
+
+## Ver 0.7.0 (24-April-2023)
 
 ### New
 
 1. [END: Add function fit_discrete_mc](https://github.com/QuantEcon/QuantEcon.py/pull/681) ([jstac](https://github.com/jstac)), ([Smit-create](https://github.com/Smit-create)) and ([oyamad](https://github.com/oyamad)) which takes a time series and fits a finite markov chain
 2. [ENH: Adding Discrete Approximation of VAR Methods](https://github.com/QuantEcon/QuantEcon.py/pull/640) ([crondonm](https://github.com/crondonm)) 
 3. [ENH: Implement LCP solver](https://github.com/QuantEcon/QuantEcon.py/pull/690) ([oyamad](https://github.com/oyamad))
```

### Comparing `quantecon-0.7.0/LICENSE` & `quantecon-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/README.md` & `quantecon-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/pyproject.toml` & `quantecon-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/__init__.py` & `quantecon-0.7.1/quantecon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 """
 Import the main names to top level.
 """
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 try:
     import numba
 except:
     raise ImportError(
         "Cannot import numba from current anaconda distribution. \
             Please run `conda install numba` to install the latest version.")
```

### Comparing `quantecon-0.7.0/quantecon/_arma.py` & `quantecon-0.7.1/quantecon/_arma.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_ce_util.py` & `quantecon-0.7.1/quantecon/_ce_util.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_compute_fp.py` & `quantecon-0.7.1/quantecon/_compute_fp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_discrete_rv.py` & `quantecon-0.7.1/quantecon/_discrete_rv.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_dle.py` & `quantecon-0.7.1/quantecon/_dle.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_ecdf.py` & `quantecon-0.7.1/quantecon/_ecdf.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_estspec.py` & `quantecon-0.7.1/quantecon/_estspec.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_filter.py` & `quantecon-0.7.1/quantecon/_filter.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_graph_tools.py` & `quantecon-0.7.1/quantecon/_graph_tools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_gridtools.py` & `quantecon-0.7.1/quantecon/_gridtools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_inequality.py` & `quantecon-0.7.1/quantecon/_inequality.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,15 +104,16 @@
 
         An index equal to 0 indicates complete immobility.
 
     References
     ----------
     .. [1] Wealth distribution and social mobility in the US:
        A quantitative approach (Benhabib, Bisin, Luo, 2017).
-       https://www.econ.nyu.edu/user/bisina/RevisionAugust.pdf
+       https://www.aeaweb.org/articles?id=10.1257/aer.20151684
+
     """
 
     A = np.asarray(A)  # Convert to array if not already
     m, n = A.shape
 
     if m != n:
         raise ValueError('A must be a square matrix')
@@ -140,14 +141,15 @@
 
     Returns
     -------
     rank_data : array_like(float, ndim=1)
         Location in the population when sorted from smallest to largest
     size_data : array_like(float, ndim=1)
         Size data for top (c x 100)% of the observations
+        
     """
     w = - np.sort(- data)                  # Reverse sort
     w = w[:int(len(w) * c)]                # extract top (c * 100)%
     rank_data = np.arange(len(w)) + 1
     size_data = w
     return rank_data, size_data
```

### Comparing `quantecon-0.7.0/quantecon/_ivp.py` & `quantecon-0.7.1/quantecon/_ivp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_kalman.py` & `quantecon-0.7.1/quantecon/_kalman.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Implements the Kalman filter for a linear Gaussian state space model.
 
 References
 ----------
 
-https://lectures.quantecon.org/py/kalman.html
+https://python.quantecon.org/kalman.html
 
 """
 from textwrap import dedent
 import numpy as np
 from scipy.linalg import inv
 from ._lss import LinearStateSpace
 from ._matrix_eqn import solve_discrete_riccati
@@ -49,19 +49,18 @@
     ----------
     Sigma, x_hat : as above
     Sigma_infinity : array_like or scalar(float)
         The infinite limit of Sigma_t
     K_infinity : array_like or scalar(float)
         The stationary Kalman gain.
 
-
     References
     ----------
 
-    https://lectures.quantecon.org/py/kalman.html
+    https://python.quantecon.org/kalman.html
 
     """
 
     def __init__(self, ss, x_hat=None, Sigma=None):
         self.ss = ss
         self.set_state(x_hat, Sigma)
         self._K_infinity = None
@@ -150,14 +149,15 @@
         that defines the Kalman instance
 
         Returns
         -------
         whitened_lss : LinearStateSpace
             This is the linear state space system that represents
             the whitened system
+
         """
         K = self.K_infinity
 
         # Get the matrix sizes
         n, k, m, l = self.ss.n, self.ss.k, self.ss.m, self.ss.l
         A, C, G, H = self.ss.A, self.ss.C, self.ss.G, self.ss.H
 
@@ -285,14 +285,15 @@
         Parameters
         ----------
         j : int
             The lag length
         coeff_type : string, either 'ma' or 'var' (default='ma')
             The type of coefficent sequence to compute.  Either 'ma' for
             moving average or 'var' for VAR.
+            
         """
         # == simplify notation == #
         A, G = self.ss.A, self.ss.G
         K_infinity = self.K_infinity
         # == compute and return coefficients == #
         coeffs = []
         i = 1
```

### Comparing `quantecon-0.7.0/quantecon/_lae.py` & `quantecon-0.7.1/quantecon/_lae.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     \frac{1}{n} \sum_{i=0}^n p(X_{t-1}^i, y)
 
 This is a density in :math:`y`.
 
 References
 ----------
 
-https://lectures.quantecon.org/py/stationary_densities.html
+https://python.quantecon.org/ar1_processes.html
 
 """
 from textwrap import dedent
 import numpy as np
 
 
 class LAE:
@@ -52,14 +52,15 @@
     def __repr__(self):
         return self.__str__()
 
     def __str__(self):
         m = """\
         Look ahead estimator
           - number of observations : {n}
+          
         """
         return dedent(m.format(n=self.X.size))
 
     def __call__(self, y):
         """
         A vectorized function that returns the value of the look ahead
         estimate at the values in the array y.
```

### Comparing `quantecon-0.7.0/quantecon/_lqcontrol.py` & `quantecon-0.7.1/quantecon/_lqcontrol.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_lqnash.py` & `quantecon-0.7.1/quantecon/_lqnash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_lss.py` & `quantecon-0.7.1/quantecon/_lss.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_matrix_eqn.py` & `quantecon-0.7.1/quantecon/_matrix_eqn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_quadsums.py` & `quantecon-0.7.1/quantecon/_quadsums.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_rank_nullspace.py` & `quantecon-0.7.1/quantecon/_rank_nullspace.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/_robustlq.py` & `quantecon-0.7.1/quantecon/_robustlq.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/arma.py` & `quantecon-0.7.1/quantecon/arma.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/ce_util.py` & `quantecon-0.7.1/quantecon/ce_util.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/compute_fp.py` & `quantecon-0.7.1/quantecon/compute_fp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/discrete_rv.py` & `quantecon-0.7.1/quantecon/discrete_rv.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/distributions.py` & `quantecon-0.7.1/quantecon/distributions.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/dle.py` & `quantecon-0.7.1/quantecon/dle.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/ecdf.py` & `quantecon-0.7.1/quantecon/ecdf.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/estspec.py` & `quantecon-0.7.1/quantecon/estspec.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/filter.py` & `quantecon-0.7.1/quantecon/filter.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/__init__.py` & `quantecon-0.7.1/quantecon/game_theory/__init__.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/brd.py` & `quantecon-0.7.1/quantecon/game_theory/brd.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/fictplay.py` & `quantecon-0.7.1/quantecon/game_theory/fictplay.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/game_generators/bimatrix_generators.py` & `quantecon-0.7.1/quantecon/game_theory/game_generators/bimatrix_generators.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py` & `quantecon-0.7.1/quantecon/game_theory/game_generators/tests/test_bimatrix_generators.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/lemke_howson.py` & `quantecon-0.7.1/quantecon/game_theory/lemke_howson.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/localint.py` & `quantecon-0.7.1/quantecon/game_theory/localint.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/logitdyn.py` & `quantecon-0.7.1/quantecon/game_theory/logitdyn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/mclennan_tourky.py` & `quantecon-0.7.1/quantecon/game_theory/mclennan_tourky.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/normal_form_game.py` & `quantecon-0.7.1/quantecon/game_theory/normal_form_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/pure_nash.py` & `quantecon-0.7.1/quantecon/game_theory/pure_nash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/random.py` & `quantecon-0.7.1/quantecon/game_theory/random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/repeated_game.py` & `quantecon-0.7.1/quantecon/game_theory/repeated_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/support_enumeration.py` & `quantecon-0.7.1/quantecon/game_theory/support_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_brd.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_brd.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_fictplay.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_fictplay.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_lemke_howson.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_lemke_howson.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_localint.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_localint.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_logitdyn.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_logitdyn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_mclennan_tourky.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_mclennan_tourky.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_normal_form_game.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_normal_form_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_pure_nash.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_pure_nash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_random.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_repeated_game.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_repeated_game.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_support_enumeration.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_support_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_utilities.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/tests/test_vertex_enumeration.py` & `quantecon-0.7.1/quantecon/game_theory/tests/test_vertex_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/utilities.py` & `quantecon-0.7.1/quantecon/game_theory/utilities.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/game_theory/vertex_enumeration.py` & `quantecon-0.7.1/quantecon/game_theory/vertex_enumeration.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/graph_tools.py` & `quantecon-0.7.1/quantecon/graph_tools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/gridtools.py` & `quantecon-0.7.1/quantecon/gridtools.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/inequality.py` & `quantecon-0.7.1/quantecon/inequality.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/ivp.py` & `quantecon-0.7.1/quantecon/ivp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/kalman.py` & `quantecon-0.7.1/quantecon/kalman.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/lae.py` & `quantecon-0.7.1/quantecon/lae.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/lqcontrol.py` & `quantecon-0.7.1/quantecon/lqcontrol.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/lqnash.py` & `quantecon-0.7.1/quantecon/lqnash.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/lss.py` & `quantecon-0.7.1/quantecon/lss.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/_ddp_linprog_simplex.py` & `quantecon-0.7.1/quantecon/markov/_ddp_linprog_simplex.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/approximation.py` & `quantecon-0.7.1/quantecon/markov/approximation.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/core.py` & `quantecon-0.7.1/quantecon/markov/core.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/ddp.py` & `quantecon-0.7.1/quantecon/markov/ddp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/estimate.py` & `quantecon-0.7.1/quantecon/markov/estimate.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/gth_solve.py` & `quantecon-0.7.1/quantecon/markov/gth_solve.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/random.py` & `quantecon-0.7.1/quantecon/markov/random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/tests/test_approximation.py` & `quantecon-0.7.1/quantecon/markov/tests/test_approximation.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/tests/test_core.py` & `quantecon-0.7.1/quantecon/markov/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/tests/test_ddp.py` & `quantecon-0.7.1/quantecon/markov/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/tests/test_estimate.py` & `quantecon-0.7.1/quantecon/markov/tests/test_estimate.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/tests/test_gth_solve.py` & `quantecon-0.7.1/quantecon/markov/tests/test_gth_solve.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/tests/test_random.py` & `quantecon-0.7.1/quantecon/markov/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/markov/utilities.py` & `quantecon-0.7.1/quantecon/markov/utilities.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/matrix_eqn.py` & `quantecon-0.7.1/quantecon/matrix_eqn.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/meta.yaml` & `quantecon-0.7.1/quantecon/meta.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -55,12 +55,12 @@
   # requires:
     # Put any additional test requirements here.  For example
     # - nose
 
 about:
   home: https://github.com/jstac/quant-econ
   license: BSD
-  summary: 'Code for quant-econ.net'
-
+  summary: 'Code for quantecon.org'
+  
 # See
-# http://docs.continuum.io/conda/build.html for
-# more information about meta.yaml
+# https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html for 
+# more information about meta.yaml
```

### Comparing `quantecon-0.7.0/quantecon/optimize/lcp_lemke.py` & `quantecon-0.7.1/quantecon/optimize/lcp_lemke.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/linprog_simplex.py` & `quantecon-0.7.1/quantecon/optimize/linprog_simplex.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/minmax.py` & `quantecon-0.7.1/quantecon/optimize/minmax.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/nelder_mead.py` & `quantecon-0.7.1/quantecon/optimize/nelder_mead.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/pivoting.py` & `quantecon-0.7.1/quantecon/optimize/pivoting.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/root_finding.py` & `quantecon-0.7.1/quantecon/optimize/root_finding.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/scalar_maximization.py` & `quantecon-0.7.1/quantecon/optimize/scalar_maximization.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/tests/test_lcp_lemke.py` & `quantecon-0.7.1/quantecon/optimize/tests/test_lcp_lemke.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/tests/test_linprog_simplex.py` & `quantecon-0.7.1/quantecon/optimize/tests/test_linprog_simplex.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/tests/test_minmax.py` & `quantecon-0.7.1/quantecon/optimize/tests/test_minmax.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/tests/test_nelder_mead.py` & `quantecon-0.7.1/quantecon/optimize/tests/test_nelder_mead.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/tests/test_root_finding.py` & `quantecon-0.7.1/quantecon/optimize/tests/test_root_finding.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/optimize/tests/test_scalar_max.py` & `quantecon-0.7.1/quantecon/optimize/tests/test_scalar_max.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/quad.py` & `quantecon-0.7.1/quantecon/quad.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/quadsums.py` & `quantecon-0.7.1/quantecon/quadsums.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/random/tests/test_utilities.py` & `quantecon-0.7.1/quantecon/random/tests/test_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,7 +104,18 @@
         size = 1000000
         for func in self.draw_funcs:
             out = func(self.cdf, size)
             hist, bin_edges = np.histogram(out, bins=self.n, density=True)
             pmf_computed = hist * np.diff(bin_edges)
             atol = 1e-2
             assert_allclose(pmf_computed, self.pmf, atol=atol)
+
+
+@njit
+def draw_jitted_w_o_size(n):
+    cdf = np.linspace(1/n, 1, n)
+    return draw(cdf)
+
+
+def test_draw_jitted_w_o_size():
+    n = 3
+    assert_(draw_jitted_w_o_size(n) in range(n))
```

### Comparing `quantecon-0.7.0/quantecon/random/utilities.py` & `quantecon-0.7.1/quantecon/random/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,20 +207,20 @@
     else:
         r = np.random.random()
         return searchsorted(cdf, r)
 
 
 # Overload for the `draw` function
 @overload(draw)
-def ol_draw(cdf, size):
+def ol_draw(cdf, size=None):
     if isinstance(size, types.Integer):
-        def draw_impl(cdf, size):
+        def draw_impl(cdf, size=None):
             rs = np.random.random(size)
             out = np.empty(size, dtype=np.int_)
             for i in range(size):
                 out[i] = searchsorted(cdf, rs[i])
             return out
     else:
-        def draw_impl(cdf, size):
+        def draw_impl(cdf, size=None):
             r = np.random.random()
             return searchsorted(cdf, r)
     return draw_impl
```

### Comparing `quantecon-0.7.0/quantecon/rank_nullspace.py` & `quantecon-0.7.1/quantecon/rank_nullspace.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/robustlq.py` & `quantecon-0.7.1/quantecon/robustlq.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/util/array.py` & `quantecon-0.7.1/quantecon/util/array.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/util/combinatorics.py` & `quantecon-0.7.1/quantecon/util/combinatorics.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/util/notebooks.py` & `quantecon-0.7.1/quantecon/util/notebooks.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/util/numba.py` & `quantecon-0.7.1/quantecon/util/numba.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/util/random.py` & `quantecon-0.7.1/quantecon/util/random.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/quantecon/util/timing.py` & `quantecon-0.7.1/quantecon/util/timing.py`

 * *Files identical despite different names*

### Comparing `quantecon-0.7.0/PKG-INFO` & `quantecon-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantecon
-Version: 0.7.0
+Version: 0.7.1
 Summary: Import the main names to top level.
 Keywords: quantitative,economics
 Author-email: QuantEcon Project <admin@quantecon.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

