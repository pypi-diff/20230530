# Comparing `tmp/spacy-llm-0.1.2.tar.gz` & `tmp/spacy-llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.1.2.tar", last modified: Fri May 12 12:09:14 2023, max compression
+gzip compressed data, was "spacy-llm-0.2.0.tar", last modified: Tue May 30 16:13:29 2023, max compression
```

## Comparing `spacy-llm-0.1.2.tar` & `spacy-llm-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,131 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.744273 spacy-llm-0.1.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    28560 2023-05-12 12:09:14.744273 spacy-llm-0.1.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    27397 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      402 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1526 2023-05-12 12:09:14.744273 spacy-llm-0.1.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.736273 spacy-llm-0.1.2/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      338 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3454 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2535 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/backends/rest/backend/
--rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/rest/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/rest/backend/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/rest/backend/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5334 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/rest/backend/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1501 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6645 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)      981 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10296 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1327 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      135 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6632 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      876 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6349 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      602 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      582 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2247 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)      785 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3375 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.740273 spacy-llm-0.1.2/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.744273 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)    12989 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14457 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5487 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1302 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-05-12 12:09:03.000000 spacy-llm-0.1.2/spacy_llm/ty.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-12 12:09:14.736273 spacy-llm-0.1.2/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    28560 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2235 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-12 12:09:14.000000 spacy-llm-0.1.2/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    51685 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    50441 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      644 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-05-30 16:13:29.249338 spacy-llm-0.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      187 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1233 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2791 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/minichain.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/
+-rw-r--r--   0 vsts      (1001) docker     (122)      239 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/openai.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7682 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6431 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      534 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4299 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4264 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4156 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/spancat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1203 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     6917 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4104 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/span.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_minichain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      110 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      836 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4703 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/ner_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/ner_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/ner_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/templates/ner_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/templates/textcat_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)    18403 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2685 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13930 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16984 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5507 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7852 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    51685 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3872 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/ner_minichain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_minichain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_minichain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3483 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.1.2/LICENSE` & `spacy-llm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.2/PKG-INFO` & `spacy-llm-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,19 @@
-Metadata-Version: 2.1
-Name: spacy-llm
-Version: 0.1.2
-Summary: Integrating LLMs into structured NLP pipelines
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
-Project-URL: Source, https://github.com/explosion/spacy-llm
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/external.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 This package integrates Large Language Models (LLMs) into [spaCy](https://spacy.io), featuring a modular system for **fast prototyping** and **prompting**, and turning unstructured responses into **robust outputs** for various NLP tasks, **no training data** required.
 
 - Serializable `llm` **component** to integrate prompts into your pipeline
-- **Modular functions** to define the [**task**](#Tasks) (prompting and parsing) and [**backend**](#Backends) (model to use)
+- **Modular functions** to define the [**task**](#tasks) (prompting and parsing) and [**backend**](#backends) (model to use)
 - Support for **hosted APIs** and self-hosted **open-source models**
 - Integration with [`MiniChain`](https://github.com/srush/MiniChain) and [`LangChain`](https://github.com/hwchase17/langchain)
 - Access to **[OpenAI API](https://platform.openai.com/docs/api-reference/introduction)**, including GPT-4 and various GPT-3 models
 - Built-in support for **open-source [Dolly](https://huggingface.co/databricks)** models hosted on Hugging Face
 - Usage examples for **Named Entity Recognition** and **Text Classification**
 - Easy implementation of **your own functions** via [spaCy's registry](https://spacy.io/api/top-level#registry) for custom prompting, parsing and model integrations
 
@@ -73,15 +44,15 @@
 The task and the backend have to be supplied to the `llm` pipeline component using [spaCy's config
 system](https://spacy.io/api/data-formats#config). This package provides various built-in
 functionality, as detailed in the [API](#-api) documentation.
 
 ### Example 1: Add a text classifier using a GPT-3 model from OpenAI
 
 Create a new API key from openai.com or fetch an existing one, and ensure the keys are set as environmental variables.
-For more background information, see the [OpenAI](#OpenAI) section.
+For more background information, see the [OpenAI](#openai) section.
 
 Create a config file `config.cfg` containing at least the following
 (or see the full example [here](usage_examples/textcat_openai)):
 
 ```ini
 [nlp]
 lang = "en"
@@ -89,30 +60,29 @@
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
-@llm_tasks = "spacy.TextCat.v1"
+@llm_tasks = "spacy.TextCat.v2"
 labels = COMPLIMENT,INSULT
 
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
-config = {"model": "text-davinci-003", "temperature": 0.3}
+config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
 Now run:
 
 ```python
-from spacy import util
+from spacy_llm.util import assemble
 
-config = util.load_config("config.cfg")
-nlp = util.load_model_from_config(config, auto_fill=True)
+nlp = assemble("config.cfg")
 doc = nlp("You look gorgeous!")
 print(doc.cats)
 ```
 
 ### Example 2: Add NER using an open-source model through Hugging Face
 
 To run this example, ensure that you have a GPU enabled, and `transformers`, `torch` and CUDA installed.
@@ -128,30 +98,29 @@
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
-@llm_tasks = "spacy.NER.v1"
+@llm_tasks = "spacy.NER.v2"
 labels = PERSON,ORGANISATION,LOCATION
 
 [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
 Now run:
 
 ```python
-from spacy import util
+from spacy_llm.util import assemble
 
-config = util.load_config("config.cfg")
-nlp = util.load_model_from_config(config, auto_fill=True)
+nlp = assemble("config.cfg")
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
 
 Note that Hugging Face will download the `"databricks/dolly-v2-3b"` model the first time you use it. You can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
@@ -166,73 +135,87 @@
 import spacy
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "llm",
     config={
         "task": {
-            "@llm_tasks": "spacy.NER.v1",
+            "@llm_tasks": "spacy.NER.v2",
             "labels": "PERSON,ORGANISATION,LOCATION"
         },
         "backend": {
             "@llm_backends": "spacy.REST.v1",
             "api": "OpenAI",
-            "config": {"model": "text-davinci-003"},
+            "config": {"model": "gpt-3.5-turbo"},
         },
     },
 )
+nlp.initialize()
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
 
 Note that for efficient usage of resources, typically you would use [`nlp.pipe(docs)`](https://spacy.io/api/language#pipe)
 with a batch, instead of calling `nlp(doc)` with a single document.
 
 ### Example 4: Implement your own custom task
 
 To write a
 [`task`](#tasks), you
 need to implement two functions: `generate_prompts` that takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
 them into a list of prompts, and `parse_responses` that transforms the LLM outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
 
+To register your custom task with spaCy, decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer to in your config.
+
 > 📖 For more details, see the [**usage example on writing your own task**](usage_examples/README.md#writing-your-own-task)
 
 ```python
 from spacy_llm.registry import registry
+from spacy_llm.util import split_labels
+
+
+@registry.llm_tasks("my_namespace.MyTask.v1")
+def make_my_task(labels: str, my_other_config_val: float) -> "MyTask":
+    labels_list = split_labels(labels)
+    return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
+
 
-@registry.llm_tasks("spacy.MyTask.v1")
 class MyTask:
-    def __init__(self, labels: str):
+    def __init__(self, labels: List[str], my_other_config_val: float):
         ...
 
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         ...
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
         ...
 ```
 
 ```ini
 # config.cfg (excerpt)
 [components.llm.task]
-@llm_tasks = "spacy.MyTask.v1"
+@llm_tasks = "my_namespace.MyTask.v1"
 labels = LABEL1,LABEL2,LABEL3
+my_other_config_val = 0.3
 ```
 
 ## 📓 API
 
 Each `llm` component is defined by two main settings:
 
-- A [**task**](#Tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
+- A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
-- A [**backend**](#Backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
+- A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
 
+Moreover, the component also implements [**caching**](#cache) functionality to avoid running
+the same document through an LLM service (be it local or through a REST API) more than once.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -258,17 +241,89 @@
 
 | Argument    | Type            | Description              |
 | ----------- | --------------- | ------------------------ |
 | `docs`      | `Iterable[Doc]` | The input documents.     |
 | `responses` | `Iterable[Any]` | The generated prompts.   |
 | **RETURNS** | `Iterable[Doc]` | The annotated documents. |
 
+#### spacy.NER.v2
+
+The built-in NER task supports both zero-shot and few-shot prompting. This version also supports explicitly defining the provided labels with custom descriptions.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,ORGANISATION,LOCATION
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                  | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`                  | `str`                                   |                                                          | Comma-separated list of labels.                                                                                                                       |
+| `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                   | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                   | Optional function that generates examples for few-shot learning.                                                                                      |
+| `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                   | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
+| `alignment_mode`          | `str`                                   | `"contract"`                                             | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
+| `case_sensitive_matching` | `bool`                                  | `False`                                                  | Whether to search without case sensitivity.                                                                                                           |
+| `single_match`            | `bool`                                  | `False`                                                  | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
+
+The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
+This means that a form of string matching is required. This can be configured by the following parameters:
+
+- The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
+  want to mark it every time it occurs in the document.
+- The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
+- The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
+  in the call to [`doc.char_span()`](https://spacy.io/api/doc#char_span). The `"strict"` mode will only keep spans that strictly adhere to the given token boundaries.
+  `"contract"` will only keep those tokens that are fully within the given range, e.g. reducing `"New Y"` to `"New"`.
+  Finally, `"expand"` will expand the span to the next token boundaries, e.g. expanding `"New Y"` out to `"New York"`.
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: Jack and Jill went up the hill.
+  entities:
+    PERSON:
+      - Jack
+      - Jill
+    LOCATION:
+      - hill
+- text: Jack fell down and broke his crown.
+  entities:
+    PERSON:
+      - Jack
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,ORGANISATION,LOCATION
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "ner_examples.yml"
+```
+
+If you don't have specific examples to provide to the LLM, you can write definitions for each label and provide them via the `label_definitions` argument. This lets you tell the LLM exactly what you're looking for rather than relying on the LLM to interpret its task given just the label name. Label descriptions are freeform so you can write whatever you want here, but through some experiments a brief description along with some examples and counter examples seems to work quite well.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,SPORTS_TEAM
+[components.llm.task.label_definitions]
+PERSON = "Extract any named individual in the text."
+SPORTS_TEAM = "Extract the names of any professional sports team. e.g. Golden State Warriors, LA Lakers, Man City, Real Madrid"
+```
+
+> Label descriptions can also be used with explicit examples to give as much info to the LLM backend as possible.
+
 #### spacy.NER.v1
 
-The built-in NER task supports both zero-shot and few-shot prompting.
+The original version of the built-in NER task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v1"
 labels = PERSON,ORGANISATION,LOCATION
 examples = null
 ```
@@ -278,14 +333,16 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
+[ner]: https://github.com/explosion/spacy-llm/blob/main/spacy_llm/tasks/ner.py#L14
+
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
 - The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
@@ -315,20 +372,120 @@
 @llm_tasks = "spacy.NER.v1"
 labels = PERSON,ORGANISATION,LOCATION
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "ner_examples.yml"
 ```
 
-#### spacy.TextCat.v1
+#### spacy.SpanCat.v2
+
+The built-in SpanCat task is a simple adaptation of the NER task to
+support overlapping entities and store its annotations in `doc.spans`.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.SpanCat.v2"
+labels = PERSON,ORGANISATION,LOCATION
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                            | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`                  | `str`                                   |                                                                    | Comma-separated list of labels.                                                                                                                       |
+| `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                             | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
+| `spans_key`               | `str`                                   | `"sc"`                                                             | Key of the `Doc.spans` dict to save the spans under.                                                                                                  |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                             | Optional function that generates examples for few-shot learning.                                                                                      |
+| `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                             | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
+| `alignment_mode`          | `str`                                   | `"contract"`                                                       | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
+| `case_sensitive_matching` | `bool`                                  | `False`                                                            | Whether to search without case sensitivity.                                                                                                           |
+| `single_match`            | `bool`                                  | `False`                                                            | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
+
+Except for the `spans_key` parameter, the SpanCat task reuses the configuration
+from the NER task.
+Refer to [its documentation](#spacynerv2) for more insight.
+
+#### spacy.SpanCat.v1
+
+The original version of the built-in SpanCat task is a simple adaptation of the v1 NER task to
+support overlapping entities and store its annotations in `doc.spans`.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.SpanCat.v1"
+labels = PERSON,ORGANISATION,LOCATION
+examples = null
+```
+
+| Argument                  | Type                                    | Default      | Description                                                                                                                                  |
+| ------------------------- | --------------------------------------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
+| `spans_key`               | `str`                                   | `"sc"`       | Key of the `Doc.spans` dict to save the spans under.                                                                                         |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
+| `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
+| `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
+| `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
+| `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
+
+Except for the `spans_key` parameter, the SpanCat task reuses the configuration
+from the NER task.
+Refer to [its documentation](#spacynerv1) for more insight.
+
+#### spacy.TextCat.v2
 
 The built-in TextCat task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
+@llm_tasks = "spacy.TextCat.v2"
+labels = COMPLIMENT,INSULT
+examples = null
+```
+
+| Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
+| ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
+| `labels`            | `str`                                   |                                                              | Comma-separated list of labels.                                                                                                                  |
+| `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
+| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
+| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
+| `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
+| `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
+| `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```json
+[
+  {
+    "text": "You look great!",
+    "answer": "Compliment"
+  },
+  {
+    "text": "You are not very clever at all.",
+    "answer": "Insult"
+  }
+]
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.TextCat.v2"
+labels = COMPLIMENT,INSULT
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "textcat_examples.json"
+```
+
+#### spacy.TextCat.v1
+
+The original version of the built-in TextCat task supports both zero-shot and few-shot prompting.
+
+```ini
+[components.llm.task]
 @llm_tasks = "spacy.TextCat.v1"
 labels = COMPLIMENT,INSULT
 examples = null
 ```
 
 | Argument            | Type                                    | Default | Description                                                                                                                                      |
 | ------------------- | --------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
@@ -353,21 +510,62 @@
     "answer": "Insult"
   }
 ]
 ```
 
 ```ini
 [components.llm.task]
-@llm_tasks = "spacy.TextCat.v1"
+@llm_tasks = "spacy.TextCat.v2"
 labels = COMPLIMENT,INSULT
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "textcat_examples.json"
 ```
 
+#### spacy.REL.v1
+
+The built-in REL task supports both zero-shot and few-shot prompting.
+It relies on an upstream NER component for entities extraction.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.REL.v1"
+labels = LivesIn,Visits
+```
+
+| Argument            | Type                                    | Default                                              | Description                                                                                                                              |
+| ------------------- | --------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`            | `str`                                   |                                                      | Comma-separated list of relation labels.                                                                                                 |
+| `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                              |
+| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                         |
+| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                     |
+| `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                     |
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```json
+{"text": "Laura bought a house in Boston with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label": "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char": 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1, "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]}
+{"text": "Michael travelled through South America by bike.", "ents": [{"start_char": 0, "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label": "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]}
+```
+
+Note: the REL task relies on pre-extracted entities to make its prediction.
+Hence, you'll need to add a component that populates `doc.ents` with recognized
+spans to your spaCy pipeline and put it _before_ the REL component.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.REL.v1"
+labels = LivesIn,Visits
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "rel_examples.jsonl"
+```
+
 #### spacy.NoOp.v1
 
 This task is only useful for testing - it tells the LLM to do nothing, and does not set any fields on the `docs`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
@@ -377,15 +575,31 @@
 
 A _backend_ defines which LLM model to query, and how to query it. It can be a simple function taking a collection
 of prompts (consistent with the output type of `task.generate_prompts()`) and returning a collection of responses
 (consistent with the expected input of `parse_responses`). Generally speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
 but specific implementations can have other signatures, like `Callable[[Iterable[str]], Iterable[str]]`.
 
 All built-in backends are registered in `llm_backends`. If no backend is specified, the repo currently connects to the [`OpenAI` API](#openai) by default,
-using the built-in REST protocol, and accesses the `"text-davinci-003"` model.
+using the built-in REST protocol, and accesses the `"gpt-3.5-turbo"` model.
+
+> :question: _Why are there backends for third-party libraries in addition to a native REST backend and which should
+> I choose?_
+>
+> Third-party libraries like `langchain` or `minichain` focus on prompt management, integration of many different LLM
+> APIs, and other related features such as conversational memory or agents. `spacy-llm` on the other hand emphasizes
+> features we consider useful in the context of NLP pipelines utilizing LLMs to process documents (mostly) independent
+> from each other. It makes sense that the feature set of such third-party libraries and `spacy-llm` is not identical -
+> and users might want to take advantage of features not available in `spacy-llm`.
+>
+> The advantage of offering our own REST backend is that we can ensure a larger degree of stability of robustness, as
+> we can guarantee backwards-compatibility and more smoothly integrated error handling.
+>
+> Ultimately we recommend trying to implement your use case using the REST backend first (which is configured as the
+> default backend). If however there are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting mechanism, if so required.
 
 #### OpenAI
 
 When the backend uses OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
 environmental variables:
 
 ```shell
@@ -397,15 +611,15 @@
 
 This default backend uses `requests` and a simple retry mechanism to access an API.
 
 ```ini
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
-config = {"model": "text-davinci-003", "temperature": 0.3}
+config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
 | Argument    | Type             | Default | Description                                                                                                          |
 | ----------- | ---------------- | ------- | -------------------------------------------------------------------------------------------------------------------- |
 | `api`       | `str`            |         | The name of a supported API. In v.0.1.0, only "OpenAI" is supported.                                                 |
 | `config`    | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the backend.                                                                      |
 | `strict`    | `bool`           | `True`  | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
@@ -434,14 +648,16 @@
 
 #### spacy.MiniChain.v1
 
 To use [MiniChain](https://github.com/srush/MiniChain) for the API retrieval part, make sure you have installed it first:
 
 ```shell
 python -m pip install "minichain>=0.3,<0.4"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[minichain]"
 ```
 
 Note that MiniChain currently only supports Python 3.8, 3.9 and 3.10.
 
 Example config blocks:
 
 ```ini
@@ -463,14 +679,16 @@
 
 #### spacy.LangChain.v1
 
 To use [LangChain](https://github.com/hwchase17/langchain) for the API retrieval part, make sure you have installed it first:
 
 ```shell
 python -m pip install "langchain>=0.0.144,<0.1"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[langchain]"
 ```
 
 Note that LangChain currently only supports Python 3.9 and beyond.
 
 Example config block:
 
 ```ini
@@ -491,17 +709,18 @@
 
 #### spacy.DollyHF.v1
 
 To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
 This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
 ```shell
-python -m pip install "cupy-cuda11x"
 python -m pip install "torch>=1.13.1,<2.0"
 python -m pip install "transformers>=4.28.1,<5.0"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[transformers]"
 ```
 
 If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries.
 
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
@@ -526,14 +745,40 @@
 - `"databricks/dolly-v2-7b"`
 - `"databricks/dolly-v2-12b"`
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
+### Cache
+
+Interacting with LLMs, either through an external API or a local instance, is costly.
+Since developing an NLP pipeline generally means a lot of exploration and prototyping,
+`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
+
+Example config block:
+
+```ini
+[components.llm.cache]
+@llm_misc = "spacy.BatchCache.v1",
+path = "path/to/cache"
+batch_size = 64
+max_batches_in_mem = 4
+```
+
+| Argument             | Type                         | Default | Description                                          |
+| -------------------- | ---------------------------- | ------- | ---------------------------------------------------- |
+| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed. |
+| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file).                  |
+| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory.            |
+
+Note that since the cache is generated by a registered function, you can also provide your own registered function
+returning your own cache implementation. If you wish to do so, ensure that your cache object adheres to the
+`Protocol` defined in `spacy_llm.ty.Cache`.
+
 ### Various functions
 
 #### spacy.FewShotReader.v1
 
 This function is registered in spaCy's `misc` registry, and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file.
 It uses [`srsly`](https://github.com/explosion/srsly) to read in these files and parses them depending on the file extension.
 
@@ -543,14 +788,30 @@
 path = "ner_examples.yml"
 ```
 
 | Argument | Type               | Description                                                                |
 | -------- | ------------------ | -------------------------------------------------------------------------- |
 | `path`   | `Union[str, Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
 
+#### spacy.FileReader.v1
+
+This function is registered in spaCy's `misc` registry, and reads a file provided to the `path` to return a `str`
+representation of its contents. This function is typically used to read
+[Jinja](https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt template.
+
+```ini
+[components.llm.task.template]
+@misc = "spacy.FileReader.v1"
+path = "ner_template.jinja2"
+```
+
+| Argument | Type               | Description                  |
+| -------- | ------------------ | ---------------------------- |
+| `path`   | `Union[str, Path]` | Path to the file to be read. |
+
 #### Normalizer functions
 
 These functions provide simple normalizations for string comparisons, e.g. between a list of specified labels
 and a label given in the raw text of the LLM response. They are registered in spaCy's `misc` registry
 and have the signature `Callable[[str], str]`.
 
 - `spacy.StripNormalizer.v1`: only apply `text.strip()`
```

#### html2text {}

```diff
@@ -1,146 +1,139 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.1.2 Summary: Integrating LLMs
-into structured NLP pipelines Author: Explosion Author-email:
-contact@explosion.ai License: MIT Project-URL: Release notes, https://
-github.com/explosion/spacy-llm/releases Project-URL: Source, https://
-github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/
-img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP pipelines !
-[GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/
-explosion/spacy-llm/external.yml) [![pypi Version](https://img.shields.io/pypi/
-v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/
-project/spacy-llm/) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/
-black) This package integrates Large Language Models (LLMs) into [spaCy](https:
-//spacy.io), featuring a modular system for **fast prototyping** and
-**prompting**, and turning unstructured responses into **robust outputs** for
-various NLP tasks, **no training data** required. - Serializable `llm`
-**component** to integrate prompts into your pipeline - **Modular functions**
-to define the [**task**](#Tasks) (prompting and parsing) and [**backend**]
-(#Backends) (model to use) - Support for **hosted APIs** and self-hosted
-**open-source models** - Integration with [`MiniChain`](https://github.com/
-srush/MiniChain) and [`LangChain`](https://github.com/hwchase17/langchain) -
-Access to **[OpenAI API](https://platform.openai.com/docs/api-reference/
-introduction)**, including GPT-4 and various GPT-3 models - Built-in support
-for **open-source [Dolly](https://huggingface.co/databricks)** models hosted on
-Hugging Face - Usage examples for **Named Entity Recognition** and **Text
-Classification** - Easy implementation of **your own functions** via [spaCy's
-registry](https://spacy.io/api/top-level#registry) for custom prompting,
-parsing and model integrations ## ð§  Motivation Large Language Models (LLMs)
-feature powerful natural language understanding capabilities. With only a few
-(and sometimes no) examples, an LLM can be prompted to perform custom NLP tasks
-such as text categorization, named entity recognition, coreference resolution,
-information extraction and more. [spaCy](https://spacy.io) is a well-
-established library for building systems that need to work with language in
-various ways. spaCy's built-in components are generally powered by supervised
-learning or rule-based approaches. Supervised learning is much worse than LLM
-prompting for prototyping, but for many tasks it's much better for production.
-A transformer model that runs comfortably on a single GPU is extremely
-powerful, and it's likely to be a better choice for any task for which you have
-a well-defined output. You train the model with anything from a few hundred to
-a few thousand labelled examples, and it will learn to do exactly that.
-Efficiency, reliability and control are all better with supervised learning,
-and accuracy will generally be higher than LLM prompting as well. `spacy-llm`
-lets you have **the best of both worlds**. You can quickly initialize a
-pipeline with components powered by LLM prompts, and freely mix in components
-powered by other approaches. As your project progresses, you can look at
-replacing some or all of the LLM-powered components as you require. Of course,
-there can be components in your system for which the power of an LLM is fully
-justified. If you want a system that can synthesize information from multiple
-documents in subtle ways and generate a nuanced summary for you, bigger is
-better. However, even if your production system needs an LLM for some of the
-task, that doesn't mean you need an LLM for all of it. Maybe you want to use a
-cheap text classification model to help you find the texts to summarize, or
-maybe you want to add a rule-based system to sanity check the output of the
-summary. These before-and-after tasks are much easier with a mature and well-
-thought-out library, which is exactly what spaCy provides. ## â³ Install
-`spacy-llm` will be installed automatically in future spaCy versions. For now,
-you can run the following in the same virtual environment where you already
-have `spacy` [installed](https://spacy.io/usage). ```bash python -m pip install
-spacy-llm ``` > â ï¸ This package is still experimental and it is possible
-that changes made to the interface will be breaking in minor version updates.
-## ð Usage The task and the backend have to be supplied to the `llm`
-pipeline component using [spaCy's config system](https://spacy.io/api/data-
-formats#config). This package provides various built-in functionality, as
-detailed in the [API](#-api) documentation. ### Example 1: Add a text
-classifier using a GPT-3 model from OpenAI Create a new API key from openai.com
-or fetch an existing one, and ensure the keys are set as environmental
-variables. For more background information, see the [OpenAI](#OpenAI) section.
-Create a config file `config.cfg` containing at least the following (or see the
-full example [here](usage_examples/textcat_openai)): ```ini [nlp] lang = "en"
-pipeline = ["llm"] [components] [components.llm] factory = "llm"
-[components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
-COMPLIMENT,INSULT [components.llm.backend] @llm_backends = "spacy.REST.v1" api
-= "OpenAI" config = {"model": "text-davinci-003", "temperature": 0.3} ``` Now
-run: ```python from spacy import util config = util.load_config("config.cfg")
-nlp = util.load_model_from_config(config, auto_fill=True) doc = nlp("You look
-gorgeous!") print(doc.cats) ``` ### Example 2: Add NER using an open-source
-model through Hugging Face To run this example, ensure that you have a GPU
-enabled, and `transformers`, `torch` and CUDA installed. For more background
-information, see the [DollyHF](#spacydollyhfv1) section. Create a config file
+[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
+structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
+github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
+(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg?style=flat-square)](https://github.com/ambv/black) This package
+integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
+featuring a modular system for **fast prototyping** and **prompting**, and
+turning unstructured responses into **robust outputs** for various NLP tasks,
+**no training data** required. - Serializable `llm` **component** to integrate
+prompts into your pipeline - **Modular functions** to define the [**task**]
+(#tasks) (prompting and parsing) and [**backend**](#backends) (model to use) -
+Support for **hosted APIs** and self-hosted **open-source models** -
+Integration with [`MiniChain`](https://github.com/srush/MiniChain) and
+[`LangChain`](https://github.com/hwchase17/langchain) - Access to **[OpenAI
+API](https://platform.openai.com/docs/api-reference/introduction)**, including
+GPT-4 and various GPT-3 models - Built-in support for **open-source [Dolly]
+(https://huggingface.co/databricks)** models hosted on Hugging Face - Usage
+examples for **Named Entity Recognition** and **Text Classification** - Easy
+implementation of **your own functions** via [spaCy's registry](https://
+spacy.io/api/top-level#registry) for custom prompting, parsing and model
+integrations ## ð§  Motivation Large Language Models (LLMs) feature powerful
+natural language understanding capabilities. With only a few (and sometimes no)
+examples, an LLM can be prompted to perform custom NLP tasks such as text
+categorization, named entity recognition, coreference resolution, information
+extraction and more. [spaCy](https://spacy.io) is a well-established library
+for building systems that need to work with language in various ways. spaCy's
+built-in components are generally powered by supervised learning or rule-based
+approaches. Supervised learning is much worse than LLM prompting for
+prototyping, but for many tasks it's much better for production. A transformer
+model that runs comfortably on a single GPU is extremely powerful, and it's
+likely to be a better choice for any task for which you have a well-defined
+output. You train the model with anything from a few hundred to a few thousand
+labelled examples, and it will learn to do exactly that. Efficiency,
+reliability and control are all better with supervised learning, and accuracy
+will generally be higher than LLM prompting as well. `spacy-llm` lets you have
+**the best of both worlds**. You can quickly initialize a pipeline with
+components powered by LLM prompts, and freely mix in components powered by
+other approaches. As your project progresses, you can look at replacing some or
+all of the LLM-powered components as you require. Of course, there can be
+components in your system for which the power of an LLM is fully justified. If
+you want a system that can synthesize information from multiple documents in
+subtle ways and generate a nuanced summary for you, bigger is better. However,
+even if your production system needs an LLM for some of the task, that doesn't
+mean you need an LLM for all of it. Maybe you want to use a cheap text
+classification model to help you find the texts to summarize, or maybe you want
+to add a rule-based system to sanity check the output of the summary. These
+before-and-after tasks are much easier with a mature and well-thought-out
+library, which is exactly what spaCy provides. ## â³ Install `spacy-llm` will
+be installed automatically in future spaCy versions. For now, you can run the
+following in the same virtual environment where you already have `spacy`
+[installed](https://spacy.io/usage). ```bash python -m pip install spacy-llm
+``` > â ï¸ This package is still experimental and it is possible that changes
+made to the interface will be breaking in minor version updates. ## ð Usage
+The task and the backend have to be supplied to the `llm` pipeline component
+using [spaCy's config system](https://spacy.io/api/data-formats#config). This
+package provides various built-in functionality, as detailed in the [API](#-
+api) documentation. ### Example 1: Add a text classifier using a GPT-3 model
+from OpenAI Create a new API key from openai.com or fetch an existing one, and
+ensure the keys are set as environmental variables. For more background
+information, see the [OpenAI](#openai) section. Create a config file
 `config.cfg` containing at least the following (or see the full example [here]
+(usage_examples/textcat_openai)): ```ini [nlp] lang = "en" pipeline = ["llm"]
+[components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
+= "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.backend]
+@llm_backends = "spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-
+turbo", "temperature": 0.3} ``` Now run: ```python from spacy_llm.util import
+assemble nlp = assemble("config.cfg") doc = nlp("You look gorgeous!") print
+(doc.cats) ``` ### Example 2: Add NER using an open-source model through
+Hugging Face To run this example, ensure that you have a GPU enabled, and
+`transformers`, `torch` and CUDA installed. For more background information,
+see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
+containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.NER.v1" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
+= "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1" # For better performance, use databricks/
 dolly-v2-12b instead model = "databricks/dolly-v2-3b" ``` Now run: ```python
-from spacy import util config = util.load_config("config.cfg") nlp =
-util.load_model_from_config(config, auto_fill=True) doc = nlp("Jack and Jill
-rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for ent in
-doc.ents]) ``` Note that Hugging Face will download the `"databricks/dolly-v2-
-3b"` model the first time you use it. You can [define the cached directory]
-(https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
-setting the environmental variable `HF_HOME`. Also, you can upgrade the model
-to be `"databricks/dolly-v2-12b"` for better performance. ### Example 3: Create
-the component directly in Python The `llm` component behaves as any other spaCy
-component does, so adding it to an existing pipeline follows the same pattern:
-```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config=
-{ "task": { "@llm_tasks": "spacy.NER.v1", "labels":
+from spacy_llm.util import assemble nlp = assemble("config.cfg") doc = nlp
+("Jack and Jill rode up the hill in Les Deux Alpes") print([(ent.text,
+ent.label_) for ent in doc.ents]) ``` Note that Hugging Face will download the
+`"databricks/dolly-v2-3b"` model the first time you use it. You can [define the
+cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/
+manage-cache) by setting the environmental variable `HF_HOME`. Also, you can
+upgrade the model to be `"databricks/dolly-v2-12b"` for better performance. ###
+Example 3: Create the component directly in Python The `llm` component behaves
+as any other spaCy component does, so adding it to an existing pipeline follows
+the same pattern: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
+( "llm", config={ "task": { "@llm_tasks": "spacy.NER.v2", "labels":
 "PERSON,ORGANISATION,LOCATION" }, "backend": { "@llm_backends":
-"spacy.REST.v1", "api": "OpenAI", "config": {"model": "text-davinci-003"}, },
-}, ) doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes") print([
-(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient usage
-of resources, typically you would use [`nlp.pipe(docs)`](https://spacy.io/api/
-language#pipe) with a batch, instead of calling `nlp(doc)` with a single
-document. ### Example 4: Implement your own custom task To write a [`task`]
-(#tasks), you need to implement two functions: `generate_prompts` that takes a
-list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms them
-into a list of prompts, and `parse_responses` that transforms the LLM outputs
-into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans,
-text categories and more. > ð For more details, see the [**usage example on
-writing your own task**](usage_examples/README.md#writing-your-own-task)
-```python from spacy_llm.registry import registry @registry.llm_tasks
-("spacy.MyTask.v1") class MyTask: def __init__(self, labels: str): ... def
+"spacy.REST.v1", "api": "OpenAI", "config": {"model": "gpt-3.5-turbo"}, }, }, )
+nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
+print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
+usage of resources, typically you would use [`nlp.pipe(docs)`](https://
+spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
+single document. ### Example 4: Implement your own custom task To write a
+[`task`](#tasks), you need to implement two functions: `generate_prompts` that
+takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
+them into a list of prompts, and `parse_responses` that transforms the LLM
+outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity
+spans, text categories and more. To register your custom task with spaCy,
+decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator
+with a custom name that you can refer to in your config. > ð For more
+details, see the [**usage example on writing your own task**](usage_examples/
+README.md#writing-your-own-task) ```python from spacy_llm.registry import
+registry from spacy_llm.util import split_labels @registry.llm_tasks
+("my_namespace.MyTask.v1") def make_my_task(labels: str, my_other_config_val:
+float) -> "MyTask": labels_list = split_labels(labels) return MyTask
+(labels=labels_list, my_other_config_val=my_other_config_val) class MyTask: def
+__init__(self, labels: List[str], my_other_config_val: float): ... def
 generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]: ... def
 parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] ) -
 > Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
-@llm_tasks = "spacy.MyTask.v1" labels = LABEL1,LABEL2,LABEL3 ``` ## ð API
-Each `llm` component is defined by two main settings: - A [**task**](#Tasks),
-defining the prompt to send to the LLM as well as the functionality to parse
-the resulting response back into structured fields on spaCy's [Doc](https://
-spacy.io/api/doc) objects. - A [**backend**](#Backends) defining the model to
-use and how to connect to it. Note that `spacy-llm` supports both access to
-external APIs (such as OpenAI) as well as access to self-hosted open-source
-LLMs (such as using Dolly through Hugging Face). ### Tasks A _task_ defines an
-NLP problem or question, that will be sent to the LLM via a prompt. Further,
-the task defines how to parse the LLM's responses back into structured
-information. All tasks are registered in spaCy's `llm_tasks` registry.
-Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined
-in [`ty.py`](spacy_llm/ty.py). It needs to define a `generate_prompts` function
-and a `parse_responses` function. #### function `task.generate_prompts` Takes a
+@llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
+my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
+two main settings: - A [**task**](#tasks), defining the prompt to send to the
+LLM as well as the functionality to parse the resulting response back into
+structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
+[**backend**](#backends) defining the model to use and how to connect to it.
+Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
+well as access to self-hosted open-source LLMs (such as using Dolly through
+Hugging Face). Moreover, the component also implements [**caching**](#cache)
+functionality to avoid running the same document through an LLM service (be it
+local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
+problem or question, that will be sent to the LLM via a prompt. Further, the
+task defines how to parse the LLM's responses back into structured information.
+All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
+a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
+(spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
+`parse_responses` function. #### function `task.generate_prompts` Takes a
 collection of documents, and returns a collection of "prompts", which can be of
 type `Any`. Often, prompts are of type `str` - but this is not enforced to
 allow for maximum flexibility in the framework. | Argument | Type | Description
 | | ----------- | --------------- | ---------------------- | | `docs` |
 `Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
 generated prompts. | #### function `task.parse_responses` Takes a collection of
 LLM responses and the original documents, parses the responses into structured
@@ -148,31 +141,92 @@
 function is free to set the annotations in any way, including `Doc` fields like
 `ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
 of type `Iterable[Any]`, though they will often be `str` objects. This depends
 on the return type of the [backend](#backends). | Argument | Type | Description
 | | ----------- | --------------- | ------------------------ | | `docs` |
 `Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
 generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
-| #### spacy.NER.v1 The built-in NER task supports both zero-shot and few-shot
-prompting. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
+| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
+prompting. This version also supports explicitly defining the provided labels
+with custom descriptions. ```ini [components.llm.task] @llm_tasks =
+"spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
+Argument | Type | Default | Description | | ------------------------- | -------
+-------------------------------- | --------------------------------------------
+------------ | ----------------------------------------------------------------
+-------------------------------------------------------------------------------
+------ | | `labels` | `str` | | Comma-separated list of labels. | | `template`
+| `str` | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom
+prompt template to send to LLM backend. Default templates for each task are
+located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
+`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
+description of that label. These descriptions are added to the prompt to help
+instruct the LLM on what to extract. | | `examples` | `Optional[Callable[[],
+Iterable[Any]]]` | `None` | Optional function that generates examples for few-
+shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
+Function that normalizes the labels as returned by the LLM. If `None`, defaults
+to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"`
+| Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | The NER
+task implementation doesn't currently ask the LLM for specific offsets, but
+simply expects a list of strings that represent the enties in the document.
+This means that a form of string matching is required. This can be configured
+by the following parameters: - The `single_match` parameter is typically set to
+`False` to allow for multiple matches. For instance, the response from the LLM
+might only mention the entity "Paris" once, but you'd still want to mark it
+every time it occurs in the document. - The case-sensitive matching is
+typically set to `False` to be robust against case variances in the LLM's
+output. - The `alignment_mode` argument is used to match entities as returned
+by the LLM to the tokens from the original `Doc` - specifically it's used as
+argument in the call to [`doc.char_span()`](https://spacy.io/api/
+doc#char_span). The `"strict"` mode will only keep spans that strictly adhere
+to the given token boundaries. `"contract"` will only keep those tokens that
+are fully within the given range, e.g. reducing `"New Y"` to `"New"`. Finally,
+`"expand"` will expand the span to the next token boundaries, e.g. expanding
+`"New Y"` out to `"New York"`. To perform few-shot learning, you can write down
+a few examples in a separate file, and provide these to be injected into the
+prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```yaml - text: Jack and Jill went up the hill.
+entities: PERSON: - Jack - Jill LOCATION: - hill - text: Jack fell down and
+broke his crown. entities: PERSON: - Jack ``` ```ini [components.llm.task]
+@llm_tasks = "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"ner_examples.yml" ``` If you don't have specific examples to provide to the
+LLM, you can write definitions for each label and provide them via the
+`label_definitions` argument. This lets you tell the LLM exactly what you're
+looking for rather than relying on the LLM to interpret its task given just the
+label name. Label descriptions are freeform so you can write whatever you want
+here, but through some experiments a brief description along with some examples
+and counter examples seems to work quite well. ```ini [components.llm.task]
+@llm_tasks = "spacy.NER.v2" labels = PERSON,SPORTS_TEAM
+[components.llm.task.label_definitions] PERSON = "Extract any named individual
+in the text." SPORTS_TEAM = "Extract the names of any professional sports team.
+e.g. Golden State Warriors, LA Lakers, Man City, Real Madrid" ``` > Label
+descriptions can also be used with explicit examples to give as much info to
+the LLM backend as possible. #### spacy.NER.v1 The original version of the
+built-in NER task supports both zero-shot and few-shot prompting. ```ini
+[components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
 Description | | ------------------------- | -----------------------------------
 ---- | ------------ | ---------------------------------------------------------
 -------------------------------------------------------------------------------
 ---- | | `labels` | `str` | | Comma-separated list of labels. | | `examples` |
 `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
 generates examples for few-shot learning. | | `normalizer` | `Optional[Callable
 [[str], str]]` | `None` | Function that normalizes the labels as returned by
 the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | |
 `alignment_mode` | `str` | `"contract"` | Alignment mode in case the LLM
 returns entities that do not align with token boundaries. Options are
 `"strict"`, `"contract"` or `"expand"`. | | `case_sensitive_matching` | `bool`
 | `False` | Whether to search without case sensitivity. | | `single_match` |
 `bool` | `False` | Whether to match an entity in the LLM's response only once
-(the first hit) or multiple times. | The NER task implementation doesn't
+(the first hit) or multiple times. | [ner]: https://github.com/explosion/spacy-
+llm/blob/main/spacy_llm/tasks/ner.py#L14 The NER task implementation doesn't
 currently ask the LLM for specific offsets, but simply expects a list of
 strings that represent the enties in the document. This means that a form of
 string matching is required. This can be configured by the following
 parameters: - The `single_match` parameter is typically set to `False` to allow
 for multiple matches. For instance, the response from the LLM might only
 mention the entity "Paris" once, but you'd still want to mark it every time it
 occurs in the document. - The case-sensitive matching is typically set to
@@ -187,58 +241,185 @@
 perform few-shot learning, you can write down a few examples in a separate
 file, and provide these to be injected into the prompt to the LLM. The default
 reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
 ```yaml - text: Jack and Jill went up the hill. entities: PERSON: - Jack - Jill
 LOCATION: - hill - text: Jack fell down and broke his crown. entities: PERSON:
 - Jack ``` ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.TextCat.v1
-The built-in TextCat task supports both zero-shot and few-shot prompting.
-```ini [components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
-COMPLIMENT,INSULT examples = null ``` | Argument | Type | Default | Description
-| | ------------------- | --------------------------------------- | ------- | -
+"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.SpanCat.v2
+The built-in SpanCat task is a simple adaptation of the NER task to support
+overlapping entities and store its annotations in `doc.spans`. ```ini
+[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels =
+PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
+Description | | ------------------------- | -----------------------------------
+---- | ------------------------------------------------------------------ | ---
 -------------------------------------------------------------------------------
----------------------------------------------------------------- | | `labels` |
-str | | Comma-separated list of labels. | | `examples` | `Optional[Callable[[],
-Iterable[Any]]]` | `None` | Optional function that generates examples for few-
-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
-Function that normalizes the labels as returned by the LLM. If `None`, falls
+------------------------------------------------------------------- | |
+`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
+[`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom
+prompt template to send to LLM backend. Default templates for each task are
+located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
+`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
+description of that label. These descriptions are added to the prompt to help
+instruct the LLM on what to extract. | | `spans_key` | `str` | `"sc"` | Key of
+the `Doc.spans` dict to save the spans under. | | `examples` | `Optional
+[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
+examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
+str]]` | `None` | Function that normalizes the labels as returned by the LLM.
+If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` |
+`str` | `"contract"` | Alignment mode in case the LLM returns entities that do
+not align with token boundaries. Options are `"strict"`, `"contract"` or
+`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
+search without case sensitivity. | | `single_match` | `bool` | `False` |
+Whether to match an entity in the LLM's response only once (the first hit) or
+multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
+the configuration from the NER task. Refer to [its documentation](#spacynerv2)
+for more insight. #### spacy.SpanCat.v1 The original version of the built-in
+SpanCat task is a simple adaptation of the v1 NER task to support overlapping
+entities and store its annotations in `doc.spans`. ```ini [components.llm.task]
+@llm_tasks = "spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples
+= null ``` | Argument | Type | Default | Description | | ----------------------
+--- | --------------------------------------- | ------------ | ----------------
+-------------------------------------------------------------------------------
+--------------------------------------------- | | `labels` | `str` | | Comma-
+separated list of labels. | | `spans_key` | `str` | `"sc"` | Key of the
+`Doc.spans` dict to save the spans under. | | `examples` | `Optional[Callable[
+[], Iterable[Any]]]` | `None` | Optional function that generates examples for
+few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
+| Function that normalizes the labels as returned by the LLM. If `None`,
+defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` |
+`"contract"` | Alignment mode in case the LLM returns entities that do not
+align with token boundaries. Options are `"strict"`, `"contract"` or
+`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
+search without case sensitivity. | | `single_match` | `bool` | `False` |
+Whether to match an entity in the LLM's response only once (the first hit) or
+multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
+the configuration from the NER task. Refer to [its documentation](#spacynerv1)
+for more insight. #### spacy.TextCat.v2 The built-in TextCat task supports both
+zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = COMPLIMENT,INSULT examples = null ``` | Argument |
+Type | Default | Description | | ------------------- | ------------------------
+--------------- | -----------------------------------------------------------
+- | ---------------------------------------------------------------------------
+--------------------------------------------------------------------- | |
+`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
+[`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt
+template to send to LLM backend. Default templates for each task are located in
+the `spacy_llm/tasks/templates` directory. | | `examples` | `Optional[Callable[
+[], Iterable[Any]]]` | `None` | Optional function that generates examples for
+few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
+| Function that normalizes the labels as returned by the LLM. If `None`, falls
 back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
 `False` | If set to `True`, only one label per document should be valid. If set
 to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
 `True` | When set to `True`, allows the LLM to not return any of the given
 label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
 | | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
 when the LLM returns invalid responses. | To perform few-shot learning, you can
 write down a few examples in a separate file, and provide these to be injected
 into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
 supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
 great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
 "answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v1" labels = COMPLIMENT,INSULT [components.llm.task.examples]
+"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
-spacy.NoOp.v1 This task is only useful for testing - it tells the LLM to do
-nothing, and does not set any fields on the `docs`. ```ini
-[components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ### Backends A _backend_
-defines which LLM model to query, and how to query it. It can be a simple
-function taking a collection of prompts (consistent with the output type of
-`task.generate_prompts()`) and returning a collection of responses (consistent
-with the expected input of `parse_responses`). Generally speaking, it's a
-function of type `Callable[[Iterable[Any]], Iterable[Any]]`, but specific
-implementations can have other signatures, like `Callable[[Iterable[str]],
-Iterable[str]]`. All built-in backends are registered in `llm_backends`. If no
-backend is specified, the repo currently connects to the [`OpenAI` API]
-(#openai) by default, using the built-in REST protocol, and accesses the
-`"text-davinci-003"` model. #### OpenAI When the backend uses OpenAI, you have
+spacy.TextCat.v1 The original version of the built-in TextCat task supports
+both zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks
+= "spacy.TextCat.v1" labels = COMPLIMENT,INSULT examples = null ``` | Argument
+| Type | Default | Description | | ------------------- | ----------------------
+----------------- | ------- | -------------------------------------------------
+-------------------------------------------------------------------------------
+---------------- | | `labels` | str | | Comma-separated list of labels. | |
+`examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional
+function that generates examples for few-shot learning. | | `normalizer` |
+`Optional[Callable[[str], str]]` | `None` | Function that normalizes the labels
+as returned by the LLM. If `None`, falls back to
+`spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
+set to `True`, only one label per document should be valid. If set to `False`,
+one document can have multiple labels. | | `allow_none` | `bool` | `True` |
+When set to `True`, allows the LLM to not return any of the given label. The
+resulting dict in `doc.cats` will have `0.0` scores for all labels. | |
+`verbose` | `bool` | `False` | If set to `True`, warnings will be generated
+when the LLM returns invalid responses. | To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
+great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
+"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
+spacy.REL.v1 The built-in REL task supports both zero-shot and few-shot
+prompting. It relies on an upstream NER component for entities extraction.
+```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels =
+LivesIn,Visits ``` | Argument | Type | Default | Description | | --------------
+----- | --------------------------------------- | -----------------------------
+----------------------- | -----------------------------------------------------
+-------------------------------------------------------------------------------
+---- | | `labels` | `str` | | Comma-separated list of relation labels. | |
+`template` | `str` | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) |
+Custom prompt template to send to LLM backend. Default templates for each task
+are located in the `spacy_llm/tasks/templates` directory. | |
+`label_description` | `Optional[Dict[str, str]]` | `None` | Dictionary
+providing a description for each relation label. | | `examples` | `Optional
+[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
+examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
+str]]` | `None` | Function that normalizes the labels as returned by the LLM.
+If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose` | `bool`
+| `False` | If set to `True`, warnings will be generated when the LLM returns
+invalid responses. | To perform few-shot learning, you can write down a few
+examples in a separate file, and provide these to be injected into the prompt
+to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```json {"text": "Laura bought a house in Boston
+with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label":
+"PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char":
+48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1,
+"relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]} {"text":
+"Michael travelled through South America by bike.", "ents": [{"start_char": 0,
+"end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
+"LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
+the REL task relies on pre-extracted entities to make its prediction. Hence,
+you'll need to add a component that populates `doc.ents` with recognized spans
+to your spaCy pipeline and put it _before_ the REL component. ```ini
+[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = LivesIn,Visits
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
+testing - it tells the LLM to do nothing, and does not set any fields on the
+`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
+Backends A _backend_ defines which LLM model to query, and how to query it. It
+can be a simple function taking a collection of prompts (consistent with the
+output type of `task.generate_prompts()`) and returning a collection of
+responses (consistent with the expected input of `parse_responses`). Generally
+speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
+but specific implementations can have other signatures, like `Callable[
+[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
+`llm_backends`. If no backend is specified, the repo currently connects to the
+[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
+accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
+third-party libraries in addition to a native REST backend and which should > I
+choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
+prompt management, integration of many different LLM > APIs, and other related
+features such as conversational memory or agents. `spacy-llm` on the other hand
+emphasizes > features we consider useful in the context of NLP pipelines
+utilizing LLMs to process documents (mostly) independent > from each other. It
+makes sense that the feature set of such third-party libraries and `spacy-llm`
+is not identical - > and users might want to take advantage of features not
+available in `spacy-llm`. > > The advantage of offering our own REST backend is
+that we can ensure a larger degree of stability of robustness, as > we can
+guarantee backwards-compatibility and more smoothly integrated error handling.
+> > Ultimately we recommend trying to implement your use case using the REST
+backend first (which is configured as the > default backend). If however there
+are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting
+mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
 to get an API key from openai.com, and ensure that the keys are set as
 environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
 OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
 `requests` and a simple retry mechanism to access an API. ```ini
 [components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
-= {"model": "text-davinci-003", "temperature": 0.3} ``` | Argument | Type |
+= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
 Default | Description | | ----------- | ---------------- | ------- | ----------
 -------------------------------------------------------------------------------
 --------------------------- | | `api` | `str` | | The name of a supported API.
 In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
 | Further configuration passed on to the backend. | | `strict` | `bool` |
 `True` | If `True`, raises an error if the LLM API returns a malformed
 response. Otherwise, return the error responses as is. | | `max_tries` | `int`
@@ -249,15 +430,16 @@
 32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
 `"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
 babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
 `"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
 For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
 completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
 srush/MiniChain) for the API retrieval part, make sure you have installed it
-first: ```shell python -m pip install "minichain>=0.3,<0.4" ``` Note that
+first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
+spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
 MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
 blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
 api = "OpenAI" [components.llm.backend.query] @llm_queries =
 "spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
 --- | -------------------------------------------------------------------------
 -------- | ------- | ----------------------------------------------------------
 ------------------------- | | `api` | `str` | | The name of an API supported by
@@ -265,15 +447,16 @@
 configuration passed on to the backend. | | `query` | `Optional[Callable[
 ["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
 Function that executes the prompts. If `None`, defaults to
 `spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
 executes the prompts by running `model(text).run()` for each given textual
 prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
 hwchase17/langchain) for the API retrieval part, make sure you have installed
-it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" ``` Note
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
+with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
 that LangChain currently only supports Python 3.9 and beyond. Example config
 block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
 = "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
 {"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
 - | ---------------------------------------------------------------------------
 --- | ------- | ---------------------------------------------------------------
 --------------------- | | `api` | `str` | | The name of an API supported by
@@ -283,46 +466,68 @@
 that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
 The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
 `model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
 `torch` and CUDA in your virtual environment. This allows you to have the
 setting `device=cuda:0` in your config, which ensures that the model is loaded
 entirely on the GPU (and fails otherwise). ```shell python -m pip install
-"cupy-cuda11x" python -m pip install "torch>=1.13.1,<2.0" python -m pip install
-"transformers>=4.28.1,<5.0" ``` If you don't have access to a GPU, you can
-install `accelerate` and set`device_map=auto` instead, but be aware that this
-may result in some layers getting distributed to the CPU or even the hard
-drive, which may ultimately result in extremely slow queries. ```shell python -
-m pip install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+"torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0" # Or
+install with spacy-llm directly python -m pip install "spacy-llm[transformers]"
+``` If you don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
 "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
 ---- | ---------------- | ------- | -------------------------------------------
 ----------------------------------------------------- | | `model` | `str` | |
 The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
 `{}` | Further configuration passed on to the construction of the model with
 `transformers.pipeline()`. | Supported models (see the [Databricks models page]
 (https://huggingface.co/databricks) on Hugging Face for details): -
 `"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` - `"databricks/dolly-
 v2-12b"` Note that Hugging Face will download this model the first time you use
 it - you can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. ### Various functions #### spacy.FewShotReader.v1 This
-function is registered in spaCy's `misc` registry, and reads in examples from a
-`.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
-github.com/explosion/srsly) to read in these files and parses them depending on
-the file extension. ```ini [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument | Type |
-Description | | -------- | ------------------ | -------------------------------
-------------------------------------------- | | `path` | `Union[str, Path]` |
-Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
-#### Normalizer functions These functions provide simple normalizations for
-string comparisons, e.g. between a list of specified labels and a label given
-in the raw text of the LLM response. They are registered in spaCy's `misc`
-registry and have the signature `Callable[[str], str]`. -
-`spacy.StripNormalizer.v1`: only apply `text.strip()` -
+variable `HF_HOME`. ### Cache Interacting with LLMs, either through an external
+API or a local instance, is costly. Since developing an NLP pipeline generally
+means a lot of exploration and prototyping, `spacy-llm` implements a built-in
+cache to avoid reprocessing the same documents at each run. Example config
+block: ```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1", path =
+"path/to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
+Default | Description | | -------------------- | ---------------------------- |
+------- | ---------------------------------------------------- | | `path` |
+`Optional[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching
+is performed. | | `batch_size` | `int` | 64 | Number of docs in one batch
+(file). | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
+in memory. | Note that since the cache is generated by a registered function,
+you can also provide your own registered function returning your own cache
+implementation. If you wish to do so, ensure that your cache object adheres to
+the `Protocol` defined in `spacy_llm.ty.Cache`. ### Various functions ####
+spacy.FewShotReader.v1 This function is registered in spaCy's `misc` registry,
+and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses
+[`srsly`](https://github.com/explosion/srsly) to read in these files and parses
+them depending on the file extension. ```ini [components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument |
+Type | Description | | -------- | ------------------ | ------------------------
+-------------------------------------------------- | | `path` | `Union[str,
+Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or
+`.jsonl`. | #### spacy.FileReader.v1 This function is registered in spaCy's
+`misc` registry, and reads a file provided to the `path` to return a `str`
+representation of its contents. This function is typically used to read [Jinja]
+(https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt
+template. ```ini [components.llm.task.template] @misc = "spacy.FileReader.v1"
+path = "ner_template.jinja2" ``` | Argument | Type | Description | | -------- |
+------------------ | ---------------------------- | | `path` | `Union[str,
+Path]` | Path to the file to be read. | #### Normalizer functions These
+functions provide simple normalizations for string comparisons, e.g. between a
+list of specified labels and a label given in the raw text of the LLM response.
+They are registered in spaCy's `misc` registry and have the signature `Callable
+[[str], str]`. - `spacy.StripNormalizer.v1`: only apply `text.strip()` -
 `spacy.LowercaseNormalizer.v1`: applies `text.strip().lower()` to compare
 strings in a case-insensitive way. ## ð Ongoing work In the near future, we
 will - Add more example tasks - Support a broader range of models - Provide
 more example use-cases and tutorials - Make the built-in tasks easier to
 customize via Jinja templates to define the instructions & examples PRs are
 always welcome! ## ðï¸ Reporting issues If you have questions regarding the
 usage of `spacy-llm`, or want to give us feedback after giving it a spin,
```

### Comparing `spacy-llm-0.1.2/spacy_llm/backends/dolly.py` & `spacy-llm-0.2.0/spacy_llm/backends/integration/dolly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import warnings
 from typing import Any, Callable, Dict, Iterable
 
 from spacy.util import SimpleFrozenList, SimpleFrozenDict
 from thinc.compat import has_torch_cuda_gpu
 
-from ..compat import has_accelerate, has_torch, has_transformers, torch, transformers
-from ..registry.util import registry
+from . import Backend
+from ...compat import has_accelerate, has_torch, has_transformers, torch, transformers
+from ...registry.util import registry
 
 
 supported_models = SimpleFrozenList(
     ["databricks/dolly-v2-3b", "databricks/dolly-v2-7b", "databricks/dolly-v2-12b"]
 )
 
 
@@ -58,14 +59,25 @@
             raise ValueError(
                 "Install CUDA to load and run the LLM on the GPU, or install 'accelerate' to dynamically "
                 "distribute the LLM on the CPU or even the hard disk. The latter may be slow."
             )
     return default_cfg
 
 
+def query_dolly(
+    pipeline: "transformers.pipeline", prompts: Iterable[str]
+) -> Iterable[str]:
+    """Queries Dolly HF model.
+    pipeline (transformers.pipeline): Transformers pipeline to query.
+    prompts (Iterable[str]): Prompts to query Dolly model with.
+    RETURNS (Iterable[str]): Prompt responses.
+    """
+    return [pipeline(pr)[0]["generated_text"] for pr in prompts]
+
+
 @registry.llm_backends("spacy.DollyHF.v1")
 def backend_dolly_hf(
     model: str,
     config: Dict[Any, Any] = SimpleFrozenDict(),
 ) -> Callable[[Iterable[str]], Iterable[str]]:
     """Returns Callable that can execute a set of prompts and return the raw responses.
     model (str): Name of the HF model.
@@ -74,13 +86,10 @@
     """
     _check_installation()
     _check_model(model)
 
     if not config or len(config) == 0:
         config = _compile_default_config()
 
-    llm_pipeline = transformers.pipeline(model=model, **config)
-
-    def query(prompts: Iterable[str]) -> Iterable[str]:
-        return [llm_pipeline(pr)[0]["generated_text"] for pr in prompts]
-
-    return query
+    return Backend(
+        integration=transformers.pipeline(model=model, **config), query=query_dolly  # type: ignore[arg-type]
+    )
```

### Comparing `spacy-llm-0.1.2/spacy_llm/backends/langchain.py` & `spacy-llm-0.2.0/spacy_llm/backends/integration/langchain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 from typing import Any, Callable, Dict, Iterable, Optional, Type
-from typing import TYPE_CHECKING
 
 from spacy.util import SimpleFrozenDict
 
-from ..compat import has_langchain, langchain
-from ..registry import registry
-
-if TYPE_CHECKING and has_langchain:
-    from langchain.llms.base import BaseLLM  # type: ignore[import]
+from . import Backend
+from ...compat import has_langchain, langchain
+from ...registry import registry
 
 
 def _check_installation() -> None:
     """Checks whether `langchain` is installed. Raises an error otherwise."""
     if not has_langchain:
         raise ValueError(
             "The LangChain backend requires `langchain` to be installed, which it is not. See "
             "https://github.com/hwchase17/langchain for installation instructions."
         )
 
 
 @registry.llm_queries("spacy.CallLangChain.v1")
-def query_langchain() -> Callable[["BaseLLM", Iterable[Any]], Iterable[Any]]:
+def query_langchain() -> Callable[
+    ["langchain.llms.base.BaseLLM", Iterable[Any]], Iterable[Any]
+]:
     """Returns query Callable for LangChain.
     RETURNS (Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]:): Callable executing simple prompts on
         the specified LangChain backend.
     """
+    return _prompt_langchain
 
-    def prompt(backend: "BaseLLM", prompts: Iterable[Any]) -> Iterable[Any]:
-        return [backend(pr) for pr in prompts]
 
-    return prompt
+def _prompt_langchain(
+    backend: "langchain.llms.base.BaseLLM", prompts: Iterable[Any]
+) -> Iterable[Any]:
+    return [backend(pr) for pr in prompts]
 
 
 @registry.llm_backends("spacy.LangChain.v1")
 def backend_langchain(
     api: str,
-    query: Optional[Callable[["BaseLLM", Iterable[str]], Iterable[str]]] = None,
+    query: Optional[
+        Callable[["langchain.llms.base.BaseLLM", Iterable[str]], Iterable[str]]
+    ] = None,
     config: Dict[Any, Any] = SimpleFrozenDict(),
 ) -> Callable[[Iterable[Any]], Iterable[Any]]:
     """Returns Callable using MiniChain backend to prompt specified API.
     api (str): Name of any API/class in langchain.llms.type_to_cls_dict, e. g. "openai".
     query (Callable[["langchain.llms.BaseLLM", Iterable[str]], Iterable[str]]): Callable implementing querying this
         API.
     config (Dict[Any, Any]): LLM config arguments passed on to the initialization of the langchain.llms.BaseLLM
         instance.
     RETURNS (Callable[[Iterable[str]], Iterable[str]]]): Callable using the querying the specified API using the
         specified backend.
     """
     _check_installation()
 
+    if "model" not in config:
+        raise ValueError("The LLM model must be specified in the config.")
+
     # langchain.llms.type_to_cls_dict contains all API names in lowercase, so this allows to be more forgiving and make
     # "OpenAI" work as well "openai".
     api = api.lower()
-    type_to_cls_dict: Dict[str, Type[BaseLLM]] = langchain.llms.type_to_cls_dict
+    type_to_cls_dict: Dict[
+        str, Type[langchain.llms.base.BaseLLM]
+    ] = langchain.llms.type_to_cls_dict
 
     if api in type_to_cls_dict:
-        backend = type_to_cls_dict[api](**config)
-
-        query_fn = query_langchain() if query is None else query
-
-        def _query(prompts: Iterable[Any]) -> Iterable[Any]:
-            return query_fn(backend, prompts)
-
-        return _query
+        model = config.pop("model")
+        return Backend(
+            integration=type_to_cls_dict[api](model_name=model, **config),
+            query=query_langchain() if query is None else query,
+        )
     else:
         raise KeyError(
             f"The requested API {api} is not available in `langchain.llms.type_to_cls_dict`."
         )
```

### Comparing `spacy-llm-0.1.2/spacy_llm/backends/minichain.py` & `spacy-llm-0.2.0/spacy_llm/backends/integration/minichain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Callable, Dict, Iterable, Optional
 
 from spacy.util import SimpleFrozenDict
 
-from ..compat import has_minichain, minichain
-from ..registry import registry
+from . import Backend
+from ...compat import has_minichain, minichain
+from ...registry import registry
 
 
 def _check_installation() -> None:
     """Checks whether `minichain` is installed. Raises an error otherwise."""
     if not has_minichain:
         raise ValueError(
             "The MiniChain backend requires `minichain` to be installed, which it is not. See "
@@ -51,20 +52,19 @@
     config (Dict[Any, Any]): LLM config arguments passed on to the initialization of the minichain.Backend
         instance.
     RETURNS (Callable[[Iterable[str]], Iterable[str]]]): Callable querying the specified API using the
         specified backend.
     """
     _check_installation()
 
-    if hasattr(minichain.backend, api):
-        backend = getattr(minichain.backend, api)(**config)
-
-        query_fn = query_minichain() if query is None else query
-
-        def _query(prompts: Iterable[str]) -> Iterable[str]:
-            return query_fn(backend, prompts)
+    if "model" not in config:
+        raise ValueError("The LLM model must be specified in the config.")
 
-        return _query
+    if hasattr(minichain.backend, api):
+        return Backend(
+            integration=getattr(minichain.backend, api)(**config),
+            query=query_minichain() if query is None else query,
+        )
     else:
         raise KeyError(
             f"The requested API {api} is not available in `minichain.backend`."
         )
```

### Comparing `spacy-llm-0.1.2/spacy_llm/backends/rest/backend/noop.py` & `spacy-llm-0.2.0/spacy_llm/backends/rest/backend/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.2/spacy_llm/backends/rest/backend/openai.py` & `spacy-llm-0.2.0/spacy_llm/backends/rest/backend/openai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import os
 from enum import Enum
-from typing import Dict, Iterable, List, Union
+from typing import Any, Dict, Iterable, List, Sized
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
+from requests import HTTPError
 
 from .base import Backend
 
 
 class Endpoints(str, Enum):
-    chat = "https://api.openai.com/v1/chat/completions"
-    non_chat = "https://api.openai.com/v1/completions"
+    CHAT = "https://api.openai.com/v1/chat/completions"
+    NON_CHAT = "https://api.openai.com/v1/completions"
 
 
 class OpenAIBackend(Backend):
     @property
     def supported_models(self) -> Dict[str, str]:
         """Returns supported models with their endpoints.
         RETURNS (Dict[str, str]): Supported models with their endpoints.
         """
         return {
-            "gpt-4": Endpoints.chat.value,
-            "gpt-4-0314": Endpoints.chat.value,
-            "gpt-4-32k": Endpoints.chat.value,
-            "gpt-4-32k-0314": Endpoints.chat.value,
-            "gpt-3.5-turbo": Endpoints.chat.value,
-            "gpt-3.5-turbo-0301": Endpoints.chat.value,
-            "text-davinci-003": Endpoints.non_chat.value,
-            "text-davinci-002": Endpoints.non_chat.value,
-            "text-curie-001": Endpoints.non_chat.value,
-            "text-babbage-001": Endpoints.non_chat.value,
-            "text-ada-001": Endpoints.non_chat.value,
-            "davinci": Endpoints.non_chat.value,
-            "curie": Endpoints.non_chat.value,
-            "babbage": Endpoints.non_chat,
-            "ada": Endpoints.non_chat.value,
+            "gpt-4": Endpoints.CHAT.value,
+            "gpt-4-0314": Endpoints.CHAT.value,
+            "gpt-4-32k": Endpoints.CHAT.value,
+            "gpt-4-32k-0314": Endpoints.CHAT.value,
+            "gpt-3.5-turbo": Endpoints.CHAT.value,
+            "gpt-3.5-turbo-0301": Endpoints.CHAT.value,
+            "text-davinci-003": Endpoints.NON_CHAT.value,
+            "text-davinci-002": Endpoints.NON_CHAT.value,
+            "text-curie-001": Endpoints.NON_CHAT.value,
+            "text-babbage-001": Endpoints.NON_CHAT.value,
+            "text-ada-001": Endpoints.NON_CHAT.value,
+            "davinci": Endpoints.NON_CHAT.value,
+            "curie": Endpoints.NON_CHAT.value,
+            "babbage": Endpoints.NON_CHAT.value,
+            "ada": Endpoints.NON_CHAT.value,
         }
 
     @property
     def credentials(self) -> Dict[str, str]:
         model = self._config["model"]
         # Fetch and check the key
         api_key = os.getenv("OPENAI_API_KEY")
@@ -54,88 +55,113 @@
         # Even if the model is None, this call is used as a healthcheck to verify access.
         headers = {
             "Authorization": f"Bearer {api_key}",
         }
         if api_org:
             headers["OpenAI-Organization"] = api_org
         r = self.retry(
-            lambda: requests.get(
-                "https://api.openai.com/v1/models",
-                headers=headers,
-            ),
+            call_method=requests.get,
+            url="https://api.openai.com/v1/models",
+            headers=headers,
+            timeout=self._max_request_time,
         )
         if r.status_code == 422:
             raise ValueError(
                 "Could not access api.openai.com -- 422 permission denied."
                 "Visit https://platform.openai.com/account/api-keys to check your API keys."
             )
         elif r.status_code != 200:
             raise ValueError(
-                "Error accessing api.openai.com" f"{r.status_code}: {r.text}"
+                f"Error accessing api.openai.com ({r.status_code}): {r.text}"
             )
 
         response = r.json()["data"]
         models = [response[i]["id"] for i in range(len(response))]
         if model not in models:
             raise ValueError(
                 f"The specified model '{model}' is not available. Choices are: {sorted(set(models))}"
             )
 
         if model not in self.supported_models:
             raise ValueError(
                 f"The specified model '{model}' is not supported by the /v1/completions endpoint. "
                 f"Choices are: {sorted(list(self.supported_models))} ."
-                "(See OpenAI API documentation: https://platform.openai.com/docs/models/gpt-3)"
+                "(See OpenAI API documentation: https://platform.openai.com/docs/models/)"
+            )
+
+        # Ensure endpoint is supported.
+        url = self._url if self._url else self.supported_models[self._config["model"]]
+        if url not in (Endpoints.NON_CHAT, Endpoints.CHAT):
+            raise ValueError(
+                f"Endpoint {url} isn't supported. Please use one of: {Endpoints.CHAT}, {Endpoints.NON_CHAT}."
             )
 
         assert api_key is not None
         return headers
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "Content-Type": "application/json",
         }
         api_responses: List[str] = []
         prompts = list(prompts)
-
-        data: Dict[str, Union[List[str], List[Dict[str, str]]]] = {}
         url = self._url if self._url else self.supported_models[self._config["model"]]
-        if url == Endpoints.chat:
-            data = {
-                "messages": [{"role": "user", "content": prompt} for prompt in prompts]
-            }
-        elif url == Endpoints.non_chat:
-            data = {"prompt": prompts}
 
-        r = self.retry(
-            lambda: requests.post(
-                url,
+        def _request(json_data: Dict[str, Any]) -> Dict[str, Any]:
+            r = self.retry(
+                call_method=requests.post,
+                url=url,
                 headers=headers,
-                json={**data, **self._config},
-                timeout=self._timeout,
-            ),
-        )
-        r.raise_for_status()
-        responses = r.json()
-
-        # Process responses.
-        if "error" in responses:
-            if self._strict:
-                raise ValueError(f"API call failed: {responses}.")
-            else:
-                return [srsly.json_dumps(responses)] * len(prompts)
-        assert len(responses["choices"]) == len(prompts)
-
-        for prompt, response in zip(prompts, responses["choices"]):
-            if url == Endpoints.chat:
-                if "message" in response:
-                    api_responses.append(response["message"]["content"])
+                json={**json_data, **self._config},
+                timeout=self._max_request_time,
+            )
+            try:
+                r.raise_for_status()
+            except HTTPError as ex:
+                res_content = srsly.json_loads(r.content.decode("utf-8"))
+                # Include specific error message in exception.
+                raise ValueError(
+                    f"Request to OpenAI API failed: {res_content.get('error', {}).get('message', str(res_content))}"
+                ) from ex
+            responses = r.json()
+
+            if "error" in responses:
+                if self._strict:
+                    raise ValueError(f"API call failed: {responses}.")
                 else:
-                    api_responses.append(srsly.json_dumps(response))
-            elif url == Endpoints.non_chat:
+                    assert isinstance(prompts, Sized)
+                    return {"error": [srsly.json_dumps(responses)] * len(prompts)}
+
+            return responses
+
+        if url == Endpoints.CHAT:
+            # The OpenAI API doesn't support batching for /chat/completions yet, so we have to send individual requests.
+            for prompt in prompts:
+                responses = _request(
+                    {"messages": [{"role": "user", "content": prompt}]}
+                )
+                if "error" in responses:
+                    return responses["error"]
+
+                # Process responses.
+                assert len(responses["choices"]) == 1
+                response = responses["choices"][0]
+                api_responses.append(
+                    response.get("message", {}).get(
+                        "content", srsly.json_dumps(response)
+                    )
+                )
+
+        elif url == Endpoints.NON_CHAT:
+            responses = _request({"prompt": prompts})
+            if "error" in responses:
+                return responses["error"]
+            assert len(responses["choices"]) == len(prompts)
+
+            for response in responses["choices"]:
                 if "text" in response:
                     api_responses.append(response["text"])
                 else:
                     api_responses.append(srsly.json_dumps(response))
 
         return api_responses
```

### Comparing `spacy-llm-0.1.2/spacy_llm/backends/rest/registry.py` & `spacy-llm-0.2.0/spacy_llm/backends/rest/registry.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 
 
 @registry.llm_backends("spacy.REST.v1")
 def backend_rest(
     api: str,
     config: Dict[Any, Any] = SimpleFrozenDict(),
     strict: bool = True,
-    max_tries: int = 3,
-    timeout: int = 30,
+    max_tries: int = 5,
+    interval: float = 1.0,
+    max_request_time: float = 30,
 ) -> Callable[[Iterable[str]], Iterable[str]]:
     """Returns Callable using minimal REST backend to prompt specified API.
     api (str): Name of any API. Currently supported: "OpenAI".
     config (Dict[Any, Any]): LLM config arguments passed on to the initialization of the Backend instance.
     strict (bool): If True, ValueError is raised if the LLM API returns a malformed response (i. e. any kind of JSON
         or other response object that does not conform to the expectation of how a well-formed response object from
         this API should look like). If False, the API error responses are returned by __call__(), but no error will
         be raised.
     max_tries (int): Max. number of tries for API request.
-    timeout (int): Timeout for API request in seconds.
+    interval (float): Time interval (in seconds) for API retries in seconds. We implement a base 2 exponential backoff
+        at each retry.
+    max_request_time (float): Max. time (in seconds) to wait for request to terminate before raising an exception.
     RETURNS (Callable[[Iterable[str]], Iterable[str]]]): Callable using the querying the specified API using a
         Backend instance.
     """
 
     backend = supported_apis[api](
-        config=config, strict=strict, max_tries=max_tries, timeout=timeout
+        config=config,
+        strict=strict,
+        max_tries=max_tries,
+        interval=interval,
+        max_request_time=max_request_time,
     )
-
-    def _query(prompts: Iterable[str]) -> Iterable[str]:
-        return backend(prompts)
-
-    return _query
+    return backend
```

### Comparing `spacy-llm-0.1.2/spacy_llm/cache.py` & `spacy-llm-0.2.0/spacy_llm/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-import os
 from pathlib import Path
-from typing import Dict, Union, Optional, Iterable, List
+from typing import Dict, Iterable, List, Optional, Union
+import numpy
 
 import srsly  # type: ignore[import]
 from spacy.tokens import Doc, DocBin
 from spacy.vocab import Vocab
 
+from .registry import registry
 
-class Cache:
+
+@registry.llm_misc("spacy.BatchCache.v1")
+def make_cache(
+    path: Optional[Union[str, Path]],
+    batch_size: int,
+    max_batches_in_mem: int,
+):
+    return BatchCache(
+        path=path, batch_size=batch_size, max_batches_in_mem=max_batches_in_mem
+    )
+
+
+class BatchCache:
     """Utility class handling caching functionality for the `llm` component."""
 
     _INDEX_NAME: str = "index.jsonl"
 
     def __init__(
         self,
-        path: Union[str, Path],
+        path: Optional[Union[str, Path]],
         batch_size: int,
         max_batches_in_mem: int,
-        vocab: Vocab,
     ):
         """Initialize Cache instance.
-        path (Path): Cache directory.
+        path (Optional[Union[str,Path]]): Cache directory.
         batch_size (int): Number of docs in one batch (file).
         max_batches_in_mem (int): Max. number of batches to hold in memory.
-        vocab (Vocab): Vocab object.
         """
         self._path = Path(path) if path else None
 
         # Number of Docs in one batch.
         self._batch_size = batch_size
         # Max. number of batches to keep in memory.
         self.max_batches_in_mem = max_batches_in_mem
-        self._vocab = vocab
+        self._vocab: Optional[Vocab] = None
 
         # Stores doc hash -> batch hash to allow efficient lookup of available Docs.
         self._doc2batch: Dict[int, int] = {}
         # Hashes of batches loaded into memory.
         self._batch_hashes: List[int] = []
         # Container for currently loaded batch of Docs (batch hash -> doc hash -> Doc).
         self._loaded_docs: Dict[int, Dict[int, Doc]] = {}
@@ -47,20 +58,34 @@
             "missed": 0,
             "added": 0,
             "persisted": 0,
         }
 
         self._init_cache_index()
 
+    @property
+    def vocab(self) -> Optional[Vocab]:
+        """Vocab used for deserializing docs.
+        RETURNS (Vocab): Vocab used for deserializing docs.
+        """
+        return self._vocab
+
+    @vocab.setter
+    def vocab(self, vocab: Vocab) -> None:
+        """Set vocab to use for deserializing docs.
+        vocab (Vocab): Vocab to use for deserializing docs.
+        """
+        self._vocab = vocab
+
     def _init_cache_index(self) -> None:
         """Init cache index and directory."""
         if self._path is None:
             return
 
-        if self._path.exists() and not os.path.isdir(self._path):
+        if self._path.exists() and not self._path.is_dir():
             raise ValueError("Cache directory exists and is not a directory.")
         self._path.mkdir(parents=True, exist_ok=True)
 
         index_path = self._index_path
         if index_path.exists():
             for rec in srsly.read_jsonl(index_path):
                 self._doc2batch = {
@@ -70,15 +95,15 @@
 
     @property
     def _index_path(self) -> Path:
         """Returns full path to index file.
         RETURNS (Path): Full path to index file.
         """
         assert self._path is not None
-        return self._path / Cache._INDEX_NAME
+        return self._path / BatchCache._INDEX_NAME
 
     def _batch_path(self, batch_id: int) -> Path:
         """Returns full path to batch file.
         batch_id (int): Batch id/hash
         RETURNS (Path): Full path to batch file.
         """
         assert self._path is not None
@@ -86,23 +111,25 @@
 
     @staticmethod
     def _doc_id(doc: Doc) -> int:
         """Generate a unique ID for one doc.
         doc (Doc): Doc to generate a unique ID for.
         RETURN (int): Unique ID for this doc.
         """
-        return sum(token.orth for token in doc)
+        return numpy.sum(doc.to_array(["ORTH"]), dtype=numpy.uint64).item()
 
     @staticmethod
     def _batch_id(doc_ids: Iterable[int]) -> int:
         """Generate a unique ID for a batch, given a set of doc ids
         doc_ids (Iterable[int]): doc ids
         RETURN (int): Unique ID for this batch.
         """
-        return sum(doc_id for doc_id in doc_ids)
+        return numpy.sum(
+            numpy.asarray(doc_ids, dtype=numpy.uint64), dtype=numpy.uint64
+        ).item()
 
     def add(self, doc: Doc) -> None:
         """Adds processed doc. Note: Adding a doc does _not_ mean that this doc is immediately persisted to disk. This
         happens only after the specified batch size has been reached or _persist() has been called explicitly.
         doc (Doc): Doc to add to persistence queue.
         """
         if self._path is None:
@@ -112,21 +139,26 @@
         self._stats["added"] += 1
         if len(self._cache_queue) == self._batch_size:
             self._persist()
 
     def _persist(self) -> None:
         """Persists all processed docs in the queue to disk as one file."""
         assert self._path
-        doc_hashes = [self._doc_id(doc) for doc in self._cache_queue]
-        batch_id = self._batch_id(doc_hashes)
+
+        doc_ids = [self._doc_id(doc) for doc in self._cache_queue]
+        batch_id = self._batch_id(doc_ids)
+
+        for doc_id in doc_ids:
+            self._doc2batch[doc_id] = batch_id
+
         batch_path = self._batch_path(batch_id)
         DocBin(docs=self._cache_queue, store_user_data=True).to_disk(batch_path)
         srsly.write_jsonl(
             self._index_path,
-            lines=[{str(doc_hash): str(batch_id)} for doc_hash in doc_hashes],
+            lines=[{str(doc_id): str(batch_id)} for doc_id in doc_ids],
             append=True,
             append_new_line=False,
         )
         self._stats["persisted"] += len(self._cache_queue)
         self._cache_queue = []
 
     def __contains__(self, doc: Doc) -> bool:
@@ -158,14 +190,19 @@
 
         # Doc's batch is currently not loaded.
         if batch_id not in self._loaded_docs:
             if self._path is None:
                 raise ValueError(
                     "Cache directory path was not configured. Documents can't be read from cache."
                 )
+            if self._vocab is None:
+                raise ValueError(
+                    "Vocab must be set in order to Cache.__get_item__() to work."
+                )
+
             # Discard batch, if maximal number of batches would be exceeded otherwise.
             if len(self._loaded_docs) == self.max_batches_in_mem:
                 self._loaded_docs.pop(self._batch_hashes[0])
                 self._batch_hashes = self._batch_hashes[1:]
 
             # Load target batch.
             self._batch_hashes.append(batch_id)
```

### Comparing `spacy-llm-0.1.2/spacy_llm/compat.py` & `spacy-llm-0.2.0/spacy_llm/compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # mypy: ignore-errors
 import sys
-import os
 
 if sys.version_info[:2] >= (3, 8):  # Python 3.8+
     from typing import Protocol, runtime_checkable, Literal
 else:
     from typing_extensions import Protocol, runtime_checkable, Literal  # noqa: F401
 
+if sys.version_info[:2] >= (3, 9):  # Python 3.8+
+    from typing import TypedDict  # noqa: F401
+else:
+    from typing_extensions import TypedDict  # noqa: F401
+
 try:
     import langchain
 
     has_langchain = True
 except (ImportError, AttributeError):
     langchain = None
     has_langchain = False
@@ -42,12 +46,7 @@
 try:
     import accelerate
 
     has_accelerate = True
 except ImportError:
     accelerate = None
     has_accelerate = False
-
-if os.getenv("OPENAI_API_KEY") is None:
-    has_openai_key = False
-else:
-    has_openai_key = True
```

### Comparing `spacy-llm-0.1.2/spacy_llm/registry/normalizer.py` & `spacy-llm-0.2.0/spacy_llm/registry/normalizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 @registry.misc("spacy.StripNormalizer.v1")
 def strip_normalizer() -> Callable[[str], str]:
     """Return the labels as-is with stripped whitespaces
 
     RETURNS (Callable[[str], str])
     """
+    return _strip
 
-    def noop(s: str) -> str:
-        return s.strip()
 
-    return noop
+def _strip(s: str) -> str:
+    return s.strip()
 
 
 @registry.misc("spacy.LowercaseNormalizer.v1")
 def lowercase_normalizer() -> Callable[[str], str]:
     """Return lowercase versions of the labels
 
     RETURNS (Callable[[str], str])
     """
+    return _lowercase_strip
 
-    def lowercase(s: str) -> str:
-        return s.strip().lower()
 
-    return lowercase
+def _lowercase_strip(s: str) -> str:
+    return s.strip().lower()
```

### Comparing `spacy-llm-0.1.2/spacy_llm/registry/reader.py` & `spacy-llm-0.2.0/spacy_llm/registry/reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,51 @@
+import functools
 from pathlib import Path
-from typing import Any, Callable, Iterable, Union
+from typing import Any, Callable, Dict, Iterable, Union, cast
 
 import srsly
 
-from .util import registry
 
+def file_reader(path: Union[str, Path]) -> str:
+    """Read a file from a path and return its contents.
 
-@registry.misc("spacy.FewShotReader.v1")
-def fewshot_reader(path: Union[str, Path]) -> Callable[[], Iterable[Any]]:
+    path (Union[str, Path]): path to the file
+
+    RETURNS (str): the contents of the file
+    """
+    tpl_path = Path(path) if isinstance(path, str) else path
+    with tpl_path.open("r", encoding="utf8") as tpl_file:
+        tpl_text = tpl_file.read()
+
+    return tpl_text
+
+
+def fewshot_reader(path: Union[str, Path]) -> Callable[[], Iterable[Dict[str, Any]]]:
     """Read a file containing examples to include in few-shot learning
 
     path (Union[str,Path]): path to an examples file (.yml, .yaml, .json, .jsonl)
 
-    RETURNS (Iterable[Any]): an iterable of examples to be parsed by the template
+    RETURNS (Iterable[Dict[str, Any]]): an iterable of examples to be parsed by the template
     """
-
-    # typecast string path so that we can use pathlib functionality
     eg_path = Path(path) if isinstance(path, str) else path
+    return functools.partial(_fewshot_reader, eg_path=eg_path)
 
-    def reader() -> Iterable[Any]:
-        if eg_path is None:
-            data = []
-        elif eg_path.suffix in (".yml", ".yaml"):
-            data = srsly.read_yaml(eg_path)
-        elif eg_path.suffix == ".json":
-            data = srsly.read_json(eg_path)
-        elif eg_path.suffix == ".jsonl":
-            data = list(srsly.read_jsonl(eg_path))
-        else:
-            raise ValueError(
-                "The examples file expects a .yml, .yaml, .json, or .jsonl file type."
-            )
-
-        if not isinstance(data, list):
-            raise ValueError(
-                f"Cannot interpret prompt examples from {path}. Please check your formatting"
-            )
-        return data
 
-    return reader
+def _fewshot_reader(eg_path: Path) -> Iterable[Any]:
+    if eg_path is None:
+        data = []
+    elif eg_path.suffix in (".yml", ".yaml"):
+        data = srsly.read_yaml(eg_path)
+    elif eg_path.suffix == ".json":
+        data = srsly.read_json(eg_path)
+    elif eg_path.suffix == ".jsonl":
+        data = list(srsly.read_jsonl(eg_path))
+    else:
+        raise ValueError(
+            "The examples file expects a .yml, .yaml, .json, or .jsonl file type."
+        )
+
+    if not isinstance(data, list) or not all(isinstance(d, dict) for d in data):
+        raise ValueError(
+            f"Cannot interpret prompt examples from {str(eg_path)}. Please check your formatting"
+        )
+    return cast(Iterable[Dict[str, Any]], data)
```

### Comparing `spacy-llm-0.1.2/spacy_llm/tasks/textcat.py` & `spacy-llm-0.2.0/spacy_llm/tasks/textcat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-from typing import Any, Callable, Dict, Iterable, Optional
+from typing import Callable, Dict, List, Iterable, Optional
 
 import jinja2
 from pydantic import BaseModel
 from spacy.tokens import Doc
 from wasabi import msg
 
 from ..registry import lowercase_normalizer, registry
+from ..ty import ExamplesConfigType
+from ..util import split_labels
+from .templates import read_template
+
+
+_DEFAULT_TEXTCAT_TEMPLATE_v1 = read_template("textcat")
+_DEFAULT_TEXTCAT_TEMPLATE_v2 = read_template("textcat.v2")
 
 
 class TextCatExample(BaseModel):
     text: str
     answer: str
 
 
 @registry.llm_tasks("spacy.TextCat.v1")
-class TextCatTask:
-    _TEMPLATE_STR = """
-{%- if labels|length == 1 -%}
-{%- set label = labels[0] -%}
-Classify whether the text below belongs to the {{ label }} category or not.
-If it is a {{ label }}, answer `POS`. If it is not a {{ label }}, answer `NEG`.
-{%- else -%}
-Classify the text below to any of the following labels: {{ labels|join(", ") }}
-{# whitespace #}
-{%- if exclusive_classes -%}
-The task is exclusive, so only choose one label from what I provided.
-{%- else -%}
-The task is non-exclusive, so you can provide more than one label as long as
-they're comma-delimited. For example: Label1, Label2, Label3.
-{%- if allow_none -%}
-{# whitespace #}
-If the text cannot be classified into any of the provided labels, answer `==NONE==`.
-{%- endif -%}
-{%- endif -%}
-{# whitespace #}
-{%- endif -%}
-{# whitespace #}
-{%- if examples -%}
-{# whitespace #}
-Below are some examples (only use these as a guide):
-{# whitespace #}
-{# whitespace #}
-{%- for example in examples -%}
-{# whitespace #}
-Text:
-'''
-{{ example.text }}
-'''
-{# whitespace #}
-{{ example.answer }}
-{# whitespace #}
-{%- endfor -%}
-{%- endif -%}
-{# whitespace #}
-{# whitespace #}
-Here is the text that needs classification
-{# whitespace #}
-{# whitespace #}
-Text:
-'''
-{{ text }}
-'''
-    """
+def make_textcat_task(
+    labels: str,
+    examples: ExamplesConfigType = None,
+    normalizer: Optional[Callable[[str], str]] = None,
+    exclusive_classes: bool = False,
+    allow_none: bool = True,
+    verbose: bool = False,
+) -> "TextCatTask":
+    labels_list = split_labels(labels)
+    raw_examples = examples() if callable(examples) else examples
+    textcat_examples = (
+        [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
+    )
+    return TextCatTask(
+        labels=labels_list,
+        template=_DEFAULT_TEXTCAT_TEMPLATE_v1,
+        examples=textcat_examples,
+        normalizer=normalizer,
+        exclusive_classes=exclusive_classes,
+        allow_none=allow_none,
+        verbose=verbose,
+    )
+
+
+@registry.llm_tasks("spacy.TextCat.v2")
+def make_textcat_task_v2(
+    labels: str,
+    template: str = _DEFAULT_TEXTCAT_TEMPLATE_v2,
+    examples: ExamplesConfigType = None,
+    normalizer: Optional[Callable[[str], str]] = None,
+    exclusive_classes: bool = False,
+    allow_none: bool = True,
+    verbose: bool = False,
+) -> "TextCatTask":
+    labels_list = split_labels(labels)
+    raw_examples = examples() if callable(examples) else examples
+    textcat_examples = (
+        [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
+    )
+    return TextCatTask(
+        labels=labels_list,
+        template=template,
+        examples=textcat_examples,
+        normalizer=normalizer,
+        exclusive_classes=exclusive_classes,
+        allow_none=allow_none,
+        verbose=verbose,
+    )
 
+
+class TextCatTask:
     def __init__(
         self,
-        labels: str,
-        examples: Optional[Callable[[], Iterable[Any]]] = None,
+        labels: List[str],
+        template: str = _DEFAULT_TEXTCAT_TEMPLATE_v2,
+        examples: Optional[List[TextCatExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         exclusive_classes: bool = False,
         allow_none: bool = True,
         verbose: bool = False,
     ):
         """Default TextCat task.
 
@@ -85,30 +95,28 @@
         dictionary of strings and their score.
 
         Lastly, you can toggle between exclusive or no-exclusive text
         categorization by passing a flag to the `exclusive_classes` parameter.
 
         labels (str): Comma-separated list of labels to pass to the template. This task
             assumes binary classification if a single label is provided.
+        template (str): Prompt template passed to the model.
         examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): Optional normalizer function.
         exclusive_classes (bool): If True, require the language model to suggest only one
             label per class. This is automatically set when using binary classification.
         allow_none (bool): if True, there might be cases where no label is applicable.
         verbose (bool): If True, show extra information.
         """
+        self._template = template
         self._normalizer = normalizer if normalizer else lowercase_normalizer()
-        self._label_dict = {
-            self._normalizer(label): label for label in labels.split(",")
-        }
-        self._examples = (
-            [TextCatExample(**eg) for eg in examples()] if examples else None
-        )
+        self._label_dict = {self._normalizer(label): label for label in labels}
+        self._examples = examples
         # Textcat configuration
         self._use_binary = True if len(self._label_dict) == 1 else False
         self._exclusive_classes = exclusive_classes
         self._allow_none = allow_none
         self._verbose = verbose
 
         if self._use_binary and not self._exclusive_classes:
@@ -116,15 +124,15 @@
                 "Binary classification should always be exclusive. Setting "
                 "the `exclusive_classes` parameter to True."
             )
             self._exclusive_classes = True
 
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
-        _template = environment.from_string(self._TEMPLATE_STR)
+        _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
                 examples=self._examples,
                 exclusive_classes=self._exclusive_classes,
                 allow_none=self._allow_none,
```

### Comparing `spacy-llm-0.1.2/spacy_llm/tests/backends/test_dolly.py` & `spacy-llm-0.2.0/spacy_llm/tests/backends/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.2/spacy_llm/tests/backends/test_langchain.py` & `spacy-llm-0.2.0/spacy_llm/tests/backends/test_minichain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import spacy
 import pytest
-
-from spacy_llm.compat import has_langchain
+from spacy_llm.compat import has_minichain
 
 PIPE_CFG = {
     "backend": {
-        "@llm_backends": "spacy.LangChain.v1",
+        "@llm_backends": "spacy.MiniChain.v1",
         "api": "OpenAI",
-        "config": {"temperature": 0.3},
-        "query": {"@llm_queries": "spacy.CallLangChain.v1"},
+        "config": {"model": "gpt-3.5-turbo"},
+        "query": {"@llm_queries": "spacy.RunMiniChain.v1"},
     },
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
 }
 
 
 @pytest.mark.external
-@pytest.mark.skipif(has_langchain is False, reason="LangChain is not installed")
+@pytest.mark.skipif(has_minichain is False, reason="MiniChain is not installed")
 def test_initialization():
     """Test initialization and simple run"""
     nlp = spacy.blank("en")
     nlp.add_pipe("llm", config=PIPE_CFG)
     nlp("This is a test.")
```

### Comparing `spacy-llm-0.1.2/spacy_llm/tests/conftest.py` & `spacy-llm-0.2.0/spacy_llm/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import os
+
 import pytest
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--external",
         action="store_true",
-        default=False,
+        default=bool(int(os.environ.get("TEST_EXTERNAL", 0))),
         help="include tests that connects to third-party API",
     )
 
 
 def pytest_runtest_setup(item):
     def getopt(opt):
         return item.config.getoption(f"--{opt}", False)
```

### Comparing `spacy-llm-0.1.2/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.2.0/spacy_llm/tests/tasks/test_spancat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# mypy: ignore-errors
 from pathlib import Path
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import strip_normalizer, lowercase_normalizer, fewshot_reader
-from spacy_llm.tasks.ner import find_substrings, NERTask
-from spacy_llm.compat import has_openai_key
+from spacy_llm.registry import fewshot_reader, lowercase_normalizer, strip_normalizer
+from spacy_llm.tasks import make_spancat_task_v2
+from spacy_llm.tasks.util import find_substrings
+
+from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 
 
 @pytest.fixture
 def zeroshot_cfg_string():
     return """
@@ -25,15 +26,15 @@
 
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
-    @llm_tasks = "spacy.NER.v1"
+    @llm_tasks = "spacy.SpanCat.v2"
     labels = PER,ORG,LOC
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
 
     [components.llm.backend]
     @llm_backends = "spacy.REST.v1"
@@ -52,15 +53,15 @@
 
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
-    @llm_tasks = "spacy.NER.v1"
+    @llm_tasks = "spacy.SpanCat.v2"
     labels = PER,ORG,LOC
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
     path = {str((Path(__file__).parent / "examples" / "ner_examples.yml"))}
 
     [components.llm.task.normalizer]
@@ -69,55 +70,56 @@
     [components.llm.backend]
     @llm_backends = "spacy.REST.v1"
     api = "OpenAI"
     config: {{}}
     """
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
-@pytest.mark.parametrize("cfg_string", ["fewshot_cfg_string"])  # "zeroshot_cfg_string",
-def test_ner_config(cfg_string, request):
+@pytest.mark.parametrize("cfg_string", ["fewshot_cfg_string", "zeroshot_cfg_string"])
+def test_spancat_config(cfg_string, request):
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
 @pytest.mark.external
 @pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
-def test_ner_predict(cfg_string, request):
+def test_spancat_predict(cfg_string, request):
     """Use OpenAI to get zero-shot NER results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed to be consistent/predictable
     """
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     text = "Marc and Bob both live in Ireland."
     doc = nlp(text)
-    assert len(doc.ents) > 0
-    for ent in doc.ents:
+    assert len(doc.spans["sc"]) > 0
+    for ent in doc.spans["sc"]:
         assert ent.label_ in ["PER", "ORG", "LOC"]
 
 
 @pytest.mark.external
 @pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
-def test_ner_io(cfg_string, request):
+def test_spancat_io(cfg_string, request):
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
     # ensure you can save a pipeline to disk and run it after loading
     with make_tempdir() as tmpdir:
         nlp.to_disk(tmpdir)
         nlp2 = spacy.load(tmpdir)
     assert nlp2.pipe_names == ["llm"]
     text = "Marc and Bob both live in Ireland."
     doc = nlp2(text)
-    assert len(doc.ents) > 0
-    for ent in doc.ents:
+    assert len(doc.spans["sc"]) > 0
+    for ent in doc.spans["sc"]:
         assert ent.label_ in ["PER", "ORG", "LOC"]
 
 
 @pytest.mark.parametrize(
     "text,input_strings,result_strings,result_offsets",
     [
         (
@@ -149,51 +151,55 @@
     # those strings first from the text
     assert result_offsets == offsets
     found_substrings = [text[start:end] for start, end in offsets]
     assert result_strings == found_substrings
 
 
 @pytest.mark.parametrize(
-    "text,response,gold_ents",
+    "text,response,gold_spans",
     [
         # simple
         (
             "Jean Jacques and Jaime went to the library.",
             "PER: Jean Jacques, Jaime\nLOC: library",
             [("Jean Jacques", "PER"), ("Jaime", "PER"), ("library", "LOC")],
         ),
-        # overlapping: should only return the longest span
+        # overlapping: should only return all spans
         (
             "The Manila Observatory was founded in 1865.",
             "LOC: The Manila Observatory, Manila, Manila Observatory",
-            [("The Manila Observatory", "LOC")],
+            [
+                ("The Manila Observatory", "LOC"),
+                ("Manila", "LOC"),
+                ("Manila Observatory", "LOC"),
+            ],
         ),
         # flipped: order shouldn't matter
         (
             "Take the road from Downtown and turn left at the public market.",
             "LOC: public market, Downtown",
             [("Downtown", "LOC"), ("public market", "LOC")],
         ),
     ],
 )
-def test_ner_zero_shot_task(text, response, gold_ents):
+def test_spancat_zero_shot_task(text, response, gold_spans):
     labels = "PER,ORG,LOC"
-    llm_ner = NERTask(labels=labels)
+    llm_spancat = make_spancat_task_v2(labels=labels)
     # Prepare doc
     nlp = spacy.blank("xx")
     doc_in = nlp.make_doc(text)
     # Pass to the parser
     # Note: parser() returns a list so we get what's inside
-    doc_out = list(llm_ner.parse_responses([doc_in], [response]))[0]
-    pred_ents = [(ent.text, ent.label_) for ent in doc_out.ents]
-    assert pred_ents == gold_ents
+    doc_out = list(llm_spancat.parse_responses([doc_in], [response]))[0]
+    pred_spans = [(span.text, span.label_) for span in doc_out.spans["sc"]]
+    assert pred_spans == gold_spans
 
 
 @pytest.mark.parametrize(
-    "response,normalizer,gold_ents",
+    "response,normalizer,gold_spans",
     [
         (
             "PER: Jean Jacques, Jaime",
             None,
             [("Jean Jacques", "PER"), ("Jaime", "PER")],
         ),
         (
@@ -229,30 +235,30 @@
         (
             "per: Jean Jacques, Jaime\nRANDOM: library",
             lowercase_normalizer(),
             [("Jean Jacques", "PER"), ("Jaime", "PER")],
         ),
     ],
 )
-def test_ner_labels(response, normalizer, gold_ents):
+def test_spancat_labels(response, normalizer, gold_spans):
     text = "Jean Jacques and Jaime went to the library."
     labels = "PER,ORG,LOC"
-    llm_ner = NERTask(labels=labels, normalizer=normalizer)
+    llm_spancat = make_spancat_task_v2(labels=labels, normalizer=normalizer)
     # Prepare doc
     nlp = spacy.blank("xx")
     doc_in = nlp.make_doc(text)
     # Pass to the parser
     # Note: parser() returns a list
-    doc_out = list(llm_ner.parse_responses([doc_in], [response]))[0]
-    pred_ents = [(ent.text, ent.label_) for ent in doc_out.ents]
-    assert pred_ents == gold_ents
+    doc_out = list(llm_spancat.parse_responses([doc_in], [response]))[0]
+    pred_spans = [(span.text, span.label_) for span in doc_out.spans["sc"]]
+    assert pred_spans == gold_spans
 
 
 @pytest.mark.parametrize(
-    "response,alignment_mode,gold_ents",
+    "response,alignment_mode,gold_spans",
     [
         (
             "PER: Jacq",
             "strict",
             [],
         ),
         (
@@ -278,36 +284,36 @@
         (
             "PER: random",
             "expand",
             [],
         ),
     ],
 )
-def test_ner_alignment(response, alignment_mode, gold_ents):
+def test_spancat_alignment(response, alignment_mode, gold_spans):
     text = "Jean Jacques and Jaime went to the library."
     labels = "PER,ORG,LOC"
-    llm_ner = NERTask(labels=labels, alignment_mode=alignment_mode)
+    llm_spancat = make_spancat_task_v2(labels=labels, alignment_mode=alignment_mode)
     # Prepare doc
     nlp = spacy.blank("xx")
     doc_in = nlp.make_doc(text)
     # Pass to the parser
     # Note: parser() returns a list
-    doc_out = list(llm_ner.parse_responses([doc_in], [response]))[0]
-    pred_ents = [(ent.text, ent.label_) for ent in doc_out.ents]
-    assert pred_ents == gold_ents
+    doc_out = list(llm_spancat.parse_responses([doc_in], [response]))[0]
+    pred_spans = [(span.text, span.label_) for span in doc_out.spans["sc"]]
+    assert pred_spans == gold_spans
 
 
 def test_invalid_alignment_mode():
     labels = "PER,ORG,LOC"
     with pytest.raises(ValueError, match="Unsupported alignment mode 'invalid"):
-        NERTask(labels=labels, alignment_mode="invalid")
+        make_spancat_task_v2(labels=labels, alignment_mode="invalid")
 
 
 @pytest.mark.parametrize(
-    "response,case_sensitive,single_match,gold_ents",
+    "response,case_sensitive,single_match,gold_spans",
     [
         (
             "PER: Jean",
             False,
             False,
             [("jean", "PER"), ("Jean", "PER"), ("Jean", "PER")],
         ),
@@ -327,51 +333,55 @@
             "PER: Jean",
             True,
             True,
             [("Jean", "PER")],
         ),
     ],
 )
-def test_ner_matching(response, case_sensitive, single_match, gold_ents):
+def test_spancat_matching(response, case_sensitive, single_match, gold_spans):
     text = "This guy jean (or Jean) is the president of the Jean Foundation."
     labels = "PER,ORG,LOC"
-    llm_ner = NERTask(
+    llm_spancat = make_spancat_task_v2(
         labels=labels, case_sensitive_matching=case_sensitive, single_match=single_match
     )
     # Prepare doc
     nlp = spacy.blank("xx")
     doc_in = nlp.make_doc(text)
     # Pass to the parser
     # Note: parser() returns a list
-    doc_out = list(llm_ner.parse_responses([doc_in], [response]))[0]
-    pred_ents = [(ent.text, ent.label_) for ent in doc_out.ents]
-    assert pred_ents == gold_ents
+    doc_out = list(llm_spancat.parse_responses([doc_in], [response]))[0]
+    pred_spans = [(span.text, span.label_) for span in doc_out.spans["sc"]]
+    assert pred_spans == gold_spans
 
 
 def test_jinja_template_rendering_without_examples():
     """Test if jinja template renders as we expected
 
     We apply the .strip() method for each prompt so that we don't have to deal
     with annoying newlines and spaces at the edge of the text.
     """
     labels = "PER,ORG,LOC"
     nlp = spacy.blank("xx")
     doc = nlp.make_doc("Alice and Bob went to the supermarket")
 
-    llm_ner = NERTask(labels=labels, examples=None)
-    prompt = list(llm_ner.generate_prompts([doc]))[0]
+    llm_spancat = make_spancat_task_v2(labels=labels, examples=None)
+    prompt = list(llm_spancat.generate_prompts([doc]))[0]
 
     assert (
         prompt.strip()
         == """
-From the text below, extract the following entities in the following format:
+You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
+The entities you extract for each label can overlap with each other.
+From the Text input provided, extract named entities for each label in the following format:
+
 PER: <comma delimited list of strings>
 ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
 
+
 Here is the text that needs labeling:
 
 Text:
 '''
 Alice and Bob went to the supermarket
 '''
 """.strip()
@@ -393,47 +403,51 @@
     with annoying newlines and spaces at the edge of the text.
     """
     labels = "PER,ORG,LOC"
     nlp = spacy.blank("xx")
     doc = nlp.make_doc("Alice and Bob went to the supermarket")
 
     examples = fewshot_reader(examples_path)
-    llm_ner = NERTask(labels=labels, examples=examples)
-    prompt = list(llm_ner.generate_prompts([doc]))[0]
+    llm_spancat = make_spancat_task_v2(labels=labels, examples=examples)
+    prompt = list(llm_spancat.generate_prompts([doc]))[0]
 
     assert (
         prompt.strip()
         == """
-From the text below, extract the following entities in the following format:
+You are an expert Named Entity Recognition (NER) system. Your task is to accept Text as input and extract named entities for the set of predefined entity labels.
+The entities you extract for each label can overlap with each other.
+From the Text input provided, extract named entities for each label in the following format:
+
 PER: <comma delimited list of strings>
 ORG: <comma delimited list of strings>
 LOC: <comma delimited list of strings>
 
-Below are some examples (only use these as a guide):
 
+Below are some examples (only use these as a guide):
 
 Text:
 '''
 Jack and Jill went up the hill.
 '''
+
 PER: Jack, Jill
 LOC: hill
 
-
 Text:
 '''
 Jack fell down and broke his crown.
 '''
-PER: Jack
 
+PER: Jack
 
 Text:
 '''
 Jill came tumbling after.
 '''
+
 PER: Jill
 
 
 Here is the text that needs labeling:
 
 Text:
 '''
@@ -451,8 +465,10 @@
         }
     ]
     with make_tempdir() as tmpdir:
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
         with pytest.raises(ValidationError):
-            NERTask(labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path))
+            make_spancat_task_v2(
+                labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path)
+            )
```

### Comparing `spacy-llm-0.1.2/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.2.0/spacy_llm/tests/tasks/test_textcat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# mypy: ignore-errors
 from pathlib import Path
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import lowercase_normalizer, fewshot_reader
-from spacy_llm.tasks.textcat import TextCatTask
-from spacy_llm.compat import has_openai_key
+from spacy_llm.registry import lowercase_normalizer
+from spacy_llm.registry import fewshot_reader, file_reader
+from spacy_llm.tasks.textcat import make_textcat_task_v2
 
+from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
+TEMPLATES_DIR = Path(__file__).parent / "templates"
 
 
 @pytest.fixture
 def zeroshot_cfg_string():
     return """
     [nlp]
     lang = "en"
@@ -73,14 +74,48 @@
     @llm_backends = "spacy.REST.v1"
     api = "OpenAI"
     config = {{}}
     """
 
 
 @pytest.fixture
+def ext_template_cfg_string():
+    """Simple zero-shot config with an external template"""
+
+    return f"""
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+    batch_size = 128
+
+    [components]
+
+    [components.llm]
+    factory = "llm"
+
+    [components.llm.task]
+    @llm_tasks = "spacy.TextCat.v2"
+    labels = "Recipe"
+    exclusive_classes = true
+
+    [components.llm.task.template]
+    @misc = "spacy.FileReader.v1"
+    path = {str((Path(__file__).parent / "templates" / "textcat_template.jinja2"))}
+
+    [components.llm.task.normalizer]
+    @misc = "spacy.LowercaseNormalizer.v1"
+
+    [components.llm.backend]
+    @llm_backends = "spacy.REST.v1"
+    api = "OpenAI"
+    config = {{}}
+    """
+
+
+@pytest.fixture
 def binary():
     text = "Get 1 cup of sugar, half a cup of butter, and mix them together to make a cream"
     labels = "Recipe"
     gold_cats = ["Recipe"]
     exclusive_classes = True
     examples_path = str(EXAMPLES_DIR / "textcat_binary_examples.yml")
     return text, labels, gold_cats, exclusive_classes, examples_path
@@ -102,17 +137,24 @@
     labels = "Recipe,Feedback,Comment"
     gold_cats = ["Recipe", "Feedback", "Comment"]
     exclusive_classes = False
     examples_path = str(EXAMPLES_DIR / "textcat_multi_nonexcl_examples.yml")
     return text, labels, gold_cats, exclusive_classes, examples_path
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
-@pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
-@pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
+@pytest.mark.parametrize(
+    "task",
+    ["binary", "multilabel_nonexcl", "multilabel_excl"],
+)
+@pytest.mark.parametrize(
+    "cfg_string",
+    ["zeroshot_cfg_string", "fewshot_cfg_string", "ext_template_cfg_string"],
+)
 def test_textcat_config(task, cfg_string, request):
     """Simple test to check if the config loads properly given different settings"""
 
     task = request.getfixturevalue(task)
     _, labels, _, exclusive_classes, examples = task
     overrides = {
         "components.llm.task.labels": labels,
@@ -125,20 +167,24 @@
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string, overrides=overrides)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
 @pytest.mark.external
+@pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
-@pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
+@pytest.mark.parametrize(
+    "cfg_string",
+    ["zeroshot_cfg_string", "fewshot_cfg_string", "ext_template_cfg_string"],
+)
 def test_textcat_predict(task, cfg_string, request):
-    """Use OpenAI to get zero-shot Textcat results
+    """Use OpenAI to get Textcat results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed
-    to be consistent/predictable
+    to be consistent/predictable.
     """
     task = request.getfixturevalue(task)
     text, labels, gold_cats, exclusive_classes, examples = task
     overrides = {
         "components.llm.task.labels": labels,
         "components.llm.task.exclusive_classes": exclusive_classes,
     }
@@ -152,16 +198,20 @@
     doc = nlp(text)
     assert len(doc.cats) >= 0  # can be 0 if binary and negative
     for cat in list(doc.cats.keys()):
         assert cat in gold_cats
 
 
 @pytest.mark.external
+@pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
-@pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
+@pytest.mark.parametrize(
+    "cfg_string",
+    ["zeroshot_cfg_string", "fewshot_cfg_string", "ext_template_cfg_string"],
+)
 def test_textcat_io(task, cfg_string, request):
     task = request.getfixturevalue(task)
     text, labels, gold_cats, exclusive_classes, examples = task
     overrides = {
         "components.llm.task.labels": labels,
         "components.llm.task.exclusive_classes": exclusive_classes,
     }
@@ -183,15 +233,15 @@
     assert len(doc.cats) >= 0  # can be 0 if binary and negative
     for cat in list(doc.cats.keys()):
         assert cat in gold_cats
 
 
 def test_textcat_sets_exclusive_classes_if_binary():
     """Test if the textcat task automatically sets exclusive classes to True if binary"""
-    llm_textcat = TextCatTask(labels="Recipe", exclusive_classes=False)
+    llm_textcat = make_textcat_task_v2(labels="Recipe", exclusive_classes=False)
     assert llm_textcat._exclusive_classes
 
 
 @pytest.mark.parametrize(
     "text,response,expected_score",
     [
         ("Some test text with positive response", "POS", 1.0),
@@ -204,15 +254,15 @@
     ],
 )
 def test_textcat_binary_labels_are_correct(text, response, expected_score):
     """Test if positive label for textcat binary is always the label name and the negative
     label is an empty dictionary
     """
     label = "Recipe"
-    llm_textcat = TextCatTask(
+    llm_textcat = make_textcat_task_v2(
         labels=label, exclusive_classes=True, normalizer=lowercase_normalizer()
     )
 
     nlp = spacy.blank("xx")
     doc = nlp(text)
     pred = list(llm_textcat.parse_responses([doc], [response]))[0]
     assert list(pred.cats.keys())[0] == label
@@ -235,15 +285,15 @@
         # fmt: on
     ],
 )
 def test_textcat_multilabel_labels_are_correct(
     text, exclusive_classes, response, expected
 ):
     labels = "Recipe,Comment,Feedback"
-    llm_textcat = TextCatTask(
+    llm_textcat = make_textcat_task_v2(
         labels=labels,
         exclusive_classes=exclusive_classes,
         normalizer=lowercase_normalizer(),
     )
     nlp = spacy.blank("xx")
     doc = nlp.make_doc(text)
     pred = list(llm_textcat.parse_responses([doc], [response]))[0]
@@ -267,25 +317,29 @@
     with annoying newlines and spaces at the edge of the text.
     """
     text, labels, _, exclusive_classes, _ = binary
     nlp = spacy.blank("xx")
     doc = nlp(text)
 
     examples = fewshot_reader(examples_path)
-    llm_textcat = TextCatTask(
+    llm_textcat = make_textcat_task_v2(
         labels=labels,
         examples=examples,
         exclusive_classes=exclusive_classes,
     )
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
 Classify whether the text below belongs to the Recipe category or not.
 If it is a Recipe, answer `POS`. If it is not a Recipe, answer `NEG`.
+Do not put any other text in your answer, only one of 'POS' or 'NEG' with nothing before or after.
 Below are some examples (only use these as a guide):
 
 
 Text:
 '''
 Macaroni and cheese is the best budget meal for students, unhealthy tho
 '''
@@ -329,25 +383,29 @@
     examples_path, multilabel_excl
 ):
     text, labels, _, exclusive_classes, _ = multilabel_excl
     nlp = spacy.blank("xx")
     doc = nlp(text)
 
     examples = fewshot_reader(examples_path)
-    llm_textcat = TextCatTask(
+    llm_textcat = make_textcat_task_v2(
         labels=labels,
         examples=examples,
         exclusive_classes=exclusive_classes,
     )
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
 Classify the text below to any of the following labels: Recipe, Feedback, Comment
 The task is exclusive, so only choose one label from what I provided.
+Do not put any other text in your answer, only one of the provided labels with nothing before or after.
 Below are some examples (only use these as a guide):
 
 
 Text:
 '''
 Macaroni and cheese is the best budget meal for students, unhealthy tho
 '''
@@ -391,26 +449,30 @@
     examples_path, multilabel_nonexcl
 ):
     text, labels, _, exclusive_classes, _ = multilabel_nonexcl
     nlp = spacy.blank("xx")
     doc = nlp(text)
 
     examples = fewshot_reader(examples_path)
-    llm_textcat = TextCatTask(
+    llm_textcat = make_textcat_task_v2(
         labels=labels,
         examples=examples,
         exclusive_classes=exclusive_classes,
     )
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
-    Classify the text below to any of the following labels: Recipe, Feedback, Comment
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
+Classify the text below to any of the following labels: Recipe, Feedback, Comment
 The task is non-exclusive, so you can provide more than one label as long as
 they're comma-delimited. For example: Label1, Label2, Label3.
+Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
 If the text cannot be classified into any of the provided labels, answer `==NONE==`.
 Below are some examples (only use these as a guide):
 
 
 Text:
 '''
 Macaroni and cheese is the best budget meal for students, unhealthy tho
@@ -455,12 +517,32 @@
 )
 def test_example_not_following_basemodel(wrong_example, labels, exclusive_classes):
     with make_tempdir() as tmpdir:
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
         with pytest.raises(ValidationError):
-            TextCatTask(
+            make_textcat_task_v2(
                 labels=labels,
                 examples=fewshot_reader(tmp_path),
                 exclusive_classes=exclusive_classes,
             )
+
+
+def test_external_template_actually_loads():
+    template_path = str(TEMPLATES_DIR / "textcat_template.jinja2")
+    template = file_reader(template_path)
+    labels = "Recipe"
+    nlp = spacy.blank("xx")
+    doc = nlp.make_doc("Combine 2 cloves of garlic with soy sauce")
+
+    llm_textcat = make_textcat_task_v2(labels=labels, template=template)
+    prompt = list(llm_textcat.generate_prompts([doc]))[0]
+    assert (
+        prompt.strip()
+        == """
+This is a test textcat template. Here is/are the label/s
+Recipe
+
+Here is the text: Combine 2 cloves of garlic with soy sauce
+""".strip()
+    )
```

### Comparing `spacy-llm-0.1.2/spacy_llm/tests/test_cache.py` & `spacy-llm-0.2.0/spacy_llm/tests/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 import srsly  # type: ignore[import]
 import spacy
 from spacy import Language
 from spacy.tokens import DocBin
 import copy
 
-from ..cache import Cache
+from ..cache import BatchCache
 
 
 _DEFAULT_CFG = {
     "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
     "cache": {
         "batch_size": 2,
@@ -55,20 +55,20 @@
         cache = nlp.get_pipe("llm")._cache  # type: ignore
         assert cache._stats["hit"] == 0
         assert cache._stats["missed"] == n
         assert cache._stats["added"] == n
         assert cache._stats["persisted"] == n
         # Check whether docs are in the batch files they are supposed to be in.
         for doc in docs:
-            doc_id = Cache._doc_id(doc)
+            doc_id = BatchCache._doc_id(doc)
             batch_id = index_dict[doc_id]
             batch_path = cache._batch_path(batch_id)
             batch_docs = DocBin().from_disk(batch_path).get_docs(nlp.vocab)
-            doc_ids = [Cache._doc_id(d) for d in batch_docs]
-            assert Cache._batch_id(doc_ids) == batch_id
+            doc_ids = [BatchCache._doc_id(d) for d in batch_docs]
+            assert BatchCache._batch_id(doc_ids) == batch_id
             assert doc_id in doc_ids
 
         #######################################################
         # Test cache reading
         #######################################################
 
         nlp_2 = _init_nlp(tmpdir)
```

### Comparing `spacy-llm-0.1.2/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.1.2
+Version: 0.2.0
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -21,28 +21,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: minichain
+Provides-Extra: langchain
+Provides-Extra: transformers
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/external.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 This package integrates Large Language Models (LLMs) into [spaCy](https://spacy.io), featuring a modular system for **fast prototyping** and **prompting**, and turning unstructured responses into **robust outputs** for various NLP tasks, **no training data** required.
 
 - Serializable `llm` **component** to integrate prompts into your pipeline
-- **Modular functions** to define the [**task**](#Tasks) (prompting and parsing) and [**backend**](#Backends) (model to use)
+- **Modular functions** to define the [**task**](#tasks) (prompting and parsing) and [**backend**](#backends) (model to use)
 - Support for **hosted APIs** and self-hosted **open-source models**
 - Integration with [`MiniChain`](https://github.com/srush/MiniChain) and [`LangChain`](https://github.com/hwchase17/langchain)
 - Access to **[OpenAI API](https://platform.openai.com/docs/api-reference/introduction)**, including GPT-4 and various GPT-3 models
 - Built-in support for **open-source [Dolly](https://huggingface.co/databricks)** models hosted on Hugging Face
 - Usage examples for **Named Entity Recognition** and **Text Classification**
 - Easy implementation of **your own functions** via [spaCy's registry](https://spacy.io/api/top-level#registry) for custom prompting, parsing and model integrations
 
@@ -73,15 +76,15 @@
 The task and the backend have to be supplied to the `llm` pipeline component using [spaCy's config
 system](https://spacy.io/api/data-formats#config). This package provides various built-in
 functionality, as detailed in the [API](#-api) documentation.
 
 ### Example 1: Add a text classifier using a GPT-3 model from OpenAI
 
 Create a new API key from openai.com or fetch an existing one, and ensure the keys are set as environmental variables.
-For more background information, see the [OpenAI](#OpenAI) section.
+For more background information, see the [OpenAI](#openai) section.
 
 Create a config file `config.cfg` containing at least the following
 (or see the full example [here](usage_examples/textcat_openai)):
 
 ```ini
 [nlp]
 lang = "en"
@@ -89,30 +92,29 @@
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
-@llm_tasks = "spacy.TextCat.v1"
+@llm_tasks = "spacy.TextCat.v2"
 labels = COMPLIMENT,INSULT
 
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
-config = {"model": "text-davinci-003", "temperature": 0.3}
+config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
 Now run:
 
 ```python
-from spacy import util
+from spacy_llm.util import assemble
 
-config = util.load_config("config.cfg")
-nlp = util.load_model_from_config(config, auto_fill=True)
+nlp = assemble("config.cfg")
 doc = nlp("You look gorgeous!")
 print(doc.cats)
 ```
 
 ### Example 2: Add NER using an open-source model through Hugging Face
 
 To run this example, ensure that you have a GPU enabled, and `transformers`, `torch` and CUDA installed.
@@ -128,30 +130,29 @@
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
-@llm_tasks = "spacy.NER.v1"
+@llm_tasks = "spacy.NER.v2"
 labels = PERSON,ORGANISATION,LOCATION
 
 [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
 Now run:
 
 ```python
-from spacy import util
+from spacy_llm.util import assemble
 
-config = util.load_config("config.cfg")
-nlp = util.load_model_from_config(config, auto_fill=True)
+nlp = assemble("config.cfg")
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
 
 Note that Hugging Face will download the `"databricks/dolly-v2-3b"` model the first time you use it. You can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
@@ -166,73 +167,87 @@
 import spacy
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "llm",
     config={
         "task": {
-            "@llm_tasks": "spacy.NER.v1",
+            "@llm_tasks": "spacy.NER.v2",
             "labels": "PERSON,ORGANISATION,LOCATION"
         },
         "backend": {
             "@llm_backends": "spacy.REST.v1",
             "api": "OpenAI",
-            "config": {"model": "text-davinci-003"},
+            "config": {"model": "gpt-3.5-turbo"},
         },
     },
 )
+nlp.initialize()
 doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents])
 ```
 
 Note that for efficient usage of resources, typically you would use [`nlp.pipe(docs)`](https://spacy.io/api/language#pipe)
 with a batch, instead of calling `nlp(doc)` with a single document.
 
 ### Example 4: Implement your own custom task
 
 To write a
 [`task`](#tasks), you
 need to implement two functions: `generate_prompts` that takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
 them into a list of prompts, and `parse_responses` that transforms the LLM outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
 
+To register your custom task with spaCy, decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer to in your config.
+
 > 📖 For more details, see the [**usage example on writing your own task**](usage_examples/README.md#writing-your-own-task)
 
 ```python
 from spacy_llm.registry import registry
+from spacy_llm.util import split_labels
+
+
+@registry.llm_tasks("my_namespace.MyTask.v1")
+def make_my_task(labels: str, my_other_config_val: float) -> "MyTask":
+    labels_list = split_labels(labels)
+    return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
+
 
-@registry.llm_tasks("spacy.MyTask.v1")
 class MyTask:
-    def __init__(self, labels: str):
+    def __init__(self, labels: List[str], my_other_config_val: float):
         ...
 
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         ...
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
         ...
 ```
 
 ```ini
 # config.cfg (excerpt)
 [components.llm.task]
-@llm_tasks = "spacy.MyTask.v1"
+@llm_tasks = "my_namespace.MyTask.v1"
 labels = LABEL1,LABEL2,LABEL3
+my_other_config_val = 0.3
 ```
 
 ## 📓 API
 
 Each `llm` component is defined by two main settings:
 
-- A [**task**](#Tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
+- A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
-- A [**backend**](#Backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
+- A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
 
+Moreover, the component also implements [**caching**](#cache) functionality to avoid running
+the same document through an LLM service (be it local or through a REST API) more than once.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -258,17 +273,89 @@
 
 | Argument    | Type            | Description              |
 | ----------- | --------------- | ------------------------ |
 | `docs`      | `Iterable[Doc]` | The input documents.     |
 | `responses` | `Iterable[Any]` | The generated prompts.   |
 | **RETURNS** | `Iterable[Doc]` | The annotated documents. |
 
+#### spacy.NER.v2
+
+The built-in NER task supports both zero-shot and few-shot prompting. This version also supports explicitly defining the provided labels with custom descriptions.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,ORGANISATION,LOCATION
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                  | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`                  | `str`                                   |                                                          | Comma-separated list of labels.                                                                                                                       |
+| `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                   | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                   | Optional function that generates examples for few-shot learning.                                                                                      |
+| `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                   | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
+| `alignment_mode`          | `str`                                   | `"contract"`                                             | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
+| `case_sensitive_matching` | `bool`                                  | `False`                                                  | Whether to search without case sensitivity.                                                                                                           |
+| `single_match`            | `bool`                                  | `False`                                                  | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
+
+The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
+This means that a form of string matching is required. This can be configured by the following parameters:
+
+- The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
+  want to mark it every time it occurs in the document.
+- The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
+- The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
+  in the call to [`doc.char_span()`](https://spacy.io/api/doc#char_span). The `"strict"` mode will only keep spans that strictly adhere to the given token boundaries.
+  `"contract"` will only keep those tokens that are fully within the given range, e.g. reducing `"New Y"` to `"New"`.
+  Finally, `"expand"` will expand the span to the next token boundaries, e.g. expanding `"New Y"` out to `"New York"`.
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: Jack and Jill went up the hill.
+  entities:
+    PERSON:
+      - Jack
+      - Jill
+    LOCATION:
+      - hill
+- text: Jack fell down and broke his crown.
+  entities:
+    PERSON:
+      - Jack
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,ORGANISATION,LOCATION
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "ner_examples.yml"
+```
+
+If you don't have specific examples to provide to the LLM, you can write definitions for each label and provide them via the `label_definitions` argument. This lets you tell the LLM exactly what you're looking for rather than relying on the LLM to interpret its task given just the label name. Label descriptions are freeform so you can write whatever you want here, but through some experiments a brief description along with some examples and counter examples seems to work quite well.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.NER.v2"
+labels = PERSON,SPORTS_TEAM
+[components.llm.task.label_definitions]
+PERSON = "Extract any named individual in the text."
+SPORTS_TEAM = "Extract the names of any professional sports team. e.g. Golden State Warriors, LA Lakers, Man City, Real Madrid"
+```
+
+> Label descriptions can also be used with explicit examples to give as much info to the LLM backend as possible.
+
 #### spacy.NER.v1
 
-The built-in NER task supports both zero-shot and few-shot prompting.
+The original version of the built-in NER task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v1"
 labels = PERSON,ORGANISATION,LOCATION
 examples = null
 ```
@@ -278,14 +365,16 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
+[ner]: https://github.com/explosion/spacy-llm/blob/main/spacy_llm/tasks/ner.py#L14
+
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
 - The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
@@ -315,20 +404,120 @@
 @llm_tasks = "spacy.NER.v1"
 labels = PERSON,ORGANISATION,LOCATION
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "ner_examples.yml"
 ```
 
-#### spacy.TextCat.v1
+#### spacy.SpanCat.v2
+
+The built-in SpanCat task is a simple adaptation of the NER task to
+support overlapping entities and store its annotations in `doc.spans`.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.SpanCat.v2"
+labels = PERSON,ORGANISATION,LOCATION
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                            | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`                  | `str`                                   |                                                                    | Comma-separated list of labels.                                                                                                                       |
+| `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                             | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
+| `spans_key`               | `str`                                   | `"sc"`                                                             | Key of the `Doc.spans` dict to save the spans under.                                                                                                  |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                             | Optional function that generates examples for few-shot learning.                                                                                      |
+| `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                             | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
+| `alignment_mode`          | `str`                                   | `"contract"`                                                       | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
+| `case_sensitive_matching` | `bool`                                  | `False`                                                            | Whether to search without case sensitivity.                                                                                                           |
+| `single_match`            | `bool`                                  | `False`                                                            | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
+
+Except for the `spans_key` parameter, the SpanCat task reuses the configuration
+from the NER task.
+Refer to [its documentation](#spacynerv2) for more insight.
+
+#### spacy.SpanCat.v1
+
+The original version of the built-in SpanCat task is a simple adaptation of the v1 NER task to
+support overlapping entities and store its annotations in `doc.spans`.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.SpanCat.v1"
+labels = PERSON,ORGANISATION,LOCATION
+examples = null
+```
+
+| Argument                  | Type                                    | Default      | Description                                                                                                                                  |
+| ------------------------- | --------------------------------------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
+| `spans_key`               | `str`                                   | `"sc"`       | Key of the `Doc.spans` dict to save the spans under.                                                                                         |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
+| `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
+| `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
+| `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
+| `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
+
+Except for the `spans_key` parameter, the SpanCat task reuses the configuration
+from the NER task.
+Refer to [its documentation](#spacynerv1) for more insight.
+
+#### spacy.TextCat.v2
 
 The built-in TextCat task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
+@llm_tasks = "spacy.TextCat.v2"
+labels = COMPLIMENT,INSULT
+examples = null
+```
+
+| Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
+| ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
+| `labels`            | `str`                                   |                                                              | Comma-separated list of labels.                                                                                                                  |
+| `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
+| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
+| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
+| `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
+| `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
+| `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```json
+[
+  {
+    "text": "You look great!",
+    "answer": "Compliment"
+  },
+  {
+    "text": "You are not very clever at all.",
+    "answer": "Insult"
+  }
+]
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.TextCat.v2"
+labels = COMPLIMENT,INSULT
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "textcat_examples.json"
+```
+
+#### spacy.TextCat.v1
+
+The original version of the built-in TextCat task supports both zero-shot and few-shot prompting.
+
+```ini
+[components.llm.task]
 @llm_tasks = "spacy.TextCat.v1"
 labels = COMPLIMENT,INSULT
 examples = null
 ```
 
 | Argument            | Type                                    | Default | Description                                                                                                                                      |
 | ------------------- | --------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
@@ -353,21 +542,62 @@
     "answer": "Insult"
   }
 ]
 ```
 
 ```ini
 [components.llm.task]
-@llm_tasks = "spacy.TextCat.v1"
+@llm_tasks = "spacy.TextCat.v2"
 labels = COMPLIMENT,INSULT
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "textcat_examples.json"
 ```
 
+#### spacy.REL.v1
+
+The built-in REL task supports both zero-shot and few-shot prompting.
+It relies on an upstream NER component for entities extraction.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.REL.v1"
+labels = LivesIn,Visits
+```
+
+| Argument            | Type                                    | Default                                              | Description                                                                                                                              |
+| ------------------- | --------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
+| `labels`            | `str`                                   |                                                      | Comma-separated list of relation labels.                                                                                                 |
+| `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                              |
+| `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                         |
+| `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                     |
+| `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                     |
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```json
+{"text": "Laura bought a house in Boston with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label": "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char": 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1, "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]}
+{"text": "Michael travelled through South America by bike.", "ents": [{"start_char": 0, "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label": "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]}
+```
+
+Note: the REL task relies on pre-extracted entities to make its prediction.
+Hence, you'll need to add a component that populates `doc.ents` with recognized
+spans to your spaCy pipeline and put it _before_ the REL component.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.REL.v1"
+labels = LivesIn,Visits
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "rel_examples.jsonl"
+```
+
 #### spacy.NoOp.v1
 
 This task is only useful for testing - it tells the LLM to do nothing, and does not set any fields on the `docs`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
@@ -377,15 +607,31 @@
 
 A _backend_ defines which LLM model to query, and how to query it. It can be a simple function taking a collection
 of prompts (consistent with the output type of `task.generate_prompts()`) and returning a collection of responses
 (consistent with the expected input of `parse_responses`). Generally speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
 but specific implementations can have other signatures, like `Callable[[Iterable[str]], Iterable[str]]`.
 
 All built-in backends are registered in `llm_backends`. If no backend is specified, the repo currently connects to the [`OpenAI` API](#openai) by default,
-using the built-in REST protocol, and accesses the `"text-davinci-003"` model.
+using the built-in REST protocol, and accesses the `"gpt-3.5-turbo"` model.
+
+> :question: _Why are there backends for third-party libraries in addition to a native REST backend and which should
+> I choose?_
+>
+> Third-party libraries like `langchain` or `minichain` focus on prompt management, integration of many different LLM
+> APIs, and other related features such as conversational memory or agents. `spacy-llm` on the other hand emphasizes
+> features we consider useful in the context of NLP pipelines utilizing LLMs to process documents (mostly) independent
+> from each other. It makes sense that the feature set of such third-party libraries and `spacy-llm` is not identical -
+> and users might want to take advantage of features not available in `spacy-llm`.
+>
+> The advantage of offering our own REST backend is that we can ensure a larger degree of stability of robustness, as
+> we can guarantee backwards-compatibility and more smoothly integrated error handling.
+>
+> Ultimately we recommend trying to implement your use case using the REST backend first (which is configured as the
+> default backend). If however there are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting mechanism, if so required.
 
 #### OpenAI
 
 When the backend uses OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
 environmental variables:
 
 ```shell
@@ -397,15 +643,15 @@
 
 This default backend uses `requests` and a simple retry mechanism to access an API.
 
 ```ini
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
-config = {"model": "text-davinci-003", "temperature": 0.3}
+config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
 | Argument    | Type             | Default | Description                                                                                                          |
 | ----------- | ---------------- | ------- | -------------------------------------------------------------------------------------------------------------------- |
 | `api`       | `str`            |         | The name of a supported API. In v.0.1.0, only "OpenAI" is supported.                                                 |
 | `config`    | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the backend.                                                                      |
 | `strict`    | `bool`           | `True`  | If `True`, raises an error if the LLM API returns a malformed response. Otherwise, return the error responses as is. |
@@ -434,14 +680,16 @@
 
 #### spacy.MiniChain.v1
 
 To use [MiniChain](https://github.com/srush/MiniChain) for the API retrieval part, make sure you have installed it first:
 
 ```shell
 python -m pip install "minichain>=0.3,<0.4"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[minichain]"
 ```
 
 Note that MiniChain currently only supports Python 3.8, 3.9 and 3.10.
 
 Example config blocks:
 
 ```ini
@@ -463,14 +711,16 @@
 
 #### spacy.LangChain.v1
 
 To use [LangChain](https://github.com/hwchase17/langchain) for the API retrieval part, make sure you have installed it first:
 
 ```shell
 python -m pip install "langchain>=0.0.144,<0.1"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[langchain]"
 ```
 
 Note that LangChain currently only supports Python 3.9 and beyond.
 
 Example config block:
 
 ```ini
@@ -491,17 +741,18 @@
 
 #### spacy.DollyHF.v1
 
 To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
 This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
 ```shell
-python -m pip install "cupy-cuda11x"
 python -m pip install "torch>=1.13.1,<2.0"
 python -m pip install "transformers>=4.28.1,<5.0"
+# Or install with spacy-llm directly
+python -m pip install "spacy-llm[transformers]"
 ```
 
 If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries.
 
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
@@ -526,14 +777,40 @@
 - `"databricks/dolly-v2-7b"`
 - `"databricks/dolly-v2-12b"`
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
+### Cache
+
+Interacting with LLMs, either through an external API or a local instance, is costly.
+Since developing an NLP pipeline generally means a lot of exploration and prototyping,
+`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
+
+Example config block:
+
+```ini
+[components.llm.cache]
+@llm_misc = "spacy.BatchCache.v1",
+path = "path/to/cache"
+batch_size = 64
+max_batches_in_mem = 4
+```
+
+| Argument             | Type                         | Default | Description                                          |
+| -------------------- | ---------------------------- | ------- | ---------------------------------------------------- |
+| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed. |
+| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file).                  |
+| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory.            |
+
+Note that since the cache is generated by a registered function, you can also provide your own registered function
+returning your own cache implementation. If you wish to do so, ensure that your cache object adheres to the
+`Protocol` defined in `spacy_llm.ty.Cache`.
+
 ### Various functions
 
 #### spacy.FewShotReader.v1
 
 This function is registered in spaCy's `misc` registry, and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file.
 It uses [`srsly`](https://github.com/explosion/srsly) to read in these files and parses them depending on the file extension.
 
@@ -543,14 +820,30 @@
 path = "ner_examples.yml"
 ```
 
 | Argument | Type               | Description                                                                |
 | -------- | ------------------ | -------------------------------------------------------------------------- |
 | `path`   | `Union[str, Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
 
+#### spacy.FileReader.v1
+
+This function is registered in spaCy's `misc` registry, and reads a file provided to the `path` to return a `str`
+representation of its contents. This function is typically used to read
+[Jinja](https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt template.
+
+```ini
+[components.llm.task.template]
+@misc = "spacy.FileReader.v1"
+path = "ner_template.jinja2"
+```
+
+| Argument | Type               | Description                  |
+| -------- | ------------------ | ---------------------------- |
+| `path`   | `Union[str, Path]` | Path to the file to be read. |
+
 #### Normalizer functions
 
 These functions provide simple normalizations for string comparisons, e.g. between a list of specified labels
 and a label given in the raw text of the LLM response. They are registered in spaCy's `misc` registry
 and have the signature `Callable[[str], str]`.
 
 - `spacy.StripNormalizer.v1`: only apply `text.strip()`
```

#### html2text {}

```diff
@@ -1,146 +1,156 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.1.2 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.0 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/
-img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP pipelines !
-[GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/
-explosion/spacy-llm/external.yml) [![pypi Version](https://img.shields.io/pypi/
-v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/
-project/spacy-llm/) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/
-black) This package integrates Large Language Models (LLMs) into [spaCy](https:
-//spacy.io), featuring a modular system for **fast prototyping** and
-**prompting**, and turning unstructured responses into **robust outputs** for
-various NLP tasks, **no training data** required. - Serializable `llm`
-**component** to integrate prompts into your pipeline - **Modular functions**
-to define the [**task**](#Tasks) (prompting and parsing) and [**backend**]
-(#Backends) (model to use) - Support for **hosted APIs** and self-hosted
-**open-source models** - Integration with [`MiniChain`](https://github.com/
-srush/MiniChain) and [`LangChain`](https://github.com/hwchase17/langchain) -
-Access to **[OpenAI API](https://platform.openai.com/docs/api-reference/
-introduction)**, including GPT-4 and various GPT-3 models - Built-in support
-for **open-source [Dolly](https://huggingface.co/databricks)** models hosted on
-Hugging Face - Usage examples for **Named Entity Recognition** and **Text
-Classification** - Easy implementation of **your own functions** via [spaCy's
-registry](https://spacy.io/api/top-level#registry) for custom prompting,
-parsing and model integrations ## ð§  Motivation Large Language Models (LLMs)
-feature powerful natural language understanding capabilities. With only a few
-(and sometimes no) examples, an LLM can be prompted to perform custom NLP tasks
-such as text categorization, named entity recognition, coreference resolution,
-information extraction and more. [spaCy](https://spacy.io) is a well-
-established library for building systems that need to work with language in
-various ways. spaCy's built-in components are generally powered by supervised
-learning or rule-based approaches. Supervised learning is much worse than LLM
-prompting for prototyping, but for many tasks it's much better for production.
-A transformer model that runs comfortably on a single GPU is extremely
-powerful, and it's likely to be a better choice for any task for which you have
-a well-defined output. You train the model with anything from a few hundred to
-a few thousand labelled examples, and it will learn to do exactly that.
-Efficiency, reliability and control are all better with supervised learning,
-and accuracy will generally be higher than LLM prompting as well. `spacy-llm`
-lets you have **the best of both worlds**. You can quickly initialize a
-pipeline with components powered by LLM prompts, and freely mix in components
-powered by other approaches. As your project progresses, you can look at
-replacing some or all of the LLM-powered components as you require. Of course,
-there can be components in your system for which the power of an LLM is fully
-justified. If you want a system that can synthesize information from multiple
-documents in subtle ways and generate a nuanced summary for you, bigger is
-better. However, even if your production system needs an LLM for some of the
-task, that doesn't mean you need an LLM for all of it. Maybe you want to use a
-cheap text classification model to help you find the texts to summarize, or
-maybe you want to add a rule-based system to sanity check the output of the
-summary. These before-and-after tasks are much easier with a mature and well-
-thought-out library, which is exactly what spaCy provides. ## â³ Install
-`spacy-llm` will be installed automatically in future spaCy versions. For now,
-you can run the following in the same virtual environment where you already
-have `spacy` [installed](https://spacy.io/usage). ```bash python -m pip install
-spacy-llm ``` > â ï¸ This package is still experimental and it is possible
-that changes made to the interface will be breaking in minor version updates.
-## ð Usage The task and the backend have to be supplied to the `llm`
-pipeline component using [spaCy's config system](https://spacy.io/api/data-
-formats#config). This package provides various built-in functionality, as
-detailed in the [API](#-api) documentation. ### Example 1: Add a text
-classifier using a GPT-3 model from OpenAI Create a new API key from openai.com
-or fetch an existing one, and ensure the keys are set as environmental
-variables. For more background information, see the [OpenAI](#OpenAI) section.
-Create a config file `config.cfg` containing at least the following (or see the
-full example [here](usage_examples/textcat_openai)): ```ini [nlp] lang = "en"
-pipeline = ["llm"] [components] [components.llm] factory = "llm"
-[components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
-COMPLIMENT,INSULT [components.llm.backend] @llm_backends = "spacy.REST.v1" api
-= "OpenAI" config = {"model": "text-davinci-003", "temperature": 0.3} ``` Now
-run: ```python from spacy import util config = util.load_config("config.cfg")
-nlp = util.load_model_from_config(config, auto_fill=True) doc = nlp("You look
-gorgeous!") print(doc.cats) ``` ### Example 2: Add NER using an open-source
-model through Hugging Face To run this example, ensure that you have a GPU
-enabled, and `transformers`, `torch` and CUDA installed. For more background
-information, see the [DollyHF](#spacydollyhfv1) section. Create a config file
+Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
+Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
+assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
+pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
+workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
+explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
+img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg?style=flat-square)](https://github.com/ambv/black) This package
+integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
+featuring a modular system for **fast prototyping** and **prompting**, and
+turning unstructured responses into **robust outputs** for various NLP tasks,
+**no training data** required. - Serializable `llm` **component** to integrate
+prompts into your pipeline - **Modular functions** to define the [**task**]
+(#tasks) (prompting and parsing) and [**backend**](#backends) (model to use) -
+Support for **hosted APIs** and self-hosted **open-source models** -
+Integration with [`MiniChain`](https://github.com/srush/MiniChain) and
+[`LangChain`](https://github.com/hwchase17/langchain) - Access to **[OpenAI
+API](https://platform.openai.com/docs/api-reference/introduction)**, including
+GPT-4 and various GPT-3 models - Built-in support for **open-source [Dolly]
+(https://huggingface.co/databricks)** models hosted on Hugging Face - Usage
+examples for **Named Entity Recognition** and **Text Classification** - Easy
+implementation of **your own functions** via [spaCy's registry](https://
+spacy.io/api/top-level#registry) for custom prompting, parsing and model
+integrations ## ð§  Motivation Large Language Models (LLMs) feature powerful
+natural language understanding capabilities. With only a few (and sometimes no)
+examples, an LLM can be prompted to perform custom NLP tasks such as text
+categorization, named entity recognition, coreference resolution, information
+extraction and more. [spaCy](https://spacy.io) is a well-established library
+for building systems that need to work with language in various ways. spaCy's
+built-in components are generally powered by supervised learning or rule-based
+approaches. Supervised learning is much worse than LLM prompting for
+prototyping, but for many tasks it's much better for production. A transformer
+model that runs comfortably on a single GPU is extremely powerful, and it's
+likely to be a better choice for any task for which you have a well-defined
+output. You train the model with anything from a few hundred to a few thousand
+labelled examples, and it will learn to do exactly that. Efficiency,
+reliability and control are all better with supervised learning, and accuracy
+will generally be higher than LLM prompting as well. `spacy-llm` lets you have
+**the best of both worlds**. You can quickly initialize a pipeline with
+components powered by LLM prompts, and freely mix in components powered by
+other approaches. As your project progresses, you can look at replacing some or
+all of the LLM-powered components as you require. Of course, there can be
+components in your system for which the power of an LLM is fully justified. If
+you want a system that can synthesize information from multiple documents in
+subtle ways and generate a nuanced summary for you, bigger is better. However,
+even if your production system needs an LLM for some of the task, that doesn't
+mean you need an LLM for all of it. Maybe you want to use a cheap text
+classification model to help you find the texts to summarize, or maybe you want
+to add a rule-based system to sanity check the output of the summary. These
+before-and-after tasks are much easier with a mature and well-thought-out
+library, which is exactly what spaCy provides. ## â³ Install `spacy-llm` will
+be installed automatically in future spaCy versions. For now, you can run the
+following in the same virtual environment where you already have `spacy`
+[installed](https://spacy.io/usage). ```bash python -m pip install spacy-llm
+``` > â ï¸ This package is still experimental and it is possible that changes
+made to the interface will be breaking in minor version updates. ## ð Usage
+The task and the backend have to be supplied to the `llm` pipeline component
+using [spaCy's config system](https://spacy.io/api/data-formats#config). This
+package provides various built-in functionality, as detailed in the [API](#-
+api) documentation. ### Example 1: Add a text classifier using a GPT-3 model
+from OpenAI Create a new API key from openai.com or fetch an existing one, and
+ensure the keys are set as environmental variables. For more background
+information, see the [OpenAI](#openai) section. Create a config file
 `config.cfg` containing at least the following (or see the full example [here]
+(usage_examples/textcat_openai)): ```ini [nlp] lang = "en" pipeline = ["llm"]
+[components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
+= "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.backend]
+@llm_backends = "spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-
+turbo", "temperature": 0.3} ``` Now run: ```python from spacy_llm.util import
+assemble nlp = assemble("config.cfg") doc = nlp("You look gorgeous!") print
+(doc.cats) ``` ### Example 2: Add NER using an open-source model through
+Hugging Face To run this example, ensure that you have a GPU enabled, and
+`transformers`, `torch` and CUDA installed. For more background information,
+see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
+containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.NER.v1" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
+= "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1" # For better performance, use databricks/
 dolly-v2-12b instead model = "databricks/dolly-v2-3b" ``` Now run: ```python
-from spacy import util config = util.load_config("config.cfg") nlp =
-util.load_model_from_config(config, auto_fill=True) doc = nlp("Jack and Jill
-rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for ent in
-doc.ents]) ``` Note that Hugging Face will download the `"databricks/dolly-v2-
-3b"` model the first time you use it. You can [define the cached directory]
-(https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by
-setting the environmental variable `HF_HOME`. Also, you can upgrade the model
-to be `"databricks/dolly-v2-12b"` for better performance. ### Example 3: Create
-the component directly in Python The `llm` component behaves as any other spaCy
-component does, so adding it to an existing pipeline follows the same pattern:
-```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config=
-{ "task": { "@llm_tasks": "spacy.NER.v1", "labels":
+from spacy_llm.util import assemble nlp = assemble("config.cfg") doc = nlp
+("Jack and Jill rode up the hill in Les Deux Alpes") print([(ent.text,
+ent.label_) for ent in doc.ents]) ``` Note that Hugging Face will download the
+`"databricks/dolly-v2-3b"` model the first time you use it. You can [define the
+cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/
+manage-cache) by setting the environmental variable `HF_HOME`. Also, you can
+upgrade the model to be `"databricks/dolly-v2-12b"` for better performance. ###
+Example 3: Create the component directly in Python The `llm` component behaves
+as any other spaCy component does, so adding it to an existing pipeline follows
+the same pattern: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
+( "llm", config={ "task": { "@llm_tasks": "spacy.NER.v2", "labels":
 "PERSON,ORGANISATION,LOCATION" }, "backend": { "@llm_backends":
-"spacy.REST.v1", "api": "OpenAI", "config": {"model": "text-davinci-003"}, },
-}, ) doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes") print([
-(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient usage
-of resources, typically you would use [`nlp.pipe(docs)`](https://spacy.io/api/
-language#pipe) with a batch, instead of calling `nlp(doc)` with a single
-document. ### Example 4: Implement your own custom task To write a [`task`]
-(#tasks), you need to implement two functions: `generate_prompts` that takes a
-list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms them
-into a list of prompts, and `parse_responses` that transforms the LLM outputs
-into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans,
-text categories and more. > ð For more details, see the [**usage example on
-writing your own task**](usage_examples/README.md#writing-your-own-task)
-```python from spacy_llm.registry import registry @registry.llm_tasks
-("spacy.MyTask.v1") class MyTask: def __init__(self, labels: str): ... def
+"spacy.REST.v1", "api": "OpenAI", "config": {"model": "gpt-3.5-turbo"}, }, }, )
+nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
+print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
+usage of resources, typically you would use [`nlp.pipe(docs)`](https://
+spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
+single document. ### Example 4: Implement your own custom task To write a
+[`task`](#tasks), you need to implement two functions: `generate_prompts` that
+takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
+them into a list of prompts, and `parse_responses` that transforms the LLM
+outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity
+spans, text categories and more. To register your custom task with spaCy,
+decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator
+with a custom name that you can refer to in your config. > ð For more
+details, see the [**usage example on writing your own task**](usage_examples/
+README.md#writing-your-own-task) ```python from spacy_llm.registry import
+registry from spacy_llm.util import split_labels @registry.llm_tasks
+("my_namespace.MyTask.v1") def make_my_task(labels: str, my_other_config_val:
+float) -> "MyTask": labels_list = split_labels(labels) return MyTask
+(labels=labels_list, my_other_config_val=my_other_config_val) class MyTask: def
+__init__(self, labels: List[str], my_other_config_val: float): ... def
 generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]: ... def
 parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] ) -
 > Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
-@llm_tasks = "spacy.MyTask.v1" labels = LABEL1,LABEL2,LABEL3 ``` ## ð API
-Each `llm` component is defined by two main settings: - A [**task**](#Tasks),
-defining the prompt to send to the LLM as well as the functionality to parse
-the resulting response back into structured fields on spaCy's [Doc](https://
-spacy.io/api/doc) objects. - A [**backend**](#Backends) defining the model to
-use and how to connect to it. Note that `spacy-llm` supports both access to
-external APIs (such as OpenAI) as well as access to self-hosted open-source
-LLMs (such as using Dolly through Hugging Face). ### Tasks A _task_ defines an
-NLP problem or question, that will be sent to the LLM via a prompt. Further,
-the task defines how to parse the LLM's responses back into structured
-information. All tasks are registered in spaCy's `llm_tasks` registry.
-Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined
-in [`ty.py`](spacy_llm/ty.py). It needs to define a `generate_prompts` function
-and a `parse_responses` function. #### function `task.generate_prompts` Takes a
+@llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
+my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
+two main settings: - A [**task**](#tasks), defining the prompt to send to the
+LLM as well as the functionality to parse the resulting response back into
+structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
+[**backend**](#backends) defining the model to use and how to connect to it.
+Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
+well as access to self-hosted open-source LLMs (such as using Dolly through
+Hugging Face). Moreover, the component also implements [**caching**](#cache)
+functionality to avoid running the same document through an LLM service (be it
+local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
+problem or question, that will be sent to the LLM via a prompt. Further, the
+task defines how to parse the LLM's responses back into structured information.
+All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
+a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
+(spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
+`parse_responses` function. #### function `task.generate_prompts` Takes a
 collection of documents, and returns a collection of "prompts", which can be of
 type `Any`. Often, prompts are of type `str` - but this is not enforced to
 allow for maximum flexibility in the framework. | Argument | Type | Description
 | | ----------- | --------------- | ---------------------- | | `docs` |
 `Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
 generated prompts. | #### function `task.parse_responses` Takes a collection of
 LLM responses and the original documents, parses the responses into structured
@@ -148,31 +158,92 @@
 function is free to set the annotations in any way, including `Doc` fields like
 `ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
 of type `Iterable[Any]`, though they will often be `str` objects. This depends
 on the return type of the [backend](#backends). | Argument | Type | Description
 | | ----------- | --------------- | ------------------------ | | `docs` |
 `Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
 generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
-| #### spacy.NER.v1 The built-in NER task supports both zero-shot and few-shot
-prompting. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
+| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
+prompting. This version also supports explicitly defining the provided labels
+with custom descriptions. ```ini [components.llm.task] @llm_tasks =
+"spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
+Argument | Type | Default | Description | | ------------------------- | -------
+-------------------------------- | --------------------------------------------
+------------ | ----------------------------------------------------------------
+-------------------------------------------------------------------------------
+------ | | `labels` | `str` | | Comma-separated list of labels. | | `template`
+| `str` | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom
+prompt template to send to LLM backend. Default templates for each task are
+located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
+`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
+description of that label. These descriptions are added to the prompt to help
+instruct the LLM on what to extract. | | `examples` | `Optional[Callable[[],
+Iterable[Any]]]` | `None` | Optional function that generates examples for few-
+shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
+Function that normalizes the labels as returned by the LLM. If `None`, defaults
+to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"`
+| Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | The NER
+task implementation doesn't currently ask the LLM for specific offsets, but
+simply expects a list of strings that represent the enties in the document.
+This means that a form of string matching is required. This can be configured
+by the following parameters: - The `single_match` parameter is typically set to
+`False` to allow for multiple matches. For instance, the response from the LLM
+might only mention the entity "Paris" once, but you'd still want to mark it
+every time it occurs in the document. - The case-sensitive matching is
+typically set to `False` to be robust against case variances in the LLM's
+output. - The `alignment_mode` argument is used to match entities as returned
+by the LLM to the tokens from the original `Doc` - specifically it's used as
+argument in the call to [`doc.char_span()`](https://spacy.io/api/
+doc#char_span). The `"strict"` mode will only keep spans that strictly adhere
+to the given token boundaries. `"contract"` will only keep those tokens that
+are fully within the given range, e.g. reducing `"New Y"` to `"New"`. Finally,
+`"expand"` will expand the span to the next token boundaries, e.g. expanding
+`"New Y"` out to `"New York"`. To perform few-shot learning, you can write down
+a few examples in a separate file, and provide these to be injected into the
+prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```yaml - text: Jack and Jill went up the hill.
+entities: PERSON: - Jack - Jill LOCATION: - hill - text: Jack fell down and
+broke his crown. entities: PERSON: - Jack ``` ```ini [components.llm.task]
+@llm_tasks = "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"ner_examples.yml" ``` If you don't have specific examples to provide to the
+LLM, you can write definitions for each label and provide them via the
+`label_definitions` argument. This lets you tell the LLM exactly what you're
+looking for rather than relying on the LLM to interpret its task given just the
+label name. Label descriptions are freeform so you can write whatever you want
+here, but through some experiments a brief description along with some examples
+and counter examples seems to work quite well. ```ini [components.llm.task]
+@llm_tasks = "spacy.NER.v2" labels = PERSON,SPORTS_TEAM
+[components.llm.task.label_definitions] PERSON = "Extract any named individual
+in the text." SPORTS_TEAM = "Extract the names of any professional sports team.
+e.g. Golden State Warriors, LA Lakers, Man City, Real Madrid" ``` > Label
+descriptions can also be used with explicit examples to give as much info to
+the LLM backend as possible. #### spacy.NER.v1 The original version of the
+built-in NER task supports both zero-shot and few-shot prompting. ```ini
+[components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
 Description | | ------------------------- | -----------------------------------
 ---- | ------------ | ---------------------------------------------------------
 -------------------------------------------------------------------------------
 ---- | | `labels` | `str` | | Comma-separated list of labels. | | `examples` |
 `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
 generates examples for few-shot learning. | | `normalizer` | `Optional[Callable
 [[str], str]]` | `None` | Function that normalizes the labels as returned by
 the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | |
 `alignment_mode` | `str` | `"contract"` | Alignment mode in case the LLM
 returns entities that do not align with token boundaries. Options are
 `"strict"`, `"contract"` or `"expand"`. | | `case_sensitive_matching` | `bool`
 | `False` | Whether to search without case sensitivity. | | `single_match` |
 `bool` | `False` | Whether to match an entity in the LLM's response only once
-(the first hit) or multiple times. | The NER task implementation doesn't
+(the first hit) or multiple times. | [ner]: https://github.com/explosion/spacy-
+llm/blob/main/spacy_llm/tasks/ner.py#L14 The NER task implementation doesn't
 currently ask the LLM for specific offsets, but simply expects a list of
 strings that represent the enties in the document. This means that a form of
 string matching is required. This can be configured by the following
 parameters: - The `single_match` parameter is typically set to `False` to allow
 for multiple matches. For instance, the response from the LLM might only
 mention the entity "Paris" once, but you'd still want to mark it every time it
 occurs in the document. - The case-sensitive matching is typically set to
@@ -187,58 +258,185 @@
 perform few-shot learning, you can write down a few examples in a separate
 file, and provide these to be injected into the prompt to the LLM. The default
 reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
 ```yaml - text: Jack and Jill went up the hill. entities: PERSON: - Jack - Jill
 LOCATION: - hill - text: Jack fell down and broke his crown. entities: PERSON:
 - Jack ``` ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.TextCat.v1
-The built-in TextCat task supports both zero-shot and few-shot prompting.
-```ini [components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
-COMPLIMENT,INSULT examples = null ``` | Argument | Type | Default | Description
-| | ------------------- | --------------------------------------- | ------- | -
+"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.SpanCat.v2
+The built-in SpanCat task is a simple adaptation of the NER task to support
+overlapping entities and store its annotations in `doc.spans`. ```ini
+[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels =
+PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
+Description | | ------------------------- | -----------------------------------
+---- | ------------------------------------------------------------------ | ---
 -------------------------------------------------------------------------------
----------------------------------------------------------------- | | `labels` |
-str | | Comma-separated list of labels. | | `examples` | `Optional[Callable[[],
-Iterable[Any]]]` | `None` | Optional function that generates examples for few-
-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
-Function that normalizes the labels as returned by the LLM. If `None`, falls
+------------------------------------------------------------------- | |
+`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
+[`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom
+prompt template to send to LLM backend. Default templates for each task are
+located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
+`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
+description of that label. These descriptions are added to the prompt to help
+instruct the LLM on what to extract. | | `spans_key` | `str` | `"sc"` | Key of
+the `Doc.spans` dict to save the spans under. | | `examples` | `Optional
+[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
+examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
+str]]` | `None` | Function that normalizes the labels as returned by the LLM.
+If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` |
+`str` | `"contract"` | Alignment mode in case the LLM returns entities that do
+not align with token boundaries. Options are `"strict"`, `"contract"` or
+`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
+search without case sensitivity. | | `single_match` | `bool` | `False` |
+Whether to match an entity in the LLM's response only once (the first hit) or
+multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
+the configuration from the NER task. Refer to [its documentation](#spacynerv2)
+for more insight. #### spacy.SpanCat.v1 The original version of the built-in
+SpanCat task is a simple adaptation of the v1 NER task to support overlapping
+entities and store its annotations in `doc.spans`. ```ini [components.llm.task]
+@llm_tasks = "spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples
+= null ``` | Argument | Type | Default | Description | | ----------------------
+--- | --------------------------------------- | ------------ | ----------------
+-------------------------------------------------------------------------------
+--------------------------------------------- | | `labels` | `str` | | Comma-
+separated list of labels. | | `spans_key` | `str` | `"sc"` | Key of the
+`Doc.spans` dict to save the spans under. | | `examples` | `Optional[Callable[
+[], Iterable[Any]]]` | `None` | Optional function that generates examples for
+few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
+| Function that normalizes the labels as returned by the LLM. If `None`,
+defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` |
+`"contract"` | Alignment mode in case the LLM returns entities that do not
+align with token boundaries. Options are `"strict"`, `"contract"` or
+`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
+search without case sensitivity. | | `single_match` | `bool` | `False` |
+Whether to match an entity in the LLM's response only once (the first hit) or
+multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
+the configuration from the NER task. Refer to [its documentation](#spacynerv1)
+for more insight. #### spacy.TextCat.v2 The built-in TextCat task supports both
+zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = COMPLIMENT,INSULT examples = null ``` | Argument |
+Type | Default | Description | | ------------------- | ------------------------
+--------------- | -----------------------------------------------------------
+- | ---------------------------------------------------------------------------
+--------------------------------------------------------------------- | |
+`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
+[`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt
+template to send to LLM backend. Default templates for each task are located in
+the `spacy_llm/tasks/templates` directory. | | `examples` | `Optional[Callable[
+[], Iterable[Any]]]` | `None` | Optional function that generates examples for
+few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
+| Function that normalizes the labels as returned by the LLM. If `None`, falls
 back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
 `False` | If set to `True`, only one label per document should be valid. If set
 to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
 `True` | When set to `True`, allows the LLM to not return any of the given
 label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
 | | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
 when the LLM returns invalid responses. | To perform few-shot learning, you can
 write down a few examples in a separate file, and provide these to be injected
 into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
 supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
 great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
 "answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v1" labels = COMPLIMENT,INSULT [components.llm.task.examples]
+"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
-spacy.NoOp.v1 This task is only useful for testing - it tells the LLM to do
-nothing, and does not set any fields on the `docs`. ```ini
-[components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ### Backends A _backend_
-defines which LLM model to query, and how to query it. It can be a simple
-function taking a collection of prompts (consistent with the output type of
-`task.generate_prompts()`) and returning a collection of responses (consistent
-with the expected input of `parse_responses`). Generally speaking, it's a
-function of type `Callable[[Iterable[Any]], Iterable[Any]]`, but specific
-implementations can have other signatures, like `Callable[[Iterable[str]],
-Iterable[str]]`. All built-in backends are registered in `llm_backends`. If no
-backend is specified, the repo currently connects to the [`OpenAI` API]
-(#openai) by default, using the built-in REST protocol, and accesses the
-`"text-davinci-003"` model. #### OpenAI When the backend uses OpenAI, you have
+spacy.TextCat.v1 The original version of the built-in TextCat task supports
+both zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks
+= "spacy.TextCat.v1" labels = COMPLIMENT,INSULT examples = null ``` | Argument
+| Type | Default | Description | | ------------------- | ----------------------
+----------------- | ------- | -------------------------------------------------
+-------------------------------------------------------------------------------
+---------------- | | `labels` | str | | Comma-separated list of labels. | |
+`examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional
+function that generates examples for few-shot learning. | | `normalizer` |
+`Optional[Callable[[str], str]]` | `None` | Function that normalizes the labels
+as returned by the LLM. If `None`, falls back to
+`spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
+set to `True`, only one label per document should be valid. If set to `False`,
+one document can have multiple labels. | | `allow_none` | `bool` | `True` |
+When set to `True`, allows the LLM to not return any of the given label. The
+resulting dict in `doc.cats` will have `0.0` scores for all labels. | |
+`verbose` | `bool` | `False` | If set to `True`, warnings will be generated
+when the LLM returns invalid responses. | To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
+great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
+"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
+spacy.REL.v1 The built-in REL task supports both zero-shot and few-shot
+prompting. It relies on an upstream NER component for entities extraction.
+```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels =
+LivesIn,Visits ``` | Argument | Type | Default | Description | | --------------
+----- | --------------------------------------- | -----------------------------
+----------------------- | -----------------------------------------------------
+-------------------------------------------------------------------------------
+---- | | `labels` | `str` | | Comma-separated list of relation labels. | |
+`template` | `str` | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) |
+Custom prompt template to send to LLM backend. Default templates for each task
+are located in the `spacy_llm/tasks/templates` directory. | |
+`label_description` | `Optional[Dict[str, str]]` | `None` | Dictionary
+providing a description for each relation label. | | `examples` | `Optional
+[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
+examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
+str]]` | `None` | Function that normalizes the labels as returned by the LLM.
+If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose` | `bool`
+| `False` | If set to `True`, warnings will be generated when the LLM returns
+invalid responses. | To perform few-shot learning, you can write down a few
+examples in a separate file, and provide these to be injected into the prompt
+to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```json {"text": "Laura bought a house in Boston
+with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label":
+"PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char":
+48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1,
+"relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]} {"text":
+"Michael travelled through South America by bike.", "ents": [{"start_char": 0,
+"end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
+"LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
+the REL task relies on pre-extracted entities to make its prediction. Hence,
+you'll need to add a component that populates `doc.ents` with recognized spans
+to your spaCy pipeline and put it _before_ the REL component. ```ini
+[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = LivesIn,Visits
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
+testing - it tells the LLM to do nothing, and does not set any fields on the
+`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
+Backends A _backend_ defines which LLM model to query, and how to query it. It
+can be a simple function taking a collection of prompts (consistent with the
+output type of `task.generate_prompts()`) and returning a collection of
+responses (consistent with the expected input of `parse_responses`). Generally
+speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
+but specific implementations can have other signatures, like `Callable[
+[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
+`llm_backends`. If no backend is specified, the repo currently connects to the
+[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
+accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
+third-party libraries in addition to a native REST backend and which should > I
+choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
+prompt management, integration of many different LLM > APIs, and other related
+features such as conversational memory or agents. `spacy-llm` on the other hand
+emphasizes > features we consider useful in the context of NLP pipelines
+utilizing LLMs to process documents (mostly) independent > from each other. It
+makes sense that the feature set of such third-party libraries and `spacy-llm`
+is not identical - > and users might want to take advantage of features not
+available in `spacy-llm`. > > The advantage of offering our own REST backend is
+that we can ensure a larger degree of stability of robustness, as > we can
+guarantee backwards-compatibility and more smoothly integrated error handling.
+> > Ultimately we recommend trying to implement your use case using the REST
+backend first (which is configured as the > default backend). If however there
+are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting
+mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
 to get an API key from openai.com, and ensure that the keys are set as
 environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
 OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
 `requests` and a simple retry mechanism to access an API. ```ini
 [components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
-= {"model": "text-davinci-003", "temperature": 0.3} ``` | Argument | Type |
+= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
 Default | Description | | ----------- | ---------------- | ------- | ----------
 -------------------------------------------------------------------------------
 --------------------------- | | `api` | `str` | | The name of a supported API.
 In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
 | Further configuration passed on to the backend. | | `strict` | `bool` |
 `True` | If `True`, raises an error if the LLM API returns a malformed
 response. Otherwise, return the error responses as is. | | `max_tries` | `int`
@@ -249,15 +447,16 @@
 32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
 `"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
 babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
 `"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
 For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
 completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
 srush/MiniChain) for the API retrieval part, make sure you have installed it
-first: ```shell python -m pip install "minichain>=0.3,<0.4" ``` Note that
+first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
+spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
 MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
 blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
 api = "OpenAI" [components.llm.backend.query] @llm_queries =
 "spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
 --- | -------------------------------------------------------------------------
 -------- | ------- | ----------------------------------------------------------
 ------------------------- | | `api` | `str` | | The name of an API supported by
@@ -265,15 +464,16 @@
 configuration passed on to the backend. | | `query` | `Optional[Callable[
 ["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
 Function that executes the prompts. If `None`, defaults to
 `spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
 executes the prompts by running `model(text).run()` for each given textual
 prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
 hwchase17/langchain) for the API retrieval part, make sure you have installed
-it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" ``` Note
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
+with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
 that LangChain currently only supports Python 3.9 and beyond. Example config
 block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
 = "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
 {"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
 - | ---------------------------------------------------------------------------
 --- | ------- | ---------------------------------------------------------------
 --------------------- | | `api` | `str` | | The name of an API supported by
@@ -283,46 +483,68 @@
 that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
 The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
 `model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
 `torch` and CUDA in your virtual environment. This allows you to have the
 setting `device=cuda:0` in your config, which ensures that the model is loaded
 entirely on the GPU (and fails otherwise). ```shell python -m pip install
-"cupy-cuda11x" python -m pip install "torch>=1.13.1,<2.0" python -m pip install
-"transformers>=4.28.1,<5.0" ``` If you don't have access to a GPU, you can
-install `accelerate` and set`device_map=auto` instead, but be aware that this
-may result in some layers getting distributed to the CPU or even the hard
-drive, which may ultimately result in extremely slow queries. ```shell python -
-m pip install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+"torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0" # Or
+install with spacy-llm directly python -m pip install "spacy-llm[transformers]"
+``` If you don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
 "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
 ---- | ---------------- | ------- | -------------------------------------------
 ----------------------------------------------------- | | `model` | `str` | |
 The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
 `{}` | Further configuration passed on to the construction of the model with
 `transformers.pipeline()`. | Supported models (see the [Databricks models page]
 (https://huggingface.co/databricks) on Hugging Face for details): -
 `"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` - `"databricks/dolly-
 v2-12b"` Note that Hugging Face will download this model the first time you use
 it - you can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. ### Various functions #### spacy.FewShotReader.v1 This
-function is registered in spaCy's `misc` registry, and reads in examples from a
-`.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
-github.com/explosion/srsly) to read in these files and parses them depending on
-the file extension. ```ini [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument | Type |
-Description | | -------- | ------------------ | -------------------------------
-------------------------------------------- | | `path` | `Union[str, Path]` |
-Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
-#### Normalizer functions These functions provide simple normalizations for
-string comparisons, e.g. between a list of specified labels and a label given
-in the raw text of the LLM response. They are registered in spaCy's `misc`
-registry and have the signature `Callable[[str], str]`. -
-`spacy.StripNormalizer.v1`: only apply `text.strip()` -
+variable `HF_HOME`. ### Cache Interacting with LLMs, either through an external
+API or a local instance, is costly. Since developing an NLP pipeline generally
+means a lot of exploration and prototyping, `spacy-llm` implements a built-in
+cache to avoid reprocessing the same documents at each run. Example config
+block: ```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1", path =
+"path/to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
+Default | Description | | -------------------- | ---------------------------- |
+------- | ---------------------------------------------------- | | `path` |
+`Optional[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching
+is performed. | | `batch_size` | `int` | 64 | Number of docs in one batch
+(file). | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
+in memory. | Note that since the cache is generated by a registered function,
+you can also provide your own registered function returning your own cache
+implementation. If you wish to do so, ensure that your cache object adheres to
+the `Protocol` defined in `spacy_llm.ty.Cache`. ### Various functions ####
+spacy.FewShotReader.v1 This function is registered in spaCy's `misc` registry,
+and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses
+[`srsly`](https://github.com/explosion/srsly) to read in these files and parses
+them depending on the file extension. ```ini [components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument |
+Type | Description | | -------- | ------------------ | ------------------------
+-------------------------------------------------- | | `path` | `Union[str,
+Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or
+`.jsonl`. | #### spacy.FileReader.v1 This function is registered in spaCy's
+`misc` registry, and reads a file provided to the `path` to return a `str`
+representation of its contents. This function is typically used to read [Jinja]
+(https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt
+template. ```ini [components.llm.task.template] @misc = "spacy.FileReader.v1"
+path = "ner_template.jinja2" ``` | Argument | Type | Description | | -------- |
+------------------ | ---------------------------- | | `path` | `Union[str,
+Path]` | Path to the file to be read. | #### Normalizer functions These
+functions provide simple normalizations for string comparisons, e.g. between a
+list of specified labels and a label given in the raw text of the LLM response.
+They are registered in spaCy's `misc` registry and have the signature `Callable
+[[str], str]`. - `spacy.StripNormalizer.v1`: only apply `text.strip()` -
 `spacy.LowercaseNormalizer.v1`: applies `text.strip().lower()` to compare
 strings in a case-insensitive way. ## ð Ongoing work In the near future, we
 will - Add more example tasks - Support a broader range of models - Provide
 more example use-cases and tutorials - Make the built-in tasks easier to
 customize via Jinja templates to define the instructions & examples PRs are
 always welcome! ## ðï¸ Reporting issues If you have questions regarding the
 usage of `spacy-llm`, or want to give us feedback after giving it a spin,
```

### Comparing `spacy-llm-0.1.2/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.2.0/spacy_llm.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 pyproject.toml
 setup.cfg
 setup.py
 spacy_llm/__init__.py
 spacy_llm/cache.py
 spacy_llm/compat.py
 spacy_llm/ty.py
+spacy_llm/util.py
 spacy_llm.egg-info/PKG-INFO
 spacy_llm.egg-info/SOURCES.txt
 spacy_llm.egg-info/dependency_links.txt
 spacy_llm.egg-info/entry_points.txt
 spacy_llm.egg-info/not-zip-safe
 spacy_llm.egg-info/requires.txt
 spacy_llm.egg-info/top_level.txt
 spacy_llm/backends/__init__.py
-spacy_llm/backends/dolly.py
-spacy_llm/backends/langchain.py
-spacy_llm/backends/minichain.py
+spacy_llm/backends/integration/__init__.py
+spacy_llm/backends/integration/base.py
+spacy_llm/backends/integration/dolly.py
+spacy_llm/backends/integration/langchain.py
+spacy_llm/backends/integration/minichain.py
 spacy_llm/backends/rest/__init__.py
 spacy_llm/backends/rest/registry.py
 spacy_llm/backends/rest/backend/__init__.py
 spacy_llm/backends/rest/backend/base.py
 spacy_llm/backends/rest/backend/noop.py
 spacy_llm/backends/rest/backend/openai.py
 spacy_llm/pipeline/__init__.py
@@ -30,34 +33,72 @@
 spacy_llm/registry/__init__.py
 spacy_llm/registry/normalizer.py
 spacy_llm/registry/reader.py
 spacy_llm/registry/util.py
 spacy_llm/tasks/__init__.py
 spacy_llm/tasks/ner.py
 spacy_llm/tasks/noop.py
+spacy_llm/tasks/rel.py
+spacy_llm/tasks/spancat.py
 spacy_llm/tasks/textcat.py
+spacy_llm/tasks/templates/__init__.py
+spacy_llm/tasks/templates/ner.jinja
+spacy_llm/tasks/templates/ner.v2.jinja
+spacy_llm/tasks/templates/rel.jinja
+spacy_llm/tasks/templates/spancat.jinja
+spacy_llm/tasks/templates/spancat.v2.jinja
+spacy_llm/tasks/templates/textcat.jinja
+spacy_llm/tasks/templates/textcat.v2.jinja
+spacy_llm/tasks/util/__init__.py
+spacy_llm/tasks/util/examples.py
+spacy_llm/tasks/util/parsing.py
+spacy_llm/tasks/util/span.py
 spacy_llm/tests/__init__.py
+spacy_llm/tests/compat.py
 spacy_llm/tests/conftest.py
 spacy_llm/tests/test_cache.py
 spacy_llm/tests/test_combinations.py
+spacy_llm/tests/test_registry.py
 spacy_llm/tests/backends/__init__.py
 spacy_llm/tests/backends/test_dolly.py
 spacy_llm/tests/backends/test_langchain.py
 spacy_llm/tests/backends/test_minichain.py
 spacy_llm/tests/backends/test_rest.py
 spacy_llm/tests/pipeline/__init__.py
 spacy_llm/tests/pipeline/test_llm.py
 spacy_llm/tests/tasks/__init__.py
 spacy_llm/tests/tasks/test_ner.py
+spacy_llm/tests/tasks/test_rel.py
+spacy_llm/tests/tasks/test_spancat.py
 spacy_llm/tests/tasks/test_textcat.py
 spacy_llm/tests/tasks/examples/ner_examples.json
 spacy_llm/tests/tasks/examples/ner_examples.jsonl
 spacy_llm/tests/tasks/examples/ner_examples.yml
+spacy_llm/tests/tasks/examples/rel_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_binary_examples.json
 spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
 spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
 spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
 spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
 spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
-spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+spacy_llm/tests/tasks/templates/ner_template.jinja2
+spacy_llm/tests/tasks/templates/textcat_template.jinja2
+usage_examples/__init__.py
+usage_examples/multitask_openai/__init__.py
+usage_examples/multitask_openai/run_pipeline.py
+usage_examples/ner_dolly/__init__.py
+usage_examples/ner_dolly/run_pipeline.py
+usage_examples/ner_langchain_openai/__init__.py
+usage_examples/ner_langchain_openai/run_pipeline.py
+usage_examples/ner_minichain_openai/__init__.py
+usage_examples/ner_minichain_openai/run_pipeline.py
+usage_examples/rel_openai/__init__.py
+usage_examples/rel_openai/run_pipeline.py
+usage_examples/tests/__init__.py
+usage_examples/tests/conftest.py
+usage_examples/tests/test_readme_examples.py
+usage_examples/tests/test_usage_examples.py
+usage_examples/textcat_openai/__init__.py
+usage_examples/textcat_openai/run_pipeline.py
```

