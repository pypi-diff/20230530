# Comparing `tmp/pythainlp-4.0.1.tar.gz` & `tmp/pythainlp-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythainlp-4.0.1.tar", last modified: Wed May  3 09:06:54 2023, max compression
+gzip compressed data, was "pythainlp-4.0.2.tar", last modified: Tue May 30 17:13:13 2023, max compression
```

## Comparing `pythainlp-4.0.1.tar` & `pythainlp-4.0.2.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.004006 pythainlp-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-05-03 09:06:40.000000 pythainlp-4.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-03 09:06:40.000000 pythainlp-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-03 09:06:40.000000 pythainlp-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-03 09:06:54.004006 pythainlp-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-05-03 09:06:40.000000 pythainlp-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-05-03 09:06:40.000000 pythainlp-4.0.1/README_TH.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.988005 pythainlp-4.0.1/pythainlp/
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.988005 pythainlp-4.0.1/pythainlp/augment/
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.988005 pythainlp-4.0.1/pythainlp/augment/lm/
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/lm/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/lm/wangchanberta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.988005 pythainlp-4.0.1/pythainlp/augment/word2vec/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/word2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/word2vec/bpemb_wv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/word2vec/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/word2vec/ltw2v.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/word2vec/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/augment/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.988005 pythainlp-4.0.1/pythainlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/benchmarks/word_tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/cli/soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/cli/tag.py
--rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/cli/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/oscar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/th_en_translit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/tnc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/ttc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/corpus/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/generate/
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/generate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/generate/thai2fit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/khavee/
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/khavee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20671 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/khavee/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     6579 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/khavee/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/parse/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/parse/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/parse/esupar_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/parse/spacy_thai_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/parse/transformers_ud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/parse/ud_goeswith.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/soundex/
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/soundex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/soundex/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/soundex/lk82.py
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/soundex/metasound.py
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/soundex/prayut_and_somchaip.py
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/soundex/udom83.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.992005 pythainlp-4.0.1/pythainlp/spell/
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/spell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/spell/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/spell/phunspell.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/spell/pn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/spell/symspellpy.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/spell/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.996006 pythainlp-4.0.1/pythainlp/summarize/
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/summarize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/summarize/freq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/summarize/keybert.py
--rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/summarize/mt5.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.996006 pythainlp-4.0.1/pythainlp/tag/
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/_tag_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/chunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/crfchunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/locations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/orchid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/pos_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/thai_nner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/thainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/unigram.py
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tag/wangchanberta_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.000006 pythainlp-4.0.1/pythainlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/attacut.py
--rw-r--r--   0 runner    (1001) docker     (122)    26351 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/crfcls.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/crfcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/deepcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/etcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/longest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/multi_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/nercut.py
--rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/newmm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/nlpo3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/oskut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/sefr_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/ssg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/tcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/tcc_p.py
--rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/thaisumcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tokenize/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.000006 pythainlp-4.0.1/pythainlp/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tools/misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/tools/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.000006 pythainlp-4.0.1/pythainlp/translate/
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3440 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/translate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/translate/en_th.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/translate/th_fr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/translate/zh_th.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.000006 pythainlp-4.0.1/pythainlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/ipa.py
--rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/iso_11940.py
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/royin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/spoonerism.py
--rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/thai2rom.py
--rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/thai2rom_onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/thaig2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/w2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     5847 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/transliterate/wunsen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.000006 pythainlp-4.0.1/pythainlp/ulmfit/
--rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/ulmfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/ulmfit/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/ulmfit/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/ulmfit/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.004006 pythainlp-4.0.1/pythainlp/util/
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/emojiconv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/keywords.py
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/numtoword.py
--rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/phoneme.py
--rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/strftime.py
--rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/syllable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/thai.py
--rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/util/wordtonum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.004006 pythainlp-4.0.1/pythainlp/wangchanberta/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/wangchanberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/wangchanberta/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.004006 pythainlp-4.0.1/pythainlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-05-03 09:06:40.000000 pythainlp-4.0.1/pythainlp/word_vector/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:53.988005 pythainlp-4.0.1/pythainlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-03 09:06:53.000000 pythainlp-4.0.1/pythainlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-03 09:06:54.004006 pythainlp-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-05-03 09:06:40.000000 pythainlp-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.004006 pythainlp-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:06:54.004006 pythainlp-4.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/data/eval-details-input.json
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/data/eval-input.yml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/data/input.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/data/sentences.yml
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_khavee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)    55078 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_transliterate.py
--rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_ulmfit.py
--rw-r--r--   0 runner    (1001) docker     (122)    36563 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_wangchanberta.py
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-03 09:06:40.000000 pythainlp-4.0.1/tests/test_word_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.050603 pythainlp-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-05-30 17:13:02.000000 pythainlp-4.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-30 17:13:02.000000 pythainlp-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-30 17:13:02.000000 pythainlp-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-30 17:13:13.054603 pythainlp-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-05-30 17:13:02.000000 pythainlp-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-05-30 17:13:02.000000 pythainlp-4.0.2/README_TH.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/augment/
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/augment/lm/
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/lm/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/lm/wangchanberta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/augment/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/bpemb_wv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/ltw2v.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/benchmarks/word_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/oscar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/th_en_translit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/tnc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/ttc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/generate/
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/generate/thai2fit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/khavee/
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/khavee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20881 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/khavee/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/khavee/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/parse/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/esupar_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/spacy_thai_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/transformers_ud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/ud_goeswith.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/soundex/
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/lk82.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/metasound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/prayut_and_somchaip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/udom83.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/spell/
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/phunspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/pn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/symspellpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/tltk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/summarize/
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/freq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/keybert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/mt5.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.038602 pythainlp-4.0.2/pythainlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/_tag_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/crfchunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/orchid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/pos_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/thai_nner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/thainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/unigram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/wangchanberta_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/attacut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26351 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/crfcls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/crfcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/deepcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/etcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/longest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/multi_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/nercut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/newmm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/nlpo3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/oskut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/sefr_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/ssg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/tcc_p.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/thaisumcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/tltk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tools/misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tools/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3440 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/en_th.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/th_fr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/zh_th.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/iso_11940.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/royin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/spoonerism.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/thai2rom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/thai2rom_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/thaig2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/w2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5847 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/wunsen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/ulmfit/
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/emojiconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/numtoword.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/phoneme.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/syllable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/thai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/wordtonum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/wangchanberta/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/wangchanberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/wangchanberta/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/word_vector/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-30 17:13:13.054603 pythainlp-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-05-30 17:13:02.000000 pythainlp-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.050603 pythainlp-4.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.050603 pythainlp-4.0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/eval-details-input.json
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/eval-input.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/input.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/sentences.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_khavee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55078 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_ulmfit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36563 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_wangchanberta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_word_vector.py
```

### Comparing `pythainlp-4.0.1/CONTRIBUTING.md` & `pythainlp-4.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/LICENSE` & `pythainlp-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/PKG-INFO` & `pythainlp-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 4.0.1
+Version: 4.0.2
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
```

### Comparing `pythainlp-4.0.1/README.md` & `pythainlp-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/README_TH.md` & `pythainlp-4.0.2/README_TH.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/__init__.py` & `pythainlp-4.0.2/pythainlp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # URL: <https://pythainlp.github.io/>
 # For license information, see LICENSE
-__version__ = "4.0.1"
+__version__ = "4.0.2"
 
 thai_consonants = "กขฃคฅฆงจฉชซฌญฎฏฐฑฒณดตถทธนบปผฝพฟภมยรลวศษสหฬอฮ"  # 44 chars
 
 thai_vowels = (
     "\u0e24\u0e26\u0e30\u0e31\u0e32\u0e33\u0e34\u0e35\u0e36\u0e37"
     + "\u0e38\u0e39\u0e40\u0e41\u0e42\u0e43\u0e44\u0e45\u0e4d\u0e47"
 )  # 20
```

### Comparing `pythainlp-4.0.1/pythainlp/__main__.py` & `pythainlp-4.0.2/pythainlp/__main__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/__init__.py` & `pythainlp-4.0.2/pythainlp/augment/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/lm/__init__.py` & `pythainlp-4.0.2/pythainlp/augment/lm/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/lm/fasttext.py` & `pythainlp-4.0.2/pythainlp/augment/lm/fasttext.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/lm/wangchanberta.py` & `pythainlp-4.0.2/pythainlp/augment/lm/wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/word2vec/__init__.py` & `pythainlp-4.0.2/pythainlp/augment/word2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/word2vec/bpemb_wv.py` & `pythainlp-4.0.2/pythainlp/augment/word2vec/bpemb_wv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/word2vec/core.py` & `pythainlp-4.0.2/pythainlp/augment/word2vec/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/word2vec/ltw2v.py` & `pythainlp-4.0.2/pythainlp/augment/word2vec/ltw2v.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/word2vec/thai2fit.py` & `pythainlp-4.0.2/pythainlp/augment/word2vec/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/augment/wordnet.py` & `pythainlp-4.0.2/pythainlp/augment/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/benchmarks/__init__.py` & `pythainlp-4.0.2/pythainlp/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/benchmarks/word_tokenization.py` & `pythainlp-4.0.2/pythainlp/benchmarks/word_tokenization.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/cli/__init__.py` & `pythainlp-4.0.2/pythainlp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/cli/benchmark.py` & `pythainlp-4.0.2/pythainlp/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/cli/data.py` & `pythainlp-4.0.2/pythainlp/cli/data.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/cli/soundex.py` & `pythainlp-4.0.2/pythainlp/cli/soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/cli/tag.py` & `pythainlp-4.0.2/pythainlp/cli/tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/cli/tokenize.py` & `pythainlp-4.0.2/pythainlp/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/__init__.py` & `pythainlp-4.0.2/pythainlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/common.py` & `pythainlp-4.0.2/pythainlp/corpus/common.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/conceptnet.py` & `pythainlp-4.0.2/pythainlp/corpus/conceptnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/core.py` & `pythainlp-4.0.2/pythainlp/corpus/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/oscar.py` & `pythainlp-4.0.2/pythainlp/corpus/oscar.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/th_en_translit.py` & `pythainlp-4.0.2/pythainlp/corpus/th_en_translit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/tnc.py` & `pythainlp-4.0.2/pythainlp/corpus/tnc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/ttc.py` & `pythainlp-4.0.2/pythainlp/corpus/ttc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/util.py` & `pythainlp-4.0.2/pythainlp/corpus/util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/corpus/wordnet.py` & `pythainlp-4.0.2/pythainlp/corpus/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/generate/__init__.py` & `pythainlp-4.0.2/pythainlp/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/generate/core.py` & `pythainlp-4.0.2/pythainlp/generate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/generate/thai2fit.py` & `pythainlp-4.0.2/pythainlp/generate/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/khavee/__init__.py` & `pythainlp-4.0.2/pythainlp/khavee/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/khavee/core.py` & `pythainlp-4.0.2/pythainlp/khavee/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,18 +180,23 @@
                 sara.append('โอะ')
             else:
                 sara.append('ออ') 
         elif sara == [] and len(word) == 3:
             sara.append('ออ') 
         
         # incase บ่ 
-        if 'บ่' in word:
+        if 'บ่' == word:
             sara = []
             sara.append('ออ')
-
+        if 'ํ' in word:
+            sara = []
+            sara.append('อำ')
+        if 'เ' in word and 'ื' in word and 'อ' in word:
+            sara = []
+            sara.append('เอือ')
         if sara == []:  
             return 'Cant find Sara in this word'
         else:
             return sara[0]
 
 
     def check_marttra(self, word: str) -> str:
```

### Comparing `pythainlp-4.0.1/pythainlp/khavee/example.py` & `pythainlp-4.0.2/pythainlp/khavee/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 # 'เกอว'
 
 # การตรวจสอบคำสำผัสที่ถูกต้อง
 print('สรร อัน',kv.is_sumpus('สรร','อัน'))
 # True
 
 # การตรวจสอบคำสำผัสที่ผิด
-print('สรร ขวาน',kv.is_sumpus('สรร','ขวาน'))
+print('เพื่อน ล้วน',kv.is_sumpus('เพื่อน','ล้วน'))
 # False
 
 # การตรวจสอบคำ ครุ ลหุ 
 print('สรร',kv.check_karu_lahu('สรร'))
 #karu
+
 # การตรวจสอบคำ ครุ ลหุ 
 print('ชิชะ',kv.check_karu_lahu('ชิชะ'))
 # lahu
 
 # การตรวจสอบกลอน 8 ที่ถูกฉันทลักษณ์
 print(kv.check_klon('''ณรงค์วุฒิผู้เปี่ยมวุฒิสมสง่า มากวิชาหาความรู้ไปสู่ผล 
 เรื่องฟิสิกส์คณิตศาสตร์เอิร์นอดทน เล่นเกมเก่งลำดับต้นของโรงเรียน
```

### Comparing `pythainlp-4.0.1/pythainlp/parse/__init__.py` & `pythainlp-4.0.2/pythainlp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/parse/core.py` & `pythainlp-4.0.2/pythainlp/parse/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/parse/esupar_engine.py` & `pythainlp-4.0.2/pythainlp/parse/esupar_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/parse/spacy_thai_engine.py` & `pythainlp-4.0.2/pythainlp/parse/spacy_thai_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/parse/transformers_ud.py` & `pythainlp-4.0.2/pythainlp/parse/transformers_ud.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/parse/ud_goeswith.py` & `pythainlp-4.0.2/pythainlp/parse/ud_goeswith.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/soundex/__init__.py` & `pythainlp-4.0.2/pythainlp/soundex/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/soundex/core.py` & `pythainlp-4.0.2/pythainlp/soundex/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/soundex/lk82.py` & `pythainlp-4.0.2/pythainlp/soundex/lk82.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/soundex/metasound.py` & `pythainlp-4.0.2/pythainlp/soundex/metasound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/soundex/prayut_and_somchaip.py` & `pythainlp-4.0.2/pythainlp/soundex/prayut_and_somchaip.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/soundex/udom83.py` & `pythainlp-4.0.2/pythainlp/soundex/udom83.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/spell/__init__.py` & `pythainlp-4.0.2/pythainlp/spell/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/spell/core.py` & `pythainlp-4.0.2/pythainlp/spell/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/spell/phunspell.py` & `pythainlp-4.0.2/pythainlp/spell/phunspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/spell/pn.py` & `pythainlp-4.0.2/pythainlp/spell/pn.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/spell/symspellpy.py` & `pythainlp-4.0.2/pythainlp/spell/symspellpy.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/spell/tltk.py` & `pythainlp-4.0.2/pythainlp/spell/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/summarize/__init__.py` & `pythainlp-4.0.2/pythainlp/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/summarize/core.py` & `pythainlp-4.0.2/pythainlp/summarize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/summarize/freq.py` & `pythainlp-4.0.2/pythainlp/summarize/freq.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/summarize/keybert.py` & `pythainlp-4.0.2/pythainlp/summarize/keybert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/summarize/mt5.py` & `pythainlp-4.0.2/pythainlp/summarize/mt5.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/__init__.py` & `pythainlp-4.0.2/pythainlp/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/_tag_perceptron.py` & `pythainlp-4.0.2/pythainlp/tag/_tag_perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/blackboard.py` & `pythainlp-4.0.2/pythainlp/tag/blackboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/chunk.py` & `pythainlp-4.0.2/pythainlp/tag/chunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/crfchunk.py` & `pythainlp-4.0.2/pythainlp/tag/crfchunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/locations.py` & `pythainlp-4.0.2/pythainlp/tag/locations.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/named_entity.py` & `pythainlp-4.0.2/pythainlp/tag/named_entity.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/orchid.py` & `pythainlp-4.0.2/pythainlp/tag/orchid.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/perceptron.py` & `pythainlp-4.0.2/pythainlp/tag/perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/pos_tag.py` & `pythainlp-4.0.2/pythainlp/tag/pos_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/thai_nner.py` & `pythainlp-4.0.2/pythainlp/tag/thai_nner.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/thainer.py` & `pythainlp-4.0.2/pythainlp/tag/thainer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/tltk.py` & `pythainlp-4.0.2/pythainlp/tag/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/unigram.py` & `pythainlp-4.0.2/pythainlp/tag/unigram.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tag/wangchanberta_onnx.py` & `pythainlp-4.0.2/pythainlp/tag/wangchanberta_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/__init__.py` & `pythainlp-4.0.2/pythainlp/tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/_utils.py` & `pythainlp-4.0.2/pythainlp/tokenize/_utils.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/attacut.py` & `pythainlp-4.0.2/pythainlp/tokenize/attacut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/core.py` & `pythainlp-4.0.2/pythainlp/tokenize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/crfcls.py` & `pythainlp-4.0.2/pythainlp/tokenize/crfcls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/crfcut.py` & `pythainlp-4.0.2/pythainlp/tokenize/crfcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/deepcut.py` & `pythainlp-4.0.2/pythainlp/tokenize/deepcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/etcc.py` & `pythainlp-4.0.2/pythainlp/tokenize/etcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/longest.py` & `pythainlp-4.0.2/pythainlp/tokenize/longest.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/multi_cut.py` & `pythainlp-4.0.2/pythainlp/tokenize/multi_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/nercut.py` & `pythainlp-4.0.2/pythainlp/tokenize/nercut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/newmm.py` & `pythainlp-4.0.2/pythainlp/tokenize/newmm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/nlpo3.py` & `pythainlp-4.0.2/pythainlp/tokenize/nlpo3.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/oskut.py` & `pythainlp-4.0.2/pythainlp/tokenize/oskut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/pyicu.py` & `pythainlp-4.0.2/pythainlp/tokenize/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/sefr_cut.py` & `pythainlp-4.0.2/pythainlp/tokenize/sefr_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/ssg.py` & `pythainlp-4.0.2/pythainlp/tokenize/ssg.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/tcc.py` & `pythainlp-4.0.2/pythainlp/tokenize/tcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/tcc_p.py` & `pythainlp-4.0.2/pythainlp/tokenize/tcc_p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/thaisumcut.py` & `pythainlp-4.0.2/pythainlp/tokenize/thaisumcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tokenize/tltk.py` & `pythainlp-4.0.2/pythainlp/tokenize/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tools/__init__.py` & `pythainlp-4.0.2/pythainlp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tools/misspell.py` & `pythainlp-4.0.2/pythainlp/tools/misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/tools/path.py` & `pythainlp-4.0.2/pythainlp/tools/path.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/translate/__init__.py` & `pythainlp-4.0.2/pythainlp/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/translate/core.py` & `pythainlp-4.0.2/pythainlp/translate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/translate/en_th.py` & `pythainlp-4.0.2/pythainlp/translate/en_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/translate/th_fr.py` & `pythainlp-4.0.2/pythainlp/translate/th_fr.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/translate/zh_th.py` & `pythainlp-4.0.2/pythainlp/translate/zh_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/__init__.py` & `pythainlp-4.0.2/pythainlp/transliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/core.py` & `pythainlp-4.0.2/pythainlp/transliterate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/ipa.py` & `pythainlp-4.0.2/pythainlp/transliterate/ipa.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/iso_11940.py` & `pythainlp-4.0.2/pythainlp/transliterate/iso_11940.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/lookup.py` & `pythainlp-4.0.2/pythainlp/transliterate/lookup.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/pyicu.py` & `pythainlp-4.0.2/pythainlp/transliterate/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/royin.py` & `pythainlp-4.0.2/pythainlp/transliterate/royin.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/spoonerism.py` & `pythainlp-4.0.2/pythainlp/transliterate/spoonerism.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/thai2rom.py` & `pythainlp-4.0.2/pythainlp/transliterate/thai2rom.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/thai2rom_onnx.py` & `pythainlp-4.0.2/pythainlp/transliterate/thai2rom_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/thaig2p.py` & `pythainlp-4.0.2/pythainlp/transliterate/thaig2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/tltk.py` & `pythainlp-4.0.2/pythainlp/transliterate/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/w2p.py` & `pythainlp-4.0.2/pythainlp/transliterate/w2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/transliterate/wunsen.py` & `pythainlp-4.0.2/pythainlp/transliterate/wunsen.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/ulmfit/__init__.py` & `pythainlp-4.0.2/pythainlp/ulmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/ulmfit/core.py` & `pythainlp-4.0.2/pythainlp/ulmfit/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/ulmfit/preprocess.py` & `pythainlp-4.0.2/pythainlp/ulmfit/preprocess.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/ulmfit/tokenizer.py` & `pythainlp-4.0.2/pythainlp/ulmfit/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/__init__.py` & `pythainlp-4.0.2/pythainlp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/collate.py` & `pythainlp-4.0.2/pythainlp/util/collate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/date.py` & `pythainlp-4.0.2/pythainlp/util/date.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/digitconv.py` & `pythainlp-4.0.2/pythainlp/util/digitconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/emojiconv.py` & `pythainlp-4.0.2/pythainlp/util/emojiconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/keyboard.py` & `pythainlp-4.0.2/pythainlp/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/keywords.py` & `pythainlp-4.0.2/pythainlp/util/keywords.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/normalize.py` & `pythainlp-4.0.2/pythainlp/util/normalize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/numtoword.py` & `pythainlp-4.0.2/pythainlp/util/numtoword.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/phoneme.py` & `pythainlp-4.0.2/pythainlp/util/phoneme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/strftime.py` & `pythainlp-4.0.2/pythainlp/util/strftime.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/syllable.py` & `pythainlp-4.0.2/pythainlp/util/syllable.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/thai.py` & `pythainlp-4.0.2/pythainlp/util/thai.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/thaiwordcheck.py` & `pythainlp-4.0.2/pythainlp/util/thaiwordcheck.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/time.py` & `pythainlp-4.0.2/pythainlp/util/time.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/trie.py` & `pythainlp-4.0.2/pythainlp/util/trie.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/util/wordtonum.py` & `pythainlp-4.0.2/pythainlp/util/wordtonum.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/wangchanberta/__init__.py` & `pythainlp-4.0.2/pythainlp/wangchanberta/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/wangchanberta/core.py` & `pythainlp-4.0.2/pythainlp/wangchanberta/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/word_vector/__init__.py` & `pythainlp-4.0.2/pythainlp/word_vector/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp/word_vector/core.py` & `pythainlp-4.0.2/pythainlp/word_vector/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp.egg-info/PKG-INFO` & `pythainlp-4.0.2/pythainlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 4.0.1
+Version: 4.0.2
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
```

### Comparing `pythainlp-4.0.1/pythainlp.egg-info/SOURCES.txt` & `pythainlp-4.0.2/pythainlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/pythainlp.egg-info/requires.txt` & `pythainlp-4.0.2/pythainlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/setup.cfg` & `pythainlp-4.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/setup.py` & `pythainlp-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         "spacy_thai>=0.7.1",
         "ufal.chu-liu-edmonds>=1.0.2",
     ],
 }
 
 setup(
     name="pythainlp",
-    version="4.0.1",
+    version="4.0.2",
     description="Thai Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="PyThaiNLP",
     author_email="email@wannaphong.com",
     url="https://github.com/PyThaiNLP/pythainlp",
     packages=find_packages(exclude=["tests", "tests.*"]),
```

### Comparing `pythainlp-4.0.1/tests/data/eval-details-input.json` & `pythainlp-4.0.2/tests/data/eval-details-input.json`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/data/sentences.yml` & `pythainlp-4.0.2/tests/data/sentences.yml`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_augment.py` & `pythainlp-4.0.2/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_benchmarks.py` & `pythainlp-4.0.2/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_cli.py` & `pythainlp-4.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_corpus.py` & `pythainlp-4.0.2/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_generate.py` & `pythainlp-4.0.2/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_khavee.py` & `pythainlp-4.0.2/tests/test_khavee.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_misspell.py` & `pythainlp-4.0.2/tests/test_misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_parse.py` & `pythainlp-4.0.2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_soundex.py` & `pythainlp-4.0.2/tests/test_soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_spell.py` & `pythainlp-4.0.2/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_summarize.py` & `pythainlp-4.0.2/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_tag.py` & `pythainlp-4.0.2/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_tokenize.py` & `pythainlp-4.0.2/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_translate.py` & `pythainlp-4.0.2/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_transliterate.py` & `pythainlp-4.0.2/tests/test_transliterate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_ulmfit.py` & `pythainlp-4.0.2/tests/test_ulmfit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_util.py` & `pythainlp-4.0.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_wangchanberta.py` & `pythainlp-4.0.2/tests/test_wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.1/tests/test_word_vector.py` & `pythainlp-4.0.2/tests/test_word_vector.py`

 * *Files identical despite different names*

