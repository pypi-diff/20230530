# Comparing `tmp/lmflow-finetune-0.0.1.tar.gz` & `tmp/lmflow-finetune-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmflow-finetune-0.0.1.tar", last modified: Tue May 30 07:51:21 2023, max compression
+gzip compressed data, was "lmflow-finetune-0.0.2.tar", last modified: Tue May 30 08:39:38 2023, max compression
```

## Comparing `lmflow-finetune-0.0.1.tar` & `lmflow-finetune-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.298524 lmflow-finetune-0.0.1/
--rw-r--r--   0 kashun     (501) staff       (20)    11356 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/LICENSE
--rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-05-30 07:51:21.298302 lmflow-finetune-0.0.1/PKG-INFO
--rw-r--r--   0 kashun     (501) staff       (20)    22653 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.1/README.md
--rw-r--r--   0 kashun     (501) staff       (20)       38 2023-05-30 07:51:21.298584 lmflow-finetune-0.0.1/setup.cfg
--rw-r--r--   0 kashun     (501) staff       (20)     1545 2023-05-30 07:51:18.000000 lmflow-finetune-0.0.1/setup.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.286156 lmflow-finetune-0.0.1/src/
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.288110 lmflow-finetune-0.0.1/src/lmflow/
--rw-r--r--   0 kashun     (501) staff       (20)      494 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)    20014 2023-05-30 06:32:32.000000 lmflow-finetune-0.0.1/src/lmflow/args.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.288612 lmflow-finetune-0.0.1/src/lmflow/datasets/
--rw-r--r--   0 kashun     (501) staff       (20)      387 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/datasets/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)    11619 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.1/src/lmflow/datasets/dataset.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.292172 lmflow-finetune-0.0.1/src/lmflow/models/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/models/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)      887 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/models/auto_model.py
--rw-r--r--   0 kashun     (501) staff       (20)      162 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/models/base_model.py
--rw-r--r--   0 kashun     (501) staff       (20)      544 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/models/decoder_model.py
--rw-r--r--   0 kashun     (501) staff       (20)      550 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/models/encoder_decoder_model.py
--rw-r--r--   0 kashun     (501) staff       (20)    24039 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.1/src/lmflow/models/hf_decoder_model.py
--rw-r--r--   0 kashun     (501) staff       (20)    11568 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/models/hf_encoder_decoder_model.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.292562 lmflow-finetune-0.0.1/src/lmflow/models/interfaces/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/models/interfaces/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)      110 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/models/interfaces/tunable.py
--rw-r--r--   0 kashun     (501) staff       (20)      208 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.1/src/lmflow/models/regression_model.py
--rw-r--r--   0 kashun     (501) staff       (20)     1304 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/models/text_regression_model.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.294663 lmflow-finetune-0.0.1/src/lmflow/pipeline/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)     1042 2023-05-30 06:30:04.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/auto_pipeline.py
--rw-r--r--   0 kashun     (501) staff       (20)      593 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/base_aligner.py
--rw-r--r--   0 kashun     (501) staff       (20)      140 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/base_pipeline.py
--rw-r--r--   0 kashun     (501) staff       (20)      522 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/base_tuner.py
--rw-r--r--   0 kashun     (501) staff       (20)    12694 2023-05-30 06:25:08.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/finetuner.py
--rw-r--r--   0 kashun     (501) staff       (20)     6683 2023-05-02 23:11:41.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/inferencer.py
--rw-r--r--   0 kashun     (501) staff       (20)    17246 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/raft_aligner.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.295222 lmflow-finetune-0.0.1/src/lmflow/pipeline/utils/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/utils/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)   185721 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.1/src/lmflow/pipeline/utils/raft_trainer.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.296338 lmflow-finetune-0.0.1/src/lmflow/utils/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.1/src/lmflow/utils/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)     3884 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.1/src/lmflow/utils/constants.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.297074 lmflow-finetune-0.0.1/src/lmflow/utils/flash_attention/
--rw-r--r--   0 kashun     (501) staff       (20)        0 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.1/src/lmflow/utils/flash_attention/__init__.py
--rw-r--r--   0 kashun     (501) staff       (20)     3649 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.1/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py
--rw-r--r--   0 kashun     (501) staff       (20)     4052 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.1/src/lmflow/utils/flash_attention/llama_flash_attention.py
--rw-r--r--   0 kashun     (501) staff       (20)       21 2023-05-30 07:45:52.000000 lmflow-finetune-0.0.1/src/lmflow/version.py
-drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 07:51:21.297977 lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/
--rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-05-30 07:51:21.000000 lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/PKG-INFO
--rw-r--r--   0 kashun     (501) staff       (20)     1366 2023-05-30 07:51:21.000000 lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/SOURCES.txt
--rw-r--r--   0 kashun     (501) staff       (20)        1 2023-05-30 07:51:21.000000 lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/dependency_links.txt
--rw-r--r--   0 kashun     (501) staff       (20)      200 2023-05-30 07:51:21.000000 lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/requires.txt
--rw-r--r--   0 kashun     (501) staff       (20)        7 2023-05-30 07:51:21.000000 lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/top_level.txt
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.005690 lmflow-finetune-0.0.2/
+-rw-r--r--   0 kashun     (501) staff       (20)    11356 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/LICENSE
+-rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-05-30 08:39:38.005424 lmflow-finetune-0.0.2/PKG-INFO
+-rw-r--r--   0 kashun     (501) staff       (20)    22653 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/README.md
+-rw-r--r--   0 kashun     (501) staff       (20)       38 2023-05-30 08:39:38.005756 lmflow-finetune-0.0.2/setup.cfg
+-rw-r--r--   0 kashun     (501) staff       (20)     1545 2023-05-30 08:38:19.000000 lmflow-finetune-0.0.2/setup.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.993582 lmflow-finetune-0.0.2/src/
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.995258 lmflow-finetune-0.0.2/src/lmflow/
+-rw-r--r--   0 kashun     (501) staff       (20)      494 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)    19977 2023-05-30 08:37:31.000000 lmflow-finetune-0.0.2/src/lmflow/args.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.995688 lmflow-finetune-0.0.2/src/lmflow/datasets/
+-rw-r--r--   0 kashun     (501) staff       (20)      387 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/datasets/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)    11619 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/datasets/dataset.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.998644 lmflow-finetune-0.0.2/src/lmflow/models/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)      887 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/auto_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)      162 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/base_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)      544 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/decoder_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)      550 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/encoder_decoder_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)    24039 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/models/hf_decoder_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)    11568 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/hf_encoder_decoder_model.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:37.999131 lmflow-finetune-0.0.2/src/lmflow/models/interfaces/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/interfaces/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)      110 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/models/interfaces/tunable.py
+-rw-r--r--   0 kashun     (501) staff       (20)      208 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/models/regression_model.py
+-rw-r--r--   0 kashun     (501) staff       (20)     1304 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/models/text_regression_model.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.001248 lmflow-finetune-0.0.2/src/lmflow/pipeline/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     1042 2023-05-30 06:30:04.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/auto_pipeline.py
+-rw-r--r--   0 kashun     (501) staff       (20)      593 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/base_aligner.py
+-rw-r--r--   0 kashun     (501) staff       (20)      140 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/base_pipeline.py
+-rw-r--r--   0 kashun     (501) staff       (20)      522 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/base_tuner.py
+-rw-r--r--   0 kashun     (501) staff       (20)    12694 2023-05-30 06:25:08.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/finetuner.py
+-rw-r--r--   0 kashun     (501) staff       (20)     6683 2023-05-02 23:11:41.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/inferencer.py
+-rw-r--r--   0 kashun     (501) staff       (20)    17246 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/raft_aligner.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.001833 lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)   185721 2023-04-09 13:27:35.000000 lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/raft_trainer.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.003301 lmflow-finetune-0.0.2/src/lmflow/utils/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-03-31 09:45:12.000000 lmflow-finetune-0.0.2/src/lmflow/utils/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     3884 2023-05-02 10:29:51.000000 lmflow-finetune-0.0.2/src/lmflow/utils/constants.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.003983 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/
+-rw-r--r--   0 kashun     (501) staff       (20)        0 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/__init__.py
+-rw-r--r--   0 kashun     (501) staff       (20)     3649 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py
+-rw-r--r--   0 kashun     (501) staff       (20)     4052 2023-05-26 07:38:34.000000 lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/llama_flash_attention.py
+-rw-r--r--   0 kashun     (501) staff       (20)       21 2023-05-30 08:38:29.000000 lmflow-finetune-0.0.2/src/lmflow/version.py
+drwxr-xr-x   0 kashun     (501) staff       (20)        0 2023-05-30 08:39:38.005082 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/
+-rw-r--r--   0 kashun     (501) staff       (20)    23006 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/PKG-INFO
+-rw-r--r--   0 kashun     (501) staff       (20)     1366 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/SOURCES.txt
+-rw-r--r--   0 kashun     (501) staff       (20)        1 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/dependency_links.txt
+-rw-r--r--   0 kashun     (501) staff       (20)      200 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/requires.txt
+-rw-r--r--   0 kashun     (501) staff       (20)        7 2023-05-30 08:39:37.000000 lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/top_level.txt
```

### Comparing `lmflow-finetune-0.0.1/LICENSE` & `lmflow-finetune-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/PKG-INFO` & `lmflow-finetune-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmflow-finetune
-Version: 0.0.1
+Version: 0.0.2
 Summary: LMFlow: Large Model Flow.
 Author: The LMFlow Team
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.1 Summary: LMFlow:
+Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.2 Summary: LMFlow:
 Large Model Flow. Author: The LMFlow Team Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
 Content-Type: text/markdown License-File: LICENSE
                                    [LMFlow]
 # LMFlow
 *** English | ç®ä½ä¸­æ | EspaÃ±ol | æ¥æ¬èª | íêµ­ì´ | à¤¹à¤¿à¤à¤¦à¥
```

### Comparing `lmflow-finetune-0.0.1/README.md` & `lmflow-finetune-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/setup.py` & `lmflow-finetune-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/args.py` & `lmflow-finetune-0.0.2/src/lmflow/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,15 +526,14 @@
                 "ter", "r@1", "r@2", "mrr", "mc1", "mc2", "word_perplexity", \
                     "byte_perplexity", "bits_per_byte"],
         },
     )
 
 PIPELINE_ARGUMENT_MAPPING = {
     "finetuner": FinetunerArguments,
-    "evaluator": EvaluatorArguments,
     "inferencer": InferencerArguments,
     "raft_aligner": RaftAlignerArguments,
 }
 
 
 class AutoArguments:
     """
```

### Comparing `lmflow-finetune-0.0.1/src/lmflow/datasets/dataset.py` & `lmflow-finetune-0.0.2/src/lmflow/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/models/auto_model.py` & `lmflow-finetune-0.0.2/src/lmflow/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/models/decoder_model.py` & `lmflow-finetune-0.0.2/src/lmflow/models/decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/models/encoder_decoder_model.py` & `lmflow-finetune-0.0.2/src/lmflow/models/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/models/hf_decoder_model.py` & `lmflow-finetune-0.0.2/src/lmflow/models/hf_decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/models/hf_encoder_decoder_model.py` & `lmflow-finetune-0.0.2/src/lmflow/models/hf_encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/models/text_regression_model.py` & `lmflow-finetune-0.0.2/src/lmflow/models/text_regression_model.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/auto_pipeline.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/auto_pipeline.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/base_aligner.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/base_aligner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/base_tuner.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/base_tuner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/finetuner.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/finetuner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/inferencer.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/inferencer.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/raft_aligner.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/raft_aligner.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/pipeline/utils/raft_trainer.py` & `lmflow-finetune-0.0.2/src/lmflow/pipeline/utils/raft_trainer.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/utils/constants.py` & `lmflow-finetune-0.0.2/src/lmflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py` & `lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/gpt_neo_flash_attention.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow/utils/flash_attention/llama_flash_attention.py` & `lmflow-finetune-0.0.2/src/lmflow/utils/flash_attention/llama_flash_attention.py`

 * *Files identical despite different names*

### Comparing `lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/PKG-INFO` & `lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmflow-finetune
-Version: 0.0.1
+Version: 0.0.2
 Summary: LMFlow: Large Model Flow.
 Author: The LMFlow Team
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.1 Summary: LMFlow:
+Metadata-Version: 2.1 Name: lmflow-finetune Version: 0.0.2 Summary: LMFlow:
 Large Model Flow. Author: The LMFlow Team Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
 Content-Type: text/markdown License-File: LICENSE
                                    [LMFlow]
 # LMFlow
 *** English | ç®ä½ä¸­æ | EspaÃ±ol | æ¥æ¬èª | íêµ­ì´ | à¤¹à¤¿à¤à¤¦à¥
```

### Comparing `lmflow-finetune-0.0.1/src/lmflow_finetune.egg-info/SOURCES.txt` & `lmflow-finetune-0.0.2/src/lmflow_finetune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

