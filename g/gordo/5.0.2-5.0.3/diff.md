# Comparing `tmp/gordo-5.0.2.tar.gz` & `tmp/gordo-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gordo-5.0.2.tar", last modified: Tue May 23 14:15:31 2023, max compression
+gzip compressed data, was "gordo-5.0.3.tar", last modified: Tue May 30 18:06:18 2023, max compression
```

## Comparing `gordo-5.0.2.tar` & `gordo-5.0.3.tar`

### file list

```diff
@@ -1,281 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 14:13:17.000000 gordo-5.0.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 14:13:17.000000 gordo-5.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/dependabot.yml 
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/workflows/master-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-23 14:13:17.000000 gordo-5.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 14:13:17.000000 gordo-5.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/.trivyignore
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-23 14:13:17.000000 gordo-5.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-23 14:13:17.000000 gordo-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-23 14:13:17.000000 gordo-5.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-23 14:15:31.007681 gordo-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-23 14:13:17.000000 gordo-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/benchmarks/load_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/load_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/load_test/load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/load_test/task_set.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/test_ml_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 14:13:17.000000 gordo-5.0.2/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/Gordo_C4.README
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/Gordo_C4.svg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/_placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/endpoint-metadata.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/machine/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/model-factories.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/transformer-funcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/serializer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/server/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/server/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/server/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/server/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/general/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/general/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/general/endpoints.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/general/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-05-23 14:13:17.000000 gordo-5.0.2/examples/Gordo-Workflow-High-Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-23 14:13:17.000000 gordo-5.0.2/examples/Pipelines-with-Gordo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-23 14:13:17.000000 gordo-5.0.2/examples/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 14:13:17.000000 gordo-5.0.2/functions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/exceptions_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/anomaly/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/anomaly/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/transformer_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformer_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformer_funcs/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformers/imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/server/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/blueprints/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/blueprints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/model_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/server/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/config_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/config_elements/normalized_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/config_elements/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/workflow_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/workflow_generator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/gordo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 14:13:17.000000 gordo-5.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-23 14:13:17.000000 gordo-5.0.2/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/docs_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/full_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/mlflow_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/postgres_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/test_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.979681 gordo-5.0.2/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.979681 gordo-5.0.2/resources/grafana/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/resources/grafana/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-05-23 14:13:17.000000 gordo-5.0.2/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 14:13:17.000000 gordo-5.0.2/resources/grafana/dashboards/how_to_modify_dashboard.md
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-23 14:13:17.000000 gordo-5.0.2/resources/grafana/dashboards/machines.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-23 14:13:17.000000 gordo-5.0.2/run_workflow_and_argo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/download_argo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/github_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/trivy_scan.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:15:31.007681 gordo-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-23 14:13:17.000000 gordo-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/config-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/test_local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/cli/test_exception_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/client/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/metadata/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_factories_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_raw_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/reporters/test_mlflow_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/reporters/test_postgres_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/definition_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/test_serializer_from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/test_serializer_into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/test_serializer_load_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_anomaly_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_base_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_gordo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_model_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/test_disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/test_sensor_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_config_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_normalized_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/mocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 18:04:09.000000 gordo-5.0.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 18:04:09.000000 gordo-5.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/dependabot.yml 
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/workflows/master-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-30 18:04:09.000000 gordo-5.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 18:04:09.000000 gordo-5.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/.trivyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-30 18:04:09.000000 gordo-5.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-30 18:04:09.000000 gordo-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-30 18:04:09.000000 gordo-5.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-30 18:06:18.781191 gordo-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-30 18:04:09.000000 gordo-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/benchmarks/load_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/load_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/load_test/load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/load_test/task_set.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/test_ml_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-30 18:04:09.000000 gordo-5.0.3/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/Gordo_C4.README
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/Gordo_C4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/_placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   113230 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/architecture_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/architecture_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/argo_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/endpoint-metadata.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/api/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/loader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/api/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/model-factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/register.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/transformer-funcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/reporters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/serializer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/api/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/cluster_deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/endpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/ml/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/ml/model_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/ml/model_output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/Gordo-Workflow-High-Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/Pipelines-with-Gordo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/model-configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/test-project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-30 18:04:09.000000 gordo-5.0.3/functions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26331 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/exceptions_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/anomaly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/anomaly/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/transformer_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformer_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformer_funcs/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformers/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/server/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/blueprints/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/blueprints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/model_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/server/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/config_elements/normalized_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/config_elements/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/workflow_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/workflow_generator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/gordo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 18:04:09.000000 gordo-5.0.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 18:04:09.000000 gordo-5.0.3/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/docs_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/full_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/mlflow_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/postgres_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/test_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.757191 gordo-5.0.3/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.757191 gordo-5.0.3/resources/grafana/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/resources/grafana/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-05-30 18:04:09.000000 gordo-5.0.3/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-30 18:04:09.000000 gordo-5.0.3/resources/grafana/dashboards/how_to_modify_dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-30 18:04:09.000000 gordo-5.0.3/resources/grafana/dashboards/machines.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-30 18:04:09.000000 gordo-5.0.3/run_workflow_and_argo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/download_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/github_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/trivy_scan.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:06:18.781191 gordo-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-30 18:04:09.000000 gordo-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/config-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/tests/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/test_local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/cli/test_exception_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/client/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/metadata/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_factories_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_raw_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/reporters/test_mlflow_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/reporters/test_postgres_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/definition_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/test_serializer_from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/test_serializer_into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/test_serializer_load_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_anomaly_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_base_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_gordo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/test_disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/test_sensor_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/tests/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_normalized_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/mocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/utils.py
```

### Comparing `gordo-5.0.2/.github/workflows/main.yml` & `gordo-5.0.3/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -37,7 +37,25 @@
       - name: Install
         run: |
           pip install -r requirements/full_requirements.txt
           pip install -r requirements/test_requirements.txt
 
       - name: Test ${{ matrix.component }}
         run: bash scripts/tests.sh -n -p ${{ matrix.component }}
+
+  build-docs:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v1
+
+      - uses: actions/setup-python@v1
+        with:
+          python-version: '3.10'
+          architecture: 'x64'
+
+      - name: Install deps
+        run: |
+          pip install --upgrade pip
+          pip install .[docs]
+
+      - name: Build Docs
+        run: make docs
```

### Comparing `gordo-5.0.2/.github/workflows/master-ci.yml` & `gordo-5.0.3/.github/workflows/master-ci.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/.github/workflows/release.yml` & `gordo-5.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/.gitignore` & `gordo-5.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/Dockerfile` & `gordo-5.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/LICENSE` & `gordo-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/Makefile` & `gordo-5.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/PKG-INFO` & `gordo-5.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.2
+Version: 5.0.3
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: mlflow
 Provides-Extra: postgres
 Provides-Extra: tests
 Provides-Extra: full
+Provides-Extra: docs
 License-File: LICENSE
 
 
 
 <h1 align="center">Gordo</h1>
 <div align="center">
  <!-- Uncomment line below once we decided on 'logo.png' -->
@@ -50,14 +50,16 @@
 
 ## Components
 
 * [gordo-controller](https://github.com/equinor/gordo-controller/) - Kubernetes controller for the Gordo CRDs.
 * [gordo-core](https://github.com/equinor/gordo-core/) - Gordo core library.
 * [gordo-client](https://github.com/equinor/gordo-client/) - Gordo server's client. It can make predictions from deployed models.
 
+[Documentation is available on Read the Docs](https://gordo1.readthedocs.io/)
+
 ---
 ## Install
 
 [gordo-helm](https://github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to deploy gordo infrastructure to your Kubernetes cluster. 
 
 ### Python package 
 
@@ -125,7 +127,16 @@
 > **_NOTE:_**  To run tests it's required for your system to has (note: commands might differ from your OS):
 > - Running docker daemon.
 > - Available 5432 port for `postgres` container.
 
 > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the code of the tests.  
 > On the configuration setup for test running add to `Additional arguments:` in `pytest` 
 > section following string: `--ignore benchmarks --cov-report= --no-cov ` 
+
+### Build the documentation
+
+This command will run the local documentation server:
+
+```console
+> cd docs/
+> make watch
+```
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.2 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.0.3 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-Extra:
-tests Provides-Extra: full License-File: LICENSE
+Extra: mlflow Provides-Extra: postgres Provides-Extra: tests Provides-Extra:
+full Provides-Extra: docs License-File: LICENSE
                               ****** Gordo ******
 
      Building thousands of models with timeseries data to monitor systems.
 
                                 [Build_Status]
 --- ## About Gordo fulfills the role of inhaling config files and supplying
 components to the pipeline of: 1. Fetching data 2. Training model 3. Serving
 model ## Components * [gordo-controller](https://github.com/equinor/gordo-
 controller/) - Kubernetes controller for the Gordo CRDs. * [gordo-core](https:/
 /github.com/equinor/gordo-core/) - Gordo core library. * [gordo-client](https:/
 /github.com/equinor/gordo-client/) - Gordo server's client. It can make
-predictions from deployed models. --- ## Install [gordo-helm](https://
+predictions from deployed models. [Documentation is available on Read the Docs]
+(https://gordo1.readthedocs.io/) --- ## Install [gordo-helm](https://
 github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/
 equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to
 deploy gordo infrastructure to your Kubernetes cluster. ### Python package `pip
 install --upgrade gordo` With additional extras: `pip install gordo
 [postgres,mlflow]` Bleeding edge: `pip install git+https://github.com/equinor/
 gordo.git` ## Developer manual This section will explain how to start
 development of Gordo. ### Setup Create and activate a virtual environment
@@ -42,8 +43,10 @@
 some time, so it's faster to run tests in parallel: ``` pytest -n auto -m 'not
 dockertest' --ignore benchmarks ``` Run docker-related tests: ``` pytest -
 m 'dockertest' ``` > **_NOTE:_** To run tests it's required for your system to
 has (note: commands might differ from your OS): > - Running docker daemon. > -
 Available 5432 port for `postgres` container. > **_NOTE:_** this example is for
 Pycharm IDE to use `breakpoints` in the code of the tests. > On the
 configuration setup for test running add to `Additional arguments:` in `pytest`
-> section following string: `--ignore benchmarks --cov-report= --no-cov `
+> section following string: `--ignore benchmarks --cov-report= --no-cov ` ###
+Build the documentation This command will run the local documentation server:
+```console > cd docs/ > make watch ```
```

### Comparing `gordo-5.0.2/README.md` & `gordo-5.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 ## Components
 
 * [gordo-controller](https://github.com/equinor/gordo-controller/) - Kubernetes controller for the Gordo CRDs.
 * [gordo-core](https://github.com/equinor/gordo-core/) - Gordo core library.
 * [gordo-client](https://github.com/equinor/gordo-client/) - Gordo server's client. It can make predictions from deployed models.
 
+[Documentation is available on Read the Docs](https://gordo1.readthedocs.io/)
+
 ---
 ## Install
 
 [gordo-helm](https://github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to deploy gordo infrastructure to your Kubernetes cluster. 
 
 ### Python package 
 
@@ -104,7 +106,16 @@
 > **_NOTE:_**  To run tests it's required for your system to has (note: commands might differ from your OS):
 > - Running docker daemon.
 > - Available 5432 port for `postgres` container.
 
 > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the code of the tests.  
 > On the configuration setup for test running add to `Additional arguments:` in `pytest` 
 > section following string: `--ignore benchmarks --cov-report= --no-cov ` 
+
+### Build the documentation
+
+This command will run the local documentation server:
+
+```console
+> cd docs/
+> make watch
+```
```

#### html2text {}

```diff
@@ -5,15 +5,16 @@
                                 [Build_Status]
 --- ## About Gordo fulfills the role of inhaling config files and supplying
 components to the pipeline of: 1. Fetching data 2. Training model 3. Serving
 model ## Components * [gordo-controller](https://github.com/equinor/gordo-
 controller/) - Kubernetes controller for the Gordo CRDs. * [gordo-core](https:/
 /github.com/equinor/gordo-core/) - Gordo core library. * [gordo-client](https:/
 /github.com/equinor/gordo-client/) - Gordo server's client. It can make
-predictions from deployed models. --- ## Install [gordo-helm](https://
+predictions from deployed models. [Documentation is available on Read the Docs]
+(https://gordo1.readthedocs.io/) --- ## Install [gordo-helm](https://
 github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/
 equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to
 deploy gordo infrastructure to your Kubernetes cluster. ### Python package `pip
 install --upgrade gordo` With additional extras: `pip install gordo
 [postgres,mlflow]` Bleeding edge: `pip install git+https://github.com/equinor/
 gordo.git` ## Developer manual This section will explain how to start
 development of Gordo. ### Setup Create and activate a virtual environment
@@ -33,8 +34,10 @@
 some time, so it's faster to run tests in parallel: ``` pytest -n auto -m 'not
 dockertest' --ignore benchmarks ``` Run docker-related tests: ``` pytest -
 m 'dockertest' ``` > **_NOTE:_** To run tests it's required for your system to
 has (note: commands might differ from your OS): > - Running docker daemon. > -
 Available 5432 port for `postgres` container. > **_NOTE:_** this example is for
 Pycharm IDE to use `breakpoints` in the code of the tests. > On the
 configuration setup for test running add to `Additional arguments:` in `pytest`
-> section following string: `--ignore benchmarks --cov-report= --no-cov `
+> section following string: `--ignore benchmarks --cov-report= --no-cov ` ###
+Build the documentation This command will run the local documentation server:
+```console > cd docs/ > make watch ```
```

### Comparing `gordo-5.0.2/benchmarks/load_test/README.md` & `gordo-5.0.3/benchmarks/load_test/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/benchmarks/load_test/load_test.py` & `gordo-5.0.3/benchmarks/load_test/load_test.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/benchmarks/test_ml_server.py` & `gordo-5.0.3/benchmarks/test_ml_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/docs/_static/Gordo_C4.svg` & `gordo-5.0.3/docs/_static/Gordo_C4.svg`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/docs/_static/endpoint-metadata.png` & `gordo-5.0.3/docs/_static/endpoint-metadata.png`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/docs/components/machine/metadata.rst` & `gordo-5.0.3/docs/api/machine/metadata.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/docs/components/serializer.rst` & `gordo-5.0.3/docs/api/serializer.rst`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,37 @@
 .. automodule:: gordo.serializer.serializer
     :members:
     :undoc-members:
     :show-inheritance:
 
 
 From Definition
-===============
+^^^^^^^^^^^^^^^
 
 The ability to take a 'raw' representation of an object in ``dict`` form
 and load it into a Python object.
 
 .. automodule:: gordo.serializer.from_definition
     :members:
     :undoc-members:
     :show-inheritance:
 
 
 Into Definitiion
-================
+^^^^^^^^^^^^^^^^
 
 The ability to take a Python object, such as a scikit-learn
 pipeline and convert it into a primitive ``dict``, which can then be inserted
 into a YAML config file.
 
 .. automodule:: gordo.serializer.into_definition
     :members:
     :undoc-members:
     :show-inheritance:
+
+Utils
+^^^^^
+
+.. automodule:: gordo.serializer.utils
+    :members:
+    :undoc-members:
+    :show-inheritance:
```

### Comparing `gordo-5.0.2/docs/components/workflow.rst` & `gordo-5.0.3/docs/api/workflow.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,30 +3,39 @@
 
 The workflow component is responsible for converting a Gordo config into
 an Argo workflow which then runs the various components in order to build
 and serve the ML models.
 
 
 Normalized Config
-=================
+^^^^^^^^^^^^^^^^^
+
 .. automodule:: gordo.workflow.config_elements.normalized_config
     :members:
     :undoc-members:
     :show-inheritance:
 
 Workflow Generator
-==================
+^^^^^^^^^^^^^^^^^^
 
 Workflow loading/processing functionality to help the CLI 'workflow' sub-command.
 
 .. automodule:: gordo.workflow.workflow_generator.workflow_generator
     :members:
     :undoc-members:
     :show-inheritance:
 
+Schemas
+^^^^^^^
+
+.. automodule:: gordo.workflow.config_elements.schemas
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
 Helpers
-=======
+^^^^^^^
+
 .. automodule:: gordo.workflow.workflow_generator.helpers
     :members:
     :undoc-members:
     :show-inheritance:
-
```

### Comparing `gordo-5.0.2/docs/general/endpoints.rst` & `gordo-5.0.3/docs/general/endpoints.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,29 @@
 Endpoints
 ---------
 
-==================
-Project index page
-==================
-
 Going to the base path of the project, ie. ``/gordo/v0/my-project/`` will return the
 project level index, with returns a collection of the metadata surrounding the models currently deployed and their status.
 Each ``endpoint`` key has an associated ``endpoint-metadata`` key which is the direct transferal of metadata returned from
-the ML servers at their :ref:`ml-server-metadata-route` route.
-
-This returns *a lot* of metadata data, so we'll show a small screen-shot of some of the data you might expect to get:
-
-.. image:: ../_static/endpoint-metadata.png
-
-----
-
-==============================
-Machine Learning Server Routes
-==============================
+the ML servers at their :ref:`get-metadata` route.
 
 When a model is deployed from a config file, it results in a ML
 server capable of the following paths:
 
-Under normal Equinor deployments, paths listed below should be prefixed with ``/gordo/v0/<project-name>/<model-name>``.
+Under normal deployments, paths listed below should be prefixed with ``/gordo/v0/<project-name>/<model-name>``.
 Otherwise, the paths listed below are the raw exposed endpoints from the server's perspective.
 
-----
+A detailed example of this API usage could be found :ref:`here <general/cluster_deployment:working with api>`.
 
-/
-=
+.. _post-prediction:
 
-This is the Swagger UI for the given model. Allows for manual testing of endpoints via a GUI interface.
+POST /prediction
+^^^^^^^^^^^^^^^^
 
-----
-
-.. _prediction-endpoint:
-
-/prediction/
-============
+:func:`gordo.server.blueprints.base.post_prediction`
 
 The ``/prediction`` endpoint will return the basic values a model
 is capable of returning. Namely, this will be:
 
 - ``model-output``:
     - The raw model output, after calling ``.predict`` on the model or pipeline
       or ``.transform`` if the pipeline/model does not have a ``.predict`` method.
@@ -70,28 +51,29 @@
                                             '1': 20.382972717285156}},
           'start': {'start': {'0': None, '1': None}}}}
 
 
 
 The endpoint only accepts POST requests.
 
-``POST`` requests take raw data:
+Requests takes raw data:
 
 .. code-block:: python
 
     >>> import requests
     >>>
     >>> # Single sample:
     >>> requests.post("https://my-server.io/prediction", json={"X": [1, 2, 3, 4]})  # doctest: +SKIP
     >>>
     >>> # Multiple samples:
     >>> requests.post("https://my-server.io/prediction", json={"X": [[1, 2, 3, 4], [5, 6, 7, 8]]})  # doctest: +SKIP
 
-**NOTE:** The client must provide the correct number of input features, ie. if the model was trained on 4 features,
-the client should provide 4 feature sample(s).
+.. note::
+    The client must provide the correct number of input features, ie. if the model was trained on 4 features,
+    the client should provide 4 feature sample(s).
 
 You may also supply a dataframe using :func:`gordo.server.utils.dataframe_to_dict`:
 
 .. code-block:: python
 
     >>> import requests
     >>> import pprint
@@ -156,23 +138,25 @@
     >>> resp.ok
     True
     >>> df = utils.dataframe_from_parquet_bytes(resp.content)
 
 
 ----
 
-/anomaly/prediction/
-====================
+POST /anomaly/prediction
+^^^^^^^^^^^^^^^^^^^^^^^^
 
-The ``/anomaly/prediction`` endpoint will return the data supplied by the ``/prediction`` endpoint
-but reserved for models which inherit from :class:`gordo.model.anomaly.base.AnomalyDetectorBase`
+:func:`gordo.server.blueprints.anomaly.post_anomaly_prediction`
 
-By this restriction, additional _features_ are calculated and returned (depending on the `AnomalyDetector` model being served.
+The ``/anomaly/prediction`` endpoint will return the data supplied by the :ref:`post-prediction` endpoint
+but reserved for models which inherit from :class:`gordo.machine.model.anomaly.base.AnomalyDetectorBase`
 
-For example, the :class:`gordo.model.anomaly.diff.DiffBasedAnomalyDetector` will return the following:
+By this restriction, additional features are calculated and returned.
+
+For example, the :class:`gordo.machine.model.anomaly.diff.DiffBasedAnomalyDetector` will return the following:
 
 - ``tag-anomaly-scaled`` & ``tag-anomaly-unscaled``:
     - Anomaly per feature/tag calculated from the expected tag input (y) and the model's output for those tags (yhat),
       using scaled and unscaled values.
 - ``total-anomaly-scaled`` & ``total-anomaly-unscaled``:
     - This is the total anomaly for the given point as calculated by the model, using scaled and unscaled values.
 
@@ -231,27 +215,54 @@
           'total-anomaly-scaled': {'total-anomaly-scaled': {'2019-01-01 00:00:00': 66.71898273252445,
                                                             '2019-01-01 08:00:00': 64.37069672792737,
                                                             '2019-01-01 16:00:00': 62.024759698996235,
                                                             '2019-01-02 00:00:00': 59.68141393388054}}},
     'time-seconds': '0.1623'}
 
 
-
-This endpoint accepts only ``POST`` requests.
-Model requests are exactly the same as :ref:`prediction-endpoint`, but will require a ``y`` to compare the anomaly
+Model requests are exactly the same as :ref:`post-prediction`, but will require a ``y`` to compare the anomaly
 against.
 
-----
+.. _get-metadata:
 
-/download-model/
-================
+GET /metadata
+^^^^^^^^^^^^^
 
-Returns the current model being served. Loadable via ``gordo.serializer.loads(downloaded_bytes)``
+:func:`gordo.server.blueprints.base.get_metadata`
 
-----
+Various metadata surrounding the current model and environment.
 
-.. _ml-server-metadata-route:
+GET /expected-models
+^^^^^^^^^^^^^^^^^^^^
 
-/metadata/
-==========
+:func:`gordo.server.blueprints.base.get`
 
-Various metadata surrounding the current model and environment.
+Returns list of models for this project. Those models are expected to be built.
+
+GET /models
+^^^^^^^^^^^
+
+:func:`gordo.server.blueprints.base.get_model_list`
+
+List of the current built models.
+
+GET /revisions
+^^^^^^^^^^^^^^
+
+:func:`gordo.server.blueprints.base.get_revision_list`
+
+List of available model revisions (versions).
+
+
+GET /download-model
+^^^^^^^^^^^^^^^^^^^
+
+:func:`gordo.server.blueprints.base.get_download_model`
+
+Returns the current model being served. Loadable via :func:`gordo.serializer.loads`.
+
+DELETE /revision
+^^^^^^^^^^^^^^^^
+
+:func:`gordo.server.blueprints.base.delete_model_revision`
+
+Delete one particular revision from the storage.
```

### Comparing `gordo-5.0.2/examples/Gordo-Workflow-High-Level.ipynb` & `gordo-5.0.3/examples/Gordo-Workflow-High-Level.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/examples/Pipelines-with-Gordo.ipynb` & `gordo-5.0.3/examples/Pipelines-with-Gordo.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/examples/config.yaml` & `gordo-5.0.3/examples/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Workflow generator configuration file compatible with `gordo`'s Kubernetes
 # custom resource defintion.  You may also refer to the `config.yaml` file in
 # the `gordo-test-project` repository
 apiVersion: equinor.com/v1
 kind: Gordo
 metadata:
-  name: test-project
+  name: example
 spec:
   deploy-version: 0.32.0
   config:
     machines:
 
       - name: ct-23-0001 #1st machine
         dataset: |
```

### Comparing `gordo-5.0.2/functions.sh` & `gordo-5.0.3/functions.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/__init__.py` & `gordo-5.0.3/gordo/__init__.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/builder/build_model.py` & `gordo-5.0.3/gordo/builder/build_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         default_data_provider: Optional[str] = None,
     ):
         """
         Build a model for a given :class:`gordo.machine.Machine`
 
         Parameters
         ----------
-        machine: Machine
+        machine
 
         Example
         -------
         >>> from gordo_core.sensor_tag import SensorTag
         >>> from gordo.machine import Machine
         >>> machine = Machine.from_config(dict(
         ...     name="special-model-name",
@@ -114,27 +114,26 @@
         ``model_register_dir`` points to the model cache directory which it will
         attempt to read the model from. Supplying both will then have the effect
         of both; reading from the cache and saving that cached model to the new
         output directory.
 
         Parameters
         ----------
-        output_dir: Optional[Union[os.PathLike, str]]
+        output_dir
             A path to where the model will be deposited.
-        model_register_dir: Optional[Union[os.PathLike, str]]
+        model_register_dir
             A path to a register, see `:func:gordo.util.disk_registry`.
             If this is None then always build the model, otherwise try to resolve
             the model from the registry.
-        replace_cache: bool
+        replace_cache
             Forces a rebuild of the model, and replaces the entry in the cache
             with the new model.
 
         Returns
         -------
-        Tuple[sklearn.base.BaseEstimator, Machine]
             Built model and an updated ``Machine``
         """
         if not model_register_dir:
             model, machine = self._build()
         else:
             cache_key = self.cache_key
             logger.debug(
@@ -348,22 +347,21 @@
     @staticmethod
     def build_split_dict(X: pd.DataFrame, split_obj: Type[BaseCrossValidator]) -> dict:
         """
         Get dictionary of cross-validation training dataset split metadata
 
         Parameters
         ----------
-        X: pd.DataFrame
+        X
             The training dataset that will be split during cross-validation.
-        split_obj: Type[sklearn.model_selection.BaseCrossValidator]
+        split_obj
             The cross-validation object that returns train, test indices for splitting.
 
         Returns
         -------
-        split_metadata: Dict[str,Any]
             Dictionary of cross-validation train/test split metadata
         """
         split_metadata: Dict[str, Any] = dict()
         for i, (train_ind, test_ind) in enumerate(split_obj.split(X)):
             split_metadata.update(
                 {
                     f"fold-{i+1}-train-start": X.index[train_ind[0]],
@@ -388,19 +386,19 @@
         and '{score}' for the average score across all target tags and folds,
         and values being the callable make_scorer(metric_wrapper(score)). Note: score in
         {score}-{tag_name} is a sklearn's score function name with '_' replaced by '-'
         and tag_name corresponds to given target tag name with ' ' replaced by '-'.
 
         Parameters
         ----------
-        metrics_list: list
+        metrics_list
             List of sklearn score functions
-        y: pd.DataFrame
+        y
             Target data
-        scaler : Optional[Union[TransformerMixin, str]]
+        scaler
             Scaler which will be fitted on y, and used to transform the data before
             scoring. Useful when the metrics are sensitive to the amplitude of the data, and
             you have multiple targets.
 
 
         Returns
         -------
@@ -453,23 +451,22 @@
     ) -> int:
         """
         Determine the model's offset. How much does the output of the model differ
         from its input?
 
         Parameters
         ----------
-        model: sklearn.base.BaseEstimator
+        model
             Trained model with either ``predict`` or ``transform`` method, preference
             given to ``predict``.
-        X: Union[np.ndarray, pd.DataFrame]
+        X
             Data to pass to the model's ``predict`` or ``transform`` method.
 
         Returns
         -------
-        int
             The difference between X and the model's output lengths.
         """
         if isinstance(X, pd.DataFrame) or isinstance(X, xr.DataArray):
             X = X.values
         out = model.predict(X) if hasattr(model, "predict") else model.transform(X)
         return len(X) - len(out)
 
@@ -487,25 +484,24 @@
         output_dir: Union[os.PathLike, str],
         checksum: Optional[str] = None,
     ):
         """
         Save the model according to the expected Argo workflow procedure.
         Parameters
         ----------
-        model: BaseEstimator
+        model
             The model to save to the directory with gordo serializer.
-        machine: Union[Machine, dict]
+        machine
             Machine instance used to build this model.
-        output_dir: Union[os.PathLike, str]
+        output_dir
             The directory where to save the model, will create directories if needed.
-        checksum: Optional[str]
+        checksum
             Model revision sha512 checksum. Might be taken from `self.check key`
         Returns
         -------
-        Union[os.PathLike, str]
             Path to the saved model
         """
         os.makedirs(output_dir, exist_ok=True)  # Ok if some dirs exist
         info: Optional[dict] = None
         if checksum is not None:
             info = {"checksum": checksum}
         serializer.dump(
@@ -524,28 +520,27 @@
         Recursively check for :class:`gordo.machine.model.base.GordoBase` in a
         given ``model``. If such the model exists buried inside of a
         :class:`sklearn.pipeline.Pipeline` which is then part of another
         :class:`sklearn.base.BaseEstimator`, this function will return its metadata.
 
         Parameters
         ----------
-        model: BaseEstimator
-        metadata: dict
+        model
+        metadata
             Any initial starting metadata, but is mainly meant to be used during
             the recursive calls to accumulate any multiple
             :class:`gordo.machine.model.base.GordoBase` models found in this model
 
         Notes
         -----
         If there is a ``GordoBase`` model inside of a ``Pipeline`` which is not the final
         step, this function will not find it.
 
         Returns
         -------
-        dict
             Dictionary representing accumulated calls to
             :meth:`gordo.machine.model.base.GordoBase.get_metadata`
         """
         metadata = metadata.copy()
 
         # If it's a Pipeline, only need to get the last step, which potentially has metadata
         if isinstance(model, Pipeline):
@@ -575,15 +570,14 @@
 
     def calculate_cache_key(self, machine: Machine) -> str:
         """
         Calculates a hash-key from the model and data-config.
 
         Returns
         -------
-        str:
             A 512 byte hex value as a string based on the content of the parameters.
 
         Examples
         -------
         >>> from gordo.machine import Machine
         >>> from gordo_core.sensor_tag import SensorTag
         >>> machine = Machine.from_config(dict(
@@ -635,22 +629,21 @@
     @staticmethod
     def check_cache(model_register_dir: Union[os.PathLike, str], cache_key: str):
         """
         Checks if the model is cached, and returns its path if it exists.
 
         Parameters
         ----------
-        model_register_dir: [os.PathLike, None]
+        model_register_dir
             The register dir where the model lies.
-        cache_key: str
+        cache_key
             A 512 byte hex value as a string based on the content of the parameters.
 
-         Returns
+        Returns
         -------
-        Union[os.PathLike, None]:
             The path to the cached model, or None if it does not exist.
         """
         existing_model_location = disk_registry.get_value(model_register_dir, cache_key)
 
         # Check that the model is actually there
         if existing_model_location and Path(existing_model_location).exists():
             logger.debug(
@@ -675,25 +668,24 @@
         """
         Given a list of metric function paths. ie. sklearn.metrics.r2_score or
         simple function names which are expected to be in the ``sklearn.metrics`` module,
         this will return a list of those loaded functions.
 
         Parameters
         ----------
-        metrics: Optional[List[str]]
+        metrics
             List of function paths to use as metrics for the model Defaults to
             those specified in :class:`gordo.workflow.config_components.NormalizedConfig`
             sklearn.metrics.explained_variance_score,
             sklearn.metrics.r2_score,
             sklearn.metrics.mean_squared_error,
             sklearn.metrics.mean_absolute_error
 
         Returns
         -------
-        List[Callable]
             A list of the functions loaded
 
         Raises
         ------
         AttributeError:
            If the function cannot be loaded.
         """
```

### Comparing `gordo-5.0.2/gordo/builder/local_build.py` & `gordo-5.0.3/gordo/builder/local_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     This is very similar to the same steps as the normal workflow generation and subsequent
     Gordo deployment process makes. Should help developing locally,
     as well as giving a good indication that your config is valid for deployment
     with Gordo.
 
     Parameters
     ----------
-    config_str: str
+    config_str
         The raw yaml config file in string format.
 
     Examples
     --------
     >>> import numpy as np
     >>> config = '''
     ... machines:
@@ -57,15 +57,14 @@
     ...         name: crazy-sweet-name
     ... '''
     >>> models_n_metadata = local_build(config)
     >>> assert len(list(models_n_metadata)) == 1
 
     Returns
     -------
-    Iterable[Tuple[Union[BaseEstimator, None], Machine]]
         A generator yielding tuples of models and their metadata.
     """
 
     config = get_dict_from_yaml(io.StringIO(config_str))
     normed = NormalizedConfig(config, project_name="local-build")
     for machine in normed.machines:
         yield ModelBuilder(machine=machine).build()
```

### Comparing `gordo-5.0.2/gordo/builder/utils.py` & `gordo-5.0.3/gordo/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/cli/cli.py` & `gordo-5.0.3/gordo/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,36 +122,14 @@
     model_parameter: List[Tuple[str, Any]],
     exceptions_reporter_file: str,
     exceptions_report_level: str,
 ):
     """
     Build a model and deposit it into 'output_dir' given the appropriate config
     settings.
-
-    \b
-    Parameters
-    ----------
-    machine_config: dict
-        A dict loadable by :class:`gordo.machine.Machine.from_config`
-    output_dir: str
-        Directory to save model & metadata to.
-    model_register_dir: path
-        Path to a directory which will index existing models and their locations, used
-        for re-using old models instead of rebuilding them. If omitted then always
-        rebuild
-    model_builder_class: str
-    print_cv_scores: bool
-        Print cross validation scores to stdout
-    model_parameter: List[Tuple[str, Any]
-        List of model key-values, wheres the values will be injected into the model
-        config wherever there is a jinja variable with the key.
-    exceptions_reporter_file: str
-        JSON output file for exception information
-    exceptions_report_level: str
-        Details level for exception reporting
     """
 
     try:
         if model_parameter and isinstance(machine_config["model"], str):
             parameters = dict(model_parameter)  # convert lib of tuples to dict
             machine_config["model"] = expand_model(machine_config["model"], parameters)
 
@@ -214,27 +192,25 @@
 def expand_model(model_config: str, model_parameters: dict):
     """
     Expands the jinja template which is the model using the variables in
     `model_parameters`
 
     Parameters
     ----------
-    model_config: str
+    model_config
         Jinja template which when expanded becomes a valid model config json.
-    model_parameters:
-        Parameters for the model config.
+    model_parameters        Parameters for the model config.
 
     Raises
     ------
     ValueError
         If an undefined variable is used in the model_config.
 
     Returns
     -------
-    str
         The model config with variables expanded
 
     """
     try:
         model_template = jinja2.Environment(
             loader=jinja2.BaseLoader(), undefined=jinja2.StrictUndefined
         ).from_string(model_config)
@@ -244,33 +220,34 @@
     logger.info(f"Expanded model config: {model_config}")
     return yaml.safe_load(model_config)
 
 
 def get_all_score_strings(machine):
     """Given metadata from the model builder this function returns a list of
     strings of the following format:
-    {metric_name}-{tag_name}_{fold-fold-number} = {score_val}.  This computes the score for the given tag and
+    ``{metric_name}-{tag_name}_{fold-fold-number} = {score_val}``.  This computes the score for the given tag and
     cross validation split.
-    {metric_name}-{tag_name}_{fold-aggregation} = {score_val}. This computes the score for the given tag and aggregates
+    ``{metric_name}-{tag_name}_{fold-aggregation} = {score_val}``. This computes the score for the given tag and aggregates
     the score over all cross validation splits (aggregations currently used are mean, std, min and max)
-    {metric_name}_{fold-fold-number} = {score_val}.  This computes the score aggregate across all tags (uses sklearn's default
+    ``{metric_name}_{fold-fold-number} = {score_val}``.  This computes the score aggregate across all tags (uses sklearn's default
     aggregation method) for a given cross validation split.
-    {metric_name}_{fold-aggregation} = {score_val}.  This computes the score aggregate across all tags (uses sklearn's default
+    ``{metric_name}_{fold-aggregation} = {score_val}``.  This computes the score aggregate across all tags (uses sklearn's default
     aggregation method) and cross validation splits (aggregations currently used are mean, std, min and max).
 
     for katib to pick up.
 
     Current metric names supported are sklearn score functions: 'r2_score', 'explained_variance_score',
     'mean_squared_error' and 'mean_absolute_error'.  The underscores in such score names are replaced by '-'.
 
     All spaces in the tag name are also replaced by '-'.
 
     Parameters
     ----------
-    machine : Machine
+    machine
+        Machine to score
     """
     all_scores = []
     for (
         metric_name,
         scores,
     ) in machine.metadata.build_metadata.model.cross_validation.scores.items():
         metric_name = metric_name.replace(" ", "-")
```

### Comparing `gordo-5.0.2/gordo/cli/custom_types.py` & `gordo-5.0.3/gordo/cli/custom_types.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/cli/exceptions_reporter.py` & `gordo-5.0.3/gordo/cli/exceptions_reporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     ):
         """
         Parameters
         ----------
         exceptions
             Exceptions list with preferred exit codes for each of them
         default_exit_code
-            Default exit code. It might be used as `sys.exit()` code
+            Default exit code. It might be used as :func:`sys.exit` code
         traceback_limit
-            Limit for `traceback.format_exception()`
+            Limit for :func:`traceback.format_exception`
         """
         self.exceptions_items = self.sort_exceptions(exceptions)
         self.default_exit_code = default_exit_code
         self.traceback_limit = traceback_limit
 
     @staticmethod
     def sort_exceptions(
@@ -104,24 +104,21 @@
         for item in self.exceptions_items:
             if issubclass(exc_type, item[0]):
                 return item
         return None
 
     def exception_exit_code(self, exc_type: Optional[Type[BaseException]]) -> int:
         """
-        Possible `sys.exit()` code for given exception type
+        Possible :func:`sys.exit` code for given exception type
 
         Parameters
         ----------
         exc_type
             The exception type
 
-        Returns
-        -------
-        int
         """
         if exc_type is None:
             return 0
         item = self.found_exception_item(exc_type)
         return item[1] if item is not None else self.default_exit_code
 
     def report(
@@ -131,19 +128,19 @@
         exc_value: Optional[BaseException],
         exc_traceback: Optional[TracebackType],
         report_file: IO[str],
         max_message_len: Optional[int] = None,
     ):
         """
         Report exception to the file.
-        `exc_type`, `exc_value`, `exc_traceback` might be values returned by `sys.exc_info()`
+        ``exc_type``, ``exc_value``, ``exc_traceback`` might be values returned by :func:`sys.exc_info`
 
         Parameters
         ----------
-        level: ReportLevel
+        level
             Level of the report verbosity
         exc_type
             The exception type
         exc_value
             The exception
         exc_traceback
             The exception traceback
@@ -190,15 +187,15 @@
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         exc_traceback: Optional[TracebackType],
         report_file_path: str,
         max_message_len: Optional[int] = None,
     ):
         """
-        Basically this is a wrapper for `ExceptionsReporter.report()` function
+        Basically this is a wrapper for :func:`~ExceptionsReporter.report` function
         with additional internal exceptions handling
 
         Parameters
         ----------
         level
         exc_type
         exc_value
```

### Comparing `gordo-5.0.2/gordo/cli/workflow_generator.py` & `gordo-5.0.3/gordo/cli/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/machine/encoders.py` & `gordo-5.0.3/gordo/machine/encoders.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/machine/loader.py` & `gordo-5.0.3/gordo/machine/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 
 def load_globals_config(config: dict, json_path: str = None) -> GlobalsConfig:
     """
     Load `GlobalsConfig` from the dict
 
     Parameters
     ----------
-    config: str
+    config
         Config to load.
-    json_path: str
+    json_path
         JSON path position of the config.
 
     Returns
     -------
 
     """
     return cast(GlobalsConfig, _load_config(config, json_path))
@@ -72,17 +72,17 @@
 
 def load_machine_config(config: dict, json_path: str = None) -> MachineConfig:
     """
     Load `MachineConfig` from the dict
 
     Parameters
     ----------
-    config: str
+    config
         Config to load.
-    json_path: str
+    json_path
         JSON path position of the config.
 
     Returns
     -------
 
     """
     machine_config = _load_config(config, json_path)
@@ -95,17 +95,17 @@
 
 def load_model_config(config: dict, json_path: str = None) -> ModelConfig:
     """
     Load `ModelConfig` from the dict
 
     Parameters
     ----------
-    config: str
+    config
         Config to load.
-    json_path: str
+    json_path
         JSON path position of the config.
 
     Returns
     -------
 
     """
     model_config = cast(ModelConfig, load_machine_config(config, json_path))
```

### Comparing `gordo-5.0.2/gordo/machine/machine.py` & `gordo-5.0.3/gordo/machine/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,27 +85,25 @@
     ):
         """
         Construct an instance from a block of YAML config file which represents
         a single Machine; loaded as a ``dict``.
 
         Parameters
         ----------
-        config: dict[str, Any]
+        config
             The loaded block of config which represents a 'Machine' in YAML
-        project_name: str
+        project_name
             Name of the project this Machine belongs to.
-        config_globals:
-            The block of config within the YAML file within `globals`
-        back_compatibles: Optional[BackCompatibleLocations]
+        config_globals            The block of config within the YAML file within `globals`
+        back_compatibles
             See `gordo_core.import_utils.prepare_back_compatible_locations()` function for reference.
-        default_data_provider: Optional[str]
+        default_data_provider
 
         Returns
         -------
-        :class:`~Machine`
         """
         if config_globals is None:
             config_globals = dict()
 
         name = config["name"]
         config_model = config.get("model") or config_globals.get("model")
         if config_model is None:
@@ -152,19 +150,18 @@
 
     def normalize_sensor_tags(self, tag_list: TagsList) -> List[SensorTag]:
         """
         Finding assets for all of the tags according to information from the dataset metadata
 
         Parameters
         ----------
-        tag_list: TagsList
+        tag_list
 
         Returns
         -------
-        List[SensorTag]
 
         """
         metadata = self.metadata
         build_dataset_metadata = metadata.build_metadata.dataset.to_dict()
         asset: Optional[str] = None
         if hasattr(self.dataset, "asset"):
             asset = self.dataset.asset
```

### Comparing `gordo-5.0.2/gordo/machine/metadata/metadata.py` & `gordo-5.0.3/gordo/machine/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/machine/model/anomaly/base.py` & `gordo-5.0.3/gordo/machine/model/anomaly/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     def anomaly(
         self,
         X: Union[pd.DataFrame, xr.DataArray],
         y: Union[pd.DataFrame, xr.DataArray],
         frequency: Optional[timedelta] = None,
     ) -> Union[pd.DataFrame, xr.Dataset]:
         """
-        Take X, y and optionally frequency; returning a dataframe containing
+        Take ``X``, ``y`` and optionally frequency; returning a dataframe containing
         anomaly score(s)
         """
         ...
```

### Comparing `gordo-5.0.2/gordo/machine/model/anomaly/diff.py` & `gordo-5.0.3/gordo/machine/model/anomaly/diff.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,35 +37,35 @@
         with the original, unscaled, ``y``.
 
         Threshold calculation is based on a rolling statistic of the validation errors
         on the last fold of cross-validation.
 
         Parameters
         ----------
-        base_estimator: sklearn.base.BaseEstimator
+        base_estimator
             The model to which normal ``.fit``, ``.predict`` methods will be used.
             defaults to py:class:`gordo.machine.model.models.KerasAutoEncoder` with
             ``kind='feedforward_hourglass``
-        scaler: sklearn.base.TransformerMixin
+        scaler
             Defaults to ``sklearn.preprocessing.RobustScaler``
             Used for transforming model output and the original ``y`` to calculate
             the difference/error in model output vs expected.
-        require_thresholds: bool
+        require_thresholds
             Requires calculating ``thresholds_`` via a call to
             :func:`~DiffBasedAnomalyDetector.cross_validate`. If this is set
             (default True), but :func:`~DiffBasedAnomalyDetector.cross_validate` was not
             called before calling :func:`~DiffBasedAnomalyDetector.anomaly`
             an ``AttributeError`` will be raised.
-        shuffle: bool
+        shuffle
             Flag to shuffle or not data in ``.fit`` so that the model, if relevant,
             will be trained on a sample of data accross the time range and not just
             the last elements according to model arg ``validation_split``.
-        window: int
+        window
             Window size for smoothed thresholds
-        smoothing_method: str
+        smoothing_method
             Method to be used together with ``window`` to smooth metrics.
             Must be one of: 'smm': simple moving median, 'sma': simple moving average or
             'ewma': exponential weighted moving average.
         """
         self.base_estimator = base_estimator
         self.scaler = scaler
         self.require_thresholds = require_thresholds
@@ -84,18 +84,14 @@
             return getattr(self, item)
         else:
             return getattr(self.base_estimator, item)
 
     def get_metadata(self):
         """
         Generates model metadata.
-
-        Returns
-        -------
-        dict
         """
         metadata = dict()
         if hasattr(self, "feature_thresholds_"):
             metadata["feature-thresholds"] = self.feature_thresholds_.tolist()
         if hasattr(self, "aggregate_threshold_"):
             metadata["aggregate-threshold"] = self.aggregate_threshold_
         if hasattr(self, "feature_thresholds_per_fold_"):
@@ -152,18 +148,14 @@
         sample_weight: Optional[np.ndarray] = None,
     ) -> float:
         return self.base_estimator.score(X, y)
 
     def get_params(self, deep=True):
         """
         Get parameters for this estimator.
-
-        Returns
-        -------
-        dict
         """
         params = {
             "base_estimator": self.base_estimator,
             "scaler": self.scaler,
             "shuffle": self.shuffle,
         }
         if self.window is not None:
@@ -191,25 +183,21 @@
     ):
         """
         Run TimeSeries cross validation on the model, and will update the model's
         threshold values based on the cross validation folds.
 
         Parameters
         ----------
-        X: Union[pd.DataFrame, np.ndarray]
+        X
             Input data to the model
-        y: Union[pd.DataFrame, np.ndarray]
+        y
             Target data
-        kwargs: dict
+        kwargs
             Any additional kwargs to be passed to
             :func:`sklearn.model_selection.cross_validate`
-
-        Returns
-        -------
-        dict
         """
         # Depend on having the trained fold models
         kwargs.update(dict(return_estimator=True, cv=cv))
 
         cv_output = c_val(self, X=X, y=y, **kwargs)
 
         self.feature_thresholds_per_fold_ = pd.DataFrame()
@@ -283,21 +271,21 @@
         y_true: Union[pd.DataFrame, np.ndarray],
         y_pred: Union[pd.DataFrame, np.ndarray],
     ) -> pd.Series:
         """
         Calculate the scaled MSE per timestep/sample
         Parameters
         ----------
-        model: BaseEstimator
+        model
             Instance of a fitted :class:`~DiffBasedAnomalyDetector`
-        y_true: Union[numpy.ndarray, pd.DataFrame]
-        y_pred: Union[numpy.ndarray, pd.DataFrame]
+        y_true
+        y_pred
+
         Returns
         -------
-        panadas.Series
             The MSE calculated from the scaled y and y predicted.
         """
         try:
             scaled_y_true = model.scaler.transform(y_true)
         except (NotFittedError, ValueError):
             scaled_y_true = model.scaler.fit_transform(y_true)
         scaled_y_pred = model.scaler.transform(y_pred)
@@ -326,22 +314,21 @@
         frequency: Optional[timedelta] = None,
     ) -> Union[pd.DataFrame, xr.Dataset]:
         """
         Create an anomaly dataframe from the base provided dataframe.
 
         Parameters
         ----------
-        X: pd.DataFrame
+        X
             Dataframe representing the data to go into the model.
-        y: pd.DataFrame
+        y
             Dataframe representing the target output of the model.
 
         Returns
         -------
-        pd.DataFrame
             A superset of the original base dataframe with added anomaly specific
             features
         """
 
         if not hasattr(X, "values"):
             raise ValueError("Unable to find X.values property")
 
@@ -491,40 +478,40 @@
         with the original, unscaled, ``y``.
 
         Threshold calculation is based on a percentile of the smoothed validation
         errors as calculated from cross-validation predictions.
 
         Parameters
         ----------
-        base_estimator: sklearn.base.BaseEstimator
+        base_estimator
             The model to which normal ``.fit``, ``.predict`` methods will be used.
             defaults to py:class:`gordo.machine.model.models.KerasAutoEncoder` with
             ``kind='feedforward_hourglass``
-        scaler: sklearn.base.TransformerMixin
+        scaler
             Defaults to ``sklearn.preprocessing.RobustScaler``
             Used for transforming model output and the original ``y`` to calculate
             the difference/error in model output vs expected.
-        require_thresholds: bool
+        require_thresholds
             Requires calculating ``thresholds_`` via a call to
             :func:`~DiffBasedAnomalyDetector.cross_validate`.
             If this is set (default True), but
             :func:`~DiffBasedAnomalyDetector.cross_validate` was not called before
             calling :func:`~DiffBasedAnomalyDetector.anomaly` an ``AttributeError``
             will be raised.
-        shuffle: bool
+        shuffle
             Flag to shuffle or not data in ``.fit`` so that the model, if relevant,
             will be trained on a sample of data accross the time range and not just
             the last elements according to model arg ``validation_split``.
-        window: int
+        window
             Window size for smooth metrics and threshold calculation.
-        smoothing_method: str
+        smoothing_method
             Method to be used together with ``window`` to smooth metrics.
             Must be one of: 'smm': simple moving median, 'sma': simple moving average or
             'ewma': exponential weighted moving average.
-        threshold_percentile: float
+        threshold_percentile
             Percentile of the validation data to be used to calculate the threshold.
         """
         self.base_estimator = base_estimator
         self.scaler = scaler
         self.require_thresholds = require_thresholds
         self.window = window
         self.shuffle = shuffle
@@ -533,15 +520,14 @@
 
     def get_params(self, deep=True):
         """
         Get parameters for this estimator.
 
         Returns
         -------
-        dict
         """
         params = {
             "base_estimator": self.base_estimator,
             "scaler": self.scaler,
             "window": self.window,
             "smoothing_method": self.smoothing_method,
             "shuffle": self.shuffle,
@@ -551,15 +537,14 @@
 
     def get_metadata(self):
         """
         Generates model metadata.
 
         Returns
         -------
-        dict
         """
         metadata = dict()
 
         if hasattr(self, "feature_thresholds_"):
             metadata["feature-thresholds"] = self.feature_thresholds_.tolist()
         if hasattr(self, "aggregate_threshold_"):
             metadata["aggregate-threshold"] = self.aggregate_threshold_
@@ -588,25 +573,21 @@
     ):
         """
         Run Kfold cross validation on the model, and will update the model's threshold
         values based on a percentile of the validation metrics.
 
         Parameters
         ----------
-        X: Union[pd.DataFrame, np.ndarray]
+        X
             Input data to the model
-        y: Union[pd.DataFrame, np.ndarray]
+        y
             Target data
-        kwargs: dict
+        kwargs
             Any additional kwargs to be passed to
             :func:`sklearn.model_selection.cross_validate`
-
-        Returns
-        -------
-        dict
         """
 
         # Depend on having the trained fold models
         kwargs.update(dict(return_estimator=True, cv=cv))
 
         cv_output = c_val(self, X=X, y=y, **kwargs)
```

### Comparing `gordo-5.0.2/gordo/machine/model/base.py` & `gordo-5.0.3/gordo/machine/model/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/machine/model/factories/feedforward_autoencoder.py` & `gordo-5.0.3/gordo/machine/model/factories/feedforward_autoencoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,43 +27,42 @@
     **kwargs,
 ) -> keras.models.Sequential:
     """
     Builds a customized keras neural network auto-encoder based on a config dict
 
     Parameters
     ----------
-    n_features: int
+    n_features
         Number of features the dataset X will contain.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
-    encoding_dim: tuple
+    encoding_dim
         Tuple of numbers with the number of neurons in the encoding part.
-    decoding_dim: tuple
+    decoding_dim
         Tuple of numbers with the number of neurons in the decoding part.
-    encoding_func: tuple
+    encoding_func
         Activation functions for the encoder part.
-    decoding_func: tuple
+    decoding_func
         Activation functions for the decoder part.
-    out_func: str
+    out_func
         Activation function for the output layer
-    optimizer: Union[str, Optimizer]
+    optimizer
         If str then the name of the optimizer must be provided (e.x. "Adam").
         The arguments of the optimizer can be supplied in optimize_kwargs.
         If a Keras optimizer call the instance of the respective
         class (e.x. Adam(lr=0.01,beta_1=0.9, beta_2=0.999)).  If no arguments are
         provided Keras default values will be set.
-    optimizer_kwargs: Dict[str, Any]
+    optimizer_kwargs
         The arguments for the chosen optimizer. If not provided Keras'
         default values will be used.
-    compile_kwargs: Dict[str, Any]
+    compile_kwargs
         Parameters to pass to ``keras.Model.compile``.
 
     Returns
     -------
-    keras.models.Sequential
 
     """
 
     input_dim = n_features
     n_features_out = n_features_out or n_features
 
     check_dim_func_len("encoding", encoding_dim, encoding_func)
@@ -116,39 +115,34 @@
     **kwargs,
 ) -> keras.models.Sequential:
     """
     Builds a symmetrical feedforward model
 
     Parameters
     ----------
-    n_features: int
+    n_features
          Number of input and output neurons.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
-    dim: List[int]
+    dim
          Number of neurons per layers for the encoder, reversed for the decoder.
          Must have len > 0.
-    funcs: List[str]
+    funcs
         Activation functions for the internal layers
-    optimizer: Union[str, Optimizer]
+    optimizer
         If str then the name of the optimizer must be provided (e.x. "Adam").
         The arguments of the optimizer can be supplied in optimization_kwargs.
         If a Keras optimizer call the instance of the respective
-        class (e.x. Adam(lr=0.01,beta_1=0.9, beta_2=0.999)).  If no arguments are
+        class (e.x. ``Adam(lr=0.01,beta_1=0.9, beta_2=0.999)``).  If no arguments are
         provided Keras default values will be set.
-    optimizer_kwargs: Dict[str, Any]
+    optimizer_kwargs
         The arguments for the chosen optimizer. If not provided Keras'
         default values will be used.
-    compile_kwargs: Dict[str, Any]
+    compile_kwargs
         Parameters to pass to ``keras.Model.compile``.
-
-    Returns
-    -------
-    keras.models.Sequential
-
     """
     if len(dims) == 0:
         raise ValueError("Parameter dims must have len > 0")
     return feedforward_model(
         n_features,
         n_features_out,
         encoding_dim=dims,
@@ -177,38 +171,38 @@
     """
     Builds an hourglass shaped neural network, with decreasing number of neurons
     as one gets deeper into the encoder network and increasing number
     of neurons as one gets out of the decoder network.
 
     Parameters
     ----------
-    n_features: int
+    n_features
         Number of input and output neurons.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
-    encoding_layers: int
+    encoding_layers
         Number of layers from the input layer (exclusive) to the
         narrowest layer (inclusive). Must be > 0. The total nr of layers
         including input and output layer will be 2*encoding_layers + 1.
-    compression_factor: float
+    compression_factor
         How small the smallest layer is as a ratio of n_features
         (smallest layer is rounded up to nearest integer). Must satisfy
         0 <= compression_factor <= 1.
-    func: str
+    func
         Activation function for the internal layers
-    optimizer: Union[str, Optimizer]
+    optimizer
         If str then the name of the optimizer must be provided (e.x. "Adam").
         The arguments of the optimizer can be supplied in optimization_kwargs.
         If a Keras optimizer call the instance of the respective
         class (e.x. Adam(lr=0.01,beta_1=0.9, beta_2=0.999)).  If no arguments are
         provided Keras default values will be set.
-    optimizer_kwargs: Dict[str, Any]
+    optimizer_kwargs
         The arguments for the chosen optimizer. If not provided Keras'
         default values will be used.
-    compile_kwargs: Dict[str, Any]
+    compile_kwargs
         Parameters to pass to ``keras.Model.compile``.
 
     Notes
     -----
     The resulting model will look like this when n_features = 10, encoding_layers= 3,
     and compression_factor = 0.3::
 
@@ -220,15 +214,14 @@
                      * * * * *
                   * * * * * * * *
                 * * * * * * * * * *
 
 
     Returns
     -------
-    keras.models.Sequential
 
     Examples
     --------
     >>> model = feedforward_hourglass(10)
     >>> len(model.layers)
     7
     >>> [model.layers[i].units for i in range(len(model.layers))]
```

### Comparing `gordo-5.0.2/gordo/machine/model/factories/lstm_autoencoder.py` & `gordo-5.0.3/gordo/machine/model/factories/lstm_autoencoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,48 +29,47 @@
     **kwargs,
 ) -> tensorflow.keras.models.Sequential:
     """
     Builds a customized Keras LSTM neural network auto-encoder based on a config dict.
 
     Parameters
     ----------
-    n_features: int
+    n_features
         Number of features the dataset X will contain.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
-    lookback_window: int
+    lookback_window
         Number of timesteps used to train the model.
         One timestep = current observation in the sample.
         Two timesteps = current observation + previous observation in the sample.
         ...
-    encoding_dim: tuple
+    encoding_dim
         Tuple of numbers with the number of neurons in the encoding part.
-    decoding_dim: tuple
+    decoding_dim
         Tuple of numbers with the number of neurons in the decoding part.
-    encoding_func: tuple
+    encoding_func
         Activation functions for the encoder part.
-    decoding_func: tuple
+    decoding_func
         Activation functions for the decoder part.
-    out_func: str
+    out_func
         Activation function for the output Dense layer.
-    optimizer: Union[str, Optimizer]
+    optimizer
         If str then the name of the optimizer must be provided (e.x. "Adam").
         The arguments of the optimizer can be supplied in optimize_kwargs.
         If a Keras optimizer call the instance of the respective
         class (e.x. Adam(lr=0.01,beta_1=0.9, beta_2=0.999)).  If no arguments are
         provided Keras default values will be set.
-    optimizer_kwargs: Dict[str, Any]
+    optimizer_kwargs
         The arguments for the chosen optimizer. If not provided Keras'
         default values will be used.
-    compile_kwargs: Dict[str, Any]
+    compile_kwargs
         Parameters to pass to ``keras.Model.compile``.
 
     Returns
     -------
-    keras.models.Sequential
         Returns Keras sequential model.
 
     """
     n_features_out = n_features_out or n_features
 
     check_dim_func_len("encoding", encoding_dim, encoding_func)
     check_dim_func_len("decoding", decoding_dim, decoding_func)
@@ -118,45 +117,44 @@
     **kwargs,
 ) -> tensorflow.keras.models.Sequential:
     """
     Builds a symmetrical lstm model
 
     Parameters
     ----------
-    n_features: int
+    n_features
          Number of input and output neurons.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
-    lookback_window: int
+    lookback_window
         Number of timesteps used to train the model.
         One timestep = sample contains current observation.
         Two timesteps = sample contains current and previous observation.
         ...
-    dims: Tuple[int,...]
+    dims
          Number of neurons per layers for the encoder, reversed for the decoder.
          Must have len > 0
-    funcs: List[str]
+    funcs
         Activation functions for the internal layers.
-    out_func: str
+    out_func
         Activation function for the output Dense layer.
-    optimizer: Union[str, Optimizer]
+    optimizer
         If str then the name of the optimizer must be provided (e.x. "Adam").
         The arguments of the optimizer can be supplied in optimization_kwargs.
         If a Keras optimizer call the instance of the respective
         class (e.x. Adam(lr=0.01,beta_1=0.9, beta_2=0.999)).  If no arguments are
         provided Keras default values will be set.
-    optimizer_kwargs: Dict[str, Any]
+    optimizer_kwargs
         The arguments for the chosen optimizer. If not provided Keras'
         default values will be used.
-    compile_kwargs: Dict[str, Any]
+    compile_kwargs
         Parameters to pass to ``keras.Model.compile``.
 
     Returns
     -------
-    keras.models.Sequential
         Returns Keras sequential model.
     """
 
     if len(dims) == 0:
         raise ValueError("Parameter dims must have len > 0")
 
     return lstm_model(
@@ -196,46 +194,45 @@
     Builds an hourglass shaped neural network, with decreasing number of neurons
     as one gets deeper into the encoder network and increasing number
     of neurons as one gets out of the decoder network.
 
 
     Parameters
     ----------
-    n_features: int
+    n_features
         Number of input and output neurons.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
-    encoding_layers: int
+    encoding_layers
         Number of layers from the input layer (exclusive) to the
         narrowest layer (inclusive). Must be > 0. The total nr of layers
         including input and output layer will be 2*encoding_layers + 1.
      compression_factor: float
         How small the smallest layer is as a ratio of n_features
         (smallest layer is rounded up to nearest integer). Must satisfy
         0 <= compression_factor <= 1.
-    func: str
+    func
         Activation function for the internal layers.
-    out_func: str
+    out_func
         Activation function for the output Dense layer.
-    optimizer: Union[str, Optimizer]
+    optimizer
         If str then the name of the optimizer must be provided (e.x. "Adam").
         The arguments of the optimizer can be supplied in optimization_kwargs.
         If a Keras optimizer call the instance of the respective
         class (e.x. Adam(lr=0.01,beta_1=0.9, beta_2=0.999)).  If no arguments are
         provided Keras default values will be set.
-    optimizer_kwargs: Dict[str, Any]
+    optimizer_kwargs
         The arguments for the chosen optimizer. If not provided Keras'
         default values will be used.
-    compile_kwargs: Dict[str, Any]
+    compile_kwargs
         Parameters to pass to ``keras.Model.compile``.
 
 
     Returns
     -------
-    keras.models.Sequential
 
     Examples
     --------
     >>> model = lstm_hourglass(10)
     >>> len(model.layers)
     7
     >>> [model.layers[i].units for i in range(len(model.layers))]
```

### Comparing `gordo-5.0.2/gordo/machine/model/factories/utils.py` & `gordo-5.0.3/gordo/machine/model/factories/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,27 @@
     compression_factor: float, encoding_layers: int, n_features: int
 ) -> Tuple[int, ...]:
     """
     Calculate the layer dimensions given the number of layers, compression, and features
 
     Parameters
     ----------
-    compression_factor: float
+    compression_factor
         How small the smallest layer is as a ratio of n_features
         (smallest layer is rounded up to nearest integer). Must satisfy
         0 <= compression_factor <= 1.
-    encoding_layers: int
+    encoding_layers
         Number of layers from the input layer (exclusive) to the
         narrowest layer (inclusive). Must be > 0. The total nr of layers
         including input and output layer will be 2*encoding_layers + 1.
-    n_features_out: Optional[int]
+    n_features_out
         Number of features the model will output, default to ``n_features``.
 
     Returns
     -------
-    dims: Tuple[int,...]
          Number of neurons per layers for the encoder, reversed for the decoder.
          Must have len > 0
     """
     if not (1 >= compression_factor >= 0):
         raise ValueError("compression_factor must be 0 <= compression_factor <= 1")
     if encoding_layers < 1:
         raise ValueError("encoding_layers must be >= 1")
@@ -44,19 +43,19 @@
 
 def check_dim_func_len(prefix: str, dim: Tuple[int, ...], func: Tuple[str, ...]):
     """
     Check that the number of layer dimensions and layer functions are equal
 
     Parameters
     ----------
-    prefix: str
+    prefix
         Parameter name prefix for error message generation (Options: "encoding" or "decoding").
-    dim: tuple of int
+    dim
         Tuple of numbers with the number of neurons in the encoding or decoding part.
-    func: Tuple[str,...]
+    func
         Tuple of numbers with the number of neurons in the decoding part.
     """
     if len(dim) != len(func):
         raise ValueError(
             f"The length (i.e. the number of network layers) of {prefix}_dim "
             f"({len(dim)}) and {prefix}_func ({len(func)}) must be equal. If only "
             f"{prefix}_dim or {prefix}_func was passed, ensure that its length matches "
```

### Comparing `gordo-5.0.2/gordo/machine/model/models.py` & `gordo-5.0.3/gordo/machine/model/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,23 +57,22 @@
         kind: Union[
             str, Callable[[int, Dict[str, Any]], tensorflow.keras.models.Model]
         ],
         **kwargs,
     ) -> None:
         """
         Initialized a Scikit-Learn API compatitble Keras model with a pre-registered
-        function or a builder function
-        directly.
+        function or a builder function directly.
 
         Parameters
         ----------
-        kind: Union[callable, str]
+        kind
             The structure of the model to build. As designated by any registered builder
             functions, registered with
-            `gordo_compontents.model.register.register_model_builder`.
+            :func:`gordo.machine.model.register.register_model_builder`.
             Alternatively, one may pass a builder function directly to this argument.
             Such a function should accept `n_features` as it's first argument, and pass
             any additional parameters to `**kwargs`
 
         kwargs: dict
             Any additional args which are passed to the factory
             building function and/or any additional args to be passed
@@ -122,50 +121,44 @@
     @classmethod
     def extract_supported_fit_args(cls, kwargs):
         """
         Filtering only ``fit`` related kwargs
 
         Parameters
         ----------
-        kwargs: dict
-
-        Returns
-        -------
+        kwargs
 
         """
         fit_args = {}
         for arg in cls.supported_fit_args:
             if arg in kwargs:
                 fit_args[arg] = kwargs[arg]
         return fit_args
 
     @classmethod
     def from_definition(cls, definition: dict):
         """
-        Handler for ``gordo.serializer.from_definition``
+        Handler for :func:`gordo.serializer.from_definition`
 
         Parameters
         ----------
-        definition: dict
-
-        Returns
-        -------
+        definition
+            Model definition
 
         """
         kind = definition.pop("kind")
         kwargs = copy(definition)
         return cls(kind, **kwargs)
 
     def into_definition(self) -> dict:
         """
         Handler for ``gordo.serializer.into_definition``
 
         Returns
         -------
-        dict
 
         """
         definition = copy(self.kwargs)
         definition["kind"] = self.kind
         return definition
 
     @property
@@ -245,27 +238,22 @@
         **kwargs,
     ):
         """
         Fit the model to X given y.
 
         Parameters
         ----------
-        X: Union[np.ndarray, pd.DataFrame, xr.Dataset]
+        X
             numpy array or pandas dataframe
-        y: Union[np.ndarray, pd.DataFrame, xr.Dataset]
+        y
             numpy array or pandas dataframe
-        sample_weight: np.ndarray
+        sample_weight
             array like - weight to assign to samples
         kwargs
             Any additional kwargs to supply to keras fit method.
-
-        Returns
-        -------
-        self
-            'KerasAutoEncoder'
         """
 
         # Reshape y if needed, and set n features of target
         if isinstance(y, np.ndarray) and y.ndim == 1:
             y = y.reshape(-1, 1)
 
         logger.debug(f"Fitting to data of length: {len(X)}")
@@ -287,24 +275,18 @@
         return self
 
     def predict(self, X: np.ndarray, **kwargs) -> np.ndarray:
         """
 
         Parameters
         ----------
-        X: np.ndarray
+        X
             Input data
-        kwargs: dict
+        kwargs
             kwargs which are passed to Kera's ``predict`` method
-
-
-        Returns
-        -------
-        results:
-            np.ndarray
         """
         kwargs.setdefault("verbose", 0)
         return self.model.predict(X, **kwargs)
 
     def get_params(self, **params):
         """
         Gets the parameters for this estimator
@@ -312,15 +294,14 @@
         Parameters
         ----------
         params
             ignored (exists for API compatibility).
 
         Returns
         -------
-        Dict[str, Any]
             Parameters used in this estimator
         """
         params = super().get_params(**params)
         params.pop("build_fn", None)
         params.update({"kind": self.kind})
         params.update(self.kwargs)
         return params
@@ -347,15 +328,14 @@
         with a key "params" pointing another dictionary with various parameters.
         The metrics are defined in the params dictionary under "metrics".
         For each of the metrics there is a key who's value is a list of values for this
         metric per epoch.
 
         Returns
         -------
-        Dict
             Metadata dictionary, including a history object if present
         """
         if hasattr(self, "model") and hasattr(self, "history"):
             history = self.history.history
             history["params"] = self.history.params
             return {"history": history}
         else:
@@ -375,26 +355,25 @@
         **kwargs,
     ) -> float:
         """
         Returns the explained variance score between auto encoder's input vs output
 
         Parameters
         ----------
-        X: Union[np.ndarray, pd.DataFrame]
+        X
             Input data to the model
-        y: Union[np.ndarray, pd.DataFrame]
+        y
             Target
-        sample_weight: Optional[np.ndarray]
+        sample_weight
             sample weights
         kwargs
             Additional kwargs for model.predict()
 
         Returns
         -------
-        score: float
             Returns the explained variance score
         """
         if not hasattr(self, "model"):
             raise NotFittedError(
                 f"This {self.__class__.__name__} has not been fitted yet."
             )
 
@@ -402,16 +381,17 @@
         out = self.model.predict(X, **kwargs)
 
         return explained_variance_score(y, out)
 
 
 class KerasRawModelRegressor(KerasAutoEncoder):
     """
-    Create a scikit-learn like model with an underlying tensorflow.keras model
+    Create a scikit-learn like model with an underlying ``tensorflow.keras`` model
     from a raw config.
+
     Examples
     --------
     >>> import yaml
     >>> import numpy as np
     >>> config_str = '''
     ...   # Arguments to the .compile() method
     ...   compile:
@@ -461,46 +441,44 @@
 
         model.compile(**kwargs)
         return model
 
 
 class KerasLSTMBaseEstimator(KerasBaseEstimator, TransformerMixin, metaclass=ABCMeta):
     """
-    Abstract Base Class to allow to train a many-one LSTM autoencoder and an LSTM
-    1 step forecast
+    Abstract Base Class to allow to train a many-one LSTM autoencoder and an LSTM 1 step forecast
     """
 
     def __init__(
         self,
         kind: Union[Callable, str],
         lookback_window: int = 1,
         batch_size: int = 32,
         **kwargs,
     ) -> None:
         """
         Parameters
         ----------
-        kind: Union[Callable, str]
+        kind
             The structure of the model to build. As designated by any registered builder
-            functions, registered with
-            `gordo.machine.model.register.register_model_builder`.
+            functions, registered with :func:`gordo.machine.model.register.register_model_builder`.
             Alternatively, one may pass a builder function directly to this argument.
-            Such a function should accept `n_features` as it's first argument, and pass
-            any additional parameters to `**kwargs`.
-        lookback_window: int
+            Such a function should accept ``n_features`` as it's first argument, and pass
+            any additional parameters to ``**kwargs``.
+        lookback_window
             Number of timestamps (lags) used to train the model.
-        batch_size: int
+        batch_size
             Number of training examples used in one epoch.
-        epochs: int
+        epochs
             Number of epochs to train the model. An epoch is an iteration over the
             entire data provided.
-        verbose: int
+        verbose
             Verbosity mode. Possible values are 0, 1, or 2 where 0 = silent,
             1 = progress bar, 2 = one line per epoch.
-        kwargs: dict
+        kwargs
             Any arguments which are passed to the factory building function and/or any
             additional args to be passed to the intermediate fit method.
         """
         self.lookback_window = lookback_window
         self.batch_size = batch_size
         kwargs["lookback_window"] = lookback_window
         kwargs["kind"] = kind
@@ -537,15 +515,14 @@
 
     def get_metadata(self):
         """
         Add number of forecast steps to metadata
 
         Returns
         -------
-        metadata: dict
             Metadata dictionary, including forecast steps.
         """
         metadata = super().get_metadata()
         metadata.update({"forecast_steps": self.lookahead})
         return metadata
 
     def _validate_and_fix_size_of_X(self, X):
@@ -566,24 +543,23 @@
     ) -> "KerasLSTMForecast":
 
         """
         This fits a one step forecast LSTM architecture.
 
         Parameters
         ----------
-        X: np.ndarray
+        X
            2D numpy array of dimension n_samples x n_features. Input data to train.
-        y: np.ndarray
+        y
            2D numpy array representing the target
-        kwargs: dict
-            Any additional args to be passed to Keras `fit_generator` method.
+        kwargs
+            Any additional args to be passed to Keras ``fit_generator`` method.
 
         Returns
         -------
-        class:
             KerasLSTMForecast
 
         """
 
         X = X.values if isinstance(X, pd.DataFrame) else X
         y = y.values if isinstance(y, pd.DataFrame) else y
 
@@ -624,27 +600,23 @@
         self.model.fit(tsg, shuffle=False, **gen_kwargs)
         return self
 
     def predict(self, X: np.ndarray, **kwargs) -> np.ndarray:
         """
         Parameters
         ----------
-         X: np.ndarray
-            Data to predict/transform. 2D numpy array of dimension `n_samples x
-            n_features` where `n_samples` must be > lookback_window.
+        X
+            Data to predict/transform. 2D numpy array of dimension ``n_samples x n_features`` where ``n_samples`` must be > lookback_window.
 
         Returns
         -------
-        results: np.ndarray
-                 2D numpy array of dimension `(n_samples - lookback_window) x
-                 2*n_features`.  The first half of the array `(results[:,
-                 :n_features])` corresponds to X offset by `lookback_window+1` (i.e.,
-                 `X[lookback_window:,:]`) whereas the second half corresponds to the
-                 predicted values of `X[lookback_window:,:]`.
-
+            2D numpy array of dimension ``(n_samples - lookback_window) x 2*n_features``.
+            The first half of the array ``(results[:, :n_features])`` corresponds to X offset
+            by ``lookback_window+1`` (i.e., ``X[lookback_window:,:]``) whereas the second half corresponds to
+            the predicted values of ``X[lookback_window:,:]``.
 
         Example
         -------
         >>> import numpy as np
         >>> from gordo.machine.model.factories.lstm_autoencoder import lstm_model
         >>> from gordo.machine.model.models import KerasLSTMForecast
         >>> #Define train/test data
@@ -677,30 +649,29 @@
         X: Union[np.ndarray, pd.DataFrame],
         y: Union[np.ndarray, pd.DataFrame],
         sample_weight: Optional[np.ndarray] = None,
         **kwargs,
     ) -> float:
         """
         Returns the explained variance score between 1 step forecasted input and true
-        input at next time step (note: for LSTM X is offset by `lookback_window`).
+        input at next time step (note: for LSTM X is offset by ``lookback_window``).
 
         Parameters
         ----------
-        X: Union[np.ndarray, pd.DataFrame]
+        X
             Input data to the model.
-        y: Union[np.ndarray, pd.DataFrame]
+        y
             Target
-        sample_weight: Optional[np.ndarray]
+        sample_weight
             Sample weights
         kwargs
             Additional kwargs for predict
 
         Returns
         -------
-        score: float
             Returns the explained variance score.
         """
         if not hasattr(self, "model"):
             raise NotFittedError(
                 f"This {self.__class__.__name__} has not been fitted yet."
             )
 
@@ -728,44 +699,43 @@
     X: np.ndarray,
     y: Optional[np.ndarray],
     batch_size: int,
     lookback_window: int,
     lookahead: int,
 ) -> tensorflow.keras.preprocessing.sequence.TimeseriesGenerator:
     """
-    Provides a `keras.preprocessing.sequence.TimeseriesGenerator` for use with
+    Provides a :class:`keras.preprocessing.sequence.TimeseriesGenerator` for use with
     LSTM's, but with the added ability to specify the lookahead of the target in y.
 
     If lookahead==0 then the generated samples in X will have as their last element
     the same as the corresponding Y. If lookahead is 1 then the values in Y is shifted
     so it is one step in the future compared to the last value in the samples in X,
     and similar for larger values.
 
 
     Parameters
     ----------
-    X: np.ndarray
+    X
         2d array of values, each row being one sample.
-    y: Optional[np.ndarray]
+    y
         array representing the target.
-    batch_size: int
+    batch_size
         How big should the generated batches be?
-    lookback_window: int
+    lookback_window
         How far back should each sample see. 1 means that it contains a single
         measurement
-    lookahead: int
+    lookahead
         How much is Y shifted relative to X
 
     Returns
     -------
-    TimeseriesGenerator
         3d matrix with a list of batchX-batchY pairs, where batchX is a batch of
-        X-values, and correspondingly for batchY. A batch consist of `batch_size` nr
+        X-values, and correspondingly for batchY. A batch consist of ``batch_size`` nr
         of pairs of samples (or y-values), and each sample is a list of length
-        `lookback_window`.
+        ``lookback_window``.
 
     Examples
     -------
     >>> import numpy as np
     >>> X, y = np.random.rand(100,2), np.random.rand(100, 2)
     >>> gen = create_keras_timeseriesgenerator(X, y,
     ...                                        batch_size=10,
```

### Comparing `gordo-5.0.2/gordo/machine/model/register.py` & `gordo-5.0.3/gordo/machine/model/register.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 from tensorflow import keras
 
 logger = logging.getLogger(__name__)
 
 
 class register_model_builder:
     """
-    Decorator to register a function as an available 'type' in supporting
-    factory classes such as gordo_compontents.models._models.KerasAutoEncoder.
+        Decorator to register a function as an available 'type' in supporting
+        factory classes such as :class:`gordo.machine.model.models.KerasAutoEncoder`.
 
-    When submitting the config file, it's important that the 'kind' is compatible
-    with 'type'.
+        When submitting the config file, it's important that the 'kind' is compatible
+        with 'type'.
 
-    ie. 'type': 'KerasAutoEncoder' should support the object returned by a given
-    decorated function.
+        ie. 'type': 'KerasAutoEncoder' should support the object returned by a given
+        decorated function.
 
 
-    Example for KerasAutoEncoder:
+    .. code:: python
 
-    from gordo_compontents.models.register import register_model_builder
+        from gordo_compontents.models.register import register_model_builder
 
-    @register_model_builder(type='KerasAutoEncoder')
-    def special_keras_model_builder(n_features, ...):
-        ...
+        @register_model_builder(type='KerasAutoEncoder')
+        def special_keras_model_builder(n_features, ...):
+            ...
+
+        A valid yaml config would be:
+        model:
+            gordo.machine.models.KerasAutoEncoder:
+                kind: special_keras_model_builder
 
-    A valid yaml config would be:
-    model:
-        gordo.machine.models.KerasAutoEncoder:
-            kind: special_keras_model_builder
     """
 
     """
     Mapping of type: kind: function.
     ie.
     {
         'KerasAutoEncoder' : {'special_keras_model_builder': <gordo.builder.....>},
```

### Comparing `gordo-5.0.2/gordo/machine/model/transformers/imputer.py` & `gordo-5.0.3/gordo/machine/model/transformers/imputer.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,26 +20,26 @@
         """
         Fill inf/-inf values of a 2d array/dataframe with imputed or provided values
         By default it will find the min and max of each feature/column and fill -infs/infs
         with those values +/- ``delta``
 
         Parameters
         ----------
-        inf_fill_value: numeric
+        inf_fill_value
             Value to fill 'inf' values
-        neg_inf_fill_value: numeric
+        neg_inf_fill_value
             Value to fill '-inf' values
-        strategy: str
+        strategy
             How to fill values, irrelevant if fill value is provided.
             choices: 'extremes', 'minmax'
             -'extremes' will use the min and max values for the current datatype.
             such that 'inf' in a float32 dataset will have float32's largest value inserted.
             - 'minmax' will look at the min and max values in the feature where the -inf / inf
             appears and fill with the max/min found in that feature.
-        delta: float
+        delta
             Only applicable if ``strategy='minmax'``
             Will add/subtract the max/min value, by feature, by this delta. If the max value
             in a feature was 10 and ``delta=2`` any inf value will be filled with 12.
             Likewise, if the min feature was -10 any -inf will be filled with -12.
         """
         self.inf_fill_value = inf_fill_value
         self.neg_inf_fill_value = neg_inf_fill_value
```

### Comparing `gordo-5.0.2/gordo/machine/model/utils.py` & `gordo-5.0.3/gordo/machine/model/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     before applying the metrics.
 
 
     Parameters
     ----------
     metric
         Metric which must accept y_true and y_pred of the same length
-    scaler :  Optional[TransformerMixin]
+    scaler
         Transformer which will be applied on y and y_pred before the metrics is
-        calculated. Must have method `transform`, so for most scalers it must already
-        be fitted on `y`.
+        calculated. Must have method ``transform``, so for most scalers it must already
+        be fitted on ``y``.
     """
 
     @functools.wraps(metric)
     def _wrapper(y_true, y_pred, *args, **kwargs):
         if scaler:
             logger.debug(
                 "Transformer provided to metrics wrapper, scaling y and y_pred before "
@@ -57,33 +57,32 @@
     """
     Construct a dataframe which has a MultiIndex column consisting of top level keys
     'model-input' and 'model-output'. Takes care of aligning model output if different
     than model input lengths, as setting column names based on passed tags and target_tag_list.
 
     Parameters
     ----------
-    tags: List[Union[str, SensorTag]]
+    tags
         Tags which will be assigned to ``model-input`` and/or ``model-output`` if
         the shapes match.
-    model_input: np.ndarray
+    model_input
         Original input given to the model
-    model_output: np.ndarray
+    model_output
         Raw model output
-    target_tag_list: Optional[Union[List[SensorTag], List[str]]]
+    target_tag_list
         Tags to be assigned to ``model-output`` if not assigned but model output matches
         model input, ``tags`` will be used.
-    index: Optional[np.ndarray]
+    index
         The index which should be assigned to the resulting dataframe, will be clipped
         to the length of ``model_output``, should the model output less than its input.
-    frequency: Optional[datetime.timedelta]
+    frequency
         The spacing of the time between points.
 
     Returns
     -------
-    pd.DataFrame
     """
 
     # Set target_tag_list to default to tags if not specified.
     target_tag_list = target_tag_list if target_tag_list is not None else tags
 
     # match length of output, and ensure we're working with numpy arrays, not pandas.
     model_input = getattr(model_input, "values", model_input)[-len(model_output) :, :]
```

### Comparing `gordo-5.0.2/gordo/machine/validators.py` & `gordo-5.0.3/gordo/machine/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 logger = logging.getLogger(__name__)
 
 
 class BaseDescriptor:
     """
     Base descriptor class
 
-    New object should override __set__(self, instance, value) method to check
+    New object should override ``__set__(self, instance, value)`` method to check
     if 'value' meets required needs.
     """
 
     def __get__(self, instance, owner):
         return instance.__dict__[self.name]
 
     def __set_name__(self, owner, name):
@@ -32,15 +32,15 @@
 
     def __set__(self, instance, value):
         raise NotImplementedError("Setting value not implemented for this Validator!")
 
 
 class ValidDataset(BaseDescriptor):
     """
-    Descriptor for attributes requiring type :class:`gordo.workflow.config_elements.Dataset`
+    Descriptor for attributes requiring type :class:`gordo_core.time_series.TimeSeriesDataset`
     """
 
     def __set__(self, instance, value):
 
         # Avoid circular dependency imports
         from gordo_core.base import GordoBaseDataset
 
@@ -49,15 +49,15 @@
                 f"Expected value to be an instance of GordoBaseDataset, found {value}"
             )
         instance.__dict__[self.name] = value
 
 
 class ValidDatasetKwargs(BaseDescriptor):
     """
-    Descriptor for attributes requiring type :class:`gordo.workflow.config_elements.Dataset`
+    Descriptor for attributes requiring type :class:`gordo_core.time_series.TimeSeriesDataset`
     """
 
     def _verify_resolution(self, resolution: str):
         """
         Verifies that a resolution string is supported in pandas
         """
         try:
@@ -174,29 +174,28 @@
     """
     Resource limitations must be higher or equal to resource requests, if they are
     both specified. This bumps any limits to the corresponding request if they are both
     set.
 
     Parameters
     ----------
-    resources: dict
+    resources
         Dictionary with possible requests/limits
 
     Examples
     --------
     >>> fix_resource_limits({"requests": {"cpu": 10}, "limits":{"cpu":9}})
     {'requests': {'cpu': 10}, 'limits': {'cpu': 10}}
     >>> fix_resource_limits({"requests": {"cpu": 10}})
     {'requests': {'cpu': 10}}
 
 
     Returns
     -------
-    dict:
-        A copy of `resource_dict` with the any limits bumped to the corresponding request if
+        A copy of ``resource_dict`` with the any limits bumped to the corresponding request if
         they are both set.
     """
     resources = copy.deepcopy(resources)
     requests = resources.get("requests", dict())
     limits = resources.get("limits", dict())
     request_memory = requests.get("memory")
     limits_memory = limits.get("memory")
@@ -265,18 +264,18 @@
         ):
             raise ValueError("Requires setting a non-empty list of strings")
         instance.__dict__[self.name] = value
 
 
 class ValidUrlString(BaseDescriptor):
     """
-    Descriptor for use in objects which require valid URL values.
-    Where 'valid URL values' is Gordo's version: alphanumeric with dashes.
+        Descriptor for use in objects which require valid URL values.
+        Where 'valid URL values' is Gordo's version: alphanumeric with dashes.
 
-    Use:
+        Use:
 
     .. code-block:: python
 
         class MySpecialClass:
 
             url_attribute = ValidUrlString()
 
@@ -303,19 +302,17 @@
     def valid_url_string(string: str) -> bool:
         """
         What we (Gordo) deem to be a suitable URL is the same as kubernetes
         lowercase alphanumeric with dashes but not ending or starting with a dash
 
         Parameters
         ----------
-            string: str - String to check
+        string
+            String to check
 
-        Returns
-        -------
-            bool
         """
         return bool(
             re.match(
                 r"^([a-z0-9]([-a-z0-9]*[a-z0-9])?(\.[a-z0-9]([-a-z0-9]*[a-z0-9])?)*)$",
                 string,
             )
         )
```

### Comparing `gordo-5.0.2/gordo/reporters/base.py` & `gordo-5.0.3/gordo/reporters/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def to_dict(self) -> dict:
         """
         Serialize this object into a dict representation, which can be used to
         initialize a new object after popping 'type' from the dict.
 
         Returns
         -------
-        dict
         """
         return serializer.into_definition(self)
 
     @classmethod
     def from_dict(cls, config: Dict[str, Any]) -> "BaseReporter":
         """
         Reconstruct the reporter from a dict representation or a single
```

### Comparing `gordo-5.0.2/gordo/reporters/mlflow.py` & `gordo-5.0.3/gordo/reporters/mlflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 def _validate_dict(d: dict, required_keys: List[str]):
     """
     Validate the required keys are contained in provided dictionary
 
     Parameters
     ----------
-    d: dict
+    d
         Dictionary to validate.
-    required_keys: List[str]
+    required_keys
         Keys that must be present in provided dictionary.
     """
     if any([key not in d for key in required_keys]):
         raise MlflowLoggingError(
             f"Required keys for this dictionary include {', '.join(required_keys)}."
         )
 
@@ -55,15 +55,15 @@
     workspace_kwargs: dict = {}, service_principal_kwargs: dict = {}
 ) -> MlflowClient:
     """
     Set remote tracking URI for mlflow to AzureML workspace
 
     Parameters
     ----------
-    workspace_kwargs: dict
+    workspace_kwargs
         AzureML Workspace configuration to use for remote MLFlow tracking. An
         empty dict will result in local logging by the MlflowClient.
         Example::
 
             `{
                  "subscription_id":<value>,
                  "resource_group":<value>,
@@ -78,15 +78,14 @@
                  "tenant_id":<value>,
                  "service_principal_id":<value>,
                  "service_principal_password":<value>
              }`
 
     Returns
     -------
-    client: mlflow.tracking.MlflowClient
         Client with tracking uri set to AzureML if configured.
     """
     logger.info("Creating MLflow tracking client.")
 
     tracking_uri = None
 
     # Get AzureML tracking_uri if using Azure as backend
@@ -124,24 +123,23 @@
 
     The model key corresponds to a unique configuration of the model. The corresponding
     run must be manually stopped using the `mlflow.tracking.MlflowClient.set_terminated`
     method.
 
     Parameters
     ----------
-    client: mlflow.tracking.MlflowClient
+    client
         Client with tracking uri set to AzureML if configured.
-    experiment_name: str
+    experiment_name
         Name of experiment to log to.
-    model_key: str
+    model_key
         Unique ID of model configuration.
 
     Returns
     -------
-    run_id: str
         Unique ID of MLflow run to log to.
     """
     experiment = client.get_experiment_by_name(experiment_name)
 
     experiment_id = (
         getattr(experiment, "experiment_id")
         if experiment
@@ -152,20 +150,19 @@
 
 def _datetime_to_ms_since_epoch(dt: datetime) -> int:
     """
     Convert datetime to milliseconds since Unix epoch (UTC)
 
     Parameters
     ----------
-    dt: datetime.datetime
+    dt
         Timestamp to convert (can be timezone aware or naive).
 
     Returns
     -------
-    dt: int
         Timestamp as milliseconds since Unix epoch
 
     Example
     -------
     >>> dt = datetime(1970, 1, 1, 0, 0)
     >>> _datetime_to_ms_since_epoch(dt)
     0
@@ -177,36 +174,33 @@
 
 def epoch_now() -> int:
     """
     Get current timestamp in UTC as milliseconds since Unix epoch.
 
     Returns
     -------
-    now: int
         Milliseconds since Unix epoch.
     """
     return _datetime_to_ms_since_epoch(datetime.now(tz=UTC))
 
 
 def get_machine_log_items(machine: Machine) -> Tuple[List[Metric], List[Param]]:
     """
     Create flat lists of MLflow logging entities from multilevel dictionary
 
-    For more information, see the mlflow docs:
-    https://www.mlflow.org/docs/latest/python_api/mlflow.tracking.html#mlflow.tracking.MlflowClient.log_batch
+    For more information, see the `mlflow docs <https://www.mlflow.org/docs/latest/python_api/mlflow.tracking.html#mlflow.tracking.MlflowClient.log_batch>`_.
 
     Parameters
     ----------
-    machine: Machine
+    machine
+        Machine to log.
 
     Returns
     -------
-    metrics: List[Metric]
         List of MLFlow Metric objects to log.
-    params: List[Param]
         List of MLFlow Param objects to log.
     """
 
     metrics: List[Metric] = list()
     build_metadata = machine.metadata.build_metadata
 
     # Project/machine parameters
@@ -292,26 +286,25 @@
     Also, there the 1mb request size is not evaluated here, as doing this
     should not be necessary and is not addressable in a succint way. MLflow
     also has a limit of 1000 log items per request, but reaching this is not
     possible with AzureML's current limit on metrics.
 
     Parameters
     ----------
-    metrics: List[Metric]
+    metrics
         List of MLFlow Metric objects to log.
-    params: List[Param]
+    params
         List of MLFlow Param objects to log.
-    n_max_metrics:int
+    n_max_metrics
         Limit to number of metrics AzureML allows per batch log request payload.
-    n_max_params:int
+    n_max_params
         Limit to number of params MLFlow allows per batch log request payload.
 
     Returns
     -------
-    log_batches: List[Dict[str, Union[Metric, Param]]]
         List of MlflowClinet.log_batch keyworkd arguments, split to quatnitites
         that respect limits present for MLFlow and AzureML.
     """
 
     def _calc_n_batches(n: int, n_max: int):
         """
         Calculate the number of batches required to log n items with batches of n_max
@@ -341,21 +334,20 @@
 
 def get_kwargs_from_secret(name: str, keys: List[str]) -> dict:
     """
     Get keyword arguments dictionary from secrets environment variable
 
     Parameters
     ----------
-    name: str
+    name
         Name of the environment variable whose content is a colon separated
         list of secrets.
 
     Returns
     -------
-    kwargs: dict
         Dictionary of keyword arguments parsed from environment variable.
     """
     secret_str = os.getenv(name)
 
     if secret_str is None:
         raise MlflowLoggingError(f"The value for env var '{name}' must not be `None`.")
 
@@ -377,15 +369,14 @@
 
     The name of this environment variable is set in the Argo workflow template,
     and its value should be in the format:
     `<subscription_id>:<resource_group>:<workspace_name>`.
 
     Returns
     -------
-    workspace_kwargs: dict
         AzureML Workspace configuration to use for remote MLFlow tracking. See
         :func:`gordo.builder.mlflow_utils.get_mlflow_client`.
     """
     return get_kwargs_from_secret(
         "AZUREML_WORKSPACE_STR", ["subscription_id", "resource_group", "workspace_name"]
     )
 
@@ -395,15 +386,14 @@
 
     The name of this environment variable is set in the Argo workflow template,
     and its value should be in the format:
     `<tenant_id>:<service_principal_id>:<service_principal_password>`
 
     Returns
     -------
-    service_principal_kwargs: dict
         AzureML ServicePrincipalAuthentication keyword arguments. See
         :func:`gordo.builder.mlflow_utils.get_mlflow_client`
     """
     return get_kwargs_from_secret(
         "DL_SERVICE_AUTH_STR",
         ["tenant_id", "service_principal_id", "service_principal_password"],
     )
@@ -417,22 +407,22 @@
     service_principal_kwargs: dict = {},
 ):
     """
     Generate MLflow logger function with either a local or AzureML backend
 
     Parameters
     ----------
-    name: str
+    name
         The name of the log group to log to (e.g. a model name).
-    model_key: str
+    model_key
         Unique ID of logging run.
-    workspace_kwargs: dict
+    workspace_kwargs
         AzureML Workspace configuration to use for remote MLFlow tracking. See
         :func:`gordo.builder.mlflow_utils.get_mlflow_client`.
-    service_principal_kwargs: dict
+    service_principal_kwargs
         AzureML ServicePrincipalAuthentication keyword arguments. See
         :func:`gordo.builder.mlflow_utils.get_mlflow_client`
 
     Example
     -------
     >>> with tempfile.TemporaryDirectory as tmp_dir:
     ...     mlflow.set_tracking_uri(f"file:{tmp_dir}")
@@ -453,19 +443,19 @@
 
 def log_machine(mlflow_client: MlflowClient, run_id: str, machine: Machine):
     """
     Send logs to configured MLflow backend
 
     Parameters
     ----------
-    mlflow_client: MlflowClient
+    mlflow_client
         Client instance to call logging methods from.
-    run_id: str
+    run_id
         Unique ID off MLflow Run to log to.
-    machine: Machine
+    machine
         Machine to log with MlflowClient.
     """
     # Log machine metrics and params
     for batch_kwargs in batch_log_items(*get_machine_log_items(machine)):
         mlflow_client.log_batch(run_id, **batch_kwargs)
 
     # Send configs as JSON artifacts
```

### Comparing `gordo-5.0.2/gordo/reporters/postgres.py` & `gordo-5.0.3/gordo/reporters/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,18 @@
     def report(self, machine: GordoMachine):
         """
         Log a machine to Postgres where top level keys, 'name', 'dataset', 'model',
         and 'metadata' mappings to BinaryJSON fields.
 
         Parameters
         ----------
-        machine: gordo.machine.Machine
+        machine
 
         Returns
         -------
-        None
         """
         try:
             with self.db.atomic():
                 logger.info(f"Inserting machine {machine.name} in sql")  # type: ignore
 
                 # Ensure it's serializable using MachineJSONEncoder
                 record = json.loads(
```

### Comparing `gordo-5.0.2/gordo/serializer/from_definition.py` & `gordo-5.0.3/gordo/serializer/from_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         List of steps for the Pipeline / FeatureUnion
     constructor_class
         What to place the list of transformers into,
         either sklearn.pipeline.Pipeline/FeatureUnion
 
     Returns
     -------
-    sklearn.pipeline.Pipeline
         pipeline
     """
     # Avoid some mutation
     definition = copy.deepcopy(pipe_definition)
     return _build_step(definition)
 
 
@@ -138,29 +137,30 @@
     step: Union[str, Dict[str, Dict[str, Any]]]
 ) -> Union[FeatureUnion, Pipeline, BaseEstimator]:
     """
     Build an isolated step within a transformer list, given a dict config
 
     Parameters
     ----------
-    step: dict/str - A dict, with a single key and associated dict
-                     where the associated dict are parameters for the
-                     given step.
-
-                     Example: {'sklearn.preprocessing.PCA':
-                                    {'n_components': 4}
-                              }
-                        Gives:  PCA(n_components=4)
-
-                    Alternatively, 'step' can be a single string, in
-                    which case the step will be initiated w/ default
-                    params.
+    step
+        A dict, with a single key and associated dict
+        where the associated dict are parameters for the
+        given step.
+
+        Example: {'sklearn.preprocessing.PCA':
+                    {'n_components': 4}
+              }
+        Gives:  PCA(n_components=4)
+
+        Alternatively, 'step' can be a single string, in
+        which case the step will be initiated w/ default
+        params.
 
-                    Example: 'sklearn.preprocessing.PCA'
-                        Gives: PCA()
+        Example: 'sklearn.preprocessing.PCA'
+            Gives: PCA()
     Returns
     -------
         Scikit-Learn Transformer or BaseEstimator
     """
     logger.debug(f"Building step: {step}")
 
     # Here, 'step' _should_ be a dict with a single key
@@ -248,26 +248,25 @@
         )
 
 
 def _build_callbacks(definitions: list):
     """
     Parameters
     ----------
-    definitions: List
+    definitions
         List of callbacks definitions
 
     Examples
     --------
     >>> callbacks=_build_callbacks([{'tensorflow.keras.callbacks.EarlyStopping': {'monitor': 'val_loss,', 'patience': 10}}])
     >>> type(callbacks[0])
     <class 'keras.callbacks.EarlyStopping'>
 
     Returns
     -------
-    dict
     """
     callbacks = []
     for callback in definitions:
         callbacks.append(_build_step(callback))
     return callbacks
 
 
@@ -278,15 +277,15 @@
 
     Additionally, if the value of the top level is a dict, and that dict's len(.keys()) == 1
     AND that key can be loaded, it's assumed to be a class whose associated values
     should be passed in as kwargs.
 
     Parameters
     ----------
-    params: dict
+    params
         key value pairs of kwargs, which can have full class paths defined.
 
     Examples
     --------
     >>> params = {"key1": "value1"}
     >>> assert _load_param_classes(params) == params  # No modifications
 
@@ -300,15 +299,14 @@
     >>> params = {"base_estimator": {"sklearn.ensemble.RandomForestRegressor": {"n_estimators": 20}}}
     >>> print(_load_param_classes(params))
     {'base_estimator': RandomForestRegressor(n_estimators=20)}
 
 
     Returns
     -------
-    dict
         Updated params which has any possible class paths loaded up as instantiated
         objects
     """
     params = copy.copy(params)
     for key, value in params.items():
 
         # If value is a simple string, try to load the model/class
@@ -358,14 +356,14 @@
 
 def load_params_from_definition(definition: dict) -> dict:
     """
     Deserialize each value from a dictionary. Could be used for preparing kwargs for methods
 
     Parameters
     ----------
-    definition: dict
+    definition
     """
     if not isinstance(definition, dict):
         raise ValueError(
             "Expected definition to be a dict," f"found: {type(definition)}"
         )
     return _load_param_classes(definition)
```

### Comparing `gordo-5.0.2/gordo/serializer/into_definition.py` & `gordo-5.0.3/gordo/serializer/into_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,24 @@
     """
     Convert an instance of ``sklearn.pipeline.Pipeline`` into a dict definition
     capable of being reconstructed with
     ``gordo.serializer.from_definition``
 
     Parameters
     ----------
-    pipeline: sklearn.pipeline.Pipeline
+    pipeline
         Instance of pipeline to decompose
-    prune_default_params: bool
+    prune_default_params
         Whether to prune the default parameters found in current instance of the transformers
         vs what their default params are.
-    tuples_to_list: bool
+    tuples_to_list
         Convert all tuples in output to lists
 
     Returns
     -------
-    dict
         definitions for the pipeline, compatible to be reconstructed with
         :func:`gordo.serializer.from_definition`
 
     Example
     -------
     >>> import yaml
     >>> from sklearn.pipeline import Pipeline
@@ -80,15 +79,14 @@
         Whether to output the default parameter values into the definition. If True,
         only those parameters differing from the default params will be output.
     tuples_to_list
         Convert all tuples in output to lists
 
     Returns
     -------
-    dict
         decomposed node - Where key is the import string for the class and associated value
         is a dict of parameters for that class.
     """
 
     import_str = f"{step.__module__}.{step.__class__.__name__}"
 
     if hasattr(step, "into_definition"):
```

### Comparing `gordo-5.0.2/gordo/serializer/serializer.py` & `gordo-5.0.3/gordo/serializer/serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 def dumps(model: Union[Pipeline, GordoBase]) -> bytes:
     """
     Dump a model into a bytes representation suitable for loading from
     ``gordo.serializer.loads``
 
     Parameters
     ----------
-    model: Union[Pipeline, GordoBase]
+    model
         A gordo model/pipeline
 
     Returns
     -------
-    bytes
         Serialized model which supports loading via ``serializer.loads()``
 
     Example
     -------
     >>> from gordo.machine.model.models import KerasAutoEncoder
     >>> from gordo import serializer
     >>>
@@ -51,20 +50,19 @@
 
 def loads(bytes_object: bytes) -> GordoBase:
     """
     Load a GordoBase model from bytes dumped from ``gordo.serializer.dumps``
 
     Parameters
     ----------
-    bytes_object: bytes
+    bytes_object
         Bytes to be loaded, should be the result of `serializer.dumps(model)`
 
     Returns
     -------
-    Union[GordoBase, Pipeline, BaseEstimator]
         Custom gordo model, scikit learn pipeline or other scikit learn like object.
     """
     return pickle.loads(bytes_object)
 
 
 def metadata_path(
     source_dir: Union[os.PathLike, str]
@@ -99,21 +97,20 @@
 def load_metadata(source_dir: Union[os.PathLike, str]) -> dict:
     """
     Load the given metadata.json which was saved during the ``serializer.dump``
     will return the loaded metadata as a dict, or empty dict if no file was found
 
     Parameters
     ----------
-    source_dir: Union[os.PathLike, str]
+    source_dir
         Directory of the saved model, As with serializer.load(source_dir) this
         source_dir can be the top level, or the first dir into the serialized model.
 
     Returns
     -------
-    dict
 
     Raises
     ------
     FileNotFoundError
         If a 'metadata.json' file isn't found in or above the supplied ``source_dir``
     """
     return _load_json_file(source_dir, "metadata.json")
@@ -133,20 +130,19 @@
     a sub directory in the naming scheme: "n_step=<int>-class=<path.to.Class>"
     or the aforementioned naming scheme directory directly. Will return that
     unsterilized object.
 
 
     Parameters
     ----------
-    source_dir: Union[os.PathLike, str]
+    source_dir
         Location of the top level dir the pipeline was saved
 
     Returns
     -------
-    Union[GordoBase, Pipeline, BaseEstimator]
     """
     # This source dir should have a single pipeline entry directory.
     # may have been passed a top level dir, containing such an entry:
     with open(os.path.join(source_dir, "model.pkl"), "rb") as f:
         return pickle.load(f)
 
 
@@ -159,26 +155,25 @@
     """
     Serialize an object into a directory, the object must be pickle-able.
 
     Parameters
     ----------
     obj
         The object to dump. Must be pickle-able.
-    dest_dir: Union[os.PathLike, str]
+    dest_dir
         The directory to which to save the model metadata: dict - any additional
         metadata to be saved alongside this model if it exists, will be returned
         from the corresponding "load" function
-    metadata: Optional dict of metadata which will be serialized to a file together
+    metadata
         with the model, and loaded again by :func:`load_metadata`.
-    info: Optional[str]
+    info
         Current revision info. For now, only used for storing "checksum"
 
     Returns
     -------
-    None
 
     Example
     -------
 
     >>> from sklearn.pipeline import Pipeline
     >>> from sklearn.decomposition import PCA
     >>> from gordo.machine.model.models import KerasAutoEncoder
```

### Comparing `gordo-5.0.2/gordo/serializer/utils.py` & `gordo-5.0.3/gordo/serializer/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/server/blueprints/anomaly.py` & `gordo-5.0.3/gordo/server/blueprints/anomaly.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,20 @@
 def _create_anomaly_response(start_time: float = None):
     """
     Use the current ``X`` and ``y`` to create an anomaly specific response
     using the trained ML model's ``.anomaly()`` method.
 
     Parameters
     ----------
-    start_time: Optional[float]
+    start_time
         Start time to use when timing the processing time of the request, will construct a new
         one if not provided.
 
     Returns
     -------
-    flask.Response
         The formatted anomaly representation response object.
     """
     if start_time is None:
         start_time = timeit.default_timer()
 
     # To use this endpoint, we need a 'y' to calculate the errors.
     if g.y is None:
```

### Comparing `gordo-5.0.2/gordo/server/blueprints/base.py` & `gordo-5.0.3/gordo/server/blueprints/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,14 @@
     """
     Download the trained model
 
     Responds with a serialized copy of the current model being served.
 
     Returns
     -------
-    bytes
         Results from ``gordo.serializer.dumps()``
     """
     serialized_model = serializer.dumps(g.model)
     buff = io.BytesIO(serialized_model)
     return send_file(buff, download_name="model.pickle")
 
 
@@ -210,8 +209,11 @@
     return jsonify(
         {"latest": g.current_revision, "available-revisions": available_revisions}
     )
 
 
 @base_blueprint.route("/gordo/v0/<gordo_project>/expected-models", methods=["GET"])
 def get(gordo_project: str):
+    """
+    Returns list of models for this project. Those models are expected to be built.
+    """
     return jsonify({"expected-models": current_app.config["EXPECTED_MODELS"]})
```

### Comparing `gordo-5.0.2/gordo/server/model_io.py` & `gordo-5.0.3/gordo/server/model_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,19 @@
     """
     Get the raw output from the current model given X.
     Will try to `predict` and then `transform`, raising an error
     if both fail.
 
     Parameters
     ----------
-    X: np.ndarray
+    X
         2d array of sample(s)
 
     Returns
     -------
-    np.ndarray
         The raw output of the model in numpy array form.
     """
     try:
         return model.predict(X)  # type: ignore
 
     # Model may only be a transformer
     except AttributeError:
```

### Comparing `gordo-5.0.2/gordo/server/prometheus/metrics.py` & `gordo-5.0.3/gordo/server/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/server/prometheus/server.py` & `gordo-5.0.3/gordo/server/prometheus/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/server/properties.py` & `gordo-5.0.3/gordo/server/properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     Examples
     --------
     >>> find_path_in_dict(["parent", "child"], {"parent": {"child": 42}})
     42
 
     Parameters
     ----------
-    path: List[str]
-    data: dict
+    path
+    data
 
     Returns
     -------
 
     """
     reversed_path = copy.copy(path)
     reversed_path.reverse()
@@ -69,30 +69,28 @@
 
 def get_tags() -> list[SensorTag]:
     """
     The input tags for this model
 
     Returns
     -------
-    list[SensorTag]
     """
     dataset = g.metadata["dataset"]
     tag_list = dataset["tag_list"]
     build_dataset_metadata = load_build_dataset_metadata()
     additional_fields = get_normalize_additional_fields(dataset)
     return normalize_sensor_tags(build_dataset_metadata, tag_list, **additional_fields)
 
 
 def get_target_tags() -> list[SensorTag]:
     """
     The target tags for this model
 
     Returns
     -------
-    list[SensorTag]
     """
     # TODO refactor this part to have the same tag preparation logic as in TimeSeriesDataset
     orig_target_tag_list = []
     if "target_tag_list" in g.metadata["dataset"]:
         orig_target_tag_list = g.metadata["dataset"]["target_tag_list"]
     if orig_target_tag_list:
         build_dataset_metadata = load_build_dataset_metadata()
```

### Comparing `gordo-5.0.2/gordo/server/server.py` & `gordo-5.0.3/gordo/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 def adapt_proxy_deployment(wsgi_app: typing.Callable) -> typing.Callable:
     """
     Decorator specific to fixing behind-proxy-issues when on Kubernetes and
     using Envoy proxy.
 
     Parameters
     ----------
-    wsgi_app: typing.Callable
+    wsgi_app
         The underlying WSGI application of a flask app, for example
 
     Notes
     -----
     Special note about deploying behind Ambassador, or prefixed proxy paths in general:
 
     When deployed on kubernetes/ambassador there is a prefix in-front of the
@@ -75,15 +75,14 @@
     to the assigned route function.
 
     ie. ``/metadata`` -> metadata route function, by default, but updates
     ``/gordo/v0/some-project-name/some-target/metadata`` -> metadata route function
 
     Returns
     -------
-    Callable
 
     Example
     -------
     >>> app = Flask(__name__)
     >>> app.wsgi_app = adapt_proxy_deployment(app.wsgi_app)
     """
 
@@ -250,32 +249,32 @@
     server_app: str = "gordo.server.server:build_app()",
 ):
     """
     Run application with Gunicorn server using Gevent Async workers
 
     Parameters
     ----------
-    host: str
+    host
         The host to run the server on.
-    port: int
+    port
         The port to run the server on.
-    workers: int
+    workers
         The number of worker processes for handling requests.
-    log_level: str
+    log_level
         The log level for the `gunicorn` webserver. Valid log level names can be found
         in the [gunicorn documentation](http://docs.gunicorn.org/en/stable/settings.html#loglevel).
-    config_module: str
+    config_module
         The config module. Will be passed with `python:` [prefix](https://docs.gunicorn.org/en/stable/settings.html#config).
-    worker_connections: int
+    worker_connections
         The maximum number of simultaneous clients per worker process.
-    threads: str
+    threads
         The number of worker threads for handling requests.
-    worker_class: str
+    worker_class
         The type of workers to use.
-    server_app: str
+    server_app
         The application to run
     """
 
     cmd = [
         "gunicorn",
         "--bind",
         f"{host}:{port}",
```

### Comparing `gordo-5.0.2/gordo/server/utils.py` & `gordo-5.0.3/gordo/server/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,42 +48,40 @@
     df: pd.DataFrame, compression: str = "snappy"
 ) -> bytes:
     """
     Convert a dataframe into bytes representing a parquet table.
 
     Parameters
     ----------
-    df: pd.DataFrame
+    df
         DataFrame to be compressed
-    compression: str
+    compression
         Compression to use, passed to  :func:`pyarrow.parquet.write_table`
 
     Returns
     -------
-    bytes
     """
     table = pa.Table.from_pandas(df)
     buf = pa.BufferOutputStream()
     pq.write_table(table, buf, compression=compression)
     return buf.getvalue().to_pybytes()
 
 
 def dataframe_from_parquet_bytes(buf: bytes) -> pd.DataFrame:
     """
     Convert bytes representing a parquet table into a pandas dataframe.
 
     Parameters
     ----------
-    buf: bytes
+    buf
         Bytes representing a parquet table. Can be the direct result from
         `func`::gordo.server.utils.dataframe_into_parquet_bytes
 
     Returns
     -------
-    pandas.DataFrame
     """
     table = pq.read_table(io.BytesIO(buf))
     return table.to_pandas()
 
 
 def dataframe_to_dict(df: pd.DataFrame) -> dict:
     """
@@ -94,20 +92,19 @@
 
     This allows :func:`json.dumps` to be performed, where :meth:`pandas.DataFrame.to_dict()`
     would convert such a multi-level column dataframe into keys of ``tuple`` objects, which are
     not json serializable. However this ends up working with :meth:`pandas.DataFrame.from_dict`
 
     Parameters
     ----------
-    df: pandas.DataFrame
+    df
         Dataframe expected to have columns of type :class:`pandas.MultiIndex` 2 levels deep.
 
     Returns
     -------
-    List[dict]
         List of records representing the dataframe in a 'flattened' form.
 
 
     Examples
     --------
     >>> import pprint
     >>> import pandas as pd
@@ -149,20 +146,19 @@
     Reconstructed a MultiIndex column dataframe from a previously serialized one.
 
     Expects ``data`` to be a nested dictionary where each top level key has a value
     capable of being loaded from :func:`pandas.core.DataFrame.from_dict`
 
     Parameters
     ----------
-    data: dict
+    data
         Data to be loaded into a MultiIndex column dataframe
 
     Returns
     -------
-    pandas.core.DataFrame
         MultiIndex column dataframe.
 
     Examples
     --------
     >>> serialized = {
     ... 'feature0': {'sub-feature-0': {'2019-01-01': 0, '2019-02-01': 4},
     ...              'sub-feature-1': {'2019-01-01': 1, '2019-02-01': 5}},
@@ -214,23 +210,22 @@
     Verify the dataframe, setting the column names to ``expected_columns``
     if not already labeled and the length of the columns match the length of the expected columns.
 
     If it fails, it will return an instance of :class:`flask.wrappers.Response`
 
     Parameters
     ----------
-    df: pandas.core.DataFrame
+    df
         DataFrame to verify.
-    expected_columns: List[str]
+    expected_columns
         List of expected column names to give if the dataframe does not consist of them
         but the number of columns matches ``len(expected_columns)``
 
     Returns
     -------
-    Union[flask.wrappers.Response, pandas.core.DataFrame]
     """
     if not isinstance(df.columns, pd.MultiIndex):
         if not all(col in df.columns for col in expected_columns):
 
             # If the length doesn't mach, then we can't reliably determine what data we have hre.
             if len(df.columns) != len(expected_columns):
                 msg = dict(
@@ -262,21 +257,20 @@
     the request and assign it to flask's 'g' global request context
 
     If it fails to extract 'X' and (optionally) 'y' from the request, it will **not** run the
     function but return a ``BadRequest`` response notifying the client of the failure.
 
     Parameters
     ----------
-    method: Callable
+    method
         The flask route to decorate, and will return it's own response object
         and will want to use ``flask.g.X`` and/or ``flask.g.y``
 
     Returns
     -------
-    flask.Response
         Will either run a :class:`flask.Response` with status code 400 if it fails
         to extract the X and optionally the y. Otherwise will run the decorated ``method``
         which is also expected to return some sort of :class:`flask.Response` object.
     """
 
     @functools.wraps(method)
     def wrapper_method(*args, **kwargs):
@@ -338,23 +332,22 @@
 @lru_cache(maxsize=int(os.getenv("N_CACHED_MODELS", 2)))
 def load_model(directory: str, name: str) -> BaseEstimator:
     """
     Load a given model from the directory by name.
 
     Parameters
     ----------
-    directory: str
+    directory
         Directory to look for the model
-    name: str
+    name
         Name of the model to load, this would be the sub directory within the
         directory parameter.
 
     Returns
     -------
-    BaseEstimator
     """
     start_time = timeit.default_timer()
     model = serializer.load(os.path.join(directory, name))
     logger.debug(f"Time to load model: {timeit.default_timer() - start_time}s")
     return model
 
 
@@ -370,23 +363,22 @@
 
 def load_metadata(directory: str, name: str) -> dict:
     """
     Load metadata from a directory for a given model by name.
 
     Parameters
     ----------
-    directory: str
+    directory
         Directory to look for the model's metadata
-    name: str
+    name
         Name of the model to load metadata for, this would be the sub directory
         within the directory parameter.
 
     Returns
     -------
-    dict
     """
     compressed_metadata = _load_compressed_metadata(directory, name)
     return pickle.loads(zlib.decompress(compressed_metadata))
 
 
 _n_cached_metadata = int(os.getenv("N_CACHED_METADATA", 250))
```

### Comparing `gordo-5.0.2/gordo/util/disk_registry.py` & `gordo-5.0.3/gordo/util/disk_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 def write_key(registry_dir: Union[os.PathLike, str], key: str, val: AnyStr):
     """Registers a key-value combination into the register. Key must valid as a
     filename.
 
     Parameters
     ----------
-    registry_dir: Union[os.PathLike, str]
+    registry_dir
         Path to the registry. If it does not exists it will be created, including any
         missing folders in the path.
-    key: str
+    key
         Key to use for the key/value. Must be valid as a filename.
-    val: AnyStr
+    val
         Value to write to the registry.
 
     Examples
     --------
     In the following example we use the temp directory as the registry
     >>> import tempfile
     >>> with tempfile.TemporaryDirectory() as tmpdir:
@@ -56,22 +56,21 @@
 def get_value(registry_dir: Union[os.PathLike, str], key: str) -> Optional[AnyStr]:
     """
     Retrieves the value with key reg_key from the registry, None if it does not
     exists.
 
     Parameters
     ----------
-    registry_dir: Union[os.PathLike, str]
+    registry_dir
         Path to the registry. If it does not exist we return None
-    key: str
+    key
         Key to look up in the registry.
 
     Returns
     -------
-    Optional[AnyStr]:
         The value of `key` in the registry, None if no value is registered with that key
         in the registry.
     """
     output_val = None
 
     if registry_dir is None:
         return output_val
@@ -91,22 +90,21 @@
 def delete_value(registry_dir: Union[os.PathLike, str], key: str) -> bool:
     """
     Deletes the value with key reg_key from the registry, and returns True if it
     existed.
 
     Parameters
     ----------
-    registry_dir: Union[os.PathLike, str]
+    registry_dir
         Path to the registry. Does not need to exist
-    key: str
+    key
         Key to look up in the registry.
 
     Returns
     -------
-    bool:
         True if the key existed, false otherwise
     """
     key_file_path = Path(registry_dir).joinpath(key)
     logger.info(f"Looking for registry key {key} at path " f"{key_file_path}")
     # If the model location exists
     if key_file_path.exists():
         key_file_path.unlink()
```

### Comparing `gordo-5.0.2/gordo/util/utils.py` & `gordo-5.0.3/gordo/util/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,19 @@
     """
     Decorator that captures args and kwargs passed to a given method.
     This assumes the decorated method has a self, which has a dict of
     kwargs assigned as an attribute named _params.
 
     Parameters
     ----------
-    method: Callable
+    method
         Some method of an object, with 'self' as the first parameter.
 
     Returns
     -------
-    Any
         Returns whatever the original method would return
     """
 
     @functools.wraps(method)
     def wrapper(self, *args, **kwargs):
 
         sig_params = inspect.signature(method).parameters.items()
```

### Comparing `gordo-5.0.2/gordo/util/version.py` & `gordo-5.0.3/gordo/util/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,26 +90,25 @@
     gordo_version: str,
 ) -> Union[GordoRelease, GordoSpecial, GordoPR, GordoSHA]:
     """
     Parsing gordo version. Also supported gordo docker images tags
 
     Parameters
     ----------
-    gordo_version: str
+    gordo_version
 
     Example
     -------
     >>> parse_version('2.3.5')
     GordoRelease(major=2, minor=3, patch=5, suffix=None)
     >>> parse_version('latest')
     GordoSpecial(special=<Special.LATEST: 'latest'>)
 
     Returns
     -------
-    Union[GordoRelease, GordoSpecial, GordoPR, GordoSHA]
 
     """
     special_version = Special.find(gordo_version)
     if special_version is not None:
         return GordoSpecial(special_version)
     if gordo_version.find(pr_prefix) == 0:
         try:
```

### Comparing `gordo-5.0.2/gordo/utils.py` & `gordo-5.0.3/gordo/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/workflow/config_elements/normalized_config.py` & `gordo-5.0.3/gordo/workflow/config_elements/normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/workflow/config_elements/schemas.py` & `gordo-5.0.3/gordo/workflow/config_elements/schemas.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/workflow/workflow_generator/helpers.py` & `gordo-5.0.3/gordo/workflow/workflow_generator/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,31 +16,30 @@
 def patch_dict(original_dict: dict, patch_dictionary: dict) -> dict:
     """Patches a dict with another. Patching means that any path defines in the
     patch is either added (if it does not exist), or replaces the existing value (if
     it exists). Nothing is removed from the original dict, only added/replaced.
 
     Parameters
     ----------
-    original_dict : dict
+    original_dict
         Base dictionary which will get paths added/changed
-    patch_dictionary: dict
+    patch_dictionary
         Dictionary which will be overlaid on top of original_dict
 
     Examples
     --------
     >>> patch_dict({"highKey":{"lowkey1":1, "lowkey2":2}}, {"highKey":{"lowkey1":10}})
     {'highKey': {'lowkey1': 10, 'lowkey2': 2}}
     >>> patch_dict({"highKey":{"lowkey1":1, "lowkey2":2}}, {"highKey":{"lowkey3":3}})
     {'highKey': {'lowkey1': 1, 'lowkey2': 2, 'lowkey3': 3}}
     >>> patch_dict({"highKey":{"lowkey1":1, "lowkey2":2}}, {"highKey2":4})
     {'highKey': {'lowkey1': 1, 'lowkey2': 2}, 'highKey2': 4}
 
     Returns
     -------
-    dict
         A new dictionary which is the result of overlaying `patch_dictionary` on top of
         `original_dict`
 
     """
     diff = dictdiffer.diff(original_dict, patch_dictionary)
     adds_and_mods = [(f, d, s) for (f, d, s) in diff if f != "remove"]
     return dictdiffer.patch(adds_and_mods, original_dict)
@@ -48,15 +47,15 @@
 
 def parse_argo_version(argo_version: str) -> Optional[version.Version]:
     """
     Try to parse Argo version.
 
     Parameters
     ----------
-    argo_version: str
+    argo_version
 
     Returns
     -------
         None if failed to parse.
     """
     parsed_version = version.parse(argo_version)
     if isinstance(parsed_version, version.Version):
```

### Comparing `gordo-5.0.2/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template` & `gordo-5.0.3/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/gordo/workflow/workflow_generator/workflow_generator.py` & `gordo-5.0.3/gordo/workflow/workflow_generator/workflow_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,20 @@
 
     A valid owner reference is a dict containing at least the keys 'uid', 'name',
     'kind', and 'apiVersion'. Raises `TypeError` if not, or returns
     the list of owner references if they seem valid.
 
     Parameters
     ----------
-    owner_reference_str: str
+    owner_reference_str
         String representation of the list of owner-references, should be parsable as
         yaml/json
 
     Returns
     -------
-    list[dict]
         The list of owner-references
 
     """
     owner_ref = yaml.safe_load(owner_reference_str)
     if not type(owner_ref) == list or len(owner_ref) < 1:
         raise TypeError("Owner-references must be a list with at least one element")
     for oref in owner_ref:
@@ -103,20 +102,19 @@
 
 def load_workflow_template(workflow_template: str) -> jinja2.Template:
     """
     Loads the Jinja2 Template from a specified path
 
     Parameters
     ----------
-    workflow_template: str
+    workflow_template
         Path to a workflow template
 
     Returns
     -------
-    jinja2.Template
         Loaded but non-rendered jinja2 template for the workflow
     """
     path_to_workflow_template = os.path.abspath(workflow_template)
     template_dir = os.path.dirname(path_to_workflow_template)
 
     templateEnv = jinja2.Environment(
         loader=jinja2.FileSystemLoader(template_dir), undefined=jinja2.StrictUndefined
```

### Comparing `gordo-5.0.2/gordo.egg-info/PKG-INFO` & `gordo-5.0.3/gordo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.2
+Version: 5.0.3
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: mlflow
 Provides-Extra: postgres
 Provides-Extra: tests
 Provides-Extra: full
+Provides-Extra: docs
 License-File: LICENSE
 
 
 
 <h1 align="center">Gordo</h1>
 <div align="center">
  <!-- Uncomment line below once we decided on 'logo.png' -->
@@ -50,14 +50,16 @@
 
 ## Components
 
 * [gordo-controller](https://github.com/equinor/gordo-controller/) - Kubernetes controller for the Gordo CRDs.
 * [gordo-core](https://github.com/equinor/gordo-core/) - Gordo core library.
 * [gordo-client](https://github.com/equinor/gordo-client/) - Gordo server's client. It can make predictions from deployed models.
 
+[Documentation is available on Read the Docs](https://gordo1.readthedocs.io/)
+
 ---
 ## Install
 
 [gordo-helm](https://github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to deploy gordo infrastructure to your Kubernetes cluster. 
 
 ### Python package 
 
@@ -125,7 +127,16 @@
 > **_NOTE:_**  To run tests it's required for your system to has (note: commands might differ from your OS):
 > - Running docker daemon.
 > - Available 5432 port for `postgres` container.
 
 > **_NOTE:_** this example is for Pycharm IDE to use `breakpoints` in the code of the tests.  
 > On the configuration setup for test running add to `Additional arguments:` in `pytest` 
 > section following string: `--ignore benchmarks --cov-report= --no-cov ` 
+
+### Build the documentation
+
+This command will run the local documentation server:
+
+```console
+> cd docs/
+> make watch
+```
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.2 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.0.3 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-Extra:
-tests Provides-Extra: full License-File: LICENSE
+Extra: mlflow Provides-Extra: postgres Provides-Extra: tests Provides-Extra:
+full Provides-Extra: docs License-File: LICENSE
                               ****** Gordo ******
 
      Building thousands of models with timeseries data to monitor systems.
 
                                 [Build_Status]
 --- ## About Gordo fulfills the role of inhaling config files and supplying
 components to the pipeline of: 1. Fetching data 2. Training model 3. Serving
 model ## Components * [gordo-controller](https://github.com/equinor/gordo-
 controller/) - Kubernetes controller for the Gordo CRDs. * [gordo-core](https:/
 /github.com/equinor/gordo-core/) - Gordo core library. * [gordo-client](https:/
 /github.com/equinor/gordo-client/) - Gordo server's client. It can make
-predictions from deployed models. --- ## Install [gordo-helm](https://
+predictions from deployed models. [Documentation is available on Read the Docs]
+(https://gordo1.readthedocs.io/) --- ## Install [gordo-helm](https://
 github.com/equinor/gordo-helm) - you can use [gordo](https://github.com/
 equinor/gordo-helm/tree/main/charts/gordo) helm chart from this repository to
 deploy gordo infrastructure to your Kubernetes cluster. ### Python package `pip
 install --upgrade gordo` With additional extras: `pip install gordo
 [postgres,mlflow]` Bleeding edge: `pip install git+https://github.com/equinor/
 gordo.git` ## Developer manual This section will explain how to start
 development of Gordo. ### Setup Create and activate a virtual environment
@@ -42,8 +43,10 @@
 some time, so it's faster to run tests in parallel: ``` pytest -n auto -m 'not
 dockertest' --ignore benchmarks ``` Run docker-related tests: ``` pytest -
 m 'dockertest' ``` > **_NOTE:_** To run tests it's required for your system to
 has (note: commands might differ from your OS): > - Running docker daemon. > -
 Available 5432 port for `postgres` container. > **_NOTE:_** this example is for
 Pycharm IDE to use `breakpoints` in the code of the tests. > On the
 configuration setup for test running add to `Additional arguments:` in `pytest`
-> section following string: `--ignore benchmarks --cov-report= --no-cov `
+> section following string: `--ignore benchmarks --cov-report= --no-cov ` ###
+Build the documentation This command will run the local documentation server:
+```console > cd docs/ > make watch ```
```

### Comparing `gordo-5.0.2/gordo.egg-info/SOURCES.txt` & `gordo-5.0.3/gordo.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,40 +21,61 @@
 benchmarks/test_ml_server.py
 benchmarks/load_test/README.md
 benchmarks/load_test/load_test.py
 benchmarks/load_test/task_set.py.jinja2
 docs/Makefile
 docs/conf.py
 docs/index.rst
+docs/overview.rst
 docs/_static/Gordo_C4.README
 docs/_static/Gordo_C4.svg
 docs/_static/_placeholder.txt
+docs/_static/architecture_diagram.png
+docs/_static/architecture_diagram.py
+docs/_static/argo_logo.png
 docs/_static/endpoint-metadata.png
-docs/components/builder.rst
-docs/components/cli.rst
-docs/components/serializer.rst
-docs/components/util.rst
-docs/components/workflow.rst
-docs/components/machine/machine.rst
-docs/components/machine/metadata.rst
-docs/components/machine/validators.rst
-docs/components/machine/model/anomaly.rst
-docs/components/machine/model/model-factories.rst
-docs/components/machine/model/model.rst
-docs/components/machine/model/transformer-funcs.rst
-docs/components/machine/model/transformers.rst
-docs/components/server/anomaly.rst
-docs/components/server/base.rst
-docs/components/server/server.rst
-docs/general/architecture.rst
+docs/api/builder.rst
+docs/api/cli.rst
+docs/api/index.rst
+docs/api/reporters.rst
+docs/api/serializer.rst
+docs/api/util.rst
+docs/api/workflow.rst
+docs/api/machine/index.rst
+docs/api/machine/loader.rst
+docs/api/machine/machine.rst
+docs/api/machine/metadata.rst
+docs/api/machine/validators.rst
+docs/api/machine/model/anomaly.rst
+docs/api/machine/model/index.rst
+docs/api/machine/model/model-factories.rst
+docs/api/machine/model/model.rst
+docs/api/machine/model/register.rst
+docs/api/machine/model/transformer-funcs.rst
+docs/api/machine/model/transformers.rst
+docs/api/machine/model/utils.rst
+docs/api/server/anomaly.rst
+docs/api/server/base.rst
+docs/api/server/index.rst
+docs/api/server/prometheus.rst
+docs/api/server/properties.rst
+docs/api/server/server.rst
+docs/api/server/utils.rst
+docs/general/cli.rst
+docs/general/cluster_deployment.rst
 docs/general/endpoints.rst
-docs/general/quickstart.rst
+docs/general/index.rst
+docs/ml/index.rst
+docs/ml/model_configuration.rst
+docs/ml/model_output.rst
 examples/Gordo-Workflow-High-Level.ipynb
 examples/Pipelines-with-Gordo.ipynb
 examples/config.yaml
+examples/model-configuration.yaml
+examples/test-project.yaml
 gordo/__init__.py
 gordo/_version.py
 gordo/utils.py
 gordo.egg-info/PKG-INFO
 gordo.egg-info/SOURCES.txt
 gordo.egg-info/dependency_links.txt
 gordo.egg-info/entry_points.txt
```

### Comparing `gordo-5.0.2/gordo.egg-info/requires.txt` & `gordo-5.0.3/gordo.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 catboost~=1.1.1
 prometheus_client~=0.7
 packaging<22.0,>=21.0
 gordo-client==6.2.0
 gordo-core==0.3.0
 
 [docs]
-sphinx-rtd-theme~=0.4
-sphinxcontrib-websupport~=1.1
-sphinx~=2.1
-sphinx-click~=2.0
-pandas==1.1.4
+sphinx~=6.2
+sphinx-autobuild~=2021.3
+sphinx-copybutton~=0.5
+furo~=2023.5
+sphinx-click~=4.4
+ipython~=8.13
+mlflow~=2.3
+azureml-core~=1.49
+peewee~=3.14
+psycopg2-binary~=2.9
 
 [full]
 mlflow~=2.3
 azureml-core~=1.49
 peewee~=3.14
 psycopg2-binary~=2.9
```

### Comparing `gordo-5.0.2/pytest.ini` & `gordo-5.0.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/requirements/full_requirements.txt` & `gordo-5.0.3/requirements/full_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/requirements/test_requirements.txt` & `gordo-5.0.3/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json` & `gordo-5.0.3/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/resources/grafana/dashboards/machines.json` & `gordo-5.0.3/resources/grafana/dashboards/machines.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/run_workflow_and_argo.sh` & `gordo-5.0.3/run_workflow_and_argo.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/scripts/download_argo.py` & `gordo-5.0.3/scripts/download_argo.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/scripts/github_docker.py` & `gordo-5.0.3/scripts/github_docker.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/scripts/tests.sh` & `gordo-5.0.3/scripts/tests.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/scripts/trivy_scan.sh` & `gordo-5.0.3/scripts/trivy_scan.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/setup.py` & `gordo-5.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,21 @@
             r.strip()
             for r in f.readlines()
             if r.strip() and not r.startswith("#") and not r.startswith("-")
         ]
 
 
 extras_require = {
-    "docs": requirements("docs_requirements.in"),
     "mlflow": requirements("mlflow_requirements.in"),
     "postgres": requirements("postgres_requirements.in"),
     "tests": requirements("test_requirements.txt"),
 }
-extras_require["full"] = extras_require["mlflow"] + extras_require["postgres"]
+full_extras = extras_require["mlflow"] + extras_require["postgres"]
+extras_require["full"] = full_extras
+extras_require["docs"] = requirements("docs_requirements.in") + full_extras
 
 install_requires = requirements("requirements.in")  # Allow flexible deps for install
 
 # Read the docs have quite low memory limits on their build servers, so low
 # that pip crashes when downloading tensorflow. So we must remove it from the install
 # requirements, and set up autodoc_mock_imports in docs/conf.py
 if on_rtd:
```

### Comparing `gordo-5.0.2/tests/config-test.yaml` & `gordo-5.0.3/tests/config-test.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/conftest.py` & `gordo-5.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/builder/test_builder.py` & `gordo-5.0.3/tests/gordo/builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/builder/test_local_build.py` & `gordo-5.0.3/tests/gordo/builder/test_local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/builder/test_utils.py` & `gordo-5.0.3/tests/gordo/builder/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/cli/test_cli.py` & `gordo-5.0.3/tests/gordo/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/cli/test_exception_reporter.py` & `gordo-5.0.3/tests/gordo/cli/test_exception_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/client/test_client.py` & `gordo-5.0.3/tests/gordo/client/test_client.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/metadata/test_metadata.py` & `gordo-5.0.3/tests/gordo/machine/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py` & `gordo-5.0.3/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_factories_utils.py` & `gordo-5.0.3/tests/gordo/machine/model/test_factories_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_feedforward_autoencoder.py` & `gordo-5.0.3/tests/gordo/machine/model/test_feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_lstm_autoencoder.py` & `gordo-5.0.3/tests/gordo/machine/model/test_lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_model.py` & `gordo-5.0.3/tests/gordo/machine/model/test_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_raw_keras.py` & `gordo-5.0.3/tests/gordo/machine/model/test_raw_keras.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_register.py` & `gordo-5.0.3/tests/gordo/machine/model/test_register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_transformers.py` & `gordo-5.0.3/tests/gordo/machine/model/test_transformers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/model/test_utils.py` & `gordo-5.0.3/tests/gordo/machine/model/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/test_descriptors.py` & `gordo-5.0.3/tests/gordo/machine/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/test_loader.py` & `gordo-5.0.3/tests/gordo/machine/test_loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/machine/test_machine.py` & `gordo-5.0.3/tests/gordo/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/reporters/test_mlflow_reporter.py` & `gordo-5.0.3/tests/gordo/reporters/test_mlflow_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/reporters/test_postgres_reporter.py` & `gordo-5.0.3/tests/gordo/reporters/test_postgres_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/serializer/test_serializer_from_definition.py` & `gordo-5.0.3/tests/gordo/serializer/test_serializer_from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/serializer/test_serializer_into_definition.py` & `gordo-5.0.3/tests/gordo/serializer/test_serializer_into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/serializer/test_serializer_load_dump.py` & `gordo-5.0.3/tests/gordo/serializer/test_serializer_load_dump.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/server/test_anomaly_blueprint.py` & `gordo-5.0.3/tests/gordo/server/test_anomaly_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/server/test_base_blueprint.py` & `gordo-5.0.3/tests/gordo/server/test_base_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/server/test_gordo_server.py` & `gordo-5.0.3/tests/gordo/server/test_gordo_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/server/test_model_io.py` & `gordo-5.0.3/tests/gordo/server/test_model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/server/test_prometheus.py` & `gordo-5.0.3/tests/gordo/server/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/server/test_utils.py` & `gordo-5.0.3/tests/gordo/server/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/test_version.py` & `gordo-5.0.3/tests/gordo/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/util/test_disk_registry.py` & `gordo-5.0.3/tests/gordo/util/test_disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/util/test_version.py` & `gordo-5.0.3/tests/gordo/util/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_config_elements.py` & `gordo-5.0.3/tests/gordo/workflow/test_config_elements.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_helpers.py` & `gordo-5.0.3/tests/gordo/workflow/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_normalized_config.py` & `gordo-5.0.3/tests/gordo/workflow/test_normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py` & `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/test_examples.py` & `gordo-5.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.2/tests/utils.py` & `gordo-5.0.3/tests/utils.py`

 * *Files identical despite different names*

