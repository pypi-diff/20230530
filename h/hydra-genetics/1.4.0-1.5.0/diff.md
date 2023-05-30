# Comparing `tmp/hydra-genetics-1.4.0.tar.gz` & `tmp/hydra-genetics-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-genetics-1.4.0.tar", last modified: Tue May 16 09:56:44 2023, max compression
+gzip compressed data, was "hydra-genetics-1.5.0.tar", last modified: Tue May 30 14:38:31 2023, max compression
```

## Comparing `hydra-genetics-1.4.0.tar` & `hydra-genetics-1.5.0.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.694573 hydra-genetics-1.4.0/hydra_genetics/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/commands/prep_pipeline_env.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.698573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.698573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.698573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.690573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/output_files.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/output_files.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/units.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/images/
--rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/images/hydragenetics.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/rule-template/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/skeleton_rule.smk
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/chr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/multibp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/models/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.694573 hydra-genetics-1.4.0/hydra_genetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/io/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/io/test_mutations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/models/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/prep_pipeline_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.700339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/output_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/units.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/images/hydragenetics.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/rule-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/skeleton_rule.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/chr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/multibp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/models/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/io/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/io/test_mutations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/models/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/versioneer.py
```

### Comparing `hydra-genetics-1.4.0/LICENSE.md` & `hydra-genetics-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/PKG-INFO` & `hydra-genetics-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.4.0
+Version: 1.5.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.4.0/README.md` & `hydra-genetics-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/__init__.py` & `hydra-genetics-1.5.0/hydra_genetics/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/__main__.py` & `hydra-genetics-1.5.0/hydra_genetics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import logging
 import os
 import re
 import sys
 
 import hydra_genetics.utils
 from hydra_genetics.commands.prep_pipeline_env import environment
+from hydra_genetics.commands.references import references
 from hydra_genetics.commands.create import PipelineCreate, RuleCreate, CreateInputFiles
 import rich.console
 import rich.logging
 import rich.traceback
 
+
 # Set up logging as the root logger
 # Submodules should all traverse back to this
 log = logging.getLogger()
 
 
 def rich_force_colors():
     """
@@ -43,27 +45,36 @@
                  highlight=False)
     stderr.print("\u001b[36m hydra-core/tools version {}\033[0m\n\n".format(hydra_genetics.__version__), highlight=False)
 
     cli()
 
 
 @click.group(help="CLI tool to prepare and initialize snakemake projects")
-@click.option("-v", "--verbose", is_flag=True, default=False, help="Print verbose output to the console.")
+@click.option("--verbose", is_flag=True, default=False, help="Print verbose output to the console.")
 @click.option("-l", "--log-file", help="Save a verbose log to a file.", metavar="<filename>")
-def cli(verbose, log_file):
-    log.setLevel(logging.DEBUG)
-
+@click.option('--debug/--no-debug', default=False)
+def cli(verbose, log_file, debug):
+    loglevel = logging.WARNING
+    if debug:
+        loglevel = logging.DEBUG
+    elif verbose:
+        loglevel = logging.INFO
+
+    logging.basicConfig(level=loglevel)
+    log.setLevel(loglevel)
+    log.handlers.clear()
     log.addHandler(
         rich.logging.RichHandler(
-            level=logging.DEBUG if verbose else logging.INFO,
+            level=loglevel,
             console=rich.console.Console(stderr=True, force_terminal=rich_force_colors()),
             show_time=False,
             markup=True,
         )
     )
+    log.propagate = False
 
     if log_file:
         log_fh = logging.FileHandler(log_file, encoding="utf-8")
         log_fh.setLevel(logging.DEBUG)
         log_fh.setFormatter(logging.Formatter("[%(asctime)s] %(name)-20s [%(levelname)-7s]  %(message)s"))
         log.addHandler(log_fh)
 
@@ -257,16 +268,13 @@
                        sample_regex, read_number_regex, adapters, tc, force, default_barcode, validate, ask, th, nreads, every):
     input_files = CreateInputFiles(directory, outdir, post_file_modifier, platform, sample_type,
                                    sample_regex, read_number_regex, adapters, tc, force, default_barcode, validate, ask, th,
                                    nreads, every)
     input_files.init()
 
 
-#  @cli.command(short_help="download reference data")
-#  def referece_data():
-#    pass
-
+cli.add_command(references)
 
 cli.add_command(environment)
 
 if __name__ == "__main__":
     run()
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/commands/create.py` & `hydra-genetics-1.5.0/hydra_genetics/commands/create.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/commands/prep_pipeline_env.py` & `hydra-genetics-1.5.0/hydra_genetics/commands/prep_pipeline_env.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Controls when the action will run.
 on:
    # Triggers the workflow on push or pull request events but only for the master and develop branch
   push:
     branches:
      - develop
-     - master
+     - main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   integration-small-singularity:
     name: integration small data set singularity
@@ -42,8 +42,8 @@
           mamba install -c conda-forge -c bioconda singularity=3.8.6
       - name: Add conda to system path
         run: |
           echo $CONDA/bin >> $GITHUB_PATH
       - name: Integration test - small dataset
         working-directory: .tests/integration
         run: |
-          snakemake -s ../../workflow/Snakefile -j 1 --show-failed-logs --configfile config/config.yaml  --use-singularity --singularity-args  " --cleanenv --bind /home/runner "
+          snakemake -s ../../workflow/Snakefile -j 1 --show-failed-logs --configfiles ../../config/config.yaml config/config.yaml  --use-singularity --singularity-args  " --cleanenv --bind /home/runner "
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-name: Lint
+name: pytest
 
 # Controls when the action will run.
 on:
    # Triggers the workflow on push or pull request events but only for the master and develop branch
   push:
     branches:
      - develop
-     - master
+     - main
   pull_request:
     branches:
      - develop
-     - master
+     - main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
-  lint:
-    name: Lint workflow
+  pytest:
+    name: pytest
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v2
       - name: Set up Python 3.8
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v2
         with:
           python-version: 3.8
       - name: Install requirements.txt
         run: |
           pip install -r requirements.txt
-      - name: Linting
-        working-directory: .tests/integration
+      - name: Install requirements.test.txt
         run: |
-          snakemake --lint -n -s ../../workflow/Snakefile --configfile config.yaml"
+          pip install -r requirements.test.txt
+      - name: pytest
+        run: pytest workflow/scripts
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 # Controls when the action will run.
 on:
    # Triggers the workflow on push or pull request events but only for the master and develop branch
   push:
     branches:
      - develop
-     - master
+     - main
   pull_request:
     branches:
      - develop
-     - master
+     - main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   pycodestyle:
     name: pycodestyle
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-name: pytest
+name: Lint
 
 # Controls when the action will run.
 on:
    # Triggers the workflow on push or pull request events but only for the master and develop branch
   push:
     branches:
      - develop
-     - master
+     - main
   pull_request:
     branches:
      - develop
-     - master
+     - main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
-  pytest:
-    name: pytest
+  lint:
+    name: Lint workflow
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python 3.8
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v3
         with:
           python-version: 3.8
       - name: Install requirements.txt
         run: |
           pip install -r requirements.txt
-      - name: Install requirements.test.txt
+      - name: Linting
+        working-directory: .tests/integration
         run: |
-          pip install -r requirements.test.txt
-      - name: pytest
-        run: pytest workflow/scripts
+          snakemake --lint -n -s ../../workflow/Snakefile --configfiles ../../config/config.yaml config/config.yaml"
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 # Controls when the action will run.
 on:
    # Triggers the workflow on push or pull request events but only for the master and develop branch
   push:
     branches:
      - develop
-     - master
+     - main
   pull_request:
     branches:
      - develop
-     - master
+     - main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   snakefmt:
     name: Snakefmt
@@ -26,8 +26,9 @@
           fetch-depth: 0
       - name: Lint Code Base
         uses: github/super-linter@v4.9.0
         env:
           VALIDATE_ALL_CODEBASE: false
           GITHUB_TOKEN: {{ '${{' }} secrets.GITHUB_TOKEN {{'}}'}}
           VALIDATE_SNAKEMAKE_SNAKEFMT: true
+          DEFAULT_BRANCH: main
           OUTPUT_FOLDER: .github/linters/report
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 # Controls when the action will run.
 on:
    # Triggers the workflow on push or pull request events but only for the master and develop branch
   push:
     branches:
      - develop
-     - master
+     - main
   pull_request:
     branches:
      - develop
-     - master
+     - main
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   snakemake-dry-run:
     name: Run snakemake dry run
@@ -30,8 +30,8 @@
           pip install -r requirements.txt
       - name: Install requirements.test.txt
         run: |
           pip install -r requirements.test.txt
       - name: snakemake dry run
         working-directory: .tests/integration
         run: |
-          snakemake -n -s ../../workflow/Snakefile --configfiles config.yaml
+          snakemake -n -s ../../workflow/Snakefile --configfiles ../../config/config.yaml config/config.yaml
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/LICENSE.md` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/README.md` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # <img src="images/hydragenetics.png" width=40 /> hydra-genetics/{{ short_name }}
 
 #### {{ description }}
 
 ![Lint](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/lint.yaml/badge.svg?branch=develop)
 ![Snakefmt](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/snakefmt.yaml/badge.svg?branch=develop)
 ![snakemake dry run](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/snakemake-dry-run.yaml/badge.svg?branch=develop)
-![integration test](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/integration1.yaml/badge.svg?branch=develop)
+![integration test](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/integration.yaml/badge.svg?branch=develop)
 
-![pycodestyle](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/pycodestyl.yaml/badge.svg?branch=develop)
+![pycodestyle](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/pycodestyle.yaml/badge.svg?branch=develop)
 ![pytest](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/pytest.yaml/badge.svg?branch=develop)
 
 [![License: GPL-3](https://img.shields.io/badge/License-GPL3-yellow.svg)](https://opensource.org/licenses/gpl-3.0.html)
 
 ## :speech_balloon: Introduction
 
 The module consists of alignment  ....
 
 ## :heavy_exclamation_mark: Dependencies
 
 In order to use this module, the following dependencies are required:
 
-[![hydra-genetics](https://img.shields.io/badge/hydragenetics-v0.9.1-blue)](https://github.com/hydra-genetics/)
+[![hydra-genetics](https://img.shields.io/badge/hydragenetics-v1.3.0-blue)](https://github.com/hydra-genetics/)
 [![pandas](https://img.shields.io/badge/pandas-1.3.1-blue)](https://pandas.pydata.org/)
 [![python](https://img.shields.io/badge/python-3.8-blue)
 [![snakemake](https://img.shields.io/badge/snakemake-{{ min_snakemake_version }}-blue)](https://snakemake.readthedocs.io/en/stable/)
 [![singularity](https://img.shields.io/badge/singularity-3.0.0-blue)](https://sylabs.io/docs/)
 
 ## :school_satchel: Preparations
 
@@ -51,17 +51,17 @@
 
 ## :white_check_mark: Testing
 
 The workflow repository contains a small test dataset `.tests/integration` which can be run like so:
 
 ```bash
 $ cd .tests/integration
-$ snakemake -s ../../Snakefile -j1 --use-singularity
+$ snakemake -s ../../Snakefile --configfiles ../../config/config.yaml config/config.yaml -j1 --use-singularity
 ```
-
+`../../config/config.yaml` is the original config-file, while `config/config.yaml` is the test config. By defining two config-files the latter overwrites any overlapping variables in the first config-file.
 ## :rocket: Usage
 
 To use this module in your workflow, follow the description in the
 [snakemake docs](https://snakemake.readthedocs.io/en/stable/snakefiles/modularization.html#modules).
 Add the module to your `Snakefile` like so:
 
 ```bash
@@ -84,7 +84,8 @@
 The following output files should be targeted via another rule:
 
 | File | Description |
 |---|---|
 | `{{ short_name }}/PATH/FILE` | DESCRIPTION |
 
 ## :judge: Rule Graph
+![rule_graph_reference](images/rulegraph.svg)
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/extra.css` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/extra.css`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/index.md` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/images/hydragenetics.png` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/images/hydragenetics.png`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/mkdocs.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/rules/common.smk` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/rules/common.smk`

 * *Files 21% similar despite different names*

```diff
@@ -16,18 +16,35 @@
 from hydra_genetics.utils.units import *
 
 min_version("{{ min_snakemake_version }}")
 
 ### Set and validate config file
 
 if not workflow.overwrite_configfiles:
-    "At least one config file must be passed using --configfile/--configfiles, by command line or a profile!"
+    sys.exit("At least one config file must be passed using --configfile/--configfiles, by command line or a profile!")
 
+try:
+    validate(config, schema="../schemas/config.schema.yaml")
+except WorkflowError as we:
+    # Probably a validation error, but the original exception in lost in
+    # snakemake. Pull out the most relevant information instead of a potentially
+    # *very* long error message.
+    if not we.args[0].lower().startswith("error validating config file"):
+        raise
+    error_msg = "\n".join(we.args[0].splitlines()[:2])
+    parent_rule_ = we.args[0].splitlines()[3].split()[-1]
+    if parent_rule_ == "schema:":
+        sys.exit(error_msg)
+    else:
+        schema_hiearachy = parent_rule_.split()[-1]
+        schema_section = ".".join(re.findall(r"\['([^']+)'\]", schema_hiearachy)[1::2])
+        sys.exit(f"{error_msg} in {schema_section}")
+
+### Read and validate resources file
 
-validate(config, schema="../schemas/config.schema.yaml")
 config = load_resources(config, config["resources"])
 validate(config, schema="../schemas/resources.schema.yaml")
 
 
 ### Read and validate samples file
 
 samples = pd.read_table(config["samples"], dtype=str).set_index("sample", drop=False)
@@ -39,14 +56,16 @@
     pandas.read_table(config["units"], dtype=str)
     .set_index(["sample", "type", "flowcell", "lane", "barcode"], drop=False)
     .sort_index()
 )
 
 validate(units, schema="../schemas/units.schema.yaml")
 
+### Read and validate output file
+
 with open(config["output"]) as output:
     if config["output"].endswith("json"):
         output_spec = json.load(output)
     elif config["output"].endswith("yaml") or config["output"].endswith("yml"):
         output_spec = yaml.safe_load(output.read())
 
 validate(output_spec, schema="../schemas/output_files.schema.yaml")
@@ -83,15 +102,15 @@
     output_directory = pathlib.Path(output_spec.get("directory", "./"))
     rulestrings = []
 
     for f in output_spec["files"]:
         if f["input"] is None:
             continue
 
-        rule_name = "_copy_{}".format("_".join(re.split(r"\W+", f["name"].strip().lower())))
+        rule_name = "_copy_{}".format("_".join(re.split(r"\W{1,}", f["name"].strip().lower())))
         input_file = pathlib.Path(f["input"])
         output_file = output_directory / pathlib.Path(f["output"])
 
         mem_mb = config.get("_copy", {}).get("mem_mb", config["default_resources"]["mem_mb"])
         mem_per_cpu = config.get("_copy", {}).get("mem_per_cpu", config["default_resources"]["mem_per_cpu"])
         partition = config.get("_copy", {}).get("partition", config["default_resources"]["partition"])
         threads = config.get("_copy", {}).get("threads", config["default_resources"]["threads"])
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/rule-template/config.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/rule-template/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/rule-template/resources.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/rule-template/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/rule-template/rules.schema.yaml` & `hydra-genetics-1.5.0/hydra_genetics/rule-template/rules.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/rule-template/skeleton_rule.smk` & `hydra-genetics-1.5.0/hydra_genetics/rule-template/skeleton_rule.smk`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/io/chr.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/io/chr.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot_report.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/io/multibp.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/io/multibp.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/io/utils.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/io/utils.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/misc.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/models/hotspot.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/models/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/samples.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics/utils/units.py` & `hydra-genetics-1.5.0/hydra_genetics/utils/units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/hydra_genetics.egg-info/PKG-INFO` & `hydra-genetics-1.5.0/hydra_genetics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.4.0
+Version: 1.5.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.4.0/hydra_genetics.egg-info/SOURCES.txt` & `hydra-genetics-1.5.0/hydra_genetics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 hydra_genetics.egg-info/entry_points.txt
 hydra_genetics.egg-info/not-zip-safe
 hydra_genetics.egg-info/requires.txt
 hydra_genetics.egg-info/top_level.txt
 hydra_genetics/commands/__init__.py
 hydra_genetics/commands/create.py
 hydra_genetics/commands/prep_pipeline_env.py
+hydra_genetics/commands/references.py
 hydra_genetics/pipeline-template/.gitignore
 hydra_genetics/pipeline-template/.readthedocs.yaml
 hydra_genetics/pipeline-template/LICENSE.md
 hydra_genetics/pipeline-template/README.md
 hydra_genetics/pipeline-template/mkdocs.yaml
 hydra_genetics/pipeline-template/requirements.test.txt
 hydra_genetics/pipeline-template/requirements.txt
@@ -38,15 +39,14 @@
 hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
 hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
 hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
 hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
 hydra_genetics/pipeline-template/.tests/integration/samples.tsv
 hydra_genetics/pipeline-template/.tests/integration/units.tsv
 hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
-hydra_genetics/pipeline-template/.tests/integration/config/output_files.yaml
 hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
 hydra_genetics/pipeline-template/config/config.yaml
 hydra_genetics/pipeline-template/config/output_files.yaml
 hydra_genetics/pipeline-template/config/resources.yaml
 hydra_genetics/pipeline-template/config/samples.tsv
 hydra_genetics/pipeline-template/config/units.tsv
 hydra_genetics/pipeline-template/docs/extra.css
@@ -79,14 +79,15 @@
 hydra_genetics/utils/units.py
 hydra_genetics/utils/io/__init__.py
 hydra_genetics/utils/io/chr.py
 hydra_genetics/utils/io/hotspot.py
 hydra_genetics/utils/io/hotspot_report.py
 hydra_genetics/utils/io/multibp.py
 hydra_genetics/utils/io/readers.py
+hydra_genetics/utils/io/reference.py
 hydra_genetics/utils/io/utils.py
 hydra_genetics/utils/models/__init__.py
 hydra_genetics/utils/models/hotspot.py
 tests/__init__.py
 tests/utils/__init__.py
 tests/utils/test_misc.py
 tests/utils/test_resources.py
```

### Comparing `hydra-genetics-1.4.0/setup.py` & `hydra-genetics-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/io/test_hotspot.py` & `hydra-genetics-1.5.0/tests/utils/io/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/io/test_mutations_report.py` & `hydra-genetics-1.5.0/tests/utils/io/test_mutations_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/models/test_hotspot.py` & `hydra-genetics-1.5.0/tests/utils/models/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/test_misc.py` & `hydra-genetics-1.5.0/tests/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/test_resources.py` & `hydra-genetics-1.5.0/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/test_samples.py` & `hydra-genetics-1.5.0/tests/utils/test_samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/tests/utils/test_units.py` & `hydra-genetics-1.5.0/tests/utils/test_units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.4.0/versioneer.py` & `hydra-genetics-1.5.0/versioneer.py`

 * *Files identical despite different names*

