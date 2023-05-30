# Comparing `tmp/gisting-1.3.0.tar.gz` & `tmp/gisting-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting-1.3.0.tar", last modified: Tue May 30 05:05:18 2023, max compression
+gzip compressed data, was "gisting-1.3.1.tar", last modified: Tue May 30 05:11:54 2023, max compression
```

## Comparing `gisting-1.3.0.tar` & `gisting-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,29 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:05:18.167428 gisting-1.3.0/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      396 2023-05-30 05:05:18.167333 gisting-1.3.0/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:05:18.166593 gisting-1.3.0/gisting/
--rw-r--r--   0 owaiszahid   (501) staff       (20)       29 2023-05-30 04:41:16.000000 gisting-1.3.0/gisting/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:05:18.167204 gisting-1.3.0/gisting.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      396 2023-05-30 05:05:18.000000 gisting-1.3.0/gisting.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      182 2023-05-30 05:05:18.000000 gisting-1.3.0/gisting.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-05-30 05:05:18.000000 gisting-1.3.0/gisting.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)      225 2023-05-30 05:05:18.000000 gisting-1.3.0/gisting.egg-info/requires.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        8 2023-05-30 05:05:18.000000 gisting-1.3.0/gisting.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-05-30 05:05:18.167463 gisting-1.3.0/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      904 2023-05-30 05:04:59.000000 gisting-1.3.0/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:11:54.335621 gisting-1.3.1/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      396 2023-05-30 05:11:54.335507 gisting-1.3.1/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:11:54.331729 gisting-1.3.1/gisting/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       29 2023-05-30 04:41:16.000000 gisting-1.3.1/gisting/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:11:54.332581 gisting-1.3.1/gisting/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     6771 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/data/create_alpaca_plus_data.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:11:54.335328 gisting-1.3.1/gisting/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       25 2023-05-30 05:10:58.000000 gisting-1.3.1/gisting/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8737 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/compress.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 04:32:56.000000 gisting-1.3.1/gisting/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 05:11:54.332467 gisting-1.3.1/gisting.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      396 2023-05-30 05:11:54.000000 gisting-1.3.1/gisting.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      583 2023-05-30 05:11:54.000000 gisting-1.3.1/gisting.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-05-30 05:11:54.000000 gisting-1.3.1/gisting.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      225 2023-05-30 05:11:54.000000 gisting-1.3.1/gisting.egg-info/requires.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       33 2023-05-30 05:11:54.000000 gisting-1.3.1/gisting.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-05-30 05:11:54.335658 gisting-1.3.1/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      933 2023-05-30 05:11:24.000000 gisting-1.3.1/setup.py
```

