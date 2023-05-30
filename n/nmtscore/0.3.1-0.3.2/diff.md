# Comparing `tmp/nmtscore-0.3.1.tar.gz` & `tmp/nmtscore-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/java/Documents/nmtscore/dist/tmp_bjaf915/nmtscore-0.3.1.tar", last modified: Fri Feb 10 11:29:01 2023, max compression
+gzip compressed data, was "/home/java/Documents/nmtscore/dist/tmpazjy8it8/nmtscore-0.3.2.tar", last modified: Tue May 30 07:53:56 2023, max compression
```

## Comparing `nmtscore-0.3.1.tar` & `nmtscore-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 11:29:01.000000 nmtscore-0.3.1/
--rw-rw-r--   0 root         (0) root         (0)      103 2022-04-28 11:25:55.000000 nmtscore-0.3.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       37 2022-04-28 11:25:55.000000 nmtscore-0.3.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-02-10 11:29:01.000000 nmtscore-0.3.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      778 2023-02-10 11:29:01.000000 nmtscore-0.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore/
--rw-rw-r--   0 root         (0) root         (0)       61 2023-02-10 11:27:02.000000 nmtscore-0.3.1/src/nmtscore/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13446 2023-02-10 11:19:20.000000 nmtscore-0.3.1/src/nmtscore/scorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore/models/
--rw-rw-r--   0 root         (0) root         (0)      948 2023-01-08 17:34:57.000000 nmtscore-0.3.1/src/nmtscore/models/small100.py
--rw-rw-r--   0 root         (0) root         (0)     9794 2023-01-08 17:34:57.000000 nmtscore-0.3.1/src/nmtscore/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4708 2023-01-07 16:52:37.000000 nmtscore-0.3.1/src/nmtscore/models/m2m100.py
--rw-rw-r--   0 root         (0) root         (0)      176 2022-04-28 11:25:55.000000 nmtscore-0.3.1/src/nmtscore/models/utils.py
--rw-rw-r--   0 root         (0) root         (0)    15962 2023-01-06 05:44:09.000000 nmtscore-0.3.1/src/nmtscore/models/prism.py
--rw-rw-r--   0 root         (0) root         (0)    16232 2023-01-08 17:34:57.000000 nmtscore-0.3.1/src/nmtscore/models/tokenization_small100.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore.egg-info/
--rw-rw-r--   0 root         (0) root         (0)        9 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       79 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)     7048 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      475 2023-02-10 11:29:01.000000 nmtscore-0.3.1/src/nmtscore.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)     6467 2023-02-10 11:19:20.000000 nmtscore-0.3.1/README.md
--rw-rw-r--   0 root         (0) root         (0)     1070 2022-04-28 11:25:55.000000 nmtscore-0.3.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:53:56.000000 nmtscore-0.3.2/
+-rw-rw-r--   0 root         (0) root         (0)      103 2022-04-28 11:25:55.000000 nmtscore-0.3.2/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       37 2022-04-28 11:25:55.000000 nmtscore-0.3.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7250 2023-05-30 07:53:56.000000 nmtscore-0.3.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      778 2023-05-30 07:53:56.000000 nmtscore-0.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore/
+-rw-rw-r--   0 root         (0) root         (0)       61 2023-05-30 07:50:47.000000 nmtscore-0.3.2/src/nmtscore/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13446 2023-02-10 11:19:20.000000 nmtscore-0.3.2/src/nmtscore/scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore/models/
+-rw-rw-r--   0 root         (0) root         (0)      948 2023-01-08 17:34:57.000000 nmtscore-0.3.2/src/nmtscore/models/small100.py
+-rw-rw-r--   0 root         (0) root         (0)    10153 2023-05-26 12:55:01.000000 nmtscore-0.3.2/src/nmtscore/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4948 2023-05-26 12:56:31.000000 nmtscore-0.3.2/src/nmtscore/models/m2m100.py
+-rw-rw-r--   0 root         (0) root         (0)      176 2022-04-28 11:25:55.000000 nmtscore-0.3.2/src/nmtscore/models/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    15962 2023-01-06 05:44:09.000000 nmtscore-0.3.2/src/nmtscore/models/prism.py
+-rw-rw-r--   0 root         (0) root         (0)    16232 2023-01-08 17:34:57.000000 nmtscore-0.3.2/src/nmtscore/models/tokenization_small100.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)     7250 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      475 2023-05-30 07:53:56.000000 nmtscore-0.3.2/src/nmtscore.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)     6669 2023-05-30 07:46:27.000000 nmtscore-0.3.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)     1070 2022-04-28 11:25:55.000000 nmtscore-0.3.2/LICENSE
```

### Comparing `nmtscore-0.3.1/PKG-INFO` & `nmtscore-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmtscore
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library of translation-based text similarity measures
 Home-page: https://github.com/ZurichNLP/nmtscore
 Author: Jannis Vamvas
 Author-email: vamvas@cl.uzh.ch
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ZurichNLP/nmtscore/issues
 Platform: UNKNOWN
@@ -39,15 +39,15 @@
 
 ```python
 from nmtscore import NMTScorer
 
 scorer = NMTScorer()
 
 scorer.score("This is a sentence.", "This is another sentence.")
-# 0.45572562294591235
+# 0.5025776988808766
 ```
 
 #### Different similarity measures
 The library implements three different measures:
 
 ```python
 # Translation cross-likelihood (default)
@@ -66,15 +66,15 @@
 The scoring methods also accept lists of strings:
 
 ```python
 scorer.score(
     ["This is a sentence.", "This is a sentence.", "This is another sentence."],
     ["This is another sentence.", "This sentence is completely unrelated.", "This is another sentence."],
 )
-# [0.45572545262642583, 0.13128832336168145, 0.99999993180868]
+# [0.5025777998113548, 0.1640727324003354, 1.0000000000000049]
 ```
 
 The sentences in the first list are compared element-wise to the sentences in the second list.
 
 The default batch size is 8.
 An alternative batch size can be specified as follows (independently for translating and scoring):
 
@@ -90,15 +90,15 @@
     score_kwargs={"batch_size": 16}
 )
 ```
 
 #### Different NMT models
 This library currently supports four NMT models:
 - [`small100`](https://huggingface.co/alirezamsh/small100) by [Mohammadshahi et al. (2022)](https://aclanthology.org/2022.emnlp-main.571/)
-- [`m2m100_418M`](https://huggingface.co/facebook/m2m100_418M) and [`m2m100_1.2B`](https://huggingface.co/facebook/m2m100_1.2B) by [Fan et al. (2021)](https://www.jmlr.org/papers/volume22/20-1307/)
+- [`m2m100_418M`](https://huggingface.co/facebook/m2m100_418M) and [`m2m100_1.2B`](https://huggingface.co/facebook/m2m100_1.2B) by [Fan et al. (2021)](https://jmlr.org/papers/v22/20-1307.html)
 - [`prism`](https://github.com/thompsonb/prism) by [Thompson and Post (2020)](https://aclanthology.org/2020.emnlp-main.8/)
 
 By default, the leanest model (`small100`) is loaded. The main results in the paper are based on the Prism model, which has some extra dependencies (see "Installation" above).
 
 ```python
 scorer = NMTScorer("small100", device=None)  # default
 scorer = NMTScorer("small100", device="cuda:0")  # Enable faster inference on GPU
@@ -146,15 +146,15 @@
 
 model = load_translation_model("small100")
 
 model.translate("de", ["This is a test."])
 # ["Das ist ein Test."]
 
 model.score("de", ["This is a test."], ["Das ist ein Test."])
-# [0.8286197781562805]
+# [0.7708902359008789]
 ```
 
 ## Experiments
 See [experiments/README.md](experiments/README.md)
 
 ## Citation
 ```bibtex
@@ -173,14 +173,18 @@
 ```
 
 ## License
 - Code: MIT License
 - Data: See data subdirectories
 
 ## Changelog
+- v0.3.2
+  - Fix score calculation with `small100` model (account for the fact that the target sequence is not prefixed with the target language, as is the case for `m2m100`).
+  - Improve caching efficiency
+
 - v0.3.1
   - Implement the distilled [`small100`](https://huggingface.co/alirezamsh/small100) model by [Mohammadshahi et al. (2022)](https://aclanthology.org/2022.emnlp-main.571/) and use this model by default.
   - Enable half-precision inference for `m2m100` models and `small100` by default; see (/experiments/results/summary.md) for benchmark results
 
 - v0.2.0
   - Bugfix: Provide source language to `m2m100` models (#2). The fix is backwards-compatible but a warning is now raised if `m2m100` is used without specifying the input language.
```

### Comparing `nmtscore-0.3.1/setup.cfg` & `nmtscore-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nmtscore
-version = 0.3.1
+version = 0.3.2
 author = Jannis Vamvas
 author_email = vamvas@cl.uzh.ch
 description = A library of translation-based text similarity measures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ZurichNLP/nmtscore
 project_urls =
```

### Comparing `nmtscore-0.3.1/src/nmtscore/scorer.py` & `nmtscore-0.3.2/src/nmtscore/scorer.py`

 * *Files identical despite different names*

### Comparing `nmtscore-0.3.1/src/nmtscore/models/small100.py` & `nmtscore-0.3.2/src/nmtscore/models/small100.py`

 * *Files identical despite different names*

### Comparing `nmtscore-0.3.1/src/nmtscore/models/__init__.py` & `nmtscore-0.3.2/src/nmtscore/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
         self._set_tgt_lang(tgt_lang)
         if self.requires_src_lang:
             if src_lang is None:
                 warnings.warn(f"NMT model {self} requires the src language. Assuming 'en'; override with `src_lang`")
                 src_lang = "en"
             self._set_src_lang(src_lang)
-        translations_list = self._translate(source_sentences_list, return_score, batch_size, **kwargs)
+        if not source_sentences_list:
+            translations_list = []
+        else:
+            translations_list = self._translate(source_sentences_list, return_score, batch_size, **kwargs)
         assert len(translations_list) == len(source_sentences_list)
 
         if use_cache:
             cache_update = dict()
             for i, cached_translation in enumerate(cached_translations_list):
                 if cached_translation is not None:
                     translations_list.insert(i, cached_translation)
@@ -133,16 +136,22 @@
                 hypothesis_sentence for hypothesis_sentence, cached_score
                 in zip(full_hypothesis_sentences_list, cached_scores_list)
                 if cached_score is None
             ]
 
         self._set_tgt_lang(tgt_lang)
         if self.requires_src_lang:
+            if src_lang is None:
+                warnings.warn(f"NMT model {self} requires the src language. Assuming 'en'; override with `src_lang`")
+                src_lang = "en"
             self._set_src_lang(src_lang)
-        scores_list = self._score(source_sentences_list, hypothesis_sentences_list, batch_size, **kwargs)
+        if not source_sentences_list:
+            scores_list = []
+        else:
+            scores_list = self._score(source_sentences_list, hypothesis_sentences_list, batch_size, **kwargs)
         assert len(scores_list) == len(source_sentences_list)
 
         if use_cache:
             cache_update = dict()
             for i, cached_score in enumerate(cached_scores_list):
                 if cached_score is not None:
                     scores_list.insert(i, cached_score)
```

### Comparing `nmtscore-0.3.1/src/nmtscore/models/m2m100.py` & `nmtscore-0.3.2/src/nmtscore/models/m2m100.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import torch
 from tqdm import tqdm
 from transformers import M2M100ForConditionalGeneration, M2M100Tokenizer, TranslationPipeline
 from transformers.file_utils import PaddingStrategy
 from transformers.models.m2m_100.modeling_m2m_100 import shift_tokens_right
 
+from nmtscore.models.tokenization_small100 import SMALL100Tokenizer
 from nmtscore.models import TranslationModel
 from nmtscore.models.utils import batch
 
 
 class M2M100Model(TranslationModel):
     """
     Loads one of the models described in: Fan, Angela, et al. "Beyond english-centric multilingual machine
@@ -102,15 +103,19 @@
                 padding=padding_strategy,
             )
             inputs = inputs.to(self.model.device)
             inputs["labels"][inputs["labels"] == self.tokenizer.pad_token_id] = -100
             inputs["decoder_input_ids"] = shift_tokens_right(inputs["labels"], self.tokenizer.pad_token_id, self.model.config.decoder_start_token_id)
             output = self.model(**inputs)
             batch_scores = torch.zeros(len(src_sentences), device=self.model.device)
+            if isinstance(self.tokenizer, SMALL100Tokenizer):
+                offset = 0  # No language token in tgt
+            else:
+                offset = 1
             for i in range(len(src_sentences)):
                 loss = torch.nn.CrossEntropyLoss()(
-                    output.logits[i][1:].view(-1, self.model.config.vocab_size),
-                    inputs["labels"][i][1:].view(-1),
+                    output.logits[i][offset:].view(-1, self.model.config.vocab_size),
+                    inputs["labels"][i][offset:].view(-1),
                 )
                 batch_scores[i] = 2 ** (-loss)
             scores += batch_scores.tolist()
         return scores
```

### Comparing `nmtscore-0.3.1/src/nmtscore/models/prism.py` & `nmtscore-0.3.2/src/nmtscore/models/prism.py`

 * *Files identical despite different names*

### Comparing `nmtscore-0.3.1/src/nmtscore/models/tokenization_small100.py` & `nmtscore-0.3.2/src/nmtscore/models/tokenization_small100.py`

 * *Files identical despite different names*

### Comparing `nmtscore-0.3.1/src/nmtscore.egg-info/PKG-INFO` & `nmtscore-0.3.2/src/nmtscore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmtscore
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library of translation-based text similarity measures
 Home-page: https://github.com/ZurichNLP/nmtscore
 Author: Jannis Vamvas
 Author-email: vamvas@cl.uzh.ch
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ZurichNLP/nmtscore/issues
 Platform: UNKNOWN
@@ -39,15 +39,15 @@
 
 ```python
 from nmtscore import NMTScorer
 
 scorer = NMTScorer()
 
 scorer.score("This is a sentence.", "This is another sentence.")
-# 0.45572562294591235
+# 0.5025776988808766
 ```
 
 #### Different similarity measures
 The library implements three different measures:
 
 ```python
 # Translation cross-likelihood (default)
@@ -66,15 +66,15 @@
 The scoring methods also accept lists of strings:
 
 ```python
 scorer.score(
     ["This is a sentence.", "This is a sentence.", "This is another sentence."],
     ["This is another sentence.", "This sentence is completely unrelated.", "This is another sentence."],
 )
-# [0.45572545262642583, 0.13128832336168145, 0.99999993180868]
+# [0.5025777998113548, 0.1640727324003354, 1.0000000000000049]
 ```
 
 The sentences in the first list are compared element-wise to the sentences in the second list.
 
 The default batch size is 8.
 An alternative batch size can be specified as follows (independently for translating and scoring):
 
@@ -90,15 +90,15 @@
     score_kwargs={"batch_size": 16}
 )
 ```
 
 #### Different NMT models
 This library currently supports four NMT models:
 - [`small100`](https://huggingface.co/alirezamsh/small100) by [Mohammadshahi et al. (2022)](https://aclanthology.org/2022.emnlp-main.571/)
-- [`m2m100_418M`](https://huggingface.co/facebook/m2m100_418M) and [`m2m100_1.2B`](https://huggingface.co/facebook/m2m100_1.2B) by [Fan et al. (2021)](https://www.jmlr.org/papers/volume22/20-1307/)
+- [`m2m100_418M`](https://huggingface.co/facebook/m2m100_418M) and [`m2m100_1.2B`](https://huggingface.co/facebook/m2m100_1.2B) by [Fan et al. (2021)](https://jmlr.org/papers/v22/20-1307.html)
 - [`prism`](https://github.com/thompsonb/prism) by [Thompson and Post (2020)](https://aclanthology.org/2020.emnlp-main.8/)
 
 By default, the leanest model (`small100`) is loaded. The main results in the paper are based on the Prism model, which has some extra dependencies (see "Installation" above).
 
 ```python
 scorer = NMTScorer("small100", device=None)  # default
 scorer = NMTScorer("small100", device="cuda:0")  # Enable faster inference on GPU
@@ -146,15 +146,15 @@
 
 model = load_translation_model("small100")
 
 model.translate("de", ["This is a test."])
 # ["Das ist ein Test."]
 
 model.score("de", ["This is a test."], ["Das ist ein Test."])
-# [0.8286197781562805]
+# [0.7708902359008789]
 ```
 
 ## Experiments
 See [experiments/README.md](experiments/README.md)
 
 ## Citation
 ```bibtex
@@ -173,14 +173,18 @@
 ```
 
 ## License
 - Code: MIT License
 - Data: See data subdirectories
 
 ## Changelog
+- v0.3.2
+  - Fix score calculation with `small100` model (account for the fact that the target sequence is not prefixed with the target language, as is the case for `m2m100`).
+  - Improve caching efficiency
+
 - v0.3.1
   - Implement the distilled [`small100`](https://huggingface.co/alirezamsh/small100) model by [Mohammadshahi et al. (2022)](https://aclanthology.org/2022.emnlp-main.571/) and use this model by default.
   - Enable half-precision inference for `m2m100` models and `small100` by default; see (/experiments/results/summary.md) for benchmark results
 
 - v0.2.0
   - Bugfix: Provide source language to `m2m100` models (#2). The fix is backwards-compatible but a warning is now raised if `m2m100` is used without specifying the input language.
```

### Comparing `nmtscore-0.3.1/README.md` & `nmtscore-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ```python
 from nmtscore import NMTScorer
 
 scorer = NMTScorer()
 
 scorer.score("This is a sentence.", "This is another sentence.")
-# 0.45572562294591235
+# 0.5025776988808766
 ```
 
 #### Different similarity measures
 The library implements three different measures:
 
 ```python
 # Translation cross-likelihood (default)
@@ -48,15 +48,15 @@
 The scoring methods also accept lists of strings:
 
 ```python
 scorer.score(
     ["This is a sentence.", "This is a sentence.", "This is another sentence."],
     ["This is another sentence.", "This sentence is completely unrelated.", "This is another sentence."],
 )
-# [0.45572545262642583, 0.13128832336168145, 0.99999993180868]
+# [0.5025777998113548, 0.1640727324003354, 1.0000000000000049]
 ```
 
 The sentences in the first list are compared element-wise to the sentences in the second list.
 
 The default batch size is 8.
 An alternative batch size can be specified as follows (independently for translating and scoring):
 
@@ -72,15 +72,15 @@
     score_kwargs={"batch_size": 16}
 )
 ```
 
 #### Different NMT models
 This library currently supports four NMT models:
 - [`small100`](https://huggingface.co/alirezamsh/small100) by [Mohammadshahi et al. (2022)](https://aclanthology.org/2022.emnlp-main.571/)
-- [`m2m100_418M`](https://huggingface.co/facebook/m2m100_418M) and [`m2m100_1.2B`](https://huggingface.co/facebook/m2m100_1.2B) by [Fan et al. (2021)](https://www.jmlr.org/papers/volume22/20-1307/)
+- [`m2m100_418M`](https://huggingface.co/facebook/m2m100_418M) and [`m2m100_1.2B`](https://huggingface.co/facebook/m2m100_1.2B) by [Fan et al. (2021)](https://jmlr.org/papers/v22/20-1307.html)
 - [`prism`](https://github.com/thompsonb/prism) by [Thompson and Post (2020)](https://aclanthology.org/2020.emnlp-main.8/)
 
 By default, the leanest model (`small100`) is loaded. The main results in the paper are based on the Prism model, which has some extra dependencies (see "Installation" above).
 
 ```python
 scorer = NMTScorer("small100", device=None)  # default
 scorer = NMTScorer("small100", device="cuda:0")  # Enable faster inference on GPU
@@ -128,15 +128,15 @@
 
 model = load_translation_model("small100")
 
 model.translate("de", ["This is a test."])
 # ["Das ist ein Test."]
 
 model.score("de", ["This is a test."], ["Das ist ein Test."])
-# [0.8286197781562805]
+# [0.7708902359008789]
 ```
 
 ## Experiments
 See [experiments/README.md](experiments/README.md)
 
 ## Citation
 ```bibtex
@@ -155,13 +155,17 @@
 ```
 
 ## License
 - Code: MIT License
 - Data: See data subdirectories
 
 ## Changelog
+- v0.3.2
+  - Fix score calculation with `small100` model (account for the fact that the target sequence is not prefixed with the target language, as is the case for `m2m100`).
+  - Improve caching efficiency
+
 - v0.3.1
   - Implement the distilled [`small100`](https://huggingface.co/alirezamsh/small100) model by [Mohammadshahi et al. (2022)](https://aclanthology.org/2022.emnlp-main.571/) and use this model by default.
   - Enable half-precision inference for `m2m100` models and `small100` by default; see (/experiments/results/summary.md) for benchmark results
 
 - v0.2.0
   - Bugfix: Provide source language to `m2m100` models (#2). The fix is backwards-compatible but a warning is now raised if `m2m100` is used without specifying the input language.
```

### Comparing `nmtscore-0.3.1/LICENSE` & `nmtscore-0.3.2/LICENSE`

 * *Files identical despite different names*

