# Comparing `tmp/optuna-3.1.1.tar.gz` & `tmp/optuna-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-3.1.1.tar", last modified: Fri Apr  7 07:55:15 2023, max compression
+gzip compressed data, was "optuna-3.2.0.tar", last modified: Tue May 30 06:00:24 2023, max compression
```

## Comparing `optuna-3.1.1.tar` & `optuna-3.2.0.tar`

### file list

```diff
@@ -1,231 +1,253 @@
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.304415 optuna-3.1.1/
--rw-r--r--   0 mamu       (501) staff       (20)     3016 2023-01-13 07:07:35.000000 optuna-3.1.1/LICENSE
--rw-r--r--   0 mamu       (501) staff       (20)       16 2022-11-30 02:55:49.000000 optuna-3.1.1/MANIFEST.in
--rw-r--r--   0 mamu       (501) staff       (20)    11331 2023-04-07 07:55:15.304534 optuna-3.1.1/PKG-INFO
--rw-r--r--   0 mamu       (501) staff       (20)     8478 2023-04-07 07:49:53.000000 optuna-3.1.1/README.md
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.249302 optuna-3.1.1/benchmarks/
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.256885 optuna-3.1.1/benchmarks/asv/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/benchmarks/asv/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     2027 2022-12-23 05:37:15.000000 optuna-3.1.1/benchmarks/asv/optimize.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.257482 optuna-3.1.1/benchmarks/kurobako/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/benchmarks/kurobako/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)      969 2023-04-07 07:49:53.000000 optuna-3.1.1/benchmarks/kurobako/mo_create_study.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.257963 optuna-3.1.1/benchmarks/naslib/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/benchmarks/naslib/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     2758 2023-04-07 07:49:53.000000 optuna-3.1.1/benchmarks/naslib/problem.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.262105 optuna-3.1.1/optuna/
--rw-r--r--   0 mamu       (501) staff       (20)     1264 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     6350 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/_callbacks.py
--rw-r--r--   0 mamu       (501) staff       (20)     2395 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/_convert_positional_args.py
--rw-r--r--   0 mamu       (501) staff       (20)     6949 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/_deprecated.py
--rw-r--r--   0 mamu       (501) staff       (20)     3832 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/_experimental.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.264644 optuna-3.1.1/optuna/_hypervolume/
--rw-r--r--   0 mamu       (501) staff       (20)      373 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/_hypervolume/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     2871 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/_hypervolume/base.py
--rw-r--r--   0 mamu       (501) staff       (20)     1683 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/_hypervolume/hssp.py
--rw-r--r--   0 mamu       (501) staff       (20)     1460 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/_hypervolume/utils.py
--rw-r--r--   0 mamu       (501) staff       (20)     4130 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/_hypervolume/wfg.py
--rw-r--r--   0 mamu       (501) staff       (20)     4069 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/_imports.py
--rw-r--r--   0 mamu       (501) staff       (20)    12143 2023-04-05 02:26:58.000000 optuna-3.1.1/optuna/_transform.py
--rw-r--r--   0 mamu       (501) staff       (20)    36895 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/cli.py
--rw-r--r--   0 mamu       (501) staff       (20)    27969 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/distributions.py
--rw-r--r--   0 mamu       (501) staff       (20)     2442 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/exceptions.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.265366 optuna-3.1.1/optuna/importance/
--rw-r--r--   0 mamu       (501) staff       (20)     4685 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/importance/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     6725 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/importance/_base.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.266210 optuna-3.1.1/optuna/importance/_fanova/
--rw-r--r--   0 mamu       (501) staff       (20)      117 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/importance/_fanova/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     5265 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/importance/_fanova/_evaluator.py
--rw-r--r--   0 mamu       (501) staff       (20)     4207 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/importance/_fanova/_fanova.py
--rw-r--r--   0 mamu       (501) staff       (20)    12189 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/importance/_fanova/_tree.py
--rw-r--r--   0 mamu       (501) staff       (20)     3888 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/importance/_mean_decrease_impurity.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.271997 optuna-3.1.1/optuna/integration/
--rw-r--r--   0 mamu       (501) staff       (20)     5651 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/__init__.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.273856 optuna-3.1.1/optuna/integration/_lightgbm_tuner/
--rw-r--r--   0 mamu       (501) staff       (20)     1698 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/integration/_lightgbm_tuner/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     3499 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/integration/_lightgbm_tuner/alias.py
--rw-r--r--   0 mamu       (501) staff       (20)    43841 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/_lightgbm_tuner/optimize.py
--rw-r--r--   0 mamu       (501) staff       (20)     1239 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/_lightgbm_tuner/sklearn.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.275143 optuna-3.1.1/optuna/integration/allennlp/
--rw-r--r--   0 mamu       (501) staff       (20)      294 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/allennlp/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     2016 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/allennlp/_dump_best_config.py
--rw-r--r--   0 mamu       (501) staff       (20)      367 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/allennlp/_environment.py
--rw-r--r--   0 mamu       (501) staff       (20)     9781 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/allennlp/_executor.py
--rw-r--r--   0 mamu       (501) staff       (20)     8052 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/allennlp/_pruner.py
--rw-r--r--   0 mamu       (501) staff       (20)     2706 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/allennlp/_variables.py
--rw-r--r--   0 mamu       (501) staff       (20)    24941 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/botorch.py
--rw-r--r--   0 mamu       (501) staff       (20)      940 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/integration/catalyst.py
--rw-r--r--   0 mamu       (501) staff       (20)     4542 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/integration/catboost.py
--rw-r--r--   0 mamu       (501) staff       (20)     4284 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/chainer.py
--rw-r--r--   0 mamu       (501) staff       (20)    11287 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/chainermn.py
--rw-r--r--   0 mamu       (501) staff       (20)    20465 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/cma.py
--rw-r--r--   0 mamu       (501) staff       (20)    26584 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/dask.py
--rw-r--r--   0 mamu       (501) staff       (20)     2667 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/fastaiv1.py
--rw-r--r--   0 mamu       (501) staff       (20)     2646 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/integration/fastaiv2.py
--rw-r--r--   0 mamu       (501) staff       (20)     2799 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/keras.py
--rw-r--r--   0 mamu       (501) staff       (20)     6076 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/lightgbm.py
--rw-r--r--   0 mamu       (501) staff       (20)    11837 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/mlflow.py
--rw-r--r--   0 mamu       (501) staff       (20)     2103 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/mxnet.py
--rw-r--r--   0 mamu       (501) staff       (20)    12567 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/pytorch_distributed.py
--rw-r--r--   0 mamu       (501) staff       (20)     1411 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/pytorch_ignite.py
--rw-r--r--   0 mamu       (501) staff       (20)     5361 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/pytorch_lightning.py
--rw-r--r--   0 mamu       (501) staff       (20)     4282 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/shap.py
--rw-r--r--   0 mamu       (501) staff       (20)    31269 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/sklearn.py
--rw-r--r--   0 mamu       (501) staff       (20)    14132 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/skopt.py
--rw-r--r--   0 mamu       (501) staff       (20)     1397 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/skorch.py
--rw-r--r--   0 mamu       (501) staff       (20)     4030 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/tensorboard.py
--rw-r--r--   0 mamu       (501) staff       (20)     3036 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/tensorflow.py
--rw-r--r--   0 mamu       (501) staff       (20)     1885 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/tfkeras.py
--rw-r--r--   0 mamu       (501) staff       (20)     8336 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/wandb.py
--rw-r--r--   0 mamu       (501) staff       (20)     4822 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/integration/xgboost.py
--rw-r--r--   0 mamu       (501) staff       (20)    10009 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/logging.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.276284 optuna-3.1.1/optuna/multi_objective/
--rw-r--r--   0 mamu       (501) staff       (20)      437 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/multi_objective/__init__.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.277700 optuna-3.1.1/optuna/multi_objective/samplers/
--rw-r--r--   0 mamu       (501) staff       (20)      586 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/multi_objective/samplers/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     1989 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/multi_objective/samplers/_adapter.py
--rw-r--r--   0 mamu       (501) staff       (20)     4462 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/multi_objective/samplers/_base.py
--rw-r--r--   0 mamu       (501) staff       (20)     7401 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/multi_objective/samplers/_motpe.py
--rw-r--r--   0 mamu       (501) staff       (20)    13788 2023-01-04 00:56:42.000000 optuna-3.1.1/optuna/multi_objective/samplers/_nsga2.py
--rw-r--r--   0 mamu       (501) staff       (20)     2734 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/multi_objective/samplers/_random.py
--rw-r--r--   0 mamu       (501) staff       (20)    17554 2023-03-08 09:46:04.000000 optuna-3.1.1/optuna/multi_objective/study.py
--rw-r--r--   0 mamu       (501) staff       (20)    13674 2023-03-08 09:46:04.000000 optuna-3.1.1/optuna/multi_objective/trial.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.278136 optuna-3.1.1/optuna/multi_objective/visualization/
--rw-r--r--   0 mamu       (501) staff       (20)      177 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/multi_objective/visualization/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     7361 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/multi_objective/visualization/_pareto_front.py
--rw-r--r--   0 mamu       (501) staff       (20)     4237 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/progress_bar.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.280209 optuna-3.1.1/optuna/pruners/
--rw-r--r--   0 mamu       (501) staff       (20)     1107 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/pruners/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)      910 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/pruners/_base.py
--rw-r--r--   0 mamu       (501) staff       (20)    13907 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_hyperband.py
--rw-r--r--   0 mamu       (501) staff       (20)     2958 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_median.py
--rw-r--r--   0 mamu       (501) staff       (20)     1505 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_nop.py
--rw-r--r--   0 mamu       (501) staff       (20)     4167 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_patient.py
--rw-r--r--   0 mamu       (501) staff       (20)     7187 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_percentile.py
--rw-r--r--   0 mamu       (501) staff       (20)    10373 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_successive_halving.py
--rw-r--r--   0 mamu       (501) staff       (20)     4504 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/pruners/_threshold.py
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/py.typed
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.282481 optuna-3.1.1/optuna/samplers/
--rw-r--r--   0 mamu       (501) staff       (20)     1007 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/samplers/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     8195 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_base.py
--rw-r--r--   0 mamu       (501) staff       (20)     4581 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_brute_force.py
--rw-r--r--   0 mamu       (501) staff       (20)    26529 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_cmaes.py
--rw-r--r--   0 mamu       (501) staff       (20)    10853 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_grid.py
--rw-r--r--   0 mamu       (501) staff       (20)     3704 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_partial_fixed.py
--rw-r--r--   0 mamu       (501) staff       (20)    12886 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_qmc.py
--rw-r--r--   0 mamu       (501) staff       (20)     1893 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_random.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.283589 optuna-3.1.1/optuna/samplers/_search_space/
--rw-r--r--   0 mamu       (501) staff       (20)      464 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_search_space/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     2320 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_search_space/group_decomposed.py
--rw-r--r--   0 mamu       (501) staff       (20)     5252 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_search_space/intersection.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.284753 optuna-3.1.1/optuna/samplers/_tpe/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/samplers/_tpe/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     6036 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_tpe/_erf.py
--rw-r--r--   0 mamu       (501) staff       (20)     7552 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_tpe/_truncnorm.py
--rw-r--r--   0 mamu       (501) staff       (20)     4553 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_tpe/multi_objective_sampler.py
--rw-r--r--   0 mamu       (501) staff       (20)    18802 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_tpe/parzen_estimator.py
--rw-r--r--   0 mamu       (501) staff       (20)    34500 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/_tpe/sampler.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.285389 optuna-3.1.1/optuna/samplers/nsgaii/
--rw-r--r--   0 mamu       (501) staff       (20)      647 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/samplers/nsgaii/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     5907 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossover.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.286920 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     1972 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_base.py
--rw-r--r--   0 mamu       (501) staff       (20)     1650 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_blxalpha.py
--rw-r--r--   0 mamu       (501) staff       (20)     3901 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_sbx.py
--rw-r--r--   0 mamu       (501) staff       (20)     2130 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_spx.py
--rw-r--r--   0 mamu       (501) staff       (20)     4088 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_undx.py
--rw-r--r--   0 mamu       (501) staff       (20)     1522 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_uniform.py
--rw-r--r--   0 mamu       (501) staff       (20)     3250 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_vsbx.py
--rw-r--r--   0 mamu       (501) staff       (20)    22130 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/samplers/nsgaii/_sampler.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.288227 optuna-3.1.1/optuna/storages/
--rw-r--r--   0 mamu       (501) staff       (20)     1628 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/storages/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)    19165 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_base.py
--rw-r--r--   0 mamu       (501) staff       (20)    17417 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_cached_storage.py
--rw-r--r--   0 mamu       (501) staff       (20)     5853 2023-01-04 00:56:42.000000 optuna-3.1.1/optuna/storages/_heartbeat.py
--rw-r--r--   0 mamu       (501) staff       (20)    14394 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_in_memory.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.289546 optuna-3.1.1/optuna/storages/_journal/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/storages/_journal/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     2128 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/storages/_journal/base.py
--rw-r--r--   0 mamu       (501) staff       (20)     6567 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/storages/_journal/file.py
--rw-r--r--   0 mamu       (501) staff       (20)     3813 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_journal/redis.py
--rw-r--r--   0 mamu       (501) staff       (20)    25816 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_journal/storage.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.290572 optuna-3.1.1/optuna/storages/_rdb/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/__init__.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.291185 optuna-3.1.1/optuna/storages/_rdb/alembic/
--rw-r--r--   0 mamu       (501) staff       (20)     2161 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/env.py
--rw-r--r--   0 mamu       (501) staff       (20)      494 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/script.py.mako
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.293390 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/
--rw-r--r--   0 mamu       (501) staff       (20)     5455 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py
--rw-r--r--   0 mamu       (501) staff       (20)      963 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py
--rw-r--r--   0 mamu       (501) staff       (20)     2828 2023-01-13 07:07:35.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py
--rw-r--r--   0 mamu       (501) staff       (20)     6406 2023-01-13 07:07:35.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py
--rw-r--r--   0 mamu       (501) staff       (20)     1722 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py
--rw-r--r--   0 mamu       (501) staff       (20)     6206 2023-01-13 07:07:35.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py
--rw-r--r--   0 mamu       (501) staff       (20)     2955 2023-01-13 07:07:35.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py
--rw-r--r--   0 mamu       (501) staff       (20)     6423 2023-01-13 07:07:35.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py
--rw-r--r--   0 mamu       (501) staff       (20)     5855 2023-01-13 07:07:35.000000 optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py
--rw-r--r--   0 mamu       (501) staff       (20)     1697 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/storages/_rdb/alembic.ini
--rw-r--r--   0 mamu       (501) staff       (20)    19491 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_rdb/models.py
--rw-r--r--   0 mamu       (501) staff       (20)    47949 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/storages/_rdb/storage.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.295525 optuna-3.1.1/optuna/study/
--rw-r--r--   0 mamu       (501) staff       (20)      625 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/study/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     3791 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/study/_dataframe.py
--rw-r--r--   0 mamu       (501) staff       (20)     2826 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/study/_frozen.py
--rw-r--r--   0 mamu       (501) staff       (20)     3398 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/study/_multi_objective.py
--rw-r--r--   0 mamu       (501) staff       (20)     9008 2023-01-30 01:49:04.000000 optuna-3.1.1/optuna/study/_optimize.py
--rw-r--r--   0 mamu       (501) staff       (20)      421 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/study/_study_direction.py
--rw-r--r--   0 mamu       (501) staff       (20)     4212 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/study/_study_summary.py
--rw-r--r--   0 mamu       (501) staff       (20)     6610 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/study/_tell.py
--rw-r--r--   0 mamu       (501) staff       (20)    51543 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/study/study.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.297389 optuna-3.1.1/optuna/testing/
--rw-r--r--   0 mamu       (501) staff       (20)        0 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/testing/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)      472 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/testing/distributions.py
--rw-r--r--   0 mamu       (501) staff       (20)      197 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/testing/objectives.py
--rw-r--r--   0 mamu       (501) staff       (20)      284 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/testing/pruners.py
--rw-r--r--   0 mamu       (501) staff       (20)     1996 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/testing/samplers.py
--rw-r--r--   0 mamu       (501) staff       (20)     3399 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/testing/storages.py
--rw-r--r--   0 mamu       (501) staff       (20)      645 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/testing/threading.py
--rw-r--r--   0 mamu       (501) staff       (20)     2468 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/testing/visualization.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.298592 optuna-3.1.1/optuna/trial/
--rw-r--r--   0 mamu       (501) staff       (20)      377 2022-11-30 02:55:49.000000 optuna-3.1.1/optuna/trial/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)     3620 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/trial/_base.py
--rw-r--r--   0 mamu       (501) staff       (20)     6105 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/trial/_fixed.py
--rw-r--r--   0 mamu       (501) staff       (20)    19797 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/trial/_frozen.py
--rw-r--r--   0 mamu       (501) staff       (20)     1029 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/trial/_state.py
--rw-r--r--   0 mamu       (501) staff       (20)    28829 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/trial/_trial.py
--rw-r--r--   0 mamu       (501) staff       (20)       22 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/version.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.301752 optuna-3.1.1/optuna/visualization/
--rw-r--r--   0 mamu       (501) staff       (20)      889 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)    13632 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_contour.py
--rw-r--r--   0 mamu       (501) staff       (20)     5873 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_edf.py
--rw-r--r--   0 mamu       (501) staff       (20)     3383 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_intermediate_values.py
--rw-r--r--   0 mamu       (501) staff       (20)     8112 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_optimization_history.py
--rw-r--r--   0 mamu       (501) staff       (20)    10954 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_parallel_coordinate.py
--rw-r--r--   0 mamu       (501) staff       (20)     6290 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_param_importances.py
--rw-r--r--   0 mamu       (501) staff       (20)    17377 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_pareto_front.py
--rw-r--r--   0 mamu       (501) staff       (20)      851 2022-12-23 05:37:15.000000 optuna-3.1.1/optuna/visualization/_plotly_imports.py
--rw-r--r--   0 mamu       (501) staff       (20)     7109 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_slice.py
--rw-r--r--   0 mamu       (501) staff       (20)     5476 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/_utils.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.304225 optuna-3.1.1/optuna/visualization/matplotlib/
--rw-r--r--   0 mamu       (501) staff       (20)      926 2023-04-07 07:49:39.000000 optuna-3.1.1/optuna/visualization/matplotlib/__init__.py
--rw-r--r--   0 mamu       (501) staff       (20)    13194 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_contour.py
--rw-r--r--   0 mamu       (501) staff       (20)     4076 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_edf.py
--rw-r--r--   0 mamu       (501) staff       (20)     3190 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_intermediate_values.py
--rw-r--r--   0 mamu       (501) staff       (20)     1253 2023-04-07 07:49:39.000000 optuna-3.1.1/optuna/visualization/matplotlib/_matplotlib_imports.py
--rw-r--r--   0 mamu       (501) staff       (20)     4823 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_optimization_history.py
--rw-r--r--   0 mamu       (501) staff       (20)     5326 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_parallel_coordinate.py
--rw-r--r--   0 mamu       (501) staff       (20)     4428 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_param_importances.py
--rw-r--r--   0 mamu       (501) staff       (20)     8610 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_pareto_front.py
--rw-r--r--   0 mamu       (501) staff       (20)     5499 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_slice.py
--rw-r--r--   0 mamu       (501) staff       (20)     1827 2023-04-07 07:49:53.000000 optuna-3.1.1/optuna/visualization/matplotlib/_utils.py
-drwxr-xr-x   0 mamu       (501) staff       (20)        0 2023-04-07 07:55:15.263112 optuna-3.1.1/optuna.egg-info/
--rw-r--r--   0 mamu       (501) staff       (20)    11331 2023-04-07 07:55:15.000000 optuna-3.1.1/optuna.egg-info/PKG-INFO
--rw-r--r--   0 mamu       (501) staff       (20)     6663 2023-04-07 07:55:15.000000 optuna-3.1.1/optuna.egg-info/SOURCES.txt
--rw-r--r--   0 mamu       (501) staff       (20)        1 2023-04-07 07:55:15.000000 optuna-3.1.1/optuna.egg-info/dependency_links.txt
--rw-r--r--   0 mamu       (501) staff       (20)       44 2023-04-07 07:55:15.000000 optuna-3.1.1/optuna.egg-info/entry_points.txt
--rw-r--r--   0 mamu       (501) staff       (20)     1101 2023-04-07 07:55:15.000000 optuna-3.1.1/optuna.egg-info/requires.txt
--rw-r--r--   0 mamu       (501) staff       (20)        7 2023-04-07 07:55:15.000000 optuna-3.1.1/optuna.egg-info/top_level.txt
--rw-r--r--   0 mamu       (501) staff       (20)      814 2023-04-07 07:49:53.000000 optuna-3.1.1/pyproject.toml
--rw-r--r--   0 mamu       (501) staff       (20)      531 2023-04-07 07:55:15.304894 optuna-3.1.1/setup.cfg
--rw-r--r--   0 mamu       (501) staff       (20)     5994 2023-04-07 07:49:53.000000 optuna-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.305794 optuna-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-30 06:00:03.000000 optuna-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 06:00:03.000000 optuna-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-05-30 06:00:24.305794 optuna-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-30 06:00:03.000000 optuna-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_convert_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/_hypervolume/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/hssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/wfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36886 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28140 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/importance/_fanova/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/_fanova.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_mean_decrease_impurity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/integration/_lightgbm_tuner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43823 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/integration/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27848 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/catboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/chainermn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/cma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/fastaiv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/fastaiv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/mxnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/pytorch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/pytorch_ignite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/shap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31393 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/skopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/skorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/tfkeras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/multi_objective/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_motpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17554 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/multi_objective/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/visualization/_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/pruners/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_successive_halving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31522 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26431 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_nsgaiii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_partial_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_qmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/samplers/_search_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_search_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_search_space/intersection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/samplers/_tpe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/_erf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/_truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/multi_objective_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/parzen_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/probability_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34490 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/samplers/nsgaii/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_blxalpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_sbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_spx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_undx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_vsbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22070 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/search_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/search_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/search_space/group_decomposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/search_space/intersection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_cached_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_in_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/_journal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25886 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/_rdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/_rdb/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.2.0.a_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48100 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/study/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_study_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_study_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_tell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55112 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/terminator/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/erroreval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/terminator/improvement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/terminator/improvement/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/gp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/gp/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/terminator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.301794 optuna-3.2.0/optuna/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/pruners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/tempfile_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.301794 optuna-3.2.0/optuna/trial/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29610 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.301794 optuna-3.2.0/optuna/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_param_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_plotly_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_terminator_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.305794 optuna-3.2.0/optuna/visualization/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_matplotlib_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_param_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_terminator_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-30 06:00:03.000000 optuna-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 06:00:24.305794 optuna-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.305794 optuna-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55669 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_convert_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_transform.py
```

### Comparing `optuna-3.1.1/LICENSE` & `optuna-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/README.md` & `optuna-3.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Optuna: A hyperparameter optimization framework
 
 [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/optuna.svg)](https://pypi.python.org/pypi/optuna)
 [![conda](https://img.shields.io/conda/vn/conda-forge/optuna.svg)](https://anaconda.org/conda-forge/optuna)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/optuna/optuna)
 [![Read the Docs](https://readthedocs.org/projects/optuna/badge/?version=stable)](https://optuna.readthedocs.io/en/stable/)
-[![Codecov](https://codecov.io/gh/optuna/optuna/branch/master/graph/badge.svg)](https://codecov.io/gh/optuna/optuna/branch/master)
+[![Codecov](https://codecov.io/gh/optuna/optuna/branch/master/graph/badge.svg)](https://codecov.io/gh/optuna/optuna)
 
 [**Website**](https://optuna.org/)
 | [**Docs**](https://optuna.readthedocs.io/en/stable/)
 | [**Install Guide**](https://optuna.readthedocs.io/en/stable/installation.html)
 | [**Tutorial**](https://optuna.readthedocs.io/en/stable/tutorial/index.html)
 | [**Examples**](https://github.com/optuna/optuna-examples)
 
@@ -81,15 +81,15 @@
 
 ## Examples
 
 Examples can be found in [optuna/optuna-examples](https://github.com/optuna/optuna-examples).
 
 ## Integrations
 
-[Integrations modules](https://optuna.readthedocs.io/en/stable/tutorial/10_key_features/003_efficient_optimization_algorithms.html#integration-modules-for-pruning), which allow pruning, or early stopping, of unpromising trials are available for the following libraries:
+[Integrations modules](https://optuna-integration.readthedocs.io/en/stable/index.html), which allow pruning, or early stopping, of unpromising trials are available for the following libraries:
 
 * [AllenNLP](https://github.com/optuna/optuna-examples/tree/main/allennlp)
 * [Catalyst](https://github.com/optuna/optuna-examples/tree/main/pytorch/catalyst_simple.py)
 * [Catboost](https://github.com/optuna/optuna-examples/tree/main/catboost/catboost_pruning.py)
 * [Chainer](https://github.com/optuna/optuna-examples/tree/main/chainer/chainer_integration.py)
 * FastAI ([V1](https://github.com/optuna/optuna-examples/tree/main/fastai/fastaiv1_simple.py), [V2](https://github.com/optuna/optuna-examples/tree/main/fastai/fastaiv2_simple.py))
 * [Keras](https://github.com/optuna/optuna-examples/tree/main/keras/keras_integration.py)
```

### Comparing `optuna-3.1.1/optuna/__init__.py` & `optuna-3.2.0/optuna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from optuna import distributions
 from optuna import exceptions
 from optuna import integration
 from optuna import logging
 from optuna import multi_objective
 from optuna import pruners
 from optuna import samplers
+from optuna import search_space
 from optuna import storages
 from optuna import study
 from optuna import trial
 from optuna import version
 from optuna._imports import _LazyImport
 from optuna.exceptions import TrialPruned
 from optuna.study import copy_study
@@ -37,14 +38,15 @@
     "importance",
     "integration",
     "load_study",
     "logging",
     "multi_objective",
     "pruners",
     "samplers",
+    "search_space",
     "storages",
     "study",
     "trial",
     "version",
     "visualization",
 ]
```

### Comparing `optuna-3.1.1/optuna/_callbacks.py` & `optuna-3.2.0/optuna/_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from typing import Any
 from typing import Container
+from typing import Dict
 from typing import List
 from typing import Optional
 
 import optuna
 from optuna._experimental import experimental_class
 from optuna._experimental import experimental_func
 from optuna.trial import FrozenTrial
@@ -111,18 +113,22 @@
     def __init__(
         self, max_retry: Optional[int] = None, inherit_intermediate_values: bool = False
     ) -> None:
         self._max_retry = max_retry
         self._inherit_intermediate_values = inherit_intermediate_values
 
     def __call__(self, study: "optuna.study.Study", trial: FrozenTrial) -> None:
-        system_attrs = {"failed_trial": trial.number, "retry_history": [], **trial.system_attrs}
-        system_attrs["retry_history"].append(trial.number)  # type: ignore
+        system_attrs: Dict[str, Any] = {
+            "failed_trial": trial.number,
+            "retry_history": [],
+            **trial.system_attrs,
+        }
+        system_attrs["retry_history"].append(trial.number)
         if self._max_retry is not None:
-            if self._max_retry < len(system_attrs["retry_history"]):  # type: ignore
+            if self._max_retry < len(system_attrs["retry_history"]):
                 return
 
         study.add_trial(
             optuna.create_trial(
                 state=optuna.trial.TrialState.WAITING,
                 params=trial.params,
                 distributions=trial.distributions,
```

### Comparing `optuna-3.1.1/optuna/_convert_positional_args.py` & `optuna-3.2.0/optuna/_convert_positional_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,23 +24,21 @@
 
     Args:
         previous_positional_arg_names: List of names previously given as positional arguments.
         warning_stacklevel: Level of the stack trace where decorated function locates.
     """
 
     def converter_decorator(func: "Callable[_P, _T]") -> "Callable[_P, _T]":
-
         assert set(previous_positional_arg_names).issubset(set(signature(func).parameters)), (
             f"{set(previous_positional_arg_names)} is not a subset of"
             f" {set(signature(func).parameters)}"
         )
 
         @wraps(func)
         def converter_wrapper(*args: Any, **kwargs: Any) -> "_T":
-
             if len(args) >= 1:
                 warnings.warn(
                     f"{func.__name__}(): Please give all values as keyword arguments."
                     " See https://github.com/optuna/optuna/issues/3324 for details.",
                     FutureWarning,
                     stacklevel=warning_stacklevel,
                 )
```

### Comparing `optuna-3.1.1/optuna/_deprecated.py` & `optuna-3.2.0/optuna/_deprecated.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/_experimental.py` & `optuna-3.2.0/optuna/_experimental.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 .. note::
     Added in v{ver} as an experimental feature. The interface may change in newer versions
     without prior notice. See https://github.com/optuna/optuna/releases/tag/v{ver}.
 """
 
 
 def _validate_version(version: str) -> None:
-
     if not isinstance(version, str) or len(version.split(".")) != 3:
         raise ValueError(
             "Invalid version specification. Must follow `x.y.z` format but `{}` is given".format(
                 version
             )
         )
```

### Comparing `optuna-3.1.1/optuna/_hypervolume/base.py` & `optuna-3.2.0/optuna/_hypervolume/base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/_hypervolume/hssp.py` & `optuna-3.2.0/optuna/_hypervolume/hssp.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     For further information about algorithms to solve HSSP, please refer to the following
     paper:
 
     - `Greedy Hypervolume Subset Selection in Low Dimensions
        <https://ieeexplore.ieee.org/document/7570501>`_
     """
-    selected_vecs = []  # type: List[np.ndarray]
-    selected_indices = []  # type: List[int]
+    selected_vecs: List[np.ndarray] = []
+    selected_indices: List[int] = []
     contributions = [
         optuna._hypervolume.WFG().compute(np.asarray([v]), reference_point)
         for v in rank_i_loss_vals
     ]
     hv_selected = 0.0
     while len(selected_indices) < subset_size:
         max_index = int(np.argmax(contributions))
```

### Comparing `optuna-3.1.1/optuna/_hypervolume/utils.py` & `optuna-3.2.0/optuna/_hypervolume/utils.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/_hypervolume/wfg.py` & `optuna-3.2.0/optuna/_hypervolume/wfg.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/_imports.py` & `optuna-3.2.0/optuna/_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/_transform.py` & `optuna-3.2.0/optuna/_transform.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/cli.py` & `optuna-3.2.0/optuna/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 _dataframe = _LazyImport("optuna.study._dataframe")
 
 _DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def _check_storage_url(storage_url: Optional[str]) -> str:
-
     if storage_url is not None:
         return storage_url
 
     env_storage = os.environ.get("OPTUNA_STORAGE")
     if env_storage is not None:
         warnings.warn(
             "Specifying the storage url via 'OPTUNA_STORAGE' environment variable"
@@ -382,15 +381,14 @@
             "--flatten",
             default=False,
             action="store_true",
             help="Flatten nested columns such as directions.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         storage_url = _check_storage_url(parsed_args.storage)
         summaries = optuna.get_all_study_summaries(storage_url, include_best_trial=False)
 
         records = []
         for s in summaries:
             start = (
                 s.datetime_start.strftime(_DATETIME_FORMAT)
@@ -437,15 +435,14 @@
             "--flatten",
             default=False,
             action="store_true",
             help="Flatten nested columns such as params and user_attrs.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         warnings.warn(
             "'trials' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
         storage_url = _check_storage_url(parsed_args.storage)
         study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
@@ -488,15 +485,14 @@
             "--flatten",
             default=False,
             action="store_true",
             help="Flatten nested columns such as params and user_attrs.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         warnings.warn(
             "'best-trial' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
         storage_url = _check_storage_url(parsed_args.storage)
         study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
@@ -542,15 +538,14 @@
             "--flatten",
             default=False,
             action="store_true",
             help="Flatten nested columns such as params and user_attrs.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         warnings.warn(
             "'best-trials' is an experimental CLI command. The interface can change in the "
             "future.",
             ExperimentalWarning,
         )
 
         storage_url = _check_storage_url(parsed_args.storage)
@@ -608,15 +603,14 @@
         )
         parser.add_argument(
             "method",
             help="The method name of the objective function.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         message = (
             "The use of the `study optimize` command is deprecated. Please execute your Python "
             "script directly instead."
         )
         warnings.warn(message, FutureWarning)
 
         storage_url = _check_storage_url(parsed_args.storage)
@@ -661,15 +655,14 @@
         return 0
 
 
 class _StorageUpgrade(_BaseCommand):
     """Upgrade the schema of a storage."""
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         storage_url = _check_storage_url(parsed_args.storage)
         if storage_url.startswith("redis"):
             self.logger.info("This storage does not support upgrade yet.")
             return 1
         storage = RDBStorage(storage_url, skip_compatibility_check=True, skip_table_creation=True)
         current_version = storage.get_current_version()
         head_version = storage.get_head_version()
@@ -739,15 +732,14 @@
             "--flatten",
             default=False,
             action="store_true",
             help="Flatten nested columns such as params.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         warnings.warn(
             "'ask' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
         storage_url = _check_storage_url(parsed_args.storage)
 
@@ -858,15 +850,14 @@
             default=False,
             action="store_true",
             help="If specified, tell is skipped without any error when the trial is already "
             "finished.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-
         warnings.warn(
             "'tell' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
         storage_url = _check_storage_url(parsed_args.storage)
```

### Comparing `optuna-3.1.1/optuna/distributions.py` & `optuna-3.2.0/optuna/distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,31 +81,27 @@
             :obj:`True` if the parameter value is contained in the range of this distribution,
             otherwise :obj:`False`.
         """
 
         raise NotImplementedError
 
     def _asdict(self) -> Dict:
-
         return self.__dict__
 
     def __eq__(self, other: Any) -> bool:
-
         if not isinstance(other, BaseDistribution):
             return NotImplemented
         if not type(self) is type(other):
             return False
         return self.__dict__ == other.__dict__
 
     def __hash__(self) -> int:
-
         return hash((self.__class__,) + tuple(sorted(self.__dict__.items())))
 
     def __repr__(self) -> str:
-
         kwargs = ", ".join("{}={}".format(k, v) for k, v in sorted(self._asdict().items()))
         return "{}({})".format(self.__class__.__name__, kwargs)
 
 
 class FloatDistribution(BaseDistribution):
     """A distribution on floats.
 
@@ -135,15 +131,14 @@
             This parameter must be :obj:`None` when the parameter ``log`` is :obj:`True`.
 
     """
 
     def __init__(
         self, low: float, high: float, log: bool = False, step: Union[None, float] = None
     ) -> None:
-
         if log and step is not None:
             raise ValueError("The parameter `step` is not supported when `log` is true.")
 
         if low > high:
             raise ValueError(
                 "The `low` value must be smaller than or equal to the `high` value "
                 "(low={}, high={}).".format(low, high)
@@ -166,27 +161,25 @@
             self.step = float(step)
 
         self.low = float(low)
         self.high = float(high)
         self.log = log
 
     def single(self) -> bool:
-
         if self.step is None:
             return self.low == self.high
         else:
             if self.low == self.high:
                 return True
             high = decimal.Decimal(str(self.high))
             low = decimal.Decimal(str(self.low))
             step = decimal.Decimal(str(self.step))
             return (high - low) < step
 
     def _contains(self, param_value_in_internal_repr: float) -> bool:
-
         value = param_value_in_internal_repr
         if self.step is None:
             return self.low <= value <= self.high
         else:
             k = (value - self.low) / self.step
             return self.low <= value <= self.high and abs(k - round(k)) < 1.0e-8
 
@@ -345,15 +338,14 @@
         step:
             A discretization step. ``step`` must be a positive integer. This parameter must be 1
             when the parameter ``log`` is :obj:`True`.
 
     """
 
     def __init__(self, low: int, high: int, log: bool = False, step: int = 1) -> None:
-
         if log and step != 1:
             raise ValueError(
                 "Samplers and other components in Optuna only accept step is 1 "
                 "when `log` argument is True."
             )
 
         if low > high:
@@ -376,15 +368,14 @@
         self.log = log
         self.step = int(step)
         self.low = int(low)
         high = int(high)
         self.high = _adjust_int_uniform_high(self.low, high, self.step)
 
     def to_external_repr(self, param_value_in_internal_repr: float) -> int:
-
         return int(param_value_in_internal_repr)
 
     def to_internal_repr(self, param_value_in_external_repr: int) -> float:
         try:
             internal_repr = float(param_value_in_external_repr)
         except (ValueError, TypeError) as e:
             raise ValueError(
@@ -405,15 +396,14 @@
             return self.low == self.high
 
         if self.low == self.high:
             return True
         return (self.high - self.low) < self.step
 
     def _contains(self, param_value_in_internal_repr: float) -> bool:
-
         value = param_value_in_internal_repr
         return self.low <= value <= self.high and (value - self.low) % self.step == 0
 
 
 @deprecated_class("3.0.0", "6.0.0", text=_int_distribution_deprecated_msg)
 class IntUniformDistribution(IntDistribution):
     """A uniform distribution on integers.
@@ -518,51 +508,45 @@
     Attributes:
         choices:
             Parameter value candidates.
 
     """
 
     def __init__(self, choices: Sequence[CategoricalChoiceType]) -> None:
-
         if len(choices) == 0:
             raise ValueError("The `choices` must contain one or more elements.")
         for choice in choices:
             if choice is not None and not isinstance(choice, (bool, int, float, str)):
                 message = (
                     "Choices for a categorical distribution should be a tuple of None, bool, "
                     "int, float and str for persistent storage but contains {} which is of type "
                     "{}.".format(choice, type(choice).__name__)
                 )
                 warnings.warn(message)
 
         self.choices = tuple(choices)
 
     def to_external_repr(self, param_value_in_internal_repr: float) -> CategoricalChoiceType:
-
         return self.choices[int(param_value_in_internal_repr)]
 
     def to_internal_repr(self, param_value_in_external_repr: CategoricalChoiceType) -> float:
-
         for index, choice in enumerate(self.choices):
             if _categorical_choice_equal(param_value_in_external_repr, choice):
                 return index
 
         raise ValueError(f"'{param_value_in_external_repr}' not in {self.choices}.")
 
     def single(self) -> bool:
-
         return len(self.choices) == 1
 
     def _contains(self, param_value_in_internal_repr: float) -> bool:
-
         index = int(param_value_in_internal_repr)
         return 0 <= index < len(self.choices)
 
     def __eq__(self, other: Any) -> bool:
-
         if not isinstance(other, BaseDistribution):
             return NotImplemented
         if not isinstance(other, self.__class__):
             return False
         if self.__dict__.keys() != other.__dict__.keys():
             return False
         for key, value in self.__dict__.items():
@@ -719,15 +703,14 @@
                 low=low, old_high=old_high, high=high, step=step
             )
         )
     return high
 
 
 def _get_single_value(distribution: BaseDistribution) -> Union[int, float, CategoricalChoiceType]:
-
     assert distribution.single()
 
     if isinstance(
         distribution,
         (
             FloatDistribution,
             IntDistribution,
@@ -741,15 +724,14 @@
 
 # TODO(himkt): Remove this method with the deletion of deprecated distributions.
 # https://github.com/optuna/optuna/issues/2941
 def _convert_old_distribution_to_new_distribution(
     distribution: BaseDistribution,
     suppress_warning: bool = False,
 ) -> BaseDistribution:
-
     new_distribution: BaseDistribution
 
     # Float distributions.
     if isinstance(distribution, UniformDistribution):
         new_distribution = FloatDistribution(
             low=distribution.low,
             high=distribution.high,
@@ -795,7 +777,14 @@
         message = (
             f"{distribution} is deprecated and internally converted to"
             f" {new_distribution}. See https://github.com/optuna/optuna/issues/2941."
         )
         warnings.warn(message, FutureWarning)
 
     return new_distribution
+
+
+def _is_distribution_log(distribution: BaseDistribution) -> bool:
+    if isinstance(distribution, (FloatDistribution, IntDistribution)):
+        return distribution.log
+
+    return False
```

### Comparing `optuna-3.1.1/optuna/exceptions.py` & `optuna-3.2.0/optuna/exceptions.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/importance/__init__.py` & `optuna-3.2.0/optuna/importance/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/importance/_base.py` & `optuna-3.2.0/optuna/importance/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 from typing import Union
 
 import numpy
 
 from optuna._transform import _SearchSpaceTransform
 from optuna.distributions import BaseDistribution
-from optuna.samplers import intersection_search_space
+from optuna.search_space import intersection_search_space
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 class BaseImportanceEvaluator(abc.ABC):
     """Abstract parameter importance evaluator."""
@@ -68,15 +68,15 @@
 
 
 def _get_distributions(study: Study, params: Optional[List[str]]) -> Dict[str, BaseDistribution]:
     completed_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
     _check_evaluate_args(completed_trials, params)
 
     if params is None:
-        return intersection_search_space(study, ordered_dict=True)
+        return intersection_search_space(study.get_trials(deepcopy=False), ordered_dict=True)
 
     # New temporary required to pass mypy. Seems like a bug.
     params_not_none = params
     assert params_not_none is not None
 
     # Compute the search space based on the subset of trials containing all parameters.
     distributions = None
```

### Comparing `optuna-3.1.1/optuna/importance/_fanova/_evaluator.py` & `optuna-3.2.0/optuna/importance/_fanova/_evaluator.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/importance/_fanova/_fanova.py` & `optuna-3.2.0/optuna/importance/_fanova/_fanova.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/importance/_fanova/_tree.py` & `optuna-3.2.0/optuna/importance/_fanova/_tree.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/importance/_mean_decrease_impurity.py` & `optuna-3.2.0/optuna/importance/_mean_decrease_impurity.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
     This evaluator fits fits a random forest regression model that predicts the objective values
     of :class:`~optuna.trial.TrialState.COMPLETE` trials given their parameter configurations.
     Feature importances are then computed using MDI.
 
     .. note::
 
-        This evaluator requires the `sklean <https://scikit-learn.org/stable/>`_ Python package and
-        is based on `sklearn.ensemble.RandomForestClassifier.feature_importances_
+        This evaluator requires the `sklearn <https://scikit-learn.org/stable/>`_ Python package
+        and is based on `sklearn.ensemble.RandomForestClassifier.feature_importances_
         <https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html#sklearn.ensemble.RandomForestClassifier.feature_importances_>`_.
 
     Args:
         n_trees:
             Number of trees in the random forest.
         max_depth:
             The maximum depth of each tree in the random forest.
```

### Comparing `optuna-3.1.1/optuna/integration/__init__.py` & `optuna-3.2.0/optuna/integration/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,31 +83,38 @@
         _modules = set(_import_structure.keys())
         _class_to_module = {}
         for key, values in _import_structure.items():
             for value in values:
                 _class_to_module[value] = key
 
         def __getattr__(self, name: str) -> Any:
-
             if name in self._modules:
                 value = self._get_module(name)
             elif name in self._class_to_module.keys():
                 module = self._get_module(self._class_to_module[name])
                 value = getattr(module, name)
             else:
                 raise AttributeError("module {} has no attribute {}".format(self.__name__, name))
 
             setattr(self, name, value)
             return value
 
         def _get_module(self, module_name: str) -> ModuleType:
-
             import importlib
 
-            return importlib.import_module("." + module_name, self.__name__)
+            try:
+                return importlib.import_module("." + module_name, self.__name__)
+            except ModuleNotFoundError:
+                raise ModuleNotFoundError(
+                    "Optuna's integration modules for third-party libraries have started "
+                    "migrating from Optuna itself to a package called `optuna-integration`. "
+                    "The module you are trying to use has already been migrated to "
+                    "`optuna-integration`. Please install the package by running "
+                    "`pip install optuna-integration`."
+                )
 
     sys.modules[__name__] = _IntegrationModule(__name__)
 
 __all__ = [
     "AllenNLPExecutor",
     "AllenNLPPruningCallback",
     "BoTorchSampler",
```

### Comparing `optuna-3.1.1/optuna/integration/_lightgbm_tuner/__init__.py` & `optuna-3.2.0/optuna/integration/_lightgbm_tuner/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/integration/_lightgbm_tuner/alias.py` & `optuna-3.2.0/optuna/integration/_lightgbm_tuner/alias.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/integration/_lightgbm_tuner/optimize.py` & `optuna-3.2.0/optuna/integration/_lightgbm_tuner/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
 class _BaseTuner:
     def __init__(
         self,
         lgbm_params: Optional[Dict[str, Any]] = None,
         lgbm_kwargs: Optional[Dict[str, Any]] = None,
     ) -> None:
-
         # Handling alias metrics.
         if lgbm_params is not None:
             _handling_alias_metrics(lgbm_params)
 
         self.lgbm_params = lgbm_params or {}
         self.lgbm_kwargs = lgbm_kwargs or {}
 
@@ -88,15 +87,14 @@
         else:
             raise NotImplementedError
         metric = self._metric_with_eval_at(metric)
 
         return metric
 
     def _get_booster_best_score(self, booster: "lgb.Booster") -> float:
-
         metric = self._get_metric_for_objective()
         valid_sets: Optional[VALID_SET_TYPE] = self.lgbm_kwargs.get("valid_sets")
 
         if self.lgbm_kwargs.get("valid_names") is not None:
             if type(self.lgbm_kwargs["valid_names"]) is str:
                 valid_name = self.lgbm_kwargs["valid_names"]
             elif type(self.lgbm_kwargs["valid_names"]) in [list, tuple]:
@@ -114,15 +112,14 @@
         else:
             raise NotImplementedError
 
         val_score = booster.best_score[valid_name][metric]
         return val_score
 
     def _metric_with_eval_at(self, metric: str) -> str:
-
         if metric != "ndcg" and metric != "map":
             return metric
 
         eval_at = self.lgbm_params.get("eval_at")
         if eval_at is None:
             eval_at = self.lgbm_params.get("{}_at".format(metric))
         if eval_at is None:
@@ -139,20 +136,18 @@
             return "{}@{}".format(metric, eval_at)
         raise ValueError(
             "The value of eval_at is expected to be int or a list/tuple of int."
             "'{}' is specified.".format(eval_at)
         )
 
     def higher_is_better(self) -> bool:
-
         metric_name = self.lgbm_params.get("metric", "binary_logloss")
         return metric_name in ("auc", "auc_mu", "ndcg", "map", "average_precision")
 
     def compare_validation_metrics(self, val_score: float, best_score: float) -> bool:
-
         if self.higher_is_better():
             return val_score > best_score
         else:
             return val_score < best_score
 
 
 class _OptunaObjective(_BaseTuner):
@@ -165,15 +160,14 @@
         train_set: "lgb.Dataset",
         lgbm_kwargs: Dict[str, Any],
         best_score: float,
         step_name: str,
         model_dir: Optional[str],
         pbar: Optional[tqdm.tqdm] = None,
     ):
-
         self.target_param_names = target_param_names
         self.pbar = pbar
         self.lgbm_params = lgbm_params
         self.lgbm_kwargs = lgbm_kwargs
         self.train_set = train_set
 
         self.trial_count = 0
@@ -182,15 +176,14 @@
         self.step_name = step_name
         self.model_dir = model_dir
 
         self._check_target_names_supported()
         self.pbar_fmt = "{}, val_score: {:.6f}"
 
     def _check_target_names_supported(self) -> None:
-
         supported_param_names = [
             "lambda_l1",
             "lambda_l2",
             "num_leaves",
             "feature_fraction",
             "bagging_fraction",
             "bagging_freq",
@@ -234,15 +227,14 @@
         if isinstance(valid_sets, list):
             return [copy.copy(d) for d in valid_sets]
         if isinstance(valid_sets, tuple):
             return tuple([copy.copy(d) for d in valid_sets])
         return copy.copy(valid_sets)
 
     def __call__(self, trial: optuna.trial.Trial) -> float:
-
         self._preprocess(trial)
 
         start_time = time.time()
         train_set = copy.copy(self.train_set)
         kwargs = copy.copy(self.lgbm_kwargs)
         kwargs["valid_sets"] = self._copy_valid_sets(kwargs["valid_sets"])
         booster = lgb.train(self.lgbm_params, train_set, **kwargs)
@@ -292,34 +284,31 @@
         train_set: "lgb.Dataset",
         lgbm_kwargs: Dict[str, Any],
         best_score: float,
         step_name: str,
         model_dir: Optional[str],
         pbar: Optional[tqdm.tqdm] = None,
     ):
-
         super().__init__(
             target_param_names,
             lgbm_params,
             train_set,
             lgbm_kwargs,
             best_score,
             step_name,
             model_dir,
             pbar=pbar,
         )
 
     def _get_cv_scores(self, cv_results: Dict[str, List[float]]) -> List[float]:
-
         metric = self._get_metric_for_objective()
         val_scores = cv_results["{}-mean".format(metric)]
         return val_scores
 
     def __call__(self, trial: optuna.trial.Trial) -> float:
-
         self._preprocess(trial)
 
         start_time = time.time()
         train_set = copy.copy(self.train_set)
         cv_results = lgb.cv(self.lgbm_params, train_set, **self.lgbm_kwargs)
 
         val_scores = self._get_cv_scores(cv_results)
@@ -372,15 +361,14 @@
         optuna_callbacks: Optional[List[Callable[[Study, FrozenTrial], None]]] = None,
         verbosity: Optional[int] = None,
         show_progress_bar: bool = True,
         model_dir: Optional[str] = None,
         *,
         optuna_seed: Optional[int] = None,
     ) -> None:
-
         _imports.check()
 
         params = copy.deepcopy(params)
 
         # Handling alias metrics.
         _handling_alias_metrics(params)
 
@@ -507,15 +495,14 @@
 
         with open(path, "rb") as fin:
             booster = pickle.load(fin)
 
         return booster
 
     def _parse_args(self, *args: Any, **kwargs: Any) -> None:
-
         self.auto_options = {
             option_name: kwargs.get(option_name)
             for option_name in ["time_budget", "sample_size", "verbosity", "show_progress_bar"]
         }
 
         # Split options.
         for option_name in self.auto_options.keys():
@@ -675,40 +662,36 @@
     def _create_objective(
         self,
         target_param_names: List[str],
         train_set: "lgb.Dataset",
         step_name: str,
         pbar: Optional[tqdm.tqdm],
     ) -> _OptunaObjective:
-
         raise NotImplementedError
 
     def _create_stepwise_study(
         self, study: "optuna.study.Study", step_name: str
     ) -> "optuna.study.Study":
-
         # This class is assumed to be passed to a sampler and a pruner corresponding to the step.
         class _StepwiseStudy(optuna.study.Study):
             def __init__(self, study: optuna.study.Study, step_name: str) -> None:
-
                 super().__init__(
                     study_name=study.study_name,
                     storage=study._storage,
                     sampler=study.sampler,
                     pruner=study.pruner,
                 )
                 self._step_name = step_name
 
             def get_trials(
                 self,
                 deepcopy: bool = True,
                 states: Optional[Container[TrialState]] = None,
             ) -> List[optuna.trial.FrozenTrial]:
-
-                trials = super().get_trials(deepcopy=deepcopy, states=states)
+                trials = super()._get_trials(deepcopy=deepcopy, states=states)
                 return [t for t in trials if t.system_attrs.get(_STEP_NAME_KEY) == self._step_name]
 
             @property
             def best_trial(self) -> optuna.trial.FrozenTrial:
                 """Return the best trial in the study.
 
                 Returns:
@@ -827,15 +810,14 @@
         optuna_callbacks: Optional[List[Callable[[Study, FrozenTrial], None]]] = None,
         model_dir: Optional[str] = None,
         verbosity: Optional[int] = None,
         show_progress_bar: bool = True,
         *,
         optuna_seed: Optional[int] = None,
     ) -> None:
-
         super().__init__(
             params,
             train_set,
             num_boost_round=num_boost_round,
             fobj=fobj,
             feval=feval,
             feature_name=feature_name,
@@ -994,15 +976,14 @@
         verbosity: Optional[int] = None,
         show_progress_bar: bool = True,
         model_dir: Optional[str] = None,
         return_cvbooster: bool = False,
         *,
         optuna_seed: Optional[int] = None,
     ) -> None:
-
         super().__init__(
             params,
             train_set,
             num_boost_round,
             fobj=fobj,
             feval=feval,
             feature_name=feature_name,
```

### Comparing `optuna-3.1.1/optuna/integration/_lightgbm_tuner/sklearn.py` & `optuna-3.2.0/optuna/integration/_lightgbm_tuner/sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,43 +7,40 @@
 class LGBMModel(lgb.LGBMModel):
     """Proxy of lightgbm.LGBMModel.
 
     See: `pydoc lightgbm.LGBMModel`
     """
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-
         warnings.warn(
             "LightGBMTuner doesn't support sklearn API. "
             "Use `train()` or `LightGBMTuner` for hyperparameter tuning."
         )
         super().__init__(*args, **kwargs)
 
 
 class LGBMClassifier(lgb.LGBMClassifier):
     """Proxy of lightgbm.LGBMClassifier.
 
     See: `pydoc lightgbm.LGBMClassifier`
     """
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-
         warnings.warn(
             "LightGBMTuner doesn't support sklearn API. "
             "Use `train()` or `LightGBMTuner` for hyperparameter tuning."
         )
         super().__init__(*args, **kwargs)
 
 
 class LGBMRegressor(lgb.LGBMRegressor):
     """Proxy of LGBMRegressor.
 
     See: `pydoc lightgbm.LGBMRegressor`
     """
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-
         warnings.warn(
             "LightGBMTuner doesn't support sklearn API. "
             "Use `train()` or `LightGBMTuner` for hyperparameter tuning."
         )
         super().__init__(*args, **kwargs)
```

### Comparing `optuna-3.1.1/optuna/integration/botorch.py` & `optuna-3.2.0/optuna/integration/botorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from typing import Dict
 from typing import Optional
 from typing import Sequence
 from typing import Union
 import warnings
 
 import numpy
+from packaging import version
 
 from optuna import logging
 from optuna._experimental import experimental_class
 from optuna._experimental import experimental_func
 from optuna._imports import try_import
 from optuna._transform import _SearchSpaceTransform
 from optuna.distributions import BaseDistribution
 from optuna.samplers import BaseSampler
-from optuna.samplers import IntersectionSearchSpace
 from optuna.samplers import RandomSampler
 from optuna.samplers._base import _CONSTRAINTS_KEY
 from optuna.samplers._base import _process_constraints_after_trial
+from optuna.search_space import IntersectionSearchSpace
 from optuna.study import Study
 from optuna.study import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 with try_import() as _imports:
@@ -34,15 +35,15 @@
     from botorch.acquisition.objective import GenericMCObjective
     from botorch.models import SingleTaskGP
     from botorch.models.transforms.outcome import Standardize
     from botorch.optim import optimize_acqf
     from botorch.sampling import SobolQMCNormalSampler
     import botorch.version
 
-    if botorch.version.version_tuple < (0, 8, 0):
+    if version.parse(botorch.version.version) < version.parse("0.8.0"):
         from botorch.fit import fit_gpytorch_model as fit_gpytorch_mll
 
         def _get_sobol_qmc_normal_sampler(num_samples: int) -> SobolQMCNormalSampler:
             return SobolQMCNormalSampler(num_samples)
 
     else:
         from botorch.fit import fit_gpytorch_mll
@@ -65,14 +66,15 @@
 
 @experimental_func("2.4.0")
 def qei_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
+    pending_x: Optional["torch.Tensor"],
 ) -> "torch.Tensor":
     """Quasi MC-based batch Expected Improvement (qEI).
 
     The default value of ``candidates_func`` in :class:`~optuna.integration.BoTorchSampler`
     with single-objective optimization.
 
     Args:
@@ -92,15 +94,19 @@
             ``n_trials`` is identical to that of ``train_x``. ``n_constraints`` is the number of
             constraints. A constraint is violated if strictly larger than 0. If no constraints are
             involved in the optimization, this argument will be :obj:`None`.
         bounds:
             Search space bounds. A ``torch.Tensor`` of shape ``(2, n_params)``. ``n_params`` is
             identical to that of ``train_x``. The first and the second rows correspond to the
             lower and upper bounds for each parameter respectively.
-
+        pending_x:
+            Pending parameter configurations. A ``torch.Tensor`` of shape
+            ``(n_pending, n_params)``. ``n_pending`` is the number of the trials which are already
+            suggested all their parameters but have not completed their evaluation, and
+            ``n_params`` is identical to that of ``train_x``.
     Returns:
         Next set of candidates. Usually the return value of BoTorch's ``optimize_acqf``.
 
     """
 
     if train_obj.size(-1) != 1:
         raise ValueError("Objective may only contain single values with qEI.")
@@ -130,24 +136,27 @@
         train_y = train_obj
 
         best_f = train_obj.max()
 
         objective = None  # Using the default identity objective.
 
     train_x = normalize(train_x, bounds=bounds)
+    if pending_x is not None:
+        pending_x = normalize(pending_x, bounds=bounds)
 
     model = SingleTaskGP(train_x, train_y, outcome_transform=Standardize(m=train_y.size(-1)))
     mll = ExactMarginalLogLikelihood(model.likelihood, model)
     fit_gpytorch_mll(mll)
 
     acqf = qExpectedImprovement(
         model=model,
         best_f=best_f,
         sampler=_get_sobol_qmc_normal_sampler(256),
         objective=objective,
+        X_pending=pending_x,
     )
 
     standard_bounds = torch.zeros_like(bounds)
     standard_bounds[1] = 1
 
     candidates, _ = optimize_acqf(
         acq_function=acqf,
@@ -166,14 +175,15 @@
 
 @experimental_func("2.4.0")
 def qehvi_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
+    pending_x: Optional["torch.Tensor"],
 ) -> "torch.Tensor":
     """Quasi MC-based batch Expected Hypervolume Improvement (qEHVI).
 
     The default value of ``candidates_func`` in :class:`~optuna.integration.BoTorchSampler`
     with multi-objective optimization when the number of objectives is three or less.
 
     .. seealso::
@@ -200,14 +210,16 @@
         train_y = train_obj
 
         train_obj_feas = train_obj
 
         additional_qehvi_kwargs = {}
 
     train_x = normalize(train_x, bounds=bounds)
+    if pending_x is not None:
+        pending_x = normalize(pending_x, bounds=bounds)
 
     model = SingleTaskGP(train_x, train_y, outcome_transform=Standardize(m=train_y.shape[-1]))
     mll = ExactMarginalLogLikelihood(model.likelihood, model)
     fit_gpytorch_mll(mll)
 
     # Approximate box decomposition similar to Ax when the number of objectives is large.
     # https://github.com/facebook/Ax/blob/master/ax/models/torch/botorch_moo_defaults
@@ -223,14 +235,15 @@
     ref_point_list = ref_point.tolist()
 
     acqf = monte_carlo.qExpectedHypervolumeImprovement(
         model=model,
         ref_point=ref_point_list,
         partitioning=partitioning,
         sampler=_get_sobol_qmc_normal_sampler(256),
+        X_pending=pending_x,
         **additional_qehvi_kwargs,
     )
     standard_bounds = torch.zeros_like(bounds)
     standard_bounds[1] = 1
 
     candidates, _ = optimize_acqf(
         acq_function=acqf,
@@ -249,14 +262,15 @@
 
 @experimental_func("3.1.0")
 def qnehvi_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
+    pending_x: Optional["torch.Tensor"],
 ) -> "torch.Tensor":
     """Quasi MC-based batch Expected Noisy Hypervolume Improvement (qNEHVI).
 
     According to Botorch/Ax documentation,
     this function may perform better than qEHVI (`qehvi_candidates_func`).
     (cf. https://botorch.org/tutorials/constrained_multi_objective_bo )
 
@@ -279,14 +293,16 @@
         }
     else:
         train_y = train_obj
 
         additional_qnehvi_kwargs = {}
 
     train_x = normalize(train_x, bounds=bounds)
+    if pending_x is not None:
+        pending_x = normalize(pending_x, bounds=bounds)
 
     model = SingleTaskGP(train_x, train_y, outcome_transform=Standardize(m=train_y.shape[-1]))
     mll = ExactMarginalLogLikelihood(model.likelihood, model)
     fit_gpytorch_mll(mll)
 
     # Approximate box decomposition similar to Ax when the number of objectives is large.
     # https://github.com/facebook/Ax/blob/master/ax/models/torch/botorch_moo_defaults
@@ -304,14 +320,15 @@
     acqf = monte_carlo.qNoisyExpectedHypervolumeImprovement(
         model=model,
         ref_point=ref_point_list,
         X_baseline=train_x,
         alpha=alpha,
         prune_baseline=True,
         sampler=_get_sobol_qmc_normal_sampler(256),
+        X_pending=pending_x,
         **additional_qnehvi_kwargs,
     )
 
     standard_bounds = torch.zeros_like(bounds)
     standard_bounds[1] = 1
 
     candidates, _ = optimize_acqf(
@@ -331,14 +348,15 @@
 
 @experimental_func("2.4.0")
 def qparego_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
+    pending_x: Optional["torch.Tensor"],
 ) -> "torch.Tensor":
     """Quasi MC-based extended ParEGO (qParEGO) for constrained multi-objective optimization.
 
     The default value of ``candidates_func`` in :class:`~optuna.integration.BoTorchSampler`
     with multi-objective optimization when the number of objectives is larger than three.
 
     .. seealso::
@@ -362,24 +380,27 @@
         )
     else:
         train_y = train_obj
 
         objective = GenericMCObjective(scalarization)
 
     train_x = normalize(train_x, bounds=bounds)
+    if pending_x is not None:
+        pending_x = normalize(pending_x, bounds=bounds)
 
     model = SingleTaskGP(train_x, train_y, outcome_transform=Standardize(m=train_y.size(-1)))
     mll = ExactMarginalLogLikelihood(model.likelihood, model)
     fit_gpytorch_mll(mll)
 
     acqf = qExpectedImprovement(
         model=model,
         best_f=objective(train_y).max(),
         sampler=_get_sobol_qmc_normal_sampler(256),
         objective=objective,
+        X_pending=pending_x,
     )
 
     standard_bounds = torch.zeros_like(bounds)
     standard_bounds[1] = 1
 
     candidates, _ = optimize_acqf(
         acq_function=acqf,
@@ -400,14 +421,15 @@
     n_objectives: int,
 ) -> Callable[
     [
         "torch.Tensor",
         "torch.Tensor",
         Optional["torch.Tensor"],
         "torch.Tensor",
+        Optional["torch.Tensor"],
     ],
     "torch.Tensor",
 ]:
     if n_objectives > 3:
         return qparego_candidates_func
     elif n_objectives > 1:
         return qehvi_candidates_func
@@ -462,14 +484,21 @@
             constraint is violated. A value equal to or smaller than 0 is considered feasible.
 
             If omitted, no constraints will be passed to ``candidates_func`` nor taken into
             account during suggestion.
         n_startup_trials:
             Number of initial trials, that is the number of trials to resort to independent
             sampling.
+        consider_running_trials:
+            If True, the acquisition function takes into consideration the running parameters
+            whose evaluation has not completed. Enabling this option is considered to improve the
+            performance of parallel optimization.
+
+            .. note::
+                Added in v3.2.0 as an experimental argument.
         independent_sampler:
             An independent sampler to use for the initial trials and for parameters that are
             conditional.
         seed:
             Seed for random number generator.
         device:
             A ``torch.device`` to store input and output data of BoTorch. Please set a CUDA device
@@ -482,28 +511,31 @@
         candidates_func: Optional[
             Callable[
                 [
                     "torch.Tensor",
                     "torch.Tensor",
                     Optional["torch.Tensor"],
                     "torch.Tensor",
+                    Optional["torch.Tensor"],
                 ],
                 "torch.Tensor",
             ]
         ] = None,
         constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
         n_startup_trials: int = 10,
+        consider_running_trials: bool = True,
         independent_sampler: Optional[BaseSampler] = None,
         seed: Optional[int] = None,
         device: Optional["torch.device"] = None,
     ):
         _imports.check()
 
         self._candidates_func = candidates_func
         self._constraints_func = constraints_func
+        self._consider_running_trials = consider_running_trials
         self._independent_sampler = independent_sampler or RandomSampler(seed=seed)
         self._n_startup_trials = n_startup_trials
         self._seed = seed
 
         self._study_id: Optional[int] = None
         self._search_space = IntersectionSearchSpace()
         self._device = device or torch.device("cpu")
@@ -538,54 +570,69 @@
         search_space: Dict[str, BaseDistribution],
     ) -> Dict[str, Any]:
         assert isinstance(search_space, OrderedDict)
 
         if len(search_space) == 0:
             return {}
 
-        trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
+        completed_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
+        running_trials = [
+            t for t in study.get_trials(deepcopy=False, states=(TrialState.RUNNING,)) if t != trial
+        ]
+        trials = completed_trials + running_trials
 
         n_trials = len(trials)
+        n_completed_trials = len(completed_trials)
         if n_trials < self._n_startup_trials:
             return {}
 
         trans = _SearchSpaceTransform(search_space)
         n_objectives = len(study.directions)
         values: Union[numpy.ndarray, torch.Tensor] = numpy.empty(
             (n_trials, n_objectives), dtype=numpy.float64
         )
         params: Union[numpy.ndarray, torch.Tensor]
         con: Optional[Union[numpy.ndarray, torch.Tensor]] = None
         bounds: Union[numpy.ndarray, torch.Tensor] = trans.bounds
         params = numpy.empty((n_trials, trans.bounds.shape[0]), dtype=numpy.float64)
         for trial_idx, trial in enumerate(trials):
-            params[trial_idx] = trans.transform(trial.params)
-            assert len(study.directions) == len(trial.values)
-
-            for obj_idx, (direction, value) in enumerate(zip(study.directions, trial.values)):
-                assert value is not None
-                if direction == StudyDirection.MINIMIZE:  # BoTorch always assumes maximization.
-                    value *= -1
-                values[trial_idx, obj_idx] = value
-
-            if self._constraints_func is not None:
-                constraints = study._storage.get_trial_system_attrs(trial._trial_id).get(
-                    _CONSTRAINTS_KEY
-                )
-                if constraints is not None:
-                    n_constraints = len(constraints)
-
-                    if con is None:
-                        con = numpy.full((n_trials, n_constraints), numpy.nan, dtype=numpy.float64)
-                    elif n_constraints != con.shape[1]:
-                        raise RuntimeError(
-                            f"Expected {con.shape[1]} constraints but received {n_constraints}."
-                        )
-
-                    con[trial_idx] = constraints
+            if trial.state == TrialState.COMPLETE:
+                params[trial_idx] = trans.transform(trial.params)
+                assert len(study.directions) == len(trial.values)
+                for obj_idx, (direction, value) in enumerate(zip(study.directions, trial.values)):
+                    assert value is not None
+                    if (
+                        direction == StudyDirection.MINIMIZE
+                    ):  # BoTorch always assumes maximization.
+                        value *= -1
+                    values[trial_idx, obj_idx] = value
+                if self._constraints_func is not None:
+                    constraints = study._storage.get_trial_system_attrs(trial._trial_id).get(
+                        _CONSTRAINTS_KEY
+                    )
+                    if constraints is not None:
+                        n_constraints = len(constraints)
+
+                        if con is None:
+                            con = numpy.full(
+                                (n_completed_trials, n_constraints), numpy.nan, dtype=numpy.float64
+                            )
+                        elif n_constraints != con.shape[1]:
+                            raise RuntimeError(
+                                f"Expected {con.shape[1]} constraints "
+                                f"but received {n_constraints}."
+                            )
+                        con[trial_idx] = constraints
+            elif trial.state == TrialState.RUNNING:
+                if all(p in trial.params for p in search_space):
+                    params[trial_idx] = trans.transform(trial.params)
+                else:
+                    params[trial_idx] = numpy.nan
+            else:
+                assert False, "trail.state must be TrialState.COMPLETE or TrialState.RUNNING."
 
         if self._constraints_func is not None:
             if con is None:
                 warnings.warn(
                     "`constraints_func` was given but no call to it correctly computed "
                     "constraints. Constraints passed to `candidates_func` will be `None`."
                 )
@@ -605,19 +652,29 @@
             if con.dim() == 1:
                 con.unsqueeze_(-1)
         bounds.transpose_(0, 1)
 
         if self._candidates_func is None:
             self._candidates_func = _get_default_candidates_func(n_objectives=n_objectives)
 
+        completed_values = values[:n_completed_trials]
+        completed_params = params[:n_completed_trials]
+        if self._consider_running_trials:
+            running_params = params[n_completed_trials:]
+            running_params = running_params[~torch.isnan(running_params).any(dim=1)]
+        else:
+            running_params = None
+
         with manual_seed(self._seed):
             # `manual_seed` makes the default candidates functions reproducible.
             # `SobolQMCNormalSampler`'s constructor has a `seed` argument, but its behavior is
             # deterministic when the BoTorch's seed is fixed.
-            candidates = self._candidates_func(params, values, con, bounds)
+            candidates = self._candidates_func(
+                completed_params, completed_values, con, bounds, running_params
+            )
             if self._seed is not None:
                 self._seed += 1
 
         if not isinstance(candidates, torch.Tensor):
             raise TypeError("Candidates must be a torch.Tensor.")
         if candidates.dim() == 2:
             if candidates.size(0) != 1:
@@ -648,15 +705,15 @@
         return self._independent_sampler.sample_independent(
             study, trial, param_name, param_distribution
         )
 
     def reseed_rng(self) -> None:
         self._independent_sampler.reseed_rng()
         if self._seed is not None:
-            self._seed = numpy.random.RandomState().randint(2**60)
+            self._seed = numpy.random.RandomState().randint(numpy.iinfo(numpy.int32).max)
 
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Optional[Sequence[float]],
```

### Comparing `optuna-3.1.1/optuna/integration/catboost.py` & `optuna-3.2.0/optuna/integration/catboost.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/integration/cma.py` & `optuna-3.2.0/optuna/integration/cma.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from optuna._deprecated import deprecated_class
 from optuna._imports import try_import
 from optuna.distributions import BaseDistribution
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.samplers import BaseSampler
+from optuna.search_space import IntersectionSearchSpace
 from optuna.study import Study
 from optuna.study import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 with try_import() as _imports:
@@ -100,15 +101,15 @@
             of trials finish in the same study.
 
         independent_sampler:
             A :class:`~optuna.samplers.BaseSampler` instance that is used for independent
             sampling. The parameters not contained in the relative search space are sampled
             by this sampler.
             The search space for :class:`~optuna.integration.PyCmaSampler` is determined by
-            :func:`~optuna.samplers.intersection_search_space()`.
+            :func:`~optuna.search_space.intersection_search_space()`.
 
             If :obj:`None` is specified, :class:`~optuna.samplers.RandomSampler` is used
             as the default.
 
             .. seealso::
                 :class:`optuna.samplers` module provides built-in independent samplers
                 such as :class:`~optuna.samplers.RandomSampler` and
@@ -134,39 +135,36 @@
         cma_stds: Optional[Dict[str, float]] = None,
         seed: Optional[int] = None,
         cma_opts: Optional[Dict[str, Any]] = None,
         n_startup_trials: int = 1,
         independent_sampler: Optional[BaseSampler] = None,
         warn_independent_sampling: bool = True,
     ) -> None:
-
         _imports.check()
 
         self._x0 = x0
         self._sigma0 = sigma0
         self._cma_stds = cma_stds
         if seed is None:
             seed = random.randint(1, 2**32)
         self._cma_opts = cma_opts or {}
         self._cma_opts["seed"] = seed
         self._cma_opts.setdefault("verbose", -2)
         self._n_startup_trials = n_startup_trials
         self._independent_sampler = independent_sampler or optuna.samplers.RandomSampler(seed=seed)
         self._warn_independent_sampling = warn_independent_sampling
-        self._search_space = optuna.samplers.IntersectionSearchSpace()
+        self._search_space = IntersectionSearchSpace()
 
     def reseed_rng(self) -> None:
-
         self._cma_opts["seed"] = random.randint(1, 2**32)
         self._independent_sampler.reseed_rng()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, BaseDistribution]:
-
         search_space = {}
         for name, distribution in self._search_space.calculate(study).items():
             if distribution.single():
                 # `cma` cannot handle distributions that contain just a single value, so we skip
                 # them. Note that the parameter values for such distributions are sampled in
                 # `Trial`.
                 continue
@@ -178,30 +176,30 @@
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> float:
-
         self._raise_error_if_multi_objective(study)
 
         if self._warn_independent_sampling:
-            complete_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
+            complete_trials = study._get_trials(
+                deepcopy=False, states=(TrialState.COMPLETE,), use_cache=True
+            )
             if len(complete_trials) >= self._n_startup_trials:
                 self._log_independent_sampling(trial, param_name)
 
         return self._independent_sampler.sample_independent(
             study, trial, param_name, param_distribution
         )
 
     def sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, float]:
-
         self._raise_error_if_multi_objective(study)
 
         if len(search_space) == 0:
             return {}
 
         if len(search_space) == 1:
             _logger.info(
@@ -209,15 +207,17 @@
                 "`{}` is used instead of `PyCmaSampler`.".format(
                     self._independent_sampler.__class__.__name__
                 )
             )
             self._warn_independent_sampling = False
             return {}
 
-        complete_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
+        complete_trials = study._get_trials(
+            deepcopy=False, states=(TrialState.COMPLETE,), use_cache=True
+        )
         if len(complete_trials) < self._n_startup_trials:
             return {}
 
         if self._x0 is None:
             self._x0 = self._initialize_x0(search_space)
 
         if self._sigma0 is None:
@@ -230,15 +230,14 @@
         optimizer = _Optimizer(search_space, self._x0, sigma0, self._cma_stds, self._cma_opts)
         trials = study.trials
         last_told_trial_number = optimizer.tell(trials, study.direction)
         return optimizer.ask(trials, last_told_trial_number)
 
     @staticmethod
     def _initialize_x0(search_space: Dict[str, BaseDistribution]) -> Dict[str, Any]:
-
         x0: Dict[str, Any] = {}
         for name, distribution in search_space.items():
             if isinstance(distribution, FloatDistribution):
                 if distribution.log:
                     log_high = math.log(distribution.high)
                     log_low = math.log(distribution.low)
                     x0[name] = math.exp(numpy.mean([log_high, log_low]))
@@ -258,15 +257,14 @@
                 raise NotImplementedError(
                     "The distribution {} is not implemented.".format(distribution)
                 )
         return x0
 
     @staticmethod
     def _initialize_sigma0(search_space: Dict[str, BaseDistribution]) -> float:
-
         sigma0s = []
         for name, distribution in search_space.items():
             if isinstance(distribution, (IntDistribution, FloatDistribution)):
                 if distribution.log:
                     log_high = math.log(distribution.high)
                     log_low = math.log(distribution.low)
                     sigma0s.append((log_high - log_low) / 6)
@@ -277,15 +275,14 @@
             else:
                 raise NotImplementedError(
                     "The distribution {} is not implemented.".format(distribution)
                 )
         return min(sigma0s)
 
     def _log_independent_sampling(self, trial: FrozenTrial, param_name: str) -> None:
-
         _logger.warning(
             "The parameter '{}' in trial#{} is sampled independently "
             "by using `{}` instead of `PyCmaSampler` "
             "(optimization performance may be degraded). "
             "`PyCmaSampler` does not support dynamic search space or `CategoricalDistribution`. "
             "You can suppress this warning by setting `warn_independent_sampling` "
             "to `False` in the constructor of `PyCmaSampler`, "
@@ -297,28 +294,26 @@
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
-
         self._independent_sampler.after_trial(study, trial, state, values)
 
 
 class _Optimizer:
     def __init__(
         self,
         search_space: Dict[str, BaseDistribution],
         x0: Dict[str, Any],
         sigma0: float,
         cma_stds: Optional[Dict[str, float]],
         cma_opts: Dict[str, Any],
     ) -> None:
-
         self._search_space = search_space
         self._param_names = list(sorted(self._search_space.keys()))
 
         lows = []
         highs = []
         for param_name in self._param_names:
             dist = self._search_space[param_name]
@@ -360,15 +355,14 @@
             cma_option["CMA_stds"] = [cma_stds.get(name, 1.0) for name in self._param_names]
 
         cma_opts.update(cma_option)
 
         self._es = cma.CMAEvolutionStrategy(initial_cma_params, sigma0, cma_opts)
 
     def tell(self, trials: List[FrozenTrial], study_direction: StudyDirection) -> int:
-
         complete_trials = self._collect_target_trials(trials, target_states={TrialState.COMPLETE})
 
         popsize = self._es.popsize
         generation = len(complete_trials) // popsize
         last_told_trial_number = -1
         for i in range(generation):
             xs = []
@@ -387,15 +381,14 @@
             # Calling `ask` is required to avoid RuntimeError which claims that `tell` should only
             # be called once per iteration.
             self._es.ask()
             self._es.tell(xs, ys)
         return last_told_trial_number
 
     def ask(self, trials: List[FrozenTrial], last_told_trial_number: int) -> Dict[str, Any]:
-
         individual_index = len(self._collect_target_trials(trials, last_told_trial_number))
         popsize = self._es.popsize
 
         # individual_index may exceed the population size due to the parallel execution of multiple
         # trials. In such cases, `cma.cma.CMAEvolutionStrategy.ask` is called multiple times in an
         # iteration, and that may affect the optimization performance of CMA-ES.
         # In addition, please note that some trials may suggest the same parameters when multiple
@@ -407,15 +400,14 @@
 
         ret_val = {}
         for param_name, value in zip(self._param_names, cma_params):
             ret_val[param_name] = self._to_optuna_params(self._search_space, param_name, value)
         return ret_val
 
     def _is_compatible(self, trial: FrozenTrial) -> bool:
-
         # Thanks to `intersection_search_space()` function, in sequential optimization,
         # the parameters of complete trials are always compatible with the search space.
         #
         # However, in distributed optimization, incompatible trials may complete on a worker
         # just after an intersection search space is calculated on another worker.
 
         for name, distribution in self._search_space.items():
@@ -432,27 +424,25 @@
 
     def _collect_target_trials(
         self,
         trials: List[FrozenTrial],
         last_told: int = -1,
         target_states: Optional[Container[TrialState]] = None,
     ) -> List[FrozenTrial]:
-
         target_trials = [t for t in trials if t.number > last_told]
         target_trials = [t for t in target_trials if self._is_compatible(t)]
         if target_states is not None:
             target_trials = [t for t in target_trials if t.state in target_states]
 
         return target_trials
 
     @staticmethod
     def _to_cma_params(
         search_space: Dict[str, BaseDistribution], param_name: str, optuna_param_value: Any
     ) -> float:
-
         dist = search_space[param_name]
 
         if isinstance(dist, IntDistribution):
             if dist.log:
                 return math.log(optuna_param_value)
         elif isinstance(dist, FloatDistribution):
             if dist.log:
@@ -463,15 +453,14 @@
             return dist.choices.index(optuna_param_value)
         return optuna_param_value
 
     @staticmethod
     def _to_optuna_params(
         search_space: Dict[str, BaseDistribution], param_name: str, cma_param_value: float
     ) -> Any:
-
         dist = search_space[param_name]
         if isinstance(dist, FloatDistribution):
             if dist.log:
                 return math.exp(cma_param_value)
             elif dist.step is not None:
                 v = numpy.round(cma_param_value / dist.step) * dist.step + dist.low
                 return float(min(max(v, dist.low), dist.high))
@@ -505,15 +494,14 @@
         cma_stds: Optional[Dict[str, float]] = None,
         seed: Optional[int] = None,
         cma_opts: Optional[Dict[str, Any]] = None,
         n_startup_trials: int = 1,
         independent_sampler: Optional[BaseSampler] = None,
         warn_independent_sampling: bool = True,
     ) -> None:
-
         super().__init__(
             x0=x0,
             sigma0=sigma0,
             cma_stds=cma_stds,
             seed=seed,
             cma_opts=cma_opts,
             n_startup_trials=n_startup_trials,
```

### Comparing `optuna-3.1.1/optuna/integration/dask.py` & `optuna-3.2.0/optuna/integration/dask.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Tuple
 from typing import Union
 import uuid
 
 import optuna
 from optuna._experimental import experimental_class
 from optuna._imports import try_import
+from optuna._typing import JSONSerializable
 from optuna.distributions import BaseDistribution
 from optuna.distributions import distribution_to_json
 from optuna.distributions import json_to_distribution
 from optuna.storages import BaseStorage
 from optuna.study import StudyDirection
 from optuna.study._frozen import FrozenStudy
 from optuna.trial import FrozenTrial
@@ -342,15 +343,15 @@
 
     def set_trial_system_attr(
         self,
         comm: "distributed.comm.tcp.TCP",
         storage_name: str,
         trial_id: int,
         key: str,
-        value: Any,
+        value: JSONSerializable,
     ) -> None:
         return self.get_storage(storage_name).set_trial_system_attr(
             trial_id=trial_id,
             key=key,
             value=loads(value),  # type: ignore[no-untyped-call]
         )
 
@@ -419,18 +420,26 @@
     This storage class wraps a Optuna storage class (e.g. Optuna’s in-memory or sqlite storage)
     and is used to run optimization trials in parallel on a Dask cluster.
     The underlying Optuna storage object lives on the cluster’s scheduler and any method calls on
     the :obj:`DaskStorage` instance results in the same method being called on the underlying
     Optuna storage object.
 
     See `this example <https://github.com/optuna/optuna-examples/blob/master/
-    dask/dask_simple.py>`__
+    dask/dask_simple.py>`_ or the following YouTube video
     for how to use :obj:`DaskStorage` to extend Optuna's in-memory storage class to run across
     multiple processes.
 
+    .. raw:: html
+
+       <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/euT6_h7iIBA"
+        frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media;
+        gyroscope; picture-in-picture" allowfullscreen></iframe>
+       <br>
+       <br>
+
     Args:
         storage:
             Optuna storage url to use for underlying Optuna storage class to wrap
             (e.g. :obj:`None` for in-memory storage, ``sqlite:///example.db``
             for SQLite storage). Defaults to :obj:`None`.
 
         name:
@@ -438,39 +447,51 @@
             be useful for logging or debugging. If :obj:`None` is provided,
             a random name will be automatically generated.
 
         client:
             Dask ``Client`` to connect to. If not provided, will attempt to find an
             existing ``Client``.
 
+        register:
+            Whether or not to register this storage instance with the cluster scheduler.
+            Most common usage of this storage class will not need to specify this argument.
+            Defaults to ``True``.
+
     """
 
     def __init__(
         self,
         storage: Union[None, str, BaseStorage] = None,
         name: Optional[str] = None,
         client: Optional["distributed.Client"] = None,
+        register: bool = True,
     ):
         _imports.check()
         self.name = name or f"dask-storage-{uuid.uuid4().hex}"
-        self.client = client or get_client()
-
-        if self.client.asynchronous or getattr(thread_state, "on_event_loop_thread", False):
+        self._client = client
+        if register:
+            if self.client.asynchronous or getattr(thread_state, "on_event_loop_thread", False):
+
+                async def _register() -> DaskStorage:
+                    await self.client.run_on_scheduler(  # type: ignore[no-untyped-call]
+                        _register_with_scheduler, storage=storage, name=self.name
+                    )
+                    return self
 
-            async def _register() -> DaskStorage:
-                await self.client.run_on_scheduler(  # type: ignore[no-untyped-call]
+                self._started = asyncio.ensure_future(_register())
+            else:
+                self.client.run_on_scheduler(  # type: ignore[no-untyped-call]
                     _register_with_scheduler, storage=storage, name=self.name
                 )
-                return self
 
-            self._started = asyncio.ensure_future(_register())
-        else:
-            self.client.run_on_scheduler(  # type: ignore[no-untyped-call]
-                _register_with_scheduler, storage=storage, name=self.name
-            )
+    @property
+    def client(self) -> "distributed.Client":
+        if not self._client:
+            self._client = get_client()
+        return self._client
 
     def __await__(self) -> Generator[Any, None, "DaskStorage"]:
         if hasattr(self, "_started"):
             return self._started.__await__()
         else:
 
             async def _() -> DaskStorage:
@@ -479,15 +500,15 @@
             return _().__await__()
 
     def __reduce__(self) -> tuple:
         # We don't have a reference to underlying Optuna storage instance which lives
         # on the scheduler. This is okay since this DaskStorage instance has already been
         # registered with the scheduler, and ``storage`` is only ever needed during the
         # scheduler registration process. We use ``storage=None`` below by convention.
-        return (DaskStorage, (None, self.name))
+        return (DaskStorage, (None, self.name, None, False))
 
     def get_base_storage(self) -> BaseStorage:
         """Retrieve underlying Optuna storage instance from the scheduler.
 
         This is a convenience method to extract the Optuna storage instance stored on
         the Dask scheduler process to the local Python process.
         """
@@ -662,15 +683,15 @@
             self.client.scheduler.optuna_set_trial_user_attr,  # type: ignore[union-attr]
             storage_name=self.name,
             trial_id=trial_id,
             key=key,
             value=dumps(value),  # type: ignore[no-untyped-call]
         )
 
-    def set_trial_system_attr(self, trial_id: int, key: str, value: Any) -> None:
+    def set_trial_system_attr(self, trial_id: int, key: str, value: JSONSerializable) -> None:
         return self.client.sync(  # type: ignore[no-untyped-call]
             self.client.scheduler.optuna_set_trial_system_attr,  # type: ignore[union-attr]
             storage_name=self.name,
             trial_id=trial_id,
             key=key,
             value=dumps(value),  # type: ignore[no-untyped-call]
         )
```

### Comparing `optuna-3.1.1/optuna/integration/fastaiv1.py` & `optuna-3.2.0/optuna/integration/fastaiv1.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,23 +58,21 @@
             An evaluation metric for pruning, e.g. ``valid_loss`` and ``Accuracy``.
             Please refer to `fastai.callbacks.TrackerCallback reference
             <https://fastai1.fast.ai/callbacks.tracker.html#TrackerCallback>`_ for further
             details.
     """
 
     def __init__(self, learn: "Learner", trial: optuna.trial.Trial, monitor: str) -> None:
-
         super().__init__(learn, monitor)
 
         _imports.check()
 
         self._trial = trial
 
     def on_epoch_end(self, epoch: int, **kwargs: Any) -> None:
-
         value = self.get_monitor_value()
         if value is None:
             return
 
         # This conversion is necessary to avoid problems reported in issues.
         # - https://github.com/optuna/optuna/issue/642
         # - https://github.com/optuna/optuna/issue/655.
```

### Comparing `optuna-3.1.1/optuna/integration/fastaiv2.py` & `optuna-3.2.0/optuna/integration/fastaiv2.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/integration/lightgbm.py` & `optuna-3.2.0/optuna/integration/lightgbm.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,37 +76,34 @@
     def __init__(
         self,
         trial: optuna.trial.Trial,
         metric: str,
         valid_name: str = "valid_0",
         report_interval: int = 1,
     ) -> None:
-
         _imports.check()
 
         self._trial = trial
         self._valid_name = valid_name
         self._metric = metric
         self._report_interval = report_interval
 
     def _find_evaluation_result(
         self, target_valid_name: str, env: "CallbackEnv"
     ) -> Optional[List]:
-
         for evaluation_result in env.evaluation_result_list:
             valid_name, metric, current_score, is_higher_better = evaluation_result[:4]
             if valid_name != target_valid_name or metric != self._metric:
                 continue
 
             return evaluation_result
 
         return None
 
     def __call__(self, env: "CallbackEnv") -> None:
-
         if (env.iteration + 1) % self._report_interval == 0:
             # If this callback has been passed to `lightgbm.cv` function,
             # the value of `is_cv` becomes `True`. See also:
             # https://github.com/Microsoft/LightGBM/blob/v2.2.2/python-package/lightgbm/engine.py#L329
             # Note that `5` is not the number of folds but the length of sequence.
             is_cv = len(env.evaluation_result_list) > 0 and len(env.evaluation_result_list[0]) == 5
             if is_cv:
```

### Comparing `optuna-3.1.1/optuna/integration/mlflow.py` & `optuna-3.2.0/optuna/integration/mlflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,14 @@
         tracking_uri: Optional[str] = None,
         metric_name: Union[str, Sequence[str]] = "value",
         create_experiment: bool = True,
         mlflow_kwargs: Optional[Dict[str, Any]] = None,
         tag_study_user_attrs: bool = False,
         tag_trial_user_attrs: bool = True,
     ) -> None:
-
         _imports.check()
 
         if not isinstance(metric_name, Sequence):
             raise TypeError(
                 "Expected metric_name to be string or sequence of strings, got {}.".format(
                     type(metric_name)
                 )
@@ -139,26 +138,24 @@
         self._create_experiment = create_experiment
         self._mlflow_kwargs = mlflow_kwargs or {}
         self._tag_study_user_attrs = tag_study_user_attrs
         self._tag_trial_user_attrs = tag_trial_user_attrs
         self._lock = threading.Lock()
 
     def __call__(self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial) -> None:
-
         with self._lock:
             self._initialize_experiment(study)
 
             with mlflow.start_run(
                 run_id=trial.system_attrs.get(RUN_ID_ATTRIBUTE_KEY),
                 experiment_id=self._mlflow_kwargs.get("experiment_id"),
                 run_name=self._mlflow_kwargs.get("run_name") or str(trial.number),
                 nested=self._mlflow_kwargs.get("nested") or False,
                 tags=self._mlflow_kwargs.get("tags"),
             ):
-
                 # This sets the metrics for MLflow.
                 self._log_metrics(trial.values)
 
                 # This sets the params for MLflow.
                 self._log_params(trial.params)
 
                 # This sets the tags for MLflow.
```

### Comparing `optuna-3.1.1/optuna/integration/mxnet.py` & `optuna-3.2.0/optuna/integration/mxnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,20 @@
             ``accuracy``. If using default metrics like mxnet.metrics.Accuracy, use it's
             default metric name. For custom metrics, use the metric_name provided to
             constructor. Please refer to `mxnet.metrics reference
             <https://mxnet.apache.org/api/python/metric/metric.html>`_ for further details.
     """
 
     def __init__(self, trial: optuna.trial.Trial, eval_metric: str) -> None:
-
         _imports.check()
 
         self._trial = trial
         self._eval_metric = eval_metric
 
     def __call__(self, param: "mx.model.BatchEndParam") -> None:
-
         if param.eval_metric is not None:
             metric_names, metric_values = param.eval_metric.get()
             if type(metric_names) == list and self._eval_metric in metric_names:
                 current_score = metric_values[metric_names.index(self._eval_metric)]
             elif metric_names == self._eval_metric:
                 current_score = metric_values
             else:
```

### Comparing `optuna-3.1.1/optuna/integration/pytorch_distributed.py` & `optuna-3.2.0/optuna/integration/pytorch_distributed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import datetime
 import functools
 import pickle
 from typing import Any
 from typing import Callable
 from typing import Dict
-from typing import List
 from typing import Optional
 from typing import overload
 from typing import Sequence
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import optuna
@@ -18,29 +17,27 @@
 from optuna.distributions import BaseDistribution
 from optuna.distributions import CategoricalChoiceType
 
 
 with try_import() as _imports:
     import torch
     import torch.distributed as dist
-    from torch.distributed import ProcessGroup
+    from torch.distributed import ProcessGroup  # type: ignore[attr-defined]
 
 
 if TYPE_CHECKING:
     from typing_extensions import ParamSpec
 
     _T = TypeVar("_T")
     _P = ParamSpec("_P")
 
 
-_suggest_deprecated_msg = (
-    "Use :func:`~optuna.integration.TorchDistributedTrial.suggest_float` instead."
-)
+_suggest_deprecated_msg = "Use suggest_float{args} instead."
 
-_g_pg: List[Optional["ProcessGroup"]] = [None]
+_g_pg: Optional["ProcessGroup"] = None
 
 
 def broadcast_properties(f: "Callable[_P, _T]") -> "Callable[_P, _T]":
     """Method decorator to fetch updated trial properties from rank 0 after ``f`` is run.
 
     This decorator ensures trial properties (params, distributions, etc.) on all distributed
     processes are up-to-date with the wrapped trial stored on rank 0.
@@ -111,37 +108,38 @@
         called by all workers at once. They invoke synchronous data transmission to share
         processing results and synchronize timing.
 
     """
 
     def __init__(
         self,
-        trial: Optional[optuna.trial.Trial],
+        trial: Optional[optuna.trial.BaseTrial],
         group: Optional["ProcessGroup"] = None,
     ) -> None:
         _imports.check()
+        global _g_pg
 
         if group is not None:
             self._group: "ProcessGroup" = group
         else:
-            if _g_pg[0] is None:
+            if _g_pg is None:
                 if dist.group.WORLD is None:
                     raise RuntimeError("torch distributed is not initialized.")
                 default_pg: "ProcessGroup" = dist.group.WORLD
-                if dist.get_backend(default_pg) == "nccl":  # type: ignore[no-untyped-call]
+                if dist.get_backend(default_pg) == "nccl":
                     new_group: "ProcessGroup" = dist.new_group(  # type: ignore[no-untyped-call]
                         backend="gloo"
                     )
-                    _g_pg[0] = new_group
+                    _g_pg = new_group
                 else:
-                    _g_pg[0] = default_pg
-            self._group = _g_pg[0]
+                    _g_pg = default_pg
+            self._group = _g_pg
 
-        if dist.get_rank(self._group) == 0:  # type: ignore[no-untyped-call]
-            if not isinstance(trial, optuna.trial.Trial):
+        if dist.get_rank(self._group) == 0:
+            if not isinstance(trial, optuna.trial.BaseTrial):
                 raise ValueError(
                     "Rank 0 node expects an optuna.trial.Trial instance as the trial argument."
                 )
         else:
             if trial is not None:
                 raise ValueError(
                     "Non-rank 0 node is supposed to receive None as the trial argument."
@@ -169,27 +167,24 @@
     ) -> float:
         def func() -> float:
             assert self._delegate is not None
             return self._delegate.suggest_float(name, low, high, step=step, log=log)
 
         return self._call_and_communicate(func, torch.float)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args=""))
     def suggest_uniform(self, name: str, low: float, high: float) -> float:
-
         return self.suggest_float(name, low, high)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., log=True)"))
     def suggest_loguniform(self, name: str, low: float, high: float) -> float:
-
         return self.suggest_float(name, low, high, log=True)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., step=...)"))
     def suggest_discrete_uniform(self, name: str, low: float, high: float, q: float) -> float:
-
         return self.suggest_float(name, low, high, step=q)
 
     @broadcast_properties
     def suggest_int(self, name: str, low: int, high: int, step: int = 1, log: bool = False) -> int:
         def func() -> float:
             assert self._delegate is not None
             return self._delegate.suggest_int(name, low, high, step=step, log=log)
@@ -231,15 +226,15 @@
             return self._delegate.suggest_categorical(name, choices)
 
         return self._call_and_communicate_obj(func)
 
     @broadcast_properties
     def report(self, value: float, step: int) -> None:
         err = None
-        if dist.get_rank(self._group) == 0:  # type: ignore[no-untyped-call]
+        if dist.get_rank(self._group) == 0:
             try:
                 assert self._delegate is not None
                 self._delegate.report(value, step)
             except Exception as e:
                 err = e
             err = self._broadcast(err)
         else:
@@ -258,36 +253,38 @@
         # torch.bool seems to be the correct type, but the communication fails
         # due to the RuntimeError.
         return self._call_and_communicate(func, torch.uint8)
 
     @broadcast_properties
     def set_user_attr(self, key: str, value: Any) -> None:
         err = None
-        if dist.get_rank(self._group) == 0:  # type: ignore[no-untyped-call]
+        if dist.get_rank(self._group) == 0:
             try:
                 assert self._delegate is not None
                 self._delegate.set_user_attr(key, value)
             except Exception as e:
                 err = e
             err = self._broadcast(err)
         else:
             err = self._broadcast(err)
 
         if err is not None:
             raise err
 
     @broadcast_properties
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def set_system_attr(self, key: str, value: Any) -> None:
         err = None
 
-        if dist.get_rank(self._group) == 0:  # type: ignore[no-untyped-call]
+        if dist.get_rank(self._group) == 0:
             try:
                 assert self._delegate is not None
-                self._delegate.storage.set_trial_system_attr(self._delegate._trial_id, key, value)
+                self._delegate.storage.set_trial_system_attr(  # type: ignore[attr-defined]
+                    self._delegate._trial_id, key, value  # type: ignore[attr-defined]
+                )
             except Exception as e:
                 err = e
             err = self._broadcast(err)
         else:
             err = self._broadcast(err)
 
         if err is not None:
@@ -306,49 +303,49 @@
         return self._distributions
 
     @property
     def user_attrs(self) -> Dict[str, Any]:
         return self._user_attrs
 
     @property
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def system_attrs(self) -> Dict[str, Any]:
         return self._system_attrs
 
     @property
     def datetime_start(self) -> Optional[datetime]:
         return self._datetime_start
 
     def _call_and_communicate(self, func: Callable, dtype: "torch.dtype") -> Any:
         buffer = torch.empty(1, dtype=dtype)
-        rank = dist.get_rank(self._group)  # type: ignore[no-untyped-call]
+        rank = dist.get_rank(self._group)
         if rank == 0:
             result = func()
             buffer[0] = result
-        dist.broadcast(buffer, src=0, group=self._group)  # type: ignore[no-untyped-call]
+        dist.broadcast(buffer, src=0, group=self._group)
         return buffer.item()
 
     def _call_and_communicate_obj(self, func: Callable) -> Any:
-        rank = dist.get_rank(self._group)  # type: ignore[no-untyped-call]
+        rank = dist.get_rank(self._group)
         result = func() if rank == 0 else None
         return self._broadcast(result)
 
     def _broadcast(self, value: Optional[Any]) -> Any:
         buffer = None
         size_buffer = torch.empty(1, dtype=torch.int)
-        rank = dist.get_rank(self._group)  # type: ignore[no-untyped-call]
+        rank = dist.get_rank(self._group)
         if rank == 0:
             buffer = _to_tensor(value)
             size_buffer[0] = buffer.shape[0]
-        dist.broadcast(size_buffer, src=0, group=self._group)  # type: ignore[no-untyped-call]
+        dist.broadcast(size_buffer, src=0, group=self._group)
         buffer_size = int(size_buffer.item())
         if rank != 0:
             buffer = torch.empty(buffer_size, dtype=torch.uint8)
         assert buffer is not None
-        dist.broadcast(buffer, src=0, group=self._group)  # type: ignore[no-untyped-call]
+        dist.broadcast(buffer, src=0, group=self._group)
         return _from_tensor(buffer)
 
 
 def _to_tensor(obj: Any) -> "torch.Tensor":
     b = bytearray(pickle.dumps(obj))
     return torch.tensor(b, dtype=torch.uint8)
```

### Comparing `optuna-3.1.1/optuna/integration/pytorch_ignite.py` & `optuna-3.2.0/optuna/integration/pytorch_ignite.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,19 @@
             A name of metric for pruning, e.g., ``accuracy`` and ``loss``.
         trainer:
             A trainer engine of PyTorch Ignite. Please refer to `ignite.engine.Engine reference
             <https://pytorch.org/ignite/engine.html#ignite.engine.Engine>`_ for further details.
     """
 
     def __init__(self, trial: Trial, metric: str, trainer: "Engine") -> None:
-
         _imports.check()
 
         self._trial = trial
         self._metric = metric
         self._trainer = trainer
 
     def __call__(self, engine: "Engine") -> None:
-
         score = engine.state.metrics[self._metric]
         self._trial.report(score, self._trainer.state.epoch)
         if self._trial.should_prune():
             message = "Trial was pruned at {} epoch.".format(self._trainer.state.epoch)
             raise optuna.TrialPruned(message)
```

### Comparing `optuna-3.1.1/optuna/integration/shap.py` & `optuna-3.2.0/optuna/integration/shap.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     def evaluate(
         self,
         study: Study,
         params: Optional[List[str]] = None,
         *,
         target: Optional[Callable[[FrozenTrial], float]] = None,
     ) -> Dict[str, float]:
-
         if target is None and study._is_multi_objective():
             raise ValueError(
                 "If the `study` is being used for multi-objective optimization, "
                 "please specify the `target`. For example, use "
                 "`target=lambda t: t.values[0]` for the first objective value."
             )
```

### Comparing `optuna-3.1.1/optuna/integration/sklearn.py` & `optuna-3.2.0/optuna/integration/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,17 @@
     from sklearn.base import BaseEstimator
     from sklearn.base import clone
     from sklearn.base import is_classifier
     from sklearn.metrics import check_scoring
     from sklearn.model_selection import BaseCrossValidator
     from sklearn.model_selection import check_cv
     from sklearn.model_selection import cross_validate
+    from sklearn.utils import _safe_indexing as sklearn_safe_indexing
     from sklearn.utils import check_random_state
     from sklearn.utils.metaestimators import _safe_split
-
-    if sklearn.__version__ >= "0.22":
-        from sklearn.utils import _safe_indexing as sklearn_safe_indexing
-    else:
-        from sklearn.utils import safe_indexing as sklearn_safe_indexing
     from sklearn.utils.validation import check_is_fitted
 
 if not _imports.is_successful():
     BaseEstimator = object  # NOQA
 
 ArrayLikeType = Union[List, np.ndarray, "pd.Series", spmatrix]
 OneDimArrayLikeType = Union[List[float], np.ndarray, "pd.Series"]
@@ -60,18 +56,16 @@
 
 _logger = logging.get_logger(__name__)
 
 
 def _check_fit_params(
     X: TwoDimArrayLikeType, fit_params: Dict, indices: OneDimArrayLikeType
 ) -> Dict:
-
     fit_params_validated = {}
     for key, value in fit_params.items():
-
         # NOTE Original implementation:
         # https://github.com/scikit-learn/scikit-learn/blob/ \
         # 2467e1b84aeb493a22533fa15ff92e0d7c05ed1c/sklearn/utils/validation.py#L1324-L1328
         # Scikit-learn does not accept non-iterable inputs.
         # This line is for keeping backward compatibility.
         # (See: https://github.com/scikit-learn/scikit-learn/issues/15805)
         if not _is_arraylike(value) or _num_samples(value) != _num_samples(X):
@@ -82,35 +76,32 @@
     return fit_params_validated
 
 
 # NOTE Original implementation:
 # https://github.com/scikit-learn/scikit-learn/blob/ \
 # 8caa93889f85254fc3ca84caa0a24a1640eebdd1/sklearn/utils/validation.py#L131-L135
 def _is_arraylike(x: Any) -> bool:
-
     return hasattr(x, "__len__") or hasattr(x, "shape") or hasattr(x, "__array__")
 
 
 # NOTE Original implementation:
 # https://github.com/scikit-learn/scikit-learn/blob/ \
 # 8caa93889f85254fc3ca84caa0a24a1640eebdd1/sklearn/utils/validation.py#L217-L234
 def _make_indexable(iterable: IterableType) -> IndexableType:
-
     tocsr_func = getattr(iterable, "tocsr", None)
     if tocsr_func is not None and sp.sparse.issparse(iterable):
         return tocsr_func(iterable)
     elif hasattr(iterable, "__getitem__") or hasattr(iterable, "iloc"):
         return iterable
     elif iterable is None:
         return iterable
     return np.array(iterable)
 
 
 def _num_samples(x: ArrayLikeType) -> int:
-
     # NOTE For dask dataframes
     # https://github.com/scikit-learn/scikit-learn/blob/ \
     # 8caa93889f85254fc3ca84caa0a24a1640eebdd1/sklearn/utils/validation.py#L155-L158
     x_shape = getattr(x, "shape", None)
     if x_shape is not None:
         if isinstance(x_shape[0], Integral):
             return int(x_shape[0])
@@ -120,15 +111,14 @@
     except TypeError:
         raise TypeError("Expected sequence or array-like, got %s." % type(x)) from None
 
 
 def _safe_indexing(
     X: Union[OneDimArrayLikeType, TwoDimArrayLikeType], indices: OneDimArrayLikeType
 ) -> Union[OneDimArrayLikeType, TwoDimArrayLikeType]:
-
     if X is None:
         return X
 
     return sklearn_safe_indexing(X, indices)
 
 
 class _Objective:
@@ -186,43 +176,41 @@
 
         scoring:
             Scorer function.
     """
 
     def __init__(
         self,
-        estimator: "BaseEstimator",
+        estimator: "sklearn.base.BaseEstimator",
         param_distributions: Mapping[str, distributions.BaseDistribution],
         X: TwoDimArrayLikeType,
         y: Optional[Union[OneDimArrayLikeType, TwoDimArrayLikeType]],
         cv: "BaseCrossValidator",
         enable_pruning: bool,
         error_score: Union[Number, float, str],
         fit_params: Dict[str, Any],
         groups: Optional[OneDimArrayLikeType],
         max_iter: int,
         return_train_score: bool,
         scoring: Callable[..., Number],
     ) -> None:
-
         self.cv = cv
         self.enable_pruning = enable_pruning
         self.error_score = error_score
         self.estimator = estimator
         self.fit_params = fit_params
         self.groups = groups
         self.max_iter = max_iter
         self.param_distributions = param_distributions
         self.return_train_score = return_train_score
         self.scoring = scoring
         self.X = X
         self.y = y
 
     def __call__(self, trial: Trial) -> float:
-
         estimator = clone(self.estimator)
         params = self._get_params(trial)
 
         estimator.set_params(**params)
 
         if self.enable_pruning:
             scores = self._cross_validate_with_pruning(trial, estimator)
@@ -240,17 +228,16 @@
             )
 
         self._store_scores(trial, scores)
 
         return trial.user_attrs["mean_test_score"]
 
     def _cross_validate_with_pruning(
-        self, trial: Trial, estimator: "BaseEstimator"
+        self, trial: Trial, estimator: "sklearn.base.BaseEstimator"
     ) -> Mapping[str, OneDimArrayLikeType]:
-
         if is_classifier(estimator):
             partial_fit_params = self.fit_params.copy()
             y = self.y.values if isinstance(self.y, pd.Series) else self.y
             classes = np.unique(y)
 
             partial_fit_params.setdefault("classes", classes)
 
@@ -287,28 +274,26 @@
                 self._store_scores(trial, scores)
 
                 raise TrialPruned("trial was pruned at iteration {}.".format(step))
 
         return scores
 
     def _get_params(self, trial: Trial) -> Dict[str, Any]:
-
         return {
             name: trial._suggest(name, distribution)
             for name, distribution in self.param_distributions.items()
         }
 
     def _partial_fit_and_score(
         self,
-        estimator: "BaseEstimator",
+        estimator: "sklearn.base.BaseEstimator",
         train: List[int],
         test: List[int],
         partial_fit_params: Dict[str, Any],
     ) -> List[Number]:
-
         X_train, y_train = _safe_split(estimator, self.X, self.y, train)
         X_test, y_test = _safe_split(estimator, self.X, self.y, test, train_indices=train)
 
         start_time = time()
 
         try:
             estimator.partial_fit(X_train, y_train, **partial_fit_params)
@@ -344,15 +329,14 @@
 
         if self.return_train_score:
             ret.insert(0, train_score)
 
         return ret
 
     def _store_scores(self, trial: Trial, scores: Mapping[str, OneDimArrayLikeType]) -> None:
-
         for name, array in scores.items():
             if name in ["test_score", "train_score"]:
                 for i, score in enumerate(array):
                     trial.set_user_attr("split{}_{}".format(i, name), score)
 
             trial.set_user_attr("mean_{}".format(name), np.nanmean(array))
             trial.set_user_attr("std_{}".format(name), np.nanstd(array))
@@ -372,16 +356,17 @@
             Dictionary where keys are parameters and values are distributions.
             Distributions are assumed to implement the optuna distribution
             interface.
 
         cv:
             Cross-validation strategy. Possible inputs for cv are:
 
+            - :obj:`None`, to use the default 5-fold cross validation,
             - integer to specify the number of folds in a CV splitter,
-            - a CV splitter,
+            - `CV splitter <https://scikit-learn.org/stable/glossary.html#term-CV-splitter>`_,
             - an iterable yielding (train, validation) splits as arrays of indices.
 
             For integer, if ``estimator`` is a classifier and ``y`` is
             either binary or multiclass,
             ``sklearn.model_selection.StratifiedKFold`` is used. otherwise,
             ``sklearn.model_selection.KFold`` is used.
 
@@ -396,16 +381,16 @@
             affect the refit step, which will always raise the error.
 
         max_iter:
             Maximum number of epochs. This is only used if the underlying
             estimator supports ``partial_fit``.
 
         n_jobs:
-            Number of :obj:`threading` based parallel jobs. ``-1`` means
-            using the number is set to CPU count.
+            Number of :obj:`threading` based parallel jobs. :obj:`None` means ``1``.
+            ``-1`` means using the number is set to CPU count.
 
                 .. note::
                     ``n_jobs`` allows parallelization using :obj:`threading` and may suffer from
                     `Python's GIL <https://wiki.python.org/moin/GlobalInterpreterLock>`_.
                     It is recommended to use :ref:`process-based parallelization<distributed>`
                     if ``func`` is CPU bound.
 
@@ -517,15 +502,14 @@
         For the minimization problem, please multiply ``-1``.
     """
 
     _required_parameters = ["estimator", "param_distributions"]
 
     @property
     def _estimator_type(self) -> str:
-
         return self.estimator._estimator_type
 
     @property
     def best_index_(self) -> int:
         """Trial number which corresponds to the best candidate parameter setting.
 
         Retuned value is equivant to ``optuna_search.best_trial_.number``.
@@ -685,33 +669,33 @@
 
         self._check_is_fitted()
 
         return self.study_.trials_dataframe
 
     def __init__(
         self,
-        estimator: "BaseEstimator",
+        estimator: "sklearn.base.BaseEstimator",
         param_distributions: Mapping[str, distributions.BaseDistribution],
-        cv: Optional[Union["BaseCrossValidator", int]] = 5,
+        *,
+        cv: Optional[Union[int, "BaseCrossValidator", Iterable]] = None,
         enable_pruning: bool = False,
         error_score: Union[Number, float, str] = np.nan,
         max_iter: int = 1000,
-        n_jobs: int = 1,
+        n_jobs: Optional[int] = None,
         n_trials: int = 10,
         random_state: Optional[Union[int, np.random.RandomState]] = None,
         refit: bool = True,
         return_train_score: bool = False,
         scoring: Optional[Union[Callable[..., float], str]] = None,
         study: Optional[study_module.Study] = None,
         subsample: Union[float, int] = 1.0,
         timeout: Optional[float] = None,
         verbose: int = 0,
         callbacks: Optional[List[Callable[[study_module.Study, FrozenTrial], None]]] = None,
     ) -> None:
-
         _imports.check()
 
         if not isinstance(param_distributions, dict):
             raise TypeError("param_distributions must be a dictionary.")
 
         # Rejecting deprecated distributions as they may cause cryptic error
         # when cloning OptunaSearchCV instance.
@@ -726,37 +710,35 @@
 
         self.cv = cv
         self.enable_pruning = enable_pruning
         self.error_score = error_score
         self.estimator = estimator
         self.max_iter = max_iter
         self.n_trials = n_trials
-        self.n_jobs = n_jobs
+        self.n_jobs = n_jobs if n_jobs else 1
         self.param_distributions = param_distributions
         self.random_state = random_state
         self.refit = refit
         self.return_train_score = return_train_score
         self.scoring = scoring
         self.study = study
         self.subsample = subsample
         self.timeout = timeout
         self.verbose = verbose
         self.callbacks = callbacks
 
     def _check_is_fitted(self) -> None:
-
         attributes = ["n_splits_", "sample_indices_", "scorer_", "study_"]
 
         if self.refit:
             attributes += ["best_estimator_", "refit_time_"]
 
         check_is_fitted(self, attributes)
 
     def _check_params(self) -> None:
-
         if not hasattr(self.estimator, "fit"):
             raise ValueError("estimator must be a scikit-learn estimator.")
 
         for name, distribution in self.param_distributions.items():
             if not isinstance(distribution, distributions.BaseDistribution):
                 raise ValueError("Value of {} must be a optuna distribution.".format(name))
 
@@ -766,24 +748,22 @@
         if self.max_iter <= 0:
             raise ValueError("max_iter must be > 0, got {}.".format(self.max_iter))
 
         if self.study is not None and self.study.direction != StudyDirection.MAXIMIZE:
             raise ValueError("direction of study must be 'maximize'.")
 
     def _more_tags(self) -> Dict[str, bool]:
-
         return {"non_deterministic": True, "no_validation": True}
 
     def _refit(
         self,
         X: TwoDimArrayLikeType,
         y: Optional[Union[OneDimArrayLikeType, TwoDimArrayLikeType]] = None,
         **fit_params: Any,
     ) -> "OptunaSearchCV":
-
         n_samples = _num_samples(X)
 
         self.best_estimator_ = clone(self.estimator)
 
         try:
             self.best_estimator_.set_params(**self.study_.best_params)
         except ValueError as e:
```

### Comparing `optuna-3.1.1/optuna/integration/skopt.py` & `optuna-3.2.0/optuna/integration/skopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,54 +12,40 @@
 
 import optuna
 from optuna import distributions
 from optuna import samplers
 from optuna._imports import try_import
 from optuna.exceptions import ExperimentalWarning
 from optuna.samplers import BaseSampler
+from optuna.search_space import IntersectionSearchSpace
 from optuna.study import Study
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 with try_import() as _imports:
     import skopt
     from skopt.space import space
 
 
 class SkoptSampler(BaseSampler):
     """Sampler using Scikit-Optimize as the backend.
 
-    Example:
-
-        Optimize a simple quadratic function by using :class:`~optuna.integration.SkoptSampler`.
-
-        .. testcode::
-
-            import optuna
-
-
-            def objective(trial):
-                x = trial.suggest_float("x", -10, 10)
-                y = trial.suggest_int("y", 0, 10)
-                return x**2 + y
-
-
-            sampler = optuna.integration.SkoptSampler()
-            study = optuna.create_study(sampler=sampler)
-            study.optimize(objective, n_trials=10)
+    The use of :class:`~optuna.integration.SkoptSampler` is highly not recommended, as the
+    development of Scikit-Optimize has been inactive and we have identified compatibility
+    issues with newer NumPy versions.
 
     Args:
         independent_sampler:
             A :class:`~optuna.samplers.BaseSampler` instance that is used for independent
             sampling. The parameters not contained in the relative search space are sampled
             by this sampler.
             The search space for :class:`~optuna.integration.SkoptSampler` is determined by
-            :func:`~optuna.samplers.intersection_search_space()`.
+            :func:`~optuna.search_space.intersection_search_space()`.
 
             If :obj:`None` is specified, :class:`~optuna.samplers.RandomSampler` is used
             as the default.
 
             .. seealso::
                 :class:`optuna.samplers` module provides built-in independent samplers
                 such as :class:`~optuna.samplers.RandomSampler` and
@@ -110,47 +96,44 @@
         warn_independent_sampling: bool = True,
         skopt_kwargs: Optional[Dict[str, Any]] = None,
         n_startup_trials: int = 1,
         *,
         consider_pruned_trials: bool = False,
         seed: Optional[int] = None,
     ) -> None:
-
         _imports.check()
 
         self._skopt_kwargs = skopt_kwargs or {}
         if "dimensions" in self._skopt_kwargs:
             del self._skopt_kwargs["dimensions"]
 
         self._independent_sampler = independent_sampler or samplers.RandomSampler(seed=seed)
         self._warn_independent_sampling = warn_independent_sampling
         self._n_startup_trials = n_startup_trials
-        self._search_space = samplers.IntersectionSearchSpace()
+        self._search_space = IntersectionSearchSpace()
         self._consider_pruned_trials = consider_pruned_trials
 
         if self._consider_pruned_trials:
             warnings.warn(
                 "`consider_pruned_trials` option is an experimental feature."
                 " The interface can change in the future.",
                 ExperimentalWarning,
             )
 
         if seed is not None and "random_state" not in self._skopt_kwargs:
             self._skopt_kwargs["random_state"] = seed
         self._rng: Optional[np.random.RandomState] = None
 
     def reseed_rng(self) -> None:
-
-        self._skopt_kwargs["random_state"] = random.randint(1, 2**32)
+        self._skopt_kwargs["random_state"] = random.randint(1, np.iinfo(np.int32).max)
         self._independent_sampler.reseed_rng()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, distributions.BaseDistribution]:
-
         search_space = {}
         for name, distribution in self._search_space.calculate(study).items():
             if distribution.single():
                 if not isinstance(distribution, distributions.CategoricalDistribution):
                     # `skopt` cannot handle non-categorical distributions that contain just
                     # a single value, so we skip this distribution.
                     #
@@ -163,15 +146,14 @@
 
     def sample_relative(
         self,
         study: Study,
         trial: FrozenTrial,
         search_space: Dict[str, distributions.BaseDistribution],
     ) -> Dict[str, Any]:
-
         self._raise_error_if_multi_objective(study)
 
         if len(search_space) == 0:
             return {}
 
         complete_trials = self._get_trials(study)
         if len(complete_trials) < self._n_startup_trials:
@@ -188,43 +170,41 @@
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: distributions.BaseDistribution,
     ) -> Any:
-
         self._raise_error_if_multi_objective(study)
 
         if self._warn_independent_sampling:
             complete_trials = self._get_trials(study)
             if len(complete_trials) >= self._n_startup_trials:
                 self._log_independent_sampling(trial, param_name)
 
         return self._independent_sampler.sample_independent(
             study, trial, param_name, param_distribution
         )
 
     def _log_independent_sampling(self, trial: FrozenTrial, param_name: str) -> None:
-
         logger = optuna.logging.get_logger(__name__)
         logger.warning(
             "The parameter '{}' in trial#{} is sampled independently "
             "by using `{}` instead of `SkoptSampler` "
             "(optimization performance may be degraded). "
             "You can suppress this warning by setting `warn_independent_sampling` "
             "to `False` in the constructor of `SkoptSampler`, "
             "if this independent sampling is intended behavior.".format(
                 param_name, trial.number, self._independent_sampler.__class__.__name__
             )
         )
 
     def _get_trials(self, study: Study) -> List[FrozenTrial]:
         complete_trials = []
-        for t in study.get_trials(deepcopy=False):
+        for t in study._get_trials(deepcopy=False, use_cache=True):
             if t.state == TrialState.COMPLETE:
                 complete_trials.append(t)
             elif (
                 t.state == TrialState.PRUNED
                 and len(t.intermediate_values) > 0
                 and self._consider_pruned_trials
             ):
@@ -240,23 +220,21 @@
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
-
         self._independent_sampler.after_trial(study, trial, state, values)
 
 
 class _Optimizer:
     def __init__(
         self, search_space: Dict[str, distributions.BaseDistribution], skopt_kwargs: Dict[str, Any]
     ) -> None:
-
         self._search_space = search_space
 
         dimensions = []
         for name, distribution in sorted(self._search_space.items()):
             if isinstance(distribution, distributions.IntDistribution):
                 if distribution.log:
                     low = distribution.low - 0.5
@@ -284,30 +262,28 @@
                 )
 
             dimensions.append(dimension)
 
         self._optimizer = skopt.Optimizer(dimensions, **skopt_kwargs)
 
     def tell(self, study: Study, complete_trials: List[FrozenTrial]) -> None:
-
         xs = []
         ys = []
 
         for trial in complete_trials:
             if not self._is_compatible(trial):
                 continue
 
             x, y = self._complete_trial_to_skopt_observation(study, trial)
             xs.append(x)
             ys.append(y)
 
         self._optimizer.tell(xs, ys)
 
     def ask(self) -> Dict[str, Any]:
-
         params = {}
         param_values = self._optimizer.ask()
         for (name, distribution), value in zip(sorted(self._search_space.items()), param_values):
             if isinstance(distribution, distributions.FloatDistribution):
                 # Type of value is np.floating, so cast it to Python's built-in float.
                 value = float(value)
                 if distribution.step is not None:
@@ -320,15 +296,14 @@
                     value = int(value * distribution.step + distribution.low)
 
             params[name] = value
 
         return params
 
     def _is_compatible(self, trial: FrozenTrial) -> bool:
-
         # Thanks to `intersection_search_space()` function, in sequential optimization,
         # the parameters of complete trials are always compatible with the search space.
         #
         # However, in distributed optimization, incompatible trials may complete on a worker
         # just after an intersection search space is calculated on another worker.
 
         for name, distribution in self._search_space.items():
@@ -342,15 +317,14 @@
                 return False
 
         return True
 
     def _complete_trial_to_skopt_observation(
         self, study: Study, trial: FrozenTrial
     ) -> Tuple[List[Any], float]:
-
         param_values = []
         for name, distribution in sorted(self._search_space.items()):
             param_value = trial.params[name]
 
             if isinstance(distribution, distributions.FloatDistribution):
                 if distribution.step is not None:
                     param_value = (param_value - distribution.low) // distribution.step
```

### Comparing `optuna-3.1.1/optuna/integration/tensorboard.py` & `optuna-3.2.0/optuna/integration/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         with tf.summary.create_file_writer(run_dir).as_default():
             hp.hparams(hparams, trial_id=run_name)  # record the values used in this trial
             tf.summary.scalar(self._metric_name, trial_value, step=trial.number)
 
     def _add_distributions(
         self, distributions: Dict[str, optuna.distributions.BaseDistribution]
     ) -> None:
-
         supported_distributions = (
             optuna.distributions.CategoricalDistribution,
             optuna.distributions.FloatDistribution,
             optuna.distributions.IntDistribution,
         )
 
         for param_name, param_distribution in distributions.items():
```

### Comparing `optuna-3.1.1/optuna/integration/wandb.py` & `optuna-3.2.0/optuna/integration/wandb.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 
     def __init__(
         self,
         metric_name: Union[str, Sequence[str]] = "value",
         wandb_kwargs: Optional[Dict[str, Any]] = None,
         as_multirun: bool = False,
     ) -> None:
-
         _imports.check()
 
         if not isinstance(metric_name, Sequence):
             raise TypeError(
                 "Expected metric_name to be string or sequence of strings, got {}.".format(
                     type(metric_name)
                 )
@@ -127,15 +126,14 @@
         self._wandb_kwargs = wandb_kwargs or {}
         self._as_multirun = as_multirun
 
         if not self._as_multirun:
             self._initialize_run()
 
     def __call__(self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial) -> None:
-
         if isinstance(self._metric_name, str):
             if len(trial.values) > 1:
                 # Broadcast default name for multi-objective optimization.
                 names = ["{}_{}".format(self._metric_name, i) for i in range(len(trial.values))]
 
             else:
                 names = [self._metric_name]
@@ -215,15 +213,14 @@
         Returns:
             Objective function with W&B tracking enabled.
         """
 
         def decorator(func: ObjectiveFuncType) -> ObjectiveFuncType:
             @functools.wraps(func)
             def wrapper(trial: optuna.trial.Trial) -> Union[float, Sequence[float]]:
-
                 run = wandb.run  # Uses global run when `as_multirun` is set to False.
                 if not run:
                     run = self._initialize_run()
                     run.name = f"trial/{trial.number}/{run.name}"
 
                 return func(trial)
```

### Comparing `optuna-3.1.1/optuna/integration/xgboost.py` & `optuna-3.2.0/optuna/integration/xgboost.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         __doc__ = _doc
 
         def __init__(self, trial: optuna.trial.Trial, observation_key: str) -> None:
             self._trial = trial
             self._observation_key = observation_key
 
         def __call__(self, env: "xgb.core.CallbackEnv") -> None:  # type: ignore
-
             context = _get_callback_context(env)
             evaluation_result_list = env.evaluation_result_list
             if context == "cv":
                 # Remove a third element: the stddev of the metric across the
                 # cross-validation folds.
                 evaluation_result_list = [
                     (key, metric) for key, metric, _ in evaluation_result_list
```

### Comparing `optuna-3.1.1/optuna/logging.py` & `optuna-3.2.0/optuna/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from logging import CRITICAL
 from logging import DEBUG
 from logging import ERROR
 from logging import FATAL
 from logging import INFO
 from logging import WARN
 from logging import WARNING
+import os
+import sys
 import threading
 from typing import Optional
 
 import colorlog
 
 
 __all__ = [
@@ -22,37 +24,49 @@
     "WARNING",
 ]
 
 _lock: threading.Lock = threading.Lock()
 _default_handler: Optional[logging.Handler] = None
 
 
-def create_default_formatter() -> colorlog.ColoredFormatter:
+def create_default_formatter() -> logging.Formatter:
     """Create a default formatter of log messages.
 
     This function is not supposed to be directly accessed by library users.
     """
-
-    return colorlog.ColoredFormatter(
-        "%(log_color)s[%(levelname)1.1s %(asctime)s]%(reset)s %(message)s"
-    )
+    header = "[%(levelname)1.1s %(asctime)s]"
+    message = "%(message)s"
+    if _color_supported():
+        return colorlog.ColoredFormatter(
+            f"%(log_color)s{header}%(reset)s {message}",
+        )
+    return logging.Formatter(f"{header} {message}")
+
+
+def _color_supported() -> bool:
+    """Detection of color support."""
+    # NO_COLOR environment variable:
+    if os.environ.get("NO_COLOR", None):
+        return False
+
+    if not hasattr(sys.stderr, "isatty") or not sys.stderr.isatty():
+        return False
+    else:
+        return True
 
 
 def _get_library_name() -> str:
-
     return __name__.split(".")[0]
 
 
 def _get_library_root_logger() -> logging.Logger:
-
     return logging.getLogger(_get_library_name())
 
 
 def _configure_library_root_logger() -> None:
-
     global _default_handler
 
     with _lock:
         if _default_handler:
             # This library has already configured the library root logger.
             return
         _default_handler = logging.StreamHandler()  # Set sys.stderr as stream.
@@ -62,15 +76,14 @@
         library_root_logger: logging.Logger = _get_library_root_logger()
         library_root_logger.addHandler(_default_handler)
         library_root_logger.setLevel(logging.INFO)
         library_root_logger.propagate = False
 
 
 def _reset_library_root_logger() -> None:
-
     global _default_handler
 
     with _lock:
         if not _default_handler:
             return
 
         library_root_logger: logging.Logger = _get_library_root_logger()
```

### Comparing `optuna-3.1.1/optuna/multi_objective/samplers/__init__.py` & `optuna-3.2.0/optuna/multi_objective/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/multi_objective/samplers/_adapter.py` & `optuna-3.2.0/optuna/multi_objective/samplers/_adapter.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/multi_objective/samplers/_base.py` & `optuna-3.2.0/optuna/multi_objective/samplers/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             trial:
                 Target trial object.
 
         Returns:
             A dictionary containing the parameter names and parameter's distributions.
 
         .. seealso::
-            Please refer to :func:`~optuna.samplers.intersection_search_space` as an
+            Please refer to :func:`~optuna.search_space.intersection_search_space` as an
             implementation of
             :func:`~optuna.multi_objective.samplers.BaseMultiObjectiveSampler.infer_relative_search_space`.
         """
 
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `optuna-3.1.1/optuna/multi_objective/samplers/_motpe.py` & `optuna-3.2.0/optuna/multi_objective/samplers/_motpe.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         consider_endpoints: bool = True,
         n_startup_trials: int = 10,
         n_ehvi_candidates: int = 24,
         gamma: Callable[[int], int] = default_gamma,
         weights_above: Callable[[int], np.ndarray] = _default_weights_above,
         seed: Optional[int] = None,
     ) -> None:
-
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", ExperimentalWarning)
             self._motpe_sampler = MOTPESampler(
                 consider_prior=consider_prior,
                 prior_weight=prior_weight,
                 consider_magic_clip=consider_magic_clip,
                 consider_endpoints=consider_endpoints,
@@ -147,15 +146,14 @@
     def sample_independent(
         self,
         study: "multi_objective.study.MultiObjectiveStudy",
         trial: "multi_objective.trial.FrozenMultiObjectiveTrial",
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-
         return self._motpe_sampler.sample_independent(
             _create_study(study), _create_trial(trial), param_name, param_distribution
         )
 
 
 def _create_study(mo_study: "multi_objective.study.MultiObjectiveStudy") -> "optuna.Study":
     study = create_study(
```

### Comparing `optuna-3.1.1/optuna/multi_objective/samplers/_nsga2.py` & `optuna-3.2.0/optuna/multi_objective/samplers/_nsga2.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/multi_objective/samplers/_random.py` & `optuna-3.2.0/optuna/multi_objective/samplers/_random.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/multi_objective/study.py` & `optuna-3.2.0/optuna/multi_objective/study.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/multi_objective/trial.py` & `optuna-3.2.0/optuna/multi_objective/trial.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/multi_objective/visualization/_pareto_front.py` & `optuna-3.2.0/optuna/multi_objective/visualization/_pareto_front.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
         raise ValueError("`plot_pareto_front` function only supports 2 or 3 objective studies.")
 
 
 def _get_non_pareto_front_trials(
     study: MultiObjectiveStudy,
     pareto_trials: List["multi_objective.trial.FrozenMultiObjectiveTrial"],
 ) -> List["multi_objective.trial.FrozenMultiObjectiveTrial"]:
-
     non_pareto_trials = []
     for trial in study.get_trials():
         if trial.state == TrialState.COMPLETE and trial not in pareto_trials:
             non_pareto_trials.append(trial)
     return non_pareto_trials
```

### Comparing `optuna-3.1.1/optuna/progress_bar.py` & `optuna-3.2.0/optuna/progress_bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any
 from typing import Optional
 from typing import TYPE_CHECKING
 
 from tqdm.auto import tqdm
 
 from optuna import logging as optuna_logging
-from optuna._experimental import experimental_func
 
 
 if TYPE_CHECKING:
     from optuna.study import Study
 
 _tqdm_handler: Optional["_TqdmLoggingHandler"] = None
 
@@ -42,43 +41,36 @@
 
     def __init__(
         self,
         is_valid: bool,
         n_trials: Optional[int] = None,
         timeout: Optional[float] = None,
     ) -> None:
-
         self._is_valid = is_valid and (n_trials or timeout) is not None
         self._n_trials = n_trials
         self._timeout = timeout
         self._last_elapsed_seconds = 0.0
 
         if self._is_valid:
-            self._init_valid()
-
-    # TODO(hvy): Remove initialization indirection via this method when the progress bar is no
-    # longer experimental.
-    @experimental_func("1.2.0", name="Progress bar")
-    def _init_valid(self) -> None:
-
-        if self._n_trials is not None:
-            self._progress_bar = tqdm(total=self._n_trials)
-
-        else:
-            total = tqdm.format_interval(self._timeout)
-            fmt = "{desc} {percentage:3.0f}%|{bar}| {elapsed}/" + total
-            self._progress_bar = tqdm(total=self._timeout, bar_format=fmt)
-
-        global _tqdm_handler
-
-        _tqdm_handler = _TqdmLoggingHandler()
-        _tqdm_handler.setLevel(logging.INFO)
-        _tqdm_handler.setFormatter(optuna_logging.create_default_formatter())
-        optuna_logging.disable_default_handler()
-        optuna_logging._get_library_root_logger().addHandler(_tqdm_handler)
+            if self._n_trials is not None:
+                self._progress_bar = tqdm(total=self._n_trials)
+            elif self._timeout is not None:
+                total = tqdm.format_interval(self._timeout)
+                fmt = "{desc} {percentage:3.0f}%|{bar}| {elapsed}/" + total
+                self._progress_bar = tqdm(total=self._timeout, bar_format=fmt)
+            else:
+                assert False
+
+            global _tqdm_handler
+
+            _tqdm_handler = _TqdmLoggingHandler()
+            _tqdm_handler.setLevel(logging.INFO)
+            _tqdm_handler.setFormatter(optuna_logging.create_default_formatter())
+            optuna_logging.disable_default_handler()
+            optuna_logging._get_library_root_logger().addHandler(_tqdm_handler)
 
     def update(self, elapsed_seconds: float, study: "Study") -> None:
         """Update the progress bars if ``is_valid`` is :obj:`True`.
 
         Args:
             elapsed_seconds:
                 The time past since :func:`~optuna.study.Study.optimize` started.
```

### Comparing `optuna-3.1.1/optuna/pruners/__init__.py` & `optuna-3.2.0/optuna/pruners/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/pruners/_base.py` & `optuna-3.2.0/optuna/pruners/_base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/pruners/_hyperband.py` & `optuna-3.2.0/optuna/pruners/_hyperband.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     .. note::
         Hyperband has several :class:`~optuna.pruners.SuccessiveHalvingPruner`\\ s. Each
         :class:`~optuna.pruners.SuccessiveHalvingPruner` is referred to as "bracket" in the
         original paper. The number of brackets is an important factor to control the early
         stopping behavior of Hyperband and is automatically determined by ``min_resource``,
         ``max_resource`` and ``reduction_factor`` as
         :math:`\\mathrm{The\\ number\\ of\\ brackets} =
-        \\mathrm{floor}(\\log_{\\texttt{reduction_factor}}
-        (\\frac{\\texttt{max_resource}}{\\texttt{min_resource}})) + 1`.
+        \\mathrm{floor}(\\log_{\\texttt{reduction}\\_\\texttt{factor}}
+        (\\frac{\\texttt{max}\\_\\texttt{resource}}{\\texttt{min}\\_\\texttt{resource}})) + 1`.
         Please set ``reduction_factor`` so that the number of brackets is not too large (about 4 –
         6 in most use cases). Please see Section 3.6 of the `original paper
         <http://www.jmlr.org/papers/volume18/16-558/16-558.pdf>`_ for the detail.
 
     Example:
 
         We minimize an objective function with Hyperband pruning algorithm.
@@ -139,15 +139,14 @@
     def __init__(
         self,
         min_resource: int = 1,
         max_resource: Union[str, int] = "auto",
         reduction_factor: int = 3,
         bootstrap_count: int = 0,
     ) -> None:
-
         self._min_resource = min_resource
         self._max_resource = max_resource
         self._reduction_factor = reduction_factor
         self._pruners: List[SuccessiveHalvingPruner] = []
         self._bootstrap_count = bootstrap_count
         self._total_trial_allocation_budget = 0
         self._trial_allocation_budgets: List[int] = []
@@ -259,30 +258,31 @@
         self, study: "optuna.study.Study", bracket_id: int
     ) -> "optuna.study.Study":
         # This class is assumed to be passed to
         # `SuccessiveHalvingPruner.prune` in which `get_trials`,
         # `direction`, and `storage` are used.
         # But for safety, prohibit the other attributes explicitly.
         class _BracketStudy(optuna.study.Study):
-
             _VALID_ATTRS = (
                 "get_trials",
+                "_get_trials",
                 "directions",
                 "direction",
                 "_directions",
                 "_storage",
                 "_study_id",
                 "pruner",
                 "study_name",
                 "_bracket_id",
                 "sampler",
                 "trials",
                 "_is_multi_objective",
                 "stop",
                 "_study",
+                "_thread_local",
             )
 
             def __init__(
                 self, study: "optuna.study.Study", pruner: HyperbandPruner, bracket_id: int
             ) -> None:
                 super().__init__(
                     study_name=study.study_name,
@@ -294,15 +294,15 @@
                 self._bracket_id = bracket_id
 
             def get_trials(
                 self,
                 deepcopy: bool = True,
                 states: Optional[Container[TrialState]] = None,
             ) -> List["optuna.trial.FrozenTrial"]:
-                trials = super().get_trials(deepcopy=deepcopy, states=states)
+                trials = super()._get_trials(deepcopy=deepcopy, states=states)
                 pruner = self.pruner
                 assert isinstance(pruner, HyperbandPruner)
                 return [t for t in trials if pruner._get_bracket_id(self, t) == self._bracket_id]
 
             def stop(self) -> None:
                 # `stop` should stop the original study's optimization loop instead of
                 # `_BracketStudy`.
```

### Comparing `optuna-3.1.1/optuna/pruners/_median.py` & `optuna-3.2.0/optuna/pruners/_median.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,11 +71,10 @@
         self,
         n_startup_trials: int = 5,
         n_warmup_steps: int = 0,
         interval_steps: int = 1,
         *,
         n_min_trials: int = 1,
     ) -> None:
-
         super().__init__(
             50.0, n_startup_trials, n_warmup_steps, interval_steps, n_min_trials=n_min_trials
         )
```

### Comparing `optuna-3.1.1/optuna/pruners/_nop.py` & `optuna-3.2.0/optuna/pruners/_nop.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,9 +40,8 @@
 
 
             study = optuna.create_study(direction="maximize", pruner=optuna.pruners.NopPruner())
             study.optimize(objective, n_trials=20)
     """
 
     def prune(self, study: "optuna.study.Study", trial: "optuna.trial.FrozenTrial") -> bool:
-
         return False
```

### Comparing `optuna-3.1.1/optuna/pruners/_patient.py` & `optuna-3.2.0/optuna/pruners/_patient.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             This value should be non-negative.
 
     """
 
     def __init__(
         self, wrapped_pruner: Optional[BasePruner], patience: int, min_delta: float = 0.0
     ) -> None:
-
         if patience < 0:
             raise ValueError(f"patience cannot be negative but got {patience}.")
 
         if min_delta < 0:
             raise ValueError(f"min_delta cannot be negative but got {min_delta}.")
 
         self._wrapped_pruner = wrapped_pruner
```

### Comparing `optuna-3.1.1/optuna/pruners/_percentile.py` & `optuna-3.2.0/optuna/pruners/_percentile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,27 @@
 from optuna.study._study_direction import StudyDirection
 from optuna.trial._state import TrialState
 
 
 def _get_best_intermediate_result_over_steps(
     trial: "optuna.trial.FrozenTrial", direction: StudyDirection
 ) -> float:
-
     values = np.asarray(list(trial.intermediate_values.values()), dtype=float)
     if direction == StudyDirection.MAXIMIZE:
         return np.nanmax(values)
     return np.nanmin(values)
 
 
 def _get_percentile_intermediate_result_over_trials(
     completed_trials: List["optuna.trial.FrozenTrial"],
     direction: StudyDirection,
     step: int,
     percentile: float,
     n_min_trials: int,
 ) -> float:
-
     if len(completed_trials) == 0:
         raise ValueError("No trials have been completed.")
 
     intermediate_values = [
         t.intermediate_values[step] for t in completed_trials if step in t.intermediate_values
     ]
 
@@ -49,15 +47,14 @@
         )
     )
 
 
 def _is_first_in_interval_step(
     step: int, intermediate_steps: KeysView[int], n_warmup_steps: int, interval_steps: int
 ) -> bool:
-
     nearest_lower_pruning_step = (
         step - n_warmup_steps
     ) // interval_steps * interval_steps + n_warmup_steps
     assert nearest_lower_pruning_step >= 0
 
     # `intermediate_steps` may not be sorted so we must go through all elements.
     second_last_step = functools.reduce(
@@ -140,15 +137,14 @@
         percentile: float,
         n_startup_trials: int = 5,
         n_warmup_steps: int = 0,
         interval_steps: int = 1,
         *,
         n_min_trials: int = 1,
     ) -> None:
-
         if not 0.0 <= percentile <= 100:
             raise ValueError(
                 "Percentile must be between 0 and 100 inclusive but got {}.".format(percentile)
             )
         if n_startup_trials < 0:
             raise ValueError(
                 "Number of startup trials cannot be negative but got {}.".format(n_startup_trials)
@@ -169,15 +165,14 @@
         self._percentile = percentile
         self._n_startup_trials = n_startup_trials
         self._n_warmup_steps = n_warmup_steps
         self._interval_steps = interval_steps
         self._n_min_trials = n_min_trials
 
     def prune(self, study: "optuna.study.Study", trial: "optuna.trial.FrozenTrial") -> bool:
-
         completed_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
         n_trials = len(completed_trials)
 
         if n_trials == 0:
             return False
 
         if n_trials < self._n_startup_trials:
```

### Comparing `optuna-3.1.1/optuna/pruners/_successive_halving.py` & `optuna-3.2.0/optuna/pruners/_successive_halving.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     `Asynchronous Successive Halving <http://arxiv.org/abs/1810.05934>`_ for detailed descriptions.
 
     Note that, this class does not take care of the parameter for the maximum
     resource, referred to as :math:`R` in the paper. The maximum resource allocated to a trial is
     typically limited inside the objective function (e.g., ``step`` number in `simple_pruning.py
     <https://github.com/optuna/optuna-examples/blob/main/simple_pruning.py>`_,
     ``EPOCH`` number in `chainer_integration.py
-    <https://github.com/optuna/optuna-examples/tree/main/chainer/chainer_integration.py#L77>`_).
+    <https://github.com/optuna/optuna-examples/tree/main/chainer/chainer_integration.py#L73>`_).
 
     .. seealso::
         Please refer to :meth:`~optuna.trial.Trial.report`.
 
     Example:
 
         We minimize an objective function with ``SuccessiveHalvingPruner``.
@@ -112,15 +112,14 @@
     def __init__(
         self,
         min_resource: Union[str, int] = "auto",
         reduction_factor: int = 4,
         min_early_stopping_rate: int = 0,
         bootstrap_count: int = 0,
     ) -> None:
-
         if isinstance(min_resource, str) and min_resource != "auto":
             raise ValueError(
                 "The value of `min_resource` is {}, "
                 "but must be either `min_resource` >= 1 or 'auto'".format(min_resource)
             )
 
         if isinstance(min_resource, int) and min_resource < 1:
@@ -157,15 +156,14 @@
         if isinstance(min_resource, int):
             self._min_resource = min_resource
         self._reduction_factor = reduction_factor
         self._min_early_stopping_rate = min_early_stopping_rate
         self._bootstrap_count = bootstrap_count
 
     def prune(self, study: "optuna.study.Study", trial: "optuna.trial.FrozenTrial") -> bool:
-
         step = trial.last_step
         if step is None:
             return False
 
         rung = _get_current_rung(trial)
         value = trial.intermediate_values[step]
         trials: Optional[List["optuna.trial.FrozenTrial"]] = None
@@ -210,57 +208,52 @@
             ):
                 return True
 
             rung += 1
 
 
 def _estimate_min_resource(trials: List["optuna.trial.FrozenTrial"]) -> Optional[int]:
-
     n_steps = [
         t.last_step for t in trials if t.state == TrialState.COMPLETE and t.last_step is not None
     ]
 
     if not n_steps:
         return None
 
     # Get the maximum number of steps and divide it by 100.
     last_step = max(n_steps)
     return max(last_step // 100, 1)
 
 
 def _get_current_rung(trial: "optuna.trial.FrozenTrial") -> int:
-
     # The following loop takes `O(log step)` iterations.
     rung = 0
     while _completed_rung_key(rung) in trial.system_attrs:
         rung += 1
     return rung
 
 
 def _completed_rung_key(rung: int) -> str:
-
     return "completed_rung_{}".format(rung)
 
 
 def _get_competing_values(
     trials: List["optuna.trial.FrozenTrial"], value: float, rung_key: str
 ) -> List[float]:
-
     competing_values = [t.system_attrs[rung_key] for t in trials if rung_key in t.system_attrs]
     competing_values.append(value)
     return competing_values
 
 
 def _is_trial_promotable_to_next_rung(
     value: float,
     competing_values: List[float],
     reduction_factor: int,
     study_direction: StudyDirection,
 ) -> bool:
-
     promotable_idx = (len(competing_values) // reduction_factor) - 1
 
     if promotable_idx == -1:
         # Optuna does not support suspending or resuming ongoing trials. Therefore, for the first
         # `eta - 1` trials, this implementation instead promotes the trial if its value is the
         # smallest one among the competing values.
         promotable_idx = 0
```

### Comparing `optuna-3.1.1/optuna/pruners/_threshold.py` & `optuna-3.2.0/optuna/pruners/_threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def __init__(
         self,
         lower: Optional[float] = None,
         upper: Optional[float] = None,
         n_warmup_steps: int = 0,
         interval_steps: int = 1,
     ) -> None:
-
         if lower is None and upper is None:
             raise TypeError("Either lower or upper must be specified.")
         if lower is not None:
             lower = _check_value(lower)
         if upper is not None:
             upper = _check_value(upper)
 
@@ -108,15 +107,14 @@
 
         self._lower = lower
         self._upper = upper
         self._n_warmup_steps = n_warmup_steps
         self._interval_steps = interval_steps
 
     def prune(self, study: "optuna.study.Study", trial: "optuna.trial.FrozenTrial") -> bool:
-
         step = trial.last_step
         if step is None:
             return False
 
         n_warmup_steps = self._n_warmup_steps
         if step < n_warmup_steps:
             return False
```

### Comparing `optuna-3.1.1/optuna/samplers/__init__.py` & `optuna-3.2.0/optuna/samplers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from optuna.samplers import nsgaii
 from optuna.samplers._base import BaseSampler
 from optuna.samplers._brute_force import BruteForceSampler
 from optuna.samplers._cmaes import CmaEsSampler
 from optuna.samplers._grid import GridSampler
+from optuna.samplers._nsgaiii import NSGAIIISampler
 from optuna.samplers._partial_fixed import PartialFixedSampler
 from optuna.samplers._qmc import QMCSampler
 from optuna.samplers._random import RandomSampler
 from optuna.samplers._search_space import intersection_search_space
 from optuna.samplers._search_space import IntersectionSearchSpace
 from optuna.samplers._tpe.multi_objective_sampler import MOTPESampler
 from optuna.samplers._tpe.sampler import TPESampler
@@ -17,14 +18,15 @@
     "BaseSampler",
     "BruteForceSampler",
     "CmaEsSampler",
     "GridSampler",
     "IntersectionSearchSpace",
     "MOTPESampler",
     "NSGAIISampler",
+    "NSGAIIISampler",
     "PartialFixedSampler",
     "QMCSampler",
     "RandomSampler",
     "TPESampler",
     "intersection_search_space",
     "nsgaii",
 ]
```

### Comparing `optuna-3.1.1/optuna/samplers/_base.py` & `optuna-3.2.0/optuna/samplers/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 
     *The independent sampling* determines a value of a single parameter without considering any
     relationship between parameters. Target parameters of the independent sampling are the
     parameters not described in the relative search space.
 
     More specifically, parameters are sampled by the following procedure.
     At the beginning of a trial, :meth:`~optuna.samplers.BaseSampler.infer_relative_search_space`
-    is called to determine the relative search space for the trial. Then,
-    :meth:`~optuna.samplers.BaseSampler.sample_relative` is invoked to sample parameters
-    from the relative search space. During the execution of the objective function,
+    is called to determine the relative search space for the trial.
+    During the execution of the objective function,
+    :meth:`~optuna.samplers.BaseSampler.sample_relative` is called only once
+    when sampling the parameters belonging to the relative search space for the first time.
     :meth:`~optuna.samplers.BaseSampler.sample_independent` is used to sample
     parameters that don't belong to the relative search space.
 
     The following figure depicts the lifetime of a trial and how the above three methods are
     called in the trial.
 
     .. image:: ../../../../image/sampling-sequence.png
@@ -67,15 +68,15 @@
                 Target trial object.
                 Take a copy before modifying this object.
 
         Returns:
             A dictionary containing the parameter names and parameter's distributions.
 
         .. seealso::
-            Please refer to :func:`~optuna.samplers.intersection_search_space` as an
+            Please refer to :func:`~optuna.search_space.intersection_search_space` as an
             implementation of :func:`~optuna.samplers.BaseSampler.infer_relative_search_space`.
         """
 
         raise NotImplementedError
 
     @abc.abstractmethod
     def sample_relative(
@@ -187,15 +188,14 @@
         same values. To prevent this issue, this method assigns a different seed to each random
         number generator.
         """
 
         pass
 
     def _raise_error_if_multi_objective(self, study: Study) -> None:
-
         if study._is_multi_objective():
             raise ValueError(
                 "If the study is being used for multi-objective optimization, "
                 f"{self.__class__.__name__} cannot be used."
             )
```

### Comparing `optuna-3.1.1/optuna/samplers/_brute_force.py` & `optuna-3.2.0/optuna/samplers/_partial_fixed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,116 @@
-import decimal
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Sequence
-
-import numpy as np
+import warnings
 
 from optuna._experimental import experimental_class
 from optuna.distributions import BaseDistribution
-from optuna.distributions import CategoricalDistribution
-from optuna.distributions import FloatDistribution
-from optuna.distributions import IntDistribution
 from optuna.samplers import BaseSampler
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
-@experimental_class("3.1.0")
-class BruteForceSampler(BaseSampler):
-    """Sampler using brute force.
-
-    This sampler performs exhaustive search on the defined search space.
+@experimental_class("2.4.0")
+class PartialFixedSampler(BaseSampler):
+    """Sampler with partially fixed parameters.
 
     Example:
 
+        After several steps of optimization, you can fix the value of ``y`` and re-optimize it.
+
         .. testcode::
 
             import optuna
 
 
             def objective(trial):
-                c = trial.suggest_categorical("c", ["float", "int"])
-                if c == "float":
-                    return trial.suggest_float("x", 1, 3, step=0.5)
-                elif c == "int":
-                    a = trial.suggest_int("a", 1, 3)
-                    b = trial.suggest_int("b", a, 3)
-                    return a + b
-
-
-            study = optuna.create_study(sampler=optuna.samplers.BruteForceSampler())
-            study.optimize(objective)
-
-    Note:
-        The defined search space must be finite. Therefore, when using
-        :class:`~optuna.distributions.FloatDistribution` or
-        :func:`~optuna.trial.Trial.suggest_float`, ``step=None`` is not allowed.
-
-    Note:
-        This sampler assumes that it suggests all parameters and that the search space is fixed.
-        For example, the sampler may fail to try the entire search space in the following cases.
+                x = trial.suggest_float("x", -1, 1)
+                y = trial.suggest_int("y", -1, 1)
+                return x**2 + y
+
+
+            study = optuna.create_study()
+            study.optimize(objective, n_trials=10)
+
+            best_params = study.best_params
+            fixed_params = {"y": best_params["y"]}
+            partial_sampler = optuna.samplers.PartialFixedSampler(fixed_params, study.sampler)
 
-        * Using with other samplers or :meth:`~optuna.study.Study.enqueue_trial`
-        * Changing suggestion ranges or adding parameters in the same :class:`~optuna.study.Study`
+            study.sampler = partial_sampler
+            study.optimize(objective, n_trials=10)
 
     Args:
-        seed:
-            A seed to fix the order of trials as the search order randomly shuffled. Please note
-            that it is not recommended using this option in distributed optimization settings since
-            this option cannot ensure the order of trials and may increase the number of duplicate
-            suggestions during distributed optimization.
+
+        fixed_params:
+            A dictionary of parameters to be fixed.
+
+        base_sampler:
+            A sampler which samples unfixed parameters.
+
     """
 
-    def __init__(self, seed: Optional[int] = None) -> None:
-        self._rng = np.random.RandomState(seed)
+    def __init__(self, fixed_params: Dict[str, Any], base_sampler: BaseSampler) -> None:
+        self._fixed_params = fixed_params
+        self._base_sampler = base_sampler
+
+    def reseed_rng(self) -> None:
+        self._base_sampler.reseed_rng()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, BaseDistribution]:
-        return {}
+        search_space = self._base_sampler.infer_relative_search_space(study, trial)
+
+        # Remove fixed params from relative search space to return fixed values.
+        for param_name in self._fixed_params.keys():
+            if param_name in search_space:
+                del search_space[param_name]
+
+        return search_space
 
     def sample_relative(
-        self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
+        self,
+        study: Study,
+        trial: FrozenTrial,
+        search_space: Dict[str, BaseDistribution],
     ) -> Dict[str, Any]:
-        return {}
+        # Fixed params are never sampled here.
+        return self._base_sampler.sample_relative(study, trial, search_space)
 
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-        candidates = _enumerate_candidates(param_distribution)
-        assert len(candidates) > 0
-
-        self._rng.shuffle(candidates)
-
-        for value in candidates[1:]:
-            params = trial.params.copy()
-            params[param_name] = value
-            study.enqueue_trial(params, skip_if_exists=True)
-
-        return candidates[0]
+        if param_name not in self._fixed_params:
+            # Unfixed params are sampled here.
+            return self._base_sampler.sample_independent(
+                study, trial, param_name, param_distribution
+            )
+        else:
+            # Fixed params are sampled here.
+            # Check if a parameter value is contained in the range of this distribution.
+            param_value = self._fixed_params[param_name]
+
+            param_value_in_internal_repr = param_distribution.to_internal_repr(param_value)
+            contained = param_distribution._contains(param_value_in_internal_repr)
+
+            if not contained:
+                warnings.warn(
+                    f"Fixed parameter '{param_name}' with value {param_value} is out of range "
+                    f"for distribution {param_distribution}."
+                )
+            return param_value
 
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
-        if len(study.get_trials(deepcopy=False, states=(TrialState.WAITING,))) == 0:
-            study.stop()
-
-
-def _enumerate_candidates(param_distribution: BaseDistribution) -> Sequence[Any]:
-    if isinstance(param_distribution, FloatDistribution):
-        if param_distribution.step is None:
-            raise ValueError(
-                "FloatDistribution.step must be given for BruteForceSampler"
-                " (otherwise, the search space will be infinite)."
-            )
-        low = decimal.Decimal(str(param_distribution.low))
-        high = decimal.Decimal(str(param_distribution.high))
-        step = decimal.Decimal(str(param_distribution.step))
-
-        ret = []
-        value = low
-        while value <= high:
-            ret.append(float(value))
-            value += step
-
-        return ret
-    elif isinstance(param_distribution, IntDistribution):
-        return list(
-            range(param_distribution.low, param_distribution.high + 1, param_distribution.step)
-        )
-    elif isinstance(param_distribution, CategoricalDistribution):
-        return list(param_distribution.choices)
-    else:
-        raise ValueError(f"Unknown distribution {param_distribution}.")
+        self._base_sampler.after_trial(study, trial, state, values)
```

### Comparing `optuna-3.1.1/optuna/samplers/_cmaes.py` & `optuna-3.2.0/optuna/samplers/_cmaes.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from optuna._imports import _LazyImport
 from optuna._transform import _SearchSpaceTransform
 from optuna.distributions import BaseDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.exceptions import ExperimentalWarning
 from optuna.samplers import BaseSampler
+from optuna.search_space import IntersectionSearchSpace
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 if TYPE_CHECKING:
     import cmaes
@@ -41,17 +42,22 @@
 
 _EPS = 1e-10
 # The value of system_attrs must be less than 2046 characters on RDBStorage.
 _SYSTEM_ATTR_MAX_LENGTH = 2045
 
 
 class _CmaEsAttrKeys(NamedTuple):
-    optimizer: str
-    n_restarts: str
+    optimizer: Callable[[int], str]
     generation: Callable[[int], str]
+    popsize: Callable[[], str]
+    n_restarts: Callable[[], str]
+    n_restarts_with_large: str
+    poptype: str
+    small_n_eval: str
+    large_n_eval: str
 
 
 class CmaEsSampler(BaseSampler):
     """A sampler using `cmaes <https://github.com/CyberAgentAILab/cmaes>`_ as the backend.
 
     Example:
 
@@ -88,14 +94,17 @@
 
     - `N. Hansen, The CMA Evolution Strategy: A Tutorial. arXiv:1604.00772, 2016.
       <https://arxiv.org/abs/1604.00772>`_
     - `A. Auger and N. Hansen. A restart CMA evolution strategy with increasing population
       size. In Proceedings of the IEEE Congress on Evolutionary Computation (CEC 2005),
       pages 1769–1776. IEEE Press, 2005.
       <http://www.cmap.polytechnique.fr/~nikolaus.hansen/cec2005ipopcmaes.pdf>`_
+    - `N. Hansen. Benchmarking a BI-Population CMA-ES on the BBOB-2009 Function Testbed.
+      GECCO Workshop, 2009.
+      <https://dl.acm.org/doi/10.1145/1570256.1570333>`_
     - `Raymond Ros, Nikolaus Hansen. A Simple Modification in CMA-ES Achieving Linear Time and
       Space Complexity. 10th International Conference on Parallel Problem Solving From Nature,
       Sep 2008, Dortmund, Germany. inria-00287367.
       <https://hal.inria.fr/inria-00287367/document>`_
     - `Masahiro Nomura, Shuhei Watanabe, Youhei Akimoto, Yoshihiko Ozaki, Masaki Onishi.
       Warm Starting CMA-ES for Hyperparameter Optimization, AAAI. 2021.
       <https://arxiv.org/abs/2012.06932>`_
@@ -128,15 +137,15 @@
             of trials finish in the same study.
 
         independent_sampler:
             A :class:`~optuna.samplers.BaseSampler` instance that is used for independent
             sampling. The parameters not contained in the relative search space are sampled
             by this sampler.
             The search space for :class:`~optuna.samplers.CmaEsSampler` is determined by
-            :func:`~optuna.samplers.intersection_search_space()`.
+            :func:`~optuna.search_space.intersection_search_space()`.
 
             If :obj:`None` is specified, :class:`~optuna.samplers.RandomSampler` is used
             as the default.
 
             .. seealso::
                 :class:`optuna.samplers` module provides built-in independent samplers
                 such as :class:`~optuna.samplers.RandomSampler` and
@@ -147,30 +156,34 @@
             the value of a parameter is sampled by using an independent sampler.
 
             Note that the parameters of the first trial in a study are always sampled
             via an independent sampler, so no warning messages are emitted in this case.
 
         restart_strategy:
             Strategy for restarting CMA-ES optimization when converges to a local minimum.
-            If given :obj:`None`, CMA-ES will not restart (default).
-            If given 'ipop', CMA-ES will restart with increasing population size.
+            If :obj:`None` is given, CMA-ES will not restart (default).
+            If 'ipop' is given, CMA-ES will restart with increasing population size.
+            if 'bipop' is given, CMA-ES will restart with the population size
+            increased or decreased.
             Please see also ``inc_popsize`` parameter.
 
             .. note::
                 Added in v2.1.0 as an experimental feature. The interface may change in newer
                 versions without prior notice. See
                 https://github.com/optuna/optuna/releases/tag/v2.1.0.
 
         popsize:
-            A population size of CMA-ES. When set ``restart_strategy = 'ipop'``, this is used
-            as the initial population size.
+            A population size of CMA-ES. When ``restart_strategy = 'ipop'``
+            or ``restart_strategy = 'bipop'`` is specified,
+            this is used as the initial population size.
 
         inc_popsize:
             Multiplier for increasing population size before each restart.
-            This argument will be used when setting ``restart_strategy = 'ipop'``.
+            This argument will be used when ``restart_strategy = 'ipop'``
+            or ``restart_strategy = 'bipop'`` is specified.
 
         consider_pruned_trials:
             If this is :obj:`True`, the PRUNED trials are considered for sampling.
 
             .. note::
                 Added in v2.0.0 as an experimental feature. The interface may change in newer
                 versions without prior notice. See
@@ -238,18 +251,18 @@
     ) -> None:
         self._x0 = x0
         self._sigma0 = sigma0
         self._independent_sampler = independent_sampler or optuna.samplers.RandomSampler(seed=seed)
         self._n_startup_trials = n_startup_trials
         self._warn_independent_sampling = warn_independent_sampling
         self._cma_rng = np.random.RandomState(seed)
-        self._search_space = optuna.samplers.IntersectionSearchSpace()
+        self._search_space = IntersectionSearchSpace()
         self._consider_pruned_trials = consider_pruned_trials
         self._restart_strategy = restart_strategy
-        self._popsize = popsize
+        self._initial_popsize = popsize
         self._inc_popsize = inc_popsize
         self._use_separable_cma = use_separable_cma
         self._with_margin = with_margin
         self._source_trials = source_trials
 
         if self._restart_strategy:
             warnings.warn(
@@ -294,23 +307,22 @@
 
         # TODO(c-bata): Support WS-sep-CMA-ES.
         if source_trials is not None and use_separable_cma:
             raise ValueError(
                 "It is prohibited to pass `source_trials` argument when using separable CMA-ES."
             )
 
-        # TODO(c-bata): Support BIPOP-CMA-ES.
         if restart_strategy not in (
             "ipop",
+            "bipop",
             None,
         ):
             raise ValueError(
-                "restart_strategy={} is unsupported. Please specify: 'ipop' or None.".format(
-                    restart_strategy
-                )
+                "restart_strategy={} is unsupported. "
+                "Please specify: 'ipop', 'bipop', or None.".format(restart_strategy)
             )
 
         # TODO(knshnb): Support sep-CMA-ES with margin.
         if self._use_separable_cma and self._with_margin:
             raise ValueError(
                 "Currently, we do not support `use_separable_cma=True` and `with_margin=True`."
             )
@@ -339,83 +351,137 @@
 
     def sample_relative(
         self,
         study: "optuna.Study",
         trial: "optuna.trial.FrozenTrial",
         search_space: Dict[str, BaseDistribution],
     ) -> Dict[str, Any]:
-
         self._raise_error_if_multi_objective(study)
 
         if len(search_space) == 0:
             return {}
 
         completed_trials = self._get_trials(study)
         if len(completed_trials) < self._n_startup_trials:
             return {}
 
         if len(search_space) == 1:
-            _logger.info(
-                "`CmaEsSampler` only supports two or more dimensional continuous "
-                "search space. `{}` is used instead of `CmaEsSampler`.".format(
-                    self._independent_sampler.__class__.__name__
+            if self._warn_independent_sampling:
+                _logger.warning(
+                    "`CmaEsSampler` only supports two or more dimensional continuous "
+                    "search space. `{}` is used instead of `CmaEsSampler`.".format(
+                        self._independent_sampler.__class__.__name__
+                    )
                 )
-            )
-            self._warn_independent_sampling = False
+                self._warn_independent_sampling = False
             return {}
 
         # When `with_margin=True`, bounds in discrete dimensions are handled inside `CMAwM`.
         trans = _SearchSpaceTransform(
             search_space, transform_step=not self._with_margin, transform_0_1=True
         )
 
-        optimizer, n_restarts = self._restore_optimizer(completed_trials)
+        if self._initial_popsize is None:
+            self._initial_popsize = 4 + math.floor(3 * math.log(len(trans.bounds)))
+
+        popsize: int = self._initial_popsize
+        n_restarts: int = 0
+        n_restarts_with_large: int = 0
+        poptype: str = "small"
+        small_n_eval: int = 0
+        large_n_eval: int = 0
+        if len(completed_trials) != 0:
+            latest_trial = completed_trials[-1]
+
+            popsize_attr_key = self._attr_keys.popsize()
+            if popsize_attr_key in latest_trial.system_attrs:
+                popsize = latest_trial.system_attrs[popsize_attr_key]
+            else:
+                popsize = self._initial_popsize
+
+            n_restarts_attr_key = self._attr_keys.n_restarts()
+            n_restarts = latest_trial.system_attrs.get(n_restarts_attr_key, 0)
+            n_restarts_with_large = latest_trial.system_attrs.get(
+                self._attr_keys.n_restarts_with_large, 0
+            )
+            poptype = latest_trial.system_attrs.get(self._attr_keys.poptype, "small")
+            small_n_eval = latest_trial.system_attrs.get(self._attr_keys.small_n_eval, 0)
+            large_n_eval = latest_trial.system_attrs.get(self._attr_keys.large_n_eval, 0)
+
+        optimizer = self._restore_optimizer(completed_trials, n_restarts)
         if optimizer is None:
-            n_restarts = 0
-            optimizer = self._init_optimizer(trans, study.direction, population_size=self._popsize)
+            optimizer = self._init_optimizer(
+                trans, study.direction, population_size=self._initial_popsize
+            )
 
         if optimizer.dim != len(trans.bounds):
-            _logger.info(
-                "`CmaEsSampler` does not support dynamic search space. "
-                "`{}` is used instead of `CmaEsSampler`.".format(
-                    self._independent_sampler.__class__.__name__
+            if self._warn_independent_sampling:
+                _logger.warning(
+                    "`CmaEsSampler` does not support dynamic search space. "
+                    "`{}` is used instead of `CmaEsSampler`.".format(
+                        self._independent_sampler.__class__.__name__
+                    )
                 )
-            )
-            self._warn_independent_sampling = False
+                self._warn_independent_sampling = False
             return {}
 
         # TODO(c-bata): Reduce the number of wasted trials during parallel optimization.
         # See https://github.com/optuna/optuna/pull/920#discussion_r385114002 for details.
         solution_trials = self._get_solution_trials(
             completed_trials, optimizer.generation, n_restarts
         )
 
-        if len(solution_trials) >= optimizer.population_size:
+        if len(solution_trials) >= popsize:
             solutions: List[Tuple[np.ndarray, float]] = []
-            for t in solution_trials[: optimizer.population_size]:
+            for t in solution_trials[:popsize]:
                 assert t.value is not None, "completed trials must have a value"
                 if isinstance(optimizer, cmaes.CMAwM):
                     x = np.array(t.system_attrs["x_for_tell"])
                 else:
                     x = trans.transform(t.params)
                 y = t.value if study.direction == StudyDirection.MINIMIZE else -t.value
                 solutions.append((x, y))
 
             optimizer.tell(solutions)
 
             if self._restart_strategy == "ipop" and optimizer.should_stop():
                 n_restarts += 1
-                popsize = optimizer.population_size * self._inc_popsize
+                popsize = popsize * self._inc_popsize
+                optimizer = self._init_optimizer(
+                    trans, study.direction, population_size=popsize, randomize_start_point=True
+                )
+
+            if self._restart_strategy == "bipop" and optimizer.should_stop():
+                n_restarts += 1
+
+                n_eval = popsize * optimizer.generation
+                if poptype == "small":
+                    small_n_eval += n_eval
+                else:  # poptype == "large"
+                    large_n_eval += n_eval
+
+                if small_n_eval < large_n_eval:
+                    poptype = "small"
+                    popsize_multiplier = self._inc_popsize**n_restarts_with_large
+                    popsize = math.floor(
+                        self._initial_popsize
+                        * popsize_multiplier ** (self._cma_rng.uniform() ** 2)
+                    )
+                else:
+                    poptype = "large"
+                    n_restarts_with_large += 1
+                    popsize = self._initial_popsize * (self._inc_popsize**n_restarts_with_large)
+
                 optimizer = self._init_optimizer(
                     trans, study.direction, population_size=popsize, randomize_start_point=True
                 )
 
             # Store optimizer.
             optimizer_str = pickle.dumps(optimizer).hex()
-            optimizer_attrs = self._split_optimizer_str(optimizer_str)
+            optimizer_attrs = self._split_optimizer_str(optimizer_str, n_restarts)
             for key in optimizer_attrs:
                 study._storage.set_trial_system_attr(trial._trial_id, key, optimizer_attrs[key])
 
         # Caution: optimizer should update its seed value.
         seed = self._cma_rng.randint(1, 2**16) + trial.number
         optimizer._rng.seed(seed)
         if isinstance(optimizer, cmaes.CMAwM):
@@ -426,77 +492,116 @@
         else:
             params = optimizer.ask()
 
         generation_attr_key = self._attr_keys.generation(n_restarts)
         study._storage.set_trial_system_attr(
             trial._trial_id, generation_attr_key, optimizer.generation
         )
+        popsize_attr_key = self._attr_keys.popsize()
+        study._storage.set_trial_system_attr(trial._trial_id, popsize_attr_key, popsize)
+        n_restarts_attr_key = self._attr_keys.n_restarts()
+        study._storage.set_trial_system_attr(trial._trial_id, n_restarts_attr_key, n_restarts)
+        study._storage.set_trial_system_attr(
+            trial._trial_id, self._attr_keys.n_restarts_with_large, n_restarts_with_large
+        )
+        study._storage.set_trial_system_attr(trial._trial_id, self._attr_keys.poptype, poptype)
         study._storage.set_trial_system_attr(
-            trial._trial_id, self._attr_keys.n_restarts, n_restarts
+            trial._trial_id, self._attr_keys.small_n_eval, small_n_eval
+        )
+        study._storage.set_trial_system_attr(
+            trial._trial_id, self._attr_keys.large_n_eval, large_n_eval
         )
 
         external_values = trans.untransform(params)
 
         return external_values
 
     @property
     def _attr_keys(self) -> _CmaEsAttrKeys:
-
         if self._use_separable_cma:
             attr_prefix = "sepcma:"
         elif self._with_margin:
             attr_prefix = "cmawm:"
         else:
             attr_prefix = "cma:"
 
+        def optimizer_key_template(restart: int) -> str:
+            if self._restart_strategy is None:
+                return attr_prefix + "optimizer"
+            else:
+                return attr_prefix + "{}:restart_{}:optimizer".format(
+                    self._restart_strategy, restart
+                )
+
         def generation_attr_key_template(restart: int) -> str:
             if self._restart_strategy is None:
                 return attr_prefix + "generation"
             else:
-                return attr_prefix + "restart_{}:generation".format(restart)
+                return attr_prefix + "{}:restart_{}:generation".format(
+                    self._restart_strategy, restart
+                )
+
+        def popsize_attr_key_template() -> str:
+            if self._restart_strategy is None:
+                return attr_prefix + "popsize"
+            else:
+                return attr_prefix + "{}:popsize".format(self._restart_strategy)
+
+        def n_restarts_attr_key_template() -> str:
+            if self._restart_strategy is None:
+                return attr_prefix + "n_restarts"
+            else:
+                return attr_prefix + "{}:n_restarts".format(self._restart_strategy)
 
         return _CmaEsAttrKeys(
-            attr_prefix + "optimizer",
-            attr_prefix + "n_restarts",
+            optimizer_key_template,
             generation_attr_key_template,
+            popsize_attr_key_template,
+            n_restarts_attr_key_template,
+            attr_prefix + "n_restarts_with_large",
+            attr_prefix + "poptype",
+            attr_prefix + "small_n_eval",
+            attr_prefix + "large_n_eval",
         )
 
-    def _concat_optimizer_attrs(self, optimizer_attrs: Dict[str, str]) -> str:
+    def _concat_optimizer_attrs(self, optimizer_attrs: Dict[str, str], n_restarts: int = 0) -> str:
         return "".join(
-            optimizer_attrs["{}:{}".format(self._attr_keys.optimizer, i)]
+            optimizer_attrs["{}:{}".format(self._attr_keys.optimizer(n_restarts), i)]
             for i in range(len(optimizer_attrs))
         )
 
-    def _split_optimizer_str(self, optimizer_str: str) -> Dict[str, str]:
+    def _split_optimizer_str(self, optimizer_str: str, n_restarts: int = 0) -> Dict[str, str]:
         optimizer_len = len(optimizer_str)
         attrs = {}
         for i in range(math.ceil(optimizer_len / _SYSTEM_ATTR_MAX_LENGTH)):
             start = i * _SYSTEM_ATTR_MAX_LENGTH
             end = min((i + 1) * _SYSTEM_ATTR_MAX_LENGTH, optimizer_len)
-            attrs["{}:{}".format(self._attr_keys.optimizer, i)] = optimizer_str[start:end]
+            attrs["{}:{}".format(self._attr_keys.optimizer(n_restarts), i)] = optimizer_str[
+                start:end
+            ]
         return attrs
 
     def _restore_optimizer(
         self,
         completed_trials: "List[optuna.trial.FrozenTrial]",
-    ) -> Tuple[Optional["CmaClass"], int]:
+        n_restarts: int = 0,
+    ) -> Optional["CmaClass"]:
         # Restore a previous CMA object.
         for trial in reversed(completed_trials):
             optimizer_attrs = {
                 key: value
                 for key, value in trial.system_attrs.items()
-                if key.startswith(self._attr_keys.optimizer)
+                if key.startswith(self._attr_keys.optimizer(n_restarts))
             }
             if len(optimizer_attrs) == 0:
                 continue
 
-            optimizer_str = self._concat_optimizer_attrs(optimizer_attrs)
-            n_restarts: int = trial.system_attrs.get(self._attr_keys.n_restarts, 0)
-            return pickle.loads(bytes.fromhex(optimizer_str)), n_restarts
-        return None, 0
+            optimizer_str = self._concat_optimizer_attrs(optimizer_attrs, n_restarts)
+            return pickle.loads(bytes.fromhex(optimizer_str))
+        return None
 
     def _init_optimizer(
         self,
         trans: _SearchSpaceTransform,
         direction: StudyDirection,
         population_size: Optional[int] = None,
         randomize_start_point: bool = False,
@@ -555,15 +660,20 @@
             )
 
         if self._with_margin:
             steps = np.empty(len(trans._search_space), dtype=float)
             for i, dist in enumerate(trans._search_space.values()):
                 assert isinstance(dist, (IntDistribution, FloatDistribution))
                 # Set step 0.0 for continuous search space.
-                steps[i] = dist.step or 0.0
+                if dist.step is None or dist.log:
+                    steps[i] = 0.0
+                elif dist.low == dist.high:
+                    steps[i] = 1.0
+                else:
+                    steps[i] = dist.step / (dist.high - dist.low)
 
             return cmaes.CMAwM(
                 mean=mean,
                 sigma=sigma0,
                 bounds=trans.bounds,
                 steps=steps,
                 cov=cov,
@@ -585,15 +695,14 @@
     def sample_independent(
         self,
         study: "optuna.Study",
         trial: "optuna.trial.FrozenTrial",
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-
         self._raise_error_if_multi_objective(study)
 
         if self._warn_independent_sampling:
             complete_trials = self._get_trials(study)
             if len(complete_trials) >= self._n_startup_trials:
                 self._log_independent_sampling(trial, param_name)
 
@@ -612,15 +721,15 @@
             "if this independent sampling is intended behavior.".format(
                 param_name, trial.number, self._independent_sampler.__class__.__name__
             )
         )
 
     def _get_trials(self, study: "optuna.Study") -> List[FrozenTrial]:
         complete_trials = []
-        for t in study.get_trials(deepcopy=False):
+        for t in study._get_trials(deepcopy=False, use_cache=True):
             if t.state == TrialState.COMPLETE:
                 complete_trials.append(t)
             elif (
                 t.state == TrialState.PRUNED
                 and len(t.intermediate_values) > 0
                 and self._consider_pruned_trials
             ):
@@ -642,15 +751,14 @@
     def after_trial(
         self,
         study: "optuna.Study",
         trial: "optuna.trial.FrozenTrial",
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
-
         self._independent_sampler.after_trial(study, trial, state, values)
 
 
 def _is_compatible_search_space(
     trans: _SearchSpaceTransform, search_space: Dict[str, BaseDistribution]
 ) -> bool:
     intersection_size = len(set(trans._search_space.keys()).intersection(search_space.keys()))
```

### Comparing `optuna-3.1.1/optuna/samplers/_grid.py` & `optuna-3.2.0/optuna/samplers/_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,41 +98,33 @@
             this option cannot ensure the order of trials and may increase the number of duplicate
             suggestions during distributed optimization.
     """
 
     def __init__(
         self, search_space: Mapping[str, Sequence[GridValueType]], seed: Optional[int] = None
     ) -> None:
-
         for param_name, param_values in search_space.items():
             for value in param_values:
                 self._check_value(param_name, value)
 
         self._search_space = collections.OrderedDict()
         for param_name, param_values in sorted(search_space.items()):
             self._search_space[param_name] = list(param_values)
 
         self._all_grids = list(itertools.product(*self._search_space.values()))
         self._param_names = sorted(search_space.keys())
         self._n_min_trials = len(self._all_grids)
         self._rng = np.random.RandomState(seed)
 
     def reseed_rng(self) -> None:
-
         self._rng.seed()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, BaseDistribution]:
-
-        return {}
-
-    def sample_relative(
-        self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
-    ) -> Dict[str, Any]:
         # Instead of returning param values, GridSampler puts the target grid id as a system attr,
         # and the values are returned from `sample_independent`. This is because the distribution
         # object is hard to get at the beginning of trial, while we need the access to the object
         # to validate the sampled value.
 
         # When the trial is created by RetryFailedTrialCallback or enqueue_trial, we should not
         # assign a new grid_id.
@@ -160,22 +152,26 @@
         grid_id = int(self._rng.choice(target_grids))
 
         study._storage.set_trial_system_attr(trial._trial_id, "search_space", self._search_space)
         study._storage.set_trial_system_attr(trial._trial_id, "grid_id", grid_id)
 
         return {}
 
+    def sample_relative(
+        self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
+    ) -> Dict[str, Any]:
+        return {}
+
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-
         if "grid_id" not in trial.system_attrs:
             message = "All parameters must be specified when using GridSampler with enqueue_trial."
             raise ValueError(message)
 
         if param_name not in self._search_space:
             message = "The parameter name, {}, is not found in the given grid.".format(param_name)
             raise ValueError(message)
@@ -208,27 +204,25 @@
         elif len(target_grids) == 1:
             grid_id = study._storage.get_trial_system_attrs(trial._trial_id)["grid_id"]
             if grid_id == target_grids[0]:
                 study.stop()
 
     @staticmethod
     def _check_value(param_name: str, param_value: Any) -> None:
-
         if param_value is None or isinstance(param_value, (str, int, float, bool)):
             return
 
         message = (
             "{} contains a value with the type of {}, which is not supported by "
             "`GridSampler`. Please make sure a value is `str`, `int`, `float`, `bool`"
             " or `None` for persistent storage.".format(param_name, type(param_value))
         )
         warnings.warn(message)
 
     def _get_unvisited_grid_ids(self, study: Study) -> List[int]:
-
         # List up unvisited grids based on already finished ones.
         visited_grids = []
         running_grids = []
 
         # We directly query the storage to get trials here instead of `study.get_trials`,
         # since some pruners such as `HyperbandPruner` use the study transformed
         # to filter trials. See https://github.com/optuna/optuna/issues/2327 for details.
@@ -255,15 +249,14 @@
     @staticmethod
     def _grid_value_equal(value1: GridValueType, value2: GridValueType) -> bool:
         value1_is_nan = isinstance(value1, Real) and np.isnan(float(value1))
         value2_is_nan = isinstance(value2, Real) and np.isnan(float(value2))
         return (value1 == value2) or (value1_is_nan and value2_is_nan)
 
     def _same_search_space(self, search_space: Mapping[str, Sequence[GridValueType]]) -> bool:
-
         if set(search_space.keys()) != set(self._search_space.keys()):
             return False
 
         for param_name in search_space.keys():
             if len(search_space[param_name]) != len(self._search_space[param_name]):
                 return False
```

### Comparing `optuna-3.1.1/optuna/samplers/_qmc.py` & `optuna-3.2.0/optuna/samplers/_qmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 @experimental_class("3.0.0")
 class QMCSampler(BaseSampler):
     """A Quasi Monte Carlo Sampler that generates low-discrepancy sequences.
 
     Quasi Monte Carlo (QMC) sequences are designed to have lower discrepancies than
     standard random sequences. They are known to perform better than the standard
-    randam sequences in hyperparameter optimization.
+    random sequences in hyperparameter optimization.
 
     For further information about the use of QMC sequences for hyperparameter optimization,
     please refer to the following paper:
 
     - `Bergstra, James, and Yoshua Bengio. Random search for hyper-parameter optimization.
       Journal of machine learning research 13.2, 2012.
       <https://jmlr.org/papers/v13/bergstra12a.html>`_
@@ -147,17 +147,16 @@
         qmc_type: str = "sobol",
         scramble: bool = False,  # default is False for simplicity in distributed environment.
         seed: Optional[int] = None,
         independent_sampler: Optional[BaseSampler] = None,
         warn_asynchronous_seeding: bool = True,
         warn_independent_sampling: bool = True,
     ) -> None:
-
         self._scramble = scramble
-        self._seed = seed or np.random.PCG64().random_raw()
+        self._seed = np.random.PCG64().random_raw() if seed is None else seed
         self._independent_sampler = independent_sampler or optuna.samplers.RandomSampler(seed=seed)
         self._initial_search_space: Optional[Dict[str, BaseDistribution]] = None
         self._warn_independent_sampling = warn_independent_sampling
 
         if qmc_type in ("halton", "sobol"):
             self._qmc_type = qmc_type
         else:
@@ -168,41 +167,38 @@
             raise ValueError(message)
 
         if seed is None and scramble and warn_asynchronous_seeding:
             # Sobol/Halton sequences without scrambling do not use seed.
             self._log_asynchronous_seeding()
 
     def reseed_rng(self) -> None:
-
         # We must not reseed the `self._seed` like below. Otherwise, workers will have different
         # seed under parallel execution because `self.reseed_rng()` is called when starting each
         # parallel executor.
         # >>> self._seed = np.random.MT19937().random_raw()
 
         self._independent_sampler.reseed_rng()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, BaseDistribution]:
-
         if self._initial_search_space is not None:
             return self._initial_search_space
 
-        past_trials = study.get_trials(deepcopy=False, states=_SUGGESTED_STATES)
+        past_trials = study._get_trials(deepcopy=False, states=_SUGGESTED_STATES, use_cache=True)
         # The initial trial is sampled by the independent sampler.
         if len(past_trials) == 0:
             return {}
         # If an initial trial was already made,
         # construct search_space of this sampler from the initial trial.
         first_trial = min(past_trials, key=lambda t: t.number)
         self._initial_search_space = self._infer_initial_search_space(first_trial)
         return self._initial_search_space
 
     def _infer_initial_search_space(self, trial: FrozenTrial) -> Dict[str, BaseDistribution]:
-
         search_space: Dict[str, BaseDistribution] = {}
         for param_name, distribution in trial.distributions.items():
             if isinstance(distribution, CategoricalDistribution):
                 continue
             search_space[param_name] = distribution
 
         return search_space
@@ -230,27 +226,25 @@
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-
         if self._initial_search_space is not None:
             if self._warn_independent_sampling:
                 self._log_independent_sampling(trial, param_name)
 
         return self._independent_sampler.sample_independent(
             study, trial, param_name, param_distribution
         )
 
     def sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, Any]:
-
         if search_space == {}:
             return {}
 
         sample = self._sample_qmc(study, search_space)
         trans = _SearchSpaceTransform(search_space)
         sample = trans.bounds[:, 0] + sample * (trans.bounds[:, 1] - trans.bounds[:, 0])
         return trans.untransform(sample[0, :])
@@ -261,15 +255,14 @@
         trial: "optuna.trial.FrozenTrial",
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
         self._independent_sampler.after_trial(study, trial, state, values)
 
     def _sample_qmc(self, study: Study, search_space: Dict[str, BaseDistribution]) -> np.ndarray:
-
         # Lazy import because the `scipy.stats.qmc` is slow to import.
         qmc_module = _LazyImport("scipy.stats.qmc")
 
         sample_id = self._find_sample_id(study)
         d = len(search_space)
 
         if self._qmc_type == "halton":
@@ -285,15 +278,14 @@
         if forward_size > 0:
             qmc_engine.fast_forward(forward_size)
         sample = qmc_engine.random(1)
 
         return sample
 
     def _find_sample_id(self, study: Study) -> int:
-
         qmc_id = ""
         qmc_id += self._qmc_type
         # Sobol/Halton sequences without scrambling do not use seed.
         if self._scramble:
             qmc_id += f" (scramble=True, seed={self._seed})"
         else:
             qmc_id += " (scramble=False)"
```

### Comparing `optuna-3.1.1/optuna/samplers/_random.py` & `optuna-3.2.0/optuna/samplers/_random.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,39 +35,34 @@
             study.optimize(objective, n_trials=10)
 
     Args:
         seed: Seed for random number generator.
     """
 
     def __init__(self, seed: Optional[int] = None) -> None:
-
         self._rng = numpy.random.RandomState(seed)
 
     def reseed_rng(self) -> None:
-
         self._rng.seed()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, BaseDistribution]:
-
         return {}
 
     def sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, Any]:
-
         return {}
 
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: distributions.BaseDistribution,
     ) -> Any:
-
         search_space = {param_name: param_distribution}
         trans = _SearchSpaceTransform(search_space)
         trans_params = self._rng.uniform(trans.bounds[:, 0], trans.bounds[:, 1])
 
         return trans.untransform(trans_params)[param_name]
```

### Comparing `optuna-3.1.1/optuna/samplers/_search_space/group_decomposed.py` & `optuna-3.2.0/optuna/search_space/group_decomposed.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,11 +52,11 @@
 
         states_of_interest: Tuple[TrialState, ...]
         if self._include_pruned:
             states_of_interest = (TrialState.COMPLETE, TrialState.PRUNED)
         else:
             states_of_interest = (TrialState.COMPLETE,)
 
-        for trial in study.get_trials(deepcopy=False, states=states_of_interest):
+        for trial in study._get_trials(deepcopy=False, states=states_of_interest, use_cache=False):
             self._search_space.add_distributions(trial.distributions)
 
         return copy.deepcopy(self._search_space)
```

### Comparing `optuna-3.1.1/optuna/samplers/_search_space/intersection.py` & `optuna-3.2.0/optuna/samplers/_search_space/intersection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from collections import OrderedDict
 import copy
 from typing import Dict
 from typing import Optional
 
 import optuna
+from optuna._deprecated import deprecated_class
+from optuna._deprecated import deprecated_func
 from optuna.distributions import BaseDistribution
 from optuna.study import Study
 
 
+@deprecated_class(
+    "3.2.0",
+    "4.0.0",
+    name="optuna.samplers.IntersectionSearchSpace",
+    text="Please use optuna.search_space.IntersectionSearchSpace instead.",
+)
 class IntersectionSearchSpace:
     """A class to calculate the intersection search space of a :class:`~optuna.study.Study`.
 
     Intersection search space contains the intersection of parameter distributions that have been
     suggested in the completed trials of the study so far.
     If there are multiple parameters that have the same name but different distributions,
     neither is included in the resulting search space
@@ -64,15 +72,15 @@
             optuna.trial.TrialState.WAITING,
             optuna.trial.TrialState.RUNNING,
         ]
 
         if self._include_pruned:
             states_of_interest.append(optuna.trial.TrialState.PRUNED)
 
-        trials = study.get_trials(deepcopy=False, states=states_of_interest)
+        trials = study._get_trials(deepcopy=False, states=states_of_interest, use_cache=False)
 
         next_cursor = trials[-1].number + 1 if len(trials) > 0 else -1
         for trial in reversed(trials):
             if self._cursor > trial.number:
                 break
 
             if not trial.state.is_finished():
@@ -94,14 +102,20 @@
 
         if ordered_dict:
             search_space = OrderedDict(sorted(search_space.items(), key=lambda x: x[0]))
 
         return copy.deepcopy(search_space)
 
 
+@deprecated_func(
+    "3.2.0",
+    "4.0.0",
+    name="optuna.samplers.intersection_search_space",
+    text="Please use optuna.search_space.intersection_search_space instead.",
+)
 def intersection_search_space(
     study: Study, ordered_dict: bool = False, include_pruned: bool = False
 ) -> Dict[str, BaseDistribution]:
     """Return the intersection search space of the :class:`~optuna.study.Study`.
 
     Intersection search space contains the intersection of parameter distributions that have been
     suggested in the completed trials of the study so far.
```

### Comparing `optuna-3.1.1/optuna/samplers/_tpe/_erf.py` & `optuna-3.2.0/optuna/samplers/_tpe/_erf.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #  * Permission to use, copy, modify, and distribute this
 #  * software is freely granted, provided that this notice
 #  * is preserved.
 #  * ====================================================
 #  */
 
 import numpy as np
+from numpy.polynomial import Polynomial
 
 
 half = 0.5
 one = 1
 two = 2
 
 erx = 8.45062911510467529297e-01
@@ -110,49 +111,53 @@
     case_big = a >= 6
 
     def calc_case_tiny(x: np.ndarray) -> np.ndarray:
         return x + efx * x
 
     def calc_case_small1(x: np.ndarray) -> np.ndarray:
         z = x * x
-        r = pp0 + z * (pp1 + z * (pp2 + z * (pp3 + z * pp4)))
-        s = one + z * (qq1 + z * (qq2 + z * (qq3 + z * (qq4 + z * qq5))))
+        r = Polynomial([pp0, pp1, pp2, pp3, pp4])(z)  # type: ignore[no-untyped-call]
+        s = Polynomial([one, qq1, qq2, qq3, qq4, qq5])(z)  # type: ignore[no-untyped-call]
         y = r / s
         return x + x * y
 
     def calc_case_small2(x: np.ndarray) -> np.ndarray:
         s = np.abs(x) - one
-        P = pa0 + s * (pa1 + s * (pa2 + s * (pa3 + s * (pa4 + s * (pa5 + s * pa6)))))
-        Q = one + s * (qa1 + s * (qa2 + s * (qa3 + s * (qa4 + s * (qa5 + s * qa6)))))
+        P = Polynomial([pa0, pa1, pa2, pa3, pa4, pa5, pa6])(s)  # type: ignore[no-untyped-call]
+        Q = Polynomial([one, qa1, qa2, qa3, qa4, qa5, qa6])(s)  # type: ignore[no-untyped-call]
         absout = erx + P / Q
         return absout * np.sign(x)
 
     def calc_case_med1(x: np.ndarray) -> np.ndarray:
         sign = np.sign(x)
         x = np.abs(x)
         s = one / (x * x)
-        R = ra0 + s * (ra1 + s * (ra2 + s * (ra3 + s * (ra4 + s * (ra5 + s * (ra6 + s * ra7))))))
-        S = one + s * (
-            sa1 + s * (sa2 + s * (sa3 + s * (sa4 + s * (sa5 + s * (sa6 + s * (sa7 + s * sa8))))))
+        R = Polynomial([ra0, ra1, ra2, ra3, ra4, ra5, ra6, ra7])(  # type: ignore[no-untyped-call]
+            s
         )
+        S = Polynomial(  # type: ignore[no-untyped-call]
+            [one, sa1, sa2, sa3, sa4, sa5, sa6, sa7, sa8]
+        )(s)
         # the following 3 lines are omitted for the following reasons:
         # (1) there are no easy way to implement SET_LOW_WORD equivalent method in NumPy
         # (2) we don't need very high accuracy in our use case.
         # z = x
         # SET_LOW_WORD(z, 0)
         # r = np.exp(-z * z - 0.5625) * np.exp((z - x) * (z + x) + R / S)
         r = np.exp(-x * x - 0.5625) * np.exp(R / S)
         return (one - r / x) * sign
 
     def calc_case_med2(x: np.ndarray) -> np.ndarray:
         sign = np.sign(x)
         x = np.abs(x)
         s = one / (x * x)
-        R = rb0 + s * (rb1 + s * (rb2 + s * (rb3 + s * (rb4 + s * (rb5 + s * rb6)))))
-        S = one + s * (sb1 + s * (sb2 + s * (sb3 + s * (sb4 + s * (sb5 + s * (sb6 + s * sb7))))))
+        R = Polynomial([rb0, rb1, rb2, rb3, rb4, rb5, rb6])(s)  # type: ignore[no-untyped-call]
+        S = Polynomial([one, sb1, sb2, sb3, sb4, sb5, sb6, sb7])(  # type: ignore[no-untyped-call]
+            s
+        )
         # z = x
         # SET_LOW_WORD(z, 0)
         # r = np.exp(-z * z - 0.5625) * np.exp((z - x) * (z + x) + R / S)
         r = np.exp(-x * x - 0.5625) * np.exp(R / S)
         return (one - r / x) * sign
 
     def calc_case_big(x: np.ndarray) -> np.ndarray:
```

### Comparing `optuna-3.1.1/optuna/samplers/_tpe/_truncnorm.py` & `optuna-3.2.0/optuna/samplers/_tpe/_truncnorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,18 +203,18 @@
 
 
 def rvs(
     a: np.ndarray,
     b: np.ndarray,
     loc: Union[np.ndarray, float] = 0,
     scale: Union[np.ndarray, float] = 1,
-    size: int = 1,
     random_state: Optional[np.random.RandomState] = None,
 ) -> np.ndarray:
     random_state = random_state or np.random.RandomState()
+    size = np.broadcast(a, b, loc, scale).shape
     percentiles = random_state.uniform(low=0, high=1, size=size)
     return ppf(percentiles, a, b) * scale + loc
 
 
 def logpdf(
     x: np.ndarray,
     a: Union[np.ndarray, float],
```

### Comparing `optuna-3.1.1/optuna/samplers/_tpe/multi_objective_sampler.py` & `optuna-3.2.0/optuna/samplers/_tpe/multi_objective_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
         consider_endpoints: bool = True,
         n_startup_trials: int = 10,
         n_ehvi_candidates: int = 24,
         gamma: Callable[[int], int] = default_gamma,
         weights_above: Callable[[int], np.ndarray] = _default_weights_above,
         seed: Optional[int] = None,
     ) -> None:
-
         super().__init__(
             consider_prior=consider_prior,
             prior_weight=prior_weight,
             consider_magic_clip=consider_magic_clip,
             consider_endpoints=consider_endpoints,
             n_startup_trials=n_startup_trials,
             n_ei_candidates=n_ehvi_candidates,
```

### Comparing `optuna-3.1.1/optuna/samplers/_tpe/sampler.py` & `optuna-3.2.0/optuna/samplers/_tpe/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,41 +17,38 @@
 from optuna.distributions import BaseDistribution
 from optuna.exceptions import ExperimentalWarning
 from optuna.logging import get_logger
 from optuna.samplers._base import _CONSTRAINTS_KEY
 from optuna.samplers._base import _process_constraints_after_trial
 from optuna.samplers._base import BaseSampler
 from optuna.samplers._random import RandomSampler
-from optuna.samplers._search_space import IntersectionSearchSpace
-from optuna.samplers._search_space.group_decomposed import _GroupDecomposedSearchSpace
-from optuna.samplers._search_space.group_decomposed import _SearchSpaceGroup
 from optuna.samplers._tpe.parzen_estimator import _ParzenEstimator
 from optuna.samplers._tpe.parzen_estimator import _ParzenEstimatorParameters
+from optuna.search_space import IntersectionSearchSpace
+from optuna.search_space.group_decomposed import _GroupDecomposedSearchSpace
+from optuna.search_space.group_decomposed import _SearchSpaceGroup
 from optuna.study import Study
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 EPS = 1e-12
 _logger = get_logger(__name__)
 
 
 def default_gamma(x: int) -> int:
-
     return min(int(np.ceil(0.1 * x)), 25)
 
 
 def hyperopt_default_gamma(x: int) -> int:
-
     return min(int(np.ceil(0.25 * np.sqrt(x))), 25)
 
 
 def default_weights(x: int) -> np.ndarray:
-
     if x == 0:
         return np.asarray([])
     elif x < 25:
         return np.ones(x)
     else:
         ramp = np.linspace(1.0 / x, 1.0, num=x - 25)
         flat = np.ones(25)
@@ -247,15 +244,14 @@
         *,
         multivariate: bool = False,
         group: bool = False,
         warn_independent_sampling: bool = True,
         constant_liar: bool = False,
         constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
     ) -> None:
-
         self._parzen_estimator_parameters = _ParzenEstimatorParameters(
             consider_prior,
             prior_weight,
             consider_magic_clip,
             consider_endpoints,
             weights,
             multivariate,
@@ -308,22 +304,20 @@
             warnings.warn(
                 "The ``constraints_func`` option is an experimental feature."
                 " The interface can change in the future.",
                 ExperimentalWarning,
             )
 
     def reseed_rng(self) -> None:
-
         self._rng.seed()
         self._random_sampler.reseed_rng()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
     ) -> Dict[str, BaseDistribution]:
-
         if not self._multivariate:
             return {}
 
         search_space: Dict[str, BaseDistribution] = {}
 
         if self._group:
             assert self._group_decomposed_search_space is not None
@@ -357,15 +351,14 @@
                     "to `False` in the constructor of `TPESampler`, "
                     "if this independent sampling is intended behavior."
                 )
 
     def sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, Any]:
-
         if self._group:
             assert self._search_space_group is not None
             params = {}
             for sub_space in self._search_space_group.search_spaces:
                 search_space = {}
                 # Sort keys because Python's string hashing is nondeterministic.
                 for name, distribution in sorted(sub_space.items()):
@@ -375,15 +368,14 @@
             return params
         else:
             return self._sample_relative(study, trial, search_space)
 
     def _sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, Any]:
-
         if search_space == {}:
             return {}
 
         param_names = list(search_space.keys())
         values, scores, violations = _get_observation_pairs(
             study,
             param_names,
@@ -431,15 +423,14 @@
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-
         values, scores, violations = _get_observation_pairs(
             study,
             [param_name],
             self._constant_liar,
             self._constraints_func is not None,
         )
 
@@ -490,15 +481,14 @@
     @classmethod
     def _compare(
         cls,
         samples: Dict[str, np.ndarray],
         log_l: np.ndarray,
         log_g: np.ndarray,
     ) -> Dict[str, Union[float, int]]:
-
         sample_size = next(iter(samples.values())).size
         if sample_size:
             score = log_l - log_g
             if sample_size != score.size:
                 raise ValueError(
                     "The size of the 'samples' and that of the 'score' "
                     "should be same. "
@@ -627,15 +617,15 @@
         states = (TrialState.COMPLETE, TrialState.PRUNED, TrialState.RUNNING)
     else:
         states = (TrialState.COMPLETE, TrialState.PRUNED)
 
     scores = []
     values: Dict[str, List[Optional[float]]] = {param_name: [] for param_name in param_names}
     violations: Optional[List[float]] = [] if constraints_enabled else None
-    for trial in study.get_trials(deepcopy=False, states=states):
+    for trial in study._get_trials(deepcopy=False, states=states, use_cache=not constant_liar):
         # We extract score from the trial.
         if trial.state is TrialState.COMPLETE:
             if trial.values is None:
                 continue
             score = (-float("inf"), [sign * v for sign, v in zip(signs, trial.values)])
         elif trial.state is TrialState.PRUNED:
             if study._is_multi_objective():
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/__init__.py` & `optuna-3.2.0/optuna/samplers/nsgaii/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossover.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     study: Study,
     rng: np.random.RandomState,
     swapping_prob: float,
     categorical_search_space: Dict[str, BaseDistribution],
     numerical_search_space: Dict[str, BaseDistribution],
     numerical_transform: Optional[_SearchSpaceTransform],
 ) -> Dict[str, Any]:
-
     child_params: Dict[str, Any] = {}
 
     if len(categorical_search_space) > 0:
         parents_categorical_params = np.array(
             [
                 [parent.params[p] for p in categorical_search_space]
                 for parent in [parents[0], parents[-1]]
@@ -83,15 +82,14 @@
     study: Study,
     parent_population: Sequence[FrozenTrial],
     search_space: Dict[str, BaseDistribution],
     rng: np.random.RandomState,
     swapping_prob: float,
     dominates: Callable[[FrozenTrial, FrozenTrial, Sequence[StudyDirection]], bool],
 ) -> Dict[str, Any]:
-
     numerical_search_space: Dict[str, BaseDistribution] = {}
     categorical_search_space: Dict[str, BaseDistribution] = {}
     for key, value in search_space.items():
         if isinstance(value, _NUMERICAL_DISTRIBUTIONS):
             numerical_search_space[key] = value
         else:
             categorical_search_space[key] = value
@@ -122,15 +120,14 @@
 def _select_parents(
     crossover: BaseCrossover,
     study: Study,
     parent_population: Sequence[FrozenTrial],
     rng: np.random.RandomState,
     dominates: Callable[[FrozenTrial, FrozenTrial, Sequence[StudyDirection]], bool],
 ) -> List[FrozenTrial]:
-
     parents: List[FrozenTrial] = []
     for _ in range(crossover.n_parents):
         parent = _select_parent(
             study, [t for t in parent_population if t not in parents], rng, dominates
         )
         parents.append(parent)
 
@@ -165,15 +162,14 @@
 
 def _inlined_categorical_uniform_crossover(
     parent_params: np.ndarray,
     rng: np.random.RandomState,
     swapping_prob: float,
     search_space: Dict[str, BaseDistribution],
 ) -> np.ndarray:
-
     # We can't use uniform crossover implementation of `BaseCrossover` for
     # parameters from `CategoricalDistribution`, since categorical params are
     # passed to crossover untransformed, which is not what `BaseCrossover`
     # implementations expect.
     n_categorical_params = len(search_space)
     masks = (rng.rand(n_categorical_params) >= swapping_prob).astype(int)
     return parent_params[masks, range(n_categorical_params)]
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_base.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     .. note::
         Concrete implementations of this class are expected to only accept parameters
         from numerical distributions. At the moment, only crossover operation for categorical
         parameters (uniform crossover) is built-in into :class:`~optuna.samplers.NSGAIISampler`.
     """
 
     def __str__(self) -> str:
-
         return self.__class__.__name__
 
     @property
     @abc.abstractmethod
     def n_parents(self) -> int:
         """Number of parent individuals required to perform crossover."""
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_blxalpha.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_blxalpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,23 @@
         alpha:
             Parametrizes blend operation.
     """
 
     n_parents = 2
 
     def __init__(self, alpha: float = 0.5) -> None:
-
         self._alpha = alpha
 
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
         search_space_bounds: np.ndarray,
     ) -> np.ndarray:
-
         # http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.465.6900&rep=rep1&type=pdf
         # Section 2 Crossover Operators for RCGA 2.1 Blend Crossover
 
         parents_min = parents_params.min(axis=0)
         parents_max = parents_params.max(axis=0)
         diff = self._alpha * (parents_max - parents_min)  # Equation (1).
         low = parents_min - diff  # Equation (1).
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_sbx.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_sbx.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,23 @@
             to be selected as children solutions. If not specified, takes default
             value of ``2`` for single objective functions and ``20`` for multi objective.
     """
 
     n_parents = 2
 
     def __init__(self, eta: Optional[float] = None) -> None:
-
         self._eta = eta
 
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
         search_space_bounds: np.ndarray,
     ) -> np.ndarray:
-
         # https://www.researchgate.net/profile/M-M-Raghuwanshi/publication/267198495_Simulated_Binary_Crossover_with_Lognormal_Distribution/links/5576c78408ae7536375205d7/Simulated-Binary-Crossover-with-Lognormal-Distribution.pdf
         # Section 2 Simulated Binary Crossover (SBX)
 
         # To avoid generating solutions that violate the box constraints,
         # alpha1, alpha2, xls and xus are introduced, unlike the reference.
         xls = search_space_bounds[..., 0]
         xus = search_space_bounds[..., 1]
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_spx.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_spx.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,23 @@
         epsilon:
             Expansion rate. If not specified, defaults to ``sqrt(len(search_space) + 2)``.
     """
 
     n_parents = 3
 
     def __init__(self, epsilon: Optional[float] = None) -> None:
-
         self._epsilon = epsilon
 
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
         search_space_bounds: np.ndarray,
     ) -> np.ndarray:
-
         # https://www.researchgate.net/publication/2388486_Progress_Toward_Linkage_Learning_in_Real-Coded_GAs_with_Simplex_Crossover
         # Section 2 A Brief Review of SPX
 
         n = self.n_parents - 1
         G = np.mean(parents_params, axis=0)  # Equation (1).
         rs = np.power(rng.rand(n), 1 / (np.arange(n) + 1))  # Equation (2).
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_undx.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_undx.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,33 +28,30 @@
             Parametrizes normal distribution from which ``etas`` are drawn.
             If not specified, defaults to ``0.35 / sqrt(len(search_space))``.
     """
 
     n_parents = 3
 
     def __init__(self, sigma_xi: float = 0.5, sigma_eta: Optional[float] = None) -> None:
-
         self._sigma_xi = sigma_xi
         self._sigma_eta = sigma_eta
 
     def _distance_from_x_to_psl(self, parents_params: np.ndarray) -> np.floating:
-
         # The line connecting x1 to x2 is called psl (primary search line).
         # Compute the 2-norm of the vector orthogonal to psl from x3.
         e_12 = UNDXCrossover._normalized_x1_to_x2(
             parents_params
         )  # Normalized vector from x1 to x2.
         v_13 = parents_params[2] - parents_params[0]  # Vector from x1 to x3.
         v_12_3 = v_13 - np.dot(v_13, e_12) * e_12  # Vector orthogonal to v_12 through x3.
         m_12_3 = np.linalg.norm(v_12_3, ord=2)  # 2-norm of v_12_3.
 
         return m_12_3
 
     def _orthonormal_basis_vector_to_psl(self, parents_params: np.ndarray, n: int) -> np.ndarray:
-
         # Compute orthogonal basis vectors for the subspace orthogonal to psl.
         e_12 = UNDXCrossover._normalized_x1_to_x2(
             parents_params
         )  # Normalized vector from x1 to x2.
         basis_matrix = np.identity(n)
 
         if np.count_nonzero(e_12) != 0:
@@ -68,15 +65,14 @@
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
         search_space_bounds: np.ndarray,
     ) -> np.ndarray:
-
         # https://ieeexplore.ieee.org/document/782672
         # Section 2 Unimodal Normal Distribution Crossover
         n = len(search_space_bounds)
         xp = (parents_params[0] + parents_params[1]) / 2  # Section 2 (2).
         d = parents_params[0] - parents_params[1]  # Section 2 (3).
         if self._sigma_eta is None:
             sigma_eta = 0.35 / np.sqrt(n)
@@ -102,14 +98,13 @@
         else:
             child_params = one + two
 
         return child_params
 
     @staticmethod
     def _normalized_x1_to_x2(parents_params: np.ndarray) -> np.ndarray:
-
         # Compute the normalized vector from x1 to x2.
         v_12 = parents_params[1] - parents_params[0]
         m_12 = np.linalg.norm(v_12, ord=2)
         e_12 = v_12 / np.clip(m_12, 1e-10, None)
 
         return e_12
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_uniform.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_uniform.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,25 +19,23 @@
         swapping_prob:
             Probability of swapping each parameter of the parents during crossover.
     """
 
     n_parents = 2
 
     def __init__(self, swapping_prob: float = 0.5) -> None:
-
         self._swapping_prob = swapping_prob
 
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
         search_space_bounds: np.ndarray,
     ) -> np.ndarray:
-
         # https://www.researchgate.net/publication/201976488_Uniform_Crossover_in_Genetic_Algorithms
         # Section 1 Introduction
 
         n_params = len(search_space_bounds)
         masks = (rng.rand(n_params) >= self._swapping_prob).astype(int)
         child_params = parents_params[masks, range(n_params)]
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_crossovers/_vsbx.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_vsbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from optuna._experimental import experimental_class
 from optuna.samplers.nsgaii._crossovers._base import BaseCrossover
 from optuna.study import Study
 
 
 @experimental_class("3.0.0")
 class VSBXCrossover(BaseCrossover):
-    """Modified Simulated Binary Crossover operation used by :class:`~optuna.samplers.NSGAIISampler`.
+    """Modified Simulated Binary Crossover operation used by
+    :class:`~optuna.samplers.NSGAIISampler`.
 
     vSBX generates child individuals without excluding any region of the parameter space,
     while maintaining the excellent properties of SBX.
 
     - `Pedro J. Ballester, Jonathan N. Carter.
       Real-Parameter Genetic Algorithms for Finding Multiple Optimal Solutions
       in Multi-modal Optimization. GECCO 2003: 706-717
@@ -25,25 +26,23 @@
             to be selected as children solutions. If not specified, takes default
             value of ``2`` for single objective functions and ``20`` for multi objective.
     """
 
     n_parents = 2
 
     def __init__(self, eta: Optional[float] = None) -> None:
-
         self._eta = eta
 
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
         search_space_bounds: np.ndarray,
     ) -> np.ndarray:
-
         # https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.422.952&rep=rep1&type=pdf
         # Section 3.2 Crossover Schemes (vSBX)
         if self._eta is None:
             eta = 20.0 if study._is_multi_objective() else 2.0
         else:
             eta = self._eta
```

### Comparing `optuna-3.1.1/optuna/samplers/nsgaii/_sampler.py` & `optuna-3.2.0/optuna/samplers/nsgaii/_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import optuna
 from optuna.distributions import BaseDistribution
 from optuna.exceptions import ExperimentalWarning
 from optuna.samplers._base import _CONSTRAINTS_KEY
 from optuna.samplers._base import _process_constraints_after_trial
 from optuna.samplers._base import BaseSampler
 from optuna.samplers._random import RandomSampler
-from optuna.samplers._search_space import IntersectionSearchSpace
 from optuna.samplers.nsgaii._crossover import perform_crossover
 from optuna.samplers.nsgaii._crossovers._base import BaseCrossover
 from optuna.samplers.nsgaii._crossovers._uniform import UniformCrossover
+from optuna.search_space import IntersectionSearchSpace
 from optuna.study import Study
 from optuna.study import StudyDirection
 from optuna.study._multi_objective import _dominates
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
@@ -249,15 +249,15 @@
         # 3. A parameter excluded from the intersection search space.
 
         return self._random_sampler.sample_independent(
             study, trial, param_name, param_distribution
         )
 
     def _collect_parent_population(self, study: Study) -> Tuple[int, List[FrozenTrial]]:
-        trials = study.get_trials(deepcopy=False)
+        trials = study._get_trials(deepcopy=False, use_cache=True)
 
         generation_to_runnings = defaultdict(list)
         generation_to_population = defaultdict(list)
         for trial in trials:
             if _GENERATION_KEY not in trial.system_attrs:
                 continue
 
@@ -327,76 +327,28 @@
 
         return parent_generation, parent_population
 
     def _select_elite_population(
         self, study: Study, population: List[FrozenTrial]
     ) -> List[FrozenTrial]:
         elite_population: List[FrozenTrial] = []
-        population_per_rank = self._fast_non_dominated_sort(population, study.directions)
+        population_per_rank = _fast_non_dominated_sort(
+            population, study.directions, self._constraints_func
+        )
         for population in population_per_rank:
             if len(elite_population) + len(population) < self._population_size:
                 elite_population.extend(population)
             else:
                 n = self._population_size - len(elite_population)
                 _crowding_distance_sort(population)
                 elite_population.extend(population[:n])
                 break
 
         return elite_population
 
-    def _fast_non_dominated_sort(
-        self,
-        population: List[FrozenTrial],
-        directions: List[optuna.study.StudyDirection],
-    ) -> List[List[FrozenTrial]]:
-        if self._constraints_func is not None:
-            for _trial in population:
-                _constraints = _trial.system_attrs.get(_CONSTRAINTS_KEY)
-                if _constraints is None:
-                    continue
-                if np.any(np.isnan(np.array(_constraints))):
-                    raise ValueError("NaN is not acceptable as constraint value.")
-
-        dominated_count: DefaultDict[int, int] = defaultdict(int)
-        dominates_list = defaultdict(list)
-
-        dominates = _dominates if self._constraints_func is None else _constrained_dominates
-
-        for p, q in itertools.combinations(population, 2):
-            if dominates(p, q, directions):
-                dominates_list[p.number].append(q.number)
-                dominated_count[q.number] += 1
-            elif dominates(q, p, directions):
-                dominates_list[q.number].append(p.number)
-                dominated_count[p.number] += 1
-
-        population_per_rank = []
-        while population:
-            non_dominated_population = []
-            i = 0
-            while i < len(population):
-                if dominated_count[population[i].number] == 0:
-                    individual = population[i]
-                    if i == len(population) - 1:
-                        population.pop()
-                    else:
-                        population[i] = population.pop()
-                    non_dominated_population.append(individual)
-                else:
-                    i += 1
-
-            for x in non_dominated_population:
-                for y in dominates_list[x.number]:
-                    dominated_count[y] -= 1
-
-            assert non_dominated_population
-            population_per_rank.append(non_dominated_population)
-
-        return population_per_rank
-
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
@@ -530,7 +482,58 @@
         # trial1 satisfies the constraints, but trial0 violates them.
         return False
 
     # Both trials violate the constraints.
     violation0 = sum(v for v in constraints0 if v > 0)
     violation1 = sum(v for v in constraints1 if v > 0)
     return violation0 < violation1
+
+
+def _fast_non_dominated_sort(
+    population: List[FrozenTrial],
+    directions: List[optuna.study.StudyDirection],
+    constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
+) -> List[List[FrozenTrial]]:
+    if constraints_func is not None:
+        for _trial in population:
+            _constraints = _trial.system_attrs.get(_CONSTRAINTS_KEY)
+            if _constraints is None:
+                continue
+            if np.any(np.isnan(np.array(_constraints))):
+                raise ValueError("NaN is not acceptable as constraint value.")
+
+    dominated_count: DefaultDict[int, int] = defaultdict(int)
+    dominates_list = defaultdict(list)
+
+    dominates = _dominates if constraints_func is None else _constrained_dominates
+
+    for p, q in itertools.combinations(population, 2):
+        if dominates(p, q, directions):
+            dominates_list[p.number].append(q.number)
+            dominated_count[q.number] += 1
+        elif dominates(q, p, directions):
+            dominates_list[q.number].append(p.number)
+            dominated_count[p.number] += 1
+
+    population_per_rank = []
+    while population:
+        non_dominated_population = []
+        i = 0
+        while i < len(population):
+            if dominated_count[population[i].number] == 0:
+                individual = population[i]
+                if i == len(population) - 1:
+                    population.pop()
+                else:
+                    population[i] = population.pop()
+                non_dominated_population.append(individual)
+            else:
+                i += 1
+
+        for x in non_dominated_population:
+            for y in dominates_list[x.number]:
+                dominated_count[y] -= 1
+
+        assert non_dominated_population
+        population_per_rank.append(non_dominated_population)
+
+    return population_per_rank
```

### Comparing `optuna-3.1.1/optuna/storages/__init__.py` & `optuna-3.2.0/optuna/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_base.py` & `optuna-3.2.0/optuna/storages/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
+from optuna._typing import JSONSerializable
 from optuna.distributions import BaseDistribution
 from optuna.study._frozen import FrozenStudy
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
@@ -107,15 +108,15 @@
         Raises:
             :exc:`KeyError`:
                 If no study with the matching ``study_id`` exists.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def set_study_system_attr(self, study_id: int, key: str, value: Any) -> None:
+    def set_study_system_attr(self, study_id: int, key: str, value: JSONSerializable) -> None:
         """Register an optuna-internal attribute to a study.
 
         This method overwrites any existing attribute.
 
         Args:
             study_id:
                 ID of the study.
@@ -218,15 +219,15 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_all_studies(self) -> List[FrozenStudy]:
         """Read a list of :class:`~optuna.study.FrozenStudy` objects.
 
         Returns:
-            A list of :class:`~optuna.study.FrozenStudy` objects.
+            A list of :class:`~optuna.study.FrozenStudy` objects, sorted by ``study_id``.
 
         """
         raise NotImplementedError
 
     # Basic trial manipulation
 
     @abc.abstractmethod
@@ -419,15 +420,15 @@
                 If no trial with the matching ``trial_id`` exists.
             :exc:`RuntimeError`:
                 If the trial is already finished.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def set_trial_system_attr(self, trial_id: int, key: str, value: Any) -> None:
+    def set_trial_system_attr(self, trial_id: int, key: str, value: JSONSerializable) -> None:
         """Set an optuna-internal attribute to a trial.
 
         This method overwrites any existing attribute.
 
         Args:
             trial_id:
                 ID of the trial.
@@ -478,15 +479,15 @@
             deepcopy:
                 Whether to copy the list of trials before returning.
                 Set to :obj:`True` if you intend to update the list or elements of the list.
             states:
                 Trial states to filter on. If :obj:`None`, include all states.
 
         Returns:
-            List of trials in the study.
+            List of trials in the study, sorted by ``trial_id``.
 
         Raises:
             :exc:`KeyError`:
                 If no study with the matching ``study_id`` exists.
         """
         raise NotImplementedError
```

### Comparing `optuna-3.1.1/optuna/storages/_heartbeat.py` & `optuna-3.2.0/optuna/storages/_heartbeat.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_in_memory.py` & `optuna-3.2.0/optuna/storages/_in_memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 import uuid
 
 import optuna
 from optuna import distributions  # NOQA
+from optuna._typing import JSONSerializable
 from optuna.exceptions import DuplicatedStudyError
 from optuna.storages import BaseStorage
 from optuna.storages._base import DEFAULT_STUDY_NAME_PREFIX
 from optuna.study._frozen import FrozenStudy
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
@@ -50,15 +51,14 @@
     def __setstate__(self, state: Dict[Any, Any]) -> None:
         self.__dict__.update(state)
         self._lock = threading.RLock()
 
     def create_new_study(
         self, directions: Sequence[StudyDirection], study_name: Optional[str] = None
     ) -> int:
-
         with self._lock:
             study_id = self._max_study_id + 1
             self._max_study_id += 1
 
             if study_name is not None:
                 if study_name in self._study_name_to_id:
                     raise DuplicatedStudyError
@@ -70,66 +70,58 @@
             self._study_name_to_id[study_name] = study_id
 
             _logger.info("A new study created in memory with name: {}".format(study_name))
 
             return study_id
 
     def delete_study(self, study_id: int) -> None:
-
         with self._lock:
             self._check_study_id(study_id)
 
             for trial in self._studies[study_id].trials:
                 del self._trial_id_to_study_id_and_number[trial._trial_id]
             study_name = self._studies[study_id].name
             del self._study_name_to_id[study_name]
             del self._studies[study_id]
 
     def set_study_user_attr(self, study_id: int, key: str, value: Any) -> None:
-
         with self._lock:
             self._check_study_id(study_id)
 
             self._studies[study_id].user_attrs[key] = value
 
-    def set_study_system_attr(self, study_id: int, key: str, value: Any) -> None:
-
+    def set_study_system_attr(self, study_id: int, key: str, value: JSONSerializable) -> None:
         with self._lock:
             self._check_study_id(study_id)
 
             self._studies[study_id].system_attrs[key] = value
 
     def get_study_id_from_name(self, study_name: str) -> int:
-
         with self._lock:
             if study_name not in self._study_name_to_id:
                 raise KeyError("No such study {}.".format(study_name))
 
             return self._study_name_to_id[study_name]
 
     def get_study_name_from_id(self, study_id: int) -> str:
-
         with self._lock:
             self._check_study_id(study_id)
             return self._studies[study_id].name
 
     def get_study_directions(self, study_id: int) -> List[StudyDirection]:
-
         with self._lock:
             self._check_study_id(study_id)
             return self._studies[study_id].directions
 
     def get_study_user_attrs(self, study_id: int) -> Dict[str, Any]:
-
         with self._lock:
             self._check_study_id(study_id)
             return self._studies[study_id].user_attrs
 
     def get_study_system_attrs(self, study_id: int) -> Dict[str, Any]:
-
         with self._lock:
             self._check_study_id(study_id)
             return self._studies[study_id].system_attrs
 
     def get_all_studies(self) -> List[FrozenStudy]:
         with self._lock:
             return [self._build_frozen_study(study_id) for study_id in self._studies]
@@ -142,15 +134,14 @@
             directions=study.directions,
             user_attrs=copy.deepcopy(study.user_attrs),
             system_attrs=copy.deepcopy(study.system_attrs),
             study_id=study_id,
         )
 
     def create_new_trial(self, study_id: int, template_trial: Optional[FrozenTrial] = None) -> int:
-
         with self._lock:
             self._check_study_id(study_id)
 
             if template_trial is None:
                 trial = self._create_running_trial()
             else:
                 trial = copy.deepcopy(template_trial)
@@ -162,15 +153,14 @@
             self._trial_id_to_study_id_and_number[trial_id] = (study_id, trial.number)
             self._studies[study_id].trials.append(trial)
             self._update_cache(trial_id, study_id)
             return trial_id
 
     @staticmethod
     def _create_running_trial() -> FrozenTrial:
-
         return FrozenTrial(
             trial_id=-1,  # dummy value.
             number=-1,  # dummy value.
             state=TrialState.RUNNING,
             params={},
             distributions={},
             user_attrs={},
@@ -184,15 +174,14 @@
     def set_trial_param(
         self,
         trial_id: int,
         param_name: str,
         param_value_internal: float,
         distribution: distributions.BaseDistribution,
     ) -> None:
-
         with self._lock:
             trial = self._get_trial(trial_id)
 
             self.check_trial_is_updatable(trial_id, trial.state)
 
             study_id = self._trial_id_to_study_id_and_number[trial_id][0]
             # Check param distribution compatibility with previous trial(s).
@@ -209,15 +198,14 @@
             trial.params = copy.copy(trial.params)
             trial.params[param_name] = distribution.to_external_repr(param_value_internal)
             trial.distributions = copy.copy(trial.distributions)
             trial.distributions[param_name] = distribution
             self._set_trial(trial_id, trial)
 
     def get_trial_id_from_study_id_trial_number(self, study_id: int, trial_number: int) -> int:
-
         with self._lock:
             study = self._studies.get(study_id)
             if study is None:
                 raise KeyError("No study with study_id {} exists.".format(study_id))
 
             trials = study.trials
             if len(trials) <= trial_number:
@@ -229,47 +217,43 @@
 
             trial = trials[trial_number]
             assert trial.number == trial_number
 
             return trial._trial_id
 
     def get_trial_number_from_id(self, trial_id: int) -> int:
-
         with self._lock:
             self._check_trial_id(trial_id)
 
             return self._trial_id_to_study_id_and_number[trial_id][1]
 
     def get_best_trial(self, study_id: int) -> FrozenTrial:
-
         with self._lock:
             self._check_study_id(study_id)
 
             best_trial_id = self._studies[study_id].best_trial_id
 
             if best_trial_id is None:
                 raise ValueError("No trials are completed yet.")
             elif len(self._studies[study_id].directions) > 1:
                 raise RuntimeError(
                     "Best trial can be obtained only for single-objective optimization."
                 )
             return self.get_trial(best_trial_id)
 
     def get_trial_param(self, trial_id: int, param_name: str) -> float:
-
         with self._lock:
             trial = self._get_trial(trial_id)
 
             distribution = trial.distributions[param_name]
             return distribution.to_internal_repr(trial.params[param_name])
 
     def set_trial_state_values(
         self, trial_id: int, state: TrialState, values: Optional[Sequence[float]] = None
     ) -> bool:
-
         with self._lock:
             trial = copy.copy(self._get_trial(trial_id))
             self.check_trial_is_updatable(trial_id, trial.state)
 
             if state == TrialState.RUNNING and trial.state != TrialState.WAITING:
                 return False
 
@@ -287,15 +271,14 @@
                 self._update_cache(trial_id, study_id)
             else:
                 self._set_trial(trial_id, trial)
 
             return True
 
     def _update_cache(self, trial_id: int, study_id: int) -> None:
-
         trial = self._get_trial(trial_id)
 
         if trial.state != TrialState.COMPLETE:
             return
 
         best_trial_id = self._studies[study_id].best_trial_id
         if best_trial_id is None:
@@ -323,93 +306,84 @@
         else:
             if best_value > new_value:
                 self._studies[study_id].best_trial_id = trial_id
 
     def set_trial_intermediate_value(
         self, trial_id: int, step: int, intermediate_value: float
     ) -> None:
-
         with self._lock:
             trial = self._get_trial(trial_id)
             self.check_trial_is_updatable(trial_id, trial.state)
 
             trial = copy.copy(trial)
             trial.intermediate_values = copy.copy(trial.intermediate_values)
             trial.intermediate_values[step] = intermediate_value
             self._set_trial(trial_id, trial)
 
     def set_trial_user_attr(self, trial_id: int, key: str, value: Any) -> None:
-
         with self._lock:
             self._check_trial_id(trial_id)
             trial = self._get_trial(trial_id)
             self.check_trial_is_updatable(trial_id, trial.state)
 
             trial = copy.copy(trial)
             trial.user_attrs = copy.copy(trial.user_attrs)
             trial.user_attrs[key] = value
             self._set_trial(trial_id, trial)
 
-    def set_trial_system_attr(self, trial_id: int, key: str, value: Any) -> None:
-
+    def set_trial_system_attr(self, trial_id: int, key: str, value: JSONSerializable) -> None:
         with self._lock:
             trial = self._get_trial(trial_id)
             self.check_trial_is_updatable(trial_id, trial.state)
 
             trial = copy.copy(trial)
             trial.system_attrs = copy.copy(trial.system_attrs)
             trial.system_attrs[key] = value
             self._set_trial(trial_id, trial)
 
     def get_trial(self, trial_id: int) -> FrozenTrial:
-
         with self._lock:
             return self._get_trial(trial_id)
 
     def _get_trial(self, trial_id: int) -> FrozenTrial:
-
         self._check_trial_id(trial_id)
         study_id, trial_number = self._trial_id_to_study_id_and_number[trial_id]
         return self._studies[study_id].trials[trial_number]
 
     def _set_trial(self, trial_id: int, trial: FrozenTrial) -> None:
         study_id, trial_number = self._trial_id_to_study_id_and_number[trial_id]
         self._studies[study_id].trials[trial_number] = trial
 
     def get_all_trials(
         self,
         study_id: int,
         deepcopy: bool = True,
         states: Optional[Container[TrialState]] = None,
     ) -> List[FrozenTrial]:
-
         with self._lock:
             self._check_study_id(study_id)
 
-            trials = self._studies[
+            trials: Union[List[FrozenTrial], Iterator[FrozenTrial]] = self._studies[
                 study_id
-            ].trials  # type: Union[List[FrozenTrial], Iterator[FrozenTrial]]
-
+            ].trials
             if states is not None:
                 trials = filter(lambda t: t.state in states, trials)
 
             if deepcopy:
                 trials = copy.deepcopy(list(trials))
             else:
                 trials = list(trials)
 
         return trials
 
     def _check_study_id(self, study_id: int) -> None:
-
         if study_id not in self._studies:
             raise KeyError("No study with study_id {} exists.".format(study_id))
 
     def _check_trial_id(self, trial_id: int) -> None:
-
         if trial_id not in self._trial_id_to_study_id_and_number:
             raise KeyError("No trial with trial_id {} exists.".format(trial_id))
 
 
 class _StudyInfo:
     def __init__(self, name: str, directions: List[StudyDirection]) -> None:
         self.trials: List[FrozenTrial] = []
```

### Comparing `optuna-3.1.1/optuna/storages/_journal/base.py` & `optuna-3.2.0/optuna/storages/_journal/base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_journal/file.py` & `optuna-3.2.0/optuna/storages/_journal/file.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_journal/redis.py` & `optuna-3.2.0/optuna/storages/_journal/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
             cause errors.
         prefix:
             Prefix of the preserved key of logs. This is useful when multiple users work on one
             Redis server.
     """
 
     def __init__(self, url: str, use_cluster: bool = False, prefix: str = "") -> None:
-
         _imports.check()
 
         self._url = url
         self._redis = redis.Redis.from_url(url)
         self._use_cluster = use_cluster
         self._prefix = prefix
 
@@ -50,15 +49,14 @@
         return state
 
     def __setstate__(self, state: Dict[Any, Any]) -> None:
         self.__dict__.update(state)
         self._redis = redis.Redis.from_url(self._url)
 
     def read_logs(self, log_number_from: int) -> List[Dict[str, Any]]:
-
         max_log_number_bytes = self._redis.get(f"{self._prefix}:log_number")
         if max_log_number_bytes is None:
             return []
         max_log_number = int(max_log_number_bytes)
 
         logs = []
         for log_number in range(log_number_from, max_log_number + 1):
@@ -73,15 +71,14 @@
                 logs.append(json.loads(log))
             except json.JSONDecodeError as err:
                 if log_number != max_log_number:
                     raise err
         return logs
 
     def append_logs(self, logs: List[Dict[str, Any]]) -> None:
-
         self._redis.setnx(f"{self._prefix}:log_number", -1)
         for log in logs:
             if not self._use_cluster:
                 self._redis.eval(  # type: ignore
                     "local i = redis.call('incr', string.format('%s:log_number', ARGV[1])) "
                     "redis.call('set', string.format('%s:log:%d', ARGV[1], i), ARGV[2])",
                     0,
```

### Comparing `optuna-3.1.1/optuna/storages/_journal/storage.py` & `optuna-3.2.0/optuna/storages/_journal/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import List
 from typing import Optional
 from typing import Sequence
 import uuid
 
 import optuna
 from optuna._experimental import experimental_class
+from optuna._typing import JSONSerializable
 from optuna.distributions import BaseDistribution
 from optuna.distributions import check_distribution_compatibility
 from optuna.distributions import distribution_to_json
 from optuna.distributions import json_to_distribution
 from optuna.exceptions import DuplicatedStudyError
 from optuna.storages import BaseStorage
 from optuna.storages._base import DEFAULT_STUDY_NAME_PREFIX
@@ -184,15 +185,15 @@
 
     def set_study_user_attr(self, study_id: int, key: str, value: Any) -> None:
         log: Dict[str, Any] = {"study_id": study_id, "user_attr": {key: value}}
         with self._thread_lock:
             self._write_log(JournalOperation.SET_STUDY_USER_ATTR, log)
             self._sync_with_backend()
 
-    def set_study_system_attr(self, study_id: int, key: str, value: Any) -> None:
+    def set_study_system_attr(self, study_id: int, key: str, value: JSONSerializable) -> None:
         log: Dict[str, Any] = {"study_id": study_id, "system_attr": {key: value}}
         with self._thread_lock:
             self._write_log(JournalOperation.SET_STUDY_SYSTEM_ATTR, log)
             self._sync_with_backend()
 
     def get_study_id_from_name(self, study_name: str) -> int:
         with self._thread_lock:
@@ -349,15 +350,15 @@
             "user_attr": {key: value},
         }
 
         with self._thread_lock:
             self._write_log(JournalOperation.SET_TRIAL_USER_ATTR, log)
             self._sync_with_backend()
 
-    def set_trial_system_attr(self, trial_id: int, key: str, value: Any) -> None:
+    def set_trial_system_attr(self, trial_id: int, key: str, value: JSONSerializable) -> None:
         log: Dict[str, Any] = {
             "trial_id": trial_id,
             "system_attr": {key: value},
         }
 
         with self._thread_lock:
             self._write_log(JournalOperation.SET_TRIAL_SYSTEM_ATTR, log)
```

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/env.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py` & `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/alembic.ini` & `optuna-3.2.0/optuna/storages/_rdb/alembic.ini`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/storages/_rdb/models.py` & `optuna-3.2.0/optuna/storages/_rdb/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,36 +52,33 @@
     study_id = Column(Integer, primary_key=True)
     study_name = Column(String(MAX_INDEXED_STRING_LENGTH), index=True, unique=True, nullable=False)
 
     @classmethod
     def find_or_raise_by_id(
         cls, study_id: int, session: orm.Session, for_update: bool = False
     ) -> "StudyModel":
-
         query = session.query(cls).filter(cls.study_id == study_id)
 
         if for_update:
             query = query.with_for_update()
 
         study = query.one_or_none()
         if study is None:
             raise KeyError(NOT_FOUND_MSG)
 
         return study
 
     @classmethod
     def find_by_name(cls, study_name: str, session: orm.Session) -> Optional["StudyModel"]:
-
         study = session.query(cls).filter(cls.study_name == study_name).one_or_none()
 
         return study
 
     @classmethod
     def find_or_raise_by_name(cls, study_name: str, session: orm.Session) -> "StudyModel":
-
         study = cls.find_by_name(study_name, session)
         if study is None:
             raise KeyError(NOT_FOUND_MSG)
 
         return study
 
 
@@ -95,15 +92,14 @@
 
     study = orm.relationship(
         StudyModel, backref=orm.backref("directions", cascade="all, delete-orphan")
     )
 
     @classmethod
     def where_study_id(cls, study_id: int, session: orm.Session) -> List["StudyDirectionModel"]:
-
         return session.query(cls).filter(cls.study_id == study_id).all()
 
 
 class StudyUserAttributeModel(BaseModel):
     __tablename__ = "study_user_attributes"
     __table_args__: Any = (UniqueConstraint("study_id", "key"),)
     study_user_attribute_id = Column(Integer, primary_key=True)
@@ -115,29 +111,27 @@
         StudyModel, backref=orm.backref("user_attributes", cascade="all, delete-orphan")
     )
 
     @classmethod
     def find_by_study_and_key(
         cls, study: StudyModel, key: str, session: orm.Session
     ) -> Optional["StudyUserAttributeModel"]:
-
         attribute = (
             session.query(cls)
             .filter(cls.study_id == study.study_id)
             .filter(cls.key == key)
             .one_or_none()
         )
 
         return attribute
 
     @classmethod
     def where_study_id(
         cls, study_id: int, session: orm.Session
     ) -> List["StudyUserAttributeModel"]:
-
         return session.query(cls).filter(cls.study_id == study_id).all()
 
 
 class StudySystemAttributeModel(BaseModel):
     __tablename__ = "study_system_attributes"
     __table_args__: Any = (UniqueConstraint("study_id", "key"),)
     study_system_attribute_id = Column(Integer, primary_key=True)
@@ -149,53 +143,50 @@
         StudyModel, backref=orm.backref("system_attributes", cascade="all, delete-orphan")
     )
 
     @classmethod
     def find_by_study_and_key(
         cls, study: StudyModel, key: str, session: orm.Session
     ) -> Optional["StudySystemAttributeModel"]:
-
         attribute = (
             session.query(cls)
             .filter(cls.study_id == study.study_id)
             .filter(cls.key == key)
             .one_or_none()
         )
 
         return attribute
 
     @classmethod
     def where_study_id(
         cls, study_id: int, session: orm.Session
     ) -> List["StudySystemAttributeModel"]:
-
         return session.query(cls).filter(cls.study_id == study_id).all()
 
 
 class TrialModel(BaseModel):
     __tablename__ = "trials"
     trial_id = Column(Integer, primary_key=True)
     # No `UniqueConstraint` is put on the `number` columns although it in practice is constrained
     # to be unique. This is to reduce code complexity as table-level locking would be required
     # otherwise. See https://github.com/optuna/optuna/pull/939#discussion_r387447632.
     number = Column(Integer)
-    study_id = Column(Integer, ForeignKey("studies.study_id"))
+    study_id = Column(Integer, ForeignKey("studies.study_id"), index=True)
     state = Column(Enum(TrialState), nullable=False)
     datetime_start = Column(DateTime)
     datetime_complete = Column(DateTime)
 
     study = orm.relationship(
         StudyModel, backref=orm.backref("trials", cascade="all, delete-orphan")
     )
 
     @classmethod
     def find_max_value_trial(
         cls, study_id: int, objective: int, session: orm.Session
     ) -> "TrialModel":
-
         trial = (
             session.query(cls)
             .filter(cls.study_id == study_id)
             .filter(cls.state == TrialState.COMPLETE)
             .join(TrialValueModel)
             .filter(TrialValueModel.objective == objective)
             .order_by(
@@ -214,15 +205,14 @@
             raise ValueError(NOT_FOUND_MSG)
         return trial
 
     @classmethod
     def find_min_value_trial(
         cls, study_id: int, objective: int, session: orm.Session
     ) -> "TrialModel":
-
         trial = (
             session.query(cls)
             .filter(cls.study_id == study_id)
             .filter(cls.state == TrialState.COMPLETE)
             .join(TrialValueModel)
             .filter(TrialValueModel.objective == objective)
             .order_by(
@@ -241,15 +231,14 @@
             raise ValueError(NOT_FOUND_MSG)
         return trial
 
     @classmethod
     def find_or_raise_by_id(
         cls, trial_id: int, session: orm.Session, for_update: bool = False
     ) -> "TrialModel":
-
         query = session.query(cls).filter(cls.trial_id == trial_id)
 
         # "FOR UPDATE" clause is used for row-level locking.
         # Please note that SQLite3 doesn't support this clause.
         if for_update:
             query = query.with_for_update()
 
@@ -262,25 +251,23 @@
     @classmethod
     def count(
         cls,
         session: orm.Session,
         study: Optional[StudyModel] = None,
         state: Optional[TrialState] = None,
     ) -> int:
-
         trial_count = session.query(func.count(cls.trial_id))
         if study is not None:
             trial_count = trial_count.filter(cls.study_id == study.study_id)
         if state is not None:
             trial_count = trial_count.filter(cls.state == state)
 
         return trial_count.scalar()
 
     def count_past_trials(self, session: orm.Session) -> int:
-
         trial_count = session.query(func.count(TrialModel.trial_id)).filter(
             TrialModel.study_id == self.study_id, TrialModel.trial_id < self.trial_id
         )
         return trial_count.scalar()
 
 
 class TrialUserAttributeModel(BaseModel):
@@ -295,29 +282,27 @@
         TrialModel, backref=orm.backref("user_attributes", cascade="all, delete-orphan")
     )
 
     @classmethod
     def find_by_trial_and_key(
         cls, trial: TrialModel, key: str, session: orm.Session
     ) -> Optional["TrialUserAttributeModel"]:
-
         attribute = (
             session.query(cls)
             .filter(cls.trial_id == trial.trial_id)
             .filter(cls.key == key)
             .one_or_none()
         )
 
         return attribute
 
     @classmethod
     def where_trial_id(
         cls, trial_id: int, session: orm.Session
     ) -> List["TrialUserAttributeModel"]:
-
         return session.query(cls).filter(cls.trial_id == trial_id).all()
 
 
 class TrialSystemAttributeModel(BaseModel):
     __tablename__ = "trial_system_attributes"
     __table_args__: Any = (UniqueConstraint("trial_id", "key"),)
     trial_system_attribute_id = Column(Integer, primary_key=True)
@@ -329,29 +314,27 @@
         TrialModel, backref=orm.backref("system_attributes", cascade="all, delete-orphan")
     )
 
     @classmethod
     def find_by_trial_and_key(
         cls, trial: TrialModel, key: str, session: orm.Session
     ) -> Optional["TrialSystemAttributeModel"]:
-
         attribute = (
             session.query(cls)
             .filter(cls.trial_id == trial.trial_id)
             .filter(cls.key == key)
             .one_or_none()
         )
 
         return attribute
 
     @classmethod
     def where_trial_id(
         cls, trial_id: int, session: orm.Session
     ) -> List["TrialSystemAttributeModel"]:
-
         return session.query(cls).filter(cls.trial_id == trial_id).all()
 
 
 class TrialParamModel(BaseModel):
     __tablename__ = "trial_params"
     __table_args__: Any = (UniqueConstraint("trial_id", "param_name"),)
     param_id = Column(Integer, primary_key=True)
@@ -361,22 +344,20 @@
     distribution_json = Column(Text())
 
     trial = orm.relationship(
         TrialModel, backref=orm.backref("params", cascade="all, delete-orphan")
     )
 
     def check_and_add(self, session: orm.Session) -> None:
-
         self._check_compatibility_with_previous_trial_param_distributions(session)
         session.add(self)
 
     def _check_compatibility_with_previous_trial_param_distributions(
         self, session: orm.Session
     ) -> None:
-
         trial = TrialModel.find_or_raise_by_id(self.trial_id, session)
 
         previous_record = (
             session.query(TrialParamModel)
             .join(TrialModel)
             .filter(TrialModel.study_id == trial.study_id)
             .filter(TrialParamModel.param_name == self.param_name)
@@ -388,39 +369,36 @@
                 distributions.json_to_distribution(self.distribution_json),
             )
 
     @classmethod
     def find_by_trial_and_param_name(
         cls, trial: TrialModel, param_name: str, session: orm.Session
     ) -> Optional["TrialParamModel"]:
-
         param_distribution = (
             session.query(cls)
             .filter(cls.trial_id == trial.trial_id)
             .filter(cls.param_name == param_name)
             .one_or_none()
         )
 
         return param_distribution
 
     @classmethod
     def find_or_raise_by_trial_and_param_name(
         cls, trial: TrialModel, param_name: str, session: orm.Session
     ) -> "TrialParamModel":
-
         param_distribution = cls.find_by_trial_and_param_name(trial, param_name, session)
 
         if param_distribution is None:
             raise KeyError(NOT_FOUND_MSG)
 
         return param_distribution
 
     @classmethod
     def where_trial_id(cls, trial_id: int, session: orm.Session) -> List["TrialParamModel"]:
-
         trial_params = session.query(cls).filter(cls.trial_id == trial_id).all()
 
         return trial_params
 
 
 class TrialValueModel(BaseModel):
     class TrialValueType(enum.Enum):
@@ -465,27 +443,25 @@
             assert value is not None
             return value
 
     @classmethod
     def find_by_trial_and_objective(
         cls, trial: TrialModel, objective: int, session: orm.Session
     ) -> Optional["TrialValueModel"]:
-
         trial_value = (
             session.query(cls)
             .filter(cls.trial_id == trial.trial_id)
             .filter(cls.objective == objective)
             .one_or_none()
         )
 
         return trial_value
 
     @classmethod
     def where_trial_id(cls, trial_id: int, session: orm.Session) -> List["TrialValueModel"]:
-
         trial_values = (
             session.query(cls).filter(cls.trial_id == trial_id).order_by(asc(cls.objective)).all()
         )
 
         return trial_values
 
 
@@ -540,29 +516,27 @@
             assert value is not None
             return value
 
     @classmethod
     def find_by_trial_and_step(
         cls, trial: TrialModel, step: int, session: orm.Session
     ) -> Optional["TrialIntermediateValueModel"]:
-
         trial_intermediate_value = (
             session.query(cls)
             .filter(cls.trial_id == trial.trial_id)
             .filter(cls.step == step)
             .one_or_none()
         )
 
         return trial_intermediate_value
 
     @classmethod
     def where_trial_id(
         cls, trial_id: int, session: orm.Session
     ) -> List["TrialIntermediateValueModel"]:
-
         trial_intermediate_values = session.query(cls).filter(cls.trial_id == trial_id).all()
 
         return trial_intermediate_values
 
 
 class TrialHeartbeatModel(BaseModel):
     __tablename__ = "trial_heartbeats"
@@ -588,11 +562,10 @@
     __table_args__: Any = (CheckConstraint("version_info_id=1"),)
     version_info_id = Column(Integer, primary_key=True, autoincrement=False, default=1)
     schema_version = Column(Integer)
     library_version = Column(String(MAX_VERSION_LENGTH))
 
     @classmethod
     def find(cls, session: orm.Session) -> "VersionInfoModel":
-
         version_info = session.query(cls).one_or_none()
 
         return version_info
```

### Comparing `optuna-3.1.1/optuna/storages/_rdb/storage.py` & `optuna-3.2.0/optuna/storages/_rdb/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import TYPE_CHECKING
 import uuid
 
 import optuna
 from optuna import distributions
 from optuna import version
 from optuna._imports import _LazyImport
+from optuna._typing import JSONSerializable
 from optuna.storages._base import BaseStorage
 from optuna.storages._base import DEFAULT_STUDY_NAME_PREFIX
 from optuna.storages._heartbeat import BaseHeartbeat
 from optuna.storages._rdb.models import TrialValueModel
 from optuna.study._frozen import FrozenStudy
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
@@ -194,15 +195,14 @@
         heartbeat_interval: Optional[int] = None,
         grace_period: Optional[int] = None,
         failed_trial_callback: Optional[
             Callable[["optuna.study.Study", FrozenTrial], None]
         ] = None,
         skip_table_creation: bool = False,
     ) -> None:
-
         self.engine_kwargs = engine_kwargs or {}
         self.url = self._fill_storage_url_template(url)
         self.skip_compatibility_check = skip_compatibility_check
         if heartbeat_interval is not None and heartbeat_interval <= 0:
             raise ValueError("The value of `heartbeat_interval` should be a positive integer.")
         if grace_period is not None and grace_period <= 0:
             raise ValueError("The value of `grace_period` should be a positive integer.")
@@ -227,23 +227,21 @@
             models.BaseModel.metadata.create_all(self.engine)
 
         self._version_manager = _VersionManager(self.url, self.engine, self.scoped_session)
         if not skip_compatibility_check:
             self._version_manager.check_table_schema_compatibility()
 
     def __getstate__(self) -> Dict[Any, Any]:
-
         state = self.__dict__.copy()
         del state["scoped_session"]
         del state["engine"]
         del state["_version_manager"]
         return state
 
     def __setstate__(self, state: Dict[Any, Any]) -> None:
-
         self.__dict__.update(state)
         try:
             self.engine = sqlalchemy.engine.create_engine(self.url, **self.engine_kwargs)
         except ImportError as e:
             raise ImportError(
                 "Failed to import DB access module for the specified storage URL. "
                 "Please install appropriate one."
@@ -256,15 +254,14 @@
         self._version_manager = _VersionManager(self.url, self.engine, self.scoped_session)
         if not self.skip_compatibility_check:
             self._version_manager.check_table_schema_compatibility()
 
     def create_new_study(
         self, directions: Sequence[StudyDirection], study_name: Optional[str] = None
     ) -> int:
-
         try:
             with _create_scoped_session(self.scoped_session) as session:
                 if study_name is None:
                     study_name = self._create_unique_study_name(session)
 
                 direction_models = [
                     models.StudyDirectionModel(objective=objective, direction=d)
@@ -282,130 +279,122 @@
             )
 
         _logger.info("A new study created in RDB with name: {}".format(study_name))
 
         return self.get_study_id_from_name(study_name)
 
     def delete_study(self, study_id: int) -> None:
-
         with _create_scoped_session(self.scoped_session, True) as session:
             study = models.StudyModel.find_or_raise_by_id(study_id, session)
             session.delete(study)
 
     @staticmethod
     def _create_unique_study_name(session: "sqlalchemy_orm.Session") -> str:
-
         while True:
             study_uuid = str(uuid.uuid4())
             study_name = DEFAULT_STUDY_NAME_PREFIX + study_uuid
             study = models.StudyModel.find_by_name(study_name, session)
             if study is None:
                 break
 
         return study_name
 
     def set_study_user_attr(self, study_id: int, key: str, value: Any) -> None:
-
         with _create_scoped_session(self.scoped_session, True) as session:
             study = models.StudyModel.find_or_raise_by_id(study_id, session)
             attribute = models.StudyUserAttributeModel.find_by_study_and_key(study, key, session)
             if attribute is None:
                 attribute = models.StudyUserAttributeModel(
                     study_id=study_id, key=key, value_json=json.dumps(value)
                 )
                 session.add(attribute)
             else:
                 attribute.value_json = json.dumps(value)
 
-    def set_study_system_attr(self, study_id: int, key: str, value: Any) -> None:
-
+    def set_study_system_attr(self, study_id: int, key: str, value: JSONSerializable) -> None:
         with _create_scoped_session(self.scoped_session, True) as session:
             study = models.StudyModel.find_or_raise_by_id(study_id, session)
             attribute = models.StudySystemAttributeModel.find_by_study_and_key(study, key, session)
             if attribute is None:
                 attribute = models.StudySystemAttributeModel(
                     study_id=study_id, key=key, value_json=json.dumps(value)
                 )
                 session.add(attribute)
             else:
                 attribute.value_json = json.dumps(value)
 
     def get_study_id_from_name(self, study_name: str) -> int:
-
         with _create_scoped_session(self.scoped_session) as session:
             study = models.StudyModel.find_or_raise_by_name(study_name, session)
             study_id = study.study_id
 
         return study_id
 
     def get_study_name_from_id(self, study_id: int) -> str:
-
         with _create_scoped_session(self.scoped_session) as session:
             study = models.StudyModel.find_or_raise_by_id(study_id, session)
             study_name = study.study_name
 
         return study_name
 
     def get_study_directions(self, study_id: int) -> List[StudyDirection]:
-
         with _create_scoped_session(self.scoped_session) as session:
             study = models.StudyModel.find_or_raise_by_id(study_id, session)
             directions = [d.direction for d in study.directions]
 
         return directions
 
     def get_study_user_attrs(self, study_id: int) -> Dict[str, Any]:
-
         with _create_scoped_session(self.scoped_session) as session:
             # Ensure that that study exists.
             models.StudyModel.find_or_raise_by_id(study_id, session)
             attributes = models.StudyUserAttributeModel.where_study_id(study_id, session)
             user_attrs = {attr.key: json.loads(attr.value_json) for attr in attributes}
 
         return user_attrs
 
     def get_study_system_attrs(self, study_id: int) -> Dict[str, Any]:
-
         with _create_scoped_session(self.scoped_session) as session:
             # Ensure that that study exists.
             models.StudyModel.find_or_raise_by_id(study_id, session)
             attributes = models.StudySystemAttributeModel.where_study_id(study_id, session)
             system_attrs = {attr.key: json.loads(attr.value_json) for attr in attributes}
 
         return system_attrs
 
     def get_trial_user_attrs(self, trial_id: int) -> Dict[str, Any]:
-
         with _create_scoped_session(self.scoped_session) as session:
             # Ensure trial exists.
             models.TrialModel.find_or_raise_by_id(trial_id, session)
 
             attributes = models.TrialUserAttributeModel.where_trial_id(trial_id, session)
             user_attrs = {attr.key: json.loads(attr.value_json) for attr in attributes}
 
         return user_attrs
 
     def get_trial_system_attrs(self, trial_id: int) -> Dict[str, Any]:
-
         with _create_scoped_session(self.scoped_session) as session:
             # Ensure trial exists.
             models.TrialModel.find_or_raise_by_id(trial_id, session)
 
             attributes = models.TrialSystemAttributeModel.where_trial_id(trial_id, session)
             system_attrs = {attr.key: json.loads(attr.value_json) for attr in attributes}
 
         return system_attrs
 
     def get_all_studies(self) -> List[FrozenStudy]:
         with _create_scoped_session(self.scoped_session) as session:
-
-            studies = session.query(
-                models.StudyModel.study_id,
-                models.StudyModel.study_name,
-            ).all()
+            studies = (
+                session.query(
+                    models.StudyModel.study_id,
+                    models.StudyModel.study_name,
+                )
+                .order_by(models.StudyModel.study_id)
+                .all()
+            )
 
             _directions = defaultdict(list)
             for direction_model in session.query(models.StudyDirectionModel).all():
                 _directions[direction_model.study_id].append(direction_model.direction)
 
             _user_attrs = defaultdict(list)
             for attribute_model in session.query(models.StudyUserAttributeModel).all():
@@ -430,15 +419,14 @@
                         study_id=study.study_id,
                     )
                 )
 
             return frozen_studies
 
     def create_new_trial(self, study_id: int, template_trial: Optional[FrozenTrial] = None) -> int:
-
         return self._create_new_trial(study_id, template_trial)._trial_id
 
     def _create_new_trial(
         self, study_id: int, template_trial: Optional[FrozenTrial] = None
     ) -> FrozenTrial:
         """Create a new trial and returns a :class:`~optuna.trial.FrozenTrial`.
 
@@ -467,15 +455,15 @@
 
                     trial = self._get_prepared_new_trial(study_id, template_trial, session)
                     break  # Successfully created trial.
                 except sqlalchemy_exc.OperationalError:
                     if n_retries > 2:
                         raise
 
-            n_retries += 1
+                n_retries += 1
 
             if template_trial:
                 frozen = copy.deepcopy(template_trial)
                 frozen.number = trial.number
                 frozen.datetime_start = trial.datetime_start
                 frozen._trial_id = trial.trial_id
             else:
@@ -570,29 +558,27 @@
     def set_trial_param(
         self,
         trial_id: int,
         param_name: str,
         param_value_internal: float,
         distribution: distributions.BaseDistribution,
     ) -> None:
-
         with _create_scoped_session(self.scoped_session, True) as session:
             self._set_trial_param_without_commit(
                 session, trial_id, param_name, param_value_internal, distribution
             )
 
     def _set_trial_param_without_commit(
         self,
         session: "sqlalchemy_orm.Session",
         trial_id: int,
         param_name: str,
         param_value_internal: float,
         distribution: distributions.BaseDistribution,
     ) -> None:
-
         trial = models.TrialModel.find_or_raise_by_id(trial_id, session)
         self.check_trial_is_updatable(trial_id, trial.state)
 
         trial_param = models.TrialParamModel.find_by_trial_and_param_name(
             trial, param_name, session
         )
 
@@ -618,43 +604,40 @@
         self,
         study_id: int,
         trial_id: int,
         param_name: str,
         param_value_internal: float,
         distribution: distributions.BaseDistribution,
     ) -> None:
-
         with _create_scoped_session(self.scoped_session) as session:
             # Acquire lock.
             #
             # Assume that study exists.
             models.StudyModel.find_or_raise_by_id(study_id, session, for_update=True)
 
             models.TrialParamModel(
                 trial_id=trial_id,
                 param_name=param_name,
                 param_value=param_value_internal,
                 distribution_json=distributions.distribution_to_json(distribution),
             ).check_and_add(session)
 
     def get_trial_param(self, trial_id: int, param_name: str) -> float:
-
         with _create_scoped_session(self.scoped_session) as session:
             trial = models.TrialModel.find_or_raise_by_id(trial_id, session)
             trial_param = models.TrialParamModel.find_or_raise_by_trial_and_param_name(
                 trial, param_name, session
             )
             param_value = trial_param.param_value
 
         return param_value
 
     def set_trial_state_values(
         self, trial_id: int, state: TrialState, values: Optional[Sequence[float]] = None
     ) -> bool:
-
         try:
             with _create_scoped_session(self.scoped_session) as session:
                 trial = models.TrialModel.find_or_raise_by_id(trial_id, session, for_update=True)
                 self.check_trial_is_updatable(trial_id, trial.state)
 
                 if values is not None:
                     for objective, v in enumerate(values):
@@ -673,15 +656,14 @@
         except sqlalchemy_exc.IntegrityError:
             return False
         return True
 
     def _set_trial_value_without_commit(
         self, session: "sqlalchemy_orm.Session", trial_id: int, objective: int, value: float
     ) -> None:
-
         trial = models.TrialModel.find_or_raise_by_id(trial_id, session)
         self.check_trial_is_updatable(trial_id, trial.state)
         stored_value, value_type = TrialValueModel.value_to_stored_repr(value)
 
         trial_value = models.TrialValueModel.find_by_trial_and_objective(trial, objective, session)
         if trial_value is None:
             trial_value = models.TrialValueModel(
@@ -691,28 +673,26 @@
         else:
             trial_value.value = stored_value
             trial_value.value_type = value_type
 
     def set_trial_intermediate_value(
         self, trial_id: int, step: int, intermediate_value: float
     ) -> None:
-
         with _create_scoped_session(self.scoped_session, True) as session:
             self._set_trial_intermediate_value_without_commit(
                 session, trial_id, step, intermediate_value
             )
 
     def _set_trial_intermediate_value_without_commit(
         self,
         session: "sqlalchemy_orm.Session",
         trial_id: int,
         step: int,
         intermediate_value: float,
     ) -> None:
-
         trial = models.TrialModel.find_or_raise_by_id(trial_id, session)
         self.check_trial_is_updatable(trial_id, trial.state)
 
         (
             stored_value,
             value_type,
         ) = models.TrialIntermediateValueModel.intermediate_value_to_stored_repr(
@@ -730,57 +710,52 @@
             )
             session.add(trial_intermediate_value)
         else:
             trial_intermediate_value.intermediate_value = stored_value
             trial_intermediate_value.intermediate_value_type = value_type
 
     def set_trial_user_attr(self, trial_id: int, key: str, value: Any) -> None:
-
         with _create_scoped_session(self.scoped_session, True) as session:
             self._set_trial_user_attr_without_commit(session, trial_id, key, value)
 
     def _set_trial_user_attr_without_commit(
         self, session: "sqlalchemy_orm.Session", trial_id: int, key: str, value: Any
     ) -> None:
-
         trial = models.TrialModel.find_or_raise_by_id(trial_id, session)
         self.check_trial_is_updatable(trial_id, trial.state)
 
         attribute = models.TrialUserAttributeModel.find_by_trial_and_key(trial, key, session)
         if attribute is None:
             attribute = models.TrialUserAttributeModel(
                 trial_id=trial_id, key=key, value_json=json.dumps(value)
             )
             session.add(attribute)
         else:
             attribute.value_json = json.dumps(value)
 
-    def set_trial_system_attr(self, trial_id: int, key: str, value: Any) -> None:
-
+    def set_trial_system_attr(self, trial_id: int, key: str, value: JSONSerializable) -> None:
         with _create_scoped_session(self.scoped_session, True) as session:
             self._set_trial_system_attr_without_commit(session, trial_id, key, value)
 
     def _set_trial_system_attr_without_commit(
-        self, session: "sqlalchemy_orm.Session", trial_id: int, key: str, value: Any
+        self, session: "sqlalchemy_orm.Session", trial_id: int, key: str, value: JSONSerializable
     ) -> None:
-
         trial = models.TrialModel.find_or_raise_by_id(trial_id, session)
         self.check_trial_is_updatable(trial_id, trial.state)
 
         attribute = models.TrialSystemAttributeModel.find_by_trial_and_key(trial, key, session)
         if attribute is None:
             attribute = models.TrialSystemAttributeModel(
                 trial_id=trial_id, key=key, value_json=json.dumps(value)
             )
             session.add(attribute)
         else:
             attribute.value_json = json.dumps(value)
 
     def get_trial_id_from_study_id_trial_number(self, study_id: int, trial_number: int) -> int:
-
         with _create_scoped_session(self.scoped_session) as session:
             trial_id = (
                 session.query(models.TrialModel.trial_id)
                 .filter(
                     models.TrialModel.number == trial_number,
                     models.TrialModel.study_id == study_id,
                 )
@@ -791,39 +766,36 @@
                     "No trial with trial number {} exists in study with study_id {}.".format(
                         trial_number, study_id
                     )
                 )
             return trial_id[0]
 
     def get_trial(self, trial_id: int) -> FrozenTrial:
-
         with _create_scoped_session(self.scoped_session) as session:
             trial_model = models.TrialModel.find_or_raise_by_id(trial_id, session)
             frozen_trial = self._build_frozen_trial_from_trial_model(trial_model)
 
         return frozen_trial
 
     def get_all_trials(
         self,
         study_id: int,
         deepcopy: bool = True,
         states: Optional[Container[TrialState]] = None,
     ) -> List[FrozenTrial]:
-
         trials = self._get_trials(study_id, states, set())
 
         return copy.deepcopy(trials) if deepcopy else trials
 
     def _get_trials(
         self,
         study_id: int,
         states: Optional[Container[TrialState]],
         excluded_trial_ids: Set[int],
     ) -> List[FrozenTrial]:
-
         with _create_scoped_session(self.scoped_session) as session:
             # Ensure that the study exists.
             models.StudyModel.find_or_raise_by_id(study_id, session)
             query = session.query(models.TrialModel.trial_id).filter(
                 models.TrialModel.study_id == study_id
             )
 
@@ -877,15 +849,14 @@
                 trial_models = [t for t in trial_models if t.trial_id in trial_ids]
 
             trials = [self._build_frozen_trial_from_trial_model(trial) for trial in trial_models]
 
         return trials
 
     def _build_frozen_trial_from_trial_model(self, trial: "models.TrialModel") -> FrozenTrial:
-
         values: Optional[List[float]]
         if trial.values:
             values = [0 for _ in trial.values]
             for value_model in trial.values:
                 values[value_model.objective] = TrialValueModel.stored_repr_to_value(
                     value_model.value, value_model.value_type
                 )
@@ -919,15 +890,14 @@
                 )
                 for v in trial.intermediate_values
             },
             trial_id=trial.trial_id,
         )
 
     def get_best_trial(self, study_id: int) -> FrozenTrial:
-
         with _create_scoped_session(self.scoped_session) as session:
             _directions = self.get_study_directions(study_id)
             if len(_directions) > 1:
                 raise RuntimeError(
                     "Best trial can be obtained only for single-objective optimization."
                 )
             direction = _directions[0]
@@ -938,15 +908,14 @@
                 trial = models.TrialModel.find_min_value_trial(study_id, 0, session)
             trial_id = trial.trial_id
 
         return self.get_trial(trial_id)
 
     @staticmethod
     def _set_default_engine_kwargs_for_mysql(url: str, engine_kwargs: Dict[str, Any]) -> None:
-
         # Skip if RDB is not MySQL.
         if not url.startswith("mysql"):
             return
 
         # Do not overwrite value.
         if "pool_pre_ping" in engine_kwargs:
             return
@@ -956,15 +925,14 @@
         # errors. For further details, please refer to the following document:
         # https://docs.sqlalchemy.org/en/13/core/pooling.html#pool-disconnects-pessimistic
         engine_kwargs["pool_pre_ping"] = True
         _logger.debug("pool_pre_ping=True was set to engine_kwargs to prevent connection timeout.")
 
     @staticmethod
     def _fill_storage_url_template(template: str) -> str:
-
         return template.format(SCHEMA_VERSION=models.SCHEMA_VERSION)
 
     def remove_session(self) -> None:
         """Removes the current session.
 
         A session is stored in SQLAlchemy's ThreadLocalRegistry for each thread. This method
         closes and removes the session which is associated to the current thread. Particularly,
@@ -1036,53 +1004,48 @@
                 heartbeat = trial.heartbeats[0].heartbeat
                 if (current_heartbeat - heartbeat).seconds > grace_period:
                     stale_trial_ids.append(trial.trial_id)
 
         return stale_trial_ids
 
     def get_heartbeat_interval(self) -> Optional[int]:
-
         return self.heartbeat_interval
 
     def get_failed_trial_callback(
         self,
     ) -> Optional[Callable[["optuna.study.Study", FrozenTrial], None]]:
-
         return self.failed_trial_callback
 
 
 class _VersionManager:
     def __init__(
         self,
         url: str,
         engine: "sqlalchemy.engine.Engine",
         scoped_session: "sqlalchemy_orm.scoped_session",
     ) -> None:
-
         self.url = url
         self.engine = engine
         self.scoped_session = scoped_session
         self._init_version_info_model()
         self._init_alembic()
 
     def _init_version_info_model(self) -> None:
-
         with _create_scoped_session(self.scoped_session, True) as session:
             version_info = models.VersionInfoModel.find(session)
             if version_info is not None:
                 return
 
             version_info = models.VersionInfoModel(
                 schema_version=models.SCHEMA_VERSION,
                 library_version=version.__version__,
             )
             session.add(version_info)
 
     def _init_alembic(self) -> None:
-
         logging.getLogger("alembic").setLevel(logging.WARN)
 
         with self.engine.connect() as connection:
             context = alembic_migration.MigrationContext.configure(connection)
             is_initialized = context.get_current_revision() is not None
 
             if is_initialized:
@@ -1101,15 +1064,14 @@
         with self.engine.connect() as connection:
             context = alembic_migration.MigrationContext.configure(connection)
             with connection.begin():
                 script = self._create_alembic_script()
                 context.stamp(script, revision)
 
     def check_table_schema_compatibility(self) -> None:
-
         with _create_scoped_session(self.scoped_session) as session:
             # NOTE: After invocation of `_init_version_info_model` method,
             #       it is ensured that a `VersionInfoModel` entry exists.
             version_info = models.VersionInfoModel.find(session)
 
             assert version_info is not None
 
@@ -1141,69 +1103,61 @@
             context = alembic_migration.MigrationContext.configure(connection)
             version = context.get_current_revision()
         assert version is not None
 
         return version
 
     def get_head_version(self) -> str:
-
         script = self._create_alembic_script()
         current_head = script.get_current_head()
         assert current_head is not None
         return current_head
 
     def _get_base_version(self) -> str:
-
         script = self._create_alembic_script()
         base = script.get_base()
         assert base is not None, "There should be exactly one base, i.e. v0.9.0.a."
         return base
 
     def get_all_versions(self) -> List[str]:
-
         script = self._create_alembic_script()
         return [r.revision for r in script.walk_revisions()]
 
     def upgrade(self) -> None:
-
         config = self._create_alembic_config()
         alembic_command.upgrade(config, "head")
 
         with _create_scoped_session(self.scoped_session, True) as session:
             version_info = models.VersionInfoModel.find(session)
             assert version_info is not None
             version_info.schema_version = models.SCHEMA_VERSION
             version_info.library_version = version.__version__
 
     def _is_alembic_supported(self) -> bool:
-
         with _create_scoped_session(self.scoped_session) as session:
             version_info = models.VersionInfoModel.find(session)
 
             if version_info is None:
                 # `None` means this storage was created just now.
                 return True
 
             return version_info.schema_version == models.SCHEMA_VERSION
 
     def _create_alembic_script(self) -> "alembic_script.ScriptDirectory":
-
         config = self._create_alembic_config()
         script = alembic_script.ScriptDirectory.from_config(config)
         return script
 
     def _create_alembic_config(self) -> "alembic_config.Config":
-
         alembic_dir = os.path.join(os.path.dirname(__file__), "alembic")
 
         config = alembic_config.Config(os.path.join(os.path.dirname(__file__), "alembic.ini"))
         config.set_main_option("script_location", escape_alembic_config_value(alembic_dir))
         config.set_main_option("sqlalchemy.url", escape_alembic_config_value(self.url))
         return config
 
 
 def escape_alembic_config_value(value: str) -> str:
-
     # We must escape '%' in a value string because the character
     # is regarded as the trigger of variable expansion.
     # Please see the documentation of `configparser.BasicInterpolation` for more details.
     return value.replace("%", "%%")
```

### Comparing `optuna-3.1.1/optuna/study/__init__.py` & `optuna-3.2.0/optuna/study/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/study/_dataframe.py` & `optuna-3.2.0/optuna/study/_dataframe.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict
 from typing import List
 from typing import Set
 from typing import Tuple
 
 import optuna
 from optuna._imports import try_import
+from optuna.study.study import _SYSTEM_ATTR_METRIC_NAMES
 from optuna.trial._state import TrialState
 
 
 with try_import() as _imports:
     # `Study.trials_dataframe` is disabled if pandas is not available.
     import pandas as pd
 
@@ -21,15 +22,14 @@
 
 __all__ = ["pd"]
 
 
 def _create_records_and_aggregate_column(
     study: "optuna.Study", attrs: Tuple[str, ...]
 ) -> Tuple[List[Dict[Tuple[str, str], Any]], List[Tuple[str, str]]]:
-
     attrs_to_df_columns: Dict[str, str] = collections.OrderedDict()
     for attr in attrs:
         if attr.startswith("_"):
             # Python conventional underscores are omitted in the dataframe.
             df_column = attr[1:]
         else:
             df_column = attr
@@ -37,36 +37,49 @@
 
     # column_agg is an aggregator of column names.
     # Keys of column agg are attributes of `FrozenTrial` such as 'trial_id' and 'params'.
     # Values are dataframe columns such as ('trial_id', '') and ('params', 'n_layers').
     column_agg: DefaultDict[str, Set] = collections.defaultdict(set)
     non_nested_attr = ""
 
+    metric_names = study._storage.get_study_system_attrs(study._study_id).get(
+        _SYSTEM_ATTR_METRIC_NAMES
+    )
+
     records = []
     for trial in study.get_trials(deepcopy=False):
         record = {}
         for attr, df_column in attrs_to_df_columns.items():
             value = getattr(trial, attr)
             if isinstance(value, TrialState):
                 value = value.name
             if isinstance(value, dict):
                 for nested_attr, nested_value in value.items():
                     record[(df_column, nested_attr)] = nested_value
                     column_agg[attr].add((df_column, nested_attr))
-            elif isinstance(value, list):
+            elif attr == "values":
                 # Expand trial.values.
-                for nested_attr, nested_value in enumerate(value):
+                # trial.values should be None when the trial's state is FAIL or PRUNED.
+                trial_values = [None] * len(study.directions) if value is None else value
+                iterator = (
+                    enumerate(trial_values)
+                    if metric_names is None
+                    else zip(metric_names, trial_values)
+                )
+                for nested_attr, nested_value in iterator:
                     record[(df_column, nested_attr)] = nested_value
                     column_agg[attr].add((df_column, nested_attr))
-            elif attr == "values":
-                # trial.values should be None when the trial's state is FAIL or PRUNED.
-                assert value is None
-                for nested_attr in range(len(study.directions)):
-                    record[(df_column, nested_attr)] = None
+            elif isinstance(value, list):
+                for nested_attr, nested_value in enumerate(value):
+                    record[(df_column, nested_attr)] = nested_value
                     column_agg[attr].add((df_column, nested_attr))
+            elif attr == "value":
+                nested_attr = non_nested_attr if metric_names is None else metric_names[0]
+                record[(df_column, nested_attr)] = value
+                column_agg[attr].add((df_column, nested_attr))
             else:
                 record[(df_column, non_nested_attr)] = value
                 column_agg[attr].add((df_column, non_nested_attr))
 
         records.append(record)
 
     columns: List[Tuple[str, str]] = sum(
```

### Comparing `optuna-3.1.1/optuna/study/_frozen.py` & `optuna-3.2.0/optuna/study/_frozen.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,41 +55,36 @@
         else:
             raise ValueError("Specify only one of `direction` and `directions`.")
         self.user_attrs = user_attrs
         self.system_attrs = system_attrs
         self._study_id = study_id
 
     def __eq__(self, other: Any) -> bool:
-
         if not isinstance(other, FrozenStudy):
             return NotImplemented
 
         return other.__dict__ == self.__dict__
 
     def __lt__(self, other: Any) -> bool:
-
         if not isinstance(other, FrozenStudy):
             return NotImplemented
 
         return self._study_id < other._study_id
 
     def __le__(self, other: Any) -> bool:
-
         if not isinstance(other, FrozenStudy):
             return NotImplemented
 
         return self._study_id <= other._study_id
 
     @property
     def direction(self) -> StudyDirection:
-
         if len(self._directions) > 1:
             raise RuntimeError(
                 "This attribute is not available during multi-objective optimization."
             )
 
         return self._directions[0]
 
     @property
     def directions(self) -> List[StudyDirection]:
-
         return self._directions
```

### Comparing `optuna-3.1.1/optuna/study/_multi_objective.py` & `optuna-3.2.0/optuna/study/_multi_objective.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/study/_optimize.py` & `optuna-3.2.0/optuna/study/_optimize.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/study/_study_summary.py` & `optuna-3.2.0/optuna/study/_study_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             :func:`optuna.study.Study.set_user_attr`.
         system_attrs:
             Dictionary that contains the attributes of the :class:`~optuna.study.Study` internally
             set by Optuna.
 
             .. warning::
                 Deprecated in v3.1.0. ``system_attrs`` argument will be removed in the future.
-                The removal of this feature is currently scheduled for v6.0.0,
+                The removal of this feature is currently scheduled for v5.0.0,
                 but this schedule is subject to change.
                 See https://github.com/optuna/optuna/releases/tag/v3.1.0.
         n_trials:
             The number of trials ran in the :class:`~optuna.study.Study`.
         datetime_start:
             Datetime where the :class:`~optuna.study.Study` started.
 
@@ -59,15 +59,14 @@
         system_attrs: Dict[str, Any],
         n_trials: int,
         datetime_start: Optional[datetime.datetime],
         study_id: int,
         *,
         directions: Optional[Sequence[StudyDirection]] = None,
     ):
-
         self.study_name = study_name
         if direction is None and directions is None:
             raise ValueError("Specify one of `direction` and `directions`.")
         elif directions is not None:
             self._directions = list(directions)
         elif direction is not None:
             self._directions = [direction]
@@ -77,53 +76,48 @@
         self.user_attrs = user_attrs
         self._system_attrs = system_attrs
         self.n_trials = n_trials
         self.datetime_start = datetime_start
         self._study_id = study_id
 
     def __eq__(self, other: Any) -> bool:
-
         if not isinstance(other, StudySummary):
             return NotImplemented
 
         return other.__dict__ == self.__dict__
 
     def __lt__(self, other: Any) -> bool:
-
         if not isinstance(other, StudySummary):
             return NotImplemented
 
         return self._study_id < other._study_id
 
     def __le__(self, other: Any) -> bool:
-
         if not isinstance(other, StudySummary):
             return NotImplemented
 
         return self._study_id <= other._study_id
 
     @property
     def direction(self) -> StudyDirection:
-
         if len(self._directions) > 1:
             raise RuntimeError(
                 "This attribute is not available during multi-objective optimization."
             )
 
         return self._directions[0]
 
     @property
     def directions(self) -> Sequence[StudyDirection]:
-
         return self._directions
 
     @property
     def system_attrs(self) -> Dict[str, Any]:
         warnings.warn(
             "`system_attrs` has been deprecated in v3.1.0. "
-            "The removal of this feature is currently scheduled for v6.0.0, "
+            "The removal of this feature is currently scheduled for v5.0.0, "
             "but this schedule is subject to change. "
             "See https://github.com/optuna/optuna/releases/tag/v3.1.0.",
             FutureWarning,
         )
 
         return self._system_attrs
```

### Comparing `optuna-3.1.1/optuna/study/_tell.py` & `optuna-3.2.0/optuna/study/_tell.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,17 @@
     Args:
         suppress_warning:
             If :obj:`True`, tell will not show warnings when tell receives an invalid
             values. This flag is expected to be :obj:`True` only when it is invoked by
             Study.optimize.
     """
 
+    # We must invalidate all trials cache here as it is only valid within a trial.
+    study._thread_local.cached_all_trials = None
+
     # Validate the trial argument.
     frozen_trial = _get_frozen_trial(study, trial)
     if frozen_trial.state.is_finished() and skip_if_finished:
         _logger.info(
             f"Skipped telling trial {frozen_trial.number} with values "
             f"{value_or_values} and state {state} since trial was already finished. "
             f"Finished trial has values {frozen_trial.values} and state {frozen_trial.state}."
```

### Comparing `optuna-3.1.1/optuna/study/study.py` & `optuna-3.2.0/optuna/study/study.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any
 from typing import Callable
 from typing import cast
 from typing import Container
 from typing import Dict
 from typing import Iterable
 from typing import List
+from typing import Mapping
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import Union
 import warnings
@@ -22,18 +23,19 @@
 from optuna import logging
 from optuna import pruners
 from optuna import samplers
 from optuna import storages
 from optuna import trial as trial_module
 from optuna._convert_positional_args import convert_positional_args
 from optuna._deprecated import deprecated_func
+from optuna._experimental import experimental_func
 from optuna._imports import _LazyImport
+from optuna._typing import JSONSerializable
 from optuna.distributions import _convert_old_distribution_to_new_distribution
 from optuna.distributions import BaseDistribution
-from optuna.storages._cached_storage import _CachedStorage
 from optuna.storages._heartbeat import is_heartbeat_enabled
 from optuna.study._multi_objective import _get_pareto_front_trials
 from optuna.study._optimize import _optimize
 from optuna.study._study_direction import StudyDirection
 from optuna.study._study_summary import StudySummary  # NOQA
 from optuna.study._tell import _tell_with_warning
 from optuna.trial import create_trial
@@ -44,21 +46,23 @@
 _dataframe = _LazyImport("optuna.study._dataframe")
 
 if TYPE_CHECKING:
     from optuna.study._dataframe import pd
 
 
 ObjectiveFuncType = Callable[[trial_module.Trial], Union[float, Sequence[float]]]
+_SYSTEM_ATTR_METRIC_NAMES = "study:metric_names"
 
 
 _logger = logging.get_logger(__name__)
 
 
 class _ThreadLocalStudyAttribute(threading.local):
     in_optimize_loop: bool = False
+    cached_all_trials: Optional[List["FrozenTrial"]] = None
 
 
 class Study:
     """A study corresponds to an optimization task, i.e., a set of trials.
 
     This object provides interfaces to run a new :class:`~optuna.trial.Trial`, access trials'
     history, set/get user-defined attributes of the study itself.
@@ -72,36 +76,33 @@
     def __init__(
         self,
         study_name: str,
         storage: Union[str, storages.BaseStorage],
         sampler: Optional["samplers.BaseSampler"] = None,
         pruner: Optional[pruners.BasePruner] = None,
     ) -> None:
-
         self.study_name = study_name
         storage = storages.get_storage(storage)
         study_id = storage.get_study_id_from_name(study_name)
         self._study_id = study_id
         self._storage = storage
         self._directions = storage.get_study_directions(study_id)
 
         self.sampler = sampler or samplers.TPESampler()
         self.pruner = pruner or pruners.MedianPruner()
 
         self._thread_local = _ThreadLocalStudyAttribute()
         self._stop_flag = False
 
     def __getstate__(self) -> Dict[Any, Any]:
-
         state = self.__dict__.copy()
         del state["_thread_local"]
         return state
 
     def __setstate__(self, state: Dict[Any, Any]) -> None:
-
         self.__dict__.update(state)
         self._thread_local = _ThreadLocalStudyAttribute()
 
     @property
     def best_params(self) -> Dict[str, Any]:
         """Return parameters of the best trial in the study.
 
@@ -259,16 +260,33 @@
                 the study may corrupt and unexpected behavior may happen.
             states:
                 Trial states to filter on. If :obj:`None`, include all states.
 
         Returns:
             A list of :class:`~optuna.trial.FrozenTrial` objects.
         """
-        if isinstance(self._storage, _CachedStorage):
-            self._storage.read_trials_from_remote_storage(self._study_id)
+        return self._get_trials(deepcopy, states, use_cache=False)
+
+    def _get_trials(
+        self,
+        deepcopy: bool = True,
+        states: Optional[Container[TrialState]] = None,
+        use_cache: bool = False,
+    ) -> List[FrozenTrial]:
+        if use_cache:
+            if self._thread_local.cached_all_trials is None:
+                self._thread_local.cached_all_trials = self._storage.get_all_trials(
+                    self._study_id, deepcopy=False
+                )
+            trials = self._thread_local.cached_all_trials
+            if states is not None:
+                filtered_trials = [t for t in trials if t.state in states]
+            else:
+                filtered_trials = trials
+            return copy.deepcopy(filtered_trials) if deepcopy else filtered_trials
 
         return self._storage.get_all_trials(self._study_id, deepcopy=deepcopy, states=states)
 
     @property
     def user_attrs(self) -> Dict[str, Any]:
         """Return user attributes.
 
@@ -304,15 +322,15 @@
         Returns:
             A dictionary containing all user attributes.
         """
 
         return copy.deepcopy(self._storage.get_study_user_attrs(self._study_id))
 
     @property
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def system_attrs(self) -> Dict[str, Any]:
         """Return system attributes.
 
         Returns:
             A dictionary containing all system attributes.
         """
 
@@ -410,15 +428,15 @@
                 .. seealso::
 
                     :ref:`out-of-memory-gc-collect`
 
             show_progress_bar:
                 Flag to show progress bars or not. To disable progress bar, set this :obj:`False`.
                 Currently, progress bar is experimental feature and disabled
-                when ``n_trials`` is :obj:`None`, ``timeout`` not is :obj:`None`, and
+                when ``n_trials`` is :obj:`None`, ``timeout`` is not :obj:`None`, and
                 ``n_jobs`` :math:`\\ne 1`.
 
         Raises:
             RuntimeError:
                 If nested invocation of this method occurs.
         """
 
@@ -506,16 +524,15 @@
         fixed_distributions = fixed_distributions or {}
         fixed_distributions = {
             key: _convert_old_distribution_to_new_distribution(dist)
             for key, dist in fixed_distributions.items()
         }
 
         # Sync storage once every trial.
-        if isinstance(self._storage, _CachedStorage):
-            self._storage.read_trials_from_remote_storage(self._study_id)
+        self._thread_local.cached_all_trials = None
 
         trial_id = self._pop_waiting_trial_id()
         if trial_id is None:
             trial_id = self._storage.create_new_trial(self._study_id)
         trial = trial_module.Trial(self, trial_id)
 
         for name, param in fixed_distributions.items():
@@ -655,15 +672,15 @@
             key: A key string of the attribute.
             value: A value of the attribute. The value should be JSON serializable.
 
         """
 
         self._storage.set_study_user_attr(self._study_id, key, value)
 
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def set_system_attr(self, key: str, value: Any) -> None:
         """Set a system attribute to the study.
 
         Note that Optuna internally uses this method to save system messages. Please use
         :func:`~optuna.study.Study.set_user_attr` to set users' attributes.
 
         Args:
@@ -730,14 +747,19 @@
 
         .. _DataFrame: http://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html
         .. _MultiIndex: https://pandas.pydata.org/pandas-docs/stable/advanced.html
 
         Note:
             If ``value`` is in ``attrs`` during multi-objective optimization, it is implicitly
             replaced with ``values``.
+
+        Note:
+            If :meth:`~optuna.study.Study.set_metric_names` is called, the ``value`` or ``values``
+            is implicitly replaced with the dictionary with the objective name as key and the
+            objective value as value.
         """
         return _dataframe._trials_dataframe(self, attrs, multi_index)
 
     def stop(self) -> None:
         """Exit from the current optimization loop after the running trials finish.
 
         This method lets the running :meth:`~optuna.study.Study.optimize` method return
@@ -895,14 +917,21 @@
         Args:
             trial: Trial to add.
 
         """
 
         trial._validate()
 
+        if trial.values is not None and len(self.directions) != len(trial.values):
+            raise ValueError(
+                f"The added trial has {len(trial.values)} values, which is different from the "
+                f"number of objectives {len(self.directions)} in the study (determined by "
+                "Study.directions)."
+            )
+
         self._storage.create_new_trial(self._study_id, template_trial=trial)
 
     def add_trials(self, trials: Iterable[FrozenTrial]) -> None:
         """Add trials to study.
 
         The trials are validated before being added.
 
@@ -937,38 +966,81 @@
             trials: Trials to add.
 
         """
 
         for trial in trials:
             self.add_trial(trial)
 
+    @experimental_func("3.2.0")
+    def set_metric_names(self, metric_names: List[str]) -> None:
+        """Set metric names.
+
+        This method names each dimension of the returned values of the objective function.
+        It is particularly useful in multi-objective optimization. The metric names are
+        mainly referenced by the visualization functions.
+
+        Example:
+
+            .. testcode::
+
+                import optuna
+                import pandas
+
+
+                def objective(trial):
+                    x = trial.suggest_float("x", 0, 10)
+                    return x**2, x + 1
+
+
+                study = optuna.create_study(directions=["minimize", "minimize"])
+                study.set_metric_names(["x**2", "x+1"])
+                study.optimize(objective, n_trials=3)
+
+                df = study.trials_dataframe(multi_index=True)
+                assert isinstance(df, pandas.DataFrame)
+                assert list(df.get("values").keys()) == ["x**2", "x+1"]
+
+        .. seealso::
+            The names set by this method are used in :meth:`~optuna.study.Study.trials_dataframe`
+            and :func:`~optuna.visualization.plot_pareto_front`.
+
+        Args:
+            metric_names: A list of metric names for the objective function.
+        """
+        if len(self.directions) != len(metric_names):
+            raise ValueError(
+                "The number of objectives must match thhe length of the metric names."
+            )
+
+        self._storage.set_study_system_attr(
+            self._study_id, _SYSTEM_ATTR_METRIC_NAMES, metric_names
+        )
+
     def _is_multi_objective(self) -> bool:
         """Return :obj:`True` if the study has multiple objectives.
 
         Returns:
             A boolean value indicates if `self.directions` has more than 1 element or not.
         """
 
         return len(self.directions) > 1
 
     def _pop_waiting_trial_id(self) -> Optional[int]:
-
         for trial in self._storage.get_all_trials(
             self._study_id, deepcopy=False, states=(TrialState.WAITING,)
         ):
             if not self._storage.set_trial_state_values(trial._trial_id, state=TrialState.RUNNING):
                 continue
 
             _logger.debug("Trial {} popped from the trial queue.".format(trial.number))
             return trial._trial_id
 
         return None
 
-    def _should_skip_enqueue(self, params: Dict[str, Any]) -> bool:
-
+    def _should_skip_enqueue(self, params: Mapping[str, JSONSerializable]) -> bool:
         for trial in self.get_trials(deepcopy=False):
             trial_params = trial.system_attrs.get("fixed_params", trial.params)
             if trial_params.keys() != params.keys():
                 # Can't have repeated trials if different params are suggested.
                 continue
 
             repeated_params: List[bool] = []
@@ -1005,27 +1077,41 @@
     ) -> None:
         self.tell(trial, values, state)
 
     def _log_completed_trial(self, trial: trial_module.FrozenTrial) -> None:
         if not _logger.isEnabledFor(logging.INFO):
             return
 
+        metric_names = self._storage.get_study_system_attrs(self._study_id).get(
+            _SYSTEM_ATTR_METRIC_NAMES
+        )
+
         if len(trial.values) > 1:
+            trial_values: Union[List[float], Dict[str, float]]
+            if metric_names is None:
+                trial_values = trial.values
+            else:
+                trial_values = {name: value for name, value in zip(metric_names, trial.values)}
             _logger.info(
                 "Trial {} finished with values: {} and parameters: {}. ".format(
-                    trial.number, trial.values, trial.params
+                    trial.number, trial_values, trial.params
                 )
             )
         elif len(trial.values) == 1:
             best_trial = self.best_trial
+            trial_value: Union[float, Dict[str, float]]
+            if metric_names is None:
+                trial_value = trial.values[0]
+            else:
+                trial_value = {metric_names[0]: trial.values[0]}
             _logger.info(
                 "Trial {} finished with value: {} and parameters: {}. "
                 "Best is trial {} with value: {}.".format(
                     trial.number,
-                    trial.values[0],
+                    trial_value,
                     trial.params,
                     best_trial.number,
                     best_trial.value,
                 )
             )
         else:
             assert False, "Should not reach."
@@ -1476,15 +1562,14 @@
     """
 
     storage = storages.get_storage(storage)
     frozen_studies = storage.get_all_studies()
     study_summaries = []
 
     for s in frozen_studies:
-
         all_trials = storage.get_all_trials(s._study_id)
         completed_trials = [t for t in all_trials if t.state == TrialState.COMPLETE]
 
         n_trials = len(all_trials)
 
         if len(s.directions) == 1:
             direction = s.direction
```

### Comparing `optuna-3.1.1/optuna/testing/samplers.py` & `optuna-3.2.0/optuna/testing/samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,27 +37,25 @@
 class FirstTrialOnlyRandomSampler(optuna.samplers.RandomSampler):
     def sample_relative(
         self,
         study: "optuna.study.Study",
         trial: "optuna.trial.FrozenTrial",
         search_space: Dict[str, BaseDistribution],
     ) -> Dict[str, float]:
-
         if len(study.trials) > 1:
             raise RuntimeError("`FirstTrialOnlyRandomSampler` only works on the first trial.")
 
         return super(FirstTrialOnlyRandomSampler, self).sample_relative(study, trial, search_space)
 
     def sample_independent(
         self,
         study: "optuna.study.Study",
         trial: "optuna.trial.FrozenTrial",
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> float:
-
         if len(study.trials) > 1:
             raise RuntimeError("`FirstTrialOnlyRandomSampler` only works on the first trial.")
 
         return super(FirstTrialOnlyRandomSampler, self).sample_independent(
             study, trial, param_name, param_distribution
         )
```

### Comparing `optuna-3.1.1/optuna/testing/storages.py` & `optuna-3.2.0/optuna/testing/storages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from __future__ import annotations
 
 import sys
-import tempfile
 from types import TracebackType
 from typing import Any
 from typing import IO
 from typing import Optional
 from typing import Type
 from typing import Union
 
 import fakeredis
 import pytest
 
 import optuna
 from optuna.storages import JournalFileStorage
+from optuna.testing.tempfile_pool import NamedTemporaryFilePool
 
 
 try:
     import distributed
-
-    _has_distributed = True
 except ImportError:
-    _has_distributed = False
+    pass
 
 STORAGE_MODES: list[Any] = [
     "inmemory",
     "sqlite",
     "cached_sqlite",
     "journal",
     "journal_redis",
@@ -48,19 +46,18 @@
 ]
 
 SQLITE3_TIMEOUT = 300
 
 
 class StorageSupplier:
     def __init__(self, storage_specifier: str, **kwargs: Any) -> None:
-
         self.storage_specifier = storage_specifier
-        self.tempfile: Optional[IO[Any]] = None
         self.extra_args = kwargs
         self.dask_client: Optional["distributed.Client"] = None
+        self.tempfile: IO[Any] | None = None
 
     def __enter__(
         self,
     ) -> Union[
         optuna.storages.InMemoryStorage,
         optuna.storages._CachedStorage,
         optuna.storages.RDBStorage,
@@ -68,45 +65,45 @@
         "optuna.integration.DaskStorage",
     ]:
         if self.storage_specifier == "inmemory":
             if len(self.extra_args) > 0:
                 raise ValueError("InMemoryStorage does not accept any arguments!")
             return optuna.storages.InMemoryStorage()
         elif "sqlite" in self.storage_specifier:
-            self.tempfile = tempfile.NamedTemporaryFile()
+            self.tempfile = NamedTemporaryFilePool().tempfile()
             url = "sqlite:///{}".format(self.tempfile.name)
             rdb_storage = optuna.storages.RDBStorage(
                 url,
                 engine_kwargs={"connect_args": {"timeout": SQLITE3_TIMEOUT}},
                 **self.extra_args,
             )
             return (
                 optuna.storages._CachedStorage(rdb_storage)
                 if "cached" in self.storage_specifier
                 else rdb_storage
             )
         elif self.storage_specifier == "journal_redis":
             journal_redis_storage = optuna.storages.JournalRedisStorage("redis://localhost")
             journal_redis_storage._redis = self.extra_args.get(
-                "redis", fakeredis.FakeStrictRedis()
+                "redis", fakeredis.FakeStrictRedis()  # type: ignore[no-untyped-call]
             )
             return optuna.storages.JournalStorage(journal_redis_storage)
         elif "journal" in self.storage_specifier:
-            file_storage = JournalFileStorage(tempfile.NamedTemporaryFile().name)
+            self.tempfile = NamedTemporaryFilePool().tempfile()
+            file_storage = JournalFileStorage(self.tempfile.name)
             return optuna.storages.JournalStorage(file_storage)
         elif self.storage_specifier == "dask":
             self.dask_client = distributed.Client()  # type: ignore[no-untyped-call]
 
             return optuna.integration.DaskStorage(client=self.dask_client, **self.extra_args)
         else:
             assert False
 
     def __exit__(
         self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: TracebackType
     ) -> None:
-
         if self.tempfile:
             self.tempfile.close()
 
         if self.dask_client:
             self.dask_client.shutdown()  # type: ignore[no-untyped-call]
             self.dask_client.close()  # type: ignore[no-untyped-call]
```

### Comparing `optuna-3.1.1/optuna/testing/threading.py` & `optuna-3.2.0/optuna/testing/threading.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/testing/visualization.py` & `optuna-3.2.0/optuna/testing/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 
 def prepare_study_with_trials(
     n_objectives: int = 1,
     direction: str = "minimize",
     value_for_first_trial: float = 0.0,
 ) -> Study:
-
     """Return a dummy study object for tests.
 
     This function is added to reduce the code to set up dummy study object in each test case.
     However, you can only use this function for unit tests that are loosely coupled with the
     dummy study object. Unit tests that are tightly coupled with the study become difficult to
     read because of `Mystery Guest <http://xunitpatterns.com/Obscure%20Test.html#Mystery%20Guest>`_
     and/or `Eager Test <http://xunitpatterns.com/Obscure%20Test.html#Eager%20Test>`_ anti-patterns.
```

### Comparing `optuna-3.1.1/optuna/trial/_base.py` & `optuna-3.2.0/optuna/trial/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,38 +23,33 @@
         name: str,
         low: float,
         high: float,
         *,
         step: Optional[float] = None,
         log: bool = False,
     ) -> float:
-
         raise NotImplementedError
 
     @deprecated_func("3.0.0", "6.0.0")
     @abc.abstractmethod
     def suggest_uniform(self, name: str, low: float, high: float) -> float:
-
         raise NotImplementedError
 
     @deprecated_func("3.0.0", "6.0.0")
     @abc.abstractmethod
     def suggest_loguniform(self, name: str, low: float, high: float) -> float:
-
         raise NotImplementedError
 
     @deprecated_func("3.0.0", "6.0.0")
     @abc.abstractmethod
     def suggest_discrete_uniform(self, name: str, low: float, high: float, q: float) -> float:
-
         raise NotImplementedError
 
     @abc.abstractmethod
     def suggest_int(self, name: str, low: int, high: int, step: int = 1, log: bool = False) -> int:
-
         raise NotImplementedError
 
     @overload
     @abc.abstractmethod
     def suggest_categorical(self, name: str, choices: Sequence[None]) -> None:
         ...
 
@@ -85,65 +80,54 @@
     ) -> CategoricalChoiceType:
         ...
 
     @abc.abstractmethod
     def suggest_categorical(
         self, name: str, choices: Sequence[CategoricalChoiceType]
     ) -> CategoricalChoiceType:
-
         raise NotImplementedError
 
     @abc.abstractmethod
     def report(self, value: float, step: int) -> None:
-
         raise NotImplementedError
 
     @abc.abstractmethod
     def should_prune(self) -> bool:
-
         raise NotImplementedError
 
     @abc.abstractmethod
     def set_user_attr(self, key: str, value: Any) -> None:
-
         raise NotImplementedError
 
     @abc.abstractmethod
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def set_system_attr(self, key: str, value: Any) -> None:
-
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def params(self) -> Dict[str, Any]:
-
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def distributions(self) -> Dict[str, BaseDistribution]:
-
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def user_attrs(self) -> Dict[str, Any]:
-
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def system_attrs(self) -> Dict[str, Any]:
-
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def datetime_start(self) -> Optional[datetime.datetime]:
-
         raise NotImplementedError
 
     @property
     def number(self) -> int:
-
         raise NotImplementedError
```

### Comparing `optuna-3.1.1/optuna/trial/_fixed.py` & `optuna-3.2.0/optuna/trial/_fixed.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from optuna.distributions import CategoricalChoiceType
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.trial._base import BaseTrial
 
 
-_suggest_deprecated_msg = "Use :func:`~optuna.trial.FixedTrial.suggest_float` instead."
+_suggest_deprecated_msg = "Use suggest_float{args} instead."
 
 
 class FixedTrial(BaseTrial):
     """A trial class which suggests a fixed value for each parameter.
 
     This object has the same methods as :class:`~optuna.trial.Trial`, and it suggests pre-defined
     parameter values. The parameter values can be determined at the construction of the
@@ -54,15 +54,14 @@
             A dictionary containing all parameters.
         number:
             A trial number. Defaults to ``0``.
 
     """
 
     def __init__(self, params: Dict[str, Any], number: int = 0) -> None:
-
         self._params = params
         self._suggested_params: Dict[str, Any] = {}
         self._distributions: Dict[str, BaseDistribution] = {}
         self._user_attrs: Dict[str, Any] = {}
         self._system_attrs: Dict[str, Any] = {}
         self._datetime_start = datetime.datetime.now()
         self._number = number
@@ -72,30 +71,26 @@
         name: str,
         low: float,
         high: float,
         *,
         step: Optional[float] = None,
         log: bool = False,
     ) -> float:
-
         return self._suggest(name, FloatDistribution(low, high, log=log, step=step))
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args=""))
     def suggest_uniform(self, name: str, low: float, high: float) -> float:
-
         return self.suggest_float(name, low, high)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., log=True)"))
     def suggest_loguniform(self, name: str, low: float, high: float) -> float:
-
         return self.suggest_float(name, low, high, log=True)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., step=...)"))
     def suggest_discrete_uniform(self, name: str, low: float, high: float, q: float) -> float:
-
         return self.suggest_float(name, low, high, step=q)
 
     def suggest_int(self, name: str, low: int, high: int, step: int = 1, log: bool = False) -> int:
         return int(self._suggest(name, IntDistribution(low, high, log=log, step=step)))
 
     @overload
     def suggest_categorical(self, name: str, choices: Sequence[None]) -> None:
@@ -122,36 +117,30 @@
         self, name: str, choices: Sequence[CategoricalChoiceType]
     ) -> CategoricalChoiceType:
         ...
 
     def suggest_categorical(
         self, name: str, choices: Sequence[CategoricalChoiceType]
     ) -> CategoricalChoiceType:
-
         return self._suggest(name, CategoricalDistribution(choices=choices))
 
     def report(self, value: float, step: int) -> None:
-
         pass
 
     def should_prune(self) -> bool:
-
         return False
 
     def set_user_attr(self, key: str, value: Any) -> None:
-
         self._user_attrs[key] = value
 
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def set_system_attr(self, key: str, value: Any) -> None:
-
         self._system_attrs[key] = value
 
     def _suggest(self, name: str, distribution: BaseDistribution) -> Any:
-
         if name not in self._params:
             raise ValueError(
                 "The value of the parameter '{}' is not found. Please set it at "
                 "the construction of the FixedTrial object.".format(name)
             )
 
         value = self._params[name]
@@ -168,34 +157,28 @@
         self._suggested_params[name] = value
         self._distributions[name] = distribution
 
         return value
 
     @property
     def params(self) -> Dict[str, Any]:
-
         return self._suggested_params
 
     @property
     def distributions(self) -> Dict[str, BaseDistribution]:
-
         return self._distributions
 
     @property
     def user_attrs(self) -> Dict[str, Any]:
-
         return self._user_attrs
 
     @property
     def system_attrs(self) -> Dict[str, Any]:
-
         return self._system_attrs
 
     @property
     def datetime_start(self) -> Optional[datetime.datetime]:
-
         return self._datetime_start
 
     @property
     def number(self) -> int:
-
         return self._number
```

### Comparing `optuna-3.1.1/optuna/trial/_frozen.py` & `optuna-3.2.0/optuna/trial/_frozen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import datetime
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
+from typing import Mapping
 from typing import Optional
 from typing import overload
 from typing import Sequence
 import warnings
 
 from optuna import distributions
 from optuna import logging
 from optuna._deprecated import deprecated_func
+from optuna._typing import JSONSerializable
 from optuna.distributions import _convert_old_distribution_to_new_distribution
 from optuna.distributions import BaseDistribution
 from optuna.distributions import CategoricalChoiceType
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.trial._base import BaseTrial
 from optuna.trial._state import TrialState
 
 
 _logger = logging.get_logger(__name__)
-_suggest_deprecated_msg = "Use :func:`~optuna.trial.FrozenTrial.suggest_float` instead."
+_suggest_deprecated_msg = "Use suggest_float{args} instead."
 
 
 class FrozenTrial(BaseTrial):
     """Status and results of a :class:`~optuna.trial.Trial`.
 
     An object of this class has the same methods as :class:`~optuna.trial.Trial`, but is not
     associated with, nor has any references to a :class:`~optuna.study.Study`.
@@ -144,15 +147,14 @@
         user_attrs: Dict[str, Any],
         system_attrs: Dict[str, Any],
         intermediate_values: Dict[int, float],
         trial_id: int,
         *,
         values: Optional[Sequence[float]] = None,
     ) -> None:
-
         self._number = number
         self.state = state
         self._values: Optional[List[float]] = None
         if value is not None and values is not None:
             raise ValueError("Specify only one of `value` and `values`.")
         elif value is not None:
             self._values = [value]
@@ -164,39 +166,34 @@
         self._user_attrs = user_attrs
         self._system_attrs = system_attrs
         self.intermediate_values = intermediate_values
         self._distributions = distributions
         self._trial_id = trial_id
 
     def __eq__(self, other: Any) -> bool:
-
         if not isinstance(other, FrozenTrial):
             return NotImplemented
         return other.__dict__ == self.__dict__
 
     def __lt__(self, other: Any) -> bool:
-
         if not isinstance(other, FrozenTrial):
             return NotImplemented
 
         return self.number < other.number
 
     def __le__(self, other: Any) -> bool:
-
         if not isinstance(other, FrozenTrial):
             return NotImplemented
 
         return self.number <= other.number
 
     def __hash__(self) -> int:
-
         return hash(tuple(getattr(self, field) for field in self.__dict__))
 
     def __repr__(self) -> str:
-
         return "{cls}({kwargs})".format(
             cls=self.__class__.__name__,
             kwargs=", ".join(
                 "{field}={value}".format(
                     field=field if not field.startswith("_") else field[1:],
                     value=repr(getattr(self, field)),
                 )
@@ -210,30 +207,26 @@
         name: str,
         low: float,
         high: float,
         *,
         step: Optional[float] = None,
         log: bool = False,
     ) -> float:
-
         return self._suggest(name, FloatDistribution(low, high, log=log, step=step))
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args=""))
     def suggest_uniform(self, name: str, low: float, high: float) -> float:
-
         return self.suggest_float(name, low, high)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., log=True)"))
     def suggest_loguniform(self, name: str, low: float, high: float) -> float:
-
         return self.suggest_float(name, low, high, log=True)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., step=...)"))
     def suggest_discrete_uniform(self, name: str, low: float, high: float, q: float) -> float:
-
         return self.suggest_float(name, low, high, step=q)
 
     def suggest_int(self, name: str, low: int, high: int, step: int = 1, log: bool = False) -> int:
         return int(self._suggest(name, IntDistribution(low, high, log=log, step=step)))
 
     @overload
     def suggest_categorical(self, name: str, choices: Sequence[None]) -> None:
@@ -260,15 +253,14 @@
         self, name: str, choices: Sequence[CategoricalChoiceType]
     ) -> CategoricalChoiceType:
         ...
 
     def suggest_categorical(
         self, name: str, choices: Sequence[CategoricalChoiceType]
     ) -> CategoricalChoiceType:
-
         return self._suggest(name, CategoricalDistribution(choices=choices))
 
     def report(self, value: float, step: int) -> None:
         """Interface of report function.
 
         Since :class:`~optuna.trial.FrozenTrial` is not pruned,
         this report function does nothing.
@@ -299,24 +291,21 @@
         Returns:
             :obj:`False`.
         """
 
         return False
 
     def set_user_attr(self, key: str, value: Any) -> None:
-
         self._user_attrs[key] = value
 
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def set_system_attr(self, key: str, value: Any) -> None:
-
         self._system_attrs[key] = value
 
     def _validate(self) -> None:
-
         if self.state != TrialState.WAITING and self.datetime_start is None:
             raise ValueError(
                 "`datetime_start` is supposed to be set when the trial state is not waiting."
             )
 
         if self.state.is_finished():
             if self.datetime_complete is None:
@@ -344,15 +333,14 @@
             if not distribution._contains(param_value_in_internal_repr):
                 raise ValueError(
                     "The value {} of parameter '{}' isn't contained in the distribution "
                     "{}.".format(param_value, param_name, distribution)
                 )
 
     def _suggest(self, name: str, distribution: BaseDistribution) -> Any:
-
         if name not in self._params:
             raise ValueError(
                 "The value of the parameter '{}' is not found. Please set it at "
                 "the construction of the FrozenTrial object.".format(name)
             )
 
         value = self._params[name]
@@ -368,36 +356,32 @@
 
         self._distributions[name] = distribution
 
         return value
 
     @property
     def number(self) -> int:
-
         return self._number
 
     @number.setter
     def number(self, value: int) -> None:
-
         self._number = value
 
     @property
     def value(self) -> Optional[float]:
-
         if self._values is not None:
             if len(self._values) > 1:
                 raise RuntimeError(
                     "This attribute is not available during multi-objective optimization."
                 )
             return self._values[0]
         return None
 
     @value.setter
     def value(self, v: Optional[float]) -> None:
-
         if self._values is not None:
             if len(self._values) > 1:
                 raise RuntimeError(
                     "This attribute is not available during multi-objective optimization."
                 )
 
         if v is not None:
@@ -405,75 +389,63 @@
         else:
             self._values = None
 
     # These `_get_values`, `_set_values`, and `values = property(_get_values, _set_values)` are
     # defined to pass the mypy.
     # See https://github.com/python/mypy/issues/3004#issuecomment-726022329.
     def _get_values(self) -> Optional[List[float]]:
-
         return self._values
 
     def _set_values(self, v: Optional[Sequence[float]]) -> None:
-
         if v is not None:
             self._values = list(v)
         else:
             self._values = None
 
     values = property(_get_values, _set_values)
 
     @property
     def datetime_start(self) -> Optional[datetime.datetime]:
-
         return self._datetime_start
 
     @datetime_start.setter
     def datetime_start(self, value: Optional[datetime.datetime]) -> None:
-
         self._datetime_start = value
 
     @property
     def params(self) -> Dict[str, Any]:
-
         return self._params
 
     @params.setter
     def params(self, params: Dict[str, Any]) -> None:
-
         self._params = params
 
     @property
     def distributions(self) -> Dict[str, BaseDistribution]:
-
         return self._distributions
 
     @distributions.setter
     def distributions(self, value: Dict[str, BaseDistribution]) -> None:
-
         self._distributions = value
 
     @property
     def user_attrs(self) -> Dict[str, Any]:
-
         return self._user_attrs
 
     @user_attrs.setter
     def user_attrs(self, value: Dict[str, Any]) -> None:
-
         self._user_attrs = value
 
     @property
     def system_attrs(self) -> Dict[str, Any]:
-
         return self._system_attrs
 
     @system_attrs.setter
-    def system_attrs(self, value: Dict[str, Any]) -> None:
-
-        self._system_attrs = value
+    def system_attrs(self, value: Mapping[str, JSONSerializable]) -> None:
+        self._system_attrs = cast(Dict[str, Any], value)
 
     @property
     def last_step(self) -> Optional[int]:
         """Return the maximum step of :attr:`intermediate_values` in the trial.
 
         Returns:
             The maximum step of intermediates.
```

### Comparing `optuna-3.1.1/optuna/trial/_state.py` & `optuna-3.2.0/optuna/trial/_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     RUNNING = 0
     COMPLETE = 1
     PRUNED = 2
     FAIL = 3
     WAITING = 4
 
     def __repr__(self) -> str:
-
         return str(self)
 
     def is_finished(self) -> bool:
         """Return a bool value to represent whether the trial state is unfinished or not.
 
         The unfinished state is either ``RUNNING`` or ``WAITING``.
         """
```

### Comparing `optuna-3.1.1/optuna/trial/_trial.py` & `optuna-3.2.0/optuna/trial/_trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from collections import UserDict
 import copy
 import datetime
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import overload
 from typing import Sequence
@@ -18,15 +21,15 @@
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.trial import FrozenTrial
 from optuna.trial._base import BaseTrial
 
 
 _logger = logging.get_logger(__name__)
-_suggest_deprecated_msg = "Use :func:`~optuna.trial.Trial.suggest_float` instead."
+_suggest_deprecated_msg = "Use suggest_float{args} instead."
 
 
 class Trial(BaseTrial):
     """A trial is a process of evaluating an objective function.
 
     This object is passed to an objective function and provides interfaces to get parameter
     suggestion, manage the trial's state, and set/get user-defined attributes of the trial.
@@ -41,49 +44,50 @@
             A :class:`~optuna.study.Study` object.
         trial_id:
             A trial ID that is automatically generated.
 
     """
 
     def __init__(self, study: "optuna.study.Study", trial_id: int) -> None:
-
         self.study = study
         self._trial_id = trial_id
 
         # TODO(Yanase): Remove _study_id attribute, and use study._study_id instead.
         self._study_id = self.study._study_id
         self.storage = self.study._storage
 
-        self._init_relative_params()
-
-    def _init_relative_params(self) -> None:
-
         self._cached_frozen_trial = self.storage.get_trial(self._trial_id)
         study = pruners._filter_study(self.study, self._cached_frozen_trial)
 
         self.relative_search_space = self.study.sampler.infer_relative_search_space(
             study, self._cached_frozen_trial
         )
-        self.relative_params = self.study.sampler.sample_relative(
-            study, self._cached_frozen_trial, self.relative_search_space
-        )
+        self._relative_params: Optional[Dict[str, Any]] = None
+        self._fixed_params = self._cached_frozen_trial.system_attrs.get("fixed_params", {})
+
+    @property
+    def relative_params(self) -> Dict[str, Any]:
+        if self._relative_params is None:
+            study = pruners._filter_study(self.study, self._cached_frozen_trial)
+            self._relative_params = self.study.sampler.sample_relative(
+                study, self._cached_frozen_trial, self.relative_search_space
+            )
+        return self._relative_params
 
     def suggest_float(
         self,
         name: str,
         low: float,
         high: float,
         *,
         step: Optional[float] = None,
         log: bool = False,
     ) -> float:
         """Suggest a value for the floating point parameter.
 
-        .. versionadded:: 1.3.0
-
         Example:
 
             Suggest a momentum, learning rate and scaling factor of learning rate
             for neural network training.
 
             .. testcode::
 
@@ -154,15 +158,15 @@
         """
 
         distribution = FloatDistribution(low, high, log=log, step=step)
         suggested_value = self._suggest(name, distribution)
         self._check_distribution(name, distribution)
         return suggested_value
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args=""))
     def suggest_uniform(self, name: str, low: float, high: float) -> float:
         """Suggest a value for the continuous parameter.
 
         The value is sampled from the range :math:`[\\mathsf{low}, \\mathsf{high})`
         in the linear domain. When :math:`\\mathsf{low} = \\mathsf{high}`, the value of
         :math:`\\mathsf{low}` will be returned.
 
@@ -176,15 +180,15 @@
 
         Returns:
             A suggested float value.
         """
 
         return self.suggest_float(name, low, high)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., log=True)"))
     def suggest_loguniform(self, name: str, low: float, high: float) -> float:
         """Suggest a value for the continuous parameter.
 
         The value is sampled from the range :math:`[\\mathsf{low}, \\mathsf{high})`
         in the log domain. When :math:`\\mathsf{low} = \\mathsf{high}`, the value of
         :math:`\\mathsf{low}` will be returned.
 
@@ -198,15 +202,15 @@
 
         Returns:
             A suggested float value.
         """
 
         return self.suggest_float(name, low, high, log=True)
 
-    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg)
+    @deprecated_func("3.0.0", "6.0.0", text=_suggest_deprecated_msg.format(args="(..., step=...)"))
     def suggest_discrete_uniform(self, name: str, low: float, high: float, q: float) -> float:
         """Suggest a value for the discrete parameter.
 
         The value is sampled from the range :math:`[\\mathsf{low}, \\mathsf{high}]`,
         and the step of discretization is :math:`q`. More specifically,
         this method returns one of the values in the sequence
         :math:`\\mathsf{low}, \\mathsf{low} + q, \\mathsf{low} + 2 q, \\dots,
@@ -522,15 +526,15 @@
         """
 
         if len(self.study.directions) > 1:
             raise NotImplementedError(
                 "Trial.should_prune is not supported for multi-objective optimization."
             )
 
-        trial = copy.deepcopy(self._get_latest_trial())
+        trial = self._get_latest_trial()
         return self.study.pruner.prune(self.study, trial)
 
     def set_user_attr(self, key: str, value: Any) -> None:
         """Set user attributes to the trial.
 
         The user attributes in the trial can be access via :func:`optuna.trial.Trial.user_attrs`.
 
@@ -582,15 +586,15 @@
             value:
                 A value of the attribute. The value should be JSON serializable.
         """
 
         self.storage.set_trial_user_attr(self._trial_id, key, value)
         self._cached_frozen_trial.user_attrs[key] = value
 
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def set_system_attr(self, key: str, value: Any) -> None:
         """Set system attributes to the trial.
 
         Note that Optuna internally uses this method to save system messages such as failure
         reason of trials. Please use :func:`~optuna.trial.Trial.set_user_attr` to set users'
         attributes.
 
@@ -601,27 +605,26 @@
                 A value of the attribute. The value should be JSON serializable.
         """
 
         self.storage.set_trial_system_attr(self._trial_id, key, value)
         self._cached_frozen_trial.system_attrs[key] = value
 
     def _suggest(self, name: str, distribution: BaseDistribution) -> Any:
-
         storage = self.storage
         trial_id = self._trial_id
 
         trial = self._get_latest_trial()
 
         if name in trial.distributions:
             # No need to sample if already suggested.
             distributions.check_distribution_compatibility(trial.distributions[name], distribution)
             param_value = trial.params[name]
         else:
             if self._is_fixed_param(name, distribution):
-                param_value = trial.system_attrs["fixed_params"][name]
+                param_value = self._fixed_params[name]
             elif distribution.single():
                 param_value = distributions._get_single_value(distribution)
             elif self._is_relative_param(name, distribution):
                 param_value = self.relative_params[name]
             else:
                 study = pruners._filter_study(self.study, trial)
                 param_value = self.study.sampler.sample_independent(
@@ -633,35 +636,29 @@
             storage.set_trial_param(trial_id, name, param_value_in_internal_repr, distribution)
 
             self._cached_frozen_trial.distributions[name] = distribution
             self._cached_frozen_trial.params[name] = param_value
         return param_value
 
     def _is_fixed_param(self, name: str, distribution: BaseDistribution) -> bool:
-
-        system_attrs = self._cached_frozen_trial.system_attrs
-        if "fixed_params" not in system_attrs:
-            return False
-
-        if name not in system_attrs["fixed_params"]:
+        if name not in self._fixed_params:
             return False
 
-        param_value = system_attrs["fixed_params"][name]
+        param_value = self._fixed_params[name]
         param_value_in_internal_repr = distribution.to_internal_repr(param_value)
 
         contained = distribution._contains(param_value_in_internal_repr)
         if not contained:
             warnings.warn(
                 "Fixed parameter '{}' with value {} is out of range "
                 "for distribution {}.".format(name, param_value, distribution)
             )
         return True
 
     def _is_relative_param(self, name: str, distribution: BaseDistribution) -> bool:
-
         if name not in self.relative_params:
             return False
 
         if name not in self.relative_search_space:
             raise ValueError(
                 "The parameter '{}' was sampled by `sample_relative` method "
                 "but it is not contained in the relative search space.".format(name)
@@ -671,33 +668,34 @@
         distributions.check_distribution_compatibility(relative_distribution, distribution)
 
         param_value = self.relative_params[name]
         param_value_in_internal_repr = distribution.to_internal_repr(param_value)
         return distribution._contains(param_value_in_internal_repr)
 
     def _check_distribution(self, name: str, distribution: BaseDistribution) -> None:
-
         old_distribution = self._cached_frozen_trial.distributions.get(name, distribution)
         if old_distribution != distribution:
             warnings.warn(
                 'Inconsistent parameter values for distribution with name "{}"! '
                 "This might be a configuration mistake. "
                 "Optuna allows to call the same distribution with the same "
                 "name more than once in a trial. "
                 "When the parameter values are inconsistent optuna only "
                 "uses the values of the first call and ignores all following. "
                 "Using these values: {}".format(name, old_distribution._asdict()),
                 RuntimeWarning,
             )
 
     def _get_latest_trial(self) -> FrozenTrial:
-        # TODO(eukaryo): Remove this method after `system_attrs` property is deprecated.
-        system_attrs = copy.deepcopy(self.storage.get_trial_system_attrs(self._trial_id))
-        self._cached_frozen_trial.system_attrs = system_attrs
-        return self._cached_frozen_trial
+        # TODO(eukaryo): Remove this method after `system_attrs` property is removed.
+        latest_trial = copy.deepcopy(self._cached_frozen_trial)
+        latest_trial.system_attrs = _LazyTrialSystemAttrs(  # type: ignore[assignment]
+            self._trial_id, self.storage
+        )
+        return latest_trial
 
     @property
     def params(self) -> Dict[str, Any]:
         """Return parameters to be optimized.
 
         Returns:
             A dictionary containing all parameters.
@@ -722,15 +720,15 @@
         Returns:
             A dictionary containing all user attributes.
         """
 
         return copy.deepcopy(self._cached_frozen_trial.user_attrs)
 
     @property
-    @deprecated_func("3.1.0", "6.0.0")
+    @deprecated_func("3.1.0", "5.0.0")
     def system_attrs(self) -> Dict[str, Any]:
         """Return system attributes.
 
         Returns:
             A dictionary containing all system attributes.
         """
 
@@ -750,7 +748,22 @@
         """Return trial's number which is consecutive and unique in a study.
 
         Returns:
             A trial number.
         """
 
         return self._cached_frozen_trial.number
+
+
+class _LazyTrialSystemAttrs(UserDict):
+    def __init__(self, trial_id: int, storage: optuna.storages.BaseStorage) -> None:
+        super().__init__()
+        self._trial_id = trial_id
+        self._storage = storage
+        self._initialized = False
+
+    def __getattribute__(self, key: str) -> Any:
+        if key == "data":
+            if not self._initialized:
+                self._initialized = True
+                super().update(self._storage.get_trial_system_attrs(self._trial_id))
+        return super().__getattribute__(key)
```

### Comparing `optuna-3.1.1/optuna/visualization/__init__.py` & `optuna-3.2.0/optuna/visualization/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 from optuna.visualization._contour import plot_contour
 from optuna.visualization._edf import plot_edf
 from optuna.visualization._intermediate_values import plot_intermediate_values
 from optuna.visualization._optimization_history import plot_optimization_history
 from optuna.visualization._parallel_coordinate import plot_parallel_coordinate
 from optuna.visualization._param_importances import plot_param_importances
 from optuna.visualization._pareto_front import plot_pareto_front
+from optuna.visualization._rank import plot_rank
 from optuna.visualization._slice import plot_slice
+from optuna.visualization._terminator_improvement import plot_terminator_improvement
+from optuna.visualization._timeline import plot_timeline
 from optuna.visualization._utils import is_available
 
 
 __all__ = [
     "is_available",
     "matplotlib",
     "plot_contour",
     "plot_edf",
     "plot_intermediate_values",
     "plot_optimization_history",
     "plot_parallel_coordinate",
     "plot_param_importances",
     "plot_pareto_front",
     "plot_slice",
+    "plot_rank",
+    "plot_terminator_improvement",
+    "plot_timeline",
 ]
```

### Comparing `optuna-3.1.1/optuna/visualization/_contour.py` & `optuna-3.2.0/optuna/visualization/_contour.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+from __future__ import annotations
+
 import math
 from typing import Callable
-from typing import Dict
-from typing import List
 from typing import NamedTuple
-from typing import Optional
-from typing import Tuple
-from typing import Union
 
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 from optuna.visualization._plotly_imports import _imports
 from optuna.visualization._utils import _check_plot_args
@@ -30,39 +27,39 @@
 
 
 PADDING_RATIO = 0.05
 
 
 class _AxisInfo(NamedTuple):
     name: str
-    range: Tuple[float, float]
+    range: tuple[float, float]
     is_log: bool
     is_cat: bool
-    indices: List[Union[str, int, float]]
-    values: List[Union[str, float, None]]
+    indices: list[str | int | float]
+    values: list[str | float | None]
 
 
 class _SubContourInfo(NamedTuple):
     xaxis: _AxisInfo
     yaxis: _AxisInfo
-    z_values: Dict[Tuple[int, int], float]
+    z_values: dict[tuple[int, int], float]
 
 
 class _ContourInfo(NamedTuple):
-    sorted_params: List[str]
-    sub_plot_infos: List[List[_SubContourInfo]]
+    sorted_params: list[str]
+    sub_plot_infos: list[list[_SubContourInfo]]
     reverse_scale: bool
     target_name: str
 
 
 def plot_contour(
     study: Study,
-    params: Optional[List[str]] = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "go.Figure":
     """Plot the parameter relationship as contour plot in a study.
 
     Note that, if a parameter contains missing values, a trial with missing values is not plotted.
 
     Example:
@@ -111,15 +108,14 @@
 
     _imports.check()
     info = _get_contour_info(study, params, target, target_name)
     return _get_contour_plot(info)
 
 
 def _get_contour_plot(info: _ContourInfo) -> "go.Figure":
-
     layout = go.Layout(title="Contour Plot")
 
     sorted_params = info.sorted_params
     sub_plot_infos = info.sub_plot_infos
     reverse_scale = info.reverse_scale
     target_name = info.target_name
 
@@ -193,16 +189,15 @@
     return figure
 
 
 def _get_contour_subplot(
     info: _SubContourInfo,
     reverse_scale: bool,
     target_name: str = "Objective Value",
-) -> Tuple["Contour", "Scatter"]:
-
+) -> tuple["Contour", "Scatter"]:
     x_indices = info.xaxis.indices
     y_indices = info.yaxis.indices
     x_values = []
     y_values = []
     for x_value, y_value in zip(info.xaxis.values, info.yaxis.values):
         if x_value is not None and y_value is not None:
             x_values.append(x_value)
@@ -239,19 +234,18 @@
     )
 
     return contour, scatter
 
 
 def _get_contour_info(
     study: Study,
-    params: Optional[List[str]] = None,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    params: list[str] | None = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> _ContourInfo:
-
     _check_plot_args(study, target, target_name)
 
     trials = _filter_nonfinite(
         study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), target=target
     )
 
     all_params = {p_name for t in trials for p_name in t.params.keys()}
@@ -265,15 +259,15 @@
             _logger.warning("The length of params must be greater than 1.")
 
         for input_p_name in params:
             if input_p_name not in all_params:
                 raise ValueError("Parameter {} does not exist in your study.".format(input_p_name))
         sorted_params = sorted(set(params))
 
-    sub_plot_infos: List[List[_SubContourInfo]]
+    sub_plot_infos: list[list[_SubContourInfo]]
     if len(sorted_params) == 2:
         x_param = sorted_params[0]
         y_param = sorted_params[1]
         sub_plot_info = _get_contour_subplot_info(trials, x_param, y_param, target)
         sub_plot_infos = [[sub_plot_info]]
     else:
         sub_plot_infos = []
@@ -290,20 +284,19 @@
         sub_plot_infos=sub_plot_infos,
         reverse_scale=reverse_scale,
         target_name=target_name,
     )
 
 
 def _get_contour_subplot_info(
-    trials: List[FrozenTrial],
+    trials: list[FrozenTrial],
     x_param: str,
     y_param: str,
-    target: Optional[Callable[[FrozenTrial], float]],
+    target: Callable[[FrozenTrial], float] | None,
 ) -> _SubContourInfo:
-
     xaxis = _get_axis_info(trials, x_param)
     yaxis = _get_axis_info(trials, y_param)
 
     if x_param == y_param:
         return _SubContourInfo(xaxis=xaxis, yaxis=yaxis, z_values={})
 
     if len(xaxis.indices) < 2:
@@ -331,16 +324,16 @@
         assert value is not None
 
         z_values[(x_i, y_i)] = value
 
     return _SubContourInfo(xaxis=xaxis, yaxis=yaxis, z_values=z_values)
 
 
-def _get_axis_info(trials: List[FrozenTrial], param_name: str) -> _AxisInfo:
-    values: List[Union[str, float, None]]
+def _get_axis_info(trials: list[FrozenTrial], param_name: str) -> _AxisInfo:
+    values: list[str | float | None]
     if _is_numerical(trials, param_name):
         values = [t.params.get(param_name) for t in trials]
     else:
         values = [
             str(t.params.get(param_name)) if param_name in t.params else None for t in trials
         ]
```

### Comparing `optuna-3.1.1/optuna/visualization/_edf.py` & `optuna-3.2.0/optuna/visualization/_edf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+from __future__ import annotations
+
 from typing import Callable
 from typing import cast
-from typing import List
 from typing import NamedTuple
-from typing import Optional
 from typing import Sequence
-from typing import Union
 
 import numpy as np
 
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
@@ -28,22 +27,22 @@
 
 class _EDFLineInfo(NamedTuple):
     study_name: str
     y_values: np.ndarray
 
 
 class _EDFInfo(NamedTuple):
-    lines: List[_EDFLineInfo]
+    lines: list[_EDFLineInfo]
     x_values: np.ndarray
 
 
 def plot_edf(
-    study: Union[Study, Sequence[Study]],
+    study: Study | Sequence[Study],
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "go.Figure":
     """Plot the objective value EDF (empirical distribution function) of a study.
 
     Note that only the complete trials are considered when plotting the EDF.
 
     .. note::
@@ -135,19 +134,18 @@
     figure = go.Figure(data=traces, layout=layout)
     figure.update_yaxes(range=[0, 1])
 
     return figure
 
 
 def _get_edf_info(
-    study: Union[Study, Sequence[Study]],
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    study: Study | Sequence[Study],
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> _EDFInfo:
-
     if isinstance(study, Study):
         studies = [study]
     else:
         studies = list(study)
 
     _check_plot_args(studies, target, target_name)
 
@@ -159,15 +157,15 @@
 
         def _target(t: FrozenTrial) -> float:
             return cast(float, t.value)
 
         target = _target
 
     study_names = []
-    all_values: List[np.ndarray] = []
+    all_values: list[np.ndarray] = []
     for study in studies:
         trials = _filter_nonfinite(
             study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), target=target
         )
 
         values = np.array([target(trial) for trial in trials])
         all_values.append(values)
@@ -178,12 +176,12 @@
         return _EDFInfo(lines=[], x_values=np.array([]))
 
     min_x_value = np.min(np.concatenate(all_values))
     max_x_value = np.max(np.concatenate(all_values))
     x_values = np.linspace(min_x_value, max_x_value, NUM_SAMPLES_X_AXIS)
 
     edf_line_info_list = []
-    for (study_name, values) in zip(study_names, all_values):
+    for study_name, values in zip(study_names, all_values):
         y_values = np.sum(values[:, np.newaxis] <= x_values, axis=0) / values.size
         edf_line_info_list.append(_EDFLineInfo(study_name=study_name, y_values=y_values))
 
     return _EDFInfo(lines=edf_line_info_list, x_values=x_values)
```

### Comparing `optuna-3.1.1/optuna/visualization/_intermediate_values.py` & `optuna-3.2.0/optuna/visualization/_intermediate_values.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import List
+from __future__ import annotations
+
 from typing import NamedTuple
-from typing import Tuple
 
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import TrialState
 from optuna.visualization._plotly_imports import _imports
 
 
@@ -12,19 +12,19 @@
     from optuna.visualization._plotly_imports import go
 
 _logger = get_logger(__name__)
 
 
 class _TrialInfo(NamedTuple):
     trial_number: int
-    sorted_intermediate_values: List[Tuple[int, float]]
+    sorted_intermediate_values: list[tuple[int, float]]
 
 
 class _IntermediatePlotInfo(NamedTuple):
-    trial_infos: List[_TrialInfo]
+    trial_infos: list[_TrialInfo]
 
 
 def _get_intermediate_plot_info(study: Study) -> _IntermediatePlotInfo:
     trials = study.get_trials(
         deepcopy=False, states=(TrialState.PRUNED, TrialState.COMPLETE, TrialState.RUNNING)
     )
     trial_infos = [
@@ -97,15 +97,14 @@
     """
 
     _imports.check()
     return _get_intermediate_plot(_get_intermediate_plot_info(study))
 
 
 def _get_intermediate_plot(info: _IntermediatePlotInfo) -> "go.Figure":
-
     layout = go.Layout(
         title="Intermediate Values Plot",
         xaxis={"title": "Step"},
         yaxis={"title": "Intermediate Value"},
         showlegend=False,
     )
```

### Comparing `optuna-3.1.1/optuna/visualization/_optimization_history.py` & `optuna-3.2.0/optuna/visualization/_optimization_history.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+from __future__ import annotations
+
 from typing import Callable
 from typing import cast
-from typing import List
 from typing import NamedTuple
-from typing import Optional
 from typing import Sequence
-from typing import Tuple
-from typing import Union
 
 import numpy as np
 
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
@@ -21,47 +19,46 @@
 if _imports.is_successful():
     from optuna.visualization._plotly_imports import go
 
 _logger = get_logger(__name__)
 
 
 class _ValuesInfo(NamedTuple):
-    values: List[float]
-    stds: Optional[List[float]]
+    values: list[float]
+    stds: list[float] | None
     label_name: str
 
 
 class _OptimizationHistoryInfo(NamedTuple):
-    trial_numbers: List[int]
+    trial_numbers: list[int]
     values_info: _ValuesInfo
-    best_values_info: Optional[_ValuesInfo]
+    best_values_info: _ValuesInfo | None
 
 
 def _get_optimization_history_info_list(
-    study: Union[Study, Sequence[Study]],
-    target: Optional[Callable[[FrozenTrial], float]],
+    study: Study | Sequence[Study],
+    target: Callable[[FrozenTrial], float] | None,
     target_name: str,
     error_bar: bool,
-) -> List[_OptimizationHistoryInfo]:
-
+) -> list[_OptimizationHistoryInfo]:
     _check_plot_args(study, target, target_name)
     if isinstance(study, Study):
         studies = [study]
     else:
         studies = list(study)
 
-    info_list: List[_OptimizationHistoryInfo] = []
+    info_list: list[_OptimizationHistoryInfo] = []
     for study in studies:
         trials = study.get_trials(states=(TrialState.COMPLETE,))
         label_name = target_name if len(studies) == 1 else f"{target_name} of {study.study_name}"
         if target is not None:
             values = [target(t) for t in trials]
             # We don't calculate best for user-defined target function since we cannot tell
             # which direction is better.
-            best_values_info: Optional[_ValuesInfo] = None
+            best_values_info: _ValuesInfo | None = None
         else:
             values = [cast(float, t.value) for t in trials]
             if study.direction == StudyDirection.MINIMIZE:
                 best_values = list(np.minimum.accumulate(values))
             else:
                 best_values = list(np.maximum.accumulate(values))
             best_label_name = (
@@ -88,40 +85,40 @@
 
     # When error_bar=True, a list of 0 or 1 element is returned.
     if len(info_list) == 0:
         return []
     all_trial_numbers = [number for info in info_list for number in info.trial_numbers]
     max_num_trial = max(all_trial_numbers) + 1
 
-    def _aggregate(label_name: str, use_best_value: bool) -> Tuple[List[int], _ValuesInfo]:
+    def _aggregate(label_name: str, use_best_value: bool) -> tuple[list[int], _ValuesInfo]:
         # Calculate mean and std of values for each trial number.
-        values: List[List[float]] = [[] for _ in range(max_num_trial)]
+        values: list[list[float]] = [[] for _ in range(max_num_trial)]
         assert info_list is not None
         for trial_numbers, values_info, best_values_info in info_list:
             if use_best_value:
                 assert best_values_info is not None
                 values_info = best_values_info
             for trial_number, value in zip(trial_numbers, values_info.values):
                 values[trial_number].append(value)
         trial_numbers_union = [i for i in range(max_num_trial) if len(values[i]) > 0]
         value_means = [np.mean(v).item() for v in values if len(v) > 0]
         value_stds = [np.std(v).item() for v in values if len(v) > 0]
         return trial_numbers_union, _ValuesInfo(value_means, value_stds, label_name)
 
     eb_trial_numbers, eb_values_info = _aggregate(target_name, False)
-    eb_best_values_info: Optional[_ValuesInfo] = None
+    eb_best_values_info: _ValuesInfo | None = None
     if target is None:
         _, eb_best_values_info = _aggregate("Best Value", True)
     return [_OptimizationHistoryInfo(eb_trial_numbers, eb_values_info, eb_best_values_info)]
 
 
 def plot_optimization_history(
-    study: Union[Study, Sequence[Study]],
+    study: Study | Sequence[Study],
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
     error_bar: bool = False,
 ) -> "go.Figure":
     """Plot optimization history of all trials in a study.
 
     Example:
 
@@ -167,18 +164,17 @@
     _imports.check()
 
     info_list = _get_optimization_history_info_list(study, target, target_name, error_bar)
     return _get_optimization_history_plot(info_list, target_name)
 
 
 def _get_optimization_history_plot(
-    info_list: List[_OptimizationHistoryInfo],
+    info_list: list[_OptimizationHistoryInfo],
     target_name: str,
 ) -> "go.Figure":
-
     layout = go.Layout(
         title="Optimization History Plot",
         xaxis={"title": "Trial"},
         yaxis={"title": target_name},
     )
 
     traces = []
```

### Comparing `optuna-3.1.1/optuna/visualization/_parallel_coordinate.py` & `optuna-3.2.0/optuna/visualization/_parallel_coordinate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
+from __future__ import annotations
+
 from collections import defaultdict
 import math
 from typing import Any
 from typing import Callable
 from typing import cast
-from typing import DefaultDict
-from typing import Dict
-from typing import List
 from typing import NamedTuple
-from typing import Optional
-from typing import Tuple
-from typing import Union
 
 import numpy as np
 
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
@@ -32,34 +28,34 @@
     from optuna.visualization._utils import COLOR_SCALE
 
 _logger = get_logger(__name__)
 
 
 class _DimensionInfo(NamedTuple):
     label: str
-    values: Tuple[float, ...]
-    range: Tuple[float, float]
+    values: tuple[float, ...]
+    range: tuple[float, float]
     is_log: bool
     is_cat: bool
-    tickvals: List[Union[int, float]]
-    ticktext: List[str]
+    tickvals: list[int | float]
+    ticktext: list[str]
 
 
 class _ParallelCoordinateInfo(NamedTuple):
     dim_objective: _DimensionInfo
-    dims_params: List[_DimensionInfo]
+    dims_params: list[_DimensionInfo]
     reverse_scale: bool
     target_name: str
 
 
 def plot_parallel_coordinate(
     study: Study,
-    params: Optional[List[str]] = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "go.Figure":
     """Plot the high-dimensional parameter relationships in a study.
 
     Note that, if a parameter contains missing values, a trial with missing values is not plotted.
 
     Example:
@@ -108,15 +104,14 @@
 
     _imports.check()
     info = _get_parallel_coordinate_info(study, params, target, target_name)
     return _get_parallel_coordinate_plot(info)
 
 
 def _get_parallel_coordinate_plot(info: _ParallelCoordinateInfo) -> "go.Figure":
-
     layout = go.Layout(title="Parallel Coordinate Plot")
 
     if len(info.dims_params) == 0 or len(info.dim_objective.values) == 0:
         return go.Figure(data=[], layout=layout)
 
     dims = _get_dims_from_info(info)
     reverse_scale = info.reverse_scale
@@ -140,19 +135,18 @@
     figure = go.Figure(data=traces, layout=layout)
 
     return figure
 
 
 def _get_parallel_coordinate_info(
     study: Study,
-    params: Optional[List[str]] = None,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    params: list[str] | None = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> _ParallelCoordinateInfo:
-
     _check_plot_args(study, target, target_name)
 
     reverse_scale = _is_reverse_scale(study, target)
 
     trials = _filter_nonfinite(
         study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), target=target
     )
@@ -201,49 +195,47 @@
         return _ParallelCoordinateInfo(
             dim_objective=dim_objective,
             dims_params=[],
             reverse_scale=reverse_scale,
             target_name=target_name,
         )
 
-    numeric_cat_params_indices: List[int] = []
+    numeric_cat_params_indices: list[int] = []
     dims = []
     for dim_index, p_name in enumerate(sorted_params, start=1):
         values = []
         for t in trials:
             if t.number in skipped_trial_numbers:
                 continue
 
             if p_name in t.params:
                 values.append(t.params[p_name])
 
         if _is_log_scale(trials, p_name):
             values = [math.log10(v) for v in values]
             min_value = min(values)
             max_value = max(values)
-            tickvals: List[Union[int, float]] = list(
-                range(math.ceil(min_value), math.ceil(max_value))
-            )
+            tickvals: list[int | float] = list(range(math.ceil(min_value), math.ceil(max_value)))
             if min_value not in tickvals:
                 tickvals = [min_value] + tickvals
             if max_value not in tickvals:
                 tickvals = tickvals + [max_value]
             dim = _DimensionInfo(
                 label=_truncate_label(p_name),
                 values=tuple(values),
                 range=(min_value, max_value),
                 is_log=True,
                 is_cat=False,
                 tickvals=tickvals,
                 ticktext=["{:.3g}".format(math.pow(10, x)) for x in tickvals],
             )
         elif _is_categorical(trials, p_name):
-            vocab: DefaultDict[Union[int, str], int] = defaultdict(lambda: len(vocab))
+            vocab: defaultdict[int | str, int] = defaultdict(lambda: len(vocab))
 
-            ticktext: List[str]
+            ticktext: list[str]
             if _is_numerical(trials, p_name):
                 _ = [vocab[v] for v in sorted(values)]
                 values = [vocab[v] for v in values]
                 ticktext = [str(v) for v in list(sorted(vocab.keys()))]
                 numeric_cat_params_indices.append(dim_index)
             else:
                 values = [vocab[v] for v in values]
@@ -297,15 +289,15 @@
         dim_objective=dim_objective,
         dims_params=dims,
         reverse_scale=reverse_scale,
         target_name=target_name,
     )
 
 
-def _get_dims_from_info(info: _ParallelCoordinateInfo) -> List[Dict[str, Any]]:
+def _get_dims_from_info(info: _ParallelCoordinateInfo) -> list[dict[str, Any]]:
     dims = [
         {
             "label": info.dim_objective.label,
             "values": info.dim_objective.values,
             "range": info.dim_objective.range,
         }
     ]
```

### Comparing `optuna-3.1.1/optuna/visualization/_param_importances.py` & `optuna-3.2.0/optuna/visualization/_param_importances.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from __future__ import annotations
+
 from collections import OrderedDict
 from typing import Callable
-from typing import List
 from typing import NamedTuple
-from typing import Optional
 
 import optuna
 from optuna.distributions import BaseDistribution
 from optuna.importance._base import BaseImportanceEvaluator
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
@@ -22,25 +22,25 @@
     from optuna.visualization._plotly_imports import go
 
 
 logger = get_logger(__name__)
 
 
 class _ImportancesInfo(NamedTuple):
-    importance_values: List[float]
-    param_names: List[str]
-    importance_labels: List[str]
+    importance_values: list[float]
+    param_names: list[str]
+    importance_labels: list[str]
     target_name: str
 
 
 def _get_importances_info(
     study: Study,
-    evaluator: Optional[BaseImportanceEvaluator],
-    params: Optional[List[str]],
-    target: Optional[Callable[[FrozenTrial], float]],
+    evaluator: BaseImportanceEvaluator | None,
+    params: list[str] | None,
+    target: Callable[[FrozenTrial], float] | None,
     target_name: str,
 ) -> _ImportancesInfo:
     _check_plot_args(study, target, target_name)
 
     trials = _filter_nonfinite(
         study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), target=target
     )
@@ -69,18 +69,18 @@
         importance_labels=importance_labels,
         target_name=target_name,
     )
 
 
 def plot_param_importances(
     study: Study,
-    evaluator: Optional[BaseImportanceEvaluator] = None,
-    params: Optional[List[str]] = None,
+    evaluator: BaseImportanceEvaluator | None = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "go.Figure":
     """Plot hyperparameter importances.
 
     Example:
 
         The following code snippet shows how to plot hyperparameter importances.
@@ -138,16 +138,15 @@
     _imports.check()
 
     importances_info = _get_importances_info(study, evaluator, params, target, target_name)
     hover_template = _get_hover_template(importances_info, study)
     return _get_importances_plot(importances_info, hover_template)
 
 
-def _get_importances_plot(info: _ImportancesInfo, hover_template: List[str]) -> "go.Figure":
-
+def _get_importances_plot(info: _ImportancesInfo, hover_template: list[str]) -> "go.Figure":
     layout = go.Layout(
         title="Hyperparameter Importances",
         xaxis={"title": f"Importance for {info.target_name}"},
         yaxis={"title": "Hyperparameter"},
         showlegend=False,
     )
 
@@ -185,14 +184,14 @@
 
 def _make_hovertext(param_name: str, importance: float, study: Study) -> str:
     return "{} ({}): {}<extra></extra>".format(
         param_name, _get_distribution(param_name, study).__class__.__name__, importance
     )
 
 
-def _get_hover_template(importances_info: _ImportancesInfo, study: Study) -> List[str]:
+def _get_hover_template(importances_info: _ImportancesInfo, study: Study) -> list[str]:
     return [
         _make_hovertext(param_name, importance, study)
         for param_name, importance in zip(
             importances_info.param_names, importances_info.importance_values
         )
     ]
```

### Comparing `optuna-3.1.1/optuna/visualization/_pareto_front.py` & `optuna-3.2.0/optuna/visualization/_pareto_front.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,52 @@
+from __future__ import annotations
+
 import collections
-import json
 from typing import Any
 from typing import Callable
-from typing import Dict
-from typing import List
 from typing import NamedTuple
-from typing import Optional
 from typing import Sequence
-from typing import Tuple
-from typing import Union
 import warnings
 
 import optuna
 from optuna.exceptions import ExperimentalWarning
 from optuna.study import Study
 from optuna.study._multi_objective import _get_pareto_front_trials_by_trials
+from optuna.study.study import _SYSTEM_ATTR_METRIC_NAMES
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 from optuna.visualization._plotly_imports import _imports
+from optuna.visualization._utils import _make_hovertext
 
 
 if _imports.is_successful():
     from optuna.visualization._plotly_imports import go
 
 _logger = optuna.logging.get_logger(__name__)
 
 
 class _ParetoFrontInfo(NamedTuple):
     n_targets: int
-    target_names: List[str]
-    best_trials_with_values: List[Tuple[FrozenTrial, List[float]]]
-    non_best_trials_with_values: List[Tuple[FrozenTrial, List[float]]]
-    infeasible_trials_with_values: List[Tuple[FrozenTrial, List[float]]]
-    axis_order: List[int]
+    target_names: list[str]
+    best_trials_with_values: list[tuple[FrozenTrial, list[float]]]
+    non_best_trials_with_values: list[tuple[FrozenTrial, list[float]]]
+    infeasible_trials_with_values: list[tuple[FrozenTrial, list[float]]]
+    axis_order: list[int]
     include_dominated_trials: bool
     has_constraints_func: bool
 
 
 def plot_pareto_front(
     study: Study,
     *,
-    target_names: Optional[List[str]] = None,
+    target_names: list[str] | None = None,
     include_dominated_trials: bool = True,
-    axis_order: Optional[List[int]] = None,
-    constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
-    targets: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
+    axis_order: list[int] | None = None,
+    constraints_func: Callable[[FrozenTrial], Sequence[float]] | None = None,
+    targets: Callable[[FrozenTrial], Sequence[float]] | None = None,
 ) -> "go.Figure":
     """Plot the Pareto front of a study.
 
     .. seealso::
         Please refer to :ref:`multi_objective` for the tutorial of the Pareto front visualization.
 
     Example:
@@ -71,14 +69,46 @@
 
             study = optuna.create_study(directions=["minimize", "minimize"])
             study.optimize(objective, n_trials=50)
 
             fig = optuna.visualization.plot_pareto_front(study)
             fig.show()
 
+    Example:
+
+        The following code snippet shows how to plot a 2-dimensional Pareto front
+        of a 3-dimensional study.
+        This example is scalable, e.g., for plotting a 2- or 3-dimensional Pareto front
+        of a 4-dimensional study and so on.
+
+        .. plotly::
+
+            import optuna
+
+            def objective(trial):
+                x = trial.suggest_float("x", 0, 5)
+                y = trial.suggest_float("y", 0, 3)
+                v0 = 5 * x ** 2 + 3 * y ** 2
+                v1 = (x - 10) ** 2 + (y - 10) ** 2
+                v2 = x + y
+
+                return v0, v1, v2
+
+            study = optuna.create_study(directions=["minimize", "minimize", "minimize"])
+
+            study.optimize(objective, n_trials=100)
+
+            fig = optuna.visualization.plot_pareto_front(
+                study,
+                targets=lambda t: (t.values[0], t.values[1]),
+                target_names=["Objective 0", "Objective 1"],
+            )
+
+            fig.show()
+
     Args:
         study:
             A :class:`~optuna.study.Study` object whose trials are plotted for their objective
             values. ``study.n_objectives`` must be either 2 or 3 when ``targets`` is :obj:`None`.
         target_names:
             Objective name list used as the axis titles. If :obj:`None` is specified,
             "Objective {objective_index}" is used instead. If ``targets`` is specified
@@ -199,19 +229,19 @@
             },
         )
     return go.Figure(data=data, layout=layout)
 
 
 def _get_pareto_front_info(
     study: Study,
-    target_names: Optional[List[str]] = None,
+    target_names: list[str] | None = None,
     include_dominated_trials: bool = True,
-    axis_order: Optional[List[int]] = None,
-    constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
-    targets: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
+    axis_order: list[int] | None = None,
+    constraints_func: Callable[[FrozenTrial], Sequence[float]] | None = None,
+    targets: Callable[[FrozenTrial], Sequence[float]] | None = None,
 ) -> _ParetoFrontInfo:
     if axis_order is not None:
         warnings.warn(
             "`axis_order` has been deprecated in v3.0.0. "
             "This feature will be removed in v5.0.0. "
             "See https://github.com/optuna/optuna/releases/tag/v3.0.0.",
             FutureWarning,
@@ -241,22 +271,21 @@
             non_best_trials = _get_non_pareto_front_trials(feasible_trials, best_trials)
         else:
             non_best_trials = []
 
         if len(best_trials) == 0:
             _logger.warning("Your study does not have any completed and feasible trials.")
     else:
-        best_trials = study.best_trials
+        all_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
+        best_trials = _get_pareto_front_trials_by_trials(all_trials, study.directions)
         if len(best_trials) == 0:
             _logger.warning("Your study does not have any completed trials.")
 
         if include_dominated_trials:
-            non_best_trials = _get_non_pareto_front_trials(
-                study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), best_trials
-            )
+            non_best_trials = _get_non_pareto_front_trials(all_trials, best_trials)
         else:
             non_best_trials = []
         infeasible_trials = []
 
     _targets = targets
     if _targets is None:
         if len(study.directions) in (2, 3):
@@ -265,33 +294,33 @@
             raise ValueError(
                 "`plot_pareto_front` function only supports 2 or 3 objective"
                 " studies when using `targets` is `None`. Please use `targets`"
                 " if your objective studies have more than 3 objectives."
             )
 
     def _make_trials_with_values(
-        trials: List[FrozenTrial],
+        trials: list[FrozenTrial],
         targets: Callable[[FrozenTrial], Sequence[float]],
-    ) -> List[Tuple[FrozenTrial, List[float]]]:
+    ) -> list[tuple[FrozenTrial, list[float]]]:
         target_values = [targets(trial) for trial in trials]
         for v in target_values:
             if not isinstance(v, collections.abc.Sequence):
                 raise ValueError(
                     "`targets` should return a sequence of target values."
                     " your `targets` returns {}".format(type(v))
                 )
         return [(trial, list(v)) for trial, v in zip(trials, target_values)]
 
     best_trials_with_values = _make_trials_with_values(best_trials, _targets)
     non_best_trials_with_values = _make_trials_with_values(non_best_trials, _targets)
     infeasible_trials_with_values = _make_trials_with_values(infeasible_trials, _targets)
 
     def _infer_n_targets(
-        trials_with_values: Sequence[Tuple[FrozenTrial, Sequence[float]]]
-    ) -> Optional[int]:
+        trials_with_values: Sequence[tuple[FrozenTrial, Sequence[float]]]
+    ) -> int | None:
         if len(trials_with_values) > 0:
             return len(trials_with_values[0][1])
         return None
 
     # Check for `non_best_trials_with_values` can be skipped, because if `best_trials_with_values`
     # is empty, then `non_best_trials_with_values` will also be empty.
     n_targets = _infer_n_targets(best_trials_with_values) or _infer_n_targets(
@@ -310,15 +339,21 @@
     if n_targets not in (2, 3):
         raise ValueError(
             "`plot_pareto_front` function only supports 2 or 3 targets."
             " you used {} targets now.".format(n_targets)
         )
 
     if target_names is None:
-        target_names = [f"Objective {i}" for i in range(n_targets)]
+        metric_names = study._storage.get_study_system_attrs(study._study_id).get(
+            _SYSTEM_ATTR_METRIC_NAMES
+        )
+        if metric_names is None:
+            target_names = [f"Objective {i}" for i in range(n_targets)]
+        else:
+            target_names = metric_names
     elif len(target_names) != n_targets:
         raise ValueError(f"The length of `target_names` is supposed to be {n_targets}.")
 
     if axis_order is None:
         axis_order = list(range(n_targets))
     else:
         if len(axis_order) != n_targets:
@@ -352,42 +387,32 @@
 
 
 def _targets_default(trial: FrozenTrial) -> Sequence[float]:
     return trial.values
 
 
 def _get_non_pareto_front_trials(
-    trials: List[FrozenTrial], pareto_trials: List[FrozenTrial]
-) -> List[FrozenTrial]:
-
+    trials: list[FrozenTrial], pareto_trials: list[FrozenTrial]
+) -> list[FrozenTrial]:
     non_pareto_trials = []
     for trial in trials:
         if trial not in pareto_trials:
             non_pareto_trials.append(trial)
     return non_pareto_trials
 
 
-def _make_json_compatible(value: Any) -> Any:
-    try:
-        json.dumps(value)
-        return value
-    except TypeError:
-        # The value can't be converted to JSON directly, so return a string representation.
-        return str(value)
-
-
 def _make_scatter_object(
     n_targets: int,
     axis_order: Sequence[int],
     include_dominated_trials: bool,
-    trials_with_values: Sequence[Tuple[FrozenTrial, Sequence[float]]],
+    trials_with_values: Sequence[tuple[FrozenTrial, Sequence[float]]],
     hovertemplate: str,
     infeasible: bool = False,
     dominated_trials: bool = False,
-) -> Union["go.Scatter", "go.Scatter3d"]:
+) -> "go.Scatter" | "go.Scatter3d":
     trials_with_values = trials_with_values or []
 
     marker = _make_marker(
         [trial for trial, _ in trials_with_values],
         include_dominated_trials,
         dominated_trials=dominated_trials,
         infeasible=infeasible,
@@ -413,35 +438,20 @@
             marker=marker,
             showlegend=False,
         )
     else:
         assert False, "Must not reach here"
 
 
-def _make_hovertext(trial: FrozenTrial) -> str:
-    user_attrs = {key: _make_json_compatible(value) for key, value in trial.user_attrs.items()}
-    user_attrs_dict = {"user_attrs": user_attrs} if user_attrs else {}
-    text = json.dumps(
-        {
-            "number": trial.number,
-            "values": trial.values,
-            "params": trial.params,
-            **user_attrs_dict,
-        },
-        indent=2,
-    )
-    return text.replace("\n", "<br>")
-
-
 def _make_marker(
     trials: Sequence[FrozenTrial],
     include_dominated_trials: bool,
     dominated_trials: bool = False,
     infeasible: bool = False,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     if dominated_trials and not include_dominated_trials:
         assert len(trials) == 0
 
     if infeasible:
         return {
             "color": "#cccccc",
         }
```

### Comparing `optuna-3.1.1/optuna/visualization/_plotly_imports.py` & `optuna-3.2.0/optuna/visualization/_plotly_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-3.1.1/optuna/visualization/_slice.py` & `optuna-3.2.0/optuna/visualization/_slice.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from __future__ import annotations
+
 from typing import Any
 from typing import Callable
 from typing import cast
-from typing import List
 from typing import NamedTuple
-from typing import Optional
 
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 from optuna.visualization._plotly_imports import _imports
 from optuna.visualization._utils import _check_plot_args
@@ -23,34 +23,33 @@
     from optuna.visualization._utils import COLOR_SCALE
 
 _logger = get_logger(__name__)
 
 
 class _SliceSubplotInfo(NamedTuple):
     param_name: str
-    x: List[Any]
-    y: List[float]
-    trial_numbers: List[int]
+    x: list[Any]
+    y: list[float]
+    trial_numbers: list[int]
     is_log: bool
     is_numerical: bool
 
 
 class _SlicePlotInfo(NamedTuple):
     target_name: str
-    subplots: List[_SliceSubplotInfo]
+    subplots: list[_SliceSubplotInfo]
 
 
 def _get_slice_subplot_info(
-    trials: List[FrozenTrial],
+    trials: list[FrozenTrial],
     param: str,
-    target: Optional[Callable[[FrozenTrial], float]],
+    target: Callable[[FrozenTrial], float] | None,
     log_scale: bool,
     numerical: bool,
 ) -> _SliceSubplotInfo:
-
     if target is None:
 
         def _target(t: FrozenTrial) -> float:
             return cast(float, t.value)
 
         target = _target
 
@@ -62,19 +61,18 @@
         is_log=log_scale,
         is_numerical=numerical,
     )
 
 
 def _get_slice_plot_info(
     study: Study,
-    params: Optional[List[str]],
-    target: Optional[Callable[[FrozenTrial], float]],
+    params: list[str] | None,
+    target: Callable[[FrozenTrial], float] | None,
     target_name: str,
 ) -> _SlicePlotInfo:
-
     _check_plot_args(study, target, target_name)
 
     trials = _filter_nonfinite(
         study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), target=target
     )
 
     if len(trials) == 0:
@@ -103,17 +101,17 @@
             for param in sorted_params
         ],
     )
 
 
 def plot_slice(
     study: Study,
-    params: Optional[List[str]] = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "go.Figure":
     """Plot the parameter relationship as slice plot in a study.
 
     Note that, if a parameter contains missing values, a trial with missing values is not plotted.
 
     Example:
@@ -157,15 +155,14 @@
     """
 
     _imports.check()
     return _get_slice_plot(_get_slice_plot_info(study, params, target, target_name))
 
 
 def _get_slice_plot(info: _SlicePlotInfo) -> "go.Figure":
-
     layout = go.Layout(title="Slice Plot")
 
     if len(info.subplots) == 0:
         return go.Figure(data=[], layout=layout)
     elif len(info.subplots) == 1:
         figure = go.Figure(data=[_generate_slice_subplot(info.subplots[0])], layout=layout)
         figure.update_xaxes(title_text=info.subplots[0].param_name)
```

### Comparing `optuna-3.1.1/optuna/visualization/_utils.py` & `optuna-3.2.0/optuna/visualization/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from __future__ import annotations
+
+import json
 from typing import Any
 from typing import Callable
 from typing import cast
-from typing import List
-from typing import Optional
 from typing import Sequence
-from typing import Set
-from typing import Union
 import warnings
 
 import numpy as np
 
 import optuna
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
@@ -44,19 +43,18 @@
 if is_available():
     import plotly.colors
 
     COLOR_SCALE = plotly.colors.sequential.Blues
 
 
 def _check_plot_args(
-    study: Union[Study, Sequence[Study]],
-    target: Optional[Callable[[FrozenTrial], float]],
+    study: Study | Sequence[Study],
+    target: Callable[[FrozenTrial], float] | None,
     target_name: str,
 ) -> None:
-
     studies: Sequence[Study]
     if isinstance(study, Study):
         studies = [study]
     else:
         studies = study
 
     if target is None and any(study._is_multi_objective() for study in studies):
@@ -67,56 +65,53 @@
 
     if target is not None and target_name == "Objective Value":
         warnings.warn(
             "`target` is specified, but `target_name` is the default value, 'Objective Value'."
         )
 
 
-def _is_log_scale(trials: List[FrozenTrial], param: str) -> bool:
-
+def _is_log_scale(trials: list[FrozenTrial], param: str) -> bool:
     for trial in trials:
         if param in trial.params:
             dist = trial.distributions[param]
 
             if isinstance(dist, (FloatDistribution, IntDistribution)):
                 if dist.log:
                     return True
 
     return False
 
 
-def _is_categorical(trials: List[FrozenTrial], param: str) -> bool:
-
+def _is_categorical(trials: list[FrozenTrial], param: str) -> bool:
     return any(
         isinstance(t.distributions[param], CategoricalDistribution)
         for t in trials
         if param in t.params
     )
 
 
-def _is_numerical(trials: List[FrozenTrial], param: str) -> bool:
+def _is_numerical(trials: list[FrozenTrial], param: str) -> bool:
     return all(
         (isinstance(t.params[param], int) or isinstance(t.params[param], float))
         and not isinstance(t.params[param], bool)
         for t in trials
         if param in t.params
     )
 
 
-def _get_param_values(trials: List[FrozenTrial], p_name: str) -> List[Any]:
-
+def _get_param_values(trials: list[FrozenTrial], p_name: str) -> list[Any]:
     values = [t.params[p_name] for t in trials if p_name in t.params]
     if _is_numerical(trials, p_name):
         return values
     return list(map(str, values))
 
 
 def _get_skipped_trial_numbers(
-    trials: List[FrozenTrial], used_param_names: Sequence[str]
-) -> Set[int]:
+    trials: list[FrozenTrial], used_param_names: Sequence[str]
+) -> set[int]:
     """Utility function for ``plot_parallel_coordinate``.
 
     If trial's parameters do not contain a parameter in ``used_param_names``,
     ``plot_parallel_coordinate`` methods do not use such trials.
 
     Args:
         trials:
@@ -134,31 +129,30 @@
             if used_param not in trial.params.keys():
                 skipped_trial_numbers.add(trial.number)
                 break
     return skipped_trial_numbers
 
 
 def _filter_nonfinite(
-    trials: List[FrozenTrial],
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    trials: list[FrozenTrial],
+    target: Callable[[FrozenTrial], float] | None = None,
     with_message: bool = True,
-) -> List[FrozenTrial]:
-
+) -> list[FrozenTrial]:
     # For multi-objective optimization target must be specified to select
     # one of objective values to filter trials by (and plot by later on).
     # This function is not raising when target is missing, since we're
     # assuming plot args have been sanitized before.
     if target is None:
 
         def _target(t: FrozenTrial) -> float:
             return cast(float, t.value)
 
         target = _target
 
-    filtered_trials: List[FrozenTrial] = []
+    filtered_trials: list[FrozenTrial] = []
     for trial in trials:
         value = target(trial)
 
         try:
             value = float(value)
         except (
             ValueError,
@@ -178,10 +172,33 @@
                 )
         else:
             filtered_trials.append(trial)
 
     return filtered_trials
 
 
-def _is_reverse_scale(study: Study, target: Optional[Callable[[FrozenTrial], float]]) -> bool:
-
+def _is_reverse_scale(study: Study, target: Callable[[FrozenTrial], float] | None) -> bool:
     return target is not None or study.direction == StudyDirection.MINIMIZE
+
+
+def _make_json_compatible(value: Any) -> Any:
+    try:
+        json.dumps(value)
+        return value
+    except TypeError:
+        # The value can't be converted to JSON directly, so return a string representation.
+        return str(value)
+
+
+def _make_hovertext(trial: FrozenTrial) -> str:
+    user_attrs = {key: _make_json_compatible(value) for key, value in trial.user_attrs.items()}
+    user_attrs_dict = {"user_attrs": user_attrs} if user_attrs else {}
+    text = json.dumps(
+        {
+            "number": trial.number,
+            "values": trial.values,
+            "params": trial.params,
+            **user_attrs_dict,
+        },
+        indent=2,
+    )
+    return text.replace("\n", "<br>")
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_contour.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_contour.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
+from __future__ import annotations
+
 from typing import Callable
-from typing import Dict
-from typing import List
-from typing import Optional
 from typing import Sequence
-from typing import Tuple
-from typing import Union
 
 import numpy as np
 
 from optuna._experimental import experimental_func
 from optuna._imports import try_import
 from optuna.logging import get_logger
 from optuna.study import Study
@@ -34,17 +31,17 @@
 
 CONTOUR_POINT_NUM = 100
 
 
 @experimental_func("2.2.0")
 def plot_contour(
     study: Study,
-    params: Optional[List[str]] = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
     """Plot the parameter relationship as contour plot in a study with Matplotlib.
 
     Note that, if a parameter contains missing values, a trial with missing values is not plotted.
 
     .. seealso::
@@ -104,15 +101,14 @@
         "those of the Plotly-based `plot_contour`."
     )
     info = _get_contour_info(study, params, target, target_name)
     return _get_contour_plot(info)
 
 
 def _get_contour_plot(info: _ContourInfo) -> "Axes":
-
     sorted_params = info.sorted_params
     sub_plot_infos = info.sub_plot_infos
     reverse_scale = info.reverse_scale
     target_name = info.target_name
 
     if len(sorted_params) <= 1:
         _, ax = plt.subplots()
@@ -154,49 +150,48 @@
 def _set_cmap(reverse_scale: bool) -> "Colormap":
     cmap = "Blues_r" if not reverse_scale else "Blues"
     return plt.get_cmap(cmap)
 
 
 class _LabelEncoder:
     def __init__(self) -> None:
-        self.labels: List[str] = []
+        self.labels: list[str] = []
 
-    def fit(self, labels: List[str]) -> "_LabelEncoder":
+    def fit(self, labels: list[str]) -> "_LabelEncoder":
         self.labels = sorted(set(labels))
         return self
 
-    def transform(self, labels: List[str]) -> List[int]:
+    def transform(self, labels: list[str]) -> list[int]:
         return [self.labels.index(label) for label in labels]
 
-    def fit_transform(self, labels: List[str]) -> List[int]:
+    def fit_transform(self, labels: list[str]) -> list[int]:
         return self.fit(labels).transform(labels)
 
-    def get_labels(self) -> List[str]:
+    def get_labels(self) -> list[str]:
         return self.labels
 
-    def get_indices(self) -> List[int]:
+    def get_indices(self) -> list[int]:
         return list(range(len(self.labels)))
 
 
 def _calculate_griddata(
     xaxis: _AxisInfo,
     yaxis: _AxisInfo,
-    z_values_dict: Dict[Tuple[int, int], float],
-) -> Tuple[
+    z_values_dict: dict[tuple[int, int], float],
+) -> tuple[
     np.ndarray,
     np.ndarray,
     np.ndarray,
-    List[int],
-    List[str],
-    List[int],
-    List[str],
-    List[Union[int, float]],
-    List[Union[int, float]],
+    list[int],
+    list[str],
+    list[int],
+    list[str],
+    list[int | float],
+    list[int | float],
 ]:
-
     x_values = []
     y_values = []
     z_values = []
     for x_value, y_value in zip(xaxis.values, yaxis.values):
         if x_value is not None and y_value is not None:
             x_values.append(x_value)
             y_values.append(y_value)
@@ -206,21 +201,20 @@
 
     # Return empty values when x or y has no value.
     if len(x_values) == 0 or len(y_values) == 0:
         return np.array([]), np.array([]), np.array([]), [], [], [], [], [], []
 
     def _calculate_axis_data(
         axis: _AxisInfo,
-        values: Sequence[Union[str, float]],
-    ) -> Tuple[np.ndarray, List[str], List[int], List[Union[int, float]]]:
-
+        values: Sequence[str | float],
+    ) -> tuple[np.ndarray, list[str], list[int], list[int | float]]:
         # Convert categorical values to int.
-        cat_param_labels = []  # type: List[str]
-        cat_param_pos = []  # type: List[int]
-        returned_values: Sequence[Union[int, float]]
+        cat_param_labels: list[str] = []
+        cat_param_pos: list[int] = []
+        returned_values: Sequence[int | float]
         if axis.is_cat:
             enc = _LabelEncoder()
             returned_values = enc.fit_transform(list(map(str, values)))
             cat_param_labels = enc.get_labels()
             cat_param_pos = enc.get_indices()
         else:
             returned_values = list(map(lambda x: float(x), values))
@@ -260,15 +254,14 @@
         cat_param_labels_y,
         transformed_x_values,
         transformed_y_values,
     )
 
 
 def _generate_contour_subplot(info: _SubContourInfo, ax: "Axes", cmap: "Colormap") -> "ContourSet":
-
     if len(info.xaxis.indices) < 2 or len(info.yaxis.indices) < 2:
         ax.label_outer()
         return ax
 
     ax.set(xlabel=info.xaxis.name, ylabel=info.yaxis.name)
     ax.set_xlim(info.xaxis.range[0], info.xaxis.range[1])
     ax.set_ylim(info.yaxis.range[0], info.yaxis.range[1])
@@ -315,21 +308,20 @@
         ax.set_yticks(y_cat_param_pos)
         ax.set_yticklabels(y_cat_param_label)
     ax.label_outer()
     return cs
 
 
 def _create_zmap(
-    x_values: List[Union[int, float]],
-    y_values: List[Union[int, float]],
-    z_values: List[float],
+    x_values: list[int | float],
+    y_values: list[int | float],
+    z_values: list[float],
     xi: np.ndarray,
     yi: np.ndarray,
-) -> Dict[Tuple[int, int], float]:
-
+) -> dict[tuple[int, int], float]:
     # Creates z-map from trial values and params.
     # z-map is represented by hashmap of coordinate and trial value pairs.
     #
     # Coordinates are represented by tuple of integers, where the first item
     # indicates x-axis index and the second item indicates y-axis index
     # and refer to a position of trial value on irregular param grid.
     #
@@ -341,16 +333,15 @@
         xindex = int(np.argmin(np.abs(xi - x)))
         yindex = int(np.argmin(np.abs(yi - y)))
         zmap[(xindex, yindex)] = z
 
     return zmap
 
 
-def _interpolate_zmap(zmap: Dict[Tuple[int, int], float], contour_plot_num: int) -> np.ndarray:
-
+def _interpolate_zmap(zmap: dict[tuple[int, int], float], contour_plot_num: int) -> np.ndarray:
     # Implements interpolation formulation used in Plotly
     # to interpolate heatmaps and contour plots
     # https://github.com/plotly/plotly.js/blob/95b3bd1bb19d8dc226627442f8f66bce9576def8/src/traces/heatmap/interp2d.js#L15-L20
     # citing their doc:
     #
     # > Fill in missing data from a 2D array using an iterative
     # > poisson equation solver with zero-derivative BC at edges.
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_edf.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_edf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from __future__ import annotations
+
 from typing import Callable
-from typing import Optional
 from typing import Sequence
-from typing import Union
 
 from optuna._experimental import experimental_func
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.visualization._edf import _get_edf_info
 from optuna.visualization.matplotlib._matplotlib_imports import _imports
@@ -16,17 +16,17 @@
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 _logger = get_logger(__name__)
 
 
 @experimental_func("2.2.0")
 def plot_edf(
-    study: Union[Study, Sequence[Study]],
+    study: Study | Sequence[Study],
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
     """Plot the objective value EDF (empirical distribution function) of a study with Matplotlib.
 
     Note that only the complete trials are considered when plotting the EDF.
 
     .. seealso::
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_intermediate_values.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_intermediate_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     """
 
     _imports.check()
     return _get_intermediate_plot(_get_intermediate_plot_info(study))
 
 
 def _get_intermediate_plot(info: _IntermediatePlotInfo) -> "Axes":
-
     # Set up the graph style.
     plt.style.use("ggplot")  # Use ggplot style sheet for similar outputs to plotly.
     _, ax = plt.subplots(tight_layout=True)
     ax.set_title("Intermediate Values Plot")
     ax.set_xlabel("Step")
     ax.set_ylabel("Intermediate Value")
     cmap = plt.get_cmap("tab20")  # Use tab20 colormap for multiple line plots.
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_matplotlib_imports.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_matplotlib_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     from matplotlib import __version__ as matplotlib_version
     from matplotlib import pyplot as plt
     from matplotlib.axes._axes import Axes
     from matplotlib.collections import LineCollection
     from matplotlib.collections import PathCollection
     from matplotlib.colors import Colormap
     from matplotlib.contour import ContourSet
-    from matplotlib.patches import Rectangle
 
     # TODO(ytknzw): Set precise version.
     if version.parse(matplotlib_version) < version.parse("3.0.0"):
         raise ImportError(
             "Your version of Matplotlib is " + matplotlib_version + " . "
             "Please install Matplotlib version 3.0.0 or higher. "
             "Matplotlib can be installed by executing `$ pip install -U matplotlib>=3.0.0`. "
@@ -31,9 +30,8 @@
     "matplotlib_version",
     "plt",
     "Axes",
     "LineCollection",
     "PathCollection",
     "Colormap",
     "ContourSet",
-    "Rectangle",
 ]
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_optimization_history.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_optimization_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from __future__ import annotations
+
 from typing import Callable
-from typing import List
-from typing import Optional
 from typing import Sequence
-from typing import Union
 
 import numpy as np
 
 from optuna._experimental import experimental_func
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.visualization._optimization_history import _get_optimization_history_info_list
@@ -17,17 +16,17 @@
 if _imports.is_successful():
     from optuna.visualization.matplotlib._matplotlib_imports import Axes
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
 @experimental_func("2.2.0")
 def plot_optimization_history(
-    study: Union[Study, Sequence[Study]],
+    study: Study | Sequence[Study],
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
     error_bar: bool = False,
 ) -> "Axes":
     """Plot optimization history of all trials in a study with Matplotlib.
 
     .. seealso::
         Please refer to :func:`optuna.visualization.plot_optimization_history` for an example.
@@ -81,18 +80,17 @@
     _imports.check()
 
     info_list = _get_optimization_history_info_list(study, target, target_name, error_bar)
     return _get_optimization_history_plot(info_list, target_name)
 
 
 def _get_optimization_history_plot(
-    info_list: List[_OptimizationHistoryInfo],
+    info_list: list[_OptimizationHistoryInfo],
     target_name: str,
 ) -> "Axes":
-
     # Set up the graph style.
     plt.style.use("ggplot")  # Use ggplot style sheet for similar outputs to plotly.
     _, ax = plt.subplots()
     ax.set_title("Optimization History Plot")
     ax.set_xlabel("Trial")
     ax.set_ylabel(target_name)
     cmap = plt.get_cmap("tab10")  # Use tab10 colormap for similar outputs to plotly.
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_parallel_coordinate.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_parallel_coordinate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from __future__ import annotations
+
 from typing import Callable
-from typing import List
-from typing import Optional
 
 import numpy as np
 
 from optuna._experimental import experimental_func
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.visualization._parallel_coordinate import _get_parallel_coordinate_info
@@ -17,17 +17,17 @@
     from optuna.visualization.matplotlib._matplotlib_imports import LineCollection
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
 @experimental_func("2.2.0")
 def plot_parallel_coordinate(
     study: Study,
-    params: Optional[List[str]] = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
     """Plot the high-dimensional parameter relationships in a study with Matplotlib.
 
     Note that, if a parameter contains missing values, a trial with missing values is not plotted.
 
     .. seealso::
@@ -77,15 +77,14 @@
 
     _imports.check()
     info = _get_parallel_coordinate_info(study, params, target, target_name)
     return _get_parallel_coordinate_plot(info)
 
 
 def _get_parallel_coordinate_plot(info: _ParallelCoordinateInfo) -> "Axes":
-
     reversescale = info.reverse_scale
     target_name = info.target_name
 
     # Set up the graph style.
     fig, ax = plt.subplots()
     cmap = plt.get_cmap("Blues_r" if reversescale else "Blues")
     ax.set_title("Parallel Coordinate Plot")
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_param_importances.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_param_importances.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from __future__ import annotations
+
 from typing import Callable
-from typing import List
-from typing import Optional
 
 import numpy as np
 
 from optuna._experimental import experimental_func
 from optuna.importance._base import BaseImportanceEvaluator
 from optuna.logging import get_logger
 from optuna.study import Study
@@ -24,18 +24,18 @@
 
 AXES_PADDING_RATIO = 1.05
 
 
 @experimental_func("2.2.0")
 def plot_param_importances(
     study: Study,
-    evaluator: Optional[BaseImportanceEvaluator] = None,
-    params: Optional[List[str]] = None,
+    evaluator: BaseImportanceEvaluator | None = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
     """Plot hyperparameter importances with Matplotlib.
 
     .. seealso::
         Please refer to :func:`optuna.visualization.plot_param_importances` for an example.
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_pareto_front.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_pareto_front.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from __future__ import annotations
+
 from typing import Callable
-from typing import List
-from typing import Optional
 from typing import Sequence
 
 from optuna._experimental import experimental_func
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.visualization._pareto_front import _get_pareto_front_info
 from optuna.visualization._pareto_front import _ParetoFrontInfo
@@ -16,19 +16,19 @@
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
 @experimental_func("2.8.0")
 def plot_pareto_front(
     study: Study,
     *,
-    target_names: Optional[List[str]] = None,
+    target_names: list[str] | None = None,
     include_dominated_trials: bool = True,
-    axis_order: Optional[List[int]] = None,
-    constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
-    targets: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
+    axis_order: list[int] | None = None,
+    constraints_func: Callable[[FrozenTrial], Sequence[float]] | None = None,
+    targets: Callable[[FrozenTrial], Sequence[float]] | None = None,
 ) -> "Axes":
     """Plot the Pareto front of a study.
 
     .. seealso::
         Please refer to :func:`optuna.visualization.plot_pareto_front` for an example.
 
     Example:
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_slice.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_slice.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+from __future__ import annotations
+
 import math
 from typing import Any
 from typing import Callable
-from typing import List
-from typing import Optional
-from typing import Tuple
 
 from optuna._experimental import experimental_func
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.visualization._slice import _get_slice_plot_info
 from optuna.visualization._slice import _SlicePlotInfo
 from optuna.visualization._slice import _SliceSubplotInfo
@@ -21,17 +20,17 @@
     from optuna.visualization.matplotlib._matplotlib_imports import PathCollection
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
 @experimental_func("2.2.0")
 def plot_slice(
     study: Study,
-    params: Optional[List[str]] = None,
+    params: list[str] | None = None,
     *,
-    target: Optional[Callable[[FrozenTrial], float]] = None,
+    target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
     """Plot the parameter relationship as slice plot in a study with Matplotlib.
 
     .. seealso::
         Please refer to :func:`optuna.visualization.plot_slice` for an example.
 
@@ -76,15 +75,14 @@
     """
 
     _imports.check()
     return _get_slice_plot(_get_slice_plot_info(study, params, target, target_name))
 
 
 def _get_slice_plot(info: _SlicePlotInfo) -> "Axes":
-
     if len(info.subplots) == 0:
         _, ax = plt.subplots()
         return ax
 
     # Set up the graph style.
     cmap = plt.get_cmap("Blues")
     padding_ratio = 0.05
@@ -144,16 +142,16 @@
     )
     ax.label_outer()
 
     return sc
 
 
 def _calc_lim_with_padding(
-    values: List[Any], padding_ratio: float, scale: Optional[str]
-) -> Tuple[float, float]:
+    values: list[Any], padding_ratio: float, scale: str | None
+) -> tuple[float, float]:
     value_max = max(values)
     value_min = min(values)
     if scale == "log":
         padding = (math.log10(value_max) - math.log10(value_min)) * padding_ratio
         return (
             math.pow(10, math.log10(value_min) - padding),
             math.pow(10, math.log10(value_max) + padding),
```

### Comparing `optuna-3.1.1/optuna/visualization/matplotlib/_utils.py` & `optuna-3.2.0/optuna/visualization/matplotlib/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from __future__ import annotations
 
 from optuna._experimental import experimental_func
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.trial import FrozenTrial
 from optuna.visualization.matplotlib import _matplotlib_imports
@@ -25,36 +25,34 @@
     Returns:
         :obj:`True` if visualization with Matplotlib is available, :obj:`False` otherwise.
     """
 
     return _matplotlib_imports._imports.is_successful()
 
 
-def _is_log_scale(trials: List[FrozenTrial], param: str) -> bool:
-
+def _is_log_scale(trials: list[FrozenTrial], param: str) -> bool:
     for trial in trials:
         if param in trial.params:
             dist = trial.distributions[param]
 
             if isinstance(dist, (FloatDistribution, IntDistribution)):
                 if dist.log:
                     return True
 
     return False
 
 
-def _is_categorical(trials: List[FrozenTrial], param: str) -> bool:
-
+def _is_categorical(trials: list[FrozenTrial], param: str) -> bool:
     return any(
         isinstance(t.distributions[param], CategoricalDistribution)
         for t in trials
         if param in t.params
     )
 
 
-def _is_numerical(trials: List[FrozenTrial], param: str) -> bool:
+def _is_numerical(trials: list[FrozenTrial], param: str) -> bool:
     return all(
         (isinstance(t.params[param], int) or isinstance(t.params[param], float))
         and not isinstance(t.params[param], bool)
         for t in trials
         if param in t.params
     )
```

### Comparing `optuna-3.1.1/optuna.egg-info/SOURCES.txt` & `optuna-3.2.0/optuna.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
-benchmarks/asv/__init__.py
-benchmarks/asv/optimize.py
-benchmarks/kurobako/__init__.py
-benchmarks/kurobako/mo_create_study.py
-benchmarks/naslib/__init__.py
-benchmarks/naslib/problem.py
 optuna/__init__.py
 optuna/_callbacks.py
 optuna/_convert_positional_args.py
 optuna/_deprecated.py
 optuna/_experimental.py
 optuna/_imports.py
 optuna/_transform.py
+optuna/_typing.py
 optuna/cli.py
 optuna/distributions.py
 optuna/exceptions.py
 optuna/logging.py
 optuna/progress_bar.py
 optuna/py.typed
 optuna/version.py
@@ -69,19 +63,14 @@
 optuna/integration/wandb.py
 optuna/integration/xgboost.py
 optuna/integration/_lightgbm_tuner/__init__.py
 optuna/integration/_lightgbm_tuner/alias.py
 optuna/integration/_lightgbm_tuner/optimize.py
 optuna/integration/_lightgbm_tuner/sklearn.py
 optuna/integration/allennlp/__init__.py
-optuna/integration/allennlp/_dump_best_config.py
-optuna/integration/allennlp/_environment.py
-optuna/integration/allennlp/_executor.py
-optuna/integration/allennlp/_pruner.py
-optuna/integration/allennlp/_variables.py
 optuna/multi_objective/__init__.py
 optuna/multi_objective/study.py
 optuna/multi_objective/trial.py
 optuna/multi_objective/samplers/__init__.py
 optuna/multi_objective/samplers/_adapter.py
 optuna/multi_objective/samplers/_base.py
 optuna/multi_objective/samplers/_motpe.py
@@ -99,37 +88,41 @@
 optuna/pruners/_successive_halving.py
 optuna/pruners/_threshold.py
 optuna/samplers/__init__.py
 optuna/samplers/_base.py
 optuna/samplers/_brute_force.py
 optuna/samplers/_cmaes.py
 optuna/samplers/_grid.py
+optuna/samplers/_nsgaiii.py
 optuna/samplers/_partial_fixed.py
 optuna/samplers/_qmc.py
 optuna/samplers/_random.py
 optuna/samplers/_search_space/__init__.py
-optuna/samplers/_search_space/group_decomposed.py
 optuna/samplers/_search_space/intersection.py
 optuna/samplers/_tpe/__init__.py
 optuna/samplers/_tpe/_erf.py
 optuna/samplers/_tpe/_truncnorm.py
 optuna/samplers/_tpe/multi_objective_sampler.py
 optuna/samplers/_tpe/parzen_estimator.py
+optuna/samplers/_tpe/probability_distributions.py
 optuna/samplers/_tpe/sampler.py
 optuna/samplers/nsgaii/__init__.py
 optuna/samplers/nsgaii/_crossover.py
 optuna/samplers/nsgaii/_sampler.py
 optuna/samplers/nsgaii/_crossovers/__init__.py
 optuna/samplers/nsgaii/_crossovers/_base.py
 optuna/samplers/nsgaii/_crossovers/_blxalpha.py
 optuna/samplers/nsgaii/_crossovers/_sbx.py
 optuna/samplers/nsgaii/_crossovers/_spx.py
 optuna/samplers/nsgaii/_crossovers/_undx.py
 optuna/samplers/nsgaii/_crossovers/_uniform.py
 optuna/samplers/nsgaii/_crossovers/_vsbx.py
+optuna/search_space/__init__.py
+optuna/search_space/group_decomposed.py
+optuna/search_space/intersection.py
 optuna/storages/__init__.py
 optuna/storages/_base.py
 optuna/storages/_cached_storage.py
 optuna/storages/_heartbeat.py
 optuna/storages/_in_memory.py
 optuna/storages/_journal/__init__.py
 optuna/storages/_journal/base.py
@@ -147,29 +140,41 @@
 optuna/storages/_rdb/alembic/versions/v1.3.0.a.py
 optuna/storages/_rdb/alembic/versions/v2.4.0.a.py
 optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py
 optuna/storages/_rdb/alembic/versions/v3.0.0.a.py
 optuna/storages/_rdb/alembic/versions/v3.0.0.b.py
 optuna/storages/_rdb/alembic/versions/v3.0.0.c.py
 optuna/storages/_rdb/alembic/versions/v3.0.0.d.py
+optuna/storages/_rdb/alembic/versions/v3.2.0.a_.py
 optuna/study/__init__.py
 optuna/study/_dataframe.py
 optuna/study/_frozen.py
 optuna/study/_multi_objective.py
 optuna/study/_optimize.py
 optuna/study/_study_direction.py
 optuna/study/_study_summary.py
 optuna/study/_tell.py
 optuna/study/study.py
+optuna/terminator/__init__.py
+optuna/terminator/callback.py
+optuna/terminator/erroreval.py
+optuna/terminator/terminator.py
+optuna/terminator/improvement/__init__.py
+optuna/terminator/improvement/_preprocessing.py
+optuna/terminator/improvement/evaluator.py
+optuna/terminator/improvement/gp/__init__.py
+optuna/terminator/improvement/gp/base.py
+optuna/terminator/improvement/gp/botorch.py
 optuna/testing/__init__.py
 optuna/testing/distributions.py
 optuna/testing/objectives.py
 optuna/testing/pruners.py
 optuna/testing/samplers.py
 optuna/testing/storages.py
+optuna/testing/tempfile_pool.py
 optuna/testing/threading.py
 optuna/testing/visualization.py
 optuna/trial/__init__.py
 optuna/trial/_base.py
 optuna/trial/_fixed.py
 optuna/trial/_frozen.py
 optuna/trial/_state.py
@@ -179,20 +184,36 @@
 optuna/visualization/_edf.py
 optuna/visualization/_intermediate_values.py
 optuna/visualization/_optimization_history.py
 optuna/visualization/_parallel_coordinate.py
 optuna/visualization/_param_importances.py
 optuna/visualization/_pareto_front.py
 optuna/visualization/_plotly_imports.py
+optuna/visualization/_rank.py
 optuna/visualization/_slice.py
+optuna/visualization/_terminator_improvement.py
+optuna/visualization/_timeline.py
 optuna/visualization/_utils.py
 optuna/visualization/matplotlib/__init__.py
 optuna/visualization/matplotlib/_contour.py
 optuna/visualization/matplotlib/_edf.py
 optuna/visualization/matplotlib/_intermediate_values.py
 optuna/visualization/matplotlib/_matplotlib_imports.py
 optuna/visualization/matplotlib/_optimization_history.py
 optuna/visualization/matplotlib/_parallel_coordinate.py
 optuna/visualization/matplotlib/_param_importances.py
 optuna/visualization/matplotlib/_pareto_front.py
+optuna/visualization/matplotlib/_rank.py
 optuna/visualization/matplotlib/_slice.py
-optuna/visualization/matplotlib/_utils.py
+optuna/visualization/matplotlib/_terminator_improvement.py
+optuna/visualization/matplotlib/_timeline.py
+optuna/visualization/matplotlib/_utils.py
+tests/test_callbacks.py
+tests/test_cli.py
+tests/test_convert_positional_args.py
+tests/test_deprecated.py
+tests/test_distributions.py
+tests/test_experimental.py
+tests/test_imports.py
+tests/test_logging.py
+tests/test_multi_objective.py
+tests/test_transform.py
```

### Comparing `optuna-3.1.1/optuna.egg-info/requires.txt` & `optuna-3.2.0/optuna.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -13,82 +13,83 @@
 cma
 scikit-optimize
 virtualenv
 
 [checking]
 black
 blackdoc
-hacking
+flake8
 isort
 mypy
 types-PyYAML
 types-redis
 types-setuptools
+types-tqdm
 typing_extensions>=3.10.0.0
 
 [document]
 cma
+botorch
 distributed
 fvcore
 lightgbm
 matplotlib!=3.6.0
 mlflow
 pandas
 pillow
 plotly>=4.9.0
 scikit-learn
 scikit-optimize
-sphinx<6
+sphinx
 sphinx-copybutton
 sphinx-gallery
 sphinx-plotly-directive
 sphinx_rtd_theme
-torch==1.11.0
-torchaudio==0.11.0
-torchvision==0.12.0
+torch
+torchaudio
+torchvision
 
 [integration]
-chainer>=5.0.0
 cma
 distributed
-mpi4py
+mlflow
 pandas
 scikit-learn>=0.24.2
 wandb
 xgboost
 
 [integration:python_version < "3.11"]
-allennlp>=2.2.0
-cached-path<=1.1.2
-botorch<0.8.0,>=0.4.0
-catalyst>=21.3
-catboost>=0.26
+botorch>=0.4.0
 fastai
 lightgbm
-mlflow
 mxnet
 pytorch-ignite
-pytorch-lightning>=1.5.0
+pytorch-lightning>=1.6.0
 scikit-optimize
 shap
-skorch
 tensorflow
-tensorflow-datasets
-torch==1.11.0
-torchaudio==0.11.0
-torchvision==0.12.0
+torch
+torchaudio
+torchvision
+
+[integration:sys_platform != "darwin"]
+catboost>=0.26
+
+[integration:sys_platform == "darwin"]
+catboost<1.2,>=0.26
 
 [optional]
+botorch
 matplotlib!=3.6.0
 pandas
 plotly>=4.9.0
 redis
 scikit-learn>=0.24.2
 
 [test]
-codecov
+coverage
 fakeredis[lua]
 kaleido
 pytest
 
 [test:python_version >= "3.8"]
 scipy>=1.9.2
```

### Comparing `optuna-3.1.1/setup.cfg` & `optuna-3.2.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [flake8]
 ignore = 
 	E203,
-	W503,
-	H306
+	W503
 max-line-length = 99
 statistics = True
-exclude = venv,build,tutorial,.asv
+exclude = .venv,venv,build,tutorial,.asv
 
 [mypy]
 warn_unused_configs = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 check_untyped_defs = True
 no_implicit_optional = True
 warn_redundant_casts = True
 strict_equality = True
 strict_concatenate = True
 no_implicit_reexport = True
 ignore_missing_imports = True
-exclude = venv|build|docs|tutorial|optuna/storages/_rdb/alembic
+exclude = .venv|venv|build|docs|tutorial|optuna/storages/_rdb/alembic
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

