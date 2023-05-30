# Comparing `tmp/gene-ranking-shootout-0.1.2.tar.gz` & `tmp/gene-ranking-shootout-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene-ranking-shootout-0.1.2.tar", last modified: Fri May  5 13:09:20 2023, max compression
+gzip compressed data, was "gene-ranking-shootout-0.1.3.tar", last modified: Tue May 30 10:30:26 2023, max compression
```

## Comparing `gene-ranking-shootout-0.1.2.tar` & `gene-ranking-shootout-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.013414 gene-ranking-shootout-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.017414 gene-ranking-shootout-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.017414 gene-ranking-shootout-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.github/workflows/release-please.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.013414 gene-ranking-shootout-0.1.2/docker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.017414 gene-ranking-shootout-0.1.2/docker/cada/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/docker/cada/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/docker/cada/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.021414 gene-ranking-shootout-0.1.2/gene_ranking_shootout/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.021414 gene-ranking-shootout-0.1.2/gene_ranking_shootout/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.025414 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1439512 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_all_cases.json
--rw-r--r--   0 runner    (1001) docker     (123)   292840 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_cases_test.json
--rw-r--r--   0 runner    (1001) docker     (123)   871083 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_cases_train.json
--rw-r--r--   0 runner    (1001) docker     (123)   286957 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_cases_validate.json
--rw-r--r--   0 runner    (1001) docker     (123)   758682 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_clinvar_cases.json
--rw-r--r--   0 runner    (1001) docker     (123)   680832 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_collaborator_cases.json
--rw-r--r--   0 runner    (1001) docker     (123)  1546549 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/gnomad_counts.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.021414 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-05 13:09:19.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 13:09:20.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:09:19.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 13:09:19.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:09:19.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 13:09:19.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 13:09:19.000000 gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.017414 gene-ranking-shootout-0.1.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/tests/data/amelie/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/amelie/query.json
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/amelie/response.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/tests/data/cada/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/cada/query.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/cada/result.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:09:20.029414 gene-ranking-shootout-0.1.2/tests/data/phen2gene/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/phen2gene/genes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/phen2gene/output_file.associated_gene_list
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/data/phen2gene/terms.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 13:09:13.000000 gene-ranking-shootout-0.1.2/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.147379 gene-ranking-shootout-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.151379 gene-ranking-shootout-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.151379 gene-ranking-shootout-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.github/workflows/automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.147379 gene-ranking-shootout-0.1.3/docker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.151379 gene-ranking-shootout-0.1.3/docker/cada/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/docker/cada/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/docker/cada/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.151379 gene-ranking-shootout-0.1.3/gene_ranking_shootout/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.151379 gene-ranking-shootout-0.1.3/gene_ranking_shootout/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.155379 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1439512 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_all_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)   292840 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_cases_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)   871083 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_cases_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)   286957 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_cases_validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)   758682 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_clinvar_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)   680832 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_collaborator_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1546549 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/gnomad_counts.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.151379 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 10:30:26.000000 gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.147379 gene-ranking-shootout-0.1.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/tests/data/amelie/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/amelie/query.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/amelie/response.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/tests/data/cada/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/cada/query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/cada/result.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:30:26.159379 gene-ranking-shootout-0.1.3/tests/data/phen2gene/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/phen2gene/genes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/phen2gene/output_file.associated_gene_list
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/data/phen2gene/terms.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 10:30:17.000000 gene-ranking-shootout-0.1.3/tests/test_example.py
```

### Comparing `gene-ranking-shootout-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `gene-ranking-shootout-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/.github/workflows/main.yml` & `gene-ranking-shootout-0.1.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/.github/workflows/release-please.yml` & `gene-ranking-shootout-0.1.3/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/.gitignore` & `gene-ranking-shootout-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/CHANGELOG.md` & `gene-ranking-shootout-0.1.3/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+### [0.1.3](https://www.github.com/bihealth/gene-ranking-shootout/compare/v0.1.2...v0.1.3) (2023-05-30)
+
+
+### Bug Fixes
+
+* filter CADA results to candidate gene IDs ([#22](https://www.github.com/bihealth/gene-ranking-shootout/issues/22)) ([#23](https://www.github.com/bihealth/gene-ranking-shootout/issues/23)) ([eb65c72](https://www.github.com/bihealth/gene-ranking-shootout/commit/eb65c72f22ee8fc0632e6e5416edfacf58736482))
+
+
+### Documentation
+
+* adding new methods to README ([#18](https://www.github.com/bihealth/gene-ranking-shootout/issues/18)) ([8e5c82d](https://www.github.com/bihealth/gene-ranking-shootout/commit/8e5c82dfae243ef7f4ecf2aea4cf2e1b0ad9964f))
+* Update README.md with details on 'benchmark summarize' output ([#21](https://www.github.com/bihealth/gene-ranking-shootout/issues/21)) ([3904c92](https://www.github.com/bihealth/gene-ranking-shootout/commit/3904c92349f4f1a84af3d28c6cdb0a35cbde6b25))
+
 ### [0.1.2](https://www.github.com/bihealth/gene-ranking-shootout/compare/v0.1.1...v0.1.2) (2023-05-05)
 
 
 ### Documentation
 
 * fixing README in setup.cfg, adding PyPi badges ([#15](https://www.github.com/bihealth/gene-ranking-shootout/issues/15)) ([16d4f32](https://www.github.com/bihealth/gene-ranking-shootout/commit/16d4f32b94195a85df06ad6bddb85a6381c33bfe))
```

### Comparing `gene-ranking-shootout-0.1.2/LICENSE` & `gene-ranking-shootout-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/Makefile` & `gene-ranking-shootout-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/PKG-INFO` & `gene-ranking-shootout-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-ranking-shootout
-Version: 0.1.2
+Version: 0.1.3
 Summary: Compare gene ranking methods.
 Home-page: https://github.com/bihealth/gene-ranking-shootout
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 Keywords: genes,ranking
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -21,29 +21,33 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 [![CI](https://github.com/bihealth/gene-ranking-shootout/actions/workflows/main.yml/badge.svg)](https://github.com/bihealth/gene-ranking-shootout/actions/workflows/main.yml)
-[![Pypi Package Version](https://img.shields.io/pypi/v/gene-ranking-shootout.svg)](https://pypi.org/v/gene-ranking-shootout)
+[![Pypi Package Version](https://img.shields.io/pypi/v/gene-ranking-shootout.svg)](https://pypi.org/project/gene-ranking-shootout)
 [![Pypi Python Version](https://img.shields.io/pypi/pyversions/gene-ranking-shootout.svg)](https://pypi.org/project/gene-ranking-shootout)
 
 # Gene Ranking Shootout
 
 A benchmark for methods that rank genes according to their relevance for a given phenotype (list of HPO terms).
 
 ## Methods
 
 The following methods are currently included in the benchmark:
 
 - AMELIE (via web service)
 - CADA (via custom Docker/Podman image)
 - Phen2Gene (via official Docker/Podman image)
 - Phenix algorithm (as implemented in VarFish)
+- Exomiser Algorithms:
+  - Phenix
+  - Phive
+  - HiPhive (variants: human only, human-mouse only, all human-mouse-fish-ppi)
 
 ## Installation
 
 Simply install with `pip` (probably inside a conda environment or virtualenv):
 
 ```bash
 $ git clone https://github.com/bihealth/gene-ranking-shootout.git
@@ -115,15 +119,15 @@
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ phenix /tmp/cases.json /tmp/result-exomiser-phenix.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ phive /tmp/cases.json /tmp/result-exomiser-phive.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive /tmp/cases.json /tmp/result-exomiser-hiphive.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive-mouse /tmp/cases.json /tmp/result-exomiser-hiphive-mouse.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive-human /tmp/cases.json /tmp/result-exomiser-hiphive-human.json
 ```
 
-You can also visualize the details of the benchmark results for each result file (below for 100 cases).
+You can also visualize the details of the benchmark results for each result file (below for 100 cases). This visualization displays the number of true disease genes (from case set definitions) at TOP10 and following positions in the ranked gene list of the respective method.
 
 ```bash
 $ gene-ranking-shootout benchmark summarize /tmp/result-amelie.json
     1:   48  ################################
     2:   17  ###########
     3:    7  ####
     4:    3  ##
@@ -214,36 +218,36 @@
 ## Some Preliminary Results
 
 The following was generated on 2023/05/05 with all 4714 cases.
 
 ```
 $ for f in /tmp/result-*.json; do (set -x; gene-ranking-shootout benchmark summarize --bars-top-n 20 $f); echo; done
 + gene-ranking-shootout benchmark summarize --bars-top-n 20 result-cada.json
-    1: 1340  ##################
-    2:  290  ####
-    3:  192  ##
-    4:  164  ##
-    5:   96  #
-    6:   84  #
-    7:   94  #
-    8:   59  .
-    9:   63  .
-   10:   40  .
-   11:   62  .
-   12:   47  .
-   13:   33  .
-   14:   43  .
-   15:   38  .
-   16:   42  .
-   17:   36  .
-   18:   16  .
-   19:   30  .
-   20:   22  .
+    1: 3462  ################################################
+    2:  536  #######
+    3:  205  ##
+    4:  133  #
+    5:   71  .
+    6:   57  .
+    7:   39  .
+    8:   47  .
+    9:   16  .
+   10:   24  .
+   11:   14  .
+   12:   22  .
+   13:   14  .
+   14:   11  .
+   15:    7  .
+   16:    9  .
+   17:    8  .
+   18:    4  .
+   19:    3  .
+   20:    3  .
 
-21-..: 1923  ##########################
+21-..:   29  .
 mssng:    0  
 
 + gene-ranking-shootout benchmark summarize --bars-top-n 20 result-exomiser-hiphive-human.json
     1: 2593  ####################################
     2:  637  ########
     3:  375  #####
     4:  203  ##
```

### Comparing `gene-ranking-shootout-0.1.2/README.md` & `gene-ranking-shootout-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [![CI](https://github.com/bihealth/gene-ranking-shootout/actions/workflows/main.yml/badge.svg)](https://github.com/bihealth/gene-ranking-shootout/actions/workflows/main.yml)
-[![Pypi Package Version](https://img.shields.io/pypi/v/gene-ranking-shootout.svg)](https://pypi.org/v/gene-ranking-shootout)
+[![Pypi Package Version](https://img.shields.io/pypi/v/gene-ranking-shootout.svg)](https://pypi.org/project/gene-ranking-shootout)
 [![Pypi Python Version](https://img.shields.io/pypi/pyversions/gene-ranking-shootout.svg)](https://pypi.org/project/gene-ranking-shootout)
 
 # Gene Ranking Shootout
 
 A benchmark for methods that rank genes according to their relevance for a given phenotype (list of HPO terms).
 
 ## Methods
 
 The following methods are currently included in the benchmark:
 
 - AMELIE (via web service)
 - CADA (via custom Docker/Podman image)
 - Phen2Gene (via official Docker/Podman image)
 - Phenix algorithm (as implemented in VarFish)
+- Exomiser Algorithms:
+  - Phenix
+  - Phive
+  - HiPhive (variants: human only, human-mouse only, all human-mouse-fish-ppi)
 
 ## Installation
 
 Simply install with `pip` (probably inside a conda environment or virtualenv):
 
 ```bash
 $ git clone https://github.com/bihealth/gene-ranking-shootout.git
@@ -89,15 +93,15 @@
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ phenix /tmp/cases.json /tmp/result-exomiser-phenix.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ phive /tmp/cases.json /tmp/result-exomiser-phive.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive /tmp/cases.json /tmp/result-exomiser-hiphive.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive-mouse /tmp/cases.json /tmp/result-exomiser-hiphive-mouse.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive-human /tmp/cases.json /tmp/result-exomiser-hiphive-human.json
 ```
 
-You can also visualize the details of the benchmark results for each result file (below for 100 cases).
+You can also visualize the details of the benchmark results for each result file (below for 100 cases). This visualization displays the number of true disease genes (from case set definitions) at TOP10 and following positions in the ranked gene list of the respective method.
 
 ```bash
 $ gene-ranking-shootout benchmark summarize /tmp/result-amelie.json
     1:   48  ################################
     2:   17  ###########
     3:    7  ####
     4:    3  ##
@@ -188,36 +192,36 @@
 ## Some Preliminary Results
 
 The following was generated on 2023/05/05 with all 4714 cases.
 
 ```
 $ for f in /tmp/result-*.json; do (set -x; gene-ranking-shootout benchmark summarize --bars-top-n 20 $f); echo; done
 + gene-ranking-shootout benchmark summarize --bars-top-n 20 result-cada.json
-    1: 1340  ##################
-    2:  290  ####
-    3:  192  ##
-    4:  164  ##
-    5:   96  #
-    6:   84  #
-    7:   94  #
-    8:   59  .
-    9:   63  .
-   10:   40  .
-   11:   62  .
-   12:   47  .
-   13:   33  .
-   14:   43  .
-   15:   38  .
-   16:   42  .
-   17:   36  .
-   18:   16  .
-   19:   30  .
-   20:   22  .
+    1: 3462  ################################################
+    2:  536  #######
+    3:  205  ##
+    4:  133  #
+    5:   71  .
+    6:   57  .
+    7:   39  .
+    8:   47  .
+    9:   16  .
+   10:   24  .
+   11:   14  .
+   12:   22  .
+   13:   14  .
+   14:   11  .
+   15:    7  .
+   16:    9  .
+   17:    8  .
+   18:    4  .
+   19:    3  .
+   20:    3  .
 
-21-..: 1923  ##########################
+21-..:   29  .
 mssng:    0  
 
 + gene-ranking-shootout benchmark summarize --bars-top-n 20 result-exomiser-hiphive-human.json
     1: 2593  ####################################
     2:  637  ########
     3:  375  #####
     4:  203  ##
```

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/cli/__init__.py` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,19 +79,20 @@
         simulated_json, results_json
     )
 
 
 @benchmark.command()
 @click.option("--bars-top-n", default=10)
 @click.option("--total-width", default=80)
+@click.option("--threads", default=0)
 @click.argument("simulated_json")
 @click.argument("results_json")
-def cada(simulated_json, results_json, bars_top_n, total_width):
+def cada(simulated_json, results_json, bars_top_n, total_width, threads):
     """Benchmark the CADA container."""
-    runner.CadaRunner(bars_top_n=bars_top_n, total_width=total_width).run(
+    runner.CadaRunner(bars_top_n=bars_top_n, total_width=total_width, threads=threads).run(
         simulated_json, results_json
     )
 
 
 @benchmark.command()
 @click.option("--bars-top-n", default=10)
 @click.option("--total-width", default=80)
```

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_all_cases.json` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_all_cases.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_cases_test.json` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_cases_test.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_cases_train.json` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_cases_train.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_cases_validate.json` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_cases_validate.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_clinvar_cases.json` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_clinvar_cases.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/cada_collaborator_cases.json` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/cada_collaborator_cases.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/data/gnomad_counts.tsv` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/data/gnomad_counts.tsv`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/models.py` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/models.py`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout/runner.py` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code for running the benchmark."""
 
 from collections import Counter
 import csv
 import json
+import multiprocessing
 import subprocess
 import sys
 import tempfile
 import typing
 
 import cattrs
 from loguru import logger
@@ -59,19 +60,21 @@
         bar = gen_bar(missing)
         print(f"mssng: {missing:>4}  {bar}", file=self.outf)
 
 
 class BaseRunner:
     """Base class for the runners."""
 
-    def __init__(self, *, total_width=80, bars_top_n=10):
+    def __init__(self, *, total_width=80, bars_top_n=10, threads=0):
         #: The total display width.
         self.total_width = total_width
         #: The number of top genes to print bars for.
         self.bars_top_n = bars_top_n
+        #: The number of threads to use.
+        self.threads = threads
 
         logger.info("Loading data ...")
         #: The gnomAD counts.
         self.gnomad_data = models.load_gnomad_counts()
         #: Mapping from Entrez gene ID to gene symbol.
         self.entrez_to_symbol = {gene.entrez_id: gene.gene_symbol for gene in self.gnomad_data}
         #: Mapping from gene symbol to Entrez gene ID.
@@ -81,30 +84,46 @@
     def run(self, path_simulated_json: str, path_results_json: str):
         """Run the benchmark."""
         logger.info("Loading cases ...")
         cases = models.load_cases_json(path_simulated_json)
         logger.info("... done loading {} cases", len(cases))
 
         logger.info("Running benchmark ...")
-        results = []
-        for case in tqdm.tqdm(cases):
-            result = self.run_ranking(case)
-            if result is not None:
-                results.append(result)
+        if self.threads:
+            with multiprocessing.Pool(self.threads) as pool:
+                results = [x for x in tqdm.tqdm(pool.imap(self._run, cases), total=len(cases)) if x]
+        else:
+            results = []
+            for case in tqdm.tqdm(cases):
+                result = self.run_ranking(case)
+                if result is not None:
+                    results.append(result)
         logger.info("... done running benchmark")
 
         logger.info("Writing results ...")
         with open(path_results_json, "wt") as outf:
             json.dump(cattrs.unstructure(results), outf, indent=2)
         logger.info("... done writing results")
 
         logger.info("Displaying results overview ...")
         self.print_bars(results)
         logger.info("All done. Have a nice day!")
 
+    def _run(self, case: models.Case) -> typing.Optional[models.Result]:
+        """Run the ranking for the given case.
+
+        :param case: The case to run the ranking for.
+        :returns: result for the case or ``None`` if no result was found.
+        """
+        try:
+            return self.run_ranking(case)
+        except Exception:
+            logger.exception("Error running case {}", case.name)
+            return None
+
     def run_ranking(self, case: models.Case) -> typing.Optional[models.Result]:
         """Run the ranking for the given case.
 
         :param case: The case to run the ranking for.
         :returns: result for the case or ``None`` if no result was found.
         """
         _ = case
@@ -297,20 +316,27 @@
             ]
             try:
                 subprocess.check_output(cmd, stderr=subprocess.STDOUT)
             except subprocess.CalledProcessError:
                 logger.error("Error running CADA")
                 return None
 
+            # Get the gene IDs to consider at all.
+            candidate_gene_ids = set(case.candidate_gene_ids or [])
+
             # Read the output file.
             with open(f"{tmpdir}/result.txt", "rt") as inputf:
                 reader = csv.DictReader(inputf, delimiter="\t")
                 # Translate the gene symbols from the result to entrez ids.
                 for row in reader:
-                    result_entrez_ids.append(row["gene_id"])
+                    if (
+                        row["gene_id"] == case.disease_gene_id
+                        or row["gene_id"] in candidate_gene_ids
+                    ):
+                        result_entrez_ids.append(row["gene_id"])
 
         # Determine rank for case.
         try:
             rank = result_entrez_ids.index(case.disease_gene_id) + 1
         except ValueError:
             logger.error("Disease gene {} not found in results?", case.disease_gene_id)
             return None
```

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/PKG-INFO` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-ranking-shootout
-Version: 0.1.2
+Version: 0.1.3
 Summary: Compare gene ranking methods.
 Home-page: https://github.com/bihealth/gene-ranking-shootout
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 Keywords: genes,ranking
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -21,29 +21,33 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 [![CI](https://github.com/bihealth/gene-ranking-shootout/actions/workflows/main.yml/badge.svg)](https://github.com/bihealth/gene-ranking-shootout/actions/workflows/main.yml)
-[![Pypi Package Version](https://img.shields.io/pypi/v/gene-ranking-shootout.svg)](https://pypi.org/v/gene-ranking-shootout)
+[![Pypi Package Version](https://img.shields.io/pypi/v/gene-ranking-shootout.svg)](https://pypi.org/project/gene-ranking-shootout)
 [![Pypi Python Version](https://img.shields.io/pypi/pyversions/gene-ranking-shootout.svg)](https://pypi.org/project/gene-ranking-shootout)
 
 # Gene Ranking Shootout
 
 A benchmark for methods that rank genes according to their relevance for a given phenotype (list of HPO terms).
 
 ## Methods
 
 The following methods are currently included in the benchmark:
 
 - AMELIE (via web service)
 - CADA (via custom Docker/Podman image)
 - Phen2Gene (via official Docker/Podman image)
 - Phenix algorithm (as implemented in VarFish)
+- Exomiser Algorithms:
+  - Phenix
+  - Phive
+  - HiPhive (variants: human only, human-mouse only, all human-mouse-fish-ppi)
 
 ## Installation
 
 Simply install with `pip` (probably inside a conda environment or virtualenv):
 
 ```bash
 $ git clone https://github.com/bihealth/gene-ranking-shootout.git
@@ -115,15 +119,15 @@
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ phenix /tmp/cases.json /tmp/result-exomiser-phenix.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ phive /tmp/cases.json /tmp/result-exomiser-phive.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive /tmp/cases.json /tmp/result-exomiser-hiphive.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive-mouse /tmp/cases.json /tmp/result-exomiser-hiphive-mouse.json
 $ gene-ranking-shootout benchmark exomiser http://localhost:8081/ hiphive-human /tmp/cases.json /tmp/result-exomiser-hiphive-human.json
 ```
 
-You can also visualize the details of the benchmark results for each result file (below for 100 cases).
+You can also visualize the details of the benchmark results for each result file (below for 100 cases). This visualization displays the number of true disease genes (from case set definitions) at TOP10 and following positions in the ranked gene list of the respective method.
 
 ```bash
 $ gene-ranking-shootout benchmark summarize /tmp/result-amelie.json
     1:   48  ################################
     2:   17  ###########
     3:    7  ####
     4:    3  ##
@@ -214,36 +218,36 @@
 ## Some Preliminary Results
 
 The following was generated on 2023/05/05 with all 4714 cases.
 
 ```
 $ for f in /tmp/result-*.json; do (set -x; gene-ranking-shootout benchmark summarize --bars-top-n 20 $f); echo; done
 + gene-ranking-shootout benchmark summarize --bars-top-n 20 result-cada.json
-    1: 1340  ##################
-    2:  290  ####
-    3:  192  ##
-    4:  164  ##
-    5:   96  #
-    6:   84  #
-    7:   94  #
-    8:   59  .
-    9:   63  .
-   10:   40  .
-   11:   62  .
-   12:   47  .
-   13:   33  .
-   14:   43  .
-   15:   38  .
-   16:   42  .
-   17:   36  .
-   18:   16  .
-   19:   30  .
-   20:   22  .
+    1: 3462  ################################################
+    2:  536  #######
+    3:  205  ##
+    4:  133  #
+    5:   71  .
+    6:   57  .
+    7:   39  .
+    8:   47  .
+    9:   16  .
+   10:   24  .
+   11:   14  .
+   12:   22  .
+   13:   14  .
+   14:   11  .
+   15:    7  .
+   16:    9  .
+   17:    8  .
+   18:    4  .
+   19:    3  .
+   20:    3  .
 
-21-..: 1923  ##########################
+21-..:   29  .
 mssng:    0  
 
 + gene-ranking-shootout benchmark summarize --bars-top-n 20 result-exomiser-hiphive-human.json
     1: 2593  ####################################
     2:  637  ########
     3:  375  #####
     4:  203  ##
```

### Comparing `gene-ranking-shootout-0.1.2/gene_ranking_shootout.egg-info/SOURCES.txt` & `gene-ranking-shootout-0.1.3/gene_ranking_shootout.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE
 Makefile
 README.md
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/automerge.yml
 .github/workflows/conventional-prs.yml
 .github/workflows/main.yml
 .github/workflows/release-please.yml
 docker/cada/Dockerfile
 docker/cada/build.sh
 gene_ranking_shootout/__init__.py
 gene_ranking_shootout/models.py
```

### Comparing `gene-ranking-shootout-0.1.2/setup.cfg` & `gene-ranking-shootout-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/tests/data/amelie/response.json` & `gene-ranking-shootout-0.1.3/tests/data/amelie/response.json`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/tests/data/cada/result.txt` & `gene-ranking-shootout-0.1.3/tests/data/cada/result.txt`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/tests/data/phen2gene/genes.txt` & `gene-ranking-shootout-0.1.3/tests/data/phen2gene/genes.txt`

 * *Files identical despite different names*

### Comparing `gene-ranking-shootout-0.1.2/tests/data/phen2gene/output_file.associated_gene_list` & `gene-ranking-shootout-0.1.3/tests/data/phen2gene/output_file.associated_gene_list`

 * *Files identical despite different names*

