# Comparing `tmp/unstructured-0.6.8.tar.gz` & `tmp/unstructured-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.8.tar", last modified: Fri May 19 19:59:45 2023, max compression
+gzip compressed data, was "unstructured-0.6.9.tar", last modified: Wed May 24 22:34:42 2023, max compression
```

## Comparing `unstructured-0.6.8.tar` & `unstructured-0.6.9.tar`

### file list

```diff
@@ -1,112 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.246387 unstructured-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-19 19:59:34.000000 unstructured-0.6.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-19 19:59:45.246387 unstructured-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-05-19 19:59:34.000000 unstructured-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 19:59:45.246387 unstructured-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-19 19:59:34.000000 unstructured-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.238387 unstructured-0.6.8/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.238387 unstructured-0.6.8/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.238387 unstructured-0.6.8/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.242387 unstructured-0.6.8/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.246387 unstructured-0.6.8/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.246387 unstructured-0.6.8/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-19 19:59:45.000000 unstructured-0.6.8/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.407830 unstructured-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-24 22:34:33.000000 unstructured-0.6.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-24 22:34:33.000000 unstructured-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-24 22:34:42.407830 unstructured-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-05-24 22:34:33.000000 unstructured-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 22:34:42.407830 unstructured-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-24 22:34:33.000000 unstructured-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.403830 unstructured-0.6.9/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.407830 unstructured-0.6.9/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.407830 unstructured-0.6.9/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.8/LICENSE.md` & `unstructured-0.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/PKG-INFO` & `unstructured-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.8
+Version: 0.6.9
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.9 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.8/README.md` & `unstructured-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.9/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.9/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/test_unstructured/test_utils.py` & `unstructured-0.6.9/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/cleaners/core.py` & `unstructured-0.6.9/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/cleaners/extract.py` & `unstructured-0.6.9/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/cleaners/translate.py` & `unstructured-0.6.9/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/documents/base.py` & `unstructured-0.6.9/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/documents/elements.py` & `unstructured-0.6.9/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/documents/email_elements.py` & `unstructured-0.6.9/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/documents/html.py` & `unstructured-0.6.9/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/documents/xml.py` & `unstructured-0.6.9/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/file_utils/exploration.py` & `unstructured-0.6.9/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.9/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/file_utils/filetype.py` & `unstructured-0.6.9/unstructured/file_utils/filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,19 @@
 STR_TO_FILETYPE = {
     "application/pdf": FileType.PDF,
     "application/msword": FileType.DOC,
     "application/vnd.openxmlformats-officedocument.wordprocessingml.document": FileType.DOCX,
     "image/jpeg": FileType.JPG,
     "image/png": FileType.PNG,
     "text/plain": FileType.TXT,
+    "text/x-csv": FileType.CSV,
+    "application/csv": FileType.CSV,
+    "application/x-csv": FileType.CSV,
+    "text/comma-separated-values": FileType.CSV,
+    "text/x-comma-separated-values": FileType.CSV,
     "text/csv": FileType.CSV,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
     "application/json": FileType.JSON,
     "application/rtf": FileType.RTF,
@@ -109,17 +114,25 @@
     "application/xml": FileType.XML,
     "application/vnd.oasis.opendocument.text": FileType.ODT,
     "message/rfc822": FileType.EML,
     "application/x-ole-storage": FileType.MSG,
     "application/vnd.ms-outlook": FileType.MSG,
 }
 
-FILETYPE_TO_MIMETYPE = {
-    v: k for k, v in STR_TO_FILETYPE.items() if k not in ("text/x-markdown", "application/epub+zip")
-}
+MIMETYPES_TO_EXCLUDE = [
+    "text/x-markdown",
+    "application/epub+zip",
+    "text/x-csv",
+    "application/csv",
+    "application/x-csv",
+    "text/comma-separated-values",
+    "text/x-comma-separated-values",
+]
+
+FILETYPE_TO_MIMETYPE = {v: k for k, v in STR_TO_FILETYPE.items() if k not in MIMETYPES_TO_EXCLUDE}
 
 EXT_TO_FILETYPE = {
     ".pdf": FileType.PDF,
     ".docx": FileType.DOCX,
     ".jpg": FileType.JPG,
     ".jpeg": FileType.JPG,
     ".txt": FileType.TXT,
```

### Comparing `unstructured-0.6.8/unstructured/file_utils/metadata.py` & `unstructured-0.6.9/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/azure.py` & `unstructured-0.6.9/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.9/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/discord.py` & `unstructured-0.6.9/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.9/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/git.py` & `unstructured-0.6.9/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/github.py` & `unstructured-0.6.9/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.9/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.9/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/local.py` & `unstructured-0.6.9/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.9/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/s3.py` & `unstructured-0.6.9/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/slack.py` & `unstructured-0.6.9/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.9/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.9/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/interfaces.py` & `unstructured-0.6.9/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/ingest/main.py` & `unstructured-0.6.9/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/nlp/english-words.txt` & `unstructured-0.6.9/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/nlp/english_words.py` & `unstructured-0.6.9/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/nlp/patterns.py` & `unstructured-0.6.9/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/nlp/tokenize.py` & `unstructured-0.6.9/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/__init__.py` & `unstructured-0.6.9/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/api.py` & `unstructured-0.6.9/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/auto.py` & `unstructured-0.6.9/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/common.py` & `unstructured-0.6.9/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/csv.py` & `unstructured-0.6.9/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/doc.py` & `unstructured-0.6.9/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/docx.py` & `unstructured-0.6.9/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/email.py` & `unstructured-0.6.9/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/epub.py` & `unstructured-0.6.9/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/html.py` & `unstructured-0.6.9/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/image.py` & `unstructured-0.6.9/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/json.py` & `unstructured-0.6.9/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/md.py` & `unstructured-0.6.9/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/msg.py` & `unstructured-0.6.9/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/odt.py` & `unstructured-0.6.9/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/pdf.py` & `unstructured-0.6.9/unstructured/partition/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition import _partition_via_api
 from unstructured.partition.common import (
     exactly_one,
     spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.strategies import determine_pdf_or_image_strategy
-from unstructured.partition.text import partition_text
+from unstructured.partition.text import element_from_text, partition_text
 from unstructured.utils import requires_dependencies
 
 
 @add_metadata_with_filetype(FileType.PDF)
 def partition_pdf(
     filename: str = "",
     file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
@@ -271,33 +271,35 @@
     include_page_breaks: bool = False,
 ):
     """Uses PDF miner to split a document into pages and process them."""
     elements: List[Element] = []
 
     for i, page in enumerate(extract_pages(fp)):  # type: ignore
         metadata = ElementMetadata(filename=filename, page_number=i + 1)
+        height = page.height
 
         text_segments = []
         for obj in page:
             # NOTE(robinson) - "Figure" is an example of an object type that does
             # not have a get_text method
+            x1, y2, x2, y1 = obj.bbox
+            y1 = height - y1
+            y2 = height - y2
+
             if not hasattr(obj, "get_text"):
                 continue
             _text = obj.get_text()
             _text = re.sub(PARAGRAPH_PATTERN, " ", _text)
             _text = clean_extra_whitespace(_text)
             if _text.strip():
                 text_segments.append(_text)
-
-        text = "\n\n".join(text_segments)
-
-        _elements = partition_text(text=text)
-        for element in _elements:
-            element.metadata = metadata
-            elements.append(element)
+                element = element_from_text(_text)
+                element.coordinates = ((x1, y1), (x1, y2), (x2, y2), (x2, y1))
+                element.metadata = metadata
+                elements.append(element)
 
         if include_page_breaks:
             elements.append(PageBreak())
 
     return elements
```

### Comparing `unstructured-0.6.8/unstructured/partition/ppt.py` & `unstructured-0.6.9/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/pptx.py` & `unstructured-0.6.9/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/rtf.py` & `unstructured-0.6.9/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/strategies.py` & `unstructured-0.6.9/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/text.py` & `unstructured-0.6.9/unstructured/partition/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Text,
     Title,
 )
+from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition.common import exactly_one
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
@@ -27,15 +28,15 @@
 
 
 @add_metadata_with_filetype(FileType.TXT)
 def partition_text(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
-    encoding: Optional[str] = "utf-8",
+    encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
 ) -> List[Element]:
     """Partitions an .txt documents into its constituent elements.
     Parameters
     ----------
@@ -56,24 +57,18 @@
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text)
 
     if filename is not None:
-        with open(filename, encoding=encoding) as f:
-            try:
-                file_text = f.read()
-            except (UnicodeDecodeError, UnicodeError) as error:
-                raise error
+        encoding, file_text = read_txt_file(filename=filename, encoding=encoding)
 
     elif file is not None:
-        file_text = file.read()
-        if isinstance(file_text, bytes):
-            file_text = file_text.decode(encoding)
+        encoding, file_text = read_txt_file(file=file, encoding=encoding)
 
     elif text is not None:
         file_text = str(text)
 
     if paragraph_grouper is not None:
         file_text = paragraph_grouper(file_text)
     else:
@@ -86,21 +81,26 @@
     elements: List[Element] = []
     metadata = (
         ElementMetadata(filename=metadata_filename) if include_metadata else ElementMetadata()
     )
     for ctext in file_content:
         ctext = ctext.strip()
 
-        if ctext == "":
-            continue
-        if is_bulleted_text(ctext):
-            elements.append(ListItem(text=clean_bullets(ctext), metadata=metadata))
-        elif is_us_city_state_zip(ctext):
-            elements.append(Address(text=ctext, metadata=metadata))
-        elif is_possible_narrative_text(ctext):
-            elements.append(NarrativeText(text=ctext, metadata=metadata))
-        elif is_possible_title(ctext):
-            elements.append(Title(text=ctext, metadata=metadata))
-        else:
-            elements.append(Text(text=ctext, metadata=metadata))
+        if ctext:
+            element = element_from_text(ctext)
+            element.metadata = metadata
+            elements.append(element)
 
     return elements
+
+
+def element_from_text(text: str) -> Element:
+    if is_bulleted_text(text):
+        return ListItem(text=clean_bullets(text))
+    elif is_us_city_state_zip(text):
+        return Address(text=text)
+    elif is_possible_narrative_text(text):
+        return NarrativeText(text=text)
+    elif is_possible_title(text):
+        return Title(text=text)
+    else:
+        return Text(text=text)
```

### Comparing `unstructured-0.6.8/unstructured/partition/text_type.py` & `unstructured-0.6.9/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/xlsx.py` & `unstructured-0.6.9/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/partition/xml.py` & `unstructured-0.6.9/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/argilla.py` & `unstructured-0.6.9/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/base.py` & `unstructured-0.6.9/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/baseplate.py` & `unstructured-0.6.9/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/datasaur.py` & `unstructured-0.6.9/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/huggingface.py` & `unstructured-0.6.9/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/label_box.py` & `unstructured-0.6.9/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/label_studio.py` & `unstructured-0.6.9/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/staging/prodigy.py` & `unstructured-0.6.9/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured/utils.py` & `unstructured-0.6.9/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.8/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.9/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.8
+Version: 0.6.9
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.9 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

