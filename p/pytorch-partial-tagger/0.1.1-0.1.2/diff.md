# Comparing `tmp/pytorch_partial_tagger-0.1.1.tar.gz` & `tmp/pytorch_partial_tagger-0.1.2.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.1.tar` & `pytorch_partial_tagger-0.1.2.tar`

### file list

```diff
@@ -1,136 +1,34 @@
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/106b421343a29050
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/118021125c7251dc
--rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/11f76eaeb41d5d92
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/12415b5ac67f656
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/13608701a9b17613
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/1565abb795d586e1
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/15a8b9aa8a597371
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/182ecaf933e69e87
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/195c7349927832a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/1965053f1fd64cbf
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/1ecacb9f21faa08c
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/22956e582753705
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/2301591c3c47b639
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/2479c6691aaae7b2
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/25598cfd74d2dae7
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/27151a69f6eb5cd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/275dcf85fdc0cf0f
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/2816dbd5263a23f7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/297917b1400f12c7
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/2a828151c0a576f1
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/2ffcbecadc4b3fd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/363e4edd8d7ff82d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/36f7e4ea1bd41079
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/37e7201cc4281a7e
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/3b3b68fdba5d20e
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/3f6f323f1bb9a231
--rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/418bc6111a8ba78a
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/41e9326ebcc4b19e
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/4562057324d7e8a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/473c7b1d09edc0ae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/47c3266a778a5328
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/4970dca60df71997
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/5141e092391f04be
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/5314ac1a92aef232
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/5593b40ad4fb901b
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/613125a049354673
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/63d799f6d3bdb4aa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/654203df5ec01665
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/65b759234c4668ac
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/698d56ef37a97507
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/6f1c3ff7296035cb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/6fa1c39c4386ab0b
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/71788ae232af531a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/7573d78cce9fcc7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/7d77d5d2634dd032
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/80302dd4b75c86b2
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/81edaa82aec05cbc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/8743093306772dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/8901cd0c8af47260
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/8a1f748568d7f255
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/8a8891fa991985a3
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/8fdce7975936440
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/9843af09c7484da6
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/9d6aac9bc72fa845
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/9ebab3f4f67932ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/a48bd7dc4106feab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/a4ee7cfb47cbeceb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/a56ab753c9563d0a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/a8e39f9109ee1728
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ae59d334de76fc77
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/b299c7e633ae300
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/b8d4ca1df9d44318
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ba7275089739c5ed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/bd696adfc35bdcf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/bfc544a5229027cd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/c2cbb0df08edf925
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/c9fa762f55dfc076
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ca2fe1c176724df8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/cc47e5c19d7a3abe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d0c429bd49080258
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d434160a0e5423f8
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d53a799bd6446482
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d5a888f3adf7898b
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d629a5f0dc7f648
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d6c609fcc0dca98
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d785fe251e2e9b89
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/d8ec8be125bff75a
--rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ddb4c8f62d6bd2f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/e24b00289d490604
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/e3a28b9da6b8967b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/eaa979b8f392d046
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ec5f4ecdbad7ef09
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ecb4fe952be17977
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/ed61d6e42637b3d1
--rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/efd0f7dbc5533f0a
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/f03584a624311b85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/f1918cef7970a1dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/f45eebd3003e680d
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/f7ae8535fcbd39db
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/f80fcd7e3c7b6583
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/f8f9174fac562cfb
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/faeb112b154d577f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.ruff_cache/content/fdac70936ff5904
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/embedders.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/training.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/crf/.DS_Store
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/data/.DS_Store
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/data/batch.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/decoders/.DS_Store
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/encoders/.DS_Store
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/src/partial_tagger/encoders/linear.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/helpers.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/crf/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/crf/__init__.py
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/crf/test_functional.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/crf/test_nn.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/data/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/data/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/data/test_batch.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/tests/data/test_core.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/LICENSE
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/README.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/embedders.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/data/batch.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/data/__init__.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/data/test_batch.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/tests/data/test_core.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/README.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.2/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.1/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.2/.github/workflows/pypi-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install hatch build
     - name: Build a binary wheel and a source tarball
       run: |
         hatch version "${GITHUB_REF_NAME}"
-        build
+        python -m build
     - name: Publish a Python distribution to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/11f76eaeb41d5d92` & `pytorch_partial_tagger-0.1.2/tests/crf/test_functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,702 +1,647 @@
-00000000: 0100 0000 0000 0000 1900 0000 0000 0000  ................
-00000010: 7465 7374 732e 6372 662e 7465 7374 5f66  tests.crf.test_f
-00000020: 756e 6374 696f 6e61 6c06 0000 0000 0000  unctional.......
-00000030: 0013 0000 0000 0000 0075 6e69 7474 6573  .........unittes
-00000040: 742e 6d6f 636b 2e70 6174 6368 1a00 0000  t.mock.patch....
-00000050: 1f00 0000 0600 0000 0000 0000 7079 7465  ............pyte
-00000060: 7374 2100 0000 2e00 0000 0500 0000 0000  st!.............
-00000070: 0000 746f 7263 682f 0000 003b 0000 0017  ..torch/...;....
-00000080: 0000 0000 0000 0070 6172 7469 616c 5f74  .......partial_t
-00000090: 6167 6765 722e 6372 662e 4e49 4e46 5c00  agger.crf.NINF\.
-000000a0: 0000 6000 0000 1d00 0000 0000 0000 7061  ..`...........pa
-000000b0: 7274 6961 6c5f 7461 6767 6572 2e63 7266  rtial_tagger.crf
-000000c0: 2e66 756e 6374 696f 6e61 6c80 0000 008f  .functional.....
-000000d0: 0000 000d 0000 0000 0000 0074 6573 7473  ...........tests
-000000e0: 2e68 656c 7065 7273 a200 0000 a900 0000  .helpers........
-000000f0: 0200 0000 0000 0000 1800 0000 0000 0000  ................
-00000100: 556e 6e65 6365 7373 6172 7943 6f6d 7072  UnnecessaryCompr
-00000110: 6568 656e 7369 6f6e 3900 0000 0000 0000  ehension9.......
-00000120: 556e 6e65 6365 7373 6172 7920 606c 6973  Unnecessary `lis
-00000130: 7460 2063 6f6d 7072 6568 656e 7369 6f6e  t` comprehension
-00000140: 2028 7265 7772 6974 6520 7573 696e 6720   (rewrite using 
-00000150: 606c 6973 7428 2960 2901 1600 0000 0000  `list()`).......
-00000160: 0000 5265 7772 6974 6520 7573 696e 6720  ..Rewrite using 
-00000170: 606c 6973 7428 2960 810b 0000 960b 0000  `list()`........
-00000180: 0101 0000 0000 0000 0081 0b00 0096 0b00  ................
-00000190: 0001 0e00 0000 0000 0000 6c69 7374 2872  ..........list(r
-000001a0: 616e 6765 2835 2929 0300 0000 0000 0000  ange(5))........
-000001b0: 0000 0000 810b 0000 0f00 0000 0000 0000  ................
-000001c0: 556e 736f 7274 6564 496d 706f 7274 7329  UnsortedImports)
-000001d0: 0000 0000 0000 0049 6d70 6f72 7420 626c  .......Import bl
-000001e0: 6f63 6b20 6973 2075 6e2d 736f 7274 6564  ock is un-sorted
-000001f0: 206f 7220 756e 2d66 6f72 6d61 7474 6564   or un-formatted
-00000200: 0110 0000 0000 0000 004f 7267 616e 697a  .........Organiz
-00000210: 6520 696d 706f 7274 7300 0000 00ac 0000  e imports.......
-00000220: 0001 0100 0000 0000 0000 0000 0000 ac00  ................
-00000230: 0000 01ac 0000 0000 0000 0066 726f 6d20  ...........from 
-00000240: 756e 6974 7465 7374 2e6d 6f63 6b20 696d  unittest.mock im
-00000250: 706f 7274 2070 6174 6368 0a0a 696d 706f  port patch..impo
-00000260: 7274 2070 7974 6573 740a 696d 706f 7274  rt pytest.import
-00000270: 2074 6f72 6368 0a66 726f 6d20 7061 7274   torch.from part
-00000280: 6961 6c5f 7461 6767 6572 2e63 7266 2069  ial_tagger.crf i
-00000290: 6d70 6f72 7420 4e49 4e46 0a66 726f 6d20  mport NINF.from 
-000002a0: 7061 7274 6961 6c5f 7461 6767 6572 2e63  partial_tagger.c
-000002b0: 7266 2069 6d70 6f72 7420 6675 6e63 7469  rf import functi
-000002c0: 6f6e 616c 2061 7320 460a 0a66 726f 6d20  onal as F..from 
-000002d0: 7465 7374 7320 696d 706f 7274 2068 656c  tests import hel
-000002e0: 7065 7273 0a0a 0a03 0000 0000 0000 0000  pers............
-000002f0: 0000 0000 0000 0001 0000 0000 0000 004d  ...............M
-00000300: 0000 0000 0000 002f 5573 6572 732f 7961  ......./Users/ya
-00000310: 7375 6675 6d69 2f57 6f72 6b73 7061 6365  sufumi/Workspace
-00000320: 2f70 7974 6f72 6368 2d70 6172 7469 616c  /pytorch-partial
-00000330: 2d74 6167 6765 722f 7465 7374 732f 6372  -tagger/tests/cr
-00000340: 662f 7465 7374 5f66 756e 6374 696f 6e61  f/test_functiona
-00000350: 6c2e 7079 7728 0000 0000 0000 6672 6f6d  l.pyw(......from
-00000360: 2075 6e69 7474 6573 742e 6d6f 636b 2069   unittest.mock i
-00000370: 6d70 6f72 7420 7061 7463 680a 0a69 6d70  mport patch..imp
-00000380: 6f72 7420 7079 7465 7374 0a69 6d70 6f72  ort pytest.impor
-00000390: 7420 746f 7263 680a 0a66 726f 6d20 7061  t torch..from pa
-000003a0: 7274 6961 6c5f 7461 6767 6572 2e63 7266  rtial_tagger.crf
-000003b0: 2069 6d70 6f72 7420 4e49 4e46 0a66 726f   import NINF.fro
-000003c0: 6d20 7061 7274 6961 6c5f 7461 6767 6572  m partial_tagger
-000003d0: 2e63 7266 2069 6d70 6f72 7420 6675 6e63  .crf import func
-000003e0: 7469 6f6e 616c 2061 7320 460a 6672 6f6d  tional as F.from
-000003f0: 2074 6573 7473 2069 6d70 6f72 7420 6865   tests import he
-00000400: 6c70 6572 730a 0a0a 6465 6620 7465 7374  lpers...def test
-00000410: 5f6c 6f67 5f6c 696b 656c 6968 6f6f 645f  _log_likelihood_
-00000420: 7661 6c69 645f 6173 5f70 726f 6261 6269  valid_as_probabi
-00000430: 6c69 7479 2874 6573 745f 6461 7461 5f73  lity(test_data_s
-00000440: 6d61 6c6c 3a20 7475 706c 6529 202d 3e20  mall: tuple) -> 
-00000450: 4e6f 6e65 3a0a 2020 2020 2862 6174 6368  None:.    (batch
-00000460: 5f73 697a 652c 2073 6571 7565 6e63 655f  _size, sequence_
-00000470: 6c65 6e67 7468 2c20 6e75 6d5f 7461 6773  length, num_tags
-00000480: 292c 206c 6f67 5f70 6f74 656e 7469 616c  ), log_potential
-00000490: 7320 3d20 7465 7374 5f64 6174 615f 736d  s = test_data_sm
-000004a0: 616c 6c0a 0a20 2020 2074 6f74 616c 5f6c  all..    total_l
-000004b0: 6f67 5f70 203d 2074 6f72 6368 2e74 656e  og_p = torch.ten
-000004c0: 736f 7228 5b4e 494e 465d 202a 2062 6174  sor([NINF] * bat
-000004d0: 6368 5f73 697a 6529 0a20 2020 2066 6f72  ch_size).    for
-000004e0: 2074 6167 5f69 6e64 6963 6573 2069 6e20   tag_indices in 
-000004f0: 6865 6c70 6572 732e 6974 6572 6174 655f  helpers.iterate_
-00000500: 706f 7373 6962 6c65 5f74 6167 5f69 6e64  possible_tag_ind
-00000510: 6963 6573 2873 6571 7565 6e63 655f 6c65  ices(sequence_le
-00000520: 6e67 7468 2c20 6e75 6d5f 7461 6773 293a  ngth, num_tags):
-00000530: 0a20 2020 2020 2020 2074 6f74 616c 5f6c  .        total_l
-00000540: 6f67 5f70 203d 2074 6f72 6368 2e6c 6f67  og_p = torch.log
-00000550: 6164 6465 7870 280a 2020 2020 2020 2020  addexp(.        
-00000560: 2020 2020 746f 7461 6c5f 6c6f 675f 702c      total_log_p,
-00000570: 2046 2e6c 6f67 5f6c 696b 656c 6968 6f6f   F.log_likelihoo
-00000580: 6428 6c6f 675f 706f 7465 6e74 6961 6c73  d(log_potentials
-00000590: 2c20 746f 7263 682e 7465 6e73 6f72 2874  , torch.tensor(t
-000005a0: 6167 5f69 6e64 6963 6573 2929 0a20 2020  ag_indices)).   
-000005b0: 2020 2020 2029 0a0a 2020 2020 6173 7365       )..    asse
-000005c0: 7274 2074 6f72 6368 2e61 6c6c 636c 6f73  rt torch.allclos
-000005d0: 6528 746f 7461 6c5f 6c6f 675f 702e 6578  e(total_log_p.ex
-000005e0: 7028 292c 2074 6f72 6368 2e6f 6e65 735f  p(), torch.ones_
-000005f0: 6c69 6b65 2874 6f74 616c 5f6c 6f67 5f70  like(total_log_p
-00000600: 2929 0a0a 0a64 6566 2074 6573 745f 6d61  ))...def test_ma
-00000610: 7267 696e 616c 5f6c 6f67 5f6c 696b 656c  rginal_log_likel
-00000620: 6968 6f6f 645f 7661 6c69 645f 6173 5f70  ihood_valid_as_p
-00000630: 726f 6261 6269 6c69 7479 2874 6573 745f  robability(test_
-00000640: 6461 7461 5f73 6d61 6c6c 3a20 7475 706c  data_small: tupl
-00000650: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
-00000660: 7368 6170 652c 206c 6f67 5f70 6f74 656e  shape, log_poten
-00000670: 7469 616c 7320 3d20 7465 7374 5f64 6174  tials = test_dat
-00000680: 615f 736d 616c 6c0a 0a20 2020 2074 6167  a_small..    tag
-00000690: 5f62 6974 6d61 7020 3d20 746f 7263 682e  _bitmap = torch.
-000006a0: 6f6e 6573 2873 6861 7065 2c20 6474 7970  ones(shape, dtyp
-000006b0: 653d 746f 7263 682e 626f 6f6c 290a 2020  e=torch.bool).  
-000006c0: 2020 6c6f 675f 7020 3d20 462e 6d61 7267    log_p = F.marg
-000006d0: 696e 616c 5f6c 6f67 5f6c 696b 656c 6968  inal_log_likelih
-000006e0: 6f6f 6428 6c6f 675f 706f 7465 6e74 6961  ood(log_potentia
-000006f0: 6c73 2c20 7461 675f 6269 746d 6170 290a  ls, tag_bitmap).
-00000700: 0a20 2020 2061 7373 6572 7420 746f 7263  .    assert torc
-00000710: 682e 616c 6c63 6c6f 7365 286c 6f67 5f70  h.allclose(log_p
-00000720: 2e65 7870 2829 2c20 746f 7263 682e 6f6e  .exp(), torch.on
-00000730: 6573 5f6c 696b 6528 6c6f 675f 7029 290a  es_like(log_p)).
-00000740: 0a0a 6465 6620 7465 7374 5f6d 6172 6769  ..def test_margi
-00000750: 6e61 6c5f 6c6f 675f 6c69 6b65 6c69 686f  nal_log_likeliho
-00000760: 6f64 5f6d 6174 6368 6573 5f6c 6f67 5f6c  od_matches_log_l
-00000770: 696b 656c 6968 6f6f 645f 6966 5f6f 6e65  ikelihood_if_one
-00000780: 5f68 6f74 5f74 6167 5f62 6974 6d61 705f  _hot_tag_bitmap_
-00000790: 6973 5f67 6976 656e 280a 2020 2020 7465  is_given(.    te
-000007a0: 7374 5f64 6174 615f 736d 616c 6c3a 2074  st_data_small: t
-000007b0: 7570 6c65 2c0a 2920 2d3e 204e 6f6e 653a  uple,.) -> None:
-000007c0: 0a20 2020 2073 6861 7065 2c20 6c6f 675f  .    shape, log_
-000007d0: 706f 7465 6e74 6961 6c73 203d 2074 6573  potentials = tes
-000007e0: 745f 6461 7461 5f73 6d61 6c6c 0a0a 2020  t_data_small..  
-000007f0: 2020 666f 7220 7461 675f 6269 746d 6170    for tag_bitmap
-00000800: 2069 6e20 6865 6c70 6572 732e 6974 6572   in helpers.iter
-00000810: 6174 655f 706f 7373 6962 6c65 5f6f 6e65  ate_possible_one
-00000820: 5f68 6f74 5f74 6167 5f62 6974 6d61 7028  _hot_tag_bitmap(
-00000830: 2a73 6861 7065 293a 0a20 2020 2020 2020  *shape):.       
-00000840: 2061 203d 2046 2e6c 6f67 5f6c 696b 656c   a = F.log_likel
-00000850: 6968 6f6f 6428 6c6f 675f 706f 7465 6e74  ihood(log_potent
-00000860: 6961 6c73 2c20 7461 675f 6269 746d 6170  ials, tag_bitmap
-00000870: 2e6c 6f6e 6728 292e 6172 676d 6178 2864  .long().argmax(d
-00000880: 696d 3d2d 3129 290a 2020 2020 2020 2020  im=-1)).        
-00000890: 6220 3d20 462e 6d61 7267 696e 616c 5f6c  b = F.marginal_l
-000008a0: 6f67 5f6c 696b 656c 6968 6f6f 6428 6c6f  og_likelihood(lo
-000008b0: 675f 706f 7465 6e74 6961 6c73 2c20 7461  g_potentials, ta
-000008c0: 675f 6269 746d 6170 290a 0a20 2020 2020  g_bitmap)..     
-000008d0: 2020 2061 7373 6572 7420 746f 7263 682e     assert torch.
-000008e0: 616c 6c63 6c6f 7365 2861 2c20 6229 0a0a  allclose(a, b)..
-000008f0: 0a64 6566 2074 6573 745f 666f 7277 6172  .def test_forwar
-00000900: 645f 616c 676f 7269 7468 6d5f 7265 7475  d_algorithm_retu
-00000910: 726e 735f 7661 6c75 655f 7361 6d65 5f61  rns_value_same_a
-00000920: 735f 6272 7574 655f 666f 7263 6528 0a20  s_brute_force(. 
-00000930: 2020 2074 6573 745f 6461 7461 5f73 6d61     test_data_sma
-00000940: 6c6c 3a20 7475 706c 652c 0a29 202d 3e20  ll: tuple,.) -> 
-00000950: 4e6f 6e65 3a0a 2020 2020 5f2c 206c 6f67  None:.    _, log
-00000960: 5f70 6f74 656e 7469 616c 7320 3d20 7465  _potentials = te
-00000970: 7374 5f64 6174 615f 736d 616c 6c0a 0a20  st_data_small.. 
-00000980: 2020 206c 6f67 5f5a 203d 2046 2e66 6f72     log_Z = F.for
-00000990: 7761 7264 5f61 6c67 6f72 6974 686d 286c  ward_algorithm(l
-000009a0: 6f67 5f70 6f74 656e 7469 616c 7329 0a20  og_potentials). 
-000009b0: 2020 2065 7870 6563 7465 645f 6c6f 675f     expected_log_
-000009c0: 5a20 3d20 6865 6c70 6572 732e 636f 6d70  Z = helpers.comp
-000009d0: 7574 655f 6c6f 675f 6e6f 726d 616c 697a  ute_log_normaliz
-000009e0: 6572 5f62 795f 6272 7574 655f 666f 7263  er_by_brute_forc
-000009f0: 6528 6c6f 675f 706f 7465 6e74 6961 6c73  e(log_potentials
-00000a00: 290a 0a20 2020 2061 7373 6572 7420 746f  )..    assert to
-00000a10: 7263 682e 616c 6c63 6c6f 7365 286c 6f67  rch.allclose(log
-00000a20: 5f5a 2c20 6578 7065 6374 6564 5f6c 6f67  _Z, expected_log
-00000a30: 5f5a 290a 0a0a 6465 6620 7465 7374 5f61  _Z)...def test_a
-00000a40: 6d61 785f 7265 7475 726e 735f 7661 6c75  max_returns_valu
-00000a50: 655f 7361 6d65 5f61 735f 6272 7574 655f  e_same_as_brute_
-00000a60: 666f 7263 6528 7465 7374 5f64 6174 615f  force(test_data_
-00000a70: 736d 616c 6c3a 2074 7570 6c65 2920 2d3e  small: tuple) ->
-00000a80: 204e 6f6e 653a 0a20 2020 205f 2c20 6c6f   None:.    _, lo
-00000a90: 675f 706f 7465 6e74 6961 6c73 203d 2074  g_potentials = t
-00000aa0: 6573 745f 6461 7461 5f73 6d61 6c6c 0a0a  est_data_small..
-00000ab0: 2020 2020 6d61 785f 7363 6f72 6520 3d20      max_score = 
-00000ac0: 462e 616d 6178 286c 6f67 5f70 6f74 656e  F.amax(log_poten
-00000ad0: 7469 616c 7329 0a20 2020 2065 7870 6563  tials).    expec
-00000ae0: 7465 645f 6d61 785f 7363 6f72 652c 205f  ted_max_score, _
-00000af0: 203d 2068 656c 7065 7273 2e63 6f6d 7075   = helpers.compu
-00000b00: 7465 5f62 6573 745f 7461 675f 696e 6469  te_best_tag_indi
-00000b10: 6365 735f 6279 5f62 7275 7465 5f66 6f72  ces_by_brute_for
-00000b20: 6365 280a 2020 2020 2020 2020 6c6f 675f  ce(.        log_
-00000b30: 706f 7465 6e74 6961 6c73 0a20 2020 2029  potentials.    )
-00000b40: 0a0a 2020 2020 6173 7365 7274 2074 6f72  ..    assert tor
-00000b50: 6368 2e61 6c6c 636c 6f73 6528 6d61 785f  ch.allclose(max_
-00000b60: 7363 6f72 652c 2065 7870 6563 7465 645f  score, expected_
-00000b70: 6d61 785f 7363 6f72 6529 0a0a 0a64 6566  max_score)...def
-00000b80: 2074 6573 745f 6465 636f 6465 5f72 6574   test_decode_ret
-00000b90: 7572 6e73 5f76 616c 7565 5f73 616d 655f  urns_value_same_
-00000ba0: 6173 5f62 7275 7465 5f66 6f72 6365 2874  as_brute_force(t
-00000bb0: 6573 745f 6461 7461 5f73 6d61 6c6c 3a20  est_data_small: 
-00000bc0: 7475 706c 6529 202d 3e20 4e6f 6e65 3a0a  tuple) -> None:.
-00000bd0: 2020 2020 5f2c 206c 6f67 5f70 6f74 656e      _, log_poten
-00000be0: 7469 616c 7320 3d20 7465 7374 5f64 6174  tials = test_dat
-00000bf0: 615f 736d 616c 6c0a 0a20 2020 206d 6178  a_small..    max
-00000c00: 5f73 636f 7265 2c20 7461 675f 696e 6469  _score, tag_indi
-00000c10: 6365 7320 3d20 462e 6465 636f 6465 286c  ces = F.decode(l
-00000c20: 6f67 5f70 6f74 656e 7469 616c 7329 0a0a  og_potentials)..
-00000c30: 2020 2020 280a 2020 2020 2020 2020 6578      (.        ex
-00000c40: 7065 6374 6564 5f6d 6178 5f73 636f 7265  pected_max_score
-00000c50: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
-00000c60: 6564 5f74 6167 5f69 6e64 6963 6573 2c0a  ed_tag_indices,.
-00000c70: 2020 2020 2920 3d20 6865 6c70 6572 732e      ) = helpers.
-00000c80: 636f 6d70 7574 655f 6265 7374 5f74 6167  compute_best_tag
-00000c90: 5f69 6e64 6963 6573 5f62 795f 6272 7574  _indices_by_brut
-00000ca0: 655f 666f 7263 6528 6c6f 675f 706f 7465  e_force(log_pote
-00000cb0: 6e74 6961 6c73 290a 0a20 2020 2061 7373  ntials)..    ass
-00000cc0: 6572 7420 746f 7263 682e 616c 6c63 6c6f  ert torch.allclo
-00000cd0: 7365 286d 6178 5f73 636f 7265 2c20 6578  se(max_score, ex
-00000ce0: 7065 6374 6564 5f6d 6178 5f73 636f 7265  pected_max_score
-00000cf0: 290a 2020 2020 6173 7365 7274 2074 6f72  ).    assert tor
-00000d00: 6368 2e61 6c6c 636c 6f73 6528 7461 675f  ch.allclose(tag_
-00000d10: 696e 6469 6365 732c 2065 7870 6563 7465  indices, expecte
-00000d20: 645f 7461 675f 696e 6469 6365 7329 0a0a  d_tag_indices)..
-00000d30: 0a64 6566 2074 6573 745f 7365 7175 656e  .def test_sequen
-00000d40: 6365 5f73 636f 7265 5f63 6f6d 7075 7465  ce_score_compute
-00000d50: 735f 6d61 736b 5f63 6f72 7265 6374 6c79  s_mask_correctly
-00000d60: 280a 2020 2020 7465 7374 5f64 6174 615f  (.    test_data_
-00000d70: 7769 7468 5f6d 6173 6b3a 2074 7570 6c65  with_mask: tuple
-00000d80: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-00000d90: 205f 2c20 6c6f 675f 706f 7465 6e74 6961   _, log_potentia
-00000da0: 6c73 2c20 7461 675f 696e 6469 6365 732c  ls, tag_indices,
-00000db0: 206d 6173 6b20 3d20 7465 7374 5f64 6174   mask = test_dat
-00000dc0: 615f 7769 7468 5f6d 6173 6b0a 0a20 2020  a_with_mask..   
-00000dd0: 2077 6974 6820 7061 7463 6828 2274 6f72   with patch("tor
-00000de0: 6368 2e54 656e 736f 722e 6d75 6c22 2920  ch.Tensor.mul") 
-00000df0: 6173 206d 3a0a 2020 2020 2020 2020 462e  as m:.        F.
-00000e00: 7365 7175 656e 6365 5f73 636f 7265 286c  sequence_score(l
-00000e10: 6f67 5f70 6f74 656e 7469 616c 732c 2074  og_potentials, t
-00000e20: 6167 5f69 6e64 6963 6573 2c20 6d61 736b  ag_indices, mask
-00000e30: 290a 2020 2020 2020 2020 7573 6564 5f6d  ).        used_m
-00000e40: 6173 6b20 3d20 6d2e 6361 6c6c 5f61 7267  ask = m.call_arg
-00000e50: 735b 305d 5b30 5d0a 0a20 2020 2020 2020  s[0][0]..       
-00000e60: 2061 7373 6572 7420 6865 6c70 6572 732e   assert helpers.
-00000e70: 6368 6563 6b5f 7365 7175 656e 6365 5f73  check_sequence_s
-00000e80: 636f 7265 5f6d 6173 6b28 7573 6564 5f6d  core_mask(used_m
-00000e90: 6173 6b2c 2074 6167 5f69 6e64 6963 6573  ask, tag_indices
-00000ea0: 2c20 6d61 736b 290a 0a0a 4070 7974 6573  , mask)...@pytes
-00000eb0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00000ec0: 7a65 280a 2020 2020 2270 6172 7469 616c  ze(.    "partial
-00000ed0: 5f69 6e64 6578 222c 0a20 2020 205b 6920  _index",.    [i 
-00000ee0: 666f 7220 6920 696e 2072 616e 6765 2835  for i in range(5
-00000ef0: 295d 2c0a 290a 6465 6620 7465 7374 5f6d  )],.).def test_m
-00000f00: 756c 7469 7461 675f 7365 7175 656e 6365  ultitag_sequence
-00000f10: 5f73 636f 7265 5f63 6f72 7265 6374 6c79  _score_correctly
-00000f20: 5f6d 6173 6b73 5f6c 6f67 5f70 6f74 656e  _masks_log_poten
-00000f30: 7469 616c 7328 0a20 2020 2074 6573 745f  tials(.    test_
-00000f40: 6461 7461 5f77 6974 685f 6d61 736b 3a20  data_with_mask: 
-00000f50: 7475 706c 652c 2070 6172 7469 616c 5f69  tuple, partial_i
-00000f60: 6e64 6578 3a20 696e 740a 2920 2d3e 204e  ndex: int.) -> N
-00000f70: 6f6e 653a 0a20 2020 2028 5f2c 205f 2c20  one:.    (_, _, 
-00000f80: 6e75 6d5f 7461 6773 292c 206c 6f67 5f70  num_tags), log_p
-00000f90: 6f74 656e 7469 616c 732c 2074 6167 5f69  otentials, tag_i
-00000fa0: 6e64 6963 6573 2c20 6d61 736b 203d 2074  ndices, mask = t
-00000fb0: 6573 745f 6461 7461 5f77 6974 685f 6d61  est_data_with_ma
-00000fc0: 736b 0a20 2020 2074 6167 5f62 6974 6d61  sk.    tag_bitma
-00000fd0: 7020 3d20 462e 746f 5f74 6167 5f62 6974  p = F.to_tag_bit
-00000fe0: 6d61 7028 7461 675f 696e 6469 6365 732c  map(tag_indices,
-00000ff0: 206e 756d 5f74 6167 732c 2070 6172 7469   num_tags, parti
-00001000: 616c 5f69 6e64 6578 3d70 6172 7469 616c  al_index=partial
-00001010: 5f69 6e64 6578 290a 0a20 2020 2077 6974  _index)..    wit
-00001020: 6820 7061 7463 6828 2270 6172 7469 616c  h patch("partial
-00001030: 5f74 6167 6765 722e 6372 662e 6675 6e63  _tagger.crf.func
-00001040: 7469 6f6e 616c 2e66 6f72 7761 7264 5f61  tional.forward_a
-00001050: 6c67 6f72 6974 686d 2229 2061 7320 6d3a  lgorithm") as m:
-00001060: 0a20 2020 2020 2020 2046 2e6d 756c 7469  .        F.multi
-00001070: 7461 675f 7365 7175 656e 6365 5f73 636f  tag_sequence_sco
-00001080: 7265 286c 6f67 5f70 6f74 656e 7469 616c  re(log_potential
-00001090: 732c 2074 6167 5f62 6974 6d61 702c 206d  s, tag_bitmap, m
-000010a0: 6173 6b29 0a20 2020 2020 2020 2063 6f6e  ask).        con
-000010b0: 7374 7261 696e 6564 5f6c 6f67 5f70 6f74  strained_log_pot
-000010c0: 656e 7469 616c 7320 3d20 6d2e 6361 6c6c  entials = m.call
-000010d0: 5f61 7267 735b 305d 5b30 5d0a 0a20 2020  _args[0][0]..   
-000010e0: 2020 2020 2061 7373 6572 7420 6865 6c70       assert help
-000010f0: 6572 732e 6368 6563 6b5f 636f 6e73 7472  ers.check_constr
-00001100: 6169 6e65 645f 6c6f 675f 706f 7465 6e74  ained_log_potent
-00001110: 6961 6c73 280a 2020 2020 2020 2020 2020  ials(.          
-00001120: 2020 6c6f 675f 706f 7465 6e74 6961 6c73    log_potentials
-00001130: 2c20 636f 6e73 7472 6169 6e65 645f 6c6f  , constrained_lo
-00001140: 675f 706f 7465 6e74 6961 6c73 2c20 7461  g_potentials, ta
-00001150: 675f 696e 6469 6365 732c 206d 6173 6b2c  g_indices, mask,
-00001160: 2070 6172 7469 616c 5f69 6e64 6578 0a20   partial_index. 
-00001170: 2020 2020 2020 2029 0a0a 0a40 7079 7465         )...@pyte
-00001180: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-00001190: 697a 6528 0a20 2020 2022 6c6f 675f 706f  ize(.    "log_po
-000011a0: 7465 6e74 6961 6c73 2c20 6d61 736b 2c20  tentials, mask, 
-000011b0: 7374 6172 745f 636f 6e73 7472 6169 6e74  start_constraint
-000011c0: 732c 2065 6e64 5f63 6f6e 7374 7261 696e  s, end_constrain
-000011d0: 7473 2c20 7472 616e 7369 7469 6f6e 5f63  ts, transition_c
-000011e0: 6f6e 7374 7261 696e 7473 222c 0a20 2020  onstraints",.   
-000011f0: 205b 0a20 2020 2020 2020 2028 0a20 2020   [.        (.   
-00001200: 2020 2020 2020 2020 2074 6f72 6368 2e72           torch.r
-00001210: 616e 646e 2833 2c20 3230 2c20 352c 2035  andn(3, 20, 5, 5
-00001220: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
-00001230: 6f72 6368 2e74 656e 736f 7228 0a20 2020  orch.tensor(.   
-00001240: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 205b 5472 7565 5d20 2a20 3230 2c0a     [True] * 20,.
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 5b54 7275 655d 202a 2031 3520      [True] * 15 
-00001290: 2b20 5b46 616c 7365 5d20 2a20 352c 0a20  + [False] * 5,. 
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 205b 5472 7565 5d20 2a20 3820 2b20     [True] * 8 + 
-000012c0: 5b46 616c 7365 5d20 2a20 3132 2c0a 2020  [False] * 12,.  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-000012e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000012f0: 2064 7479 7065 3d74 6f72 6368 2e62 6f6f   dtype=torch.boo
-00001300: 6c2c 0a20 2020 2020 2020 2020 2020 2029  l,.            )
-00001310: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
-00001320: 7263 682e 7465 6e73 6f72 285b 5472 7565  rch.tensor([True
-00001330: 2c20 4661 6c73 652c 2046 616c 7365 2c20  , False, False, 
-00001340: 5472 7565 2c20 5472 7565 5d29 2c20 2023  True, True]),  #
-00001350: 2030 2c20 332c 2034 2061 7265 2061 6c6c   0, 3, 4 are all
-00001360: 6f77 6564 0a20 2020 2020 2020 2020 2020  owed.           
-00001370: 2074 6f72 6368 2e74 656e 736f 7228 5b46   torch.tensor([F
-00001380: 616c 7365 2c20 5472 7565 2c20 5472 7565  alse, True, True
-00001390: 2c20 4661 6c73 652c 2046 616c 7365 5d29  , False, False])
-000013a0: 2c20 2023 2032 2c20 3320 6172 6520 616c  ,  # 2, 3 are al
-000013b0: 6c6f 7765 640a 2020 2020 2020 2020 2020  lowed.          
-000013c0: 2020 746f 7263 682e 7465 6e73 6f72 280a    torch.tensor(.
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-000013f0: 2020 2020 2020 5b54 7275 652c 2046 616c        [True, Fal
-00001400: 7365 2c20 5472 7565 2c20 5472 7565 2c20  se, True, True, 
-00001410: 5472 7565 5d2c 2020 2320 302d 3e31 2069  True],  # 0->1 i
-00001420: 7320 6e6f 7420 616c 6c6f 7765 640a 2020  s not allowed.  
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 5b54 7275 652c 2054 7275 652c 2054    [True, True, T
-00001450: 7275 652c 2054 7275 652c 2054 7275 655d  rue, True, True]
-00001460: 2c20 2023 206e 6f20 636f 6e73 7472 6169  ,  # no constrai
-00001470: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00001480: 2020 2020 2020 2020 5b54 7275 652c 2054          [True, T
-00001490: 7275 652c 2046 616c 7365 2c20 5472 7565  rue, False, True
-000014a0: 2c20 5472 7565 5d2c 2020 2320 322d 3e32  , True],  # 2->2
-000014b0: 2069 7320 6e6f 7420 616c 6c6f 7765 640a   is not allowed.
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2020 2020 5b54 7275 652c 2046 616c 7365      [True, False
-000014e0: 2c20 5472 7565 2c20 5472 7565 2c20 5472  , True, True, Tr
-000014f0: 7565 5d2c 2020 2320 332d 3e31 2069 7320  ue],  # 3->1 is 
-00001500: 6e6f 7420 616c 6c6f 7765 640a 2020 2020  not allowed.    
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 5b54 7275 652c 2046 616c 7365 2c20 4661  [True, False, Fa
-00001530: 6c73 652c 2046 616c 7365 2c20 4661 6c73  lse, False, Fals
-00001540: 655d 2c20 2023 206f 6e6c 7920 342d 3e30  e],  # only 4->0
-00001550: 2069 7320 616c 6c6f 7765 640a 2020 2020   is allowed.    
-00001560: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00001570: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00001580: 2020 2020 2029 0a20 2020 205d 2c0a 290a       ).    ],.).
-00001590: 6465 6620 7465 7374 5f63 6f6e 7374 7261  def test_constra
-000015a0: 696e 735f 6c6f 675f 706f 7465 6e74 6961  ins_log_potentia
-000015b0: 6c73 280a 2020 2020 6c6f 675f 706f 7465  ls(.    log_pote
-000015c0: 6e74 6961 6c73 3a20 746f 7263 682e 5465  ntials: torch.Te
-000015d0: 6e73 6f72 2c0a 2020 2020 6d61 736b 3a20  nsor,.    mask: 
-000015e0: 746f 7263 682e 5465 6e73 6f72 2c0a 2020  torch.Tensor,.  
-000015f0: 2020 7374 6172 745f 636f 6e73 7472 6169    start_constrai
-00001600: 6e74 733a 2074 6f72 6368 2e54 656e 736f  nts: torch.Tenso
-00001610: 722c 0a20 2020 2065 6e64 5f63 6f6e 7374  r,.    end_const
-00001620: 7261 696e 7473 3a20 746f 7263 682e 5465  raints: torch.Te
-00001630: 6e73 6f72 2c0a 2020 2020 7472 616e 7369  nsor,.    transi
-00001640: 7469 6f6e 5f63 6f6e 7374 7261 696e 7473  tion_constraints
-00001650: 3a20 746f 7263 682e 5465 6e73 6f72 2c0a  : torch.Tensor,.
-00001660: 2920 2d3e 204e 6f6e 653a 0a20 2020 2063  ) -> None:.    c
-00001670: 6f6e 7374 7261 696e 6564 5f6c 6f67 5f70  onstrained_log_p
-00001680: 6f74 656e 7469 616c 7320 3d20 462e 636f  otentials = F.co
-00001690: 6e73 7472 6169 6e5f 6c6f 675f 706f 7465  nstrain_log_pote
-000016a0: 6e74 6961 6c73 280a 2020 2020 2020 2020  ntials(.        
-000016b0: 6c6f 675f 706f 7465 6e74 6961 6c73 2c20  log_potentials, 
-000016c0: 6d61 736b 2c20 7374 6172 745f 636f 6e73  mask, start_cons
-000016d0: 7472 6169 6e74 732c 2065 6e64 5f63 6f6e  traints, end_con
-000016e0: 7374 7261 696e 7473 2c20 7472 616e 7369  straints, transi
-000016f0: 7469 6f6e 5f63 6f6e 7374 7261 696e 7473  tion_constraints
-00001700: 0a20 2020 2029 0a20 2020 206c 656e 6774  .    ).    lengt
-00001710: 6873 203d 206d 6173 6b2e 7375 6d28 6469  hs = mask.sum(di
-00001720: 6d3d 2d31 290a 0a20 2020 2066 6f72 2069  m=-1)..    for i
-00001730: 2c20 6c6f 675f 706f 7465 6e74 6961 6c20  , log_potential 
-00001740: 696e 2065 6e75 6d65 7261 7465 2863 6f6e  in enumerate(con
-00001750: 7374 7261 696e 6564 5f6c 6f67 5f70 6f74  strained_log_pot
-00001760: 656e 7469 616c 7329 3a0a 2020 2020 2020  entials):.      
-00001770: 2020 2320 4368 6563 6b20 7374 6172 7420    # Check start 
-00001780: 636f 6e73 7472 6169 6e74 730a 2020 2020  constraints.    
-00001790: 2020 2020 666f 7220 6a2c 2076 616c 6964      for j, valid
-000017a0: 2069 6e20 656e 756d 6572 6174 6528 7374   in enumerate(st
-000017b0: 6172 745f 636f 6e73 7472 6169 6e74 7329  art_constraints)
-000017c0: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-000017d0: 7365 7274 2074 6f72 6368 2e65 7175 616c  sert torch.equal
-000017e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000017f0: 2020 6c6f 675f 706f 7465 6e74 6961 6c5b    log_potential[
-00001800: 302c 206a 2c20 6a5d 2c0a 2020 2020 2020  0, j, j],.      
-00001810: 2020 2020 2020 2020 2020 6c6f 675f 706f            log_po
-00001820: 7465 6e74 6961 6c73 5b69 2c20 302c 206a  tentials[i, 0, j
-00001830: 2c20 6a5d 2069 6620 7661 6c69 6420 656c  , j] if valid el
-00001840: 7365 2074 6f72 6368 2e74 656e 736f 7228  se torch.tensor(
-00001850: 4e49 4e46 292c 0a20 2020 2020 2020 2020  NINF),.         
-00001860: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-00001870: 4368 6563 6b20 656e 6420 636f 6e73 7472  Check end constr
-00001880: 6169 6e74 730a 2020 2020 2020 2020 666f  aints.        fo
-00001890: 7220 6a2c 2076 616c 6964 5f65 2069 6e20  r j, valid_e in 
-000018a0: 656e 756d 6572 6174 6528 656e 645f 636f  enumerate(end_co
-000018b0: 6e73 7472 6169 6e74 7329 3a0a 2020 2020  nstraints):.    
-000018c0: 2020 2020 2020 2020 656e 645f 696e 6465          end_inde
-000018d0: 7820 3d20 6c65 6e67 7468 735b 695d 202d  x = lengths[i] -
-000018e0: 2031 0a20 2020 2020 2020 2020 2020 2069   1.            i
-000018f0: 6620 7661 6c69 645f 653a 0a20 2020 2020  f valid_e:.     
-00001900: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00001910: 2c20 7661 6c69 645f 7420 696e 2065 6e75  , valid_t in enu
-00001920: 6d65 7261 7465 2874 7261 6e73 6974 696f  merate(transitio
-00001930: 6e5f 636f 6e73 7472 6169 6e74 735b 3a2c  n_constraints[:,
-00001940: 206a 5d29 3a0a 2020 2020 2020 2020 2020   j]):.          
-00001950: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00001960: 2074 6f72 6368 2e65 7175 616c 280a 2020   torch.equal(.  
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 2020 2020 2020 6c6f 675f 706f 7465 6e74        log_potent
-00001990: 6961 6c5b 656e 645f 696e 6465 782c 206b  ial[end_index, k
-000019a0: 2c20 6a5d 2c0a 2020 2020 2020 2020 2020  , j],.          
-000019b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000019c0: 675f 706f 7465 6e74 6961 6c73 5b69 2c20  g_potentials[i, 
-000019d0: 656e 645f 696e 6465 782c 206b 2c20 6a5d  end_index, k, j]
-000019e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019f0: 2020 2020 2020 2020 2069 6620 7661 6c69           if vali
-00001a00: 645f 740a 2020 2020 2020 2020 2020 2020  d_t.            
-00001a10: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001a20: 2074 6f72 6368 2e74 656e 736f 7228 4e49   torch.tensor(NI
-00001a30: 4e46 292c 0a20 2020 2020 2020 2020 2020  NF),.           
-00001a40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00001a50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00001a60: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00001a70: 6572 7420 746f 7263 682e 616c 6c28 6c6f  ert torch.all(lo
-00001a80: 675f 706f 7465 6e74 6961 6c5b 656e 645f  g_potential[end_
-00001a90: 696e 6465 782c 203a 2c20 6a5d 203d 3d20  index, :, j] == 
-00001aa0: 4e49 4e46 290a 0a20 2020 2020 2020 2023  NINF)..        #
-00001ab0: 2043 6865 636b 2074 7261 6e73 6974 696f   Check transitio
-00001ac0: 6e20 636f 6e73 7472 6169 6e74 730a 2020  n constraints.  
-00001ad0: 2020 2020 2020 666f 7220 706f 7320 696e        for pos in
-00001ae0: 2072 616e 6765 2831 2c20 6c65 6e67 7468   range(1, length
-00001af0: 735b 695d 202d 2031 293a 0a20 2020 2020  s[i] - 1):.     
-00001b00: 2020 2020 2020 2066 6f72 206a 2c20 726f         for j, ro
-00001b10: 7720 696e 2065 6e75 6d65 7261 7465 2874  w in enumerate(t
-00001b20: 7261 6e73 6974 696f 6e5f 636f 6e73 7472  ransition_constr
-00001b30: 6169 6e74 7329 3a0a 2020 2020 2020 2020  aints):.        
-00001b40: 2020 2020 2020 2020 666f 7220 6b2c 2076          for k, v
-00001b50: 616c 6964 2069 6e20 656e 756d 6572 6174  alid in enumerat
-00001b60: 6528 726f 7729 3a0a 2020 2020 2020 2020  e(row):.        
-00001b70: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00001b80: 7274 2074 6f72 6368 2e65 7175 616c 280a  rt torch.equal(.
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 2020 2020 6c6f 675f 706f 7465          log_pote
-00001bb0: 6e74 6961 6c5b 706f 732c 206a 2c20 6b5d  ntial[pos, j, k]
-00001bc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001bd0: 2020 2020 2020 2020 2020 6c6f 675f 706f            log_po
-00001be0: 7465 6e74 6961 6c73 5b69 2c20 706f 732c  tentials[i, pos,
-00001bf0: 206a 2c20 6b5d 2069 6620 7661 6c69 6420   j, k] if valid 
-00001c00: 656c 7365 2074 6f72 6368 2e74 656e 736f  else torch.tenso
-00001c10: 7228 4e49 4e46 292c 0a20 2020 2020 2020  r(NINF),.       
-00001c20: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00001c30: 0a40 7079 7465 7374 2e6d 6172 6b2e 7061  .@pytest.mark.pa
-00001c40: 7261 6d65 7472 697a 6528 0a20 2020 2022  rametrize(.    "
-00001c50: 6c6f 675f 706f 7465 6e74 6961 6c73 2c20  log_potentials, 
-00001c60: 6d61 736b 2c20 7374 6172 745f 636f 6e73  mask, start_cons
-00001c70: 7472 6169 6e74 732c 2065 6e64 5f63 6f6e  traints, end_con
-00001c80: 7374 7261 696e 7473 2c20 7472 616e 7369  straints, transi
-00001c90: 7469 6f6e 5f63 6f6e 7374 7261 696e 7473  tion_constraints
-00001ca0: 222c 0a20 2020 205b 0a20 2020 2020 2020  ",.    [.       
-00001cb0: 2028 0a20 2020 2020 2020 2020 2020 2074   (.            t
-00001cc0: 6f72 6368 2e72 616e 646e 2833 2c20 3230  orch.randn(3, 20
-00001cd0: 2c20 352c 2035 2c20 7265 7175 6972 6573  , 5, 5, requires
-00001ce0: 5f67 7261 643d 5472 7565 292c 0a20 2020  _grad=True),.   
-00001cf0: 2020 2020 2020 2020 2074 6f72 6368 2e6f           torch.o
-00001d00: 6e65 7328 2833 2c20 3230 292c 2064 7479  nes((3, 20), dty
-00001d10: 7065 3d74 6f72 6368 2e62 6f6f 6c29 2c0a  pe=torch.bool),.
-00001d20: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-00001d30: 682e 7465 6e73 6f72 285b 5472 7565 2c20  h.tensor([True, 
-00001d40: 4661 6c73 652c 2046 616c 7365 2c20 5472  False, False, Tr
-00001d50: 7565 2c20 5472 7565 5d29 2c20 2023 2030  ue, True]),  # 0
-00001d60: 2c20 332c 2034 2061 7265 2061 6c6c 6f77  , 3, 4 are allow
-00001d70: 6564 0a20 2020 2020 2020 2020 2020 2074  ed.            t
-00001d80: 6f72 6368 2e74 656e 736f 7228 5b46 616c  orch.tensor([Fal
-00001d90: 7365 2c20 5472 7565 2c20 5472 7565 2c20  se, True, True, 
-00001da0: 4661 6c73 652c 2046 616c 7365 5d29 2c20  False, False]), 
-00001db0: 2023 2032 2c20 3320 6172 6520 616c 6c6f   # 2, 3 are allo
-00001dc0: 7765 640a 2020 2020 2020 2020 2020 2020  wed.            
-00001dd0: 746f 7263 682e 7465 6e73 6f72 280a 2020  torch.tensor(.  
-00001de0: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2020 5b54 7275 652c 2046 616c 7365      [True, False
-00001e10: 2c20 5472 7565 2c20 5472 7565 2c20 5472  , True, True, Tr
-00001e20: 7565 5d2c 2020 2320 302d 3e31 2069 7320  ue],  # 0->1 is 
-00001e30: 6e6f 7420 616c 6c6f 7765 640a 2020 2020  not allowed.    
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 5b54 7275 652c 2054 7275 652c 2054 7275  [True, True, Tru
-00001e60: 652c 2054 7275 652c 2054 7275 655d 2c20  e, True, True], 
-00001e70: 2023 206e 6f20 636f 6e73 7472 6169 6e74   # no constraint
-00001e80: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00001e90: 2020 2020 2020 5b54 7275 652c 2054 7275        [True, Tru
-00001ea0: 652c 2046 616c 7365 2c20 5472 7565 2c20  e, False, True, 
-00001eb0: 5472 7565 5d2c 2020 2320 322d 3e32 2069  True],  # 2->2 i
-00001ec0: 7320 6e6f 7420 616c 6c6f 7765 640a 2020  s not allowed.  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 5b54 7275 652c 2046 616c 7365 2c20    [True, False, 
-00001ef0: 5472 7565 2c20 5472 7565 2c20 5472 7565  True, True, True
-00001f00: 5d2c 2020 2320 332d 3e31 2069 7320 6e6f  ],  # 3->1 is no
-00001f10: 7420 616c 6c6f 7765 640a 2020 2020 2020  t allowed.      
-00001f20: 2020 2020 2020 2020 2020 2020 2020 5b54                [T
-00001f30: 7275 652c 2046 616c 7365 2c20 4661 6c73  rue, False, Fals
-00001f40: 652c 2046 616c 7365 2c20 4661 6c73 655d  e, False, False]
-00001f50: 2c20 2023 206f 6e6c 7920 342d 3e30 2069  ,  # only 4->0 i
-00001f60: 7320 616c 6c6f 7765 640a 2020 2020 2020  s allowed.      
-00001f70: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00001f80: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00001f90: 2020 2029 2c0a 2020 2020 2020 2020 280a     ),.        (.
-00001fa0: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-00001fb0: 682e 7a65 726f 7328 332c 2032 302c 2035  h.zeros(3, 20, 5
-00001fc0: 2c20 352c 2072 6571 7569 7265 735f 6772  , 5, requires_gr
-00001fd0: 6164 3d54 7275 6529 2c0a 2020 2020 2020  ad=True),.      
-00001fe0: 2020 2020 2020 746f 7263 682e 6f6e 6573        torch.ones
-00001ff0: 2828 332c 2032 3029 2c20 6474 7970 653d  ((3, 20), dtype=
-00002000: 746f 7263 682e 626f 6f6c 292c 0a20 2020  torch.bool),.   
-00002010: 2020 2020 2020 2020 2074 6f72 6368 2e74           torch.t
-00002020: 656e 736f 7228 5b46 616c 7365 2c20 4661  ensor([False, Fa
-00002030: 6c73 652c 2054 7275 652c 2054 7275 652c  lse, True, True,
-00002040: 2054 7275 655d 292c 0a20 2020 2020 2020   True]),.       
-00002050: 2020 2020 2074 6f72 6368 2e74 656e 736f       torch.tenso
-00002060: 7228 5b46 616c 7365 2c20 4661 6c73 652c  r([False, False,
-00002070: 2054 7275 652c 2054 7275 652c 2054 7275   True, True, Tru
-00002080: 655d 292c 0a20 2020 2020 2020 2020 2020  e]),.           
-00002090: 2074 6f72 6368 2e74 656e 736f 7228 5b5b   torch.tensor([[
-000020a0: 5472 7565 5d20 2a20 355d 202a 2035 292c  True] * 5] * 5),
-000020b0: 0a20 2020 2020 2020 2029 2c0a 2020 2020  .        ),.    
-000020c0: 5d2c 0a29 0a64 6566 2074 6573 745f 636f  ],.).def test_co
-000020d0: 6e73 7472 6169 6e65 645f 6465 636f 6465  nstrained_decode
-000020e0: 5f72 6574 7572 6e73 5f65 7870 6563 7465  _returns_expecte
-000020f0: 645f 7461 675f 696e 6469 6365 735f 756e  d_tag_indices_un
-00002100: 6465 725f 636f 6e73 7472 6169 6e74 7328  der_constraints(
-00002110: 0a20 2020 206c 6f67 5f70 6f74 656e 7469  .    log_potenti
-00002120: 616c 733a 2074 6f72 6368 2e54 656e 736f  als: torch.Tenso
-00002130: 722c 0a20 2020 206d 6173 6b3a 2074 6f72  r,.    mask: tor
-00002140: 6368 2e54 656e 736f 722c 0a20 2020 2073  ch.Tensor,.    s
-00002150: 7461 7274 5f63 6f6e 7374 7261 696e 7473  tart_constraints
-00002160: 3a20 746f 7263 682e 5465 6e73 6f72 2c0a  : torch.Tensor,.
-00002170: 2020 2020 656e 645f 636f 6e73 7472 6169      end_constrai
-00002180: 6e74 733a 2074 6f72 6368 2e54 656e 736f  nts: torch.Tenso
-00002190: 722c 0a20 2020 2074 7261 6e73 6974 696f  r,.    transitio
-000021a0: 6e5f 636f 6e73 7472 6169 6e74 733a 2074  n_constraints: t
-000021b0: 6f72 6368 2e54 656e 736f 722c 0a29 202d  orch.Tensor,.) -
-000021c0: 3e20 4e6f 6e65 3a0a 2020 2020 636f 6e73  > None:.    cons
-000021d0: 7472 6169 6e65 645f 6c6f 675f 706f 7465  trained_log_pote
-000021e0: 6e74 6961 6c73 203d 2046 2e63 6f6e 7374  ntials = F.const
-000021f0: 7261 696e 5f6c 6f67 5f70 6f74 656e 7469  rain_log_potenti
-00002200: 616c 7328 0a20 2020 2020 2020 206c 6f67  als(.        log
-00002210: 5f70 6f74 656e 7469 616c 732c 206d 6173  _potentials, mas
-00002220: 6b2c 2073 7461 7274 5f63 6f6e 7374 7261  k, start_constra
-00002230: 696e 7473 2c20 656e 645f 636f 6e73 7472  ints, end_constr
-00002240: 6169 6e74 732c 2074 7261 6e73 6974 696f  aints, transitio
-00002250: 6e5f 636f 6e73 7472 6169 6e74 730a 2020  n_constraints.  
-00002260: 2020 290a 2020 2020 5f2c 2074 6167 5f69    ).    _, tag_i
-00002270: 6e64 6963 6573 203d 2046 2e64 6563 6f64  ndices = F.decod
-00002280: 6528 636f 6e73 7472 6169 6e65 645f 6c6f  e(constrained_lo
-00002290: 675f 706f 7465 6e74 6961 6c73 290a 0a20  g_potentials).. 
-000022a0: 2020 2061 7373 6572 7420 6865 6c70 6572     assert helper
-000022b0: 732e 6368 6563 6b5f 7461 675f 696e 6469  s.check_tag_indi
-000022c0: 6365 735f 7361 7469 7366 6965 735f 636f  ces_satisfies_co
-000022d0: 6e73 7472 6169 6e74 7328 0a20 2020 2020  nstraints(.     
-000022e0: 2020 2074 6167 5f69 6e64 6963 6573 2c20     tag_indices, 
-000022f0: 7374 6172 745f 636f 6e73 7472 6169 6e74  start_constraint
-00002300: 732c 2065 6e64 5f63 6f6e 7374 7261 696e  s, end_constrain
-00002310: 7473 2c20 7472 616e 7369 7469 6f6e 5f63  ts, transition_c
-00002320: 6f6e 7374 7261 696e 7473 0a20 2020 2029  onstraints.    )
-00002330: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-00002340: 7061 7261 6d65 7472 697a 6528 0a20 2020  parametrize(.   
-00002350: 2022 7461 675f 696e 6469 6365 732c 206e   "tag_indices, n
-00002360: 756d 5f74 6167 732c 2065 7870 6563 7465  um_tags, expecte
-00002370: 642c 2070 6172 7469 616c 5f69 6e64 6578  d, partial_index
-00002380: 222c 0a20 2020 205b 0a20 2020 2020 2020  ",.    [.       
-00002390: 2028 0a20 2020 2020 2020 2020 2020 2074   (.            t
-000023a0: 6f72 6368 2e74 656e 736f 7228 5b5b 302c  orch.tensor([[0,
-000023b0: 2031 2c20 322c 2033 2c20 345d 5d29 2c0a   1, 2, 3, 4]]),.
-000023c0: 2020 2020 2020 2020 2020 2020 352c 0a20              5,. 
-000023d0: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
-000023e0: 2e74 656e 736f 7228 0a20 2020 2020 2020  .tensor(.       
-000023f0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-00002400: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00002410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002420: 2020 2020 2020 2020 205b 5472 7565 2c20           [True, 
-00002430: 4661 6c73 652c 2046 616c 7365 2c20 4661  False, False, Fa
-00002440: 6c73 652c 2046 616c 7365 5d2c 0a20 2020  lse, False],.   
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 2020 205b 4661 6c73 652c 2054 7275       [False, Tru
-00002470: 652c 2046 616c 7365 2c20 4661 6c73 652c  e, False, False,
-00002480: 2046 616c 7365 5d2c 0a20 2020 2020 2020   False],.       
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 205b 4661 6c73 652c 2046 616c 7365 2c20   [False, False, 
-000024b0: 5472 7565 2c20 4661 6c73 652c 2046 616c  True, False, Fal
-000024c0: 7365 5d2c 0a20 2020 2020 2020 2020 2020  se],.           
-000024d0: 2020 2020 2020 2020 2020 2020 205b 4661               [Fa
-000024e0: 6c73 652c 2046 616c 7365 2c20 4661 6c73  lse, False, Fals
-000024f0: 652c 2054 7275 652c 2046 616c 7365 5d2c  e, True, False],
-00002500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002510: 2020 2020 2020 2020 205b 4661 6c73 652c           [False,
-00002520: 2046 616c 7365 2c20 4661 6c73 652c 2046   False, False, F
-00002530: 616c 7365 2c20 5472 7565 5d2c 0a20 2020  alse, True],.   
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-00002560: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-00002570: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00002580: 4e6f 6e65 2c0a 2020 2020 2020 2020 292c  None,.        ),
-00002590: 0a20 2020 2020 2020 2028 746f 7263 682e  .        (torch.
-000025a0: 7465 6e73 6f72 285b 2d31 3030 2c20 2d31  tensor([-100, -1
-000025b0: 2c20 352c 2031 3030 5d29 2c20 352c 2074  , 5, 100]), 5, t
-000025c0: 6f72 6368 2e74 656e 736f 7228 5b5b 5b46  orch.tensor([[[F
-000025d0: 616c 7365 5d20 2a20 355d 202a 2034 5d29  alse] * 5] * 4])
-000025e0: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
-000025f0: 2028 0a20 2020 2020 2020 2020 2020 2074   (.            t
-00002600: 6f72 6368 2e74 656e 736f 7228 5b5b 302c  orch.tensor([[0,
-00002610: 2031 2c20 322c 2033 2c20 342c 202d 312c   1, 2, 3, 4, -1,
-00002620: 202d 315d 5d29 2c0a 2020 2020 2020 2020   -1]]),.        
-00002630: 2020 2020 352c 0a20 2020 2020 2020 2020      5,.         
-00002640: 2020 2074 6f72 6368 2e74 656e 736f 7228     torch.tensor(
-00002650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002660: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00002670: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00000000: 6672 6f6d 2075 6e69 7474 6573 742e 6d6f  from unittest.mo
+00000010: 636b 2069 6d70 6f72 7420 7061 7463 680a  ck import patch.
+00000020: 0a69 6d70 6f72 7420 7079 7465 7374 0a69  .import pytest.i
+00000030: 6d70 6f72 7420 746f 7263 680a 6672 6f6d  mport torch.from
+00000040: 2070 6172 7469 616c 5f74 6167 6765 722e   partial_tagger.
+00000050: 6372 6620 696d 706f 7274 204e 494e 460a  crf import NINF.
+00000060: 6672 6f6d 2070 6172 7469 616c 5f74 6167  from partial_tag
+00000070: 6765 722e 6372 6620 696d 706f 7274 2066  ger.crf import f
+00000080: 756e 6374 696f 6e61 6c20 6173 2046 0a0a  unctional as F..
+00000090: 6672 6f6d 202e 2e20 696d 706f 7274 2068  from .. import h
+000000a0: 656c 7065 7273 0a0a 0a64 6566 2074 6573  elpers...def tes
+000000b0: 745f 6c6f 675f 6c69 6b65 6c69 686f 6f64  t_log_likelihood
+000000c0: 5f76 616c 6964 5f61 735f 7072 6f62 6162  _valid_as_probab
+000000d0: 696c 6974 7928 7465 7374 5f64 6174 615f  ility(test_data_
+000000e0: 736d 616c 6c3a 2074 7570 6c65 2920 2d3e  small: tuple) ->
+000000f0: 204e 6f6e 653a 0a20 2020 2028 6261 7463   None:.    (batc
+00000100: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
+00000110: 5f6c 656e 6774 682c 206e 756d 5f74 6167  _length, num_tag
+00000120: 7329 2c20 6c6f 675f 706f 7465 6e74 6961  s), log_potentia
+00000130: 6c73 203d 2074 6573 745f 6461 7461 5f73  ls = test_data_s
+00000140: 6d61 6c6c 0a0a 2020 2020 746f 7461 6c5f  mall..    total_
+00000150: 6c6f 675f 7020 3d20 746f 7263 682e 7465  log_p = torch.te
+00000160: 6e73 6f72 285b 4e49 4e46 5d20 2a20 6261  nsor([NINF] * ba
+00000170: 7463 685f 7369 7a65 290a 2020 2020 666f  tch_size).    fo
+00000180: 7220 7461 675f 696e 6469 6365 7320 696e  r tag_indices in
+00000190: 2068 656c 7065 7273 2e69 7465 7261 7465   helpers.iterate
+000001a0: 5f70 6f73 7369 626c 655f 7461 675f 696e  _possible_tag_in
+000001b0: 6469 6365 7328 7365 7175 656e 6365 5f6c  dices(sequence_l
+000001c0: 656e 6774 682c 206e 756d 5f74 6167 7329  ength, num_tags)
+000001d0: 3a0a 2020 2020 2020 2020 746f 7461 6c5f  :.        total_
+000001e0: 6c6f 675f 7020 3d20 746f 7263 682e 6c6f  log_p = torch.lo
+000001f0: 6761 6464 6578 7028 0a20 2020 2020 2020  gaddexp(.       
+00000200: 2020 2020 2074 6f74 616c 5f6c 6f67 5f70       total_log_p
+00000210: 2c20 462e 6c6f 675f 6c69 6b65 6c69 686f  , F.log_likeliho
+00000220: 6f64 286c 6f67 5f70 6f74 656e 7469 616c  od(log_potential
+00000230: 732c 2074 6f72 6368 2e74 656e 736f 7228  s, torch.tensor(
+00000240: 7461 675f 696e 6469 6365 7329 290a 2020  tag_indices)).  
+00000250: 2020 2020 2020 290a 0a20 2020 2061 7373        )..    ass
+00000260: 6572 7420 746f 7263 682e 616c 6c63 6c6f  ert torch.allclo
+00000270: 7365 2874 6f74 616c 5f6c 6f67 5f70 2e65  se(total_log_p.e
+00000280: 7870 2829 2c20 746f 7263 682e 6f6e 6573  xp(), torch.ones
+00000290: 5f6c 696b 6528 746f 7461 6c5f 6c6f 675f  _like(total_log_
+000002a0: 7029 290a 0a0a 6465 6620 7465 7374 5f6d  p))...def test_m
+000002b0: 6172 6769 6e61 6c5f 6c6f 675f 6c69 6b65  arginal_log_like
+000002c0: 6c69 686f 6f64 5f76 616c 6964 5f61 735f  lihood_valid_as_
+000002d0: 7072 6f62 6162 696c 6974 7928 7465 7374  probability(test
+000002e0: 5f64 6174 615f 736d 616c 6c3a 2074 7570  _data_small: tup
+000002f0: 6c65 2920 2d3e 204e 6f6e 653a 0a20 2020  le) -> None:.   
+00000300: 2073 6861 7065 2c20 6c6f 675f 706f 7465   shape, log_pote
+00000310: 6e74 6961 6c73 203d 2074 6573 745f 6461  ntials = test_da
+00000320: 7461 5f73 6d61 6c6c 0a0a 2020 2020 7461  ta_small..    ta
+00000330: 675f 6269 746d 6170 203d 2074 6f72 6368  g_bitmap = torch
+00000340: 2e6f 6e65 7328 7368 6170 652c 2064 7479  .ones(shape, dty
+00000350: 7065 3d74 6f72 6368 2e62 6f6f 6c29 0a20  pe=torch.bool). 
+00000360: 2020 206c 6f67 5f70 203d 2046 2e6d 6172     log_p = F.mar
+00000370: 6769 6e61 6c5f 6c6f 675f 6c69 6b65 6c69  ginal_log_likeli
+00000380: 686f 6f64 286c 6f67 5f70 6f74 656e 7469  hood(log_potenti
+00000390: 616c 732c 2074 6167 5f62 6974 6d61 7029  als, tag_bitmap)
+000003a0: 0a0a 2020 2020 6173 7365 7274 2074 6f72  ..    assert tor
+000003b0: 6368 2e61 6c6c 636c 6f73 6528 6c6f 675f  ch.allclose(log_
+000003c0: 702e 6578 7028 292c 2074 6f72 6368 2e6f  p.exp(), torch.o
+000003d0: 6e65 735f 6c69 6b65 286c 6f67 5f70 2929  nes_like(log_p))
+000003e0: 0a0a 0a64 6566 2074 6573 745f 6d61 7267  ...def test_marg
+000003f0: 696e 616c 5f6c 6f67 5f6c 696b 656c 6968  inal_log_likelih
+00000400: 6f6f 645f 6d61 7463 6865 735f 6c6f 675f  ood_matches_log_
+00000410: 6c69 6b65 6c69 686f 6f64 5f69 665f 6f6e  likelihood_if_on
+00000420: 655f 686f 745f 7461 675f 6269 746d 6170  e_hot_tag_bitmap
+00000430: 5f69 735f 6769 7665 6e28 0a20 2020 2074  _is_given(.    t
+00000440: 6573 745f 6461 7461 5f73 6d61 6c6c 3a20  est_data_small: 
+00000450: 7475 706c 652c 0a29 202d 3e20 4e6f 6e65  tuple,.) -> None
+00000460: 3a0a 2020 2020 7368 6170 652c 206c 6f67  :.    shape, log
+00000470: 5f70 6f74 656e 7469 616c 7320 3d20 7465  _potentials = te
+00000480: 7374 5f64 6174 615f 736d 616c 6c0a 0a20  st_data_small.. 
+00000490: 2020 2066 6f72 2074 6167 5f62 6974 6d61     for tag_bitma
+000004a0: 7020 696e 2068 656c 7065 7273 2e69 7465  p in helpers.ite
+000004b0: 7261 7465 5f70 6f73 7369 626c 655f 6f6e  rate_possible_on
+000004c0: 655f 686f 745f 7461 675f 6269 746d 6170  e_hot_tag_bitmap
+000004d0: 282a 7368 6170 6529 3a0a 2020 2020 2020  (*shape):.      
+000004e0: 2020 6120 3d20 462e 6c6f 675f 6c69 6b65    a = F.log_like
+000004f0: 6c69 686f 6f64 286c 6f67 5f70 6f74 656e  lihood(log_poten
+00000500: 7469 616c 732c 2074 6167 5f62 6974 6d61  tials, tag_bitma
+00000510: 702e 6c6f 6e67 2829 2e61 7267 6d61 7828  p.long().argmax(
+00000520: 6469 6d3d 2d31 2929 0a20 2020 2020 2020  dim=-1)).       
+00000530: 2062 203d 2046 2e6d 6172 6769 6e61 6c5f   b = F.marginal_
+00000540: 6c6f 675f 6c69 6b65 6c69 686f 6f64 286c  log_likelihood(l
+00000550: 6f67 5f70 6f74 656e 7469 616c 732c 2074  og_potentials, t
+00000560: 6167 5f62 6974 6d61 7029 0a0a 2020 2020  ag_bitmap)..    
+00000570: 2020 2020 6173 7365 7274 2074 6f72 6368      assert torch
+00000580: 2e61 6c6c 636c 6f73 6528 612c 2062 290a  .allclose(a, b).
+00000590: 0a0a 6465 6620 7465 7374 5f66 6f72 7761  ..def test_forwa
+000005a0: 7264 5f61 6c67 6f72 6974 686d 5f72 6574  rd_algorithm_ret
+000005b0: 7572 6e73 5f76 616c 7565 5f73 616d 655f  urns_value_same_
+000005c0: 6173 5f62 7275 7465 5f66 6f72 6365 280a  as_brute_force(.
+000005d0: 2020 2020 7465 7374 5f64 6174 615f 736d      test_data_sm
+000005e0: 616c 6c3a 2074 7570 6c65 2c0a 2920 2d3e  all: tuple,.) ->
+000005f0: 204e 6f6e 653a 0a20 2020 205f 2c20 6c6f   None:.    _, lo
+00000600: 675f 706f 7465 6e74 6961 6c73 203d 2074  g_potentials = t
+00000610: 6573 745f 6461 7461 5f73 6d61 6c6c 0a0a  est_data_small..
+00000620: 2020 2020 6c6f 675f 5a20 3d20 462e 666f      log_Z = F.fo
+00000630: 7277 6172 645f 616c 676f 7269 7468 6d28  rward_algorithm(
+00000640: 6c6f 675f 706f 7465 6e74 6961 6c73 290a  log_potentials).
+00000650: 2020 2020 6578 7065 6374 6564 5f6c 6f67      expected_log
+00000660: 5f5a 203d 2068 656c 7065 7273 2e63 6f6d  _Z = helpers.com
+00000670: 7075 7465 5f6c 6f67 5f6e 6f72 6d61 6c69  pute_log_normali
+00000680: 7a65 725f 6279 5f62 7275 7465 5f66 6f72  zer_by_brute_for
+00000690: 6365 286c 6f67 5f70 6f74 656e 7469 616c  ce(log_potential
+000006a0: 7329 0a0a 2020 2020 6173 7365 7274 2074  s)..    assert t
+000006b0: 6f72 6368 2e61 6c6c 636c 6f73 6528 6c6f  orch.allclose(lo
+000006c0: 675f 5a2c 2065 7870 6563 7465 645f 6c6f  g_Z, expected_lo
+000006d0: 675f 5a29 0a0a 0a64 6566 2074 6573 745f  g_Z)...def test_
+000006e0: 616d 6178 5f72 6574 7572 6e73 5f76 616c  amax_returns_val
+000006f0: 7565 5f73 616d 655f 6173 5f62 7275 7465  ue_same_as_brute
+00000700: 5f66 6f72 6365 2874 6573 745f 6461 7461  _force(test_data
+00000710: 5f73 6d61 6c6c 3a20 7475 706c 6529 202d  _small: tuple) -
+00000720: 3e20 4e6f 6e65 3a0a 2020 2020 5f2c 206c  > None:.    _, l
+00000730: 6f67 5f70 6f74 656e 7469 616c 7320 3d20  og_potentials = 
+00000740: 7465 7374 5f64 6174 615f 736d 616c 6c0a  test_data_small.
+00000750: 0a20 2020 206d 6178 5f73 636f 7265 203d  .    max_score =
+00000760: 2046 2e61 6d61 7828 6c6f 675f 706f 7465   F.amax(log_pote
+00000770: 6e74 6961 6c73 290a 2020 2020 6578 7065  ntials).    expe
+00000780: 6374 6564 5f6d 6178 5f73 636f 7265 2c20  cted_max_score, 
+00000790: 5f20 3d20 6865 6c70 6572 732e 636f 6d70  _ = helpers.comp
+000007a0: 7574 655f 6265 7374 5f74 6167 5f69 6e64  ute_best_tag_ind
+000007b0: 6963 6573 5f62 795f 6272 7574 655f 666f  ices_by_brute_fo
+000007c0: 7263 6528 0a20 2020 2020 2020 206c 6f67  rce(.        log
+000007d0: 5f70 6f74 656e 7469 616c 730a 2020 2020  _potentials.    
+000007e0: 290a 0a20 2020 2061 7373 6572 7420 746f  )..    assert to
+000007f0: 7263 682e 616c 6c63 6c6f 7365 286d 6178  rch.allclose(max
+00000800: 5f73 636f 7265 2c20 6578 7065 6374 6564  _score, expected
+00000810: 5f6d 6178 5f73 636f 7265 290a 0a0a 6465  _max_score)...de
+00000820: 6620 7465 7374 5f64 6563 6f64 655f 7265  f test_decode_re
+00000830: 7475 726e 735f 7661 6c75 655f 7361 6d65  turns_value_same
+00000840: 5f61 735f 6272 7574 655f 666f 7263 6528  _as_brute_force(
+00000850: 7465 7374 5f64 6174 615f 736d 616c 6c3a  test_data_small:
+00000860: 2074 7570 6c65 2920 2d3e 204e 6f6e 653a   tuple) -> None:
+00000870: 0a20 2020 205f 2c20 6c6f 675f 706f 7465  .    _, log_pote
+00000880: 6e74 6961 6c73 203d 2074 6573 745f 6461  ntials = test_da
+00000890: 7461 5f73 6d61 6c6c 0a0a 2020 2020 6d61  ta_small..    ma
+000008a0: 785f 7363 6f72 652c 2074 6167 5f69 6e64  x_score, tag_ind
+000008b0: 6963 6573 203d 2046 2e64 6563 6f64 6528  ices = F.decode(
+000008c0: 6c6f 675f 706f 7465 6e74 6961 6c73 290a  log_potentials).
+000008d0: 0a20 2020 2028 0a20 2020 2020 2020 2065  .    (.        e
+000008e0: 7870 6563 7465 645f 6d61 785f 7363 6f72  xpected_max_scor
+000008f0: 652c 0a20 2020 2020 2020 2065 7870 6563  e,.        expec
+00000900: 7465 645f 7461 675f 696e 6469 6365 732c  ted_tag_indices,
+00000910: 0a20 2020 2029 203d 2068 656c 7065 7273  .    ) = helpers
+00000920: 2e63 6f6d 7075 7465 5f62 6573 745f 7461  .compute_best_ta
+00000930: 675f 696e 6469 6365 735f 6279 5f62 7275  g_indices_by_bru
+00000940: 7465 5f66 6f72 6365 286c 6f67 5f70 6f74  te_force(log_pot
+00000950: 656e 7469 616c 7329 0a0a 2020 2020 6173  entials)..    as
+00000960: 7365 7274 2074 6f72 6368 2e61 6c6c 636c  sert torch.allcl
+00000970: 6f73 6528 6d61 785f 7363 6f72 652c 2065  ose(max_score, e
+00000980: 7870 6563 7465 645f 6d61 785f 7363 6f72  xpected_max_scor
+00000990: 6529 0a20 2020 2061 7373 6572 7420 746f  e).    assert to
+000009a0: 7263 682e 616c 6c63 6c6f 7365 2874 6167  rch.allclose(tag
+000009b0: 5f69 6e64 6963 6573 2c20 6578 7065 6374  _indices, expect
+000009c0: 6564 5f74 6167 5f69 6e64 6963 6573 290a  ed_tag_indices).
+000009d0: 0a0a 6465 6620 7465 7374 5f73 6571 7565  ..def test_seque
+000009e0: 6e63 655f 7363 6f72 655f 636f 6d70 7574  nce_score_comput
+000009f0: 6573 5f6d 6173 6b5f 636f 7272 6563 746c  es_mask_correctl
+00000a00: 7928 0a20 2020 2074 6573 745f 6461 7461  y(.    test_data
+00000a10: 5f77 6974 685f 6d61 736b 3a20 7475 706c  _with_mask: tupl
+00000a20: 652c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  e,.) -> None:.  
+00000a30: 2020 5f2c 206c 6f67 5f70 6f74 656e 7469    _, log_potenti
+00000a40: 616c 732c 2074 6167 5f69 6e64 6963 6573  als, tag_indices
+00000a50: 2c20 6d61 736b 203d 2074 6573 745f 6461  , mask = test_da
+00000a60: 7461 5f77 6974 685f 6d61 736b 0a0a 2020  ta_with_mask..  
+00000a70: 2020 7769 7468 2070 6174 6368 2822 746f    with patch("to
+00000a80: 7263 682e 5465 6e73 6f72 2e6d 756c 2229  rch.Tensor.mul")
+00000a90: 2061 7320 6d3a 0a20 2020 2020 2020 2046   as m:.        F
+00000aa0: 2e73 6571 7565 6e63 655f 7363 6f72 6528  .sequence_score(
+00000ab0: 6c6f 675f 706f 7465 6e74 6961 6c73 2c20  log_potentials, 
+00000ac0: 7461 675f 696e 6469 6365 732c 206d 6173  tag_indices, mas
+00000ad0: 6b29 0a20 2020 2020 2020 2075 7365 645f  k).        used_
+00000ae0: 6d61 736b 203d 206d 2e63 616c 6c5f 6172  mask = m.call_ar
+00000af0: 6773 5b30 5d5b 305d 0a0a 2020 2020 2020  gs[0][0]..      
+00000b00: 2020 6173 7365 7274 2068 656c 7065 7273    assert helpers
+00000b10: 2e63 6865 636b 5f73 6571 7565 6e63 655f  .check_sequence_
+00000b20: 7363 6f72 655f 6d61 736b 2875 7365 645f  score_mask(used_
+00000b30: 6d61 736b 2c20 7461 675f 696e 6469 6365  mask, tag_indice
+00000b40: 732c 206d 6173 6b29 0a0a 0a40 7079 7465  s, mask)...@pyte
+00000b50: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+00000b60: 697a 6528 0a20 2020 2022 7061 7274 6961  ize(.    "partia
+00000b70: 6c5f 696e 6465 7822 2c0a 2020 2020 6c69  l_index",.    li
+00000b80: 7374 2872 616e 6765 2835 2929 2c0a 290a  st(range(5)),.).
+00000b90: 6465 6620 7465 7374 5f6d 756c 7469 7461  def test_multita
+00000ba0: 675f 7365 7175 656e 6365 5f73 636f 7265  g_sequence_score
+00000bb0: 5f63 6f72 7265 6374 6c79 5f6d 6173 6b73  _correctly_masks
+00000bc0: 5f6c 6f67 5f70 6f74 656e 7469 616c 7328  _log_potentials(
+00000bd0: 0a20 2020 2074 6573 745f 6461 7461 5f77  .    test_data_w
+00000be0: 6974 685f 6d61 736b 3a20 7475 706c 652c  ith_mask: tuple,
+00000bf0: 2070 6172 7469 616c 5f69 6e64 6578 3a20   partial_index: 
+00000c00: 696e 740a 2920 2d3e 204e 6f6e 653a 0a20  int.) -> None:. 
+00000c10: 2020 2028 5f2c 205f 2c20 6e75 6d5f 7461     (_, _, num_ta
+00000c20: 6773 292c 206c 6f67 5f70 6f74 656e 7469  gs), log_potenti
+00000c30: 616c 732c 2074 6167 5f69 6e64 6963 6573  als, tag_indices
+00000c40: 2c20 6d61 736b 203d 2074 6573 745f 6461  , mask = test_da
+00000c50: 7461 5f77 6974 685f 6d61 736b 0a20 2020  ta_with_mask.   
+00000c60: 2074 6167 5f62 6974 6d61 7020 3d20 462e   tag_bitmap = F.
+00000c70: 746f 5f74 6167 5f62 6974 6d61 7028 7461  to_tag_bitmap(ta
+00000c80: 675f 696e 6469 6365 732c 206e 756d 5f74  g_indices, num_t
+00000c90: 6167 732c 2070 6172 7469 616c 5f69 6e64  ags, partial_ind
+00000ca0: 6578 3d70 6172 7469 616c 5f69 6e64 6578  ex=partial_index
+00000cb0: 290a 0a20 2020 2077 6974 6820 7061 7463  )..    with patc
+00000cc0: 6828 2270 6172 7469 616c 5f74 6167 6765  h("partial_tagge
+00000cd0: 722e 6372 662e 6675 6e63 7469 6f6e 616c  r.crf.functional
+00000ce0: 2e66 6f72 7761 7264 5f61 6c67 6f72 6974  .forward_algorit
+00000cf0: 686d 2229 2061 7320 6d3a 0a20 2020 2020  hm") as m:.     
+00000d00: 2020 2046 2e6d 756c 7469 7461 675f 7365     F.multitag_se
+00000d10: 7175 656e 6365 5f73 636f 7265 286c 6f67  quence_score(log
+00000d20: 5f70 6f74 656e 7469 616c 732c 2074 6167  _potentials, tag
+00000d30: 5f62 6974 6d61 702c 206d 6173 6b29 0a20  _bitmap, mask). 
+00000d40: 2020 2020 2020 2063 6f6e 7374 7261 696e         constrain
+00000d50: 6564 5f6c 6f67 5f70 6f74 656e 7469 616c  ed_log_potential
+00000d60: 7320 3d20 6d2e 6361 6c6c 5f61 7267 735b  s = m.call_args[
+00000d70: 305d 5b30 5d0a 0a20 2020 2020 2020 2061  0][0]..        a
+00000d80: 7373 6572 7420 6865 6c70 6572 732e 6368  ssert helpers.ch
+00000d90: 6563 6b5f 636f 6e73 7472 6169 6e65 645f  eck_constrained_
+00000da0: 6c6f 675f 706f 7465 6e74 6961 6c73 280a  log_potentials(.
+00000db0: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00000dc0: 706f 7465 6e74 6961 6c73 2c20 636f 6e73  potentials, cons
+00000dd0: 7472 6169 6e65 645f 6c6f 675f 706f 7465  trained_log_pote
+00000de0: 6e74 6961 6c73 2c20 7461 675f 696e 6469  ntials, tag_indi
+00000df0: 6365 732c 206d 6173 6b2c 2070 6172 7469  ces, mask, parti
+00000e00: 616c 5f69 6e64 6578 0a20 2020 2020 2020  al_index.       
+00000e10: 2029 0a0a 0a40 7079 7465 7374 2e6d 6172   )...@pytest.mar
+00000e20: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
+00000e30: 2020 2022 6c6f 675f 706f 7465 6e74 6961     "log_potentia
+00000e40: 6c73 2c20 6d61 736b 2c20 7374 6172 745f  ls, mask, start_
+00000e50: 636f 6e73 7472 6169 6e74 732c 2065 6e64  constraints, end
+00000e60: 5f63 6f6e 7374 7261 696e 7473 2c20 7472  _constraints, tr
+00000e70: 616e 7369 7469 6f6e 5f63 6f6e 7374 7261  ansition_constra
+00000e80: 696e 7473 222c 0a20 2020 205b 0a20 2020  ints",.    [.   
+00000e90: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+00000ea0: 2020 2074 6f72 6368 2e72 616e 646e 2833     torch.randn(3
+00000eb0: 2c20 3230 2c20 352c 2035 292c 0a20 2020  , 20, 5, 5),.   
+00000ec0: 2020 2020 2020 2020 2074 6f72 6368 2e74           torch.t
+00000ed0: 656e 736f 7228 0a20 2020 2020 2020 2020  ensor(.         
+00000ee0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00000ef0: 2020 2020 2020 2020 2020 2020 205b 5472               [Tr
+00000f00: 7565 5d20 2a20 3230 2c0a 2020 2020 2020  ue] * 20,.      
+00000f10: 2020 2020 2020 2020 2020 2020 2020 5b54                [T
+00000f20: 7275 655d 202a 2031 3520 2b20 5b46 616c  rue] * 15 + [Fal
+00000f30: 7365 5d20 2a20 352c 0a20 2020 2020 2020  se] * 5,.       
+00000f40: 2020 2020 2020 2020 2020 2020 205b 5472               [Tr
+00000f50: 7565 5d20 2a20 3820 2b20 5b46 616c 7365  ue] * 8 + [False
+00000f60: 5d20 2a20 3132 2c0a 2020 2020 2020 2020  ] * 12,.        
+00000f70: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00000f80: 2020 2020 2020 2020 2020 2064 7479 7065             dtype
+00000f90: 3d74 6f72 6368 2e62 6f6f 6c2c 0a20 2020  =torch.bool,.   
+00000fa0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00000fb0: 2020 2020 2020 2020 746f 7263 682e 7465          torch.te
+00000fc0: 6e73 6f72 285b 5472 7565 2c20 4661 6c73  nsor([True, Fals
+00000fd0: 652c 2046 616c 7365 2c20 5472 7565 2c20  e, False, True, 
+00000fe0: 5472 7565 5d29 2c20 2023 2030 2c20 332c  True]),  # 0, 3,
+00000ff0: 2034 2061 7265 2061 6c6c 6f77 6564 0a20   4 are allowed. 
+00001000: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
+00001010: 2e74 656e 736f 7228 5b46 616c 7365 2c20  .tensor([False, 
+00001020: 5472 7565 2c20 5472 7565 2c20 4661 6c73  True, True, Fals
+00001030: 652c 2046 616c 7365 5d29 2c20 2023 2032  e, False]),  # 2
+00001040: 2c20 3320 6172 6520 616c 6c6f 7765 640a  , 3 are allowed.
+00001050: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+00001060: 682e 7465 6e73 6f72 280a 2020 2020 2020  h.tensor(.      
+00001070: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001090: 5b54 7275 652c 2046 616c 7365 2c20 5472  [True, False, Tr
+000010a0: 7565 2c20 5472 7565 2c20 5472 7565 5d2c  ue, True, True],
+000010b0: 2020 2320 302d 3e31 2069 7320 6e6f 7420    # 0->1 is not 
+000010c0: 616c 6c6f 7765 640a 2020 2020 2020 2020  allowed.        
+000010d0: 2020 2020 2020 2020 2020 2020 5b54 7275              [Tru
+000010e0: 652c 2054 7275 652c 2054 7275 652c 2054  e, True, True, T
+000010f0: 7275 652c 2054 7275 655d 2c20 2023 206e  rue, True],  # n
+00001100: 6f20 636f 6e73 7472 6169 6e74 730a 2020  o constraints.  
+00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001120: 2020 5b54 7275 652c 2054 7275 652c 2046    [True, True, F
+00001130: 616c 7365 2c20 5472 7565 2c20 5472 7565  alse, True, True
+00001140: 5d2c 2020 2320 322d 3e32 2069 7320 6e6f  ],  # 2->2 is no
+00001150: 7420 616c 6c6f 7765 640a 2020 2020 2020  t allowed.      
+00001160: 2020 2020 2020 2020 2020 2020 2020 5b54                [T
+00001170: 7275 652c 2046 616c 7365 2c20 5472 7565  rue, False, True
+00001180: 2c20 5472 7565 2c20 5472 7565 5d2c 2020  , True, True],  
+00001190: 2320 332d 3e31 2069 7320 6e6f 7420 616c  # 3->1 is not al
+000011a0: 6c6f 7765 640a 2020 2020 2020 2020 2020  lowed.          
+000011b0: 2020 2020 2020 2020 2020 5b54 7275 652c            [True,
+000011c0: 2046 616c 7365 2c20 4661 6c73 652c 2046   False, False, F
+000011d0: 616c 7365 2c20 4661 6c73 655d 2c20 2023  alse, False],  #
+000011e0: 206f 6e6c 7920 342d 3e30 2069 7320 616c   only 4->0 is al
+000011f0: 6c6f 7765 640a 2020 2020 2020 2020 2020  lowed.          
+00001200: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00001210: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
+00001220: 0a20 2020 205d 2c0a 290a 6465 6620 7465  .    ],.).def te
+00001230: 7374 5f63 6f6e 7374 7261 696e 735f 6c6f  st_constrains_lo
+00001240: 675f 706f 7465 6e74 6961 6c73 280a 2020  g_potentials(.  
+00001250: 2020 6c6f 675f 706f 7465 6e74 6961 6c73    log_potentials
+00001260: 3a20 746f 7263 682e 5465 6e73 6f72 2c0a  : torch.Tensor,.
+00001270: 2020 2020 6d61 736b 3a20 746f 7263 682e      mask: torch.
+00001280: 5465 6e73 6f72 2c0a 2020 2020 7374 6172  Tensor,.    star
+00001290: 745f 636f 6e73 7472 6169 6e74 733a 2074  t_constraints: t
+000012a0: 6f72 6368 2e54 656e 736f 722c 0a20 2020  orch.Tensor,.   
+000012b0: 2065 6e64 5f63 6f6e 7374 7261 696e 7473   end_constraints
+000012c0: 3a20 746f 7263 682e 5465 6e73 6f72 2c0a  : torch.Tensor,.
+000012d0: 2020 2020 7472 616e 7369 7469 6f6e 5f63      transition_c
+000012e0: 6f6e 7374 7261 696e 7473 3a20 746f 7263  onstraints: torc
+000012f0: 682e 5465 6e73 6f72 2c0a 2920 2d3e 204e  h.Tensor,.) -> N
+00001300: 6f6e 653a 0a20 2020 2063 6f6e 7374 7261  one:.    constra
+00001310: 696e 6564 5f6c 6f67 5f70 6f74 656e 7469  ined_log_potenti
+00001320: 616c 7320 3d20 462e 636f 6e73 7472 6169  als = F.constrai
+00001330: 6e5f 6c6f 675f 706f 7465 6e74 6961 6c73  n_log_potentials
+00001340: 280a 2020 2020 2020 2020 6c6f 675f 706f  (.        log_po
+00001350: 7465 6e74 6961 6c73 2c20 6d61 736b 2c20  tentials, mask, 
+00001360: 7374 6172 745f 636f 6e73 7472 6169 6e74  start_constraint
+00001370: 732c 2065 6e64 5f63 6f6e 7374 7261 696e  s, end_constrain
+00001380: 7473 2c20 7472 616e 7369 7469 6f6e 5f63  ts, transition_c
+00001390: 6f6e 7374 7261 696e 7473 0a20 2020 2029  onstraints.    )
+000013a0: 0a20 2020 206c 656e 6774 6873 203d 206d  .    lengths = m
+000013b0: 6173 6b2e 7375 6d28 6469 6d3d 2d31 290a  ask.sum(dim=-1).
+000013c0: 0a20 2020 2066 6f72 2069 2c20 6c6f 675f  .    for i, log_
+000013d0: 706f 7465 6e74 6961 6c20 696e 2065 6e75  potential in enu
+000013e0: 6d65 7261 7465 2863 6f6e 7374 7261 696e  merate(constrain
+000013f0: 6564 5f6c 6f67 5f70 6f74 656e 7469 616c  ed_log_potential
+00001400: 7329 3a0a 2020 2020 2020 2020 2320 4368  s):.        # Ch
+00001410: 6563 6b20 7374 6172 7420 636f 6e73 7472  eck start constr
+00001420: 6169 6e74 730a 2020 2020 2020 2020 666f  aints.        fo
+00001430: 7220 6a2c 2076 616c 6964 2069 6e20 656e  r j, valid in en
+00001440: 756d 6572 6174 6528 7374 6172 745f 636f  umerate(start_co
+00001450: 6e73 7472 6169 6e74 7329 3a0a 2020 2020  nstraints):.    
+00001460: 2020 2020 2020 2020 6173 7365 7274 2074          assert t
+00001470: 6f72 6368 2e65 7175 616c 280a 2020 2020  orch.equal(.    
+00001480: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00001490: 706f 7465 6e74 6961 6c5b 302c 206a 2c20  potential[0, j, 
+000014a0: 6a5d 2c0a 2020 2020 2020 2020 2020 2020  j],.            
+000014b0: 2020 2020 6c6f 675f 706f 7465 6e74 6961      log_potentia
+000014c0: 6c73 5b69 2c20 302c 206a 2c20 6a5d 2069  ls[i, 0, j, j] i
+000014d0: 6620 7661 6c69 6420 656c 7365 2074 6f72  f valid else tor
+000014e0: 6368 2e74 656e 736f 7228 4e49 4e46 292c  ch.tensor(NINF),
+000014f0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00001500: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00001510: 656e 6420 636f 6e73 7472 6169 6e74 730a  end constraints.
+00001520: 2020 2020 2020 2020 666f 7220 6a2c 2076          for j, v
+00001530: 616c 6964 5f65 2069 6e20 656e 756d 6572  alid_e in enumer
+00001540: 6174 6528 656e 645f 636f 6e73 7472 6169  ate(end_constrai
+00001550: 6e74 7329 3a0a 2020 2020 2020 2020 2020  nts):.          
+00001560: 2020 656e 645f 696e 6465 7820 3d20 6c65    end_index = le
+00001570: 6e67 7468 735b 695d 202d 2031 0a20 2020  ngths[i] - 1.   
+00001580: 2020 2020 2020 2020 2069 6620 7661 6c69           if vali
+00001590: 645f 653a 0a20 2020 2020 2020 2020 2020  d_e:.           
+000015a0: 2020 2020 2066 6f72 206b 2c20 7661 6c69       for k, vali
+000015b0: 645f 7420 696e 2065 6e75 6d65 7261 7465  d_t in enumerate
+000015c0: 2874 7261 6e73 6974 696f 6e5f 636f 6e73  (transition_cons
+000015d0: 7472 6169 6e74 735b 3a2c 206a 5d29 3a0a  traints[:, j]):.
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 6173 7365 7274 2074 6f72 6368      assert torch
+00001600: 2e65 7175 616c 280a 2020 2020 2020 2020  .equal(.        
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 6c6f 675f 706f 7465 6e74 6961 6c5b 656e  log_potential[en
+00001630: 645f 696e 6465 782c 206b 2c20 6a5d 2c0a  d_index, k, j],.
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 2020 2020 2020 6c6f 675f 706f 7465          log_pote
+00001660: 6e74 6961 6c73 5b69 2c20 656e 645f 696e  ntials[i, end_in
+00001670: 6465 782c 206b 2c20 6a5d 0a20 2020 2020  dex, k, j].     
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 2020 2069 6620 7661 6c69 645f 740a 2020     if valid_t.  
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 2020 2020 2020 656c 7365 2074 6f72 6368        else torch
+000016c0: 2e74 656e 736f 7228 4e49 4e46 292c 0a20  .tensor(NINF),. 
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000016f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00001700: 2020 2020 2020 2061 7373 6572 7420 746f         assert to
+00001710: 7263 682e 616c 6c28 6c6f 675f 706f 7465  rch.all(log_pote
+00001720: 6e74 6961 6c5b 656e 645f 696e 6465 782c  ntial[end_index,
+00001730: 203a 2c20 6a5d 203d 3d20 4e49 4e46 290a   :, j] == NINF).
+00001740: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
+00001750: 2074 7261 6e73 6974 696f 6e20 636f 6e73   transition cons
+00001760: 7472 6169 6e74 730a 2020 2020 2020 2020  traints.        
+00001770: 666f 7220 706f 7320 696e 2072 616e 6765  for pos in range
+00001780: 2831 2c20 6c65 6e67 7468 735b 695d 202d  (1, lengths[i] -
+00001790: 2031 293a 0a20 2020 2020 2020 2020 2020   1):.           
+000017a0: 2066 6f72 206a 2c20 726f 7720 696e 2065   for j, row in e
+000017b0: 6e75 6d65 7261 7465 2874 7261 6e73 6974  numerate(transit
+000017c0: 696f 6e5f 636f 6e73 7472 6169 6e74 7329  ion_constraints)
+000017d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000017e0: 2020 666f 7220 6b2c 2076 616c 6964 2069    for k, valid i
+000017f0: 6e20 656e 756d 6572 6174 6528 726f 7729  n enumerate(row)
+00001800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001810: 2020 2020 2020 6173 7365 7274 2074 6f72        assert tor
+00001820: 6368 2e65 7175 616c 280a 2020 2020 2020  ch.equal(.      
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 6c6f 675f 706f 7465 6e74 6961 6c5b    log_potential[
+00001850: 706f 732c 206a 2c20 6b5d 2c0a 2020 2020  pos, j, k],.    
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 6c6f 675f 706f 7465 6e74 6961      log_potentia
+00001880: 6c73 5b69 2c20 706f 732c 206a 2c20 6b5d  ls[i, pos, j, k]
+00001890: 2069 6620 7661 6c69 6420 656c 7365 2074   if valid else t
+000018a0: 6f72 6368 2e74 656e 736f 7228 4e49 4e46  orch.tensor(NINF
+000018b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000018c0: 2020 2020 2020 2029 0a0a 0a40 7079 7465         )...@pyte
+000018d0: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+000018e0: 697a 6528 0a20 2020 2022 6c6f 675f 706f  ize(.    "log_po
+000018f0: 7465 6e74 6961 6c73 2c20 6d61 736b 2c20  tentials, mask, 
+00001900: 7374 6172 745f 636f 6e73 7472 6169 6e74  start_constraint
+00001910: 732c 2065 6e64 5f63 6f6e 7374 7261 696e  s, end_constrain
+00001920: 7473 2c20 7472 616e 7369 7469 6f6e 5f63  ts, transition_c
+00001930: 6f6e 7374 7261 696e 7473 222c 0a20 2020  onstraints",.   
+00001940: 205b 0a20 2020 2020 2020 2028 0a20 2020   [.        (.   
+00001950: 2020 2020 2020 2020 2074 6f72 6368 2e72           torch.r
+00001960: 616e 646e 2833 2c20 3230 2c20 352c 2035  andn(3, 20, 5, 5
+00001970: 2c20 7265 7175 6972 6573 5f67 7261 643d  , requires_grad=
+00001980: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+00001990: 2020 2074 6f72 6368 2e6f 6e65 7328 2833     torch.ones((3
+000019a0: 2c20 3230 292c 2064 7479 7065 3d74 6f72  , 20), dtype=tor
+000019b0: 6368 2e62 6f6f 6c29 2c0a 2020 2020 2020  ch.bool),.      
+000019c0: 2020 2020 2020 746f 7263 682e 7465 6e73        torch.tens
+000019d0: 6f72 285b 5472 7565 2c20 4661 6c73 652c  or([True, False,
+000019e0: 2046 616c 7365 2c20 5472 7565 2c20 5472   False, True, Tr
+000019f0: 7565 5d29 2c20 2023 2030 2c20 332c 2034  ue]),  # 0, 3, 4
+00001a00: 2061 7265 2061 6c6c 6f77 6564 0a20 2020   are allowed.   
+00001a10: 2020 2020 2020 2020 2074 6f72 6368 2e74           torch.t
+00001a20: 656e 736f 7228 5b46 616c 7365 2c20 5472  ensor([False, Tr
+00001a30: 7565 2c20 5472 7565 2c20 4661 6c73 652c  ue, True, False,
+00001a40: 2046 616c 7365 5d29 2c20 2023 2032 2c20   False]),  # 2, 
+00001a50: 3320 6172 6520 616c 6c6f 7765 640a 2020  3 are allowed.  
+00001a60: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
+00001a70: 7465 6e73 6f72 280a 2020 2020 2020 2020  tensor(.        
+00001a80: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00001a90: 2020 2020 2020 2020 2020 2020 2020 5b54                [T
+00001aa0: 7275 652c 2046 616c 7365 2c20 5472 7565  rue, False, True
+00001ab0: 2c20 5472 7565 2c20 5472 7565 5d2c 2020  , True, True],  
+00001ac0: 2320 302d 3e31 2069 7320 6e6f 7420 616c  # 0->1 is not al
+00001ad0: 6c6f 7765 640a 2020 2020 2020 2020 2020  lowed.          
+00001ae0: 2020 2020 2020 2020 2020 5b54 7275 652c            [True,
+00001af0: 2054 7275 652c 2054 7275 652c 2054 7275   True, True, Tru
+00001b00: 652c 2054 7275 655d 2c20 2023 206e 6f20  e, True],  # no 
+00001b10: 636f 6e73 7472 6169 6e74 730a 2020 2020  constraints.    
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b30: 5b54 7275 652c 2054 7275 652c 2046 616c  [True, True, Fal
+00001b40: 7365 2c20 5472 7565 2c20 5472 7565 5d2c  se, True, True],
+00001b50: 2020 2320 322d 3e32 2069 7320 6e6f 7420    # 2->2 is not 
+00001b60: 616c 6c6f 7765 640a 2020 2020 2020 2020  allowed.        
+00001b70: 2020 2020 2020 2020 2020 2020 5b54 7275              [Tru
+00001b80: 652c 2046 616c 7365 2c20 5472 7565 2c20  e, False, True, 
+00001b90: 5472 7565 2c20 5472 7565 5d2c 2020 2320  True, True],  # 
+00001ba0: 332d 3e31 2069 7320 6e6f 7420 616c 6c6f  3->1 is not allo
+00001bb0: 7765 640a 2020 2020 2020 2020 2020 2020  wed.            
+00001bc0: 2020 2020 2020 2020 5b54 7275 652c 2046          [True, F
+00001bd0: 616c 7365 2c20 4661 6c73 652c 2046 616c  alse, False, Fal
+00001be0: 7365 2c20 4661 6c73 655d 2c20 2023 206f  se, False],  # o
+00001bf0: 6e6c 7920 342d 3e30 2069 7320 616c 6c6f  nly 4->0 is allo
+00001c00: 7765 640a 2020 2020 2020 2020 2020 2020  wed.            
+00001c10: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00001c20: 2020 292c 0a20 2020 2020 2020 2029 2c0a    ),.        ),.
+00001c30: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+00001c40: 2020 2020 2020 746f 7263 682e 7a65 726f        torch.zero
+00001c50: 7328 332c 2032 302c 2035 2c20 352c 2072  s(3, 20, 5, 5, r
+00001c60: 6571 7569 7265 735f 6772 6164 3d54 7275  equires_grad=Tru
+00001c70: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00001c80: 746f 7263 682e 6f6e 6573 2828 332c 2032  torch.ones((3, 2
+00001c90: 3029 2c20 6474 7970 653d 746f 7263 682e  0), dtype=torch.
+00001ca0: 626f 6f6c 292c 0a20 2020 2020 2020 2020  bool),.         
+00001cb0: 2020 2074 6f72 6368 2e74 656e 736f 7228     torch.tensor(
+00001cc0: 5b46 616c 7365 2c20 4661 6c73 652c 2054  [False, False, T
+00001cd0: 7275 652c 2054 7275 652c 2054 7275 655d  rue, True, True]
+00001ce0: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
+00001cf0: 6f72 6368 2e74 656e 736f 7228 5b46 616c  orch.tensor([Fal
+00001d00: 7365 2c20 4661 6c73 652c 2054 7275 652c  se, False, True,
+00001d10: 2054 7275 652c 2054 7275 655d 292c 0a20   True, True]),. 
+00001d20: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
+00001d30: 2e74 656e 736f 7228 5b5b 5472 7565 5d20  .tensor([[True] 
+00001d40: 2a20 355d 202a 2035 292c 0a20 2020 2020  * 5] * 5),.     
+00001d50: 2020 2029 2c0a 2020 2020 5d2c 0a29 0a64     ),.    ],.).d
+00001d60: 6566 2074 6573 745f 636f 6e73 7472 6169  ef test_constrai
+00001d70: 6e65 645f 6465 636f 6465 5f72 6574 7572  ned_decode_retur
+00001d80: 6e73 5f65 7870 6563 7465 645f 7461 675f  ns_expected_tag_
+00001d90: 696e 6469 6365 735f 756e 6465 725f 636f  indices_under_co
+00001da0: 6e73 7472 6169 6e74 7328 0a20 2020 206c  nstraints(.    l
+00001db0: 6f67 5f70 6f74 656e 7469 616c 733a 2074  og_potentials: t
+00001dc0: 6f72 6368 2e54 656e 736f 722c 0a20 2020  orch.Tensor,.   
+00001dd0: 206d 6173 6b3a 2074 6f72 6368 2e54 656e   mask: torch.Ten
+00001de0: 736f 722c 0a20 2020 2073 7461 7274 5f63  sor,.    start_c
+00001df0: 6f6e 7374 7261 696e 7473 3a20 746f 7263  onstraints: torc
+00001e00: 682e 5465 6e73 6f72 2c0a 2020 2020 656e  h.Tensor,.    en
+00001e10: 645f 636f 6e73 7472 6169 6e74 733a 2074  d_constraints: t
+00001e20: 6f72 6368 2e54 656e 736f 722c 0a20 2020  orch.Tensor,.   
+00001e30: 2074 7261 6e73 6974 696f 6e5f 636f 6e73   transition_cons
+00001e40: 7472 6169 6e74 733a 2074 6f72 6368 2e54  traints: torch.T
+00001e50: 656e 736f 722c 0a29 202d 3e20 4e6f 6e65  ensor,.) -> None
+00001e60: 3a0a 2020 2020 636f 6e73 7472 6169 6e65  :.    constraine
+00001e70: 645f 6c6f 675f 706f 7465 6e74 6961 6c73  d_log_potentials
+00001e80: 203d 2046 2e63 6f6e 7374 7261 696e 5f6c   = F.constrain_l
+00001e90: 6f67 5f70 6f74 656e 7469 616c 7328 0a20  og_potentials(. 
+00001ea0: 2020 2020 2020 206c 6f67 5f70 6f74 656e         log_poten
+00001eb0: 7469 616c 732c 206d 6173 6b2c 2073 7461  tials, mask, sta
+00001ec0: 7274 5f63 6f6e 7374 7261 696e 7473 2c20  rt_constraints, 
+00001ed0: 656e 645f 636f 6e73 7472 6169 6e74 732c  end_constraints,
+00001ee0: 2074 7261 6e73 6974 696f 6e5f 636f 6e73   transition_cons
+00001ef0: 7472 6169 6e74 730a 2020 2020 290a 2020  traints.    ).  
+00001f00: 2020 5f2c 2074 6167 5f69 6e64 6963 6573    _, tag_indices
+00001f10: 203d 2046 2e64 6563 6f64 6528 636f 6e73   = F.decode(cons
+00001f20: 7472 6169 6e65 645f 6c6f 675f 706f 7465  trained_log_pote
+00001f30: 6e74 6961 6c73 290a 0a20 2020 2061 7373  ntials)..    ass
+00001f40: 6572 7420 6865 6c70 6572 732e 6368 6563  ert helpers.chec
+00001f50: 6b5f 7461 675f 696e 6469 6365 735f 7361  k_tag_indices_sa
+00001f60: 7469 7366 6965 735f 636f 6e73 7472 6169  tisfies_constrai
+00001f70: 6e74 7328 0a20 2020 2020 2020 2074 6167  nts(.        tag
+00001f80: 5f69 6e64 6963 6573 2c20 7374 6172 745f  _indices, start_
+00001f90: 636f 6e73 7472 6169 6e74 732c 2065 6e64  constraints, end
+00001fa0: 5f63 6f6e 7374 7261 696e 7473 2c20 7472  _constraints, tr
+00001fb0: 616e 7369 7469 6f6e 5f63 6f6e 7374 7261  ansition_constra
+00001fc0: 696e 7473 0a20 2020 2029 0a0a 0a40 7079  ints.    )...@py
+00001fd0: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+00001fe0: 7472 697a 6528 0a20 2020 2022 7461 675f  trize(.    "tag_
+00001ff0: 696e 6469 6365 732c 206e 756d 5f74 6167  indices, num_tag
+00002000: 732c 2065 7870 6563 7465 642c 2070 6172  s, expected, par
+00002010: 7469 616c 5f69 6e64 6578 222c 0a20 2020  tial_index",.   
+00002020: 205b 0a20 2020 2020 2020 2028 0a20 2020   [.        (.   
+00002030: 2020 2020 2020 2020 2074 6f72 6368 2e74           torch.t
+00002040: 656e 736f 7228 5b5b 302c 2031 2c20 322c  ensor([[0, 1, 2,
+00002050: 2033 2c20 345d 5d29 2c0a 2020 2020 2020   3, 4]]),.      
+00002060: 2020 2020 2020 352c 0a20 2020 2020 2020        5,.       
+00002070: 2020 2020 2074 6f72 6368 2e74 656e 736f       torch.tenso
+00002080: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00002090: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+000020a0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020c0: 2020 205b 5472 7565 2c20 4661 6c73 652c     [True, False,
+000020d0: 2046 616c 7365 2c20 4661 6c73 652c 2046   False, False, F
+000020e0: 616c 7365 5d2c 0a20 2020 2020 2020 2020  alse],.         
+000020f0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00002100: 4661 6c73 652c 2054 7275 652c 2046 616c  False, True, Fal
+00002110: 7365 2c20 4661 6c73 652c 2046 616c 7365  se, False, False
+00002120: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002130: 2020 2020 2020 2020 2020 205b 4661 6c73             [Fals
+00002140: 652c 2046 616c 7365 2c20 5472 7565 2c20  e, False, True, 
+00002150: 4661 6c73 652c 2046 616c 7365 5d2c 0a20  False, False],. 
+00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002170: 2020 2020 2020 205b 4661 6c73 652c 2046         [False, F
+00002180: 616c 7365 2c20 4661 6c73 652c 2054 7275  alse, False, Tru
+00002190: 652c 2046 616c 7365 5d2c 0a20 2020 2020  e, False],.     
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 2020 205b 4661 6c73 652c 2046 616c 7365     [False, False
+000021c0: 2c20 4661 6c73 652c 2046 616c 7365 2c20  , False, False, 
+000021d0: 5472 7565 5d2c 0a20 2020 2020 2020 2020  True],.         
+000021e0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+000021f0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+00002200: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00002210: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
+00002220: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00002230: 2020 2028 746f 7263 682e 7465 6e73 6f72     (torch.tensor
+00002240: 285b 2d31 3030 2c20 2d31 2c20 352c 2031  ([-100, -1, 5, 1
+00002250: 3030 5d29 2c20 352c 2074 6f72 6368 2e74  00]), 5, torch.t
+00002260: 656e 736f 7228 5b5b 5b46 616c 7365 5d20  ensor([[[False] 
+00002270: 2a20 355d 202a 2034 5d29 2c20 4e6f 6e65  * 5] * 4]), None
+00002280: 292c 0a20 2020 2020 2020 2028 0a20 2020  ),.        (.   
+00002290: 2020 2020 2020 2020 2074 6f72 6368 2e74           torch.t
+000022a0: 656e 736f 7228 5b5b 302c 2031 2c20 322c  ensor([[0, 1, 2,
+000022b0: 2033 2c20 342c 202d 312c 202d 315d 5d29   3, 4, -1, -1]])
+000022c0: 2c0a 2020 2020 2020 2020 2020 2020 352c  ,.            5,
+000022d0: 0a20 2020 2020 2020 2020 2020 2074 6f72  .            tor
+000022e0: 6368 2e74 656e 736f 7228 0a20 2020 2020  ch.tensor(.     
+000022f0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002310: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00002320: 2020 2020 2020 2020 2020 205b 5472 7565             [True
+00002330: 2c20 4661 6c73 652c 2046 616c 7365 2c20  , False, False, 
+00002340: 4661 6c73 652c 2046 616c 7365 5d2c 0a20  False, False],. 
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2020 2020 205b 4661 6c73 652c 2054         [False, T
+00002370: 7275 652c 2046 616c 7365 2c20 4661 6c73  rue, False, Fals
+00002380: 652c 2046 616c 7365 5d2c 0a20 2020 2020  e, False],.     
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 205b 4661 6c73 652c 2046 616c 7365     [False, False
+000023b0: 2c20 5472 7565 2c20 4661 6c73 652c 2046  , True, False, F
+000023c0: 616c 7365 5d2c 0a20 2020 2020 2020 2020  alse],.         
+000023d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000023e0: 4661 6c73 652c 2046 616c 7365 2c20 4661  False, False, Fa
+000023f0: 6c73 652c 2054 7275 652c 2046 616c 7365  lse, True, False
+00002400: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002410: 2020 2020 2020 2020 2020 205b 4661 6c73             [Fals
+00002420: 652c 2046 616c 7365 2c20 4661 6c73 652c  e, False, False,
+00002430: 2046 616c 7365 2c20 5472 7565 5d2c 0a20   False, True],. 
+00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002450: 2020 2020 2020 205b 5472 7565 2c20 5472         [True, Tr
+00002460: 7565 2c20 5472 7565 2c20 5472 7565 2c20  ue, True, True, 
+00002470: 5472 7565 5d2c 0a20 2020 2020 2020 2020  True],.         
+00002480: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00002490: 5472 7565 2c20 5472 7565 2c20 5472 7565  True, True, True
+000024a0: 2c20 5472 7565 2c20 5472 7565 5d2c 0a20  , True, True],. 
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+000024d0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+000024e0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+000024f0: 2020 2d31 2c0a 2020 2020 2020 2020 292c    -1,.        ),
+00002500: 0a20 2020 2020 2020 2028 0a20 2020 2020  .        (.     
+00002510: 2020 2020 2020 2074 6f72 6368 2e74 656e         torch.ten
+00002520: 736f 7228 5b5b 342c 2031 2c20 322c 2033  sor([[4, 1, 2, 3
+00002530: 2c20 342c 2030 2c20 305d 5d29 2c0a 2020  , 4, 0, 0]]),.  
+00002540: 2020 2020 2020 2020 2020 352c 0a20 2020            5,.   
+00002550: 2020 2020 2020 2020 2074 6f72 6368 2e74           torch.t
+00002560: 656e 736f 7228 0a20 2020 2020 2020 2020  ensor(.         
+00002570: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00002580: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 2020 2020 205b 4661 6c73 652c 2046         [False, F
+000025b0: 616c 7365 2c20 4661 6c73 652c 2046 616c  alse, False, Fal
+000025c0: 7365 2c20 5472 7565 5d2c 0a20 2020 2020  se, True],.     
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 205b 4661 6c73 652c 2054 7275 652c     [False, True,
+000025f0: 2046 616c 7365 2c20 4661 6c73 652c 2046   False, False, F
+00002600: 616c 7365 5d2c 0a20 2020 2020 2020 2020  alse],.         
+00002610: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00002620: 4661 6c73 652c 2046 616c 7365 2c20 5472  False, False, Tr
+00002630: 7565 2c20 4661 6c73 652c 2046 616c 7365  ue, False, False
+00002640: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002650: 2020 2020 2020 2020 2020 205b 4661 6c73             [Fals
+00002660: 652c 2046 616c 7365 2c20 4661 6c73 652c  e, False, False,
+00002670: 2054 7275 652c 2046 616c 7365 5d2c 0a20   True, False],. 
 00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 205b 5472 7565 2c20 4661 6c73 652c 2046   [True, False, F
+00002690: 2020 2020 2020 205b 4661 6c73 652c 2046         [False, F
 000026a0: 616c 7365 2c20 4661 6c73 652c 2046 616c  alse, False, Fal
-000026b0: 7365 5d2c 0a20 2020 2020 2020 2020 2020  se],.           
-000026c0: 2020 2020 2020 2020 2020 2020 205b 4661               [Fa
-000026d0: 6c73 652c 2054 7275 652c 2046 616c 7365  lse, True, False
-000026e0: 2c20 4661 6c73 652c 2046 616c 7365 5d2c  , False, False],
-000026f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002700: 2020 2020 2020 2020 205b 4661 6c73 652c           [False,
-00002710: 2046 616c 7365 2c20 5472 7565 2c20 4661   False, True, Fa
-00002720: 6c73 652c 2046 616c 7365 5d2c 0a20 2020  lse, False],.   
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 205b 4661 6c73 652c 2046 616c       [False, Fal
-00002750: 7365 2c20 4661 6c73 652c 2054 7275 652c  se, False, True,
-00002760: 2046 616c 7365 5d2c 0a20 2020 2020 2020   False],.       
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 205b 4661 6c73 652c 2046 616c 7365 2c20   [False, False, 
-00002790: 4661 6c73 652c 2046 616c 7365 2c20 5472  False, False, Tr
-000027a0: 7565 5d2c 0a20 2020 2020 2020 2020 2020  ue],.           
-000027b0: 2020 2020 2020 2020 2020 2020 205b 5472               [Tr
-000027c0: 7565 2c20 5472 7565 2c20 5472 7565 2c20  ue, True, True, 
-000027d0: 5472 7565 2c20 5472 7565 5d2c 0a20 2020  True, True],.   
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 2020 2020 205b 5472 7565 2c20 5472 7565       [True, True
-00002800: 2c20 5472 7565 2c20 5472 7565 2c20 5472  , True, True, Tr
-00002810: 7565 5d2c 0a20 2020 2020 2020 2020 2020  ue],.           
-00002820: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00002830: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00002840: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00002850: 2020 2020 2020 2020 2d31 2c0a 2020 2020          -1,.    
-00002860: 2020 2020 292c 0a20 2020 2020 2020 2028      ),.        (
-00002870: 0a20 2020 2020 2020 2020 2020 2074 6f72  .            tor
-00002880: 6368 2e74 656e 736f 7228 5b5b 342c 2031  ch.tensor([[4, 1
-00002890: 2c20 322c 2033 2c20 342c 2030 2c20 305d  , 2, 3, 4, 0, 0]
-000028a0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000028b0: 352c 0a20 2020 2020 2020 2020 2020 2074  5,.            t
-000028c0: 6f72 6368 2e74 656e 736f 7228 0a20 2020  orch.tensor(.   
-000028d0: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00002900: 2020 2020 2020 2020 2020 2020 205b 4661               [Fa
-00002910: 6c73 652c 2046 616c 7365 2c20 4661 6c73  lse, False, Fals
-00002920: 652c 2046 616c 7365 2c20 5472 7565 5d2c  e, False, True],
-00002930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002940: 2020 2020 2020 2020 205b 4661 6c73 652c           [False,
-00002950: 2054 7275 652c 2046 616c 7365 2c20 4661   True, False, Fa
-00002960: 6c73 652c 2046 616c 7365 5d2c 0a20 2020  lse, False],.   
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 205b 4661 6c73 652c 2046 616c       [False, Fal
-00002990: 7365 2c20 5472 7565 2c20 4661 6c73 652c  se, True, False,
-000029a0: 2046 616c 7365 5d2c 0a20 2020 2020 2020   False],.       
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 205b 4661 6c73 652c 2046 616c 7365 2c20   [False, False, 
-000029d0: 4661 6c73 652c 2054 7275 652c 2046 616c  False, True, Fal
-000029e0: 7365 5d2c 0a20 2020 2020 2020 2020 2020  se],.           
-000029f0: 2020 2020 2020 2020 2020 2020 205b 4661               [Fa
-00002a00: 6c73 652c 2046 616c 7365 2c20 4661 6c73  lse, False, Fals
-00002a10: 652c 2046 616c 7365 2c20 5472 7565 5d2c  e, False, True],
-00002a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a30: 2020 2020 2020 2020 205b 5472 7565 2c20           [True, 
-00002a40: 5472 7565 2c20 5472 7565 2c20 5472 7565  True, True, True
-00002a50: 2c20 5472 7565 5d2c 0a20 2020 2020 2020  , True],.       
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 205b 5472 7565 2c20 5472 7565 2c20 5472   [True, True, Tr
-00002a80: 7565 2c20 5472 7565 2c20 5472 7565 5d2c  ue, True, True],
-00002a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002aa0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-00002ab0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00002ac0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00002ad0: 2020 2020 302c 0a20 2020 2020 2020 2029      0,.        )
-00002ae0: 2c0a 2020 2020 5d2c 0a29 0a64 6566 2074  ,.    ],.).def t
-00002af0: 6573 745f 7461 675f 6269 746d 6170 5f72  est_tag_bitmap_r
-00002b00: 6574 7572 6e73 5f65 7870 6563 7465 645f  eturns_expected_
-00002b10: 7661 6c75 6528 0a20 2020 2074 6167 5f69  value(.    tag_i
-00002b20: 6e64 6963 6573 3a20 746f 7263 682e 5465  ndices: torch.Te
-00002b30: 6e73 6f72 2c20 6e75 6d5f 7461 6773 3a20  nsor, num_tags: 
-00002b40: 696e 742c 2065 7870 6563 7465 643a 2074  int, expected: t
-00002b50: 6f72 6368 2e54 656e 736f 722c 2070 6172  orch.Tensor, par
-00002b60: 7469 616c 5f69 6e64 6578 3a20 696e 740a  tial_index: int.
-00002b70: 2920 2d3e 204e 6f6e 653a 0a20 2020 2061  ) -> None:.    a
-00002b80: 7373 6572 7420 746f 7263 682e 6571 7561  ssert torch.equa
-00002b90: 6c28 462e 746f 5f74 6167 5f62 6974 6d61  l(F.to_tag_bitma
-00002ba0: 7028 7461 675f 696e 6469 6365 732c 206e  p(tag_indices, n
-00002bb0: 756d 5f74 6167 732c 2070 6172 7469 616c  um_tags, partial
-00002bc0: 5f69 6e64 6578 292c 2065 7870 6563 7465  _index), expecte
-00002bd0: 6429 0a                                  d).
+000026b0: 7365 2c20 5472 7565 5d2c 0a20 2020 2020  se, True],.     
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026d0: 2020 205b 5472 7565 2c20 5472 7565 2c20     [True, True, 
+000026e0: 5472 7565 2c20 5472 7565 2c20 5472 7565  True, True, True
+000026f0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002700: 2020 2020 2020 2020 2020 205b 5472 7565             [True
+00002710: 2c20 5472 7565 2c20 5472 7565 2c20 5472  , True, True, Tr
+00002720: 7565 2c20 5472 7565 5d2c 0a20 2020 2020  ue, True],.     
+00002730: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 205d 0a20 2020 2020 2020 2020 2020 2029   ].            )
+00002760: 2c0a 2020 2020 2020 2020 2020 2020 302c  ,.            0,
+00002770: 0a20 2020 2020 2020 2029 2c0a 2020 2020  .        ),.    
+00002780: 5d2c 0a29 0a64 6566 2074 6573 745f 7461  ],.).def test_ta
+00002790: 675f 6269 746d 6170 5f72 6574 7572 6e73  g_bitmap_returns
+000027a0: 5f65 7870 6563 7465 645f 7661 6c75 6528  _expected_value(
+000027b0: 0a20 2020 2074 6167 5f69 6e64 6963 6573  .    tag_indices
+000027c0: 3a20 746f 7263 682e 5465 6e73 6f72 2c20  : torch.Tensor, 
+000027d0: 6e75 6d5f 7461 6773 3a20 696e 742c 2065  num_tags: int, e
+000027e0: 7870 6563 7465 643a 2074 6f72 6368 2e54  xpected: torch.T
+000027f0: 656e 736f 722c 2070 6172 7469 616c 5f69  ensor, partial_i
+00002800: 6e64 6578 3a20 696e 740a 2920 2d3e 204e  ndex: int.) -> N
+00002810: 6f6e 653a 0a20 2020 2061 7373 6572 7420  one:.    assert 
+00002820: 746f 7263 682e 6571 7561 6c28 462e 746f  torch.equal(F.to
+00002830: 5f74 6167 5f62 6974 6d61 7028 7461 675f  _tag_bitmap(tag_
+00002840: 696e 6469 6365 732c 206e 756d 5f74 6167  indices, num_tag
+00002850: 732c 2070 6172 7469 616c 5f69 6e64 6578  s, partial_index
+00002860: 292c 2065 7870 6563 7465 6429 0a         ), expected).
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/15a8b9aa8a597371` & `pytorch_partial_tagger-0.1.2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,209 +1,182 @@
-00000000: 0100 0000 0000 0000 0e00 0000 0000 0000  ................
-00000010: 7465 7374 732e 636f 6e66 7465 7374 0300  tests.conftest..
-00000020: 0000 0000 0000 0600 0000 0000 0000 7079  ..............py
-00000030: 7465 7374 0000 0000 0d00 0000 0500 0000  test............
-00000040: 0000 0000 746f 7263 680e 0000 001a 0000  ....torch.......
-00000050: 0017 0000 0000 0000 0070 6172 7469 616c  .........partial
-00000060: 5f74 6167 6765 722e 6372 662e 4e49 4e46  _tagger.crf.NINF
-00000070: 3b00 0000 3f00 0000 0100 0000 0000 0000  ;...?...........
-00000080: 0f00 0000 0000 0000 556e 736f 7274 6564  ........Unsorted
-00000090: 496d 706f 7274 7329 0000 0000 0000 0049  Imports).......I
-000000a0: 6d70 6f72 7420 626c 6f63 6b20 6973 2075  mport block is u
-000000b0: 6e2d 736f 7274 6564 206f 7220 756e 2d66  n-sorted or un-f
-000000c0: 6f72 6d61 7474 6564 0110 0000 0000 0000  ormatted........
-000000d0: 004f 7267 616e 697a 6520 696d 706f 7274  .Organize import
-000000e0: 7300 0000 0042 0000 0001 0100 0000 0000  s....B..........
-000000f0: 0000 0000 0000 4200 0000 0141 0000 0000  ......B....A....
-00000100: 0000 0069 6d70 6f72 7420 7079 7465 7374  ...import pytest
-00000110: 0a69 6d70 6f72 7420 746f 7263 680a 6672  .import torch.fr
-00000120: 6f6d 2070 6172 7469 616c 5f74 6167 6765  om partial_tagge
-00000130: 722e 6372 6620 696d 706f 7274 204e 494e  r.crf import NIN
-00000140: 460a 0a0a 0300 0000 0000 0000 0000 0000  F...............
-00000150: 0000 0000 0100 0000 0000 0000 4200 0000  ............B...
-00000160: 0000 0000 2f55 7365 7273 2f79 6173 7566  ..../Users/yasuf
-00000170: 756d 692f 576f 726b 7370 6163 652f 7079  umi/Workspace/py
-00000180: 746f 7263 682d 7061 7274 6961 6c2d 7461  torch-partial-ta
-00000190: 6767 6572 2f74 6573 7473 2f63 6f6e 6674  gger/tests/conft
-000001a0: 6573 742e 7079 5d0b 0000 0000 0000 696d  est.py].......im
-000001b0: 706f 7274 2070 7974 6573 740a 696d 706f  port pytest.impo
-000001c0: 7274 2074 6f72 6368 0a0a 6672 6f6d 2070  rt torch..from p
-000001d0: 6172 7469 616c 5f74 6167 6765 722e 6372  artial_tagger.cr
-000001e0: 6620 696d 706f 7274 204e 494e 460a 0a0a  f import NINF...
-000001f0: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
-00000200: 6465 6620 6e75 6d5f 7461 6773 2829 202d  def num_tags() -
-00000210: 3e20 696e 743a 0a20 2020 2072 6574 7572  > int:.    retur
-00000220: 6e20 350a 0a0a 4070 7974 6573 742e 6669  n 5...@pytest.fi
-00000230: 7874 7572 650a 6465 6620 7465 7374 5f64  xture.def test_d
-00000240: 6174 615f 666f 725f 7368 6170 655f 6368  ata_for_shape_ch
-00000250: 6563 6b28 6e75 6d5f 7461 6773 3a20 696e  eck(num_tags: in
-00000260: 7429 202d 3e20 7475 706c 653a 0a20 2020  t) -> tuple:.   
-00000270: 2062 6174 6368 5f73 697a 6520 3d20 330a   batch_size = 3.
-00000280: 2020 2020 7365 7175 656e 6365 5f6c 656e      sequence_len
-00000290: 6774 6820 3d20 3230 0a20 2020 2065 6d62  gth = 20.    emb
-000002a0: 6564 6469 6e67 5f73 697a 6520 3d20 3132  edding_size = 12
-000002b0: 380a 2020 2020 656d 6265 6464 696e 6773  8.    embeddings
-000002c0: 203d 2074 6f72 6368 2e72 616e 646e 2862   = torch.randn(b
-000002d0: 6174 6368 5f73 697a 652c 2073 6571 7565  atch_size, seque
-000002e0: 6e63 655f 6c65 6e67 7468 2c20 656d 6265  nce_length, embe
-000002f0: 6464 696e 675f 7369 7a65 290a 2020 2020  dding_size).    
-00000300: 6c6f 6769 7473 203d 2074 6f72 6368 2e72  logits = torch.r
-00000310: 616e 646e 2862 6174 6368 5f73 697a 652c  andn(batch_size,
-00000320: 2073 6571 7565 6e63 655f 6c65 6e67 7468   sequence_length
-00000330: 2c20 6e75 6d5f 7461 6773 290a 2020 2020  , num_tags).    
-00000340: 6c6f 675f 706f 7465 6e74 6961 6c73 203d  log_potentials =
-00000350: 2074 6f72 6368 2e72 616e 646e 2862 6174   torch.randn(bat
-00000360: 6368 5f73 697a 652c 2073 6571 7565 6e63  ch_size, sequenc
-00000370: 655f 6c65 6e67 7468 2c20 6e75 6d5f 7461  e_length, num_ta
-00000380: 6773 2c20 6e75 6d5f 7461 6773 290a 2020  gs, num_tags).  
-00000390: 2020 7461 675f 696e 6469 6365 7320 3d20    tag_indices = 
-000003a0: 746f 7263 682e 7261 6e64 696e 7428 302c  torch.randint(0,
-000003b0: 206e 756d 5f74 6167 732c 2028 6261 7463   num_tags, (batc
-000003c0: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
-000003d0: 5f6c 656e 6774 6829 290a 2020 2020 7461  _length)).    ta
-000003e0: 675f 6269 746d 6170 203d 2074 6f72 6368  g_bitmap = torch
-000003f0: 2e6e 6e2e 6675 6e63 7469 6f6e 616c 2e6f  .nn.functional.o
-00000400: 6e65 5f68 6f74 2874 6167 5f69 6e64 6963  ne_hot(tag_indic
-00000410: 6573 2c20 6e75 6d5f 7461 6773 292e 626f  es, num_tags).bo
-00000420: 6f6c 2829 0a0a 2020 2020 7265 7475 726e  ol()..    return
-00000430: 2028 0a20 2020 2020 2020 2028 6261 7463   (.        (batc
-00000440: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
-00000450: 5f6c 656e 6774 682c 2065 6d62 6564 6469  _length, embeddi
-00000460: 6e67 5f73 697a 652c 206e 756d 5f74 6167  ng_size, num_tag
-00000470: 7329 2c0a 2020 2020 2020 2020 656d 6265  s),.        embe
-00000480: 6464 696e 6773 2c0a 2020 2020 2020 2020  ddings,.        
-00000490: 6c6f 6769 7473 2c0a 2020 2020 2020 2020  logits,.        
-000004a0: 6c6f 675f 706f 7465 6e74 6961 6c73 2c0a  log_potentials,.
-000004b0: 2020 2020 2020 2020 7461 675f 696e 6469          tag_indi
-000004c0: 6365 732c 0a20 2020 2020 2020 2074 6167  ces,.        tag
-000004d0: 5f62 6974 6d61 702c 0a20 2020 2029 0a0a  _bitmap,.    )..
-000004e0: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
-000004f0: 0a64 6566 2074 6573 745f 6461 7461 5f73  .def test_data_s
-00000500: 6d61 6c6c 286e 756d 5f74 6167 733a 2069  mall(num_tags: i
-00000510: 6e74 2920 2d3e 2074 7570 6c65 3a0a 2020  nt) -> tuple:.  
-00000520: 2020 6261 7463 685f 7369 7a65 203d 2032    batch_size = 2
-00000530: 0a20 2020 2073 6571 7565 6e63 655f 6c65  .    sequence_le
-00000540: 6e67 7468 203d 2033 0a20 2020 206c 6f67  ngth = 3.    log
-00000550: 5f70 6f74 656e 7469 616c 7320 3d20 746f  _potentials = to
-00000560: 7263 682e 7261 6e64 6e28 6261 7463 685f  rch.randn(batch_
-00000570: 7369 7a65 2c20 7365 7175 656e 6365 5f6c  size, sequence_l
-00000580: 656e 6774 682c 206e 756d 5f74 6167 732c  ength, num_tags,
-00000590: 206e 756d 5f74 6167 7329 0a20 2020 2069   num_tags).    i
-000005a0: 6e69 7469 616c 5f6d 6173 6b20 3d20 746f  nitial_mask = to
-000005b0: 7263 682e 6579 6528 6e75 6d5f 7461 6773  rch.eye(num_tags
-000005c0: 2c20 6e75 6d5f 7461 6773 292e 626f 6f6c  , num_tags).bool
-000005d0: 2829 0a20 2020 206c 6f67 5f70 6f74 656e  ().    log_poten
-000005e0: 7469 616c 735b 3a2c 2030 5d20 3d20 6c6f  tials[:, 0] = lo
-000005f0: 675f 706f 7465 6e74 6961 6c73 5b3a 2c20  g_potentials[:, 
-00000600: 305d 202a 2069 6e69 7469 616c 5f6d 6173  0] * initial_mas
-00000610: 6b20 2b20 4e49 4e46 202a 2028 7e69 6e69  k + NINF * (~ini
-00000620: 7469 616c 5f6d 6173 6b29 0a20 2020 206c  tial_mask).    l
-00000630: 6f67 5f70 6f74 656e 7469 616c 732e 7265  og_potentials.re
-00000640: 7175 6972 6573 5f67 7261 645f 2829 0a20  quires_grad_(). 
-00000650: 2020 2072 6574 7572 6e20 2862 6174 6368     return (batch
-00000660: 5f73 697a 652c 2073 6571 7565 6e63 655f  _size, sequence_
-00000670: 6c65 6e67 7468 2c20 6e75 6d5f 7461 6773  length, num_tags
-00000680: 292c 206c 6f67 5f70 6f74 656e 7469 616c  ), log_potential
-00000690: 730a 0a0a 4070 7974 6573 742e 6669 7874  s...@pytest.fixt
-000006a0: 7572 650a 6465 6620 7472 616e 7369 7469  ure.def transiti
-000006b0: 6f6e 7328 2920 2d3e 2074 6f72 6368 2e54  ons() -> torch.T
-000006c0: 656e 736f 723a 0a20 2020 2072 6574 7572  ensor:.    retur
-000006d0: 6e20 746f 7263 682e 7465 6e73 6f72 280a  n torch.tensor(.
-000006e0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-000006f0: 2020 2020 2020 2320 4f20 2020 422d 5820        # O   B-X 
-00000700: 2049 2d58 2020 422d 5920 2049 2d59 0a20   I-X  B-Y  I-Y. 
-00000710: 2020 2020 2020 2020 2020 205b 302e 302c             [0.0,
-00000720: 2031 2e30 2c20 302e 302c 2030 2e30 2c20   1.0, 0.0, 0.0, 
-00000730: 302e 305d 2c20 2023 204f 0a20 2020 2020  0.0],  # O.     
-00000740: 2020 2020 2020 205b 302e 302c 2030 2e30         [0.0, 0.0
-00000750: 2c20 312e 302c 2030 2e30 2c20 302e 305d  , 1.0, 0.0, 0.0]
-00000760: 2c20 2023 2042 2d58 0a20 2020 2020 2020  ,  # B-X.       
-00000770: 2020 2020 205b 302e 302c 2030 2e30 2c20       [0.0, 0.0, 
-00000780: 302e 302c 2031 2e30 2c20 302e 305d 2c20  0.0, 1.0, 0.0], 
-00000790: 2023 2049 2d58 0a20 2020 2020 2020 2020   # I-X.         
-000007a0: 2020 205b 302e 302c 2030 2e30 2c20 302e     [0.0, 0.0, 0.
-000007b0: 302c 2030 2e30 2c20 312e 305d 2c20 2023  0, 0.0, 1.0],  #
-000007c0: 2042 2d59 0a20 2020 2020 2020 2020 2020   B-Y.           
-000007d0: 205b 312e 302c 2030 2e30 2c20 302e 302c   [1.0, 0.0, 0.0,
-000007e0: 2030 2e30 2c20 302e 305d 2c20 2023 2049   0.0, 0.0],  # I
-000007f0: 2d59 0a20 2020 2020 2020 205d 0a20 2020  -Y.        ].   
-00000800: 2029 0a0a 0a40 7079 7465 7374 2e66 6978   )...@pytest.fix
-00000810: 7475 7265 0a64 6566 2074 6573 745f 6461  ture.def test_da
-00000820: 7461 5f62 795f 6861 6e64 286e 756d 5f74  ta_by_hand(num_t
-00000830: 6167 733a 2069 6e74 2920 2d3e 2074 7570  ags: int) -> tup
-00000840: 6c65 3a0a 2020 2020 6261 7463 685f 7369  le:.    batch_si
-00000850: 7a65 203d 2032 0a20 2020 2073 6571 7565  ze = 2.    seque
-00000860: 6e63 655f 6c65 6e67 7468 203d 2033 0a20  nce_length = 3. 
-00000870: 2020 206c 6f67 6974 7320 3d20 746f 7263     logits = torc
-00000880: 682e 7465 6e73 6f72 280a 2020 2020 2020  h.tensor(.      
-00000890: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000008a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-000008b0: 2020 5b30 2e30 2c20 312e 302c 2030 2e30    [0.0, 1.0, 0.0
-000008c0: 2c20 302e 302c 2030 2e30 5d2c 0a20 2020  , 0.0, 0.0],.   
-000008d0: 2020 2020 2020 2020 2020 2020 205b 302e               [0.
-000008e0: 302c 2030 2e30 2c20 312e 302c 2030 2e30  0, 0.0, 1.0, 0.0
-000008f0: 2c20 302e 305d 2c0a 2020 2020 2020 2020  , 0.0],.        
-00000900: 2020 2020 2020 2020 5b30 2e30 2c20 302e          [0.0, 0.
-00000910: 302c 2030 2e30 2c20 312e 302c 2030 2e30  0, 0.0, 1.0, 0.0
-00000920: 5d2c 0a20 2020 2020 2020 2020 2020 205d  ],.            ]
-00000930: 2c0a 2020 2020 2020 2020 2020 2020 5b0a  ,.            [.
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 5b30 2e30 2c20 302e 302c 2030 2e30 2c20  [0.0, 0.0, 0.0, 
-00000960: 312e 302c 2030 2e30 5d2c 0a20 2020 2020  1.0, 0.0],.     
-00000970: 2020 2020 2020 2020 2020 205b 302e 302c             [0.0,
-00000980: 2030 2e30 2c20 302e 302c 2030 2e30 2c20   0.0, 0.0, 0.0, 
-00000990: 312e 305d 2c0a 2020 2020 2020 2020 2020  1.0],.          
-000009a0: 2020 2020 2020 5b30 2e30 2c20 302e 302c        [0.0, 0.0,
-000009b0: 2030 2e30 2c20 302e 302c 2031 3030 2e30   0.0, 0.0, 100.0
-000009c0: 5d2c 0a20 2020 2020 2020 2020 2020 205d  ],.            ]
-000009d0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
-000009e0: 290a 2020 2020 7461 675f 696e 6469 6365  ).    tag_indice
-000009f0: 7320 3d20 746f 7263 682e 7465 6e73 6f72  s = torch.tensor
-00000a00: 285b 5b31 2c20 322c 2033 5d2c 205b 332c  ([[1, 2, 3], [3,
-00000a10: 2034 2c20 345d 5d29 0a20 2020 2072 6574   4, 4]]).    ret
-00000a20: 7572 6e20 2862 6174 6368 5f73 697a 652c  urn (batch_size,
-00000a30: 2073 6571 7565 6e63 655f 6c65 6e67 7468   sequence_length
-00000a40: 2c20 6e75 6d5f 7461 6773 292c 206c 6f67  , num_tags), log
-00000a50: 6974 732c 2074 6167 5f69 6e64 6963 6573  its, tag_indices
-00000a60: 0a0a 0a40 7079 7465 7374 2e66 6978 7475  ...@pytest.fixtu
-00000a70: 7265 0a64 6566 2074 6573 745f 6461 7461  re.def test_data
-00000a80: 5f77 6974 685f 6d61 736b 286e 756d 5f74  _with_mask(num_t
-00000a90: 6167 733a 2069 6e74 2920 2d3e 2074 7570  ags: int) -> tup
-00000aa0: 6c65 3a0a 2020 2020 6261 7463 685f 7369  le:.    batch_si
-00000ab0: 7a65 203d 2033 0a20 2020 2073 6571 7565  ze = 3.    seque
-00000ac0: 6e63 655f 6c65 6e67 7468 203d 2032 300a  nce_length = 20.
-00000ad0: 2020 2020 6c6f 675f 706f 7465 6e74 6961      log_potentia
-00000ae0: 6c73 203d 2074 6f72 6368 2e72 616e 646e  ls = torch.randn
-00000af0: 2862 6174 6368 5f73 697a 652c 2073 6571  (batch_size, seq
-00000b00: 7565 6e63 655f 6c65 6e67 7468 2c20 6e75  uence_length, nu
-00000b10: 6d5f 7461 6773 2c20 6e75 6d5f 7461 6773  m_tags, num_tags
-00000b20: 290a 2020 2020 2320 6120 6475 6d6d 7920  ).    # a dummy 
-00000b30: 696e 6974 6961 6c20 746f 6b65 6e0a 2020  initial token.  
-00000b40: 2020 696e 6974 6961 6c5f 6d61 736b 203d    initial_mask =
-00000b50: 2074 6f72 6368 2e65 7965 286e 756d 5f74   torch.eye(num_t
-00000b60: 6167 732c 206e 756d 5f74 6167 7329 2e62  ags, num_tags).b
-00000b70: 6f6f 6c28 290a 2020 2020 6c6f 675f 706f  ool().    log_po
-00000b80: 7465 6e74 6961 6c73 5b3a 2c20 305d 203d  tentials[:, 0] =
-00000b90: 206c 6f67 5f70 6f74 656e 7469 616c 735b   log_potentials[
-00000ba0: 3a2c 2030 5d20 2a20 696e 6974 6961 6c5f  :, 0] * initial_
-00000bb0: 6d61 736b 202b 204e 494e 4620 2a20 287e  mask + NINF * (~
-00000bc0: 696e 6974 6961 6c5f 6d61 736b 290a 2020  initial_mask).  
-00000bd0: 2020 6d61 736b 203d 2074 6f72 6368 2e74    mask = torch.t
-00000be0: 656e 736f 7228 0a20 2020 2020 2020 205b  ensor(.        [
-00000bf0: 0a20 2020 2020 2020 2020 2020 205b 5472  .            [Tr
-00000c00: 7565 5d20 2a20 2873 6571 7565 6e63 655f  ue] * (sequence_
-00000c10: 6c65 6e67 7468 202d 2032 202a 2069 2920  length - 2 * i) 
-00000c20: 2b20 5b46 616c 7365 5d20 2a20 3220 2a20  + [False] * 2 * 
-00000c30: 690a 2020 2020 2020 2020 2020 2020 666f  i.            fo
-00000c40: 7220 6920 696e 2072 616e 6765 2862 6174  r i in range(bat
-00000c50: 6368 5f73 697a 6529 0a20 2020 2020 2020  ch_size).       
-00000c60: 205d 0a20 2020 2029 0a20 2020 2074 6167   ].    ).    tag
-00000c70: 5f69 6e64 6963 6573 203d 2074 6f72 6368  _indices = torch
-00000c80: 2e72 616e 6469 6e74 2830 2c20 6e75 6d5f  .randint(0, num_
-00000c90: 7461 6773 2c20 2862 6174 6368 5f73 697a  tags, (batch_siz
-00000ca0: 652c 2073 6571 7565 6e63 655f 6c65 6e67  e, sequence_leng
-00000cb0: 7468 2929 0a20 2020 2072 6574 7572 6e20  th)).    return 
-00000cc0: 2862 6174 6368 5f73 697a 652c 2073 6571  (batch_size, seq
-00000cd0: 7565 6e63 655f 6c65 6e67 7468 2c20 6e75  uence_length, nu
-00000ce0: 6d5f 7461 6773 292c 206c 6f67 5f70 6f74  m_tags), log_pot
-00000cf0: 656e 7469 616c 732c 2074 6167 5f69 6e64  entials, tag_ind
-00000d00: 6963 6573 2c20 6d61 736b 0a              ices, mask.
+00000000: 696d 706f 7274 2070 7974 6573 740a 696d  import pytest.im
+00000010: 706f 7274 2074 6f72 6368 0a66 726f 6d20  port torch.from 
+00000020: 7061 7274 6961 6c5f 7461 6767 6572 2e63  partial_tagger.c
+00000030: 7266 2069 6d70 6f72 7420 4e49 4e46 0a0a  rf import NINF..
+00000040: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
+00000050: 0a64 6566 206e 756d 5f74 6167 7328 2920  .def num_tags() 
+00000060: 2d3e 2069 6e74 3a0a 2020 2020 7265 7475  -> int:.    retu
+00000070: 726e 2035 0a0a 0a40 7079 7465 7374 2e66  rn 5...@pytest.f
+00000080: 6978 7475 7265 0a64 6566 2074 6573 745f  ixture.def test_
+00000090: 6461 7461 5f66 6f72 5f73 6861 7065 5f63  data_for_shape_c
+000000a0: 6865 636b 286e 756d 5f74 6167 733a 2069  heck(num_tags: i
+000000b0: 6e74 2920 2d3e 2074 7570 6c65 3a0a 2020  nt) -> tuple:.  
+000000c0: 2020 6261 7463 685f 7369 7a65 203d 2033    batch_size = 3
+000000d0: 0a20 2020 2073 6571 7565 6e63 655f 6c65  .    sequence_le
+000000e0: 6e67 7468 203d 2032 300a 2020 2020 656d  ngth = 20.    em
+000000f0: 6265 6464 696e 675f 7369 7a65 203d 2031  bedding_size = 1
+00000100: 3238 0a20 2020 2065 6d62 6564 6469 6e67  28.    embedding
+00000110: 7320 3d20 746f 7263 682e 7261 6e64 6e28  s = torch.randn(
+00000120: 6261 7463 685f 7369 7a65 2c20 7365 7175  batch_size, sequ
+00000130: 656e 6365 5f6c 656e 6774 682c 2065 6d62  ence_length, emb
+00000140: 6564 6469 6e67 5f73 697a 6529 0a20 2020  edding_size).   
+00000150: 206c 6f67 6974 7320 3d20 746f 7263 682e   logits = torch.
+00000160: 7261 6e64 6e28 6261 7463 685f 7369 7a65  randn(batch_size
+00000170: 2c20 7365 7175 656e 6365 5f6c 656e 6774  , sequence_lengt
+00000180: 682c 206e 756d 5f74 6167 7329 0a20 2020  h, num_tags).   
+00000190: 206c 6f67 5f70 6f74 656e 7469 616c 7320   log_potentials 
+000001a0: 3d20 746f 7263 682e 7261 6e64 6e28 6261  = torch.randn(ba
+000001b0: 7463 685f 7369 7a65 2c20 7365 7175 656e  tch_size, sequen
+000001c0: 6365 5f6c 656e 6774 682c 206e 756d 5f74  ce_length, num_t
+000001d0: 6167 732c 206e 756d 5f74 6167 7329 0a20  ags, num_tags). 
+000001e0: 2020 2074 6167 5f69 6e64 6963 6573 203d     tag_indices =
+000001f0: 2074 6f72 6368 2e72 616e 6469 6e74 2830   torch.randint(0
+00000200: 2c20 6e75 6d5f 7461 6773 2c20 2862 6174  , num_tags, (bat
+00000210: 6368 5f73 697a 652c 2073 6571 7565 6e63  ch_size, sequenc
+00000220: 655f 6c65 6e67 7468 2929 0a20 2020 2074  e_length)).    t
+00000230: 6167 5f62 6974 6d61 7020 3d20 746f 7263  ag_bitmap = torc
+00000240: 682e 6e6e 2e66 756e 6374 696f 6e61 6c2e  h.nn.functional.
+00000250: 6f6e 655f 686f 7428 7461 675f 696e 6469  one_hot(tag_indi
+00000260: 6365 732c 206e 756d 5f74 6167 7329 2e62  ces, num_tags).b
+00000270: 6f6f 6c28 290a 0a20 2020 2072 6574 7572  ool()..    retur
+00000280: 6e20 280a 2020 2020 2020 2020 2862 6174  n (.        (bat
+00000290: 6368 5f73 697a 652c 2073 6571 7565 6e63  ch_size, sequenc
+000002a0: 655f 6c65 6e67 7468 2c20 656d 6265 6464  e_length, embedd
+000002b0: 696e 675f 7369 7a65 2c20 6e75 6d5f 7461  ing_size, num_ta
+000002c0: 6773 292c 0a20 2020 2020 2020 2065 6d62  gs),.        emb
+000002d0: 6564 6469 6e67 732c 0a20 2020 2020 2020  eddings,.       
+000002e0: 206c 6f67 6974 732c 0a20 2020 2020 2020   logits,.       
+000002f0: 206c 6f67 5f70 6f74 656e 7469 616c 732c   log_potentials,
+00000300: 0a20 2020 2020 2020 2074 6167 5f69 6e64  .        tag_ind
+00000310: 6963 6573 2c0a 2020 2020 2020 2020 7461  ices,.        ta
+00000320: 675f 6269 746d 6170 2c0a 2020 2020 290a  g_bitmap,.    ).
+00000330: 0a0a 4070 7974 6573 742e 6669 7874 7572  ..@pytest.fixtur
+00000340: 650a 6465 6620 7465 7374 5f64 6174 615f  e.def test_data_
+00000350: 736d 616c 6c28 6e75 6d5f 7461 6773 3a20  small(num_tags: 
+00000360: 696e 7429 202d 3e20 7475 706c 653a 0a20  int) -> tuple:. 
+00000370: 2020 2062 6174 6368 5f73 697a 6520 3d20     batch_size = 
+00000380: 320a 2020 2020 7365 7175 656e 6365 5f6c  2.    sequence_l
+00000390: 656e 6774 6820 3d20 330a 2020 2020 6c6f  ength = 3.    lo
+000003a0: 675f 706f 7465 6e74 6961 6c73 203d 2074  g_potentials = t
+000003b0: 6f72 6368 2e72 616e 646e 2862 6174 6368  orch.randn(batch
+000003c0: 5f73 697a 652c 2073 6571 7565 6e63 655f  _size, sequence_
+000003d0: 6c65 6e67 7468 2c20 6e75 6d5f 7461 6773  length, num_tags
+000003e0: 2c20 6e75 6d5f 7461 6773 290a 2020 2020  , num_tags).    
+000003f0: 696e 6974 6961 6c5f 6d61 736b 203d 2074  initial_mask = t
+00000400: 6f72 6368 2e65 7965 286e 756d 5f74 6167  orch.eye(num_tag
+00000410: 732c 206e 756d 5f74 6167 7329 2e62 6f6f  s, num_tags).boo
+00000420: 6c28 290a 2020 2020 6c6f 675f 706f 7465  l().    log_pote
+00000430: 6e74 6961 6c73 5b3a 2c20 305d 203d 206c  ntials[:, 0] = l
+00000440: 6f67 5f70 6f74 656e 7469 616c 735b 3a2c  og_potentials[:,
+00000450: 2030 5d20 2a20 696e 6974 6961 6c5f 6d61   0] * initial_ma
+00000460: 736b 202b 204e 494e 4620 2a20 287e 696e  sk + NINF * (~in
+00000470: 6974 6961 6c5f 6d61 736b 290a 2020 2020  itial_mask).    
+00000480: 6c6f 675f 706f 7465 6e74 6961 6c73 2e72  log_potentials.r
+00000490: 6571 7569 7265 735f 6772 6164 5f28 290a  equires_grad_().
+000004a0: 2020 2020 7265 7475 726e 2028 6261 7463      return (batc
+000004b0: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
+000004c0: 5f6c 656e 6774 682c 206e 756d 5f74 6167  _length, num_tag
+000004d0: 7329 2c20 6c6f 675f 706f 7465 6e74 6961  s), log_potentia
+000004e0: 6c73 0a0a 0a40 7079 7465 7374 2e66 6978  ls...@pytest.fix
+000004f0: 7475 7265 0a64 6566 2074 7261 6e73 6974  ture.def transit
+00000500: 696f 6e73 2829 202d 3e20 746f 7263 682e  ions() -> torch.
+00000510: 5465 6e73 6f72 3a0a 2020 2020 7265 7475  Tensor:.    retu
+00000520: 726e 2074 6f72 6368 2e74 656e 736f 7228  rn torch.tensor(
+00000530: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00000540: 2020 2020 2020 2023 204f 2020 2042 2d58         # O   B-X
+00000550: 2020 492d 5820 2042 2d59 2020 492d 590a    I-X  B-Y  I-Y.
+00000560: 2020 2020 2020 2020 2020 2020 5b30 2e30              [0.0
+00000570: 2c20 312e 302c 2030 2e30 2c20 302e 302c  , 1.0, 0.0, 0.0,
+00000580: 2030 2e30 5d2c 2020 2320 4f0a 2020 2020   0.0],  # O.    
+00000590: 2020 2020 2020 2020 5b30 2e30 2c20 302e          [0.0, 0.
+000005a0: 302c 2031 2e30 2c20 302e 302c 2030 2e30  0, 1.0, 0.0, 0.0
+000005b0: 5d2c 2020 2320 422d 580a 2020 2020 2020  ],  # B-X.      
+000005c0: 2020 2020 2020 5b30 2e30 2c20 302e 302c        [0.0, 0.0,
+000005d0: 2030 2e30 2c20 312e 302c 2030 2e30 5d2c   0.0, 1.0, 0.0],
+000005e0: 2020 2320 492d 580a 2020 2020 2020 2020    # I-X.        
+000005f0: 2020 2020 5b30 2e30 2c20 302e 302c 2030      [0.0, 0.0, 0
+00000600: 2e30 2c20 302e 302c 2031 2e30 5d2c 2020  .0, 0.0, 1.0],  
+00000610: 2320 422d 590a 2020 2020 2020 2020 2020  # B-Y.          
+00000620: 2020 5b31 2e30 2c20 302e 302c 2030 2e30    [1.0, 0.0, 0.0
+00000630: 2c20 302e 302c 2030 2e30 5d2c 2020 2320  , 0.0, 0.0],  # 
+00000640: 492d 590a 2020 2020 2020 2020 5d0a 2020  I-Y.        ].  
+00000650: 2020 290a 0a0a 4070 7974 6573 742e 6669    )...@pytest.fi
+00000660: 7874 7572 650a 6465 6620 7465 7374 5f64  xture.def test_d
+00000670: 6174 615f 6279 5f68 616e 6428 6e75 6d5f  ata_by_hand(num_
+00000680: 7461 6773 3a20 696e 7429 202d 3e20 7475  tags: int) -> tu
+00000690: 706c 653a 0a20 2020 2062 6174 6368 5f73  ple:.    batch_s
+000006a0: 697a 6520 3d20 320a 2020 2020 7365 7175  ize = 2.    sequ
+000006b0: 656e 6365 5f6c 656e 6774 6820 3d20 330a  ence_length = 3.
+000006c0: 2020 2020 6c6f 6769 7473 203d 2074 6f72      logits = tor
+000006d0: 6368 2e74 656e 736f 7228 0a20 2020 2020  ch.tensor(.     
+000006e0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+000006f0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00000700: 2020 205b 302e 302c 2031 2e30 2c20 302e     [0.0, 1.0, 0.
+00000710: 302c 2030 2e30 2c20 302e 305d 2c0a 2020  0, 0.0, 0.0],.  
+00000720: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
+00000730: 2e30 2c20 302e 302c 2031 2e30 2c20 302e  .0, 0.0, 1.0, 0.
+00000740: 302c 2030 2e30 5d2c 0a20 2020 2020 2020  0, 0.0],.       
+00000750: 2020 2020 2020 2020 205b 302e 302c 2030           [0.0, 0
+00000760: 2e30 2c20 302e 302c 2031 2e30 2c20 302e  .0, 0.0, 1.0, 0.
+00000770: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00000780: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00000790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007a0: 205b 302e 302c 2030 2e30 2c20 302e 302c   [0.0, 0.0, 0.0,
+000007b0: 2031 2e30 2c20 302e 305d 2c0a 2020 2020   1.0, 0.0],.    
+000007c0: 2020 2020 2020 2020 2020 2020 5b30 2e30              [0.0
+000007d0: 2c20 302e 302c 2030 2e30 2c20 302e 302c  , 0.0, 0.0, 0.0,
+000007e0: 2031 2e30 5d2c 0a20 2020 2020 2020 2020   1.0],.         
+000007f0: 2020 2020 2020 205b 302e 302c 2030 2e30         [0.0, 0.0
+00000800: 2c20 302e 302c 2030 2e30 2c20 3130 302e  , 0.0, 0.0, 100.
+00000810: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00000820: 5d2c 0a20 2020 2020 2020 205d 0a20 2020  ],.        ].   
+00000830: 2029 0a20 2020 2074 6167 5f69 6e64 6963   ).    tag_indic
+00000840: 6573 203d 2074 6f72 6368 2e74 656e 736f  es = torch.tenso
+00000850: 7228 5b5b 312c 2032 2c20 335d 2c20 5b33  r([[1, 2, 3], [3
+00000860: 2c20 342c 2034 5d5d 290a 2020 2020 7265  , 4, 4]]).    re
+00000870: 7475 726e 2028 6261 7463 685f 7369 7a65  turn (batch_size
+00000880: 2c20 7365 7175 656e 6365 5f6c 656e 6774  , sequence_lengt
+00000890: 682c 206e 756d 5f74 6167 7329 2c20 6c6f  h, num_tags), lo
+000008a0: 6769 7473 2c20 7461 675f 696e 6469 6365  gits, tag_indice
+000008b0: 730a 0a0a 4070 7974 6573 742e 6669 7874  s...@pytest.fixt
+000008c0: 7572 650a 6465 6620 7465 7374 5f64 6174  ure.def test_dat
+000008d0: 615f 7769 7468 5f6d 6173 6b28 6e75 6d5f  a_with_mask(num_
+000008e0: 7461 6773 3a20 696e 7429 202d 3e20 7475  tags: int) -> tu
+000008f0: 706c 653a 0a20 2020 2062 6174 6368 5f73  ple:.    batch_s
+00000900: 697a 6520 3d20 330a 2020 2020 7365 7175  ize = 3.    sequ
+00000910: 656e 6365 5f6c 656e 6774 6820 3d20 3230  ence_length = 20
+00000920: 0a20 2020 206c 6f67 5f70 6f74 656e 7469  .    log_potenti
+00000930: 616c 7320 3d20 746f 7263 682e 7261 6e64  als = torch.rand
+00000940: 6e28 6261 7463 685f 7369 7a65 2c20 7365  n(batch_size, se
+00000950: 7175 656e 6365 5f6c 656e 6774 682c 206e  quence_length, n
+00000960: 756d 5f74 6167 732c 206e 756d 5f74 6167  um_tags, num_tag
+00000970: 7329 0a20 2020 2023 2061 2064 756d 6d79  s).    # a dummy
+00000980: 2069 6e69 7469 616c 2074 6f6b 656e 0a20   initial token. 
+00000990: 2020 2069 6e69 7469 616c 5f6d 6173 6b20     initial_mask 
+000009a0: 3d20 746f 7263 682e 6579 6528 6e75 6d5f  = torch.eye(num_
+000009b0: 7461 6773 2c20 6e75 6d5f 7461 6773 292e  tags, num_tags).
+000009c0: 626f 6f6c 2829 0a20 2020 206c 6f67 5f70  bool().    log_p
+000009d0: 6f74 656e 7469 616c 735b 3a2c 2030 5d20  otentials[:, 0] 
+000009e0: 3d20 6c6f 675f 706f 7465 6e74 6961 6c73  = log_potentials
+000009f0: 5b3a 2c20 305d 202a 2069 6e69 7469 616c  [:, 0] * initial
+00000a00: 5f6d 6173 6b20 2b20 4e49 4e46 202a 2028  _mask + NINF * (
+00000a10: 7e69 6e69 7469 616c 5f6d 6173 6b29 0a20  ~initial_mask). 
+00000a20: 2020 206d 6173 6b20 3d20 746f 7263 682e     mask = torch.
+00000a30: 7465 6e73 6f72 280a 2020 2020 2020 2020  tensor(.        
+00000a40: 5b0a 2020 2020 2020 2020 2020 2020 5b54  [.            [T
+00000a50: 7275 655d 202a 2028 7365 7175 656e 6365  rue] * (sequence
+00000a60: 5f6c 656e 6774 6820 2d20 3220 2a20 6929  _length - 2 * i)
+00000a70: 202b 205b 4661 6c73 655d 202a 2032 202a   + [False] * 2 *
+00000a80: 2069 0a20 2020 2020 2020 2020 2020 2066   i.            f
+00000a90: 6f72 2069 2069 6e20 7261 6e67 6528 6261  or i in range(ba
+00000aa0: 7463 685f 7369 7a65 290a 2020 2020 2020  tch_size).      
+00000ab0: 2020 5d0a 2020 2020 290a 2020 2020 7461    ].    ).    ta
+00000ac0: 675f 696e 6469 6365 7320 3d20 746f 7263  g_indices = torc
+00000ad0: 682e 7261 6e64 696e 7428 302c 206e 756d  h.randint(0, num
+00000ae0: 5f74 6167 732c 2028 6261 7463 685f 7369  _tags, (batch_si
+00000af0: 7a65 2c20 7365 7175 656e 6365 5f6c 656e  ze, sequence_len
+00000b00: 6774 6829 290a 2020 2020 7265 7475 726e  gth)).    return
+00000b10: 2028 6261 7463 685f 7369 7a65 2c20 7365   (batch_size, se
+00000b20: 7175 656e 6365 5f6c 656e 6774 682c 206e  quence_length, n
+00000b30: 756d 5f74 6167 7329 2c20 6c6f 675f 706f  um_tags), log_po
+00000b40: 7465 6e74 6961 6c73 2c20 7461 675f 696e  tentials, tag_in
+00000b50: 6469 6365 732c 206d 6173 6b0a            dices, mask.
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/1ecacb9f21faa08c` & `pytorch_partial_tagger-0.1.2/tests/crf/test_nn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,58 @@
-00000000: 0100 0000 0000 0000 1100 0000 0000 0000  ................
-00000010: 7465 7374 732e 6372 662e 7465 7374 5f6e  tests.crf.test_n
-00000020: 6e04 0000 0000 0000 0006 0000 0000 0000  n...............
-00000030: 0070 7974 6573 7400 0000 000d 0000 0005  .pytest.........
-00000040: 0000 0000 0000 0074 6f72 6368 0e00 0000  .......torch....
-00000050: 1a00 0000 1900 0000 0000 0000 7061 7274  ............part
-00000060: 6961 6c5f 7461 6767 6572 2e63 7266 2e6e  ial_tagger.crf.n
-00000070: 6e2e 4352 463e 0000 0041 0000 000d 0000  n.CRF>...A......
-00000080: 0000 0000 0074 6573 7473 2e68 656c 7065  .....tests.helpe
-00000090: 7273 5200 0000 5900 0000 0100 0000 0000  rsR...Y.........
-000000a0: 0000 0f00 0000 0000 0000 556e 736f 7274  ..........Unsort
-000000b0: 6564 496d 706f 7274 7329 0000 0000 0000  edImports)......
-000000c0: 0049 6d70 6f72 7420 626c 6f63 6b20 6973  .Import block is
-000000d0: 2075 6e2d 736f 7274 6564 206f 7220 756e   un-sorted or un
-000000e0: 2d66 6f72 6d61 7474 6564 0110 0000 0000  -formatted......
-000000f0: 0000 004f 7267 616e 697a 6520 696d 706f  ...Organize impo
-00000100: 7274 7300 0000 005c 0000 0001 0100 0000  rts....\........
-00000110: 0000 0000 0000 0000 5c00 0000 015b 0000  ........\....[..
-00000120: 0000 0000 0069 6d70 6f72 7420 7079 7465  .....import pyte
-00000130: 7374 0a69 6d70 6f72 7420 746f 7263 680a  st.import torch.
-00000140: 6672 6f6d 2070 6172 7469 616c 5f74 6167  from partial_tag
-00000150: 6765 722e 6372 662e 6e6e 2069 6d70 6f72  ger.crf.nn impor
-00000160: 7420 4352 460a 0a66 726f 6d20 2e2e 2069  t CRF..from .. i
-00000170: 6d70 6f72 7420 6865 6c70 6572 730a 0a0a  mport helpers...
-00000180: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0100 0000 0000 0000 4500 0000 0000 0000  ........E.......
-000001a0: 2f55 7365 7273 2f79 6173 7566 756d 692f  /Users/yasufumi/
-000001b0: 576f 726b 7370 6163 652f 7079 746f 7263  Workspace/pytorc
-000001c0: 682d 7061 7274 6961 6c2d 7461 6767 6572  h-partial-tagger
-000001d0: 2f74 6573 7473 2f63 7266 2f74 6573 745f  /tests/crf/test_
-000001e0: 6e6e 2e70 7993 0300 0000 0000 0069 6d70  nn.py........imp
-000001f0: 6f72 7420 7079 7465 7374 0a69 6d70 6f72  ort pytest.impor
-00000200: 7420 746f 7263 680a 0a66 726f 6d20 7061  t torch..from pa
-00000210: 7274 6961 6c5f 7461 6767 6572 2e63 7266  rtial_tagger.crf
-00000220: 2e6e 6e20 696d 706f 7274 2043 5246 0a0a  .nn import CRF..
-00000230: 6672 6f6d 202e 2e20 696d 706f 7274 2068  from .. import h
-00000240: 656c 7065 7273 0a0a 0a40 7079 7465 7374  elpers...@pytest
-00000250: 2e66 6978 7475 7265 0a64 6566 2063 7266  .fixture.def crf
-00000260: 286e 756d 5f74 6167 733a 2069 6e74 2920  (num_tags: int) 
-00000270: 2d3e 2043 5246 3a0a 2020 2020 7265 7475  -> CRF:.    retu
-00000280: 726e 2043 5246 286e 756d 5f74 6167 7329  rn CRF(num_tags)
-00000290: 2e65 7661 6c28 290a 0a0a 6465 6620 7465  .eval()...def te
-000002a0: 7374 5f6c 6f67 5f70 6f74 656e 7469 616c  st_log_potential
-000002b0: 735f 6265 6861 7665 735f 6173 5f70 726f  s_behaves_as_pro
-000002c0: 6261 6269 6c69 7479 2863 7266 3a20 4352  bability(crf: CR
-000002d0: 462c 206e 756d 5f74 6167 733a 2069 6e74  F, num_tags: int
-000002e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2062  ) -> None:.    b
-000002f0: 6174 6368 5f73 697a 6520 3d20 3132 0a20  atch_size = 12. 
-00000300: 2020 2073 6571 7565 6e63 655f 6c65 6e67     sequence_leng
-00000310: 7468 203d 2033 0a20 2020 206c 6f67 6974  th = 3.    logit
-00000320: 7320 3d20 746f 7263 682e 7261 6e64 6e28  s = torch.randn(
-00000330: 6261 7463 685f 7369 7a65 2c20 7365 7175  batch_size, sequ
-00000340: 656e 6365 5f6c 656e 6774 682c 206e 756d  ence_length, num
-00000350: 5f74 6167 7329 0a0a 2020 2020 7769 7468  _tags)..    with
-00000360: 2074 6f72 6368 2e6e 6f5f 6772 6164 2829   torch.no_grad()
-00000370: 3a0a 2020 2020 2020 2020 6c6f 675f 706f  :.        log_po
-00000380: 7465 6e74 6961 6c73 203d 2063 7266 286c  tentials = crf(l
-00000390: 6f67 6974 7329 0a0a 2020 2020 6173 7365  ogits)..    asse
-000003a0: 7274 2068 656c 7065 7273 2e63 6865 636b  rt helpers.check
-000003b0: 5f6c 6f67 5f70 6f74 656e 7469 616c 735f  _log_potentials_
-000003c0: 6265 6861 7665 735f 6173 5f70 726f 6261  behaves_as_proba
-000003d0: 6269 6c69 7479 286c 6f67 5f70 6f74 656e  bility(log_poten
-000003e0: 7469 616c 7329 0a0a 0a64 6566 2074 6573  tials)...def tes
-000003f0: 745f 6372 665f 6d61 736b 735f 6c6f 675f  t_crf_masks_log_
-00000400: 706f 7465 6e74 6961 6c73 2863 7266 3a20  potentials(crf: 
-00000410: 4352 462c 206e 756d 5f74 6167 733a 2069  CRF, num_tags: i
-00000420: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00000430: 2062 6174 6368 5f73 697a 6520 3d20 330a   batch_size = 3.
-00000440: 2020 2020 7365 7175 656e 6365 5f6c 656e      sequence_len
-00000450: 6774 6820 3d20 3230 0a20 2020 206c 6f67  gth = 20.    log
-00000460: 6974 7320 3d20 746f 7263 682e 7261 6e64  its = torch.rand
-00000470: 6e28 6261 7463 685f 7369 7a65 2c20 7365  n(batch_size, se
-00000480: 7175 656e 6365 5f6c 656e 6774 682c 206e  quence_length, n
-00000490: 756d 5f74 6167 7329 0a20 2020 206d 6173  um_tags).    mas
-000004a0: 6b20 3d20 746f 7263 682e 7465 6e73 6f72  k = torch.tensor
-000004b0: 285b 5b54 7275 655d 202a 2032 302c 205b  ([[True] * 20, [
-000004c0: 5472 7565 5d20 2a20 3130 202b 205b 4661  True] * 10 + [Fa
-000004d0: 6c73 655d 202a 2031 302c 205b 4661 6c73  lse] * 10, [Fals
-000004e0: 655d 202a 2032 305d 290a 0a20 2020 2077  e] * 20])..    w
-000004f0: 6974 6820 746f 7263 682e 6e6f 5f67 7261  ith torch.no_gra
-00000500: 6428 293a 0a20 2020 2020 2020 206c 6f67  d():.        log
-00000510: 5f70 6f74 656e 7469 616c 7320 3d20 6372  _potentials = cr
-00000520: 6628 6c6f 6769 7473 2c20 6d61 736b 290a  f(logits, mask).
-00000530: 0a20 2020 2061 7373 6572 7420 6865 6c70  .    assert help
-00000540: 6572 732e 6368 6563 6b5f 6c6f 675f 706f  ers.check_log_po
-00000550: 7465 6e74 6961 6c73 5f6d 6173 6b65 645f  tentials_masked_
-00000560: 636f 7272 6563 746c 7928 6c6f 675f 706f  correctly(log_po
-00000570: 7465 6e74 6961 6c73 2c20 6d61 736b 290a  tentials, mask).
+00000000: 696d 706f 7274 2070 7974 6573 740a 696d  import pytest.im
+00000010: 706f 7274 2074 6f72 6368 0a66 726f 6d20  port torch.from 
+00000020: 7061 7274 6961 6c5f 7461 6767 6572 2e63  partial_tagger.c
+00000030: 7266 2e6e 6e20 696d 706f 7274 2043 5246  rf.nn import CRF
+00000040: 0a0a 6672 6f6d 202e 2e20 696d 706f 7274  ..from .. import
+00000050: 2068 656c 7065 7273 0a0a 0a40 7079 7465   helpers...@pyte
+00000060: 7374 2e66 6978 7475 7265 0a64 6566 2063  st.fixture.def c
+00000070: 7266 286e 756d 5f74 6167 733a 2069 6e74  rf(num_tags: int
+00000080: 2920 2d3e 2043 5246 3a0a 2020 2020 7265  ) -> CRF:.    re
+00000090: 7475 726e 2043 5246 286e 756d 5f74 6167  turn CRF(num_tag
+000000a0: 7329 2e65 7661 6c28 290a 0a0a 6465 6620  s).eval()...def 
+000000b0: 7465 7374 5f6c 6f67 5f70 6f74 656e 7469  test_log_potenti
+000000c0: 616c 735f 6265 6861 7665 735f 6173 5f70  als_behaves_as_p
+000000d0: 726f 6261 6269 6c69 7479 2863 7266 3a20  robability(crf: 
+000000e0: 4352 462c 206e 756d 5f74 6167 733a 2069  CRF, num_tags: i
+000000f0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00000100: 2062 6174 6368 5f73 697a 6520 3d20 3132   batch_size = 12
+00000110: 0a20 2020 2073 6571 7565 6e63 655f 6c65  .    sequence_le
+00000120: 6e67 7468 203d 2033 0a20 2020 206c 6f67  ngth = 3.    log
+00000130: 6974 7320 3d20 746f 7263 682e 7261 6e64  its = torch.rand
+00000140: 6e28 6261 7463 685f 7369 7a65 2c20 7365  n(batch_size, se
+00000150: 7175 656e 6365 5f6c 656e 6774 682c 206e  quence_length, n
+00000160: 756d 5f74 6167 7329 0a0a 2020 2020 7769  um_tags)..    wi
+00000170: 7468 2074 6f72 6368 2e6e 6f5f 6772 6164  th torch.no_grad
+00000180: 2829 3a0a 2020 2020 2020 2020 6c6f 675f  ():.        log_
+00000190: 706f 7465 6e74 6961 6c73 203d 2063 7266  potentials = crf
+000001a0: 286c 6f67 6974 7329 0a0a 2020 2020 6173  (logits)..    as
+000001b0: 7365 7274 2068 656c 7065 7273 2e63 6865  sert helpers.che
+000001c0: 636b 5f6c 6f67 5f70 6f74 656e 7469 616c  ck_log_potential
+000001d0: 735f 6265 6861 7665 735f 6173 5f70 726f  s_behaves_as_pro
+000001e0: 6261 6269 6c69 7479 286c 6f67 5f70 6f74  bability(log_pot
+000001f0: 656e 7469 616c 7329 0a0a 0a64 6566 2074  entials)...def t
+00000200: 6573 745f 6372 665f 6d61 736b 735f 6c6f  est_crf_masks_lo
+00000210: 675f 706f 7465 6e74 6961 6c73 2863 7266  g_potentials(crf
+00000220: 3a20 4352 462c 206e 756d 5f74 6167 733a  : CRF, num_tags:
+00000230: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00000240: 2020 2062 6174 6368 5f73 697a 6520 3d20     batch_size = 
+00000250: 330a 2020 2020 7365 7175 656e 6365 5f6c  3.    sequence_l
+00000260: 656e 6774 6820 3d20 3230 0a20 2020 206c  ength = 20.    l
+00000270: 6f67 6974 7320 3d20 746f 7263 682e 7261  ogits = torch.ra
+00000280: 6e64 6e28 6261 7463 685f 7369 7a65 2c20  ndn(batch_size, 
+00000290: 7365 7175 656e 6365 5f6c 656e 6774 682c  sequence_length,
+000002a0: 206e 756d 5f74 6167 7329 0a20 2020 206d   num_tags).    m
+000002b0: 6173 6b20 3d20 746f 7263 682e 7465 6e73  ask = torch.tens
+000002c0: 6f72 285b 5b54 7275 655d 202a 2032 302c  or([[True] * 20,
+000002d0: 205b 5472 7565 5d20 2a20 3130 202b 205b   [True] * 10 + [
+000002e0: 4661 6c73 655d 202a 2031 302c 205b 4661  False] * 10, [Fa
+000002f0: 6c73 655d 202a 2032 305d 290a 0a20 2020  lse] * 20])..   
+00000300: 2077 6974 6820 746f 7263 682e 6e6f 5f67   with torch.no_g
+00000310: 7261 6428 293a 0a20 2020 2020 2020 206c  rad():.        l
+00000320: 6f67 5f70 6f74 656e 7469 616c 7320 3d20  og_potentials = 
+00000330: 6372 6628 6c6f 6769 7473 2c20 6d61 736b  crf(logits, mask
+00000340: 290a 0a20 2020 2061 7373 6572 7420 6865  )..    assert he
+00000350: 6c70 6572 732e 6368 6563 6b5f 6c6f 675f  lpers.check_log_
+00000360: 706f 7465 6e74 6961 6c73 5f6d 6173 6b65  potentials_maske
+00000370: 645f 636f 7272 6563 746c 7928 6c6f 675f  d_correctly(log_
+00000380: 706f 7465 6e74 6961 6c73 2c20 6d61 736b  potentials, mask
+00000390: 290a                                     ).
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/2301591c3c47b639` & `pytorch_partial_tagger-0.1.2/tests/data/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,384 +1,351 @@
-00000000: 0100 0000 0000 0000 1400 0000 0000 0000  ................
-00000010: 7465 7374 732e 6461 7461 2e74 6573 745f  tests.data.test_
-00000020: 636f 7265 0400 0000 0000 0000 0600 0000  core............
-00000030: 0000 0000 7079 7465 7374 0000 0000 0d00  ....pytest......
-00000040: 0000 1c00 0000 0000 0000 7061 7274 6961  ..........partia
-00000050: 6c5f 7461 6767 6572 2e64 6174 612e 4c61  l_tagger.data.La
-00000060: 6265 6c53 6574 2f00 0000 3700 0000 1800  belSet/...7.....
-00000070: 0000 0000 0000 7061 7274 6961 6c5f 7461  ......partial_ta
-00000080: 6767 6572 2e64 6174 612e 5370 616e 3900  gger.data.Span9.
-00000090: 0000 3d00 0000 2100 0000 0000 0000 7061  ..=...!.......pa
-000000a0: 7274 6961 6c5f 7461 6767 6572 2e64 6174  rtial_tagger.dat
-000000b0: 612e 546f 6b65 6e69 7a65 6454 6578 743f  a.TokenizedText?
-000000c0: 0000 004c 0000 0001 0000 0000 0000 000f  ...L............
-000000d0: 0000 0000 0000 0055 6e73 6f72 7465 6449  .......UnsortedI
-000000e0: 6d70 6f72 7473 2900 0000 0000 0000 496d  mports).......Im
-000000f0: 706f 7274 2062 6c6f 636b 2069 7320 756e  port block is un
-00000100: 2d73 6f72 7465 6420 6f72 2075 6e2d 666f  -sorted or un-fo
-00000110: 726d 6174 7465 6401 1000 0000 0000 0000  rmatted.........
-00000120: 4f72 6761 6e69 7a65 2069 6d70 6f72 7473  Organize imports
-00000130: 0000 0000 4f00 0000 0101 0000 0000 0000  ....O...........
-00000140: 0000 0000 004f 0000 0001 4e00 0000 0000  .....O....N.....
-00000150: 0000 696d 706f 7274 2070 7974 6573 740a  ..import pytest.
-00000160: 6672 6f6d 2070 6172 7469 616c 5f74 6167  from partial_tag
-00000170: 6765 722e 6461 7461 2069 6d70 6f72 7420  ger.data import 
-00000180: 4c61 6265 6c53 6574 2c20 5370 616e 2c20  LabelSet, Span, 
-00000190: 546f 6b65 6e69 7a65 6454 6578 740a 0a0a  TokenizedText...
-000001a0: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0100 0000 0000 0000 4800 0000 0000 0000  ........H.......
-000001c0: 2f55 7365 7273 2f79 6173 7566 756d 692f  /Users/yasufumi/
-000001d0: 576f 726b 7370 6163 652f 7079 746f 7263  Workspace/pytorc
-000001e0: 682d 7061 7274 6961 6c2d 7461 6767 6572  h-partial-tagger
-000001f0: 2f74 6573 7473 2f64 6174 612f 7465 7374  /tests/data/test
-00000200: 5f63 6f72 652e 7079 e615 0000 0000 0000  _core.py........
-00000210: 696d 706f 7274 2070 7974 6573 740a 0a66  import pytest..f
-00000220: 726f 6d20 7061 7274 6961 6c5f 7461 6767  rom partial_tagg
-00000230: 6572 2e64 6174 6120 696d 706f 7274 204c  er.data import L
-00000240: 6162 656c 5365 742c 2053 7061 6e2c 2054  abelSet, Span, T
-00000250: 6f6b 656e 697a 6564 5465 7874 0a0a 0a40  okenizedText...@
-00000260: 7079 7465 7374 2e66 6978 7475 7265 0a64  pytest.fixture.d
-00000270: 6566 2074 6f6b 656e 697a 6564 5f74 6578  ef tokenized_tex
-00000280: 7428 2920 2d3e 2054 6f6b 656e 697a 6564  t() -> Tokenized
-00000290: 5465 7874 3a0a 2020 2020 2320 546f 6b65  Text:.    # Toke
-000002a0: 6e69 7a65 6420 6279 2052 6f42 4552 5461  nized by RoBERTa
-000002b0: 0a20 2020 2072 6574 7572 6e20 546f 6b65  .    return Toke
-000002c0: 6e69 7a65 6454 6578 7428 0a20 2020 2020  nizedText(.     
-000002d0: 2020 2022 546f 6b79 6f20 6973 2074 6865     "Tokyo is the
-000002e0: 2063 6170 6974 616c 206f 6620 4a61 7061   capital of Japa
-000002f0: 6e2e 222c 0a20 2020 2020 2020 2028 0a20  n.",.        (. 
-00000300: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
-00000310: 0a20 2020 2020 2020 2020 2020 2053 7061  .            Spa
-00000320: 6e28 302c 2033 292c 0a20 2020 2020 2020  n(0, 3),.       
-00000330: 2020 2020 2053 7061 6e28 332c 2032 292c       Span(3, 2),
-00000340: 0a20 2020 2020 2020 2020 2020 2053 7061  .            Spa
-00000350: 6e28 362c 2032 292c 0a20 2020 2020 2020  n(6, 2),.       
-00000360: 2020 2020 2053 7061 6e28 392c 2033 292c       Span(9, 3),
-00000370: 0a20 2020 2020 2020 2020 2020 2053 7061  .            Spa
-00000380: 6e28 3133 2c20 3729 2c0a 2020 2020 2020  n(13, 7),.      
-00000390: 2020 2020 2020 5370 616e 2832 312c 2032        Span(21, 2
-000003a0: 292c 0a20 2020 2020 2020 2020 2020 2053  ),.            S
-000003b0: 7061 6e28 3234 2c20 3529 2c0a 2020 2020  pan(24, 5),.    
-000003c0: 2020 2020 2020 2020 5370 616e 2832 392c          Span(29,
-000003d0: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
-000003e0: 204e 6f6e 652c 0a20 2020 2020 2020 2029   None,.        )
-000003f0: 2c0a 2020 2020 2020 2020 280a 2020 2020  ,.        (.    
-00000400: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
-00000410: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00000420: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
-00000430: 2020 2020 2032 2c0a 2020 2020 2020 2020       2,.        
-00000440: 2020 2020 322c 0a20 2020 2020 2020 2020      2,.         
-00000450: 2020 202d 312c 0a20 2020 2020 2020 2020     -1,.         
-00000460: 2020 2033 2c0a 2020 2020 2020 2020 2020     3,.          
-00000470: 2020 332c 0a20 2020 2020 2020 2020 2020    3,.           
-00000480: 202d 312c 0a20 2020 2020 2020 2020 2020   -1,.           
-00000490: 2034 2c0a 2020 2020 2020 2020 2020 2020   4,.            
-000004a0: 342c 0a20 2020 2020 2020 2020 2020 2034  4,.            4
-000004b0: 2c0a 2020 2020 2020 2020 2020 2020 2d31  ,.            -1
-000004c0: 2c0a 2020 2020 2020 2020 2020 2020 352c  ,.            5,
-000004d0: 0a20 2020 2020 2020 2020 2020 2035 2c0a  .            5,.
-000004e0: 2020 2020 2020 2020 2020 2020 352c 0a20              5,. 
-000004f0: 2020 2020 2020 2020 2020 2035 2c0a 2020             5,.  
-00000500: 2020 2020 2020 2020 2020 352c 0a20 2020            5,.   
-00000510: 2020 2020 2020 2020 2035 2c0a 2020 2020           5,.    
-00000520: 2020 2020 2020 2020 352c 0a20 2020 2020          5,.     
-00000530: 2020 2020 2020 202d 312c 0a20 2020 2020         -1,.     
-00000540: 2020 2020 2020 2036 2c0a 2020 2020 2020         6,.      
-00000550: 2020 2020 2020 362c 0a20 2020 2020 2020        6,.       
-00000560: 2020 2020 202d 312c 0a20 2020 2020 2020       -1,.       
-00000570: 2020 2020 2037 2c0a 2020 2020 2020 2020       7,.        
-00000580: 2020 2020 372c 0a20 2020 2020 2020 2020      7,.         
-00000590: 2020 2037 2c0a 2020 2020 2020 2020 2020     7,.          
-000005a0: 2020 372c 0a20 2020 2020 2020 2020 2020    7,.           
-000005b0: 2037 2c0a 2020 2020 2020 2020 2020 2020   7,.            
-000005c0: 382c 0a20 2020 2020 2020 2029 2c0a 2020  8,.        ),.  
-000005d0: 2020 290a 0a0a 4070 7974 6573 742e 6669    )...@pytest.fi
-000005e0: 7874 7572 650a 6465 6620 6c61 6265 6c5f  xture.def label_
-000005f0: 7365 7428 2920 2d3e 204c 6162 656c 5365  set() -> LabelSe
-00000600: 743a 0a20 2020 2072 6574 7572 6e20 4c61  t:.    return La
-00000610: 6265 6c53 6574 287b 224f 5247 222c 2022  belSet({"ORG", "
-00000620: 5045 5222 7d29 0a0a 0a64 6566 2074 6573  PER"})...def tes
-00000630: 745f 746f 6b65 6e73 5f61 7265 5f76 616c  t_tokens_are_val
-00000640: 6964 2874 6f6b 656e 697a 6564 5f74 6578  id(tokenized_tex
-00000650: 743a 2054 6f6b 656e 697a 6564 5465 7874  t: TokenizedText
-00000660: 2920 2d3e 204e 6f6e 653a 0a20 2020 2074  ) -> None:.    t
-00000670: 6f6b 656e 5f69 6e64 6963 6573 203d 205b  oken_indices = [
-00000680: 312c 2032 2c20 332c 2034 2c20 352c 2036  1, 2, 3, 4, 5, 6
-00000690: 2c20 372c 2038 5d0a 2020 2020 6578 7065  , 7, 8].    expe
-000006a0: 6374 6564 203d 205b 2254 6f6b 222c 2022  cted = ["Tok", "
-000006b0: 796f 222c 2022 6973 222c 2022 7468 6522  yo", "is", "the"
-000006c0: 2c20 2263 6170 6974 616c 222c 2022 6f66  , "capital", "of
-000006d0: 222c 2022 4a61 7061 6e22 2c20 222e 225d  ", "Japan", "."]
-000006e0: 0a0a 2020 2020 746f 6b65 6e73 203d 205b  ..    tokens = [
-000006f0: 5d0a 2020 2020 666f 7220 746f 6b65 6e5f  ].    for token_
-00000700: 696e 6465 7820 696e 2074 6f6b 656e 5f69  index in token_i
-00000710: 6e64 6963 6573 3a0a 2020 2020 2020 2020  ndices:.        
-00000720: 746f 6b65 6e73 2e61 7070 656e 6428 746f  tokens.append(to
-00000730: 6b65 6e69 7a65 645f 7465 7874 2e67 6574  kenized_text.get
-00000740: 5f74 6f6b 656e 2874 6f6b 656e 5f69 6e64  _token(token_ind
-00000750: 6578 2929 0a0a 2020 2020 6173 7365 7274  ex))..    assert
-00000760: 2074 6f6b 656e 7320 3d3d 2065 7870 6563   tokens == expec
-00000770: 7465 640a 0a0a 6465 6620 7465 7374 5f63  ted...def test_c
-00000780: 6f6e 7665 7274 735f 746f 6b65 6e5f 7370  onverts_token_sp
-00000790: 616e 5f74 6f5f 6368 6172 5f73 7061 6e28  an_to_char_span(
-000007a0: 746f 6b65 6e69 7a65 645f 7465 7874 3a20  tokenized_text: 
-000007b0: 546f 6b65 6e69 7a65 6454 6578 7429 202d  TokenizedText) -
-000007c0: 3e20 4e6f 6e65 3a0a 2020 2020 746f 6b65  > None:.    toke
-000007d0: 6e5f 7370 616e 7320 3d20 5b0a 2020 2020  n_spans = [.    
-000007e0: 2020 2020 5370 616e 2831 2c20 3229 2c20      Span(1, 2), 
-000007f0: 2023 2054 6f6b 2079 6f0a 2020 2020 2020   # Tok yo.      
-00000800: 2020 5370 616e 2833 2c20 3129 2c20 2023    Span(3, 1),  #
-00000810: 2069 730a 2020 2020 2020 2020 5370 616e   is.        Span
-00000820: 2834 2c20 3129 2c20 2023 2074 6865 0a20  (4, 1),  # the. 
-00000830: 2020 2020 2020 2053 7061 6e28 352c 2031         Span(5, 1
-00000840: 292c 2020 2320 6361 7069 7461 6c0a 2020  ),  # capital.  
-00000850: 2020 2020 2020 5370 616e 2836 2c20 3129        Span(6, 1)
-00000860: 2c20 2023 206f 660a 2020 2020 2020 2020  ,  # of.        
-00000870: 5370 616e 2837 2c20 3129 2c20 2023 204a  Span(7, 1),  # J
-00000880: 6170 616e 0a20 2020 2020 2020 2053 7061  apan.        Spa
-00000890: 6e28 382c 2031 292c 2020 2320 2e0a 2020  n(8, 1),  # ..  
-000008a0: 2020 5d0a 2020 2020 6578 7065 6374 6564    ].    expected
-000008b0: 203d 205b 0a20 2020 2020 2020 2053 7061   = [.        Spa
-000008c0: 6e28 302c 2035 292c 2020 2320 546f 6b79  n(0, 5),  # Toky
-000008d0: 6f0a 2020 2020 2020 2020 5370 616e 2836  o.        Span(6
-000008e0: 2c20 3229 2c20 2023 2069 730a 2020 2020  , 2),  # is.    
-000008f0: 2020 2020 5370 616e 2839 2c20 3329 2c20      Span(9, 3), 
-00000900: 2023 2074 6865 0a20 2020 2020 2020 2053   # the.        S
-00000910: 7061 6e28 3133 2c20 3729 2c20 2023 2063  pan(13, 7),  # c
-00000920: 6170 6974 616c 0a20 2020 2020 2020 2053  apital.        S
-00000930: 7061 6e28 3231 2c20 3229 2c20 2023 206f  pan(21, 2),  # o
-00000940: 660a 2020 2020 2020 2020 5370 616e 2832  f.        Span(2
-00000950: 342c 2035 292c 2020 2320 4a61 7061 6e0a  4, 5),  # Japan.
-00000960: 2020 2020 2020 2020 5370 616e 2832 392c          Span(29,
-00000970: 2031 292c 2020 2320 2e0a 2020 2020 5d0a   1),  # ..    ].
-00000980: 0a20 2020 2063 6861 725f 7370 616e 7320  .    char_spans 
-00000990: 3d20 5b5d 0a20 2020 2066 6f72 2074 6f6b  = [].    for tok
-000009a0: 656e 5f73 7061 6e20 696e 2074 6f6b 656e  en_span in token
-000009b0: 5f73 7061 6e73 3a0a 2020 2020 2020 2020  _spans:.        
-000009c0: 6368 6172 5f73 7061 6e73 2e61 7070 656e  char_spans.appen
-000009d0: 6428 746f 6b65 6e69 7a65 645f 7465 7874  d(tokenized_text
-000009e0: 2e63 6f6e 7665 7274 5f74 6f5f 6368 6172  .convert_to_char
-000009f0: 5f73 7061 6e28 746f 6b65 6e5f 7370 616e  _span(token_span
-00000a00: 2929 0a0a 2020 2020 6173 7365 7274 2063  ))..    assert c
-00000a10: 6861 725f 7370 616e 7320 3d3d 2065 7870  har_spans == exp
-00000a20: 6563 7465 640a 0a0a 6465 6620 7465 7374  ected...def test
-00000a30: 5f6c 6162 656c 5f69 735f 7661 6c69 6428  _label_is_valid(
-00000a40: 6c61 6265 6c5f 7365 743a 204c 6162 656c  label_set: Label
-00000a50: 5365 7429 202d 3e20 4e6f 6e65 3a0a 2020  Set) -> None:.  
-00000a60: 2020 696e 6469 6365 7320 3d20 5b30 2c20    indices = [0, 
-00000a70: 312c 2032 2c20 332c 2034 2c20 352c 2036  1, 2, 3, 4, 5, 6
-00000a80: 2c20 372c 2038 5d0a 2020 2020 6578 7065  , 7, 8].    expe
-00000a90: 6374 6564 203d 205b 4e6f 6e65 5d20 2b20  cted = [None] + 
-00000aa0: 5b22 4f52 4722 5d20 2a20 3420 2b20 5b22  ["ORG"] * 4 + ["
-00000ab0: 5045 5222 5d20 2a20 340a 0a20 2020 206c  PER"] * 4..    l
-00000ac0: 6162 656c 7320 3d20 5b6c 6162 656c 5f73  abels = [label_s
-00000ad0: 6574 2e67 6574 5f6c 6162 656c 2869 6e64  et.get_label(ind
-00000ae0: 6578 2920 666f 7220 696e 6465 7820 696e  ex) for index in
-00000af0: 2069 6e64 6963 6573 5d0a 0a20 2020 2061   indices]..    a
-00000b00: 7373 6572 7420 6c61 6265 6c73 203d 3d20  ssert labels == 
-00000b10: 6578 7065 6374 6564 0a0a 0a64 6566 2074  expected...def t
-00000b20: 6573 745f 7374 6172 745f 7374 6174 6573  est_start_states
-00000b30: 5f61 7265 5f76 616c 6964 286c 6162 656c  _are_valid(label
-00000b40: 5f73 6574 3a20 4c61 6265 6c53 6574 2920  _set: LabelSet) 
-00000b50: 2d3e 204e 6f6e 653a 0a20 2020 2065 7870  -> None:.    exp
-00000b60: 6563 7465 6420 3d20 5b0a 2020 2020 2020  ected = [.      
-00000b70: 2020 5472 7565 2c20 2023 204f 0a20 2020    True,  # O.   
-00000b80: 2020 2020 2054 7275 652c 2020 2320 422d       True,  # B-
-00000b90: 4f52 470a 2020 2020 2020 2020 4661 6c73  ORG.        Fals
-00000ba0: 652c 2020 2320 492d 4f52 470a 2020 2020  e,  # I-ORG.    
-00000bb0: 2020 2020 4661 6c73 652c 2020 2320 4c2d      False,  # L-
-00000bc0: 4f52 470a 2020 2020 2020 2020 5472 7565  ORG.        True
-00000bd0: 2c20 2023 2055 2d4f 5247 0a20 2020 2020  ,  # U-ORG.     
-00000be0: 2020 2054 7275 652c 2020 2320 422d 5045     True,  # B-PE
-00000bf0: 520a 2020 2020 2020 2020 4661 6c73 652c  R.        False,
-00000c00: 2020 2320 492d 5045 520a 2020 2020 2020    # I-PER.      
-00000c10: 2020 4661 6c73 652c 2020 2320 4c2d 5045    False,  # L-PE
-00000c20: 520a 2020 2020 2020 2020 5472 7565 2c20  R.        True, 
-00000c30: 2023 2055 2d50 4552 0a20 2020 205d 0a0a   # U-PER.    ]..
-00000c40: 2020 2020 6173 7365 7274 206c 6162 656c      assert label
-00000c50: 5f73 6574 2e67 6574 5f73 7461 7274 5f73  _set.get_start_s
-00000c60: 7461 7465 7328 2920 3d3d 2065 7870 6563  tates() == expec
-00000c70: 7465 640a 0a0a 6465 6620 7465 7374 5f65  ted...def test_e
-00000c80: 6e64 5f73 7461 7465 735f 6172 655f 7661  nd_states_are_va
-00000c90: 6c69 6428 6c61 6265 6c5f 7365 743a 204c  lid(label_set: L
-00000ca0: 6162 656c 5365 7429 202d 3e20 4e6f 6e65  abelSet) -> None
-00000cb0: 3a0a 2020 2020 6578 7065 6374 6564 203d  :.    expected =
-00000cc0: 205b 0a20 2020 2020 2020 2054 7275 652c   [.        True,
-00000cd0: 2020 2320 4f0a 2020 2020 2020 2020 4661    # O.        Fa
-00000ce0: 6c73 652c 2020 2320 422d 4f52 470a 2020  lse,  # B-ORG.  
-00000cf0: 2020 2020 2020 4661 6c73 652c 2020 2320        False,  # 
-00000d00: 492d 4f52 470a 2020 2020 2020 2020 5472  I-ORG.        Tr
-00000d10: 7565 2c20 2023 204c 2d4f 5247 0a20 2020  ue,  # L-ORG.   
-00000d20: 2020 2020 2054 7275 652c 2020 2320 552d       True,  # U-
-00000d30: 4f52 470a 2020 2020 2020 2020 4661 6c73  ORG.        Fals
-00000d40: 652c 2020 2320 422d 5045 520a 2020 2020  e,  # B-PER.    
-00000d50: 2020 2020 4661 6c73 652c 2020 2320 492d      False,  # I-
-00000d60: 5045 520a 2020 2020 2020 2020 5472 7565  PER.        True
-00000d70: 2c20 2023 204c 2d50 4552 0a20 2020 2020  ,  # L-PER.     
-00000d80: 2020 2054 7275 652c 2020 2320 552d 5045     True,  # U-PE
-00000d90: 520a 2020 2020 5d0a 0a20 2020 2061 7373  R.    ]..    ass
-00000da0: 6572 7420 6c61 6265 6c5f 7365 742e 6765  ert label_set.ge
-00000db0: 745f 656e 645f 7374 6174 6573 2829 203d  t_end_states() =
-00000dc0: 3d20 6578 7065 6374 6564 0a0a 0a64 6566  = expected...def
-00000dd0: 2074 6573 745f 7472 616e 7369 7469 6f6e   test_transition
-00000de0: 735f 6172 655f 7661 6c69 6428 6c61 6265  s_are_valid(labe
-00000df0: 6c5f 7365 743a 204c 6162 656c 5365 7429  l_set: LabelSet)
-00000e00: 202d 3e20 4e6f 6e65 3a0a 2020 2020 6578   -> None:.    ex
-00000e10: 7065 6374 6564 203d 205b 0a20 2020 2020  pected = [.     
-00000e20: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00000e30: 2054 7275 652c 2020 2320 4f0a 2020 2020   True,  # O.    
-00000e40: 2020 2020 2020 2020 5472 7565 2c20 2023          True,  #
-00000e50: 2042 2d4f 5247 0a20 2020 2020 2020 2020   B-ORG.         
-00000e60: 2020 2046 616c 7365 2c20 2023 2049 2d4f     False,  # I-O
-00000e70: 5247 0a20 2020 2020 2020 2020 2020 2046  RG.            F
-00000e80: 616c 7365 2c20 2023 204c 2d4f 5247 0a20  alse,  # L-ORG. 
-00000e90: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-00000ea0: 2020 2320 552d 4f52 470a 2020 2020 2020    # U-ORG.      
-00000eb0: 2020 2020 2020 5472 7565 2c20 2023 2042        True,  # B
-00000ec0: 2d50 4552 0a20 2020 2020 2020 2020 2020  -PER.           
-00000ed0: 2046 616c 7365 2c20 2023 2049 2d50 4552   False,  # I-PER
-00000ee0: 0a20 2020 2020 2020 2020 2020 2046 616c  .            Fal
-00000ef0: 7365 2c20 2023 204c 2d50 4552 0a20 2020  se,  # L-PER.   
-00000f00: 2020 2020 2020 2020 2054 7275 652c 2020           True,  
-00000f10: 2320 552d 5045 520a 2020 2020 2020 2020  # U-PER.        
-00000f20: 5d2c 2020 2320 4f0a 2020 2020 2020 2020  ],  # O.        
-00000f30: 5b0a 2020 2020 2020 2020 2020 2020 4661  [.            Fa
-00000f40: 6c73 652c 2020 2320 4f0a 2020 2020 2020  lse,  # O.      
-00000f50: 2020 2020 2020 4661 6c73 652c 2020 2320        False,  # 
-00000f60: 422d 4f52 470a 2020 2020 2020 2020 2020  B-ORG.          
-00000f70: 2020 5472 7565 2c20 2023 2049 2d4f 5247    True,  # I-ORG
-00000f80: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
-00000f90: 652c 2020 2320 4c2d 4f52 470a 2020 2020  e,  # L-ORG.    
-00000fa0: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-00000fb0: 2320 552d 4f52 470a 2020 2020 2020 2020  # U-ORG.        
-00000fc0: 2020 2020 4661 6c73 652c 2020 2320 422d      False,  # B-
-00000fd0: 5045 520a 2020 2020 2020 2020 2020 2020  PER.            
-00000fe0: 4661 6c73 652c 2020 2320 492d 5045 520a  False,  # I-PER.
-00000ff0: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-00001000: 652c 2020 2320 4c2d 5045 520a 2020 2020  e,  # L-PER.    
-00001010: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-00001020: 2320 552d 5045 520a 2020 2020 2020 2020  # U-PER.        
-00001030: 5d2c 2020 2320 422d 4f52 470a 2020 2020  ],  # B-ORG.    
-00001040: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00001050: 2020 4661 6c73 652c 2020 2320 4f0a 2020    False,  # O.  
-00001060: 2020 2020 2020 2020 2020 4661 6c73 652c            False,
-00001070: 2020 2320 422d 4f52 470a 2020 2020 2020    # B-ORG.      
-00001080: 2020 2020 2020 5472 7565 2c20 2023 2049        True,  # I
-00001090: 2d4f 5247 0a20 2020 2020 2020 2020 2020  -ORG.           
-000010a0: 2054 7275 652c 2020 2320 4c2d 4f52 470a   True,  # L-ORG.
-000010b0: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-000010c0: 652c 2020 2320 552d 4f52 470a 2020 2020  e,  # U-ORG.    
-000010d0: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-000010e0: 2320 422d 5045 520a 2020 2020 2020 2020  # B-PER.        
-000010f0: 2020 2020 4661 6c73 652c 2020 2320 492d      False,  # I-
-00001100: 5045 520a 2020 2020 2020 2020 2020 2020  PER.            
-00001110: 4661 6c73 652c 2020 2320 4c2d 5045 520a  False,  # L-PER.
-00001120: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-00001130: 652c 2020 2320 552d 5045 520a 2020 2020  e,  # U-PER.    
-00001140: 2020 2020 5d2c 2020 2320 492d 4f52 470a      ],  # I-ORG.
-00001150: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00001160: 2020 2020 2020 5472 7565 2c20 2023 204f        True,  # O
-00001170: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
-00001180: 652c 2020 2320 422d 4f52 470a 2020 2020  e,  # B-ORG.    
-00001190: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-000011a0: 2320 492d 4f52 470a 2020 2020 2020 2020  # I-ORG.        
-000011b0: 2020 2020 4661 6c73 652c 2020 2320 4c2d      False,  # L-
-000011c0: 4f52 470a 2020 2020 2020 2020 2020 2020  ORG.            
-000011d0: 5472 7565 2c20 2023 2055 2d4f 5247 0a20  True,  # U-ORG. 
-000011e0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-000011f0: 2020 2320 422d 5045 520a 2020 2020 2020    # B-PER.      
-00001200: 2020 2020 2020 4661 6c73 652c 2020 2320        False,  # 
-00001210: 492d 5045 520a 2020 2020 2020 2020 2020  I-PER.          
-00001220: 2020 4661 6c73 652c 2020 2320 4c2d 5045    False,  # L-PE
-00001230: 520a 2020 2020 2020 2020 2020 2020 5472  R.            Tr
-00001240: 7565 2c20 2023 2055 2d50 4552 0a20 2020  ue,  # U-PER.   
-00001250: 2020 2020 205d 2c20 2023 204c 2d4f 5247       ],  # L-ORG
-00001260: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-00001270: 2020 2020 2020 2054 7275 652c 2020 2320         True,  # 
-00001280: 4f0a 2020 2020 2020 2020 2020 2020 5472  O.            Tr
-00001290: 7565 2c20 2023 2042 2d4f 5247 0a20 2020  ue,  # B-ORG.   
-000012a0: 2020 2020 2020 2020 2046 616c 7365 2c20           False, 
-000012b0: 2023 2049 2d4f 5247 0a20 2020 2020 2020   # I-ORG.       
-000012c0: 2020 2020 2046 616c 7365 2c20 2023 204c       False,  # L
-000012d0: 2d4f 5247 0a20 2020 2020 2020 2020 2020  -ORG.           
-000012e0: 2054 7275 652c 2020 2320 552d 4f52 470a   True,  # U-ORG.
-000012f0: 2020 2020 2020 2020 2020 2020 5472 7565              True
-00001300: 2c20 2023 2042 2d50 4552 0a20 2020 2020  ,  # B-PER.     
-00001310: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
-00001320: 2049 2d50 4552 0a20 2020 2020 2020 2020   I-PER.         
-00001330: 2020 2046 616c 7365 2c20 2023 204c 2d50     False,  # L-P
-00001340: 4552 0a20 2020 2020 2020 2020 2020 2054  ER.            T
-00001350: 7275 652c 2020 2320 552d 5045 520a 2020  rue,  # U-PER.  
-00001360: 2020 2020 2020 5d2c 2020 2320 552d 4f52        ],  # U-OR
-00001370: 470a 2020 2020 2020 2020 5b0a 2020 2020  G.        [.    
-00001380: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-00001390: 2320 4f0a 2020 2020 2020 2020 2020 2020  # O.            
-000013a0: 4661 6c73 652c 2020 2320 422d 4f52 470a  False,  # B-ORG.
-000013b0: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-000013c0: 652c 2020 2320 492d 4f52 470a 2020 2020  e,  # I-ORG.    
-000013d0: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-000013e0: 2320 4c2d 4f52 470a 2020 2020 2020 2020  # L-ORG.        
-000013f0: 2020 2020 4661 6c73 652c 2020 2320 552d      False,  # U-
-00001400: 4f52 470a 2020 2020 2020 2020 2020 2020  ORG.            
-00001410: 4661 6c73 652c 2020 2320 422d 5045 520a  False,  # B-PER.
-00001420: 2020 2020 2020 2020 2020 2020 5472 7565              True
-00001430: 2c20 2023 2049 2d50 4552 0a20 2020 2020  ,  # I-PER.     
-00001440: 2020 2020 2020 2054 7275 652c 2020 2320         True,  # 
-00001450: 4c2d 5045 520a 2020 2020 2020 2020 2020  L-PER.          
-00001460: 2020 4661 6c73 652c 2020 2320 552d 5045    False,  # U-PE
-00001470: 520a 2020 2020 2020 2020 5d2c 2020 2320  R.        ],  # 
-00001480: 422d 5045 520a 2020 2020 2020 2020 5b0a  B-PER.        [.
-00001490: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-000014a0: 652c 2020 2320 4f0a 2020 2020 2020 2020  e,  # O.        
-000014b0: 2020 2020 4661 6c73 652c 2020 2320 422d      False,  # B-
-000014c0: 4f52 470a 2020 2020 2020 2020 2020 2020  ORG.            
-000014d0: 4661 6c73 652c 2020 2320 492d 4f52 470a  False,  # I-ORG.
-000014e0: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-000014f0: 652c 2020 2320 4c2d 4f52 470a 2020 2020  e,  # L-ORG.    
-00001500: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
-00001510: 2320 552d 4f52 470a 2020 2020 2020 2020  # U-ORG.        
-00001520: 2020 2020 4661 6c73 652c 2020 2320 422d      False,  # B-
-00001530: 5045 520a 2020 2020 2020 2020 2020 2020  PER.            
-00001540: 5472 7565 2c20 2023 2049 2d50 4552 0a20  True,  # I-PER. 
-00001550: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-00001560: 2020 2320 4c2d 5045 520a 2020 2020 2020    # L-PER.      
-00001570: 2020 2020 2020 4661 6c73 652c 2020 2320        False,  # 
-00001580: 552d 5045 520a 2020 2020 2020 2020 5d2c  U-PER.        ],
-00001590: 2020 2320 492d 5045 520a 2020 2020 2020    # I-PER.      
-000015a0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000015b0: 5472 7565 2c20 2023 204f 0a20 2020 2020  True,  # O.     
-000015c0: 2020 2020 2020 2054 7275 652c 2020 2320         True,  # 
-000015d0: 422d 4f52 470a 2020 2020 2020 2020 2020  B-ORG.          
-000015e0: 2020 4661 6c73 652c 2020 2320 492d 4f52    False,  # I-OR
-000015f0: 470a 2020 2020 2020 2020 2020 2020 4661  G.            Fa
-00001600: 6c73 652c 2020 2320 4c2d 4f52 470a 2020  lse,  # L-ORG.  
-00001610: 2020 2020 2020 2020 2020 5472 7565 2c20            True, 
-00001620: 2023 2055 2d4f 5247 0a20 2020 2020 2020   # U-ORG.       
-00001630: 2020 2020 2054 7275 652c 2020 2320 422d       True,  # B-
-00001640: 5045 520a 2020 2020 2020 2020 2020 2020  PER.            
-00001650: 4661 6c73 652c 2020 2320 492d 5045 520a  False,  # I-PER.
-00001660: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-00001670: 652c 2020 2320 4c2d 5045 520a 2020 2020  e,  # L-PER.    
-00001680: 2020 2020 2020 2020 5472 7565 2c20 2023          True,  #
-00001690: 2055 2d50 4552 0a20 2020 2020 2020 205d   U-PER.        ]
-000016a0: 2c20 2023 204c 2d50 4552 0a20 2020 2020  ,  # L-PER.     
-000016b0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-000016c0: 2054 7275 652c 2020 2320 4f0a 2020 2020   True,  # O.    
-000016d0: 2020 2020 2020 2020 5472 7565 2c20 2023          True,  #
-000016e0: 2042 2d4f 5247 0a20 2020 2020 2020 2020   B-ORG.         
-000016f0: 2020 2046 616c 7365 2c20 2023 2049 2d4f     False,  # I-O
-00001700: 5247 0a20 2020 2020 2020 2020 2020 2046  RG.            F
-00001710: 616c 7365 2c20 2023 204c 2d4f 5247 0a20  alse,  # L-ORG. 
-00001720: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-00001730: 2020 2320 552d 4f52 470a 2020 2020 2020    # U-ORG.      
-00001740: 2020 2020 2020 5472 7565 2c20 2023 2042        True,  # B
-00001750: 2d50 4552 0a20 2020 2020 2020 2020 2020  -PER.           
-00001760: 2046 616c 7365 2c20 2023 2049 2d50 4552   False,  # I-PER
-00001770: 0a20 2020 2020 2020 2020 2020 2046 616c  .            Fal
-00001780: 7365 2c20 2023 204c 2d50 4552 0a20 2020  se,  # L-PER.   
-00001790: 2020 2020 2020 2020 2054 7275 652c 2020           True,  
-000017a0: 2320 552d 5045 520a 2020 2020 2020 2020  # U-PER.        
-000017b0: 5d2c 2020 2320 552d 5045 520a 2020 2020  ],  # U-PER.    
-000017c0: 5d0a 0a20 2020 2061 7373 6572 7420 6c61  ]..    assert la
-000017d0: 6265 6c5f 7365 742e 6765 745f 7472 616e  bel_set.get_tran
-000017e0: 7369 7469 6f6e 7328 2920 3d3d 2065 7870  sitions() == exp
-000017f0: 6563 7465 640a                           ected.
+00000000: 696d 706f 7274 2070 7974 6573 740a 6672  import pytest.fr
+00000010: 6f6d 2070 6172 7469 616c 5f74 6167 6765  om partial_tagge
+00000020: 722e 6461 7461 2069 6d70 6f72 7420 4c61  r.data import La
+00000030: 6265 6c53 6574 2c20 5370 616e 2c20 546f  belSet, Span, To
+00000040: 6b65 6e69 7a65 6454 6578 740a 0a0a 4070  kenizedText...@p
+00000050: 7974 6573 742e 6669 7874 7572 650a 6465  ytest.fixture.de
+00000060: 6620 746f 6b65 6e69 7a65 645f 7465 7874  f tokenized_text
+00000070: 2829 202d 3e20 546f 6b65 6e69 7a65 6454  () -> TokenizedT
+00000080: 6578 743a 0a20 2020 2023 2054 6f6b 656e  ext:.    # Token
+00000090: 697a 6564 2062 7920 526f 4245 5254 610a  ized by RoBERTa.
+000000a0: 2020 2020 7265 7475 726e 2054 6f6b 656e      return Token
+000000b0: 697a 6564 5465 7874 280a 2020 2020 2020  izedText(.      
+000000c0: 2020 2254 6f6b 796f 2069 7320 7468 6520    "Tokyo is the 
+000000d0: 6361 7069 7461 6c20 6f66 204a 6170 616e  capital of Japan
+000000e0: 2e22 2c0a 2020 2020 2020 2020 280a 2020  .",.        (.  
+000000f0: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
+00000100: 2020 2020 2020 2020 2020 2020 5370 616e              Span
+00000110: 2830 2c20 3329 2c0a 2020 2020 2020 2020  (0, 3),.        
+00000120: 2020 2020 5370 616e 2833 2c20 3229 2c0a      Span(3, 2),.
+00000130: 2020 2020 2020 2020 2020 2020 5370 616e              Span
+00000140: 2836 2c20 3229 2c0a 2020 2020 2020 2020  (6, 2),.        
+00000150: 2020 2020 5370 616e 2839 2c20 3329 2c0a      Span(9, 3),.
+00000160: 2020 2020 2020 2020 2020 2020 5370 616e              Span
+00000170: 2831 332c 2037 292c 0a20 2020 2020 2020  (13, 7),.       
+00000180: 2020 2020 2053 7061 6e28 3231 2c20 3229       Span(21, 2)
+00000190: 2c0a 2020 2020 2020 2020 2020 2020 5370  ,.            Sp
+000001a0: 616e 2832 342c 2035 292c 0a20 2020 2020  an(24, 5),.     
+000001b0: 2020 2020 2020 2053 7061 6e28 3239 2c20         Span(29, 
+000001c0: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
+000001d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 292c  None,.        ),
+000001e0: 0a20 2020 2020 2020 2028 0a20 2020 2020  .        (.     
+000001f0: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
+00000200: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+00000210: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
+00000220: 2020 2020 322c 0a20 2020 2020 2020 2020      2,.         
+00000230: 2020 2032 2c0a 2020 2020 2020 2020 2020     2,.          
+00000240: 2020 2d31 2c0a 2020 2020 2020 2020 2020    -1,.          
+00000250: 2020 332c 0a20 2020 2020 2020 2020 2020    3,.           
+00000260: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
+00000270: 2d31 2c0a 2020 2020 2020 2020 2020 2020  -1,.            
+00000280: 342c 0a20 2020 2020 2020 2020 2020 2034  4,.            4
+00000290: 2c0a 2020 2020 2020 2020 2020 2020 342c  ,.            4,
+000002a0: 0a20 2020 2020 2020 2020 2020 202d 312c  .            -1,
+000002b0: 0a20 2020 2020 2020 2020 2020 2035 2c0a  .            5,.
+000002c0: 2020 2020 2020 2020 2020 2020 352c 0a20              5,. 
+000002d0: 2020 2020 2020 2020 2020 2035 2c0a 2020             5,.  
+000002e0: 2020 2020 2020 2020 2020 352c 0a20 2020            5,.   
+000002f0: 2020 2020 2020 2020 2035 2c0a 2020 2020           5,.    
+00000300: 2020 2020 2020 2020 352c 0a20 2020 2020          5,.     
+00000310: 2020 2020 2020 2035 2c0a 2020 2020 2020         5,.      
+00000320: 2020 2020 2020 2d31 2c0a 2020 2020 2020        -1,.      
+00000330: 2020 2020 2020 362c 0a20 2020 2020 2020        6,.       
+00000340: 2020 2020 2036 2c0a 2020 2020 2020 2020       6,.        
+00000350: 2020 2020 2d31 2c0a 2020 2020 2020 2020      -1,.        
+00000360: 2020 2020 372c 0a20 2020 2020 2020 2020      7,.         
+00000370: 2020 2037 2c0a 2020 2020 2020 2020 2020     7,.          
+00000380: 2020 372c 0a20 2020 2020 2020 2020 2020    7,.           
+00000390: 2037 2c0a 2020 2020 2020 2020 2020 2020   7,.            
+000003a0: 372c 0a20 2020 2020 2020 2020 2020 2038  7,.            8
+000003b0: 2c0a 2020 2020 2020 2020 292c 0a20 2020  ,.        ),.   
+000003c0: 2029 0a0a 0a40 7079 7465 7374 2e66 6978   )...@pytest.fix
+000003d0: 7475 7265 0a64 6566 206c 6162 656c 5f73  ture.def label_s
+000003e0: 6574 2829 202d 3e20 4c61 6265 6c53 6574  et() -> LabelSet
+000003f0: 3a0a 2020 2020 7265 7475 726e 204c 6162  :.    return Lab
+00000400: 656c 5365 7428 7b22 4f52 4722 2c20 2250  elSet({"ORG", "P
+00000410: 4552 227d 290a 0a0a 6465 6620 7465 7374  ER"})...def test
+00000420: 5f74 6f6b 656e 735f 6172 655f 7661 6c69  _tokens_are_vali
+00000430: 6428 746f 6b65 6e69 7a65 645f 7465 7874  d(tokenized_text
+00000440: 3a20 546f 6b65 6e69 7a65 6454 6578 7429  : TokenizedText)
+00000450: 202d 3e20 4e6f 6e65 3a0a 2020 2020 746f   -> None:.    to
+00000460: 6b65 6e5f 696e 6469 6365 7320 3d20 5b31  ken_indices = [1
+00000470: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
+00000480: 2037 2c20 385d 0a20 2020 2065 7870 6563   7, 8].    expec
+00000490: 7465 6420 3d20 5b22 546f 6b22 2c20 2279  ted = ["Tok", "y
+000004a0: 6f22 2c20 2269 7322 2c20 2274 6865 222c  o", "is", "the",
+000004b0: 2022 6361 7069 7461 6c22 2c20 226f 6622   "capital", "of"
+000004c0: 2c20 224a 6170 616e 222c 2022 2e22 5d0a  , "Japan", "."].
+000004d0: 0a20 2020 2074 6f6b 656e 7320 3d20 5b5d  .    tokens = []
+000004e0: 0a20 2020 2066 6f72 2074 6f6b 656e 5f69  .    for token_i
+000004f0: 6e64 6578 2069 6e20 746f 6b65 6e5f 696e  ndex in token_in
+00000500: 6469 6365 733a 0a20 2020 2020 2020 2074  dices:.        t
+00000510: 6f6b 656e 732e 6170 7065 6e64 2874 6f6b  okens.append(tok
+00000520: 656e 697a 6564 5f74 6578 742e 6765 745f  enized_text.get_
+00000530: 746f 6b65 6e28 746f 6b65 6e5f 696e 6465  token(token_inde
+00000540: 7829 290a 0a20 2020 2061 7373 6572 7420  x))..    assert 
+00000550: 746f 6b65 6e73 203d 3d20 6578 7065 6374  tokens == expect
+00000560: 6564 0a0a 0a64 6566 2074 6573 745f 636f  ed...def test_co
+00000570: 6e76 6572 7473 5f74 6f6b 656e 5f73 7061  nverts_token_spa
+00000580: 6e5f 746f 5f63 6861 725f 7370 616e 2874  n_to_char_span(t
+00000590: 6f6b 656e 697a 6564 5f74 6578 743a 2054  okenized_text: T
+000005a0: 6f6b 656e 697a 6564 5465 7874 2920 2d3e  okenizedText) ->
+000005b0: 204e 6f6e 653a 0a20 2020 2074 6f6b 656e   None:.    token
+000005c0: 5f73 7061 6e73 203d 205b 0a20 2020 2020  _spans = [.     
+000005d0: 2020 2053 7061 6e28 312c 2032 292c 2020     Span(1, 2),  
+000005e0: 2320 546f 6b20 796f 0a20 2020 2020 2020  # Tok yo.       
+000005f0: 2053 7061 6e28 332c 2031 292c 2020 2320   Span(3, 1),  # 
+00000600: 6973 0a20 2020 2020 2020 2053 7061 6e28  is.        Span(
+00000610: 342c 2031 292c 2020 2320 7468 650a 2020  4, 1),  # the.  
+00000620: 2020 2020 2020 5370 616e 2835 2c20 3129        Span(5, 1)
+00000630: 2c20 2023 2063 6170 6974 616c 0a20 2020  ,  # capital.   
+00000640: 2020 2020 2053 7061 6e28 362c 2031 292c       Span(6, 1),
+00000650: 2020 2320 6f66 0a20 2020 2020 2020 2053    # of.        S
+00000660: 7061 6e28 372c 2031 292c 2020 2320 4a61  pan(7, 1),  # Ja
+00000670: 7061 6e0a 2020 2020 2020 2020 5370 616e  pan.        Span
+00000680: 2838 2c20 3129 2c20 2023 202e 0a20 2020  (8, 1),  # ..   
+00000690: 205d 0a20 2020 2065 7870 6563 7465 6420   ].    expected 
+000006a0: 3d20 5b0a 2020 2020 2020 2020 5370 616e  = [.        Span
+000006b0: 2830 2c20 3529 2c20 2023 2054 6f6b 796f  (0, 5),  # Tokyo
+000006c0: 0a20 2020 2020 2020 2053 7061 6e28 362c  .        Span(6,
+000006d0: 2032 292c 2020 2320 6973 0a20 2020 2020   2),  # is.     
+000006e0: 2020 2053 7061 6e28 392c 2033 292c 2020     Span(9, 3),  
+000006f0: 2320 7468 650a 2020 2020 2020 2020 5370  # the.        Sp
+00000700: 616e 2831 332c 2037 292c 2020 2320 6361  an(13, 7),  # ca
+00000710: 7069 7461 6c0a 2020 2020 2020 2020 5370  pital.        Sp
+00000720: 616e 2832 312c 2032 292c 2020 2320 6f66  an(21, 2),  # of
+00000730: 0a20 2020 2020 2020 2053 7061 6e28 3234  .        Span(24
+00000740: 2c20 3529 2c20 2023 204a 6170 616e 0a20  , 5),  # Japan. 
+00000750: 2020 2020 2020 2053 7061 6e28 3239 2c20         Span(29, 
+00000760: 3129 2c20 2023 202e 0a20 2020 205d 0a0a  1),  # ..    ]..
+00000770: 2020 2020 6368 6172 5f73 7061 6e73 203d      char_spans =
+00000780: 205b 5d0a 2020 2020 666f 7220 746f 6b65   [].    for toke
+00000790: 6e5f 7370 616e 2069 6e20 746f 6b65 6e5f  n_span in token_
+000007a0: 7370 616e 733a 0a20 2020 2020 2020 2063  spans:.        c
+000007b0: 6861 725f 7370 616e 732e 6170 7065 6e64  har_spans.append
+000007c0: 2874 6f6b 656e 697a 6564 5f74 6578 742e  (tokenized_text.
+000007d0: 636f 6e76 6572 745f 746f 5f63 6861 725f  convert_to_char_
+000007e0: 7370 616e 2874 6f6b 656e 5f73 7061 6e29  span(token_span)
+000007f0: 290a 0a20 2020 2061 7373 6572 7420 6368  )..    assert ch
+00000800: 6172 5f73 7061 6e73 203d 3d20 6578 7065  ar_spans == expe
+00000810: 6374 6564 0a0a 0a64 6566 2074 6573 745f  cted...def test_
+00000820: 6c61 6265 6c5f 6973 5f76 616c 6964 286c  label_is_valid(l
+00000830: 6162 656c 5f73 6574 3a20 4c61 6265 6c53  abel_set: LabelS
+00000840: 6574 2920 2d3e 204e 6f6e 653a 0a20 2020  et) -> None:.   
+00000850: 2069 6e64 6963 6573 203d 205b 302c 2031   indices = [0, 1
+00000860: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
+00000870: 2037 2c20 385d 0a20 2020 2065 7870 6563   7, 8].    expec
+00000880: 7465 6420 3d20 5b4e 6f6e 655d 202b 205b  ted = [None] + [
+00000890: 224f 5247 225d 202a 2034 202b 205b 2250  "ORG"] * 4 + ["P
+000008a0: 4552 225d 202a 2034 0a0a 2020 2020 6c61  ER"] * 4..    la
+000008b0: 6265 6c73 203d 205b 6c61 6265 6c5f 7365  bels = [label_se
+000008c0: 742e 6765 745f 6c61 6265 6c28 696e 6465  t.get_label(inde
+000008d0: 7829 2066 6f72 2069 6e64 6578 2069 6e20  x) for index in 
+000008e0: 696e 6469 6365 735d 0a0a 2020 2020 6173  indices]..    as
+000008f0: 7365 7274 206c 6162 656c 7320 3d3d 2065  sert labels == e
+00000900: 7870 6563 7465 640a 0a0a 6465 6620 7465  xpected...def te
+00000910: 7374 5f73 7461 7274 5f73 7461 7465 735f  st_start_states_
+00000920: 6172 655f 7661 6c69 6428 6c61 6265 6c5f  are_valid(label_
+00000930: 7365 743a 204c 6162 656c 5365 7429 202d  set: LabelSet) -
+00000940: 3e20 4e6f 6e65 3a0a 2020 2020 6578 7065  > None:.    expe
+00000950: 6374 6564 203d 205b 0a20 2020 2020 2020  cted = [.       
+00000960: 2054 7275 652c 2020 2320 4f0a 2020 2020   True,  # O.    
+00000970: 2020 2020 5472 7565 2c20 2023 2042 2d4f      True,  # B-O
+00000980: 5247 0a20 2020 2020 2020 2046 616c 7365  RG.        False
+00000990: 2c20 2023 2049 2d4f 5247 0a20 2020 2020  ,  # I-ORG.     
+000009a0: 2020 2046 616c 7365 2c20 2023 204c 2d4f     False,  # L-O
+000009b0: 5247 0a20 2020 2020 2020 2054 7275 652c  RG.        True,
+000009c0: 2020 2320 552d 4f52 470a 2020 2020 2020    # U-ORG.      
+000009d0: 2020 5472 7565 2c20 2023 2042 2d50 4552    True,  # B-PER
+000009e0: 0a20 2020 2020 2020 2046 616c 7365 2c20  .        False, 
+000009f0: 2023 2049 2d50 4552 0a20 2020 2020 2020   # I-PER.       
+00000a00: 2046 616c 7365 2c20 2023 204c 2d50 4552   False,  # L-PER
+00000a10: 0a20 2020 2020 2020 2054 7275 652c 2020  .        True,  
+00000a20: 2320 552d 5045 520a 2020 2020 5d0a 0a20  # U-PER.    ].. 
+00000a30: 2020 2061 7373 6572 7420 6c61 6265 6c5f     assert label_
+00000a40: 7365 742e 6765 745f 7374 6172 745f 7374  set.get_start_st
+00000a50: 6174 6573 2829 203d 3d20 6578 7065 6374  ates() == expect
+00000a60: 6564 0a0a 0a64 6566 2074 6573 745f 656e  ed...def test_en
+00000a70: 645f 7374 6174 6573 5f61 7265 5f76 616c  d_states_are_val
+00000a80: 6964 286c 6162 656c 5f73 6574 3a20 4c61  id(label_set: La
+00000a90: 6265 6c53 6574 2920 2d3e 204e 6f6e 653a  belSet) -> None:
+00000aa0: 0a20 2020 2065 7870 6563 7465 6420 3d20  .    expected = 
+00000ab0: 5b0a 2020 2020 2020 2020 5472 7565 2c20  [.        True, 
+00000ac0: 2023 204f 0a20 2020 2020 2020 2046 616c   # O.        Fal
+00000ad0: 7365 2c20 2023 2042 2d4f 5247 0a20 2020  se,  # B-ORG.   
+00000ae0: 2020 2020 2046 616c 7365 2c20 2023 2049       False,  # I
+00000af0: 2d4f 5247 0a20 2020 2020 2020 2054 7275  -ORG.        Tru
+00000b00: 652c 2020 2320 4c2d 4f52 470a 2020 2020  e,  # L-ORG.    
+00000b10: 2020 2020 5472 7565 2c20 2023 2055 2d4f      True,  # U-O
+00000b20: 5247 0a20 2020 2020 2020 2046 616c 7365  RG.        False
+00000b30: 2c20 2023 2042 2d50 4552 0a20 2020 2020  ,  # B-PER.     
+00000b40: 2020 2046 616c 7365 2c20 2023 2049 2d50     False,  # I-P
+00000b50: 4552 0a20 2020 2020 2020 2054 7275 652c  ER.        True,
+00000b60: 2020 2320 4c2d 5045 520a 2020 2020 2020    # L-PER.      
+00000b70: 2020 5472 7565 2c20 2023 2055 2d50 4552    True,  # U-PER
+00000b80: 0a20 2020 205d 0a0a 2020 2020 6173 7365  .    ]..    asse
+00000b90: 7274 206c 6162 656c 5f73 6574 2e67 6574  rt label_set.get
+00000ba0: 5f65 6e64 5f73 7461 7465 7328 2920 3d3d  _end_states() ==
+00000bb0: 2065 7870 6563 7465 640a 0a0a 6465 6620   expected...def 
+00000bc0: 7465 7374 5f74 7261 6e73 6974 696f 6e73  test_transitions
+00000bd0: 5f61 7265 5f76 616c 6964 286c 6162 656c  _are_valid(label
+00000be0: 5f73 6574 3a20 4c61 6265 6c53 6574 2920  _set: LabelSet) 
+00000bf0: 2d3e 204e 6f6e 653a 0a20 2020 2065 7870  -> None:.    exp
+00000c00: 6563 7465 6420 3d20 5b0a 2020 2020 2020  ected = [.      
+00000c10: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00000c20: 5472 7565 2c20 2023 204f 0a20 2020 2020  True,  # O.     
+00000c30: 2020 2020 2020 2054 7275 652c 2020 2320         True,  # 
+00000c40: 422d 4f52 470a 2020 2020 2020 2020 2020  B-ORG.          
+00000c50: 2020 4661 6c73 652c 2020 2320 492d 4f52    False,  # I-OR
+00000c60: 470a 2020 2020 2020 2020 2020 2020 4661  G.            Fa
+00000c70: 6c73 652c 2020 2320 4c2d 4f52 470a 2020  lse,  # L-ORG.  
+00000c80: 2020 2020 2020 2020 2020 5472 7565 2c20            True, 
+00000c90: 2023 2055 2d4f 5247 0a20 2020 2020 2020   # U-ORG.       
+00000ca0: 2020 2020 2054 7275 652c 2020 2320 422d       True,  # B-
+00000cb0: 5045 520a 2020 2020 2020 2020 2020 2020  PER.            
+00000cc0: 4661 6c73 652c 2020 2320 492d 5045 520a  False,  # I-PER.
+00000cd0: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
+00000ce0: 652c 2020 2320 4c2d 5045 520a 2020 2020  e,  # L-PER.    
+00000cf0: 2020 2020 2020 2020 5472 7565 2c20 2023          True,  #
+00000d00: 2055 2d50 4552 0a20 2020 2020 2020 205d   U-PER.        ]
+00000d10: 2c20 2023 204f 0a20 2020 2020 2020 205b  ,  # O.        [
+00000d20: 0a20 2020 2020 2020 2020 2020 2046 616c  .            Fal
+00000d30: 7365 2c20 2023 204f 0a20 2020 2020 2020  se,  # O.       
+00000d40: 2020 2020 2046 616c 7365 2c20 2023 2042       False,  # B
+00000d50: 2d4f 5247 0a20 2020 2020 2020 2020 2020  -ORG.           
+00000d60: 2054 7275 652c 2020 2320 492d 4f52 470a   True,  # I-ORG.
+00000d70: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00000d80: 2c20 2023 204c 2d4f 5247 0a20 2020 2020  ,  # L-ORG.     
+00000d90: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+00000da0: 2055 2d4f 5247 0a20 2020 2020 2020 2020   U-ORG.         
+00000db0: 2020 2046 616c 7365 2c20 2023 2042 2d50     False,  # B-P
+00000dc0: 4552 0a20 2020 2020 2020 2020 2020 2046  ER.            F
+00000dd0: 616c 7365 2c20 2023 2049 2d50 4552 0a20  alse,  # I-PER. 
+00000de0: 2020 2020 2020 2020 2020 2046 616c 7365             False
+00000df0: 2c20 2023 204c 2d50 4552 0a20 2020 2020  ,  # L-PER.     
+00000e00: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+00000e10: 2055 2d50 4552 0a20 2020 2020 2020 205d   U-PER.        ]
+00000e20: 2c20 2023 2042 2d4f 5247 0a20 2020 2020  ,  # B-ORG.     
+00000e30: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00000e40: 2046 616c 7365 2c20 2023 204f 0a20 2020   False,  # O.   
+00000e50: 2020 2020 2020 2020 2046 616c 7365 2c20           False, 
+00000e60: 2023 2042 2d4f 5247 0a20 2020 2020 2020   # B-ORG.       
+00000e70: 2020 2020 2054 7275 652c 2020 2320 492d       True,  # I-
+00000e80: 4f52 470a 2020 2020 2020 2020 2020 2020  ORG.            
+00000e90: 5472 7565 2c20 2023 204c 2d4f 5247 0a20  True,  # L-ORG. 
+00000ea0: 2020 2020 2020 2020 2020 2046 616c 7365             False
+00000eb0: 2c20 2023 2055 2d4f 5247 0a20 2020 2020  ,  # U-ORG.     
+00000ec0: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+00000ed0: 2042 2d50 4552 0a20 2020 2020 2020 2020   B-PER.         
+00000ee0: 2020 2046 616c 7365 2c20 2023 2049 2d50     False,  # I-P
+00000ef0: 4552 0a20 2020 2020 2020 2020 2020 2046  ER.            F
+00000f00: 616c 7365 2c20 2023 204c 2d50 4552 0a20  alse,  # L-PER. 
+00000f10: 2020 2020 2020 2020 2020 2046 616c 7365             False
+00000f20: 2c20 2023 2055 2d50 4552 0a20 2020 2020  ,  # U-PER.     
+00000f30: 2020 205d 2c20 2023 2049 2d4f 5247 0a20     ],  # I-ORG. 
+00000f40: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00000f50: 2020 2020 2054 7275 652c 2020 2320 4f0a       True,  # O.
+00000f60: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00000f70: 2c20 2023 2042 2d4f 5247 0a20 2020 2020  ,  # B-ORG.     
+00000f80: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+00000f90: 2049 2d4f 5247 0a20 2020 2020 2020 2020   I-ORG.         
+00000fa0: 2020 2046 616c 7365 2c20 2023 204c 2d4f     False,  # L-O
+00000fb0: 5247 0a20 2020 2020 2020 2020 2020 2054  RG.            T
+00000fc0: 7275 652c 2020 2320 552d 4f52 470a 2020  rue,  # U-ORG.  
+00000fd0: 2020 2020 2020 2020 2020 5472 7565 2c20            True, 
+00000fe0: 2023 2042 2d50 4552 0a20 2020 2020 2020   # B-PER.       
+00000ff0: 2020 2020 2046 616c 7365 2c20 2023 2049       False,  # I
+00001000: 2d50 4552 0a20 2020 2020 2020 2020 2020  -PER.           
+00001010: 2046 616c 7365 2c20 2023 204c 2d50 4552   False,  # L-PER
+00001020: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
+00001030: 652c 2020 2320 552d 5045 520a 2020 2020  e,  # U-PER.    
+00001040: 2020 2020 5d2c 2020 2320 4c2d 4f52 470a      ],  # L-ORG.
+00001050: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00001060: 2020 2020 2020 5472 7565 2c20 2023 204f        True,  # O
+00001070: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
+00001080: 652c 2020 2320 422d 4f52 470a 2020 2020  e,  # B-ORG.    
+00001090: 2020 2020 2020 2020 4661 6c73 652c 2020          False,  
+000010a0: 2320 492d 4f52 470a 2020 2020 2020 2020  # I-ORG.        
+000010b0: 2020 2020 4661 6c73 652c 2020 2320 4c2d      False,  # L-
+000010c0: 4f52 470a 2020 2020 2020 2020 2020 2020  ORG.            
+000010d0: 5472 7565 2c20 2023 2055 2d4f 5247 0a20  True,  # U-ORG. 
+000010e0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
+000010f0: 2020 2320 422d 5045 520a 2020 2020 2020    # B-PER.      
+00001100: 2020 2020 2020 4661 6c73 652c 2020 2320        False,  # 
+00001110: 492d 5045 520a 2020 2020 2020 2020 2020  I-PER.          
+00001120: 2020 4661 6c73 652c 2020 2320 4c2d 5045    False,  # L-PE
+00001130: 520a 2020 2020 2020 2020 2020 2020 5472  R.            Tr
+00001140: 7565 2c20 2023 2055 2d50 4552 0a20 2020  ue,  # U-PER.   
+00001150: 2020 2020 205d 2c20 2023 2055 2d4f 5247       ],  # U-ORG
+00001160: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00001170: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+00001180: 204f 0a20 2020 2020 2020 2020 2020 2046   O.            F
+00001190: 616c 7365 2c20 2023 2042 2d4f 5247 0a20  alse,  # B-ORG. 
+000011a0: 2020 2020 2020 2020 2020 2046 616c 7365             False
+000011b0: 2c20 2023 2049 2d4f 5247 0a20 2020 2020  ,  # I-ORG.     
+000011c0: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+000011d0: 204c 2d4f 5247 0a20 2020 2020 2020 2020   L-ORG.         
+000011e0: 2020 2046 616c 7365 2c20 2023 2055 2d4f     False,  # U-O
+000011f0: 5247 0a20 2020 2020 2020 2020 2020 2046  RG.            F
+00001200: 616c 7365 2c20 2023 2042 2d50 4552 0a20  alse,  # B-PER. 
+00001210: 2020 2020 2020 2020 2020 2054 7275 652c             True,
+00001220: 2020 2320 492d 5045 520a 2020 2020 2020    # I-PER.      
+00001230: 2020 2020 2020 5472 7565 2c20 2023 204c        True,  # L
+00001240: 2d50 4552 0a20 2020 2020 2020 2020 2020  -PER.           
+00001250: 2046 616c 7365 2c20 2023 2055 2d50 4552   False,  # U-PER
+00001260: 0a20 2020 2020 2020 205d 2c20 2023 2042  .        ],  # B
+00001270: 2d50 4552 0a20 2020 2020 2020 205b 0a20  -PER.        [. 
+00001280: 2020 2020 2020 2020 2020 2046 616c 7365             False
+00001290: 2c20 2023 204f 0a20 2020 2020 2020 2020  ,  # O.         
+000012a0: 2020 2046 616c 7365 2c20 2023 2042 2d4f     False,  # B-O
+000012b0: 5247 0a20 2020 2020 2020 2020 2020 2046  RG.            F
+000012c0: 616c 7365 2c20 2023 2049 2d4f 5247 0a20  alse,  # I-ORG. 
+000012d0: 2020 2020 2020 2020 2020 2046 616c 7365             False
+000012e0: 2c20 2023 204c 2d4f 5247 0a20 2020 2020  ,  # L-ORG.     
+000012f0: 2020 2020 2020 2046 616c 7365 2c20 2023         False,  #
+00001300: 2055 2d4f 5247 0a20 2020 2020 2020 2020   U-ORG.         
+00001310: 2020 2046 616c 7365 2c20 2023 2042 2d50     False,  # B-P
+00001320: 4552 0a20 2020 2020 2020 2020 2020 2054  ER.            T
+00001330: 7275 652c 2020 2320 492d 5045 520a 2020  rue,  # I-PER.  
+00001340: 2020 2020 2020 2020 2020 5472 7565 2c20            True, 
+00001350: 2023 204c 2d50 4552 0a20 2020 2020 2020   # L-PER.       
+00001360: 2020 2020 2046 616c 7365 2c20 2023 2055       False,  # U
+00001370: 2d50 4552 0a20 2020 2020 2020 205d 2c20  -PER.        ], 
+00001380: 2023 2049 2d50 4552 0a20 2020 2020 2020   # I-PER.       
+00001390: 205b 0a20 2020 2020 2020 2020 2020 2054   [.            T
+000013a0: 7275 652c 2020 2320 4f0a 2020 2020 2020  rue,  # O.      
+000013b0: 2020 2020 2020 5472 7565 2c20 2023 2042        True,  # B
+000013c0: 2d4f 5247 0a20 2020 2020 2020 2020 2020  -ORG.           
+000013d0: 2046 616c 7365 2c20 2023 2049 2d4f 5247   False,  # I-ORG
+000013e0: 0a20 2020 2020 2020 2020 2020 2046 616c  .            Fal
+000013f0: 7365 2c20 2023 204c 2d4f 5247 0a20 2020  se,  # L-ORG.   
+00001400: 2020 2020 2020 2020 2054 7275 652c 2020           True,  
+00001410: 2320 552d 4f52 470a 2020 2020 2020 2020  # U-ORG.        
+00001420: 2020 2020 5472 7565 2c20 2023 2042 2d50      True,  # B-P
+00001430: 4552 0a20 2020 2020 2020 2020 2020 2046  ER.            F
+00001440: 616c 7365 2c20 2023 2049 2d50 4552 0a20  alse,  # I-PER. 
+00001450: 2020 2020 2020 2020 2020 2046 616c 7365             False
+00001460: 2c20 2023 204c 2d50 4552 0a20 2020 2020  ,  # L-PER.     
+00001470: 2020 2020 2020 2054 7275 652c 2020 2320         True,  # 
+00001480: 552d 5045 520a 2020 2020 2020 2020 5d2c  U-PER.        ],
+00001490: 2020 2320 4c2d 5045 520a 2020 2020 2020    # L-PER.      
+000014a0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+000014b0: 5472 7565 2c20 2023 204f 0a20 2020 2020  True,  # O.     
+000014c0: 2020 2020 2020 2054 7275 652c 2020 2320         True,  # 
+000014d0: 422d 4f52 470a 2020 2020 2020 2020 2020  B-ORG.          
+000014e0: 2020 4661 6c73 652c 2020 2320 492d 4f52    False,  # I-OR
+000014f0: 470a 2020 2020 2020 2020 2020 2020 4661  G.            Fa
+00001500: 6c73 652c 2020 2320 4c2d 4f52 470a 2020  lse,  # L-ORG.  
+00001510: 2020 2020 2020 2020 2020 5472 7565 2c20            True, 
+00001520: 2023 2055 2d4f 5247 0a20 2020 2020 2020   # U-ORG.       
+00001530: 2020 2020 2054 7275 652c 2020 2320 422d       True,  # B-
+00001540: 5045 520a 2020 2020 2020 2020 2020 2020  PER.            
+00001550: 4661 6c73 652c 2020 2320 492d 5045 520a  False,  # I-PER.
+00001560: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
+00001570: 652c 2020 2320 4c2d 5045 520a 2020 2020  e,  # L-PER.    
+00001580: 2020 2020 2020 2020 5472 7565 2c20 2023          True,  #
+00001590: 2055 2d50 4552 0a20 2020 2020 2020 205d   U-PER.        ]
+000015a0: 2c20 2023 2055 2d50 4552 0a20 2020 205d  ,  # U-PER.    ]
+000015b0: 0a0a 2020 2020 6173 7365 7274 206c 6162  ..    assert lab
+000015c0: 656c 5f73 6574 2e67 6574 5f74 7261 6e73  el_set.get_trans
+000015d0: 6974 696f 6e73 2829 203d 3d20 6578 7065  itions() == expe
+000015e0: 6374 6564 0a                             cted.
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/2a828151c0a576f1` & `pytorch_partial_tagger-0.1.2/tests/data/test_batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,91 @@
-00000000: 0100 0000 0000 0000 1500 0000 0000 0000  ................
-00000010: 7465 7374 732e 6461 7461 2e74 6573 745f  tests.data.test_
-00000020: 6261 7463 6808 0000 0000 0000 0006 0000  batch...........
-00000030: 0000 0000 0070 7974 6573 7400 0000 000d  .....pytest.....
-00000040: 0000 0005 0000 0000 0000 0074 6f72 6368  ...........torch
-00000050: 0e00 0000 1a00 0000 1a00 0000 0000 0000  ................
-00000060: 7472 616e 7366 6f72 6d65 7273 2e41 7574  transformers.Aut
-00000070: 6f54 6f6b 656e 697a 6572 3400 0000 4100  oTokenizer4...A.
-00000080: 0000 2100 0000 0000 0000 7061 7274 6961  ..!.......partia
-00000090: 6c5f 7461 6767 6572 2e64 6174 612e 4368  l_tagger.data.Ch
-000000a0: 6172 4261 7365 6454 6167 7363 0000 0070  arBasedTagsc...p
-000000b0: 0000 001c 0000 0000 0000 0070 6172 7469  ...........parti
-000000c0: 616c 5f74 6167 6765 722e 6461 7461 2e4c  al_tagger.data.L
-000000d0: 6162 656c 5365 7472 0000 007a 0000 0018  abelSetr...z....
-000000e0: 0000 0000 0000 0070 6172 7469 616c 5f74  .......partial_t
-000000f0: 6167 6765 722e 6461 7461 2e53 7061 6e7c  agger.data.Span|
-00000100: 0000 0080 0000 0017 0000 0000 0000 0070  ...............p
-00000110: 6172 7469 616c 5f74 6167 6765 722e 6461  artial_tagger.da
-00000120: 7461 2e54 6167 8200 0000 8500 0000 3100  ta.Tag........1.
-00000130: 0000 0000 0000 7061 7274 6961 6c5f 7461  ......partial_ta
-00000140: 6767 6572 2e64 6174 612e 6261 7463 682e  gger.data.batch.
-00000150: 5472 616e 7366 6f72 6d65 7242 6174 6368  TransformerBatch
-00000160: 4661 6374 6f72 79ac 0000 00c3 0000 0001  Factory.........
-00000170: 0000 0000 0000 000f 0000 0000 0000 0055  ...............U
-00000180: 6e73 6f72 7465 6449 6d70 6f72 7473 2900  nsortedImports).
-00000190: 0000 0000 0000 496d 706f 7274 2062 6c6f  ......Import blo
-000001a0: 636b 2069 7320 756e 2d73 6f72 7465 6420  ck is un-sorted 
-000001b0: 6f72 2075 6e2d 666f 726d 6174 7465 6401  or un-formatted.
-000001c0: 1000 0000 0000 0000 4f72 6761 6e69 7a65  ........Organize
-000001d0: 2069 6d70 6f72 7473 0000 0000 c600 0000   imports........
-000001e0: 0101 0000 0000 0000 0000 0000 00c6 0000  ................
-000001f0: 0001 c500 0000 0000 0000 696d 706f 7274  ..........import
-00000200: 2070 7974 6573 740a 696d 706f 7274 2074   pytest.import t
-00000210: 6f72 6368 0a66 726f 6d20 7061 7274 6961  orch.from partia
-00000220: 6c5f 7461 6767 6572 2e64 6174 6120 696d  l_tagger.data im
-00000230: 706f 7274 2043 6861 7242 6173 6564 5461  port CharBasedTa
-00000240: 6773 2c20 4c61 6265 6c53 6574 2c20 5370  gs, LabelSet, Sp
-00000250: 616e 2c20 5461 670a 6672 6f6d 2070 6172  an, Tag.from par
-00000260: 7469 616c 5f74 6167 6765 722e 6461 7461  tial_tagger.data
-00000270: 2e62 6174 6368 2069 6d70 6f72 7420 5472  .batch import Tr
-00000280: 616e 7366 6f72 6d65 7242 6174 6368 4661  ansformerBatchFa
-00000290: 6374 6f72 790a 6672 6f6d 2074 7261 6e73  ctory.from trans
-000002a0: 666f 726d 6572 7320 696d 706f 7274 2041  formers import A
-000002b0: 7574 6f54 6f6b 656e 697a 6572 0a0a 0a03  utoTokenizer....
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000002d0: 0000 0000 0000 0049 0000 0000 0000 002f  .......I......./
-000002e0: 5573 6572 732f 7961 7375 6675 6d69 2f57  Users/yasufumi/W
-000002f0: 6f72 6b73 7061 6365 2f70 7974 6f72 6368  orkspace/pytorch
-00000300: 2d70 6172 7469 616c 2d74 6167 6765 722f  -partial-tagger/
-00000310: 7465 7374 732f 6461 7461 2f74 6573 745f  tests/data/test_
-00000320: 6261 7463 682e 7079 b105 0000 0000 0000  batch.py........
-00000330: 696d 706f 7274 2070 7974 6573 740a 696d  import pytest.im
-00000340: 706f 7274 2074 6f72 6368 0a66 726f 6d20  port torch.from 
-00000350: 7472 616e 7366 6f72 6d65 7273 2069 6d70  transformers imp
-00000360: 6f72 7420 4175 746f 546f 6b65 6e69 7a65  ort AutoTokenize
-00000370: 720a 0a66 726f 6d20 7061 7274 6961 6c5f  r..from partial_
-00000380: 7461 6767 6572 2e64 6174 6120 696d 706f  tagger.data impo
-00000390: 7274 2043 6861 7242 6173 6564 5461 6773  rt CharBasedTags
-000003a0: 2c20 4c61 6265 6c53 6574 2c20 5370 616e  , LabelSet, Span
-000003b0: 2c20 5461 670a 6672 6f6d 2070 6172 7469  , Tag.from parti
-000003c0: 616c 5f74 6167 6765 722e 6461 7461 2e62  al_tagger.data.b
-000003d0: 6174 6368 2069 6d70 6f72 7420 5472 616e  atch import Tran
-000003e0: 7366 6f72 6d65 7242 6174 6368 4661 6374  sformerBatchFact
-000003f0: 6f72 790a 0a0a 4070 7974 6573 742e 6669  ory...@pytest.fi
-00000400: 7874 7572 650a 6465 6620 6261 7463 685f  xture.def batch_
-00000410: 6661 6374 6f72 7928 2920 2d3e 2054 7261  factory() -> Tra
-00000420: 6e73 666f 726d 6572 4261 7463 6846 6163  nsformerBatchFac
-00000430: 746f 7279 3a0a 2020 2020 7265 7475 726e  tory:.    return
-00000440: 2054 7261 6e73 666f 726d 6572 4261 7463   TransformerBatc
-00000450: 6846 6163 746f 7279 280a 2020 2020 2020  hFactory(.      
-00000460: 2020 4175 746f 546f 6b65 6e69 7a65 722e    AutoTokenizer.
-00000470: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00000480: 2264 6973 7469 6c72 6f62 6572 7461 2d62  "distilroberta-b
-00000490: 6173 6522 292c 0a20 2020 2020 2020 204c  ase"),.        L
-000004a0: 6162 656c 5365 7428 7b22 4c4f 4322 2c20  abelSet({"LOC", 
-000004b0: 224d 4953 4322 2c20 224f 5247 222c 2022  "MISC", "ORG", "
-000004c0: 5045 5222 7d29 2c0a 2020 2020 290a 0a0a  PER"}),.    )...
-000004d0: 6465 6620 7465 7374 5f63 6861 725f 6261  def test_char_ba
-000004e0: 7365 645f 7461 6773 5f61 7265 5f76 616c  sed_tags_are_val
-000004f0: 6964 2862 6174 6368 5f66 6163 746f 7279  id(batch_factory
-00000500: 3a20 5472 616e 7366 6f72 6d65 7242 6174  : TransformerBat
-00000510: 6368 4661 6374 6f72 7929 202d 3e20 4e6f  chFactory) -> No
-00000520: 6e65 3a0a 2020 2020 7465 7874 203d 2022  ne:.    text = "
-00000530: 546f 6b79 6f20 6973 2074 6865 2063 6170  Tokyo is the cap
-00000540: 6974 616c 206f 6620 4a61 7061 6e2e 220a  ital of Japan.".
-00000550: 2020 2020 7461 675f 696e 6469 6365 7320      tag_indices 
-00000560: 3d20 746f 7263 682e 7465 6e73 6f72 285b  = torch.tensor([
-00000570: 5b30 2c20 312c 2033 2c20 302c 2030 2c20  [0, 1, 3, 0, 0, 
-00000580: 302c 2030 2c20 342c 2030 2c20 305d 5d29  0, 0, 4, 0, 0]])
-00000590: 0a0a 2020 2020 6578 7065 6374 6564 203d  ..    expected =
-000005a0: 2043 6861 7242 6173 6564 5461 6773 280a   CharBasedTags(.
-000005b0: 2020 2020 2020 2020 2854 6167 2853 7061          (Tag(Spa
-000005c0: 6e28 302c 2035 292c 2022 4c4f 4322 292c  n(0, 5), "LOC"),
-000005d0: 2054 6167 2853 7061 6e28 3234 2c20 3529   Tag(Span(24, 5)
-000005e0: 2c20 224c 4f43 2229 292c 2074 6578 743d  , "LOC")), text=
-000005f0: 7465 7874 0a20 2020 2029 0a0a 2020 2020  text.    )..    
-00000600: 6261 7463 6820 3d20 6261 7463 685f 6661  batch = batch_fa
-00000610: 6374 6f72 792e 6372 6561 7465 2828 7465  ctory.create((te
-00000620: 7874 2c29 290a 2020 2020 6368 6172 5f62  xt,)).    char_b
-00000630: 6173 6564 5f74 6167 735f 636f 6c6c 6563  ased_tags_collec
-00000640: 7469 6f6e 203d 2062 6174 6368 2e63 7265  tion = batch.cre
-00000650: 6174 655f 6368 6172 5f62 6173 6564 5f74  ate_char_based_t
-00000660: 6167 7328 7461 675f 696e 6469 6365 7329  ags(tag_indices)
-00000670: 0a0a 2020 2020 6173 7365 7274 206c 656e  ..    assert len
-00000680: 2863 6861 725f 6261 7365 645f 7461 6773  (char_based_tags
-00000690: 5f63 6f6c 6c65 6374 696f 6e29 203d 3d20  _collection) == 
-000006a0: 310a 2020 2020 6173 7365 7274 2063 6861  1.    assert cha
-000006b0: 725f 6261 7365 645f 7461 6773 5f63 6f6c  r_based_tags_col
-000006c0: 6c65 6374 696f 6e5b 305d 203d 3d20 6578  lection[0] == ex
-000006d0: 7065 6374 6564 0a0a 0a64 6566 2074 6573  pected...def tes
-000006e0: 745f 7461 675f 696e 6469 6365 735f 6172  t_tag_indices_ar
-000006f0: 655f 7661 6c69 6428 6261 7463 685f 6661  e_valid(batch_fa
-00000700: 6374 6f72 793a 2054 7261 6e73 666f 726d  ctory: Transform
-00000710: 6572 4261 7463 6846 6163 746f 7279 2920  erBatchFactory) 
-00000720: 2d3e 204e 6f6e 653a 0a20 2020 2074 6578  -> None:.    tex
-00000730: 7420 3d20 2254 6f6b 796f 2069 7320 7468  t = "Tokyo is th
-00000740: 6520 6361 7069 7461 6c20 6f66 204a 6170  e capital of Jap
-00000750: 616e 2e22 0a20 2020 2074 6167 7320 3d20  an.".    tags = 
-00000760: 4368 6172 4261 7365 6454 6167 7328 2854  CharBasedTags((T
-00000770: 6167 2853 7061 6e28 302c 2035 292c 2022  ag(Span(0, 5), "
-00000780: 4c4f 4322 292c 2054 6167 2853 7061 6e28  LOC"), Tag(Span(
-00000790: 3234 2c20 3529 2c20 224c 4f43 2229 292c  24, 5), "LOC")),
-000007a0: 2074 6578 743d 7465 7874 290a 2020 2020   text=text).    
-000007b0: 756e 6b6e 6f77 6e5f 696e 6465 7820 3d20  unknown_index = 
-000007c0: 2d31 3030 0a0a 2020 2020 6578 7065 6374  -100..    expect
-000007d0: 6564 203d 2074 6f72 6368 2e74 656e 736f  ed = torch.tenso
-000007e0: 7228 5b5b 302c 2031 2c20 332c 202d 3130  r([[0, 1, 3, -10
-000007f0: 302c 202d 3130 302c 202d 3130 302c 202d  0, -100, -100, -
-00000800: 3130 302c 2034 2c20 2d31 3030 2c20 305d  100, 4, -100, 0]
-00000810: 5d29 0a0a 2020 2020 6261 7463 6820 3d20  ])..    batch = 
-00000820: 6261 7463 685f 6661 6374 6f72 792e 6372  batch_factory.cr
-00000830: 6561 7465 2828 7465 7874 2c29 290a 2020  eate((text,)).  
-00000840: 2020 7461 675f 696e 6469 6365 7320 3d20    tag_indices = 
-00000850: 6261 7463 682e 6372 6561 7465 5f74 6167  batch.create_tag
-00000860: 5f69 6e64 6963 6573 280a 2020 2020 2020  _indices(.      
-00000870: 2020 2874 6167 732c 292c 2074 6f72 6368    (tags,), torch
-00000880: 2e64 6576 6963 6528 2263 7075 2229 2c20  .device("cpu"), 
-00000890: 756e 6b6e 6f77 6e5f 696e 6465 783d 756e  unknown_index=un
-000008a0: 6b6e 6f77 6e5f 696e 6465 780a 2020 2020  known_index.    
-000008b0: 290a 0a20 2020 2061 7373 6572 7420 746f  )..    assert to
-000008c0: 7263 682e 6571 7561 6c28 7461 675f 696e  rch.equal(tag_in
-000008d0: 6469 6365 732c 2065 7870 6563 7465 6429  dices, expected)
-000008e0: 0a                                       .
+00000000: 696d 706f 7274 2070 7974 6573 740a 696d  import pytest.im
+00000010: 706f 7274 2074 6f72 6368 0a66 726f 6d20  port torch.from 
+00000020: 7061 7274 6961 6c5f 7461 6767 6572 2e64  partial_tagger.d
+00000030: 6174 6120 696d 706f 7274 2043 6861 7242  ata import CharB
+00000040: 6173 6564 5461 6773 2c20 4c61 6265 6c53  asedTags, LabelS
+00000050: 6574 2c20 5370 616e 2c20 5461 670a 6672  et, Span, Tag.fr
+00000060: 6f6d 2070 6172 7469 616c 5f74 6167 6765  om partial_tagge
+00000070: 722e 6461 7461 2e62 6174 6368 2069 6d70  r.data.batch imp
+00000080: 6f72 7420 5472 616e 7366 6f72 6d65 7242  ort TransformerB
+00000090: 6174 6368 4661 6374 6f72 790a 6672 6f6d  atchFactory.from
+000000a0: 2074 7261 6e73 666f 726d 6572 7320 696d   transformers im
+000000b0: 706f 7274 2041 7574 6f54 6f6b 656e 697a  port AutoTokeniz
+000000c0: 6572 0a0a 0a40 7079 7465 7374 2e66 6978  er...@pytest.fix
+000000d0: 7475 7265 0a64 6566 2062 6174 6368 5f66  ture.def batch_f
+000000e0: 6163 746f 7279 2829 202d 3e20 5472 616e  actory() -> Tran
+000000f0: 7366 6f72 6d65 7242 6174 6368 4661 6374  sformerBatchFact
+00000100: 6f72 793a 0a20 2020 2072 6574 7572 6e20  ory:.    return 
+00000110: 5472 616e 7366 6f72 6d65 7242 6174 6368  TransformerBatch
+00000120: 4661 6374 6f72 7928 0a20 2020 2020 2020  Factory(.       
+00000130: 2041 7574 6f54 6f6b 656e 697a 6572 2e66   AutoTokenizer.f
+00000140: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00000150: 6469 7374 696c 726f 6265 7274 612d 6261  distilroberta-ba
+00000160: 7365 2229 2c0a 2020 2020 2020 2020 4c61  se"),.        La
+00000170: 6265 6c53 6574 287b 224c 4f43 222c 2022  belSet({"LOC", "
+00000180: 4d49 5343 222c 2022 4f52 4722 2c20 2250  MISC", "ORG", "P
+00000190: 4552 227d 292c 0a20 2020 2029 0a0a 0a64  ER"}),.    )...d
+000001a0: 6566 2074 6573 745f 6368 6172 5f62 6173  ef test_char_bas
+000001b0: 6564 5f74 6167 735f 6172 655f 7661 6c69  ed_tags_are_vali
+000001c0: 6428 6261 7463 685f 6661 6374 6f72 793a  d(batch_factory:
+000001d0: 2054 7261 6e73 666f 726d 6572 4261 7463   TransformerBatc
+000001e0: 6846 6163 746f 7279 2920 2d3e 204e 6f6e  hFactory) -> Non
+000001f0: 653a 0a20 2020 2074 6578 7420 3d20 2254  e:.    text = "T
+00000200: 6f6b 796f 2069 7320 7468 6520 6361 7069  okyo is the capi
+00000210: 7461 6c20 6f66 204a 6170 616e 2e22 0a20  tal of Japan.". 
+00000220: 2020 2074 6167 5f69 6e64 6963 6573 203d     tag_indices =
+00000230: 2074 6f72 6368 2e74 656e 736f 7228 5b5b   torch.tensor([[
+00000240: 302c 2031 2c20 332c 2030 2c20 302c 2030  0, 1, 3, 0, 0, 0
+00000250: 2c20 302c 2034 2c20 302c 2030 5d5d 290a  , 0, 4, 0, 0]]).
+00000260: 0a20 2020 2065 7870 6563 7465 6420 3d20  .    expected = 
+00000270: 4368 6172 4261 7365 6454 6167 7328 0a20  CharBasedTags(. 
+00000280: 2020 2020 2020 2028 5461 6728 5370 616e         (Tag(Span
+00000290: 2830 2c20 3529 2c20 224c 4f43 2229 2c20  (0, 5), "LOC"), 
+000002a0: 5461 6728 5370 616e 2832 342c 2035 292c  Tag(Span(24, 5),
+000002b0: 2022 4c4f 4322 2929 2c20 7465 7874 3d74   "LOC")), text=t
+000002c0: 6578 740a 2020 2020 290a 0a20 2020 2062  ext.    )..    b
+000002d0: 6174 6368 203d 2062 6174 6368 5f66 6163  atch = batch_fac
+000002e0: 746f 7279 2e63 7265 6174 6528 2874 6578  tory.create((tex
+000002f0: 742c 2929 0a20 2020 2063 6861 725f 6261  t,)).    char_ba
+00000300: 7365 645f 7461 6773 5f63 6f6c 6c65 6374  sed_tags_collect
+00000310: 696f 6e20 3d20 6261 7463 682e 6372 6561  ion = batch.crea
+00000320: 7465 5f63 6861 725f 6261 7365 645f 7461  te_char_based_ta
+00000330: 6773 2874 6167 5f69 6e64 6963 6573 290a  gs(tag_indices).
+00000340: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00000350: 6368 6172 5f62 6173 6564 5f74 6167 735f  char_based_tags_
+00000360: 636f 6c6c 6563 7469 6f6e 2920 3d3d 2031  collection) == 1
+00000370: 0a20 2020 2061 7373 6572 7420 6368 6172  .    assert char
+00000380: 5f62 6173 6564 5f74 6167 735f 636f 6c6c  _based_tags_coll
+00000390: 6563 7469 6f6e 5b30 5d20 3d3d 2065 7870  ection[0] == exp
+000003a0: 6563 7465 640a 0a0a 6465 6620 7465 7374  ected...def test
+000003b0: 5f74 6167 5f69 6e64 6963 6573 5f61 7265  _tag_indices_are
+000003c0: 5f76 616c 6964 2862 6174 6368 5f66 6163  _valid(batch_fac
+000003d0: 746f 7279 3a20 5472 616e 7366 6f72 6d65  tory: Transforme
+000003e0: 7242 6174 6368 4661 6374 6f72 7929 202d  rBatchFactory) -
+000003f0: 3e20 4e6f 6e65 3a0a 2020 2020 7465 7874  > None:.    text
+00000400: 203d 2022 546f 6b79 6f20 6973 2074 6865   = "Tokyo is the
+00000410: 2063 6170 6974 616c 206f 6620 4a61 7061   capital of Japa
+00000420: 6e2e 220a 2020 2020 7461 6773 203d 2043  n.".    tags = C
+00000430: 6861 7242 6173 6564 5461 6773 2828 5461  harBasedTags((Ta
+00000440: 6728 5370 616e 2830 2c20 3529 2c20 224c  g(Span(0, 5), "L
+00000450: 4f43 2229 2c20 5461 6728 5370 616e 2832  OC"), Tag(Span(2
+00000460: 342c 2035 292c 2022 4c4f 4322 2929 2c20  4, 5), "LOC")), 
+00000470: 7465 7874 3d74 6578 7429 0a20 2020 2075  text=text).    u
+00000480: 6e6b 6e6f 776e 5f69 6e64 6578 203d 202d  nknown_index = -
+00000490: 3130 300a 0a20 2020 2065 7870 6563 7465  100..    expecte
+000004a0: 6420 3d20 746f 7263 682e 7465 6e73 6f72  d = torch.tensor
+000004b0: 285b 5b30 2c20 312c 2033 2c20 2d31 3030  ([[0, 1, 3, -100
+000004c0: 2c20 2d31 3030 2c20 2d31 3030 2c20 2d31  , -100, -100, -1
+000004d0: 3030 2c20 342c 202d 3130 302c 2030 5d5d  00, 4, -100, 0]]
+000004e0: 290a 0a20 2020 2062 6174 6368 203d 2062  )..    batch = b
+000004f0: 6174 6368 5f66 6163 746f 7279 2e63 7265  atch_factory.cre
+00000500: 6174 6528 2874 6578 742c 2929 0a20 2020  ate((text,)).   
+00000510: 2074 6167 5f69 6e64 6963 6573 203d 2062   tag_indices = b
+00000520: 6174 6368 2e63 7265 6174 655f 7461 675f  atch.create_tag_
+00000530: 696e 6469 6365 7328 0a20 2020 2020 2020  indices(.       
+00000540: 2028 7461 6773 2c29 2c20 746f 7263 682e   (tags,), torch.
+00000550: 6465 7669 6365 2822 6370 7522 292c 2075  device("cpu"), u
+00000560: 6e6b 6e6f 776e 5f69 6e64 6578 3d75 6e6b  nknown_index=unk
+00000570: 6e6f 776e 5f69 6e64 6578 0a20 2020 2029  nown_index.    )
+00000580: 0a0a 2020 2020 6173 7365 7274 2074 6f72  ..    assert tor
+00000590: 6368 2e65 7175 616c 2874 6167 5f69 6e64  ch.equal(tag_ind
+000005a0: 6963 6573 2c20 6578 7065 6374 6564 290a  ices, expected).
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/2ffcbecadc4b3fd4` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/data/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,597 +1,539 @@
-00000000: 0100 0000 0000 0000 0a00 0000 0000 0000  ................
-00000010: 6461 7461 2e62 6174 6368 0c00 0000 0000  data.batch......
-00000020: 0000 0b00 0000 0000 0000 6162 632e 4142  ..........abc.AB
-00000030: 434d 6574 6110 0000 0017 0000 0012 0000  CMeta...........
-00000040: 0000 0000 0061 6263 2e61 6273 7472 6163  .....abc.abstrac
-00000050: 746d 6574 686f 6419 0000 0027 0000 0011  tmethod....'....
-00000060: 0000 0000 0000 0069 7465 7274 6f6f 6c73  .......itertools
-00000070: 2e67 726f 7570 6279 3e00 0000 4500 0000  .groupby>...E...
-00000080: 0f00 0000 0000 0000 7479 7069 6e67 2e4f  ........typing.O
-00000090: 7074 696f 6e61 6c59 0000 0061 0000 0005  ptionalY...a....
-000000a0: 0000 0000 0000 0074 6f72 6368 6300 0000  .......torchc...
-000000b0: 6f00 0000 3300 0000 0000 0000 7472 616e  o...3.......tran
-000000c0: 7366 6f72 6d65 7273 2e74 6f6b 656e 697a  sformers.tokeniz
-000000d0: 6174 696f 6e5f 7574 696c 732e 5072 6554  ation_utils.PreT
-000000e0: 7261 696e 6564 546f 6b65 6e69 7a65 729c  rainedTokenizer.
-000000f0: 0000 00af 0000 0012 0000 0000 0000 0064  ...............d
-00000100: 6174 612e 4368 6172 4261 7365 6454 6167  ata.CharBasedTag
-00000110: 73ea 0000 00f7 0000 000d 0000 0000 0000  s...............
-00000120: 0064 6174 612e 4c61 6265 6c53 6574 f900  .data.LabelSet..
-00000130: 0000 0101 0000 0900 0000 0000 0000 6461  ..............da
-00000140: 7461 2e53 7061 6e03 0100 0007 0100 0015  ta.Span.........
-00000150: 0000 0000 0000 0064 6174 612e 5375 6277  .......data.Subw
-00000160: 6f72 6442 6173 6564 5461 6773 0901 0000  ordBasedTags....
-00000170: 1901 0000 0800 0000 0000 0000 6461 7461  ............data
-00000180: 2e54 6167 1b01 0000 1e01 0000 1200 0000  .Tag............
-00000190: 0000 0000 6461 7461 2e54 6f6b 656e 697a  ....data.Tokeniz
-000001a0: 6564 5465 7874 2001 0000 2d01 0000 0400  edText ...-.....
-000001b0: 0000 0000 0000 1800 0000 0000 0000 5a69  ..............Zi
-000001c0: 7057 6974 686f 7574 4578 706c 6963 6974  pWithoutExplicit
-000001d0: 5374 7269 6374 2f00 0000 0000 0000 607a  Strict/.......`z
-000001e0: 6970 2829 6020 7769 7468 6f75 7420 616e  ip()` without an
-000001f0: 2065 7870 6c69 6369 7420 6073 7472 6963   explicit `stric
-00000200: 743d 6020 7061 7261 6d65 7465 7200 a206  t=` parameter...
-00000210: 0000 f606 0000 0000 0000 0000 0000 00a2  ................
-00000220: 0600 0018 0000 0000 0000 005a 6970 5769  ...........ZipWi
-00000230: 7468 6f75 7445 7870 6c69 6369 7453 7472  thoutExplicitStr
-00000240: 6963 742f 0000 0000 0000 0060 7a69 7028  ict/.......`zip(
-00000250: 2960 2077 6974 686f 7574 2061 6e20 6578  )` without an ex
-00000260: 706c 6963 6974 2060 7374 7269 6374 3d60  plicit `strict=`
-00000270: 2070 6172 616d 6574 6572 00e2 0900 000e   parameter......
-00000280: 0a00 0000 0000 0000 0000 0000 e209 0000  ................
-00000290: 1800 0000 0000 0000 5a69 7057 6974 686f  ........ZipWitho
-000002a0: 7574 4578 706c 6963 6974 5374 7269 6374  utExplicitStrict
-000002b0: 2f00 0000 0000 0000 607a 6970 2829 6020  /.......`zip()` 
-000002c0: 7769 7468 6f75 7420 616e 2065 7870 6c69  without an expli
-000002d0: 6369 7420 6073 7472 6963 743d 6020 7061  cit `strict=` pa
-000002e0: 7261 6d65 7465 7200 fc1b 0000 3e1c 0000  rameter.....>...
-000002f0: 0000 0000 0000 0000 00fc 1b00 0018 0000  ................
-00000300: 0000 0000 005a 6970 5769 7468 6f75 7445  .....ZipWithoutE
-00000310: 7870 6c69 6369 7453 7472 6963 742f 0000  xplicitStrict/..
-00000320: 0000 0000 0060 7a69 7028 2960 2077 6974  .....`zip()` wit
-00000330: 686f 7574 2061 6e20 6578 706c 6963 6974  hout an explicit
-00000340: 2060 7374 7269 6374 3d60 2070 6172 616d   `strict=` param
-00000350: 6574 6572 0026 2100 0034 2100 0000 0000  eter.&!..4!.....
-00000360: 0000 0000 0000 2621 0000 0100 0000 0000  ......&!........
-00000370: 0000 5100 0000 0000 0000 2f55 7365 7273  ..Q......./Users
-00000380: 2f79 6173 7566 756d 692f 576f 726b 7370  /yasufumi/Worksp
-00000390: 6163 652f 7079 746f 7263 682d 7061 7274  ace/pytorch-part
-000003a0: 6961 6c2d 7461 6767 6572 2f73 7263 2f70  ial-tagger/src/p
-000003b0: 6172 7469 616c 5f74 6167 6765 722f 6461  artial_tagger/da
-000003c0: 7461 2f62 6174 6368 2e70 7976 2100 0000  ta/batch.pyv!...
-000003d0: 0000 0066 726f 6d20 6162 6320 696d 706f  ...from abc impo
-000003e0: 7274 2041 4243 4d65 7461 2c20 6162 7374  rt ABCMeta, abst
-000003f0: 7261 6374 6d65 7468 6f64 0a66 726f 6d20  ractmethod.from 
-00000400: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
-00000410: 2067 726f 7570 6279 0a66 726f 6d20 7479   groupby.from ty
-00000420: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
-00000430: 6f6e 616c 0a0a 696d 706f 7274 2074 6f72  onal..import tor
-00000440: 6368 0a66 726f 6d20 7472 616e 7366 6f72  ch.from transfor
-00000450: 6d65 7273 2e74 6f6b 656e 697a 6174 696f  mers.tokenizatio
-00000460: 6e5f 7574 696c 7320 696d 706f 7274 2050  n_utils import P
-00000470: 7265 5472 6169 6e65 6454 6f6b 656e 697a  reTrainedTokeniz
-00000480: 6572 0a0a 6672 6f6d 202e 2e63 7266 2e66  er..from ..crf.f
-00000490: 756e 6374 696f 6e61 6c20 696d 706f 7274  unctional import
-000004a0: 2074 6f5f 7461 675f 6269 746d 6170 0a66   to_tag_bitmap.f
-000004b0: 726f 6d20 2e20 696d 706f 7274 2043 6861  rom . import Cha
-000004c0: 7242 6173 6564 5461 6773 2c20 4c61 6265  rBasedTags, Labe
-000004d0: 6c53 6574 2c20 5370 616e 2c20 5375 6277  lSet, Span, Subw
-000004e0: 6f72 6442 6173 6564 5461 6773 2c20 5461  ordBasedTags, Ta
-000004f0: 672c 2054 6f6b 656e 697a 6564 5465 7874  g, TokenizedText
-00000500: 0a0a 5465 7874 7320 3d20 7475 706c 655b  ..Texts = tuple[
-00000510: 7374 722c 202e 2e2e 5d0a 546f 6b65 6e69  str, ...].Tokeni
-00000520: 7a65 6454 6578 7473 203d 2074 7570 6c65  zedTexts = tuple
-00000530: 5b54 6f6b 656e 697a 6564 5465 7874 2c20  [TokenizedText, 
-00000540: 2e2e 2e5d 0a0a 4368 6172 4261 7365 6454  ...]..CharBasedT
-00000550: 6167 7343 6f6c 6c65 6374 696f 6e20 3d20  agsCollection = 
-00000560: 7475 706c 655b 4368 6172 4261 7365 6454  tuple[CharBasedT
-00000570: 6167 732c 202e 2e2e 5d0a 5375 6277 6f72  ags, ...].Subwor
-00000580: 6442 6173 6564 5461 6773 436f 6c6c 6563  dBasedTagsCollec
-00000590: 7469 6f6e 203d 2074 7570 6c65 5b53 7562  tion = tuple[Sub
-000005a0: 776f 7264 4261 7365 6454 6167 732c 202e  wordBasedTags, .
-000005b0: 2e2e 5d0a 0a44 6174 6173 6574 203d 206c  ..]..Dataset = l
-000005c0: 6973 745b 7475 706c 655b 7374 722c 2043  ist[tuple[str, C
-000005d0: 6861 7242 6173 6564 5461 6773 5d5d 0a0a  harBasedTags]]..
-000005e0: 5461 6767 6572 496e 7075 7473 203d 2064  TaggerInputs = d
-000005f0: 6963 745b 7374 722c 2074 6f72 6368 2e54  ict[str, torch.T
-00000600: 656e 736f 725d 0a0a 0a64 6566 2070 6164  ensor]...def pad
-00000610: 2862 6174 6368 3a20 6c69 7374 5b6c 6973  (batch: list[lis
-00000620: 745b 696e 745d 5d2c 2066 696c 6c5f 7661  t[int]], fill_va
-00000630: 6c75 653a 2069 6e74 2920 2d3e 2074 6f72  lue: int) -> tor
-00000640: 6368 2e54 656e 736f 723a 0a20 2020 206d  ch.Tensor:.    m
-00000650: 6178 5f6c 656e 6774 6820 3d20 6d61 7828  ax_length = max(
-00000660: 6d61 7028 6c65 6e2c 2062 6174 6368 2929  map(len, batch))
-00000670: 0a20 2020 2072 6574 7572 6e20 746f 7263  .    return torc
-00000680: 682e 7465 6e73 6f72 285b 7820 2b20 5b66  h.tensor([x + [f
-00000690: 696c 6c5f 7661 6c75 655d 202a 2028 6d61  ill_value] * (ma
-000006a0: 785f 6c65 6e67 7468 202d 206c 656e 2878  x_length - len(x
-000006b0: 2929 2066 6f72 2078 2069 6e20 6261 7463  )) for x in batc
-000006c0: 685d 290a 0a0a 6465 6620 756e 7061 6428  h])...def unpad(
-000006d0: 6261 7463 683a 2074 6f72 6368 2e54 656e  batch: torch.Ten
-000006e0: 736f 722c 2066 696c 6c5f 7661 6c75 653a  sor, fill_value:
-000006f0: 2069 6e74 2920 2d3e 206c 6973 745b 6c69   int) -> list[li
-00000700: 7374 5b69 6e74 5d5d 3a0a 2020 2020 7265  st[int]]:.    re
-00000710: 7475 726e 205b 5b69 2066 6f72 2069 2069  turn [[i for i i
-00000720: 6e20 7820 6966 2069 2021 3d20 6669 6c6c  n x if i != fill
-00000730: 5f76 616c 7565 5d20 666f 7220 7820 696e  _value] for x in
-00000740: 2062 6174 6368 2e74 6f6c 6973 7428 295d   batch.tolist()]
-00000750: 0a0a 0a63 6c61 7373 2054 6167 4661 6374  ...class TagFact
-00000760: 6f72 793a 0a20 2020 2064 6566 205f 5f69  ory:.    def __i
-00000770: 6e69 745f 5f28 7365 6c66 2c20 746f 6b65  nit__(self, toke
-00000780: 6e69 7a65 645f 7465 7874 733a 2054 6f6b  nized_texts: Tok
-00000790: 656e 697a 6564 5465 7874 732c 206c 6162  enizedTexts, lab
-000007a0: 656c 5f73 6574 3a20 4c61 6265 6c53 6574  el_set: LabelSet
-000007b0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000007c0: 5f5f 746f 6b65 6e69 7a65 645f 7465 7874  __tokenized_text
-000007d0: 7320 3d20 746f 6b65 6e69 7a65 645f 7465  s = tokenized_te
-000007e0: 7874 730a 2020 2020 2020 2020 7365 6c66  xts.        self
-000007f0: 2e5f 5f6c 6162 656c 5f73 6574 203d 206c  .__label_set = l
-00000800: 6162 656c 5f73 6574 0a0a 2020 2020 4070  abel_set..    @p
-00000810: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00000820: 746f 6b65 6e69 7a65 645f 7465 7874 7328  tokenized_texts(
-00000830: 7365 6c66 2920 2d3e 2054 6f6b 656e 697a  self) -> Tokeniz
-00000840: 6564 5465 7874 733a 0a20 2020 2020 2020  edTexts:.       
-00000850: 2072 6574 7572 6e20 7365 6c66 2e5f 5f74   return self.__t
-00000860: 6f6b 656e 697a 6564 5f74 6578 7473 0a0a  okenized_texts..
-00000870: 2020 2020 6465 6620 6372 6561 7465 5f63      def create_c
-00000880: 6861 725f 6261 7365 645f 7461 6773 280a  har_based_tags(.
-00000890: 2020 2020 2020 2020 7365 6c66 2c20 7461          self, ta
-000008a0: 675f 696e 6469 6365 733a 2074 6f72 6368  g_indices: torch
-000008b0: 2e54 656e 736f 722c 2070 6164 6469 6e67  .Tensor, padding
-000008c0: 5f69 6e64 6578 3a20 696e 7420 3d20 2d31  _index: int = -1
-000008d0: 0a20 2020 2029 202d 3e20 4368 6172 4261  .    ) -> CharBa
-000008e0: 7365 6454 6167 7343 6f6c 6c65 6374 696f  sedTagsCollectio
-000008f0: 6e3a 0a20 2020 2020 2020 2072 6574 7572  n:.        retur
-00000900: 6e20 7475 706c 6528 0a20 2020 2020 2020  n tuple(.       
-00000910: 2020 2020 2074 6167 732e 6765 745f 6368       tags.get_ch
-00000920: 6172 5f62 6173 6564 5f74 6167 7328 290a  ar_based_tags().
-00000930: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000940: 7461 6773 2069 6e20 7365 6c66 2e63 7265  tags in self.cre
-00000950: 6174 655f 7375 6277 6f72 645f 6261 7365  ate_subword_base
-00000960: 645f 7461 6773 2874 6167 5f69 6e64 6963  d_tags(tag_indic
-00000970: 6573 2c20 7061 6464 696e 675f 696e 6465  es, padding_inde
-00000980: 7829 0a20 2020 2020 2020 2029 0a0a 2020  x).        )..  
-00000990: 2020 6465 6620 6372 6561 7465 5f73 7562    def create_sub
-000009a0: 776f 7264 5f62 6173 6564 5f74 6167 7328  word_based_tags(
-000009b0: 0a20 2020 2020 2020 2073 656c 662c 2074  .        self, t
-000009c0: 6167 5f69 6e64 6963 6573 3a20 746f 7263  ag_indices: torc
-000009d0: 682e 5465 6e73 6f72 2c20 7061 6464 696e  h.Tensor, paddin
-000009e0: 675f 696e 6465 783a 2069 6e74 203d 202d  g_index: int = -
-000009f0: 310a 2020 2020 2920 2d3e 2053 7562 776f  1.    ) -> Subwo
-00000a00: 7264 4261 7365 6454 6167 7343 6f6c 6c65  rdBasedTagsColle
-00000a10: 6374 696f 6e3a 0a20 2020 2020 2020 206c  ction:.        l
-00000a20: 6162 656c 5f73 6574 203d 2073 656c 662e  abel_set = self.
-00000a30: 5f5f 6c61 6265 6c5f 7365 740a 0a20 2020  __label_set..   
-00000a40: 2020 2020 2062 6174 6368 6564 5f74 6167       batched_tag
-00000a50: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
-00000a60: 666f 7220 7465 7874 2c20 696e 6469 6365  for text, indice
-00000a70: 7320 696e 207a 6970 280a 2020 2020 2020  s in zip(.      
-00000a80: 2020 2020 2020 7365 6c66 2e5f 5f74 6f6b        self.__tok
-00000a90: 656e 697a 6564 5f74 6578 7473 2c20 756e  enized_texts, un
-00000aa0: 7061 6428 7461 675f 696e 6469 6365 732c  pad(tag_indices,
-00000ab0: 2070 6164 6469 6e67 5f69 6e64 6578 290a   padding_index).
-00000ac0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00000ad0: 2020 2020 2020 2074 6167 7320 3d20 5b5d         tags = []
-00000ae0: 0a20 2020 2020 2020 2020 2020 206e 6f77  .            now
-00000af0: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-00000b00: 2066 6f72 206c 6162 656c 2c20 6772 6f75   for label, grou
-00000b10: 7020 696e 2067 726f 7570 6279 280a 2020  p in groupby(.  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00000b30: 6265 6c5f 7365 742e 6765 745f 6c61 6265  bel_set.get_labe
-00000b40: 6c28 696e 6465 7829 2066 6f72 2069 6e64  l(index) for ind
-00000b50: 6578 2069 6e20 696e 6469 6365 730a 2020  ex in indices.  
-00000b60: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00000b70: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00000b80: 6774 6820 3d20 6c65 6e28 6c69 7374 2867  gth = len(list(g
-00000b90: 726f 7570 2929 0a0a 2020 2020 2020 2020  roup))..        
-00000ba0: 2020 2020 2020 2020 6966 206c 6162 656c          if label
-00000bb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2020 7461 6773 2e61 7070 656e 6428 5461    tags.append(Ta
-00000be0: 6728 5370 616e 286e 6f77 2c20 6c65 6e67  g(Span(now, leng
-00000bf0: 7468 292c 206c 6162 656c 2929 0a0a 2020  th), label))..  
-00000c00: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00000c10: 7720 2b3d 206c 656e 6774 680a 0a20 2020  w += length..   
-00000c20: 2020 2020 2020 2020 2062 6174 6368 6564           batched
-00000c30: 5f74 6167 732e 6170 7065 6e64 2853 7562  _tags.append(Sub
-00000c40: 776f 7264 4261 7365 6454 6167 7328 7475  wordBasedTags(tu
-00000c50: 706c 6528 7461 6773 292c 2074 6578 7429  ple(tags), text)
-00000c60: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00000c70: 6e20 7475 706c 6528 6261 7463 6865 645f  n tuple(batched_
-00000c80: 7461 6773 290a 0a20 2020 2064 6566 2063  tags)..    def c
-00000c90: 7265 6174 655f 7461 675f 696e 6469 6365  reate_tag_indice
-00000ca0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00000cb0: 0a20 2020 2020 2020 2074 6167 735f 636f  .        tags_co
-00000cc0: 6c6c 6563 7469 6f6e 3a20 4368 6172 4261  llection: CharBa
-00000cd0: 7365 6454 6167 7343 6f6c 6c65 6374 696f  sedTagsCollectio
-00000ce0: 6e2c 0a20 2020 2020 2020 2064 6576 6963  n,.        devic
-00000cf0: 653a 2074 6f72 6368 2e64 6576 6963 652c  e: torch.device,
-00000d00: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-00000d10: 5f69 6e64 6578 3a20 696e 7420 3d20 2d31  _index: int = -1
-00000d20: 2c0a 2020 2020 2020 2020 756e 6b6e 6f77  ,.        unknow
-00000d30: 6e5f 696e 6465 783a 2069 6e74 203d 202d  n_index: int = -
-00000d40: 3130 302c 0a20 2020 2029 202d 3e20 746f  100,.    ) -> to
-00000d50: 7263 682e 5465 6e73 6f72 3a0a 2020 2020  rch.Tensor:.    
-00000d60: 2020 2020 7461 675f 696e 6469 6365 7320      tag_indices 
-00000d70: 3d20 5b5d 0a20 2020 2020 2020 206c 6162  = [].        lab
-00000d80: 656c 5f73 6574 203d 2073 656c 662e 5f5f  el_set = self.__
-00000d90: 6c61 6265 6c5f 7365 740a 0a20 2020 2020  label_set..     
-00000da0: 2020 2066 6f72 2074 6578 742c 2074 6167     for text, tag
-00000db0: 7320 696e 207a 6970 2873 656c 662e 5f5f  s in zip(self.__
-00000dc0: 746f 6b65 6e69 7a65 645f 7465 7874 732c  tokenized_texts,
-00000dd0: 2074 6167 735f 636f 6c6c 6563 7469 6f6e   tags_collection
-00000de0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00000df0: 6e64 6963 6573 203d 205b 756e 6b6e 6f77  ndices = [unknow
-00000e00: 6e5f 696e 6465 785d 202a 2074 6578 742e  n_index] * text.
-00000e10: 6e75 6d5f 746f 6b65 6e73 0a0a 2020 2020  num_tokens..    
-00000e20: 2020 2020 2020 2020 666f 7220 746f 6b65          for toke
-00000e30: 6e5f 696e 6465 7820 696e 2072 616e 6765  n_index in range
-00000e40: 2874 6578 742e 6e75 6d5f 746f 6b65 6e73  (text.num_tokens
-00000e50: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00000e60: 2020 2073 7061 6e20 3d20 7465 7874 2e67     span = text.g
-00000e70: 6574 5f63 6861 725f 7370 616e 2874 6f6b  et_char_span(tok
-00000e80: 656e 5f69 6e64 6578 290a 2020 2020 2020  en_index).      
-00000e90: 2020 2020 2020 2020 2020 6966 2073 7061            if spa
-00000ea0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000ec0: 6e64 6963 6573 5b74 6f6b 656e 5f69 6e64  ndices[token_ind
-00000ed0: 6578 5d20 3d20 6c61 6265 6c5f 7365 742e  ex] = label_set.
-00000ee0: 6765 745f 6f75 7473 6964 655f 696e 6465  get_outside_inde
-00000ef0: 7828 290a 0a20 2020 2020 2020 2020 2020  x()..           
-00000f00: 2066 6f72 2074 6167 2069 6e20 7461 6773   for tag in tags
-00000f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000f20: 2020 7374 6172 7420 3d20 7465 7874 2e63    start = text.c
-00000f30: 6f6e 7665 7274 5f74 6f5f 746f 6b65 6e5f  onvert_to_token_
-00000f40: 696e 6465 7828 7461 672e 7374 6172 7429  index(tag.start)
-00000f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000f60: 2065 6e64 203d 2074 6578 742e 636f 6e76   end = text.conv
-00000f70: 6572 745f 746f 5f74 6f6b 656e 5f69 6e64  ert_to_token_ind
-00000f80: 6578 2874 6167 2e73 7461 7274 202b 2074  ex(tag.start + t
-00000f90: 6167 2e6c 656e 6774 6820 2d20 3129 0a20  ag.length - 1). 
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000fb0: 6620 7374 6172 7420 3d3d 2065 6e64 3a0a  f start == end:.
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fd0: 2020 2020 696e 6469 6365 735b 7374 6172      indices[star
-00000fe0: 745d 203d 206c 6162 656c 5f73 6574 2e67  t] = label_set.g
-00000ff0: 6574 5f75 6e69 745f 696e 6465 7828 7461  et_unit_index(ta
-00001000: 672e 6c61 6265 6c29 0a20 2020 2020 2020  g.label).       
-00001010: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001030: 2020 2069 6e64 6963 6573 5b73 7461 7274     indices[start
-00001040: 5d20 3d20 6c61 6265 6c5f 7365 742e 6765  ] = label_set.ge
-00001050: 745f 7374 6172 745f 696e 6465 7828 7461  t_start_index(ta
-00001060: 672e 6c61 6265 6c29 0a20 2020 2020 2020  g.label).       
-00001070: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-00001080: 6963 6573 5b73 7461 7274 202b 2031 203a  ices[start + 1 :
-00001090: 2065 6e64 5d20 3d20 5b0a 2020 2020 2020   end] = [.      
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 6c61 6265 6c5f 7365 742e 6765 745f    label_set.get_
-000010c0: 696e 7369 6465 5f69 6e64 6578 2874 6167  inside_index(tag
-000010d0: 2e6c 6162 656c 290a 2020 2020 2020 2020  .label).        
-000010e0: 2020 2020 2020 2020 2020 2020 5d20 2a20              ] * 
-000010f0: 2865 6e64 202d 2073 7461 7274 202d 2031  (end - start - 1
-00001100: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001110: 2020 2020 2020 696e 6469 6365 735b 656e        indices[en
-00001120: 645d 203d 206c 6162 656c 5f73 6574 2e67  d] = label_set.g
-00001130: 6574 5f65 6e64 5f69 6e64 6578 2874 6167  et_end_index(tag
-00001140: 2e6c 6162 656c 290a 0a20 2020 2020 2020  .label)..       
-00001150: 2020 2020 2074 6167 5f69 6e64 6963 6573       tag_indices
-00001160: 2e61 7070 656e 6428 696e 6469 6365 7329  .append(indices)
-00001170: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001180: 2070 6164 2874 6167 5f69 6e64 6963 6573   pad(tag_indices
-00001190: 2c20 7061 6464 696e 675f 696e 6465 7829  , padding_index)
-000011a0: 2e74 6f28 6465 7669 6365 290a 0a20 2020  .to(device)..   
-000011b0: 2064 6566 2063 7265 6174 655f 7461 675f   def create_tag_
-000011c0: 6269 746d 6170 280a 2020 2020 2020 2020  bitmap(.        
-000011d0: 7365 6c66 2c0a 2020 2020 2020 2020 7461  self,.        ta
-000011e0: 6773 5f63 6f6c 6c65 6374 696f 6e3a 2043  gs_collection: C
-000011f0: 6861 7242 6173 6564 5461 6773 436f 6c6c  harBasedTagsColl
-00001200: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
-00001210: 6465 7669 6365 3a20 746f 7263 682e 6465  device: torch.de
-00001220: 7669 6365 2c0a 2020 2020 2020 2020 7061  vice,.        pa
-00001230: 6464 696e 675f 696e 6465 783a 2069 6e74  dding_index: int
-00001240: 203d 202d 312c 0a20 2020 2020 2020 2075   = -1,.        u
-00001250: 6e6b 6e6f 776e 5f69 6e64 6578 3a20 696e  nknown_index: in
-00001260: 7420 3d20 2d31 3030 2c0a 2020 2020 2920  t = -100,.    ) 
-00001270: 2d3e 2074 6f72 6368 2e54 656e 736f 723a  -> torch.Tensor:
-00001280: 0a20 2020 2020 2020 2074 6167 5f69 6e64  .        tag_ind
-00001290: 6963 6573 203d 2073 656c 662e 6372 6561  ices = self.crea
-000012a0: 7465 5f74 6167 5f69 6e64 6963 6573 280a  te_tag_indices(.
-000012b0: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-000012c0: 5f63 6f6c 6c65 6374 696f 6e2c 2064 6576  _collection, dev
-000012d0: 6963 652c 2070 6164 6469 6e67 5f69 6e64  ice, padding_ind
-000012e0: 6578 2c20 756e 6b6e 6f77 6e5f 696e 6465  ex, unknown_inde
-000012f0: 780a 2020 2020 2020 2020 290a 2020 2020  x.        ).    
-00001300: 2020 2020 7265 7475 726e 2074 6f5f 7461      return to_ta
-00001310: 675f 6269 746d 6170 280a 2020 2020 2020  g_bitmap(.      
-00001320: 2020 2020 2020 7461 675f 696e 6469 6365        tag_indice
-00001330: 732c 2073 656c 662e 5f5f 6c61 6265 6c5f  s, self.__label_
-00001340: 7365 742e 6765 745f 7461 675f 7369 7a65  set.get_tag_size
-00001350: 2829 2c20 756e 6b6e 6f77 6e5f 696e 6465  (), unknown_inde
-00001360: 780a 2020 2020 2020 2020 290a 0a0a 636c  x.        )...cl
-00001370: 6173 7320 4261 7463 683a 0a20 2020 2064  ass Batch:.    d
-00001380: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00001390: 2020 2020 2073 656c 662c 2074 6167 6765       self, tagge
-000013a0: 725f 696e 7075 7473 3a20 5461 6767 6572  r_inputs: Tagger
-000013b0: 496e 7075 7473 2c20 6d61 736b 3a20 746f  Inputs, mask: to
-000013c0: 7263 682e 5465 6e73 6f72 2c20 7461 675f  rch.Tensor, tag_
-000013d0: 6661 6374 6f72 793a 2054 6167 4661 6374  factory: TagFact
-000013e0: 6f72 790a 2020 2020 293a 0a20 2020 2020  ory.    ):.     
-000013f0: 2020 2073 656c 662e 5f5f 7461 6767 6572     self.__tagger
-00001400: 5f69 6e70 7574 7320 3d20 7461 6767 6572  _inputs = tagger
-00001410: 5f69 6e70 7574 730a 2020 2020 2020 2020  _inputs.        
-00001420: 7365 6c66 2e5f 5f6d 6173 6b20 3d20 6d61  self.__mask = ma
-00001430: 736b 0a20 2020 2020 2020 2073 656c 662e  sk.        self.
-00001440: 5f5f 7461 675f 6661 6374 6f72 7920 3d20  __tag_factory = 
-00001450: 7461 675f 6661 6374 6f72 790a 0a20 2020  tag_factory..   
-00001460: 2064 6566 2067 6574 5f74 6167 6765 725f   def get_tagger_
-00001470: 696e 7075 7473 2873 656c 662c 2064 6576  inputs(self, dev
+00000000: 6672 6f6d 2061 6263 2069 6d70 6f72 7420  from abc import 
+00000010: 4142 434d 6574 612c 2061 6273 7472 6163  ABCMeta, abstrac
+00000020: 746d 6574 686f 640a 6672 6f6d 2069 7465  tmethod.from ite
+00000030: 7274 6f6f 6c73 2069 6d70 6f72 7420 6772  rtools import gr
+00000040: 6f75 7062 790a 6672 6f6d 2074 7970 696e  oupby.from typin
+00000050: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000060: 6c0a 0a69 6d70 6f72 7420 746f 7263 680a  l..import torch.
+00000070: 6672 6f6d 2074 7261 6e73 666f 726d 6572  from transformer
+00000080: 732e 746f 6b65 6e69 7a61 7469 6f6e 5f75  s.tokenization_u
+00000090: 7469 6c73 2069 6d70 6f72 7420 5072 6554  tils import PreT
+000000a0: 7261 696e 6564 546f 6b65 6e69 7a65 720a  rainedTokenizer.
+000000b0: 0a66 726f 6d20 2e2e 6372 662e 6675 6e63  .from ..crf.func
+000000c0: 7469 6f6e 616c 2069 6d70 6f72 7420 746f  tional import to
+000000d0: 5f74 6167 5f62 6974 6d61 700a 6672 6f6d  _tag_bitmap.from
+000000e0: 202e 2069 6d70 6f72 7420 4368 6172 4261   . import CharBa
+000000f0: 7365 6454 6167 732c 204c 6162 656c 5365  sedTags, LabelSe
+00000100: 742c 2053 7061 6e2c 2053 7562 776f 7264  t, Span, Subword
+00000110: 4261 7365 6454 6167 732c 2054 6167 2c20  BasedTags, Tag, 
+00000120: 546f 6b65 6e69 7a65 6454 6578 740a 0a54  TokenizedText..T
+00000130: 6578 7473 203d 2074 7570 6c65 5b73 7472  exts = tuple[str
+00000140: 2c20 2e2e 2e5d 0a54 6f6b 656e 697a 6564  , ...].Tokenized
+00000150: 5465 7874 7320 3d20 7475 706c 655b 546f  Texts = tuple[To
+00000160: 6b65 6e69 7a65 6454 6578 742c 202e 2e2e  kenizedText, ...
+00000170: 5d0a 0a43 6861 7242 6173 6564 5461 6773  ]..CharBasedTags
+00000180: 436f 6c6c 6563 7469 6f6e 203d 2074 7570  Collection = tup
+00000190: 6c65 5b43 6861 7242 6173 6564 5461 6773  le[CharBasedTags
+000001a0: 2c20 2e2e 2e5d 0a53 7562 776f 7264 4261  , ...].SubwordBa
+000001b0: 7365 6454 6167 7343 6f6c 6c65 6374 696f  sedTagsCollectio
+000001c0: 6e20 3d20 7475 706c 655b 5375 6277 6f72  n = tuple[Subwor
+000001d0: 6442 6173 6564 5461 6773 2c20 2e2e 2e5d  dBasedTags, ...]
+000001e0: 0a0a 4461 7461 7365 7420 3d20 6c69 7374  ..Dataset = list
+000001f0: 5b74 7570 6c65 5b73 7472 2c20 4368 6172  [tuple[str, Char
+00000200: 4261 7365 6454 6167 735d 5d0a 0a54 6167  BasedTags]]..Tag
+00000210: 6765 7249 6e70 7574 7320 3d20 6469 6374  gerInputs = dict
+00000220: 5b73 7472 2c20 746f 7263 682e 5465 6e73  [str, torch.Tens
+00000230: 6f72 5d0a 0a0a 6465 6620 7061 6428 6261  or]...def pad(ba
+00000240: 7463 683a 206c 6973 745b 6c69 7374 5b69  tch: list[list[i
+00000250: 6e74 5d5d 2c20 6669 6c6c 5f76 616c 7565  nt]], fill_value
+00000260: 3a20 696e 7429 202d 3e20 746f 7263 682e  : int) -> torch.
+00000270: 5465 6e73 6f72 3a0a 2020 2020 6d61 785f  Tensor:.    max_
+00000280: 6c65 6e67 7468 203d 206d 6178 286d 6170  length = max(map
+00000290: 286c 656e 2c20 6261 7463 6829 290a 2020  (len, batch)).  
+000002a0: 2020 7265 7475 726e 2074 6f72 6368 2e74    return torch.t
+000002b0: 656e 736f 7228 5b78 202b 205b 6669 6c6c  ensor([x + [fill
+000002c0: 5f76 616c 7565 5d20 2a20 286d 6178 5f6c  _value] * (max_l
+000002d0: 656e 6774 6820 2d20 6c65 6e28 7829 2920  ength - len(x)) 
+000002e0: 666f 7220 7820 696e 2062 6174 6368 5d29  for x in batch])
+000002f0: 0a0a 0a64 6566 2075 6e70 6164 2862 6174  ...def unpad(bat
+00000300: 6368 3a20 746f 7263 682e 5465 6e73 6f72  ch: torch.Tensor
+00000310: 2c20 6669 6c6c 5f76 616c 7565 3a20 696e  , fill_value: in
+00000320: 7429 202d 3e20 6c69 7374 5b6c 6973 745b  t) -> list[list[
+00000330: 696e 745d 5d3a 0a20 2020 2072 6574 7572  int]]:.    retur
+00000340: 6e20 5b5b 6920 666f 7220 6920 696e 2078  n [[i for i in x
+00000350: 2069 6620 6920 213d 2066 696c 6c5f 7661   if i != fill_va
+00000360: 6c75 655d 2066 6f72 2078 2069 6e20 6261  lue] for x in ba
+00000370: 7463 682e 746f 6c69 7374 2829 5d0a 0a0a  tch.tolist()]...
+00000380: 636c 6173 7320 5461 6746 6163 746f 7279  class TagFactory
+00000390: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000003a0: 5f5f 2873 656c 662c 2074 6f6b 656e 697a  __(self, tokeniz
+000003b0: 6564 5f74 6578 7473 3a20 546f 6b65 6e69  ed_texts: Tokeni
+000003c0: 7a65 6454 6578 7473 2c20 6c61 6265 6c5f  zedTexts, label_
+000003d0: 7365 743a 204c 6162 656c 5365 7429 3a0a  set: LabelSet):.
+000003e0: 2020 2020 2020 2020 7365 6c66 2e5f 5f74          self.__t
+000003f0: 6f6b 656e 697a 6564 5f74 6578 7473 203d  okenized_texts =
+00000400: 2074 6f6b 656e 697a 6564 5f74 6578 7473   tokenized_texts
+00000410: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00000420: 6c61 6265 6c5f 7365 7420 3d20 6c61 6265  label_set = labe
+00000430: 6c5f 7365 740a 0a20 2020 2040 7072 6f70  l_set..    @prop
+00000440: 6572 7479 0a20 2020 2064 6566 2074 6f6b  erty.    def tok
+00000450: 656e 697a 6564 5f74 6578 7473 2873 656c  enized_texts(sel
+00000460: 6629 202d 3e20 546f 6b65 6e69 7a65 6454  f) -> TokenizedT
+00000470: 6578 7473 3a0a 2020 2020 2020 2020 7265  exts:.        re
+00000480: 7475 726e 2073 656c 662e 5f5f 746f 6b65  turn self.__toke
+00000490: 6e69 7a65 645f 7465 7874 730a 0a20 2020  nized_texts..   
+000004a0: 2064 6566 2063 7265 6174 655f 6368 6172   def create_char
+000004b0: 5f62 6173 6564 5f74 6167 7328 0a20 2020  _based_tags(.   
+000004c0: 2020 2020 2073 656c 662c 2074 6167 5f69       self, tag_i
+000004d0: 6e64 6963 6573 3a20 746f 7263 682e 5465  ndices: torch.Te
+000004e0: 6e73 6f72 2c20 7061 6464 696e 675f 696e  nsor, padding_in
+000004f0: 6465 783a 2069 6e74 203d 202d 310a 2020  dex: int = -1.  
+00000500: 2020 2920 2d3e 2043 6861 7242 6173 6564    ) -> CharBased
+00000510: 5461 6773 436f 6c6c 6563 7469 6f6e 3a0a  TagsCollection:.
+00000520: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00000530: 7570 6c65 280a 2020 2020 2020 2020 2020  uple(.          
+00000540: 2020 7461 6773 2e67 6574 5f63 6861 725f    tags.get_char_
+00000550: 6261 7365 645f 7461 6773 2829 0a20 2020  based_tags().   
+00000560: 2020 2020 2020 2020 2066 6f72 2074 6167           for tag
+00000570: 7320 696e 2073 656c 662e 6372 6561 7465  s in self.create
+00000580: 5f73 7562 776f 7264 5f62 6173 6564 5f74  _subword_based_t
+00000590: 6167 7328 7461 675f 696e 6469 6365 732c  ags(tag_indices,
+000005a0: 2070 6164 6469 6e67 5f69 6e64 6578 290a   padding_index).
+000005b0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000005c0: 6566 2063 7265 6174 655f 7375 6277 6f72  ef create_subwor
+000005d0: 645f 6261 7365 645f 7461 6773 280a 2020  d_based_tags(.  
+000005e0: 2020 2020 2020 7365 6c66 2c20 7461 675f        self, tag_
+000005f0: 696e 6469 6365 733a 2074 6f72 6368 2e54  indices: torch.T
+00000600: 656e 736f 722c 2070 6164 6469 6e67 5f69  ensor, padding_i
+00000610: 6e64 6578 3a20 696e 7420 3d20 2d31 0a20  ndex: int = -1. 
+00000620: 2020 2029 202d 3e20 5375 6277 6f72 6442     ) -> SubwordB
+00000630: 6173 6564 5461 6773 436f 6c6c 6563 7469  asedTagsCollecti
+00000640: 6f6e 3a0a 2020 2020 2020 2020 6c61 6265  on:.        labe
+00000650: 6c5f 7365 7420 3d20 7365 6c66 2e5f 5f6c  l_set = self.__l
+00000660: 6162 656c 5f73 6574 0a0a 2020 2020 2020  abel_set..      
+00000670: 2020 6261 7463 6865 645f 7461 6773 203d    batched_tags =
+00000680: 205b 5d0a 0a20 2020 2020 2020 2066 6f72   []..        for
+00000690: 2074 6578 742c 2069 6e64 6963 6573 2069   text, indices i
+000006a0: 6e20 7a69 7028 0a20 2020 2020 2020 2020  n zip(.         
+000006b0: 2020 2073 656c 662e 5f5f 746f 6b65 6e69     self.__tokeni
+000006c0: 7a65 645f 7465 7874 732c 2075 6e70 6164  zed_texts, unpad
+000006d0: 2874 6167 5f69 6e64 6963 6573 2c20 7061  (tag_indices, pa
+000006e0: 6464 696e 675f 696e 6465 7829 2c20 7374  dding_index), st
+000006f0: 7269 6374 3d54 7275 650a 2020 2020 2020  rict=True.      
+00000700: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+00000710: 2074 6167 7320 3d20 5b5d 0a20 2020 2020   tags = [].     
+00000720: 2020 2020 2020 206e 6f77 203d 2030 0a20         now = 0. 
+00000730: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+00000740: 6162 656c 2c20 6772 6f75 7020 696e 2067  abel, group in g
+00000750: 726f 7570 6279 280a 2020 2020 2020 2020  roupby(.        
+00000760: 2020 2020 2020 2020 6c61 6265 6c5f 7365          label_se
+00000770: 742e 6765 745f 6c61 6265 6c28 696e 6465  t.get_label(inde
+00000780: 7829 2066 6f72 2069 6e64 6578 2069 6e20  x) for index in 
+00000790: 696e 6469 6365 730a 2020 2020 2020 2020  indices.        
+000007a0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000007b0: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
+000007c0: 6c65 6e28 6c69 7374 2867 726f 7570 2929  len(list(group))
+000007d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000007e0: 2020 6966 206c 6162 656c 2069 7320 6e6f    if label is no
+000007f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00000800: 2020 2020 2020 2020 2020 2020 7461 6773              tags
+00000810: 2e61 7070 656e 6428 5461 6728 5370 616e  .append(Tag(Span
+00000820: 286e 6f77 2c20 6c65 6e67 7468 292c 206c  (now, length), l
+00000830: 6162 656c 2929 0a0a 2020 2020 2020 2020  abel))..        
+00000840: 2020 2020 2020 2020 6e6f 7720 2b3d 206c          now += l
+00000850: 656e 6774 680a 0a20 2020 2020 2020 2020  ength..         
+00000860: 2020 2062 6174 6368 6564 5f74 6167 732e     batched_tags.
+00000870: 6170 7065 6e64 2853 7562 776f 7264 4261  append(SubwordBa
+00000880: 7365 6454 6167 7328 7475 706c 6528 7461  sedTags(tuple(ta
+00000890: 6773 292c 2074 6578 7429 290a 0a20 2020  gs), text))..   
+000008a0: 2020 2020 2072 6574 7572 6e20 7475 706c       return tupl
+000008b0: 6528 6261 7463 6865 645f 7461 6773 290a  e(batched_tags).
+000008c0: 0a20 2020 2064 6566 2063 7265 6174 655f  .    def create_
+000008d0: 7461 675f 696e 6469 6365 7328 0a20 2020  tag_indices(.   
+000008e0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000008f0: 2020 2074 6167 735f 636f 6c6c 6563 7469     tags_collecti
+00000900: 6f6e 3a20 4368 6172 4261 7365 6454 6167  on: CharBasedTag
+00000910: 7343 6f6c 6c65 6374 696f 6e2c 0a20 2020  sCollection,.   
+00000920: 2020 2020 2064 6576 6963 653a 2074 6f72       device: tor
+00000930: 6368 2e64 6576 6963 652c 0a20 2020 2020  ch.device,.     
+00000940: 2020 2070 6164 6469 6e67 5f69 6e64 6578     padding_index
+00000950: 3a20 696e 7420 3d20 2d31 2c0a 2020 2020  : int = -1,.    
+00000960: 2020 2020 756e 6b6e 6f77 6e5f 696e 6465      unknown_inde
+00000970: 783a 2069 6e74 203d 202d 3130 302c 0a20  x: int = -100,. 
+00000980: 2020 2029 202d 3e20 746f 7263 682e 5465     ) -> torch.Te
+00000990: 6e73 6f72 3a0a 2020 2020 2020 2020 7461  nsor:.        ta
+000009a0: 675f 696e 6469 6365 7320 3d20 5b5d 0a20  g_indices = []. 
+000009b0: 2020 2020 2020 206c 6162 656c 5f73 6574         label_set
+000009c0: 203d 2073 656c 662e 5f5f 6c61 6265 6c5f   = self.__label_
+000009d0: 7365 740a 0a20 2020 2020 2020 2066 6f72  set..        for
+000009e0: 2074 6578 742c 2074 6167 7320 696e 207a   text, tags in z
+000009f0: 6970 2873 656c 662e 5f5f 746f 6b65 6e69  ip(self.__tokeni
+00000a00: 7a65 645f 7465 7874 732c 2074 6167 735f  zed_texts, tags_
+00000a10: 636f 6c6c 6563 7469 6f6e 2c20 7374 7269  collection, stri
+00000a20: 6374 3d54 7275 6529 3a0a 2020 2020 2020  ct=True):.      
+00000a30: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+00000a40: 5b75 6e6b 6e6f 776e 5f69 6e64 6578 5d20  [unknown_index] 
+00000a50: 2a20 7465 7874 2e6e 756d 5f74 6f6b 656e  * text.num_token
+00000a60: 730a 0a20 2020 2020 2020 2020 2020 2066  s..            f
+00000a70: 6f72 2074 6f6b 656e 5f69 6e64 6578 2069  or token_index i
+00000a80: 6e20 7261 6e67 6528 7465 7874 2e6e 756d  n range(text.num
+00000a90: 5f74 6f6b 656e 7329 3a0a 2020 2020 2020  _tokens):.      
+00000aa0: 2020 2020 2020 2020 2020 7370 616e 203d            span =
+00000ab0: 2074 6578 742e 6765 745f 6368 6172 5f73   text.get_char_s
+00000ac0: 7061 6e28 746f 6b65 6e5f 696e 6465 7829  pan(token_index)
+00000ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ae0: 2069 6620 7370 616e 2069 7320 4e6f 6e65   if span is None
+00000af0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000b00: 2020 2020 2020 696e 6469 6365 735b 746f        indices[to
+00000b10: 6b65 6e5f 696e 6465 785d 203d 206c 6162  ken_index] = lab
+00000b20: 656c 5f73 6574 2e67 6574 5f6f 7574 7369  el_set.get_outsi
+00000b30: 6465 5f69 6e64 6578 2829 0a0a 2020 2020  de_index()..    
+00000b40: 2020 2020 2020 2020 666f 7220 7461 6720          for tag 
+00000b50: 696e 2074 6167 733a 0a20 2020 2020 2020  in tags:.       
+00000b60: 2020 2020 2020 2020 2073 7461 7274 203d           start =
+00000b70: 2074 6578 742e 636f 6e76 6572 745f 746f   text.convert_to
+00000b80: 5f74 6f6b 656e 5f69 6e64 6578 2874 6167  _token_index(tag
+00000b90: 2e73 7461 7274 290a 2020 2020 2020 2020  .start).        
+00000ba0: 2020 2020 2020 2020 656e 6420 3d20 7465          end = te
+00000bb0: 7874 2e63 6f6e 7665 7274 5f74 6f5f 746f  xt.convert_to_to
+00000bc0: 6b65 6e5f 696e 6465 7828 7461 672e 7374  ken_index(tag.st
+00000bd0: 6172 7420 2b20 7461 672e 6c65 6e67 7468  art + tag.length
+00000be0: 202d 2031 290a 2020 2020 2020 2020 2020   - 1).          
+00000bf0: 2020 2020 2020 6966 2073 7461 7274 203d        if start =
+00000c00: 3d20 656e 643a 0a20 2020 2020 2020 2020  = end:.         
+00000c10: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+00000c20: 6573 5b73 7461 7274 5d20 3d20 6c61 6265  es[start] = labe
+00000c30: 6c5f 7365 742e 6765 745f 756e 6974 5f69  l_set.get_unit_i
+00000c40: 6e64 6578 2874 6167 2e6c 6162 656c 290a  ndex(tag.label).
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000c70: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00000c80: 735b 7374 6172 745d 203d 206c 6162 656c  s[start] = label
+00000c90: 5f73 6574 2e67 6574 5f73 7461 7274 5f69  _set.get_start_i
+00000ca0: 6e64 6578 2874 6167 2e6c 6162 656c 290a  ndex(tag.label).
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 2020 2020 696e 6469 6365 735b 7374 6172      indices[star
+00000cd0: 7420 2b20 3120 3a20 656e 645d 203d 205b  t + 1 : end] = [
+00000ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cf0: 2020 2020 2020 2020 206c 6162 656c 5f73           label_s
+00000d00: 6574 2e67 6574 5f69 6e73 6964 655f 696e  et.get_inside_in
+00000d10: 6465 7828 7461 672e 6c61 6265 6c29 0a20  dex(tag.label). 
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 2020 205d 202a 2028 656e 6420 2d20 7374     ] * (end - st
+00000d40: 6172 7420 2d20 3129 0a20 2020 2020 2020  art - 1).       
+00000d50: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00000d60: 6963 6573 5b65 6e64 5d20 3d20 6c61 6265  ices[end] = labe
+00000d70: 6c5f 7365 742e 6765 745f 656e 645f 696e  l_set.get_end_in
+00000d80: 6465 7828 7461 672e 6c61 6265 6c29 0a0a  dex(tag.label)..
+00000d90: 2020 2020 2020 2020 2020 2020 7461 675f              tag_
+00000da0: 696e 6469 6365 732e 6170 7065 6e64 2869  indices.append(i
+00000db0: 6e64 6963 6573 290a 0a20 2020 2020 2020  ndices)..       
+00000dc0: 2072 6574 7572 6e20 7061 6428 7461 675f   return pad(tag_
+00000dd0: 696e 6469 6365 732c 2070 6164 6469 6e67  indices, padding
+00000de0: 5f69 6e64 6578 292e 746f 2864 6576 6963  _index).to(devic
+00000df0: 6529 0a0a 2020 2020 6465 6620 6372 6561  e)..    def crea
+00000e00: 7465 5f74 6167 5f62 6974 6d61 7028 0a20  te_tag_bitmap(. 
+00000e10: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00000e20: 2020 2020 2074 6167 735f 636f 6c6c 6563       tags_collec
+00000e30: 7469 6f6e 3a20 4368 6172 4261 7365 6454  tion: CharBasedT
+00000e40: 6167 7343 6f6c 6c65 6374 696f 6e2c 0a20  agsCollection,. 
+00000e50: 2020 2020 2020 2064 6576 6963 653a 2074         device: t
+00000e60: 6f72 6368 2e64 6576 6963 652c 0a20 2020  orch.device,.   
+00000e70: 2020 2020 2070 6164 6469 6e67 5f69 6e64       padding_ind
+00000e80: 6578 3a20 696e 7420 3d20 2d31 2c0a 2020  ex: int = -1,.  
+00000e90: 2020 2020 2020 756e 6b6e 6f77 6e5f 696e        unknown_in
+00000ea0: 6465 783a 2069 6e74 203d 202d 3130 302c  dex: int = -100,
+00000eb0: 0a20 2020 2029 202d 3e20 746f 7263 682e  .    ) -> torch.
+00000ec0: 5465 6e73 6f72 3a0a 2020 2020 2020 2020  Tensor:.        
+00000ed0: 7461 675f 696e 6469 6365 7320 3d20 7365  tag_indices = se
+00000ee0: 6c66 2e63 7265 6174 655f 7461 675f 696e  lf.create_tag_in
+00000ef0: 6469 6365 7328 0a20 2020 2020 2020 2020  dices(.         
+00000f00: 2020 2074 6167 735f 636f 6c6c 6563 7469     tags_collecti
+00000f10: 6f6e 2c20 6465 7669 6365 2c20 7061 6464  on, device, padd
+00000f20: 696e 675f 696e 6465 782c 2075 6e6b 6e6f  ing_index, unkno
+00000f30: 776e 5f69 6e64 6578 0a20 2020 2020 2020  wn_index.       
+00000f40: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+00000f50: 6e20 746f 5f74 6167 5f62 6974 6d61 7028  n to_tag_bitmap(
+00000f60: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
+00000f70: 5f69 6e64 6963 6573 2c20 7365 6c66 2e5f  _indices, self._
+00000f80: 5f6c 6162 656c 5f73 6574 2e67 6574 5f74  _label_set.get_t
+00000f90: 6167 5f73 697a 6528 292c 2075 6e6b 6e6f  ag_size(), unkno
+00000fa0: 776e 5f69 6e64 6578 0a20 2020 2020 2020  wn_index.       
+00000fb0: 2029 0a0a 0a63 6c61 7373 2042 6174 6368   )...class Batch
+00000fc0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00000fd0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00000fe0: 2c20 7461 6767 6572 5f69 6e70 7574 733a  , tagger_inputs:
+00000ff0: 2054 6167 6765 7249 6e70 7574 732c 206d   TaggerInputs, m
+00001000: 6173 6b3a 2074 6f72 6368 2e54 656e 736f  ask: torch.Tenso
+00001010: 722c 2074 6167 5f66 6163 746f 7279 3a20  r, tag_factory: 
+00001020: 5461 6746 6163 746f 7279 0a20 2020 2029  TagFactory.    )
+00001030: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00001040: 5f74 6167 6765 725f 696e 7075 7473 203d  _tagger_inputs =
+00001050: 2074 6167 6765 725f 696e 7075 7473 0a20   tagger_inputs. 
+00001060: 2020 2020 2020 2073 656c 662e 5f5f 6d61         self.__ma
+00001070: 736b 203d 206d 6173 6b0a 2020 2020 2020  sk = mask.      
+00001080: 2020 7365 6c66 2e5f 5f74 6167 5f66 6163    self.__tag_fac
+00001090: 746f 7279 203d 2074 6167 5f66 6163 746f  tory = tag_facto
+000010a0: 7279 0a0a 2020 2020 6465 6620 6765 745f  ry..    def get_
+000010b0: 7461 6767 6572 5f69 6e70 7574 7328 7365  tagger_inputs(se
+000010c0: 6c66 2c20 6465 7669 6365 3a20 746f 7263  lf, device: torc
+000010d0: 682e 6465 7669 6365 2920 2d3e 2054 6167  h.device) -> Tag
+000010e0: 6765 7249 6e70 7574 733a 0a20 2020 2020  gerInputs:.     
+000010f0: 2020 2072 6574 7572 6e20 7b6b 6579 3a20     return {key: 
+00001100: 782e 746f 2864 6576 6963 6529 2066 6f72  x.to(device) for
+00001110: 206b 6579 2c20 7820 696e 2073 656c 662e   key, x in self.
+00001120: 5f5f 7461 6767 6572 5f69 6e70 7574 732e  __tagger_inputs.
+00001130: 6974 656d 7328 297d 0a0a 2020 2020 6465  items()}..    de
+00001140: 6620 6765 745f 6d61 736b 2873 656c 662c  f get_mask(self,
+00001150: 2064 6576 6963 653a 2074 6f72 6368 2e64   device: torch.d
+00001160: 6576 6963 6529 202d 3e20 746f 7263 682e  evice) -> torch.
+00001170: 5465 6e73 6f72 3a0a 2020 2020 2020 2020  Tensor:.        
+00001180: 7265 7475 726e 2073 656c 662e 5f5f 6d61  return self.__ma
+00001190: 736b 2e74 6f28 6465 7669 6365 290a 0a20  sk.to(device).. 
+000011a0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000011b0: 2064 6566 2074 6f6b 656e 697a 6564 5f74   def tokenized_t
+000011c0: 6578 7473 2873 656c 6629 202d 3e20 546f  exts(self) -> To
+000011d0: 6b65 6e69 7a65 6454 6578 7473 3a0a 2020  kenizedTexts:.  
+000011e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000011f0: 662e 5f5f 7461 675f 6661 6374 6f72 792e  f.__tag_factory.
+00001200: 746f 6b65 6e69 7a65 645f 7465 7874 730a  tokenized_texts.
+00001210: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00001220: 2020 2064 6566 2073 697a 6528 7365 6c66     def size(self
+00001230: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+00001240: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00001250: 6d61 736b 2e73 697a 6528 3029 0a0a 2020  mask.size(0)..  
+00001260: 2020 6465 6620 6372 6561 7465 5f63 6861    def create_cha
+00001270: 725f 6261 7365 645f 7461 6773 280a 2020  r_based_tags(.  
+00001280: 2020 2020 2020 7365 6c66 2c20 7461 675f        self, tag_
+00001290: 696e 6469 6365 733a 2074 6f72 6368 2e54  indices: torch.T
+000012a0: 656e 736f 722c 2070 6164 6469 6e67 5f69  ensor, padding_i
+000012b0: 6e64 6578 3a20 696e 7420 3d20 2d31 0a20  ndex: int = -1. 
+000012c0: 2020 2029 202d 3e20 4368 6172 4261 7365     ) -> CharBase
+000012d0: 6454 6167 7343 6f6c 6c65 6374 696f 6e3a  dTagsCollection:
+000012e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000012f0: 7365 6c66 2e5f 5f74 6167 5f66 6163 746f  self.__tag_facto
+00001300: 7279 2e63 7265 6174 655f 6368 6172 5f62  ry.create_char_b
+00001310: 6173 6564 5f74 6167 7328 7461 675f 696e  ased_tags(tag_in
+00001320: 6469 6365 732c 2070 6164 6469 6e67 5f69  dices, padding_i
+00001330: 6e64 6578 290a 0a20 2020 2064 6566 2063  ndex)..    def c
+00001340: 7265 6174 655f 7375 6277 6f72 645f 6261  reate_subword_ba
+00001350: 7365 645f 7461 6773 280a 2020 2020 2020  sed_tags(.      
+00001360: 2020 7365 6c66 2c20 7461 675f 696e 6469    self, tag_indi
+00001370: 6365 733a 2074 6f72 6368 2e54 656e 736f  ces: torch.Tenso
+00001380: 722c 2070 6164 6469 6e67 5f69 6e64 6578  r, padding_index
+00001390: 3a20 696e 7420 3d20 2d31 0a20 2020 2029  : int = -1.    )
+000013a0: 202d 3e20 5375 6277 6f72 6442 6173 6564   -> SubwordBased
+000013b0: 5461 6773 436f 6c6c 6563 7469 6f6e 3a0a  TagsCollection:.
+000013c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000013d0: 656c 662e 5f5f 7461 675f 6661 6374 6f72  elf.__tag_factor
+000013e0: 792e 6372 6561 7465 5f73 7562 776f 7264  y.create_subword
+000013f0: 5f62 6173 6564 5f74 6167 7328 7461 675f  _based_tags(tag_
+00001400: 696e 6469 6365 732c 2070 6164 6469 6e67  indices, padding
+00001410: 5f69 6e64 6578 290a 0a20 2020 2064 6566  _index)..    def
+00001420: 2063 7265 6174 655f 7461 675f 696e 6469   create_tag_indi
+00001430: 6365 7328 0a20 2020 2020 2020 2073 656c  ces(.        sel
+00001440: 662c 0a20 2020 2020 2020 2074 6167 735f  f,.        tags_
+00001450: 636f 6c6c 6563 7469 6f6e 3a20 4368 6172  collection: Char
+00001460: 4261 7365 6454 6167 7343 6f6c 6c65 6374  BasedTagsCollect
+00001470: 696f 6e2c 0a20 2020 2020 2020 2064 6576  ion,.        dev
 00001480: 6963 653a 2074 6f72 6368 2e64 6576 6963  ice: torch.devic
-00001490: 6529 202d 3e20 5461 6767 6572 496e 7075  e) -> TaggerInpu
-000014a0: 7473 3a0a 2020 2020 2020 2020 7265 7475  ts:.        retu
-000014b0: 726e 207b 6b65 793a 2078 2e74 6f28 6465  rn {key: x.to(de
-000014c0: 7669 6365 2920 666f 7220 6b65 792c 2078  vice) for key, x
-000014d0: 2069 6e20 7365 6c66 2e5f 5f74 6167 6765   in self.__tagge
-000014e0: 725f 696e 7075 7473 2e69 7465 6d73 2829  r_inputs.items()
-000014f0: 7d0a 0a20 2020 2064 6566 2067 6574 5f6d  }..    def get_m
-00001500: 6173 6b28 7365 6c66 2c20 6465 7669 6365  ask(self, device
-00001510: 3a20 746f 7263 682e 6465 7669 6365 2920  : torch.device) 
-00001520: 2d3e 2074 6f72 6368 2e54 656e 736f 723a  -> torch.Tensor:
-00001530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001540: 7365 6c66 2e5f 5f6d 6173 6b2e 746f 2864  self.__mask.to(d
-00001550: 6576 6963 6529 0a0a 2020 2020 4070 726f  evice)..    @pro
-00001560: 7065 7274 790a 2020 2020 6465 6620 746f  perty.    def to
-00001570: 6b65 6e69 7a65 645f 7465 7874 7328 7365  kenized_texts(se
-00001580: 6c66 2920 2d3e 2054 6f6b 656e 697a 6564  lf) -> Tokenized
-00001590: 5465 7874 733a 0a20 2020 2020 2020 2072  Texts:.        r
-000015a0: 6574 7572 6e20 7365 6c66 2e5f 5f74 6167  eturn self.__tag
-000015b0: 5f66 6163 746f 7279 2e74 6f6b 656e 697a  _factory.tokeniz
-000015c0: 6564 5f74 6578 7473 0a0a 2020 2020 4070  ed_texts..    @p
-000015d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000015e0: 7369 7a65 2873 656c 6629 202d 3e20 696e  size(self) -> in
-000015f0: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
-00001600: 6e20 7365 6c66 2e5f 5f6d 6173 6b2e 7369  n self.__mask.si
-00001610: 7a65 2830 290a 0a20 2020 2064 6566 2063  ze(0)..    def c
-00001620: 7265 6174 655f 6368 6172 5f62 6173 6564  reate_char_based
-00001630: 5f74 6167 7328 0a20 2020 2020 2020 2073  _tags(.        s
-00001640: 656c 662c 2074 6167 5f69 6e64 6963 6573  elf, tag_indices
-00001650: 3a20 746f 7263 682e 5465 6e73 6f72 2c20  : torch.Tensor, 
-00001660: 7061 6464 696e 675f 696e 6465 783a 2069  padding_index: i
-00001670: 6e74 203d 202d 310a 2020 2020 2920 2d3e  nt = -1.    ) ->
-00001680: 2043 6861 7242 6173 6564 5461 6773 436f   CharBasedTagsCo
-00001690: 6c6c 6563 7469 6f6e 3a0a 2020 2020 2020  llection:.      
-000016a0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-000016b0: 7461 675f 6661 6374 6f72 792e 6372 6561  tag_factory.crea
-000016c0: 7465 5f63 6861 725f 6261 7365 645f 7461  te_char_based_ta
-000016d0: 6773 2874 6167 5f69 6e64 6963 6573 2c20  gs(tag_indices, 
-000016e0: 7061 6464 696e 675f 696e 6465 7829 0a0a  padding_index)..
-000016f0: 2020 2020 6465 6620 6372 6561 7465 5f73      def create_s
-00001700: 7562 776f 7264 5f62 6173 6564 5f74 6167  ubword_based_tag
-00001710: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00001720: 2074 6167 5f69 6e64 6963 6573 3a20 746f   tag_indices: to
-00001730: 7263 682e 5465 6e73 6f72 2c20 7061 6464  rch.Tensor, padd
-00001740: 696e 675f 696e 6465 783a 2069 6e74 203d  ing_index: int =
-00001750: 202d 310a 2020 2020 2920 2d3e 2053 7562   -1.    ) -> Sub
-00001760: 776f 7264 4261 7365 6454 6167 7343 6f6c  wordBasedTagsCol
-00001770: 6c65 6374 696f 6e3a 0a20 2020 2020 2020  lection:.       
-00001780: 2072 6574 7572 6e20 7365 6c66 2e5f 5f74   return self.__t
-00001790: 6167 5f66 6163 746f 7279 2e63 7265 6174  ag_factory.creat
-000017a0: 655f 7375 6277 6f72 645f 6261 7365 645f  e_subword_based_
-000017b0: 7461 6773 2874 6167 5f69 6e64 6963 6573  tags(tag_indices
-000017c0: 2c20 7061 6464 696e 675f 696e 6465 7829  , padding_index)
-000017d0: 0a0a 2020 2020 6465 6620 6372 6561 7465  ..    def create
-000017e0: 5f74 6167 5f69 6e64 6963 6573 280a 2020  _tag_indices(.  
-000017f0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00001800: 2020 2020 7461 6773 5f63 6f6c 6c65 6374      tags_collect
-00001810: 696f 6e3a 2043 6861 7242 6173 6564 5461  ion: CharBasedTa
-00001820: 6773 436f 6c6c 6563 7469 6f6e 2c0a 2020  gsCollection,.  
-00001830: 2020 2020 2020 6465 7669 6365 3a20 746f        device: to
-00001840: 7263 682e 6465 7669 6365 2c0a 2020 2020  rch.device,.    
-00001850: 2020 2020 7061 6464 696e 675f 696e 6465      padding_inde
-00001860: 783a 2069 6e74 203d 202d 312c 0a20 2020  x: int = -1,.   
-00001870: 2020 2020 2075 6e6b 6e6f 776e 5f69 6e64       unknown_ind
-00001880: 6578 3a20 696e 7420 3d20 2d31 3030 2c0a  ex: int = -100,.
-00001890: 2020 2020 2920 2d3e 2074 6f72 6368 2e54      ) -> torch.T
-000018a0: 656e 736f 723a 0a20 2020 2020 2020 2072  ensor:.        r
-000018b0: 6574 7572 6e20 7365 6c66 2e5f 5f74 6167  eturn self.__tag
-000018c0: 5f66 6163 746f 7279 2e63 7265 6174 655f  _factory.create_
-000018d0: 7461 675f 696e 6469 6365 7328 0a20 2020  tag_indices(.   
-000018e0: 2020 2020 2020 2020 2074 6167 735f 636f           tags_co
-000018f0: 6c6c 6563 7469 6f6e 2c20 6465 7669 6365  llection, device
-00001900: 2c20 7061 6464 696e 675f 696e 6465 782c  , padding_index,
-00001910: 2075 6e6b 6e6f 776e 5f69 6e64 6578 0a20   unknown_index. 
-00001920: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00001930: 6620 6372 6561 7465 5f74 6167 5f62 6974  f create_tag_bit
-00001940: 6d61 7028 0a20 2020 2020 2020 2073 656c  map(.        sel
-00001950: 662c 0a20 2020 2020 2020 2074 6167 735f  f,.        tags_
-00001960: 636f 6c6c 6563 7469 6f6e 3a20 4368 6172  collection: Char
-00001970: 4261 7365 6454 6167 7343 6f6c 6c65 6374  BasedTagsCollect
-00001980: 696f 6e2c 0a20 2020 2020 2020 2064 6576  ion,.        dev
-00001990: 6963 653a 2074 6f72 6368 2e64 6576 6963  ice: torch.devic
-000019a0: 652c 0a20 2020 2020 2020 2070 6164 6469  e,.        paddi
-000019b0: 6e67 5f69 6e64 6578 3a20 696e 7420 3d20  ng_index: int = 
-000019c0: 2d31 2c0a 2020 2020 2020 2020 756e 6b6e  -1,.        unkn
-000019d0: 6f77 6e5f 696e 6465 783a 2069 6e74 203d  own_index: int =
-000019e0: 202d 3130 302c 0a20 2020 2029 202d 3e20   -100,.    ) -> 
-000019f0: 746f 7263 682e 5465 6e73 6f72 3a0a 2020  torch.Tensor:.  
-00001a00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001a10: 662e 5f5f 7461 675f 6661 6374 6f72 792e  f.__tag_factory.
-00001a20: 6372 6561 7465 5f74 6167 5f62 6974 6d61  create_tag_bitma
-00001a30: 7028 0a20 2020 2020 2020 2020 2020 2074  p(.            t
-00001a40: 6167 735f 636f 6c6c 6563 7469 6f6e 2c20  ags_collection, 
-00001a50: 6465 7669 6365 2c20 7061 6464 696e 675f  device, padding_
-00001a60: 696e 6465 782c 2075 6e6b 6e6f 776e 5f69  index, unknown_i
-00001a70: 6e64 6578 0a20 2020 2020 2020 2029 0a0a  ndex.        )..
-00001a80: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00001a90: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-00001aa0: 2020 2020 2020 2074 6578 745f 7374 7220         text_str 
-00001ab0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-00001ac0: 2074 6578 7420 696e 2073 656c 662e 746f   text in self.to
-00001ad0: 6b65 6e69 7a65 645f 7465 7874 733a 0a20  kenized_texts:. 
-00001ae0: 2020 2020 2020 2020 2020 2074 6578 745f             text_
-00001af0: 7374 722e 6170 7065 6e64 2866 2220 2020  str.append(f"   
-00001b00: 202d 207b 7265 7072 2874 6578 7429 7d5c   - {repr(text)}\
-00001b10: 6e22 290a 2020 2020 2020 2020 7265 7475  n").        retu
-00001b20: 726e 2022 4261 7463 683a 5c6e 2220 2b20  rn "Batch:\n" + 
-00001b30: 6622 2020 7369 7a65 3a20 7b73 656c 662e  f"  size: {self.
-00001b40: 7369 7a65 7d5c 6e22 202b 2022 2020 6461  size}\n" + "  da
-00001b50: 7461 3a5c 6e22 202b 2022 222e 6a6f 696e  ta:\n" + "".join
-00001b60: 2874 6578 745f 7374 7229 0a0a 0a63 6c61  (text_str)...cla
-00001b70: 7373 2042 6173 6542 6174 6368 4661 6374  ss BaseBatchFact
-00001b80: 6f72 7928 6d65 7461 636c 6173 733d 4142  ory(metaclass=AB
-00001b90: 434d 6574 6129 3a0a 2020 2020 4061 6273  CMeta):.    @abs
-00001ba0: 7472 6163 746d 6574 686f 640a 2020 2020  tractmethod.    
-00001bb0: 6465 6620 6372 6561 7465 2873 656c 662c  def create(self,
-00001bc0: 2074 6578 7473 3a20 5465 7874 7329 202d   texts: Texts) -
-00001bd0: 3e20 4261 7463 683a 0a20 2020 2020 2020  > Batch:.       
-00001be0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-00001bf0: 656e 7465 6445 7272 6f72 0a0a 0a63 6c61  entedError...cla
-00001c00: 7373 2054 7261 6e73 666f 726d 6572 4261  ss TransformerBa
-00001c10: 7463 6846 6163 746f 7279 2842 6173 6542  tchFactory(BaseB
-00001c20: 6174 6368 4661 6374 6f72 7929 3a0a 2020  atchFactory):.  
-00001c30: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00001c40: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00001c50: 2020 2020 2020 746f 6b65 6e69 7a65 723a        tokenizer:
-00001c60: 2050 7265 5472 6169 6e65 6454 6f6b 656e   PreTrainedToken
-00001c70: 697a 6572 2c0a 2020 2020 2020 2020 6c61  izer,.        la
-00001c80: 6265 6c5f 7365 743a 204c 6162 656c 5365  bel_set: LabelSe
-00001c90: 742c 0a20 2020 2020 2020 2074 6f6b 656e  t,.        token
-00001ca0: 697a 6572 5f61 7267 733a 204f 7074 696f  izer_args: Optio
-00001cb0: 6e61 6c5b 6469 6374 5d20 3d20 4e6f 6e65  nal[dict] = None
-00001cc0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00001cd0: 2069 6620 6e6f 7420 746f 6b65 6e69 7a65   if not tokenize
-00001ce0: 722e 6973 5f66 6173 743a 0a20 2020 2020  r.is_fast:.     
-00001cf0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00001d00: 7565 4572 726f 7228 224f 6e6c 7920 6661  ueError("Only fa
-00001d10: 7374 2074 6f6b 656e 697a 6572 2069 7320  st tokenizer is 
-00001d20: 7375 7070 6f72 7465 642e 2229 0a0a 2020  supported.")..  
-00001d30: 2020 2020 2020 7365 6c66 2e5f 5f74 6f6b        self.__tok
-00001d40: 656e 697a 6572 203d 2074 6f6b 656e 697a  enizer = tokeniz
-00001d50: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-00001d60: 5f5f 6c61 6265 6c5f 7365 7420 3d20 6c61  __label_set = la
-00001d70: 6265 6c5f 7365 740a 0a20 2020 2020 2020  bel_set..       
-00001d80: 2073 656c 662e 5f5f 746f 6b65 6e69 7a65   self.__tokenize
-00001d90: 725f 6172 6773 203d 2074 6f6b 656e 697a  r_args = tokeniz
-00001da0: 6572 5f61 7267 7320 6f72 207b 0a20 2020  er_args or {.   
-00001db0: 2020 2020 2020 2020 2022 7061 6464 696e           "paddin
-00001dc0: 6722 3a20 5472 7565 2c0a 2020 2020 2020  g": True,.      
-00001dd0: 2020 2020 2020 2272 6574 7572 6e5f 7465        "return_te
-00001de0: 6e73 6f72 7322 3a20 2270 7422 2c0a 2020  nsors": "pt",.  
-00001df0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001e00: 7365 6c66 2e5f 5f74 6f6b 656e 697a 6572  self.__tokenizer
-00001e10: 5f61 7267 735b 2272 6574 7572 6e5f 6f66  _args["return_of
-00001e20: 6673 6574 735f 6d61 7070 696e 6722 5d20  fsets_mapping"] 
-00001e30: 3d20 5472 7565 0a0a 2020 2020 6465 6620  = True..    def 
-00001e40: 6372 6561 7465 2873 656c 662c 2074 6578  create(self, tex
-00001e50: 7473 3a20 5465 7874 7329 202d 3e20 4261  ts: Texts) -> Ba
-00001e60: 7463 683a 0a20 2020 2020 2020 2062 6174  tch:.        bat
-00001e70: 6368 5f65 6e63 6f64 696e 6720 3d20 7365  ch_encoding = se
-00001e80: 6c66 2e5f 5f74 6f6b 656e 697a 6572 2874  lf.__tokenizer(t
-00001e90: 6578 7473 2c20 2a2a 7365 6c66 2e5f 5f74  exts, **self.__t
-00001ea0: 6f6b 656e 697a 6572 5f61 7267 7329 0a0a  okenizer_args)..
-00001eb0: 2020 2020 2020 2020 6d61 7070 696e 6773          mappings
-00001ec0: 203d 2062 6174 6368 5f65 6e63 6f64 696e   = batch_encodin
-00001ed0: 672e 706f 7028 226f 6666 7365 745f 6d61  g.pop("offset_ma
-00001ee0: 7070 696e 6722 292e 746f 6c69 7374 2829  pping").tolist()
-00001ef0: 0a20 2020 2020 2020 2070 6164 5f74 6f6b  .        pad_tok
-00001f00: 656e 5f69 6420 3d20 7365 6c66 2e5f 5f74  en_id = self.__t
-00001f10: 6f6b 656e 697a 6572 2e70 6164 5f74 6f6b  okenizer.pad_tok
-00001f20: 656e 5f69 640a 2020 2020 2020 2020 746f  en_id.        to
-00001f30: 6b65 6e69 7a65 645f 7465 7874 5f6c 656e  kenized_text_len
-00001f40: 6774 6873 203d 2028 6261 7463 685f 656e  gths = (batch_en
-00001f50: 636f 6469 6e67 2e69 6e70 7574 5f69 6473  coding.input_ids
-00001f60: 2021 3d20 7061 645f 746f 6b65 6e5f 6964   != pad_token_id
-00001f70: 292e 7375 6d28 6469 6d3d 3129 0a0a 2020  ).sum(dim=1)..  
-00001f80: 2020 2020 2020 746f 6b65 6e69 7a65 645f        tokenized_
-00001f90: 7465 7874 7320 3d20 5b5d 0a20 2020 2020  texts = [].     
-00001fa0: 2020 2066 6f72 2074 6f6b 656e 697a 6564     for tokenized
-00001fb0: 5f74 6578 745f 6c65 6e67 7468 2c20 6d61  _text_length, ma
-00001fc0: 7070 696e 672c 2074 6578 7420 696e 207a  pping, text in z
-00001fd0: 6970 280a 2020 2020 2020 2020 2020 2020  ip(.            
-00001fe0: 746f 6b65 6e69 7a65 645f 7465 7874 5f6c  tokenized_text_l
-00001ff0: 656e 6774 6873 2c20 6d61 7070 696e 6773  engths, mappings
-00002000: 2c20 7465 7874 730a 2020 2020 2020 2020  , texts.        
-00002010: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00002020: 6861 725f 7370 616e 7320 3d20 7475 706c  har_spans = tupl
-00002030: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00002040: 2020 2053 7061 6e28 7374 6172 742c 2065     Span(start, e
-00002050: 6e64 202d 2073 7461 7274 2920 6966 2073  nd - start) if s
-00002060: 7461 7274 2021 3d20 656e 6420 656c 7365  tart != end else
-00002070: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00002080: 2020 2020 2020 666f 7220 7374 6172 742c        for start,
-00002090: 2065 6e64 2069 6e20 6d61 7070 696e 675b   end in mapping[
-000020a0: 3a74 6f6b 656e 697a 6564 5f74 6578 745f  :tokenized_text_
-000020b0: 6c65 6e67 7468 5d0a 2020 2020 2020 2020  length].        
-000020c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000020d0: 2020 746f 6b65 6e5f 696e 6469 6365 7320    token_indices 
-000020e0: 3d20 5b2d 315d 202a 206c 656e 2874 6578  = [-1] * len(tex
-000020f0: 7429 0a20 2020 2020 2020 2020 2020 2066  t).            f
-00002100: 6f72 2074 6f6b 656e 5f69 6e64 6578 2c20  or token_index, 
-00002110: 6368 6172 5f73 7061 6e20 696e 2065 6e75  char_span in enu
-00002120: 6d65 7261 7465 2863 6861 725f 7370 616e  merate(char_span
-00002130: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00002140: 2020 2020 6966 2063 6861 725f 7370 616e      if char_span
-00002150: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00002160: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002170: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00002180: 2020 2020 2020 2073 7461 7274 203d 2063         start = c
-00002190: 6861 725f 7370 616e 2e73 7461 7274 0a20  har_span.start. 
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000021b0: 6e64 203d 2063 6861 725f 7370 616e 2e73  nd = char_span.s
-000021c0: 7461 7274 202b 2063 6861 725f 7370 616e  tart + char_span
-000021d0: 2e6c 656e 6774 680a 2020 2020 2020 2020  .length.        
-000021e0: 2020 2020 2020 2020 746f 6b65 6e5f 696e          token_in
-000021f0: 6469 6365 735b 7374 6172 743a 656e 645d  dices[start:end]
-00002200: 203d 205b 746f 6b65 6e5f 696e 6465 785d   = [token_index]
-00002210: 202a 2063 6861 725f 7370 616e 2e6c 656e   * char_span.len
-00002220: 6774 680a 0a20 2020 2020 2020 2020 2020  gth..           
-00002230: 2074 6f6b 656e 697a 6564 5f74 6578 7473   tokenized_texts
-00002240: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-00002250: 2020 2020 2020 2020 2054 6f6b 656e 697a           Tokeniz
-00002260: 6564 5465 7874 2874 6578 742c 2063 6861  edText(text, cha
-00002270: 725f 7370 616e 732c 2074 7570 6c65 2874  r_spans, tuple(t
-00002280: 6f6b 656e 5f69 6e64 6963 6573 2929 0a20  oken_indices)). 
-00002290: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000022a0: 2020 2020 2020 6c65 6e67 7468 7320 3d20        lengths = 
-000022b0: 5b74 6578 742e 6e75 6d5f 746f 6b65 6e73  [text.num_tokens
-000022c0: 2066 6f72 2074 6578 7420 696e 2074 6f6b   for text in tok
-000022d0: 656e 697a 6564 5f74 6578 7473 5d0a 2020  enized_texts].  
-000022e0: 2020 2020 2020 6d61 785f 6c65 6e67 7468        max_length
-000022f0: 203d 206d 6178 286c 656e 6774 6873 290a   = max(lengths).
-00002300: 2020 2020 2020 2020 6d61 736b 203d 2074          mask = t
-00002310: 6f72 6368 2e74 656e 736f 7228 0a20 2020  orch.tensor(.   
-00002320: 2020 2020 2020 2020 205b 5b54 7275 655d           [[True]
-00002330: 202a 206c 656e 6774 6820 2b20 5b46 616c   * length + [Fal
-00002340: 7365 5d20 2a20 286d 6178 5f6c 656e 6774  se] * (max_lengt
-00002350: 6820 2d20 6c65 6e67 7468 2920 666f 7220  h - length) for 
-00002360: 6c65 6e67 7468 2069 6e20 6c65 6e67 7468  length in length
-00002370: 735d 0a20 2020 2020 2020 2029 0a20 2020  s].        ).   
-00002380: 2020 2020 2072 6574 7572 6e20 4261 7463       return Batc
-00002390: 6828 0a20 2020 2020 2020 2020 2020 2062  h(.            b
-000023a0: 6174 6368 5f65 6e63 6f64 696e 672c 0a20  atch_encoding,. 
-000023b0: 2020 2020 2020 2020 2020 206d 6173 6b2c             mask,
-000023c0: 0a20 2020 2020 2020 2020 2020 2054 6167  .            Tag
-000023d0: 4661 6374 6f72 7928 7475 706c 6528 746f  Factory(tuple(to
-000023e0: 6b65 6e69 7a65 645f 7465 7874 7329 2c20  kenized_texts), 
-000023f0: 7365 6c66 2e5f 5f6c 6162 656c 5f73 6574  self.__label_set
-00002400: 292c 0a20 2020 2020 2020 2029 0a0a 0a63  ),.        )...c
-00002410: 6c61 7373 2043 6f6c 6c61 746f 723a 0a20  lass Collator:. 
-00002420: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00002430: 7365 6c66 2c20 6261 7463 685f 6661 6374  self, batch_fact
-00002440: 6f72 793a 2042 6173 6542 6174 6368 4661  ory: BaseBatchFa
-00002450: 6374 6f72 7929 3a0a 2020 2020 2020 2020  ctory):.        
-00002460: 7365 6c66 2e62 6174 6368 5f66 6163 746f  self.batch_facto
-00002470: 7279 203d 2062 6174 6368 5f66 6163 746f  ry = batch_facto
-00002480: 7279 0a0a 2020 2020 6465 6620 5f5f 6361  ry..    def __ca
-00002490: 6c6c 5f5f 2873 656c 662c 2065 7861 6d70  ll__(self, examp
-000024a0: 6c65 733a 2044 6174 6173 6574 2920 2d3e  les: Dataset) ->
-000024b0: 2074 7570 6c65 5b42 6174 6368 2c20 4368   tuple[Batch, Ch
-000024c0: 6172 4261 7365 6454 6167 7343 6f6c 6c65  arBasedTagsColle
-000024d0: 6374 696f 6e5d 3a0a 2020 2020 2020 2020  ction]:.        
-000024e0: 7465 7874 732c 2074 6167 735f 636f 6c6c  texts, tags_coll
-000024f0: 6563 7469 6f6e 203d 207a 6970 282a 6578  ection = zip(*ex
-00002500: 616d 706c 6573 290a 2020 2020 2020 2020  amples).        
-00002510: 7265 7475 726e 2073 656c 662e 6261 7463  return self.batc
-00002520: 685f 6661 6374 6f72 792e 6372 6561 7465  h_factory.create
-00002530: 2874 6578 7473 292c 2074 6167 735f 636f  (texts), tags_co
-00002540: 6c6c 6563 7469 6f6e 0a                   llection.
+00001490: 652c 0a20 2020 2020 2020 2070 6164 6469  e,.        paddi
+000014a0: 6e67 5f69 6e64 6578 3a20 696e 7420 3d20  ng_index: int = 
+000014b0: 2d31 2c0a 2020 2020 2020 2020 756e 6b6e  -1,.        unkn
+000014c0: 6f77 6e5f 696e 6465 783a 2069 6e74 203d  own_index: int =
+000014d0: 202d 3130 302c 0a20 2020 2029 202d 3e20   -100,.    ) -> 
+000014e0: 746f 7263 682e 5465 6e73 6f72 3a0a 2020  torch.Tensor:.  
+000014f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001500: 662e 5f5f 7461 675f 6661 6374 6f72 792e  f.__tag_factory.
+00001510: 6372 6561 7465 5f74 6167 5f69 6e64 6963  create_tag_indic
+00001520: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00001530: 7461 6773 5f63 6f6c 6c65 6374 696f 6e2c  tags_collection,
+00001540: 2064 6576 6963 652c 2070 6164 6469 6e67   device, padding
+00001550: 5f69 6e64 6578 2c20 756e 6b6e 6f77 6e5f  _index, unknown_
+00001560: 696e 6465 780a 2020 2020 2020 2020 290a  index.        ).
+00001570: 0a20 2020 2064 6566 2063 7265 6174 655f  .    def create_
+00001580: 7461 675f 6269 746d 6170 280a 2020 2020  tag_bitmap(.    
+00001590: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000015a0: 2020 7461 6773 5f63 6f6c 6c65 6374 696f    tags_collectio
+000015b0: 6e3a 2043 6861 7242 6173 6564 5461 6773  n: CharBasedTags
+000015c0: 436f 6c6c 6563 7469 6f6e 2c0a 2020 2020  Collection,.    
+000015d0: 2020 2020 6465 7669 6365 3a20 746f 7263      device: torc
+000015e0: 682e 6465 7669 6365 2c0a 2020 2020 2020  h.device,.      
+000015f0: 2020 7061 6464 696e 675f 696e 6465 783a    padding_index:
+00001600: 2069 6e74 203d 202d 312c 0a20 2020 2020   int = -1,.     
+00001610: 2020 2075 6e6b 6e6f 776e 5f69 6e64 6578     unknown_index
+00001620: 3a20 696e 7420 3d20 2d31 3030 2c0a 2020  : int = -100,.  
+00001630: 2020 2920 2d3e 2074 6f72 6368 2e54 656e    ) -> torch.Ten
+00001640: 736f 723a 0a20 2020 2020 2020 2072 6574  sor:.        ret
+00001650: 7572 6e20 7365 6c66 2e5f 5f74 6167 5f66  urn self.__tag_f
+00001660: 6163 746f 7279 2e63 7265 6174 655f 7461  actory.create_ta
+00001670: 675f 6269 746d 6170 280a 2020 2020 2020  g_bitmap(.      
+00001680: 2020 2020 2020 7461 6773 5f63 6f6c 6c65        tags_colle
+00001690: 6374 696f 6e2c 2064 6576 6963 652c 2070  ction, device, p
+000016a0: 6164 6469 6e67 5f69 6e64 6578 2c20 756e  adding_index, un
+000016b0: 6b6e 6f77 6e5f 696e 6465 780a 2020 2020  known_index.    
+000016c0: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
+000016d0: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+000016e0: 2073 7472 3a0a 2020 2020 2020 2020 7465   str:.        te
+000016f0: 7874 5f73 7472 203d 205b 5d0a 2020 2020  xt_str = [].    
+00001700: 2020 2020 666f 7220 7465 7874 2069 6e20      for text in 
+00001710: 7365 6c66 2e74 6f6b 656e 697a 6564 5f74  self.tokenized_t
+00001720: 6578 7473 3a0a 2020 2020 2020 2020 2020  exts:.          
+00001730: 2020 7465 7874 5f73 7472 2e61 7070 656e    text_str.appen
+00001740: 6428 6622 2020 2020 2d20 7b72 6570 7228  d(f"    - {repr(
+00001750: 7465 7874 297d 5c6e 2229 0a20 2020 2020  text)}\n").     
+00001760: 2020 2072 6574 7572 6e20 2242 6174 6368     return "Batch
+00001770: 3a5c 6e22 202b 2066 2220 2073 697a 653a  :\n" + f"  size:
+00001780: 207b 7365 6c66 2e73 697a 657d 5c6e 2220   {self.size}\n" 
+00001790: 2b20 2220 2064 6174 613a 5c6e 2220 2b20  + "  data:\n" + 
+000017a0: 2222 2e6a 6f69 6e28 7465 7874 5f73 7472  "".join(text_str
+000017b0: 290a 0a0a 636c 6173 7320 4261 7365 4261  )...class BaseBa
+000017c0: 7463 6846 6163 746f 7279 286d 6574 6163  tchFactory(metac
+000017d0: 6c61 7373 3d41 4243 4d65 7461 293a 0a20  lass=ABCMeta):. 
+000017e0: 2020 2040 6162 7374 7261 6374 6d65 7468     @abstractmeth
+000017f0: 6f64 0a20 2020 2064 6566 2063 7265 6174  od.    def creat
+00001800: 6528 7365 6c66 2c20 7465 7874 733a 2054  e(self, texts: T
+00001810: 6578 7473 2920 2d3e 2042 6174 6368 3a0a  exts) -> Batch:.
+00001820: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+00001830: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00001840: 720a 0a0a 636c 6173 7320 5472 616e 7366  r...class Transf
+00001850: 6f72 6d65 7242 6174 6368 4661 6374 6f72  ormerBatchFactor
+00001860: 7928 4261 7365 4261 7463 6846 6163 746f  y(BaseBatchFacto
+00001870: 7279 293a 0a20 2020 2064 6566 205f 5f69  ry):.    def __i
+00001880: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00001890: 656c 662c 0a20 2020 2020 2020 2074 6f6b  elf,.        tok
+000018a0: 656e 697a 6572 3a20 5072 6554 7261 696e  enizer: PreTrain
+000018b0: 6564 546f 6b65 6e69 7a65 722c 0a20 2020  edTokenizer,.   
+000018c0: 2020 2020 206c 6162 656c 5f73 6574 3a20       label_set: 
+000018d0: 4c61 6265 6c53 6574 2c0a 2020 2020 2020  LabelSet,.      
+000018e0: 2020 746f 6b65 6e69 7a65 725f 6172 6773    tokenizer_args
+000018f0: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
+00001900: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00001910: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
+00001920: 6f6b 656e 697a 6572 2e69 735f 6661 7374  okenizer.is_fast
+00001930: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00001940: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00001950: 4f6e 6c79 2066 6173 7420 746f 6b65 6e69  Only fast tokeni
+00001960: 7a65 7220 6973 2073 7570 706f 7274 6564  zer is supported
+00001970: 2e22 290a 0a20 2020 2020 2020 2073 656c  .")..        sel
+00001980: 662e 5f5f 746f 6b65 6e69 7a65 7220 3d20  f.__tokenizer = 
+00001990: 746f 6b65 6e69 7a65 720a 2020 2020 2020  tokenizer.      
+000019a0: 2020 7365 6c66 2e5f 5f6c 6162 656c 5f73    self.__label_s
+000019b0: 6574 203d 206c 6162 656c 5f73 6574 0a0a  et = label_set..
+000019c0: 2020 2020 2020 2020 7365 6c66 2e5f 5f74          self.__t
+000019d0: 6f6b 656e 697a 6572 5f61 7267 7320 3d20  okenizer_args = 
+000019e0: 746f 6b65 6e69 7a65 725f 6172 6773 206f  tokenizer_args o
+000019f0: 7220 7b0a 2020 2020 2020 2020 2020 2020  r {.            
+00001a00: 2270 6164 6469 6e67 223a 2054 7275 652c  "padding": True,
+00001a10: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00001a20: 7475 726e 5f74 656e 736f 7273 223a 2022  turn_tensors": "
+00001a30: 7074 222c 0a20 2020 2020 2020 207d 0a20  pt",.        }. 
+00001a40: 2020 2020 2020 2073 656c 662e 5f5f 746f         self.__to
+00001a50: 6b65 6e69 7a65 725f 6172 6773 5b22 7265  kenizer_args["re
+00001a60: 7475 726e 5f6f 6666 7365 7473 5f6d 6170  turn_offsets_map
+00001a70: 7069 6e67 225d 203d 2054 7275 650a 0a20  ping"] = True.. 
+00001a80: 2020 2064 6566 2063 7265 6174 6528 7365     def create(se
+00001a90: 6c66 2c20 7465 7874 733a 2054 6578 7473  lf, texts: Texts
+00001aa0: 2920 2d3e 2042 6174 6368 3a0a 2020 2020  ) -> Batch:.    
+00001ab0: 2020 2020 6261 7463 685f 656e 636f 6469      batch_encodi
+00001ac0: 6e67 203d 2073 656c 662e 5f5f 746f 6b65  ng = self.__toke
+00001ad0: 6e69 7a65 7228 7465 7874 732c 202a 2a73  nizer(texts, **s
+00001ae0: 656c 662e 5f5f 746f 6b65 6e69 7a65 725f  elf.__tokenizer_
+00001af0: 6172 6773 290a 0a20 2020 2020 2020 206d  args)..        m
+00001b00: 6170 7069 6e67 7320 3d20 6261 7463 685f  appings = batch_
+00001b10: 656e 636f 6469 6e67 2e70 6f70 2822 6f66  encoding.pop("of
+00001b20: 6673 6574 5f6d 6170 7069 6e67 2229 2e74  fset_mapping").t
+00001b30: 6f6c 6973 7428 290a 2020 2020 2020 2020  olist().        
+00001b40: 7061 645f 746f 6b65 6e5f 6964 203d 2073  pad_token_id = s
+00001b50: 656c 662e 5f5f 746f 6b65 6e69 7a65 722e  elf.__tokenizer.
+00001b60: 7061 645f 746f 6b65 6e5f 6964 0a20 2020  pad_token_id.   
+00001b70: 2020 2020 2074 6f6b 656e 697a 6564 5f74       tokenized_t
+00001b80: 6578 745f 6c65 6e67 7468 7320 3d20 2862  ext_lengths = (b
+00001b90: 6174 6368 5f65 6e63 6f64 696e 672e 696e  atch_encoding.in
+00001ba0: 7075 745f 6964 7320 213d 2070 6164 5f74  put_ids != pad_t
+00001bb0: 6f6b 656e 5f69 6429 2e73 756d 2864 696d  oken_id).sum(dim
+00001bc0: 3d31 290a 0a20 2020 2020 2020 2074 6f6b  =1)..        tok
+00001bd0: 656e 697a 6564 5f74 6578 7473 203d 205b  enized_texts = [
+00001be0: 5d0a 2020 2020 2020 2020 666f 7220 746f  ].        for to
+00001bf0: 6b65 6e69 7a65 645f 7465 7874 5f6c 656e  kenized_text_len
+00001c00: 6774 682c 206d 6170 7069 6e67 2c20 7465  gth, mapping, te
+00001c10: 7874 2069 6e20 7a69 7028 0a20 2020 2020  xt in zip(.     
+00001c20: 2020 2020 2020 2074 6f6b 656e 697a 6564         tokenized
+00001c30: 5f74 6578 745f 6c65 6e67 7468 732c 206d  _text_lengths, m
+00001c40: 6170 7069 6e67 732c 2074 6578 7473 2c20  appings, texts, 
+00001c50: 7374 7269 6374 3d54 7275 650a 2020 2020  strict=True.    
+00001c60: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00001c70: 2020 2063 6861 725f 7370 616e 7320 3d20     char_spans = 
+00001c80: 7475 706c 6528 0a20 2020 2020 2020 2020  tuple(.         
+00001c90: 2020 2020 2020 2053 7061 6e28 7374 6172         Span(star
+00001ca0: 742c 2065 6e64 202d 2073 7461 7274 2920  t, end - start) 
+00001cb0: 6966 2073 7461 7274 2021 3d20 656e 6420  if start != end 
+00001cc0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+00001cd0: 2020 2020 2020 2020 2020 666f 7220 7374            for st
+00001ce0: 6172 742c 2065 6e64 2069 6e20 6d61 7070  art, end in mapp
+00001cf0: 696e 675b 3a74 6f6b 656e 697a 6564 5f74  ing[:tokenized_t
+00001d00: 6578 745f 6c65 6e67 7468 5d0a 2020 2020  ext_length].    
+00001d10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00001d20: 2020 2020 2020 746f 6b65 6e5f 696e 6469        token_indi
+00001d30: 6365 7320 3d20 5b2d 315d 202a 206c 656e  ces = [-1] * len
+00001d40: 2874 6578 7429 0a20 2020 2020 2020 2020  (text).         
+00001d50: 2020 2066 6f72 2074 6f6b 656e 5f69 6e64     for token_ind
+00001d60: 6578 2c20 6368 6172 5f73 7061 6e20 696e  ex, char_span in
+00001d70: 2065 6e75 6d65 7261 7465 2863 6861 725f   enumerate(char_
+00001d80: 7370 616e 7329 3a0a 2020 2020 2020 2020  spans):.        
+00001d90: 2020 2020 2020 2020 6966 2063 6861 725f          if char_
+00001da0: 7370 616e 2069 7320 4e6f 6e65 3a0a 2020  span is None:.  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00001dd0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00001de0: 203d 2063 6861 725f 7370 616e 2e73 7461   = char_span.sta
+00001df0: 7274 0a20 2020 2020 2020 2020 2020 2020  rt.             
+00001e00: 2020 2065 6e64 203d 2063 6861 725f 7370     end = char_sp
+00001e10: 616e 2e73 7461 7274 202b 2063 6861 725f  an.start + char_
+00001e20: 7370 616e 2e6c 656e 6774 680a 2020 2020  span.length.    
+00001e30: 2020 2020 2020 2020 2020 2020 746f 6b65              toke
+00001e40: 6e5f 696e 6469 6365 735b 7374 6172 743a  n_indices[start:
+00001e50: 656e 645d 203d 205b 746f 6b65 6e5f 696e  end] = [token_in
+00001e60: 6465 785d 202a 2063 6861 725f 7370 616e  dex] * char_span
+00001e70: 2e6c 656e 6774 680a 0a20 2020 2020 2020  .length..       
+00001e80: 2020 2020 2074 6f6b 656e 697a 6564 5f74       tokenized_t
+00001e90: 6578 7473 2e61 7070 656e 6428 0a20 2020  exts.append(.   
+00001ea0: 2020 2020 2020 2020 2020 2020 2054 6f6b               Tok
+00001eb0: 656e 697a 6564 5465 7874 2874 6578 742c  enizedText(text,
+00001ec0: 2063 6861 725f 7370 616e 732c 2074 7570   char_spans, tup
+00001ed0: 6c65 2874 6f6b 656e 5f69 6e64 6963 6573  le(token_indices
+00001ee0: 2929 0a20 2020 2020 2020 2020 2020 2029  )).            )
+00001ef0: 0a0a 2020 2020 2020 2020 6c65 6e67 7468  ..        length
+00001f00: 7320 3d20 5b74 6578 742e 6e75 6d5f 746f  s = [text.num_to
+00001f10: 6b65 6e73 2066 6f72 2074 6578 7420 696e  kens for text in
+00001f20: 2074 6f6b 656e 697a 6564 5f74 6578 7473   tokenized_texts
+00001f30: 5d0a 2020 2020 2020 2020 6d61 785f 6c65  ].        max_le
+00001f40: 6e67 7468 203d 206d 6178 286c 656e 6774  ngth = max(lengt
+00001f50: 6873 290a 2020 2020 2020 2020 6d61 736b  hs).        mask
+00001f60: 203d 2074 6f72 6368 2e74 656e 736f 7228   = torch.tensor(
+00001f70: 0a20 2020 2020 2020 2020 2020 205b 5b54  .            [[T
+00001f80: 7275 655d 202a 206c 656e 6774 6820 2b20  rue] * length + 
+00001f90: 5b46 616c 7365 5d20 2a20 286d 6178 5f6c  [False] * (max_l
+00001fa0: 656e 6774 6820 2d20 6c65 6e67 7468 2920  ength - length) 
+00001fb0: 666f 7220 6c65 6e67 7468 2069 6e20 6c65  for length in le
+00001fc0: 6e67 7468 735d 0a20 2020 2020 2020 2029  ngths].        )
+00001fd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001fe0: 4261 7463 6828 0a20 2020 2020 2020 2020  Batch(.         
+00001ff0: 2020 2062 6174 6368 5f65 6e63 6f64 696e     batch_encodin
+00002000: 672c 0a20 2020 2020 2020 2020 2020 206d  g,.            m
+00002010: 6173 6b2c 0a20 2020 2020 2020 2020 2020  ask,.           
+00002020: 2054 6167 4661 6374 6f72 7928 7475 706c   TagFactory(tupl
+00002030: 6528 746f 6b65 6e69 7a65 645f 7465 7874  e(tokenized_text
+00002040: 7329 2c20 7365 6c66 2e5f 5f6c 6162 656c  s), self.__label
+00002050: 5f73 6574 292c 0a20 2020 2020 2020 2029  _set),.        )
+00002060: 0a0a 0a63 6c61 7373 2043 6f6c 6c61 746f  ...class Collato
+00002070: 723a 0a20 2020 2064 6566 205f 5f69 6e69  r:.    def __ini
+00002080: 745f 5f28 7365 6c66 2c20 6261 7463 685f  t__(self, batch_
+00002090: 6661 6374 6f72 793a 2042 6173 6542 6174  factory: BaseBat
+000020a0: 6368 4661 6374 6f72 7929 3a0a 2020 2020  chFactory):.    
+000020b0: 2020 2020 7365 6c66 2e62 6174 6368 5f66      self.batch_f
+000020c0: 6163 746f 7279 203d 2062 6174 6368 5f66  actory = batch_f
+000020d0: 6163 746f 7279 0a0a 2020 2020 6465 6620  actory..    def 
+000020e0: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2065  __call__(self, e
+000020f0: 7861 6d70 6c65 733a 2044 6174 6173 6574  xamples: Dataset
+00002100: 2920 2d3e 2074 7570 6c65 5b42 6174 6368  ) -> tuple[Batch
+00002110: 2c20 4368 6172 4261 7365 6454 6167 7343  , CharBasedTagsC
+00002120: 6f6c 6c65 6374 696f 6e5d 3a0a 2020 2020  ollection]:.    
+00002130: 2020 2020 7465 7874 732c 2074 6167 735f      texts, tags_
+00002140: 636f 6c6c 6563 7469 6f6e 203d 207a 6970  collection = zip
+00002150: 282a 6578 616d 706c 6573 2c20 7374 7269  (*examples, stri
+00002160: 6374 3d54 7275 6529 0a20 2020 2020 2020  ct=True).       
+00002170: 2072 6574 7572 6e20 7365 6c66 2e62 6174   return self.bat
+00002180: 6368 5f66 6163 746f 7279 2e63 7265 6174  ch_factory.creat
+00002190: 6528 7465 7874 7329 2c20 7461 6773 5f63  e(texts), tags_c
+000021a0: 6f6c 6c65 6374 696f 6e0a                 ollection.
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/418bc6111a8ba78a` & `pytorch_partial_tagger-0.1.2/tests/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,529 +1,461 @@
-00000000: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
-00000010: 7465 7374 732e 6865 6c70 6572 7306 0000  tests.helpers...
-00000020: 0000 0000 0011 0000 0000 0000 0069 7465  .............ite
-00000030: 7274 6f6f 6c73 2e70 726f 6475 6374 1600  rtools.product..
-00000040: 0000 1d00 0000 1000 0000 0000 0000 7479  ..............ty
-00000050: 7069 6e67 2e47 656e 6572 6174 6f72 3100  ping.Generator1.
-00000060: 0000 3a00 0000 0c00 0000 0000 0000 7479  ..:...........ty
-00000070: 7069 6e67 2e54 7570 6c65 3c00 0000 4100  ping.Tuple<...A.
-00000080: 0000 0500 0000 0000 0000 746f 7263 6843  ..........torchC
-00000090: 0000 004f 0000 0017 0000 0000 0000 0070  ...O...........p
-000000a0: 6172 7469 616c 5f74 6167 6765 722e 6372  artial_tagger.cr
-000000b0: 662e 4e49 4e46 7000 0000 7400 0000 1d00  f.NINFp...t.....
-000000c0: 0000 0000 0000 7061 7274 6961 6c5f 7461  ......partial_ta
-000000d0: 6767 6572 2e63 7266 2e66 756e 6374 696f  gger.crf.functio
-000000e0: 6e61 6c94 0000 00a3 0000 0006 0000 0000  nal.............
-000000f0: 0000 0010 0000 0000 0000 0043 6f6d 706c  ...........Compl
-00000100: 6578 5374 7275 6374 7572 653b 0000 0000  exStructure;....
-00000110: 0000 0060 6368 6563 6b5f 636f 6e73 7472  ...`check_constr
-00000120: 6169 6e65 645f 6c6f 675f 706f 7465 6e74  ained_log_potent
-00000130: 6961 6c73 6020 6973 2074 6f6f 2063 6f6d  ials` is too com
-00000140: 706c 6578 2028 3138 203e 2031 3029 00d6  plex (18 > 10)..
-00000150: 1300 00f6 1300 0000 0000 0000 0000 0000  ................
-00000160: d613 0000 1800 0000 0000 0000 5a69 7057  ............ZipW
-00000170: 6974 686f 7574 4578 706c 6963 6974 5374  ithoutExplicitSt
-00000180: 7269 6374 2f00 0000 0000 0000 607a 6970  rict/.......`zip
-00000190: 2829 6020 7769 7468 6f75 7420 616e 2065  ()` without an e
-000001a0: 7870 6c69 6369 7420 6073 7472 6963 743d  xplicit `strict=
-000001b0: 6020 7061 7261 6d65 7465 7200 b104 0000  ` parameter.....
-000001c0: d704 0000 0000 0000 0000 0000 00b1 0400  ................
-000001d0: 0018 0000 0000 0000 005a 6970 5769 7468  .........ZipWith
-000001e0: 6f75 7445 7870 6c69 6369 7453 7472 6963  outExplicitStric
-000001f0: 742f 0000 0000 0000 0060 7a69 7028 2960  t/.......`zip()`
-00000200: 2077 6974 686f 7574 2061 6e20 6578 706c   without an expl
-00000210: 6963 6974 2060 7374 7269 6374 3d60 2070  icit `strict=` p
-00000220: 6172 616d 6574 6572 0001 0800 0027 0800  arameter.....'..
-00000230: 0000 0000 0000 0000 0000 0108 0000 1800  ................
-00000240: 0000 0000 0000 5a69 7057 6974 686f 7574  ......ZipWithout
-00000250: 4578 706c 6963 6974 5374 7269 6374 2f00  ExplicitStrict/.
-00000260: 0000 0000 0000 607a 6970 2829 6020 7769  ......`zip()` wi
-00000270: 7468 6f75 7420 616e 2065 7870 6c69 6369  thout an explici
-00000280: 7420 6073 7472 6963 743d 6020 7061 7261  t `strict=` para
-00000290: 6d65 7465 7200 a411 0000 bc11 0000 0000  meter...........
-000002a0: 0000 0000 0000 00a4 1100 0018 0000 0000  ................
-000002b0: 0000 005a 6970 5769 7468 6f75 7445 7870  ...ZipWithoutExp
-000002c0: 6c69 6369 7453 7472 6963 742f 0000 0000  licitStrict/....
-000002d0: 0000 0060 7a69 7028 2960 2077 6974 686f  ...`zip()` witho
-000002e0: 7574 2061 6e20 6578 706c 6963 6974 2060  ut an explicit `
-000002f0: 7374 7269 6374 3d60 2070 6172 616d 6574  strict=` paramet
-00000300: 6572 00a2 1500 00ba 1500 0000 0000 0000  er..............
-00000310: 0000 0000 a215 0000 0f00 0000 0000 0000  ................
-00000320: 556e 736f 7274 6564 496d 706f 7274 7329  UnsortedImports)
-00000330: 0000 0000 0000 0049 6d70 6f72 7420 626c  .......Import bl
-00000340: 6f63 6b20 6973 2075 6e2d 736f 7274 6564  ock is un-sorted
-00000350: 206f 7220 756e 2d66 6f72 6d61 7474 6564   or un-formatted
-00000360: 0110 0000 0000 0000 004f 7267 616e 697a  .........Organiz
-00000370: 6520 696d 706f 7274 7300 0000 00a6 0000  e imports.......
-00000380: 0001 0100 0000 0000 0000 0000 0000 a600  ................
-00000390: 0000 01a5 0000 0000 0000 0066 726f 6d20  ...........from 
-000003a0: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
-000003b0: 2070 726f 6475 6374 0a66 726f 6d20 7479   product.from ty
-000003c0: 7069 6e67 2069 6d70 6f72 7420 4765 6e65  ping import Gene
-000003d0: 7261 746f 722c 2054 7570 6c65 0a0a 696d  rator, Tuple..im
-000003e0: 706f 7274 2074 6f72 6368 0a66 726f 6d20  port torch.from 
-000003f0: 7061 7274 6961 6c5f 7461 6767 6572 2e63  partial_tagger.c
-00000400: 7266 2069 6d70 6f72 7420 4e49 4e46 0a66  rf import NINF.f
-00000410: 726f 6d20 7061 7274 6961 6c5f 7461 6767  rom partial_tagg
-00000420: 6572 2e63 7266 2069 6d70 6f72 7420 6675  er.crf import fu
-00000430: 6e63 7469 6f6e 616c 2061 7320 460a 0a0a  nctional as F...
-00000440: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 0100 0000 0000 0000 4100 0000 0000 0000  ........A.......
-00000460: 2f55 7365 7273 2f79 6173 7566 756d 692f  /Users/yasufumi/
-00000470: 576f 726b 7370 6163 652f 7079 746f 7263  Workspace/pytorc
-00000480: 682d 7061 7274 6961 6c2d 7461 6767 6572  h-partial-tagger
-00000490: 2f74 6573 7473 2f68 656c 7065 7273 2e70  /tests/helpers.p
-000004a0: 7959 1c00 0000 0000 0066 726f 6d20 6974  yY.......from it
-000004b0: 6572 746f 6f6c 7320 696d 706f 7274 2070  ertools import p
-000004c0: 726f 6475 6374 0a66 726f 6d20 7479 7069  roduct.from typi
-000004d0: 6e67 2069 6d70 6f72 7420 4765 6e65 7261  ng import Genera
-000004e0: 746f 722c 2054 7570 6c65 0a0a 696d 706f  tor, Tuple..impo
-000004f0: 7274 2074 6f72 6368 0a0a 6672 6f6d 2070  rt torch..from p
-00000500: 6172 7469 616c 5f74 6167 6765 722e 6372  artial_tagger.cr
-00000510: 6620 696d 706f 7274 204e 494e 460a 6672  f import NINF.fr
-00000520: 6f6d 2070 6172 7469 616c 5f74 6167 6765  om partial_tagge
-00000530: 722e 6372 6620 696d 706f 7274 2066 756e  r.crf import fun
-00000540: 6374 696f 6e61 6c20 6173 2046 0a0a 0a64  ctional as F...d
-00000550: 6566 2069 7465 7261 7465 5f70 6f73 7369  ef iterate_possi
-00000560: 626c 655f 7461 675f 696e 6469 6365 7328  ble_tag_indices(
-00000570: 0a20 2020 2073 6571 7565 6e63 655f 6c65  .    sequence_le
-00000580: 6e67 7468 3a20 696e 742c 206e 756d 5f74  ngth: int, num_t
-00000590: 6167 733a 2069 6e74 0a29 202d 3e20 4765  ags: int.) -> Ge
-000005a0: 6e65 7261 746f 725b 7475 706c 652c 204e  nerator[tuple, N
-000005b0: 6f6e 652c 204e 6f6e 655d 3a0a 2020 2020  one, None]:.    
-000005c0: 7969 656c 6420 6672 6f6d 2070 726f 6475  yield from produ
-000005d0: 6374 2872 616e 6765 286e 756d 5f74 6167  ct(range(num_tag
-000005e0: 7329 2c20 7265 7065 6174 3d73 6571 7565  s), repeat=seque
-000005f0: 6e63 655f 6c65 6e67 7468 290a 0a0a 6465  nce_length)...de
-00000600: 6620 6974 6572 6174 655f 706f 7373 6962  f iterate_possib
-00000610: 6c65 5f6f 6e65 5f68 6f74 5f74 6167 5f62  le_one_hot_tag_b
-00000620: 6974 6d61 7028 0a20 2020 2062 6174 6368  itmap(.    batch
-00000630: 5f73 697a 653a 2069 6e74 2c20 7365 7175  _size: int, sequ
-00000640: 656e 6365 5f6c 656e 6774 683a 2069 6e74  ence_length: int
-00000650: 2c20 6e75 6d5f 7461 6773 3a20 696e 740a  , num_tags: int.
-00000660: 2920 2d3e 2047 656e 6572 6174 6f72 5b74  ) -> Generator[t
-00000670: 6f72 6368 2e54 656e 736f 722c 204e 6f6e  orch.Tensor, Non
-00000680: 652c 204e 6f6e 655d 3a0a 2020 2020 666f  e, None]:.    fo
-00000690: 7220 7461 675f 696e 6469 6365 7320 696e  r tag_indices in
-000006a0: 2069 7465 7261 7465 5f70 6f73 7369 626c   iterate_possibl
-000006b0: 655f 7461 675f 696e 6469 6365 7328 7365  e_tag_indices(se
-000006c0: 7175 656e 6365 5f6c 656e 6774 682c 206e  quence_length, n
-000006d0: 756d 5f74 6167 7329 3a0a 2020 2020 2020  um_tags):.      
-000006e0: 2020 7461 675f 6269 746d 6170 203d 205b    tag_bitmap = [
-000006f0: 5d0a 2020 2020 2020 2020 666f 7220 6163  ].        for ac
-00000700: 7469 7665 2069 6e20 7461 675f 696e 6469  tive in tag_indi
-00000710: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
-00000720: 2062 6974 6d61 7020 3d20 5b46 616c 7365   bitmap = [False
-00000730: 5d20 2a20 6e75 6d5f 7461 6773 0a20 2020  ] * num_tags.   
-00000740: 2020 2020 2020 2020 2062 6974 6d61 705b           bitmap[
-00000750: 6163 7469 7665 5d20 3d20 5472 7565 0a20  active] = True. 
-00000760: 2020 2020 2020 2020 2020 2074 6167 5f62             tag_b
-00000770: 6974 6d61 702e 6170 7065 6e64 2862 6974  itmap.append(bit
-00000780: 6d61 7029 0a20 2020 2020 2020 2079 6965  map).        yie
-00000790: 6c64 2074 6f72 6368 2e74 656e 736f 7228  ld torch.tensor(
-000007a0: 5b74 6167 5f62 6974 6d61 705d 202a 2062  [tag_bitmap] * b
-000007b0: 6174 6368 5f73 697a 6529 0a0a 0a64 6566  atch_size)...def
-000007c0: 2063 6f6d 7075 7465 5f6c 6f67 5f6e 6f72   compute_log_nor
-000007d0: 6d61 6c69 7a65 725f 6279 5f62 7275 7465  malizer_by_brute
-000007e0: 5f66 6f72 6365 286c 6f67 5f70 6f74 656e  _force(log_poten
-000007f0: 7469 616c 733a 2074 6f72 6368 2e54 656e  tials: torch.Ten
-00000800: 736f 7229 202d 3e20 746f 7263 682e 5465  sor) -> torch.Te
-00000810: 6e73 6f72 3a0a 2020 2020 6261 7463 685f  nsor:.    batch_
-00000820: 7369 7a65 2c20 7365 7175 656e 6365 5f6c  size, sequence_l
-00000830: 656e 6774 682c 206e 756d 5f74 6167 732c  ength, num_tags,
-00000840: 205f 203d 206c 6f67 5f70 6f74 656e 7469   _ = log_potenti
-00000850: 616c 732e 7369 7a65 2829 0a20 2020 206c  als.size().    l
-00000860: 6f67 5f5a 203d 2074 6f72 6368 2e74 656e  og_Z = torch.ten
-00000870: 736f 7228 5b4e 494e 465d 202a 2062 6174  sor([NINF] * bat
-00000880: 6368 5f73 697a 6529 0a20 2020 2066 6f72  ch_size).    for
-00000890: 2062 2069 6e20 7261 6e67 6528 6261 7463   b in range(batc
-000008a0: 685f 7369 7a65 293a 0a20 2020 2020 2020  h_size):.       
-000008b0: 2066 6f72 2074 6167 5f69 6e64 6963 6573   for tag_indices
-000008c0: 2069 6e20 6974 6572 6174 655f 706f 7373   in iterate_poss
-000008d0: 6962 6c65 5f74 6167 5f69 6e64 6963 6573  ible_tag_indices
-000008e0: 2873 6571 7565 6e63 655f 6c65 6e67 7468  (sequence_length
-000008f0: 202b 2031 2c20 6e75 6d5f 7461 6773 293a   + 1, num_tags):
-00000900: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
-00000910: 5f69 6e64 6963 6573 5f73 636f 7265 203d  _indices_score =
-00000920: 2074 6f72 6368 2e74 656e 736f 7228 302e   torch.tensor(0.
-00000930: 3029 0a20 2020 2020 2020 2020 2020 2066  0).            f
-00000940: 6f72 2069 2c20 286a 2c20 6b29 2069 6e20  or i, (j, k) in 
-00000950: 656e 756d 6572 6174 6528 7a69 7028 7461  enumerate(zip(ta
-00000960: 675f 696e 6469 6365 735b 3a2d 315d 2c20  g_indices[:-1], 
-00000970: 7461 675f 696e 6469 6365 735b 313a 5d29  tag_indices[1:])
-00000980: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00000990: 2020 2074 6167 5f69 6e64 6963 6573 5f73     tag_indices_s
-000009a0: 636f 7265 202b 3d20 6c6f 675f 706f 7465  core += log_pote
-000009b0: 6e74 6961 6c73 5b62 2c20 692c 206a 2c20  ntials[b, i, j, 
-000009c0: 6b5d 0a20 2020 2020 2020 2020 2020 206c  k].            l
-000009d0: 6f67 5f5a 5b62 5d20 3d20 746f 7263 682e  og_Z[b] = torch.
-000009e0: 6c6f 6761 6464 6578 7028 6c6f 675f 5a5b  logaddexp(log_Z[
-000009f0: 625d 2c20 7461 675f 696e 6469 6365 735f  b], tag_indices_
-00000a00: 7363 6f72 6529 0a20 2020 2072 6574 7572  score).    retur
-00000a10: 6e20 6c6f 675f 5a0a 0a0a 6465 6620 636f  n log_Z...def co
-00000a20: 6d70 7574 655f 6265 7374 5f74 6167 5f69  mpute_best_tag_i
-00000a30: 6e64 6963 6573 5f62 795f 6272 7574 655f  ndices_by_brute_
-00000a40: 666f 7263 6528 0a20 2020 206c 6f67 5f70  force(.    log_p
-00000a50: 6f74 656e 7469 616c 733a 2074 6f72 6368  otentials: torch
-00000a60: 2e54 656e 736f 722c 0a29 202d 3e20 5475  .Tensor,.) -> Tu
-00000a70: 706c 655b 746f 7263 682e 5465 6e73 6f72  ple[torch.Tensor
-00000a80: 2c20 746f 7263 682e 5465 6e73 6f72 5d3a  , torch.Tensor]:
-00000a90: 0a20 2020 2062 6174 6368 5f73 697a 652c  .    batch_size,
-00000aa0: 2073 6571 7565 6e63 655f 6c65 6e67 7468   sequence_length
-00000ab0: 2c20 6e75 6d5f 7461 6773 2c20 5f20 3d20  , num_tags, _ = 
-00000ac0: 6c6f 675f 706f 7465 6e74 6961 6c73 2e73  log_potentials.s
-00000ad0: 697a 6528 290a 2020 2020 6265 7374 5f74  ize().    best_t
-00000ae0: 6167 5f69 6e64 6963 6573 203d 2074 6f72  ag_indices = tor
-00000af0: 6368 2e74 656e 736f 7228 5b5b 2d31 5d20  ch.tensor([[-1] 
-00000b00: 2a20 7365 7175 656e 6365 5f6c 656e 6774  * sequence_lengt
-00000b10: 6820 666f 7220 5f20 696e 2072 616e 6765  h for _ in range
-00000b20: 2862 6174 6368 5f73 697a 6529 5d29 0a20  (batch_size)]). 
-00000b30: 2020 206d 6178 5f73 636f 7265 7320 3d20     max_scores = 
-00000b40: 746f 7263 682e 7465 6e73 6f72 285b 4e49  torch.tensor([NI
-00000b50: 4e46 5d20 2a20 6261 7463 685f 7369 7a65  NF] * batch_size
-00000b60: 290a 2020 2020 666f 7220 6220 696e 2072  ).    for b in r
-00000b70: 616e 6765 2862 6174 6368 5f73 697a 6529  ange(batch_size)
-00000b80: 3a0a 2020 2020 2020 2020 6d61 785f 7363  :.        max_sc
-00000b90: 6f72 6520 3d20 746f 7263 682e 7465 6e73  ore = torch.tens
-00000ba0: 6f72 284e 494e 4629 0a20 2020 2020 2020  or(NINF).       
-00000bb0: 2066 6f72 2074 6167 5f69 6e64 6963 6573   for tag_indices
-00000bc0: 2069 6e20 6974 6572 6174 655f 706f 7373   in iterate_poss
-00000bd0: 6962 6c65 5f74 6167 5f69 6e64 6963 6573  ible_tag_indices
-00000be0: 2873 6571 7565 6e63 655f 6c65 6e67 7468  (sequence_length
-00000bf0: 2c20 6e75 6d5f 7461 6773 293a 0a20 2020  , num_tags):.   
-00000c00: 2020 2020 2020 2020 2074 6167 5f69 6e64           tag_ind
-00000c10: 6963 6573 5f73 636f 7265 203d 2028 0a20  ices_score = (. 
-00000c20: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00000c30: 6f67 5f70 6f74 656e 7469 616c 735b 622c  og_potentials[b,
-00000c40: 2030 2c20 7461 675f 696e 6469 6365 735b   0, tag_indices[
-00000c50: 305d 2c20 7461 675f 696e 6469 6365 735b  0], tag_indices[
-00000c60: 305d 5d2e 6465 7461 6368 2829 2e63 6c6f  0]].detach().clo
-00000c70: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
-00000c80: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-00000c90: 6f72 2069 2c20 286a 2c20 6b29 2069 6e20  or i, (j, k) in 
-00000ca0: 656e 756d 6572 6174 6528 7a69 7028 7461  enumerate(zip(ta
-00000cb0: 675f 696e 6469 6365 735b 3a2d 315d 2c20  g_indices[:-1], 
-00000cc0: 7461 675f 696e 6469 6365 735b 313a 5d29  tag_indices[1:])
-00000cd0: 2c20 3129 3a0a 2020 2020 2020 2020 2020  , 1):.          
-00000ce0: 2020 2020 2020 7461 675f 696e 6469 6365        tag_indice
-00000cf0: 735f 7363 6f72 6520 2b3d 206c 6f67 5f70  s_score += log_p
-00000d00: 6f74 656e 7469 616c 735b 622c 2069 2c20  otentials[b, i, 
-00000d10: 6a2c 206b 5d0a 2020 2020 2020 2020 2020  j, k].          
-00000d20: 2020 6966 2074 6167 5f69 6e64 6963 6573    if tag_indices
-00000d30: 5f73 636f 7265 2e67 7428 6d61 785f 7363  _score.gt(max_sc
-00000d40: 6f72 6529 3a0a 2020 2020 2020 2020 2020  ore):.          
-00000d50: 2020 2020 2020 2320 4967 6e6f 7265 2074        # Ignore t
-00000d60: 6865 2064 756d 6d79 2069 6e69 7469 616c  he dummy initial
-00000d70: 2073 7461 7465 0a20 2020 2020 2020 2020   state.         
-00000d80: 2020 2020 2020 2062 6573 745f 7461 675f         best_tag_
-00000d90: 696e 6469 6365 735b 625d 203d 2074 6f72  indices[b] = tor
-00000da0: 6368 2e74 656e 736f 7228 7461 675f 696e  ch.tensor(tag_in
-00000db0: 6469 6365 7329 0a20 2020 2020 2020 2020  dices).         
-00000dc0: 2020 2020 2020 206d 6178 5f73 636f 7265         max_score
-00000dd0: 203d 2074 6167 5f69 6e64 6963 6573 5f73   = tag_indices_s
-00000de0: 636f 7265 0a20 2020 2020 2020 206d 6178  core.        max
-00000df0: 5f73 636f 7265 735b 625d 203d 206d 6178  _scores[b] = max
-00000e00: 5f73 636f 7265 0a20 2020 2072 6574 7572  _score.    retur
-00000e10: 6e20 6d61 785f 7363 6f72 6573 2c20 6265  n max_scores, be
-00000e20: 7374 5f74 6167 5f69 6e64 6963 6573 0a0a  st_tag_indices..
-00000e30: 0a64 6566 2063 6865 636b 5f74 6167 5f69  .def check_tag_i
-00000e40: 6e64 6963 6573 5f73 6174 6973 6669 6573  ndices_satisfies
-00000e50: 5f63 6f6e 7374 7261 696e 7473 280a 2020  _constraints(.  
-00000e60: 2020 7461 675f 696e 6469 6365 733a 2074    tag_indices: t
-00000e70: 6f72 6368 2e54 656e 736f 722c 0a20 2020  orch.Tensor,.   
-00000e80: 2073 7461 7274 5f63 6f6e 7374 7261 696e   start_constrain
-00000e90: 7473 3a20 746f 7263 682e 5465 6e73 6f72  ts: torch.Tensor
-00000ea0: 2c0a 2020 2020 656e 645f 636f 6e73 7472  ,.    end_constr
-00000eb0: 6169 6e74 733a 2074 6f72 6368 2e54 656e  aints: torch.Ten
-00000ec0: 736f 722c 0a20 2020 2074 7261 6e73 6974  sor,.    transit
-00000ed0: 696f 6e5f 636f 6e73 7472 6169 6e74 733a  ion_constraints:
-00000ee0: 2074 6f72 6368 2e54 656e 736f 722c 0a29   torch.Tensor,.)
-00000ef0: 202d 3e20 626f 6f6c 3a0a 2020 2020 7365   -> bool:.    se
-00000f00: 7175 656e 6365 5f6c 656e 6774 6820 3d20  quence_length = 
-00000f10: 7461 675f 696e 6469 6365 732e 7369 7a65  tag_indices.size
-00000f20: 282d 3129 0a20 2020 2066 6f72 2074 6167  (-1).    for tag
-00000f30: 7320 696e 2074 6167 5f69 6e64 6963 6573  s in tag_indices
-00000f40: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00000f50: 2073 7461 7274 5f63 6f6e 7374 7261 696e   start_constrain
-00000f60: 7473 5b74 6167 735b 305d 5d3a 0a20 2020  ts[tags[0]]:.   
-00000f70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000f80: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-00000f90: 206e 6f74 2065 6e64 5f63 6f6e 7374 7261   not end_constra
-00000fa0: 696e 7473 5b74 6167 735b 2d31 5d5d 3a0a  ints[tags[-1]]:.
-00000fb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000fc0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-00000fd0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00000fe0: 7365 7175 656e 6365 5f6c 656e 6774 6820  sequence_length 
-00000ff0: 2d20 3129 3a0a 2020 2020 2020 2020 2020  - 1):.          
-00001000: 2020 6966 206e 6f74 2074 7261 6e73 6974    if not transit
-00001010: 696f 6e5f 636f 6e73 7472 6169 6e74 735b  ion_constraints[
-00001020: 7461 6773 5b69 5d2c 2074 6167 735b 6920  tags[i], tags[i 
-00001030: 2b20 315d 5d3a 0a20 2020 2020 2020 2020  + 1]]:.         
-00001040: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00001050: 6c73 650a 2020 2020 7265 7475 726e 2054  lse.    return T
-00001060: 7275 650a 0a0a 6465 6620 6368 6563 6b5f  rue...def check_
-00001070: 6c6f 675f 706f 7465 6e74 6961 6c73 5f6d  log_potentials_m
-00001080: 6173 6b65 645f 636f 7272 6563 746c 7928  asked_correctly(
-00001090: 0a20 2020 206c 6f67 5f70 6f74 656e 7469  .    log_potenti
-000010a0: 616c 733a 2074 6f72 6368 2e54 656e 736f  als: torch.Tenso
-000010b0: 722c 206d 6173 6b3a 2074 6f72 6368 2e54  r, mask: torch.T
-000010c0: 656e 736f 720a 2920 2d3e 2062 6f6f 6c3a  ensor.) -> bool:
-000010d0: 0a20 2020 2073 6571 7565 6e63 655f 6c65  .    sequence_le
-000010e0: 6e67 7468 203d 206c 6f67 5f70 6f74 656e  ngth = log_poten
-000010f0: 7469 616c 732e 7369 7a65 2831 290a 2020  tials.size(1).  
-00001100: 2020 6e75 6d5f 7461 6773 203d 206c 6f67    num_tags = log
-00001110: 5f70 6f74 656e 7469 616c 732e 7369 7a65  _potentials.size
-00001120: 282d 3129 0a20 2020 206d 6173 6b5f 7661  (-1).    mask_va
-00001130: 6c75 6520 3d20 287e 746f 7263 682e 6579  lue = (~torch.ey
-00001140: 6528 6e75 6d5f 7461 6773 2c20 6e75 6d5f  e(num_tags, num_
-00001150: 7461 6773 292e 626f 6f6c 2829 292e 6d75  tags).bool()).mu
-00001160: 6c28 4e49 4e46 290a 2020 2020 6c65 6e67  l(NINF).    leng
-00001170: 7468 7320 3d20 6d61 736b 2e73 756d 2864  ths = mask.sum(d
-00001180: 696d 3d2d 3129 0a20 2020 2066 6f72 2062  im=-1).    for b
-00001190: 2c20 7265 616c 5f73 6571 7565 6e63 655f  , real_sequence_
-000011a0: 6c65 6e67 7468 2069 6e20 656e 756d 6572  length in enumer
-000011b0: 6174 6528 6c65 6e67 7468 7329 3a0a 2020  ate(lengths):.  
-000011c0: 2020 2020 2020 666f 7220 4c20 696e 2072        for L in r
-000011d0: 616e 6765 2872 6561 6c5f 7365 7175 656e  ange(real_sequen
-000011e0: 6365 5f6c 656e 6774 682c 2073 6571 7565  ce_length, seque
-000011f0: 6e63 655f 6c65 6e67 7468 293a 0a20 2020  nce_length):.   
-00001200: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00001210: 746f 7263 682e 616c 6c63 6c6f 7365 286c  torch.allclose(l
-00001220: 6f67 5f70 6f74 656e 7469 616c 735b 622c  og_potentials[b,
-00001230: 204c 5d2c 206d 6173 6b5f 7661 6c75 6529   L], mask_value)
-00001240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001250: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00001260: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00001270: 0a64 6566 2063 6865 636b 5f6c 6f67 5f70  .def check_log_p
-00001280: 6f74 656e 7469 616c 735f 6265 6861 7665  otentials_behave
-00001290: 735f 6173 5f70 726f 6261 6269 6c69 7479  s_as_probability
-000012a0: 286c 6f67 5f70 6f74 656e 7469 616c 733a  (log_potentials:
-000012b0: 2074 6f72 6368 2e54 656e 736f 7229 202d   torch.Tensor) -
-000012c0: 3e20 626f 6f6c 3a0a 2020 2020 6261 7463  > bool:.    batc
-000012d0: 685f 7369 7a65 203d 206c 6f67 5f70 6f74  h_size = log_pot
-000012e0: 656e 7469 616c 732e 7369 7a65 2830 290a  entials.size(0).
-000012f0: 2020 2020 7365 7175 656e 6365 5f6c 656e      sequence_len
-00001300: 6774 6820 3d20 6c6f 675f 706f 7465 6e74  gth = log_potent
-00001310: 6961 6c73 2e73 697a 6528 3129 0a20 2020  ials.size(1).   
-00001320: 206e 756d 5f74 6167 7320 3d20 6c6f 675f   num_tags = log_
-00001330: 706f 7465 6e74 6961 6c73 2e73 697a 6528  potentials.size(
-00001340: 3229 0a20 2020 206c 6f67 5f70 726f 6261  2).    log_proba
-00001350: 6269 6c69 7479 203d 2074 6f72 6368 2e74  bility = torch.t
-00001360: 656e 736f 7228 5b4e 494e 465d 202a 2062  ensor([NINF] * b
-00001370: 6174 6368 5f73 697a 6529 0a20 2020 2066  atch_size).    f
-00001380: 6f72 2074 6167 5f69 6e64 6963 6573 2069  or tag_indices i
-00001390: 6e20 6974 6572 6174 655f 706f 7373 6962  n iterate_possib
-000013a0: 6c65 5f74 6167 5f69 6e64 6963 6573 2873  le_tag_indices(s
-000013b0: 6571 7565 6e63 655f 6c65 6e67 7468 2c20  equence_length, 
-000013c0: 6e75 6d5f 7461 6773 293a 0a20 2020 2020  num_tags):.     
-000013d0: 2020 206c 6f67 5f70 726f 6261 6269 6c69     log_probabili
-000013e0: 7479 203d 2074 6f72 6368 2e6c 6f67 6164  ty = torch.logad
-000013f0: 6465 7870 280a 2020 2020 2020 2020 2020  dexp(.          
-00001400: 2020 6c6f 675f 7072 6f62 6162 696c 6974    log_probabilit
-00001410: 792c 2046 2e6c 6f67 5f6c 696b 656c 6968  y, F.log_likelih
-00001420: 6f6f 6428 6c6f 675f 706f 7465 6e74 6961  ood(log_potentia
-00001430: 6c73 2c20 746f 7263 682e 7465 6e73 6f72  ls, torch.tensor
-00001440: 2874 6167 5f69 6e64 6963 6573 2929 0a20  (tag_indices)). 
-00001450: 2020 2020 2020 2029 0a20 2020 2072 6574         ).    ret
-00001460: 7572 6e20 746f 7263 682e 616c 6c63 6c6f  urn torch.allclo
-00001470: 7365 286c 6f67 5f70 726f 6261 6269 6c69  se(log_probabili
-00001480: 7479 2e65 7870 2829 2c20 746f 7263 682e  ty.exp(), torch.
-00001490: 6f6e 6573 5f6c 696b 6528 6c6f 675f 7072  ones_like(log_pr
-000014a0: 6f62 6162 696c 6974 7929 290a 0a0a 6465  obability))...de
-000014b0: 6620 6368 6563 6b5f 7365 7175 656e 6365  f check_sequence
-000014c0: 5f73 636f 7265 5f6d 6173 6b28 0a20 2020  _score_mask(.   
-000014d0: 2075 7365 645f 6d61 736b 3a20 746f 7263   used_mask: torc
-000014e0: 682e 5465 6e73 6f72 2c20 7461 675f 696e  h.Tensor, tag_in
-000014f0: 6469 6365 733a 2074 6f72 6368 2e54 656e  dices: torch.Ten
-00001500: 736f 722c 206d 6173 6b3a 2074 6f72 6368  sor, mask: torch
-00001510: 2e54 656e 736f 720a 2920 2d3e 2062 6f6f  .Tensor.) -> boo
-00001520: 6c3a 0a20 2020 206e 756d 5f74 6167 7320  l:.    num_tags 
-00001530: 3d20 7573 6564 5f6d 6173 6b2e 7369 7a65  = used_mask.size
-00001540: 282d 3129 0a20 2020 206c 656e 6774 6873  (-1).    lengths
-00001550: 203d 206d 6173 6b2e 7375 6d28 6469 6d3d   = mask.sum(dim=
-00001560: 2d31 290a 2020 2020 666f 7220 622c 2072  -1).    for b, r
-00001570: 6561 6c5f 7365 7175 656e 6365 5f6c 656e  eal_sequence_len
-00001580: 6774 6820 696e 2065 6e75 6d65 7261 7465  gth in enumerate
-00001590: 286c 656e 6774 6873 293a 0a20 2020 2020  (lengths):.     
-000015a0: 2020 2023 206f 6e6c 7920 2869 2c20 6a29     # only (i, j)
-000015b0: 2069 7320 5472 7565 2c20 6f74 6865 7277   is True, otherw
-000015c0: 6973 6520 4661 6c73 650a 2020 2020 2020  ise False.      
-000015d0: 2020 7461 6773 203d 2074 6167 5f69 6e64    tags = tag_ind
-000015e0: 6963 6573 5b62 2c20 3a72 6561 6c5f 7365  ices[b, :real_se
-000015f0: 7175 656e 6365 5f6c 656e 6774 685d 2e74  quence_length].t
-00001600: 6f6c 6973 7428 290a 2020 2020 2020 2020  olist().        
-00001610: 7461 6773 203d 205b 7461 6773 5b30 5d5d  tags = [tags[0]]
-00001620: 202b 2074 6167 730a 2020 2020 2020 2020   + tags.        
-00001630: 666f 7220 706f 732c 2028 692c 206a 2920  for pos, (i, j) 
-00001640: 696e 2065 6e75 6d65 7261 7465 287a 6970  in enumerate(zip
-00001650: 2874 6167 735b 3a2d 315d 2c20 7461 6773  (tags[:-1], tags
-00001660: 5b31 3a5d 2929 3a0a 2020 2020 2020 2020  [1:])):.        
-00001670: 2020 2020 6966 206e 6f74 2075 7365 645f      if not used_
-00001680: 6d61 736b 5b62 2c20 706f 732c 2069 2c20  mask[b, pos, i, 
-00001690: 6a5d 3a0a 2020 2020 2020 2020 2020 2020  j]:.            
-000016a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000016b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000016c0: 2078 2069 6e20 7261 6e67 6528 6e75 6d5f   x in range(num_
-000016d0: 7461 6773 293a 0a20 2020 2020 2020 2020  tags):.         
-000016e0: 2020 2020 2020 2066 6f72 2079 2069 6e20         for y in 
-000016f0: 7261 6e67 6528 6e75 6d5f 7461 6773 293a  range(num_tags):
-00001700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001710: 2020 2020 2069 6620 7820 3d3d 2069 2061       if x == i a
-00001720: 6e64 2079 203d 3d20 6a3a 0a20 2020 2020  nd y == j:.     
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001760: 6966 2075 7365 645f 6d61 736b 5b62 2c20  if used_mask[b, 
-00001770: 706f 732c 2078 2c20 795d 3a0a 2020 2020  pos, x, y]:.    
-00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001790: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000017a0: 0a0a 2020 2020 2020 2020 2320 616c 6c20  ..        # all 
-000017b0: 7661 6c75 6573 2073 686f 756c 6420 6265  values should be
-000017c0: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-000017d0: 6967 6e6f 7265 7320 3d20 7573 6564 5f6d  ignores = used_m
-000017e0: 6173 6b5b 622c 2072 6561 6c5f 7365 7175  ask[b, real_sequ
-000017f0: 656e 6365 5f6c 656e 6774 683a 5d0a 2020  ence_length:].  
-00001800: 2020 2020 2020 6966 206e 6f74 2074 6f72        if not tor
-00001810: 6368 2e65 7175 616c 2869 676e 6f72 6573  ch.equal(ignores
-00001820: 2c20 746f 7263 682e 7a65 726f 735f 6c69  , torch.zeros_li
-00001830: 6b65 2869 676e 6f72 6573 2c20 6474 7970  ke(ignores, dtyp
-00001840: 653d 746f 7263 682e 626f 6f6c 2929 3a0a  e=torch.bool)):.
-00001850: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001860: 726e 2046 616c 7365 0a20 2020 2072 6574  rn False.    ret
-00001870: 7572 6e20 5472 7565 0a0a 0a64 6566 2063  urn True...def c
-00001880: 6865 636b 5f63 6f6e 7374 7261 696e 6564  heck_constrained
-00001890: 5f6c 6f67 5f70 6f74 656e 7469 616c 7328  _log_potentials(
-000018a0: 0a20 2020 206c 6f67 5f70 6f74 656e 7469  .    log_potenti
-000018b0: 616c 733a 2074 6f72 6368 2e54 656e 736f  als: torch.Tenso
-000018c0: 722c 0a20 2020 2063 6f6e 7374 7261 696e  r,.    constrain
-000018d0: 6564 5f6c 6f67 5f70 6f74 656e 7469 616c  ed_log_potential
-000018e0: 733a 2074 6f72 6368 2e54 656e 736f 722c  s: torch.Tensor,
-000018f0: 0a20 2020 2074 6167 5f69 6e64 6963 6573  .    tag_indices
-00001900: 3a20 746f 7263 682e 5465 6e73 6f72 2c0a  : torch.Tensor,.
-00001910: 2020 2020 6d61 736b 3a20 746f 7263 682e      mask: torch.
-00001920: 5465 6e73 6f72 2c0a 2020 2020 7061 7274  Tensor,.    part
-00001930: 6961 6c5f 696e 6465 783a 2069 6e74 2c0a  ial_index: int,.
-00001940: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 206e  ) -> bool:.    n
-00001950: 756d 5f74 6167 7320 3d20 6c6f 675f 706f  um_tags = log_po
-00001960: 7465 6e74 6961 6c73 2e73 697a 6528 2d31  tentials.size(-1
-00001970: 290a 2020 2020 6c65 6e67 7468 7320 3d20  ).    lengths = 
-00001980: 6d61 736b 2e73 756d 2864 696d 3d2d 3129  mask.sum(dim=-1)
-00001990: 0a20 2020 2066 6f72 2062 2c20 7265 616c  .    for b, real
-000019a0: 5f73 6571 7565 6e63 655f 6c65 6e67 7468  _sequence_length
-000019b0: 2069 6e20 656e 756d 6572 6174 6528 6c65   in enumerate(le
-000019c0: 6e67 7468 7329 3a0a 2020 2020 2020 2020  ngths):.        
-000019d0: 7461 6773 203d 2074 6167 5f69 6e64 6963  tags = tag_indic
-000019e0: 6573 5b62 2c20 3a72 6561 6c5f 7365 7175  es[b, :real_sequ
-000019f0: 656e 6365 5f6c 656e 6774 685d 2e74 6f6c  ence_length].tol
-00001a00: 6973 7428 290a 2020 2020 2020 2020 7461  ist().        ta
-00001a10: 6773 203d 205b 7461 6773 5b30 5d5d 202b  gs = [tags[0]] +
-00001a20: 2074 6167 730a 2020 2020 2020 2020 666f   tags.        fo
-00001a30: 7220 706f 732c 2028 692c 206a 2920 696e  r pos, (i, j) in
-00001a40: 2065 6e75 6d65 7261 7465 287a 6970 2874   enumerate(zip(t
-00001a50: 6167 735b 3a2d 315d 2c20 7461 6773 5b31  ags[:-1], tags[1
-00001a60: 3a5d 2929 3a0a 2020 2020 2020 2020 2020  :])):.          
-00001a70: 2020 6966 2069 203d 3d20 7061 7274 6961    if i == partia
-00001a80: 6c5f 696e 6465 7820 616e 6420 6a20 3d3d  l_index and j ==
-00001a90: 2070 6172 7469 616c 5f69 6e64 6578 3a0a   partial_index:.
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 7820 3d20 636f 6e73 7472 6169 6e65 645f  x = constrained_
-00001ac0: 6c6f 675f 706f 7465 6e74 6961 6c73 5b62  log_potentials[b
-00001ad0: 2c20 706f 735d 0a20 2020 2020 2020 2020  , pos].         
-00001ae0: 2020 2020 2020 2079 203d 206c 6f67 5f70         y = log_p
-00001af0: 6f74 656e 7469 616c 735b 622c 2070 6f73  otentials[b, pos
-00001b00: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-00001b10: 6966 2069 203d 3d20 7061 7274 6961 6c5f  if i == partial_
-00001b20: 696e 6465 783a 0a20 2020 2020 2020 2020  index:.         
-00001b30: 2020 2020 2020 2066 6f72 206e 2069 6e20         for n in 
-00001b40: 7261 6e67 6528 6e75 6d5f 7461 6773 293a  range(num_tags):
-00001b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b60: 2020 2020 2069 6620 6e20 3d3d 206a 3a0a       if n == j:.
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00000000: 6672 6f6d 2069 7465 7274 6f6f 6c73 2069  from itertools i
+00000010: 6d70 6f72 7420 7072 6f64 7563 740a 6672  mport product.fr
+00000020: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000030: 2047 656e 6572 6174 6f72 2c20 5475 706c   Generator, Tupl
+00000040: 650a 0a69 6d70 6f72 7420 746f 7263 680a  e..import torch.
+00000050: 6672 6f6d 2070 6172 7469 616c 5f74 6167  from partial_tag
+00000060: 6765 722e 6372 6620 696d 706f 7274 204e  ger.crf import N
+00000070: 494e 460a 6672 6f6d 2070 6172 7469 616c  INF.from partial
+00000080: 5f74 6167 6765 722e 6372 6620 696d 706f  _tagger.crf impo
+00000090: 7274 2066 756e 6374 696f 6e61 6c20 6173  rt functional as
+000000a0: 2046 0a0a 0a64 6566 2069 7465 7261 7465   F...def iterate
+000000b0: 5f70 6f73 7369 626c 655f 7461 675f 696e  _possible_tag_in
+000000c0: 6469 6365 7328 0a20 2020 2073 6571 7565  dices(.    seque
+000000d0: 6e63 655f 6c65 6e67 7468 3a20 696e 742c  nce_length: int,
+000000e0: 206e 756d 5f74 6167 733a 2069 6e74 0a29   num_tags: int.)
+000000f0: 202d 3e20 4765 6e65 7261 746f 725b 7475   -> Generator[tu
+00000100: 706c 652c 204e 6f6e 652c 204e 6f6e 655d  ple, None, None]
+00000110: 3a0a 2020 2020 7969 656c 6420 6672 6f6d  :.    yield from
+00000120: 2070 726f 6475 6374 2872 616e 6765 286e   product(range(n
+00000130: 756d 5f74 6167 7329 2c20 7265 7065 6174  um_tags), repeat
+00000140: 3d73 6571 7565 6e63 655f 6c65 6e67 7468  =sequence_length
+00000150: 290a 0a0a 6465 6620 6974 6572 6174 655f  )...def iterate_
+00000160: 706f 7373 6962 6c65 5f6f 6e65 5f68 6f74  possible_one_hot
+00000170: 5f74 6167 5f62 6974 6d61 7028 0a20 2020  _tag_bitmap(.   
+00000180: 2062 6174 6368 5f73 697a 653a 2069 6e74   batch_size: int
+00000190: 2c20 7365 7175 656e 6365 5f6c 656e 6774  , sequence_lengt
+000001a0: 683a 2069 6e74 2c20 6e75 6d5f 7461 6773  h: int, num_tags
+000001b0: 3a20 696e 740a 2920 2d3e 2047 656e 6572  : int.) -> Gener
+000001c0: 6174 6f72 5b74 6f72 6368 2e54 656e 736f  ator[torch.Tenso
+000001d0: 722c 204e 6f6e 652c 204e 6f6e 655d 3a0a  r, None, None]:.
+000001e0: 2020 2020 666f 7220 7461 675f 696e 6469      for tag_indi
+000001f0: 6365 7320 696e 2069 7465 7261 7465 5f70  ces in iterate_p
+00000200: 6f73 7369 626c 655f 7461 675f 696e 6469  ossible_tag_indi
+00000210: 6365 7328 7365 7175 656e 6365 5f6c 656e  ces(sequence_len
+00000220: 6774 682c 206e 756d 5f74 6167 7329 3a0a  gth, num_tags):.
+00000230: 2020 2020 2020 2020 7461 675f 6269 746d          tag_bitm
+00000240: 6170 203d 205b 5d0a 2020 2020 2020 2020  ap = [].        
+00000250: 666f 7220 6163 7469 7665 2069 6e20 7461  for active in ta
+00000260: 675f 696e 6469 6365 733a 0a20 2020 2020  g_indices:.     
+00000270: 2020 2020 2020 2062 6974 6d61 7020 3d20         bitmap = 
+00000280: 5b46 616c 7365 5d20 2a20 6e75 6d5f 7461  [False] * num_ta
+00000290: 6773 0a20 2020 2020 2020 2020 2020 2062  gs.            b
+000002a0: 6974 6d61 705b 6163 7469 7665 5d20 3d20  itmap[active] = 
+000002b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+000002c0: 2074 6167 5f62 6974 6d61 702e 6170 7065   tag_bitmap.appe
+000002d0: 6e64 2862 6974 6d61 7029 0a20 2020 2020  nd(bitmap).     
+000002e0: 2020 2079 6965 6c64 2074 6f72 6368 2e74     yield torch.t
+000002f0: 656e 736f 7228 5b74 6167 5f62 6974 6d61  ensor([tag_bitma
+00000300: 705d 202a 2062 6174 6368 5f73 697a 6529  p] * batch_size)
+00000310: 0a0a 0a64 6566 2063 6f6d 7075 7465 5f6c  ...def compute_l
+00000320: 6f67 5f6e 6f72 6d61 6c69 7a65 725f 6279  og_normalizer_by
+00000330: 5f62 7275 7465 5f66 6f72 6365 286c 6f67  _brute_force(log
+00000340: 5f70 6f74 656e 7469 616c 733a 2074 6f72  _potentials: tor
+00000350: 6368 2e54 656e 736f 7229 202d 3e20 746f  ch.Tensor) -> to
+00000360: 7263 682e 5465 6e73 6f72 3a0a 2020 2020  rch.Tensor:.    
+00000370: 6261 7463 685f 7369 7a65 2c20 7365 7175  batch_size, sequ
+00000380: 656e 6365 5f6c 656e 6774 682c 206e 756d  ence_length, num
+00000390: 5f74 6167 732c 205f 203d 206c 6f67 5f70  _tags, _ = log_p
+000003a0: 6f74 656e 7469 616c 732e 7369 7a65 2829  otentials.size()
+000003b0: 0a20 2020 206c 6f67 5f5a 203d 2074 6f72  .    log_Z = tor
+000003c0: 6368 2e74 656e 736f 7228 5b4e 494e 465d  ch.tensor([NINF]
+000003d0: 202a 2062 6174 6368 5f73 697a 6529 0a20   * batch_size). 
+000003e0: 2020 2066 6f72 2062 2069 6e20 7261 6e67     for b in rang
+000003f0: 6528 6261 7463 685f 7369 7a65 293a 0a20  e(batch_size):. 
+00000400: 2020 2020 2020 2066 6f72 2074 6167 5f69         for tag_i
+00000410: 6e64 6963 6573 2069 6e20 6974 6572 6174  ndices in iterat
+00000420: 655f 706f 7373 6962 6c65 5f74 6167 5f69  e_possible_tag_i
+00000430: 6e64 6963 6573 2873 6571 7565 6e63 655f  ndices(sequence_
+00000440: 6c65 6e67 7468 202b 2031 2c20 6e75 6d5f  length + 1, num_
+00000450: 7461 6773 293a 0a20 2020 2020 2020 2020  tags):.         
+00000460: 2020 2074 6167 5f69 6e64 6963 6573 5f73     tag_indices_s
+00000470: 636f 7265 203d 2074 6f72 6368 2e74 656e  core = torch.ten
+00000480: 736f 7228 302e 3029 0a20 2020 2020 2020  sor(0.0).       
+00000490: 2020 2020 2066 6f72 2069 2c20 286a 2c20       for i, (j, 
+000004a0: 6b29 2069 6e20 656e 756d 6572 6174 6528  k) in enumerate(
+000004b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004c0: 207a 6970 2874 6167 5f69 6e64 6963 6573   zip(tag_indices
+000004d0: 5b3a 2d31 5d2c 2074 6167 5f69 6e64 6963  [:-1], tag_indic
+000004e0: 6573 5b31 3a5d 2c20 7374 7269 6374 3d54  es[1:], strict=T
+000004f0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00000500: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00000510: 2020 2020 7461 675f 696e 6469 6365 735f      tag_indices_
+00000520: 7363 6f72 6520 2b3d 206c 6f67 5f70 6f74  score += log_pot
+00000530: 656e 7469 616c 735b 622c 2069 2c20 6a2c  entials[b, i, j,
+00000540: 206b 5d0a 2020 2020 2020 2020 2020 2020   k].            
+00000550: 6c6f 675f 5a5b 625d 203d 2074 6f72 6368  log_Z[b] = torch
+00000560: 2e6c 6f67 6164 6465 7870 286c 6f67 5f5a  .logaddexp(log_Z
+00000570: 5b62 5d2c 2074 6167 5f69 6e64 6963 6573  [b], tag_indices
+00000580: 5f73 636f 7265 290a 2020 2020 7265 7475  _score).    retu
+00000590: 726e 206c 6f67 5f5a 0a0a 0a64 6566 2063  rn log_Z...def c
+000005a0: 6f6d 7075 7465 5f62 6573 745f 7461 675f  ompute_best_tag_
+000005b0: 696e 6469 6365 735f 6279 5f62 7275 7465  indices_by_brute
+000005c0: 5f66 6f72 6365 280a 2020 2020 6c6f 675f  _force(.    log_
+000005d0: 706f 7465 6e74 6961 6c73 3a20 746f 7263  potentials: torc
+000005e0: 682e 5465 6e73 6f72 2c0a 2920 2d3e 2054  h.Tensor,.) -> T
+000005f0: 7570 6c65 5b74 6f72 6368 2e54 656e 736f  uple[torch.Tenso
+00000600: 722c 2074 6f72 6368 2e54 656e 736f 725d  r, torch.Tensor]
+00000610: 3a0a 2020 2020 6261 7463 685f 7369 7a65  :.    batch_size
+00000620: 2c20 7365 7175 656e 6365 5f6c 656e 6774  , sequence_lengt
+00000630: 682c 206e 756d 5f74 6167 732c 205f 203d  h, num_tags, _ =
+00000640: 206c 6f67 5f70 6f74 656e 7469 616c 732e   log_potentials.
+00000650: 7369 7a65 2829 0a20 2020 2062 6573 745f  size().    best_
+00000660: 7461 675f 696e 6469 6365 7320 3d20 746f  tag_indices = to
+00000670: 7263 682e 7465 6e73 6f72 285b 5b2d 315d  rch.tensor([[-1]
+00000680: 202a 2073 6571 7565 6e63 655f 6c65 6e67   * sequence_leng
+00000690: 7468 2066 6f72 205f 2069 6e20 7261 6e67  th for _ in rang
+000006a0: 6528 6261 7463 685f 7369 7a65 295d 290a  e(batch_size)]).
+000006b0: 2020 2020 6d61 785f 7363 6f72 6573 203d      max_scores =
+000006c0: 2074 6f72 6368 2e74 656e 736f 7228 5b4e   torch.tensor([N
+000006d0: 494e 465d 202a 2062 6174 6368 5f73 697a  INF] * batch_siz
+000006e0: 6529 0a20 2020 2066 6f72 2062 2069 6e20  e).    for b in 
+000006f0: 7261 6e67 6528 6261 7463 685f 7369 7a65  range(batch_size
+00000700: 293a 0a20 2020 2020 2020 206d 6178 5f73  ):.        max_s
+00000710: 636f 7265 203d 2074 6f72 6368 2e74 656e  core = torch.ten
+00000720: 736f 7228 4e49 4e46 290a 2020 2020 2020  sor(NINF).      
+00000730: 2020 666f 7220 7461 675f 696e 6469 6365    for tag_indice
+00000740: 7320 696e 2069 7465 7261 7465 5f70 6f73  s in iterate_pos
+00000750: 7369 626c 655f 7461 675f 696e 6469 6365  sible_tag_indice
+00000760: 7328 7365 7175 656e 6365 5f6c 656e 6774  s(sequence_lengt
+00000770: 682c 206e 756d 5f74 6167 7329 3a0a 2020  h, num_tags):.  
+00000780: 2020 2020 2020 2020 2020 7461 675f 696e            tag_in
+00000790: 6469 6365 735f 7363 6f72 6520 3d20 280a  dices_score = (.
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 6c6f 675f 706f 7465 6e74 6961 6c73 5b62  log_potentials[b
+000007c0: 2c20 302c 2074 6167 5f69 6e64 6963 6573  , 0, tag_indices
+000007d0: 5b30 5d2c 2074 6167 5f69 6e64 6963 6573  [0], tag_indices
+000007e0: 5b30 5d5d 2e64 6574 6163 6828 292e 636c  [0]].detach().cl
+000007f0: 6f6e 6528 290a 2020 2020 2020 2020 2020  one().          
+00000800: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00000810: 666f 7220 692c 2028 6a2c 206b 2920 696e  for i, (j, k) in
+00000820: 2065 6e75 6d65 7261 7465 280a 2020 2020   enumerate(.    
+00000830: 2020 2020 2020 2020 2020 2020 7a69 7028              zip(
+00000840: 7461 675f 696e 6469 6365 735b 3a2d 315d  tag_indices[:-1]
+00000850: 2c20 7461 675f 696e 6469 6365 735b 313a  , tag_indices[1:
+00000860: 5d2c 2073 7472 6963 743d 5472 7565 292c  ], strict=True),
+00000870: 2031 0a20 2020 2020 2020 2020 2020 2029   1.            )
+00000880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000890: 2020 7461 675f 696e 6469 6365 735f 7363    tag_indices_sc
+000008a0: 6f72 6520 2b3d 206c 6f67 5f70 6f74 656e  ore += log_poten
+000008b0: 7469 616c 735b 622c 2069 2c20 6a2c 206b  tials[b, i, j, k
+000008c0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+000008d0: 2074 6167 5f69 6e64 6963 6573 5f73 636f   tag_indices_sco
+000008e0: 7265 2e67 7428 6d61 785f 7363 6f72 6529  re.gt(max_score)
+000008f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000900: 2020 2320 4967 6e6f 7265 2074 6865 2064    # Ignore the d
+00000910: 756d 6d79 2069 6e69 7469 616c 2073 7461  ummy initial sta
+00000920: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+00000930: 2020 2062 6573 745f 7461 675f 696e 6469     best_tag_indi
+00000940: 6365 735b 625d 203d 2074 6f72 6368 2e74  ces[b] = torch.t
+00000950: 656e 736f 7228 7461 675f 696e 6469 6365  ensor(tag_indice
+00000960: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00000970: 2020 206d 6178 5f73 636f 7265 203d 2074     max_score = t
+00000980: 6167 5f69 6e64 6963 6573 5f73 636f 7265  ag_indices_score
+00000990: 0a20 2020 2020 2020 206d 6178 5f73 636f  .        max_sco
+000009a0: 7265 735b 625d 203d 206d 6178 5f73 636f  res[b] = max_sco
+000009b0: 7265 0a20 2020 2072 6574 7572 6e20 6d61  re.    return ma
+000009c0: 785f 7363 6f72 6573 2c20 6265 7374 5f74  x_scores, best_t
+000009d0: 6167 5f69 6e64 6963 6573 0a0a 0a64 6566  ag_indices...def
+000009e0: 2063 6865 636b 5f74 6167 5f69 6e64 6963   check_tag_indic
+000009f0: 6573 5f73 6174 6973 6669 6573 5f63 6f6e  es_satisfies_con
+00000a00: 7374 7261 696e 7473 280a 2020 2020 7461  straints(.    ta
+00000a10: 675f 696e 6469 6365 733a 2074 6f72 6368  g_indices: torch
+00000a20: 2e54 656e 736f 722c 0a20 2020 2073 7461  .Tensor,.    sta
+00000a30: 7274 5f63 6f6e 7374 7261 696e 7473 3a20  rt_constraints: 
+00000a40: 746f 7263 682e 5465 6e73 6f72 2c0a 2020  torch.Tensor,.  
+00000a50: 2020 656e 645f 636f 6e73 7472 6169 6e74    end_constraint
+00000a60: 733a 2074 6f72 6368 2e54 656e 736f 722c  s: torch.Tensor,
+00000a70: 0a20 2020 2074 7261 6e73 6974 696f 6e5f  .    transition_
+00000a80: 636f 6e73 7472 6169 6e74 733a 2074 6f72  constraints: tor
+00000a90: 6368 2e54 656e 736f 722c 0a29 202d 3e20  ch.Tensor,.) -> 
+00000aa0: 626f 6f6c 3a0a 2020 2020 7365 7175 656e  bool:.    sequen
+00000ab0: 6365 5f6c 656e 6774 6820 3d20 7461 675f  ce_length = tag_
+00000ac0: 696e 6469 6365 732e 7369 7a65 282d 3129  indices.size(-1)
+00000ad0: 0a20 2020 2066 6f72 2074 6167 7320 696e  .    for tags in
+00000ae0: 2074 6167 5f69 6e64 6963 6573 3a0a 2020   tag_indices:.  
+00000af0: 2020 2020 2020 6966 206e 6f74 2073 7461        if not sta
+00000b00: 7274 5f63 6f6e 7374 7261 696e 7473 5b74  rt_constraints[t
+00000b10: 6167 735b 305d 5d3a 0a20 2020 2020 2020  ags[0]]:.       
+00000b20: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00000b30: 650a 2020 2020 2020 2020 6966 206e 6f74  e.        if not
+00000b40: 2065 6e64 5f63 6f6e 7374 7261 696e 7473   end_constraints
+00000b50: 5b74 6167 735b 2d31 5d5d 3a0a 2020 2020  [tags[-1]]:.    
+00000b60: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00000b70: 616c 7365 0a20 2020 2020 2020 2066 6f72  alse.        for
+00000b80: 2069 2069 6e20 7261 6e67 6528 7365 7175   i in range(sequ
+00000b90: 656e 6365 5f6c 656e 6774 6820 2d20 3129  ence_length - 1)
+00000ba0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00000bb0: 206e 6f74 2074 7261 6e73 6974 696f 6e5f   not transition_
+00000bc0: 636f 6e73 7472 6169 6e74 735b 7461 6773  constraints[tags
+00000bd0: 5b69 5d2c 2074 6167 735b 6920 2b20 315d  [i], tags[i + 1]
+00000be0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00000bf0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00000c00: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00000c10: 0a0a 6465 6620 6368 6563 6b5f 6c6f 675f  ..def check_log_
+00000c20: 706f 7465 6e74 6961 6c73 5f6d 6173 6b65  potentials_maske
+00000c30: 645f 636f 7272 6563 746c 7928 0a20 2020  d_correctly(.   
+00000c40: 206c 6f67 5f70 6f74 656e 7469 616c 733a   log_potentials:
+00000c50: 2074 6f72 6368 2e54 656e 736f 722c 206d   torch.Tensor, m
+00000c60: 6173 6b3a 2074 6f72 6368 2e54 656e 736f  ask: torch.Tenso
+00000c70: 720a 2920 2d3e 2062 6f6f 6c3a 0a20 2020  r.) -> bool:.   
+00000c80: 2073 6571 7565 6e63 655f 6c65 6e67 7468   sequence_length
+00000c90: 203d 206c 6f67 5f70 6f74 656e 7469 616c   = log_potential
+00000ca0: 732e 7369 7a65 2831 290a 2020 2020 6e75  s.size(1).    nu
+00000cb0: 6d5f 7461 6773 203d 206c 6f67 5f70 6f74  m_tags = log_pot
+00000cc0: 656e 7469 616c 732e 7369 7a65 282d 3129  entials.size(-1)
+00000cd0: 0a20 2020 206d 6173 6b5f 7661 6c75 6520  .    mask_value 
+00000ce0: 3d20 287e 746f 7263 682e 6579 6528 6e75  = (~torch.eye(nu
+00000cf0: 6d5f 7461 6773 2c20 6e75 6d5f 7461 6773  m_tags, num_tags
+00000d00: 292e 626f 6f6c 2829 292e 6d75 6c28 4e49  ).bool()).mul(NI
+00000d10: 4e46 290a 2020 2020 6c65 6e67 7468 7320  NF).    lengths 
+00000d20: 3d20 6d61 736b 2e73 756d 2864 696d 3d2d  = mask.sum(dim=-
+00000d30: 3129 0a20 2020 2066 6f72 2062 2c20 7265  1).    for b, re
+00000d40: 616c 5f73 6571 7565 6e63 655f 6c65 6e67  al_sequence_leng
+00000d50: 7468 2069 6e20 656e 756d 6572 6174 6528  th in enumerate(
+00000d60: 6c65 6e67 7468 7329 3a0a 2020 2020 2020  lengths):.      
+00000d70: 2020 666f 7220 4c20 696e 2072 616e 6765    for L in range
+00000d80: 2872 6561 6c5f 7365 7175 656e 6365 5f6c  (real_sequence_l
+00000d90: 656e 6774 682c 2073 6571 7565 6e63 655f  ength, sequence_
+00000da0: 6c65 6e67 7468 293a 0a20 2020 2020 2020  length):.       
+00000db0: 2020 2020 2069 6620 6e6f 7420 746f 7263       if not torc
+00000dc0: 682e 616c 6c63 6c6f 7365 286c 6f67 5f70  h.allclose(log_p
+00000dd0: 6f74 656e 7469 616c 735b 622c 204c 5d2c  otentials[b, L],
+00000de0: 206d 6173 6b5f 7661 6c75 6529 3a0a 2020   mask_value):.  
+00000df0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000e00: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
+00000e10: 6574 7572 6e20 5472 7565 0a0a 0a64 6566  eturn True...def
+00000e20: 2063 6865 636b 5f6c 6f67 5f70 6f74 656e   check_log_poten
+00000e30: 7469 616c 735f 6265 6861 7665 735f 6173  tials_behaves_as
+00000e40: 5f70 726f 6261 6269 6c69 7479 286c 6f67  _probability(log
+00000e50: 5f70 6f74 656e 7469 616c 733a 2074 6f72  _potentials: tor
+00000e60: 6368 2e54 656e 736f 7229 202d 3e20 626f  ch.Tensor) -> bo
+00000e70: 6f6c 3a0a 2020 2020 6261 7463 685f 7369  ol:.    batch_si
+00000e80: 7a65 203d 206c 6f67 5f70 6f74 656e 7469  ze = log_potenti
+00000e90: 616c 732e 7369 7a65 2830 290a 2020 2020  als.size(0).    
+00000ea0: 7365 7175 656e 6365 5f6c 656e 6774 6820  sequence_length 
+00000eb0: 3d20 6c6f 675f 706f 7465 6e74 6961 6c73  = log_potentials
+00000ec0: 2e73 697a 6528 3129 0a20 2020 206e 756d  .size(1).    num
+00000ed0: 5f74 6167 7320 3d20 6c6f 675f 706f 7465  _tags = log_pote
+00000ee0: 6e74 6961 6c73 2e73 697a 6528 3229 0a20  ntials.size(2). 
+00000ef0: 2020 206c 6f67 5f70 726f 6261 6269 6c69     log_probabili
+00000f00: 7479 203d 2074 6f72 6368 2e74 656e 736f  ty = torch.tenso
+00000f10: 7228 5b4e 494e 465d 202a 2062 6174 6368  r([NINF] * batch
+00000f20: 5f73 697a 6529 0a20 2020 2066 6f72 2074  _size).    for t
+00000f30: 6167 5f69 6e64 6963 6573 2069 6e20 6974  ag_indices in it
+00000f40: 6572 6174 655f 706f 7373 6962 6c65 5f74  erate_possible_t
+00000f50: 6167 5f69 6e64 6963 6573 2873 6571 7565  ag_indices(seque
+00000f60: 6e63 655f 6c65 6e67 7468 2c20 6e75 6d5f  nce_length, num_
+00000f70: 7461 6773 293a 0a20 2020 2020 2020 206c  tags):.        l
+00000f80: 6f67 5f70 726f 6261 6269 6c69 7479 203d  og_probability =
+00000f90: 2074 6f72 6368 2e6c 6f67 6164 6465 7870   torch.logaddexp
+00000fa0: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
+00000fb0: 675f 7072 6f62 6162 696c 6974 792c 2046  g_probability, F
+00000fc0: 2e6c 6f67 5f6c 696b 656c 6968 6f6f 6428  .log_likelihood(
+00000fd0: 6c6f 675f 706f 7465 6e74 6961 6c73 2c20  log_potentials, 
+00000fe0: 746f 7263 682e 7465 6e73 6f72 2874 6167  torch.tensor(tag
+00000ff0: 5f69 6e64 6963 6573 2929 0a20 2020 2020  _indices)).     
+00001000: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
+00001010: 746f 7263 682e 616c 6c63 6c6f 7365 286c  torch.allclose(l
+00001020: 6f67 5f70 726f 6261 6269 6c69 7479 2e65  og_probability.e
+00001030: 7870 2829 2c20 746f 7263 682e 6f6e 6573  xp(), torch.ones
+00001040: 5f6c 696b 6528 6c6f 675f 7072 6f62 6162  _like(log_probab
+00001050: 696c 6974 7929 290a 0a0a 6465 6620 6368  ility))...def ch
+00001060: 6563 6b5f 7365 7175 656e 6365 5f73 636f  eck_sequence_sco
+00001070: 7265 5f6d 6173 6b28 0a20 2020 2075 7365  re_mask(.    use
+00001080: 645f 6d61 736b 3a20 746f 7263 682e 5465  d_mask: torch.Te
+00001090: 6e73 6f72 2c20 7461 675f 696e 6469 6365  nsor, tag_indice
+000010a0: 733a 2074 6f72 6368 2e54 656e 736f 722c  s: torch.Tensor,
+000010b0: 206d 6173 6b3a 2074 6f72 6368 2e54 656e   mask: torch.Ten
+000010c0: 736f 720a 2920 2d3e 2062 6f6f 6c3a 0a20  sor.) -> bool:. 
+000010d0: 2020 206e 756d 5f74 6167 7320 3d20 7573     num_tags = us
+000010e0: 6564 5f6d 6173 6b2e 7369 7a65 282d 3129  ed_mask.size(-1)
+000010f0: 0a20 2020 206c 656e 6774 6873 203d 206d  .    lengths = m
+00001100: 6173 6b2e 7375 6d28 6469 6d3d 2d31 290a  ask.sum(dim=-1).
+00001110: 2020 2020 666f 7220 622c 2072 6561 6c5f      for b, real_
+00001120: 7365 7175 656e 6365 5f6c 656e 6774 6820  sequence_length 
+00001130: 696e 2065 6e75 6d65 7261 7465 286c 656e  in enumerate(len
+00001140: 6774 6873 293a 0a20 2020 2020 2020 2023  gths):.        #
+00001150: 206f 6e6c 7920 2869 2c20 6a29 2069 7320   only (i, j) is 
+00001160: 5472 7565 2c20 6f74 6865 7277 6973 6520  True, otherwise 
+00001170: 4661 6c73 650a 2020 2020 2020 2020 7461  False.        ta
+00001180: 6773 203d 2074 6167 5f69 6e64 6963 6573  gs = tag_indices
+00001190: 5b62 2c20 3a72 6561 6c5f 7365 7175 656e  [b, :real_sequen
+000011a0: 6365 5f6c 656e 6774 685d 2e74 6f6c 6973  ce_length].tolis
+000011b0: 7428 290a 2020 2020 2020 2020 7461 6773  t().        tags
+000011c0: 203d 205b 7461 6773 5b30 5d5d 202b 2074   = [tags[0]] + t
+000011d0: 6167 730a 2020 2020 2020 2020 666f 7220  ags.        for 
+000011e0: 706f 732c 2028 692c 206a 2920 696e 2065  pos, (i, j) in e
+000011f0: 6e75 6d65 7261 7465 287a 6970 2874 6167  numerate(zip(tag
+00001200: 735b 3a2d 315d 2c20 7461 6773 5b31 3a5d  s[:-1], tags[1:]
+00001210: 2c20 7374 7269 6374 3d54 7275 6529 293a  , strict=True)):
+00001220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001230: 6e6f 7420 7573 6564 5f6d 6173 6b5b 622c  not used_mask[b,
+00001240: 2070 6f73 2c20 692c 206a 5d3a 0a20 2020   pos, i, j]:.   
+00001250: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00001260: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00001270: 2020 2020 2020 666f 7220 7820 696e 2072        for x in r
+00001280: 616e 6765 286e 756d 5f74 6167 7329 3a0a  ange(num_tags):.
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 666f 7220 7920 696e 2072 616e 6765 286e  for y in range(n
+000012b0: 756d 5f74 6167 7329 3a0a 2020 2020 2020  um_tags):.      
+000012c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000012d0: 2078 203d 3d20 6920 616e 6420 7920 3d3d   x == i and y ==
+000012e0: 206a 3a0a 2020 2020 2020 2020 2020 2020   j:.            
+000012f0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00001300: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+00001310: 2020 2020 2020 2020 2069 6620 7573 6564           if used
+00001320: 5f6d 6173 6b5b 622c 2070 6f73 2c20 782c  _mask[b, pos, x,
+00001330: 2079 5d3a 0a20 2020 2020 2020 2020 2020   y]:.           
+00001340: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00001350: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
+00001360: 2020 2023 2061 6c6c 2076 616c 7565 7320     # all values 
+00001370: 7368 6f75 6c64 2062 6520 4661 6c73 652e  should be False.
+00001380: 0a20 2020 2020 2020 2069 676e 6f72 6573  .        ignores
+00001390: 203d 2075 7365 645f 6d61 736b 5b62 2c20   = used_mask[b, 
+000013a0: 7265 616c 5f73 6571 7565 6e63 655f 6c65  real_sequence_le
+000013b0: 6e67 7468 3a5d 0a20 2020 2020 2020 2069  ngth:].        i
+000013c0: 6620 6e6f 7420 746f 7263 682e 6571 7561  f not torch.equa
+000013d0: 6c28 6967 6e6f 7265 732c 2074 6f72 6368  l(ignores, torch
+000013e0: 2e7a 6572 6f73 5f6c 696b 6528 6967 6e6f  .zeros_like(igno
+000013f0: 7265 732c 2064 7479 7065 3d74 6f72 6368  res, dtype=torch
+00001400: 2e62 6f6f 6c29 293a 0a20 2020 2020 2020  .bool)):.       
+00001410: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00001420: 650a 2020 2020 7265 7475 726e 2054 7275  e.    return Tru
+00001430: 650a 0a0a 6465 6620 6368 6563 6b5f 636f  e...def check_co
+00001440: 6e73 7472 6169 6e65 645f 6c6f 675f 706f  nstrained_log_po
+00001450: 7465 6e74 6961 6c73 280a 2020 2020 6c6f  tentials(.    lo
+00001460: 675f 706f 7465 6e74 6961 6c73 3a20 746f  g_potentials: to
+00001470: 7263 682e 5465 6e73 6f72 2c0a 2020 2020  rch.Tensor,.    
+00001480: 636f 6e73 7472 6169 6e65 645f 6c6f 675f  constrained_log_
+00001490: 706f 7465 6e74 6961 6c73 3a20 746f 7263  potentials: torc
+000014a0: 682e 5465 6e73 6f72 2c0a 2020 2020 7461  h.Tensor,.    ta
+000014b0: 675f 696e 6469 6365 733a 2074 6f72 6368  g_indices: torch
+000014c0: 2e54 656e 736f 722c 0a20 2020 206d 6173  .Tensor,.    mas
+000014d0: 6b3a 2074 6f72 6368 2e54 656e 736f 722c  k: torch.Tensor,
+000014e0: 0a20 2020 2070 6172 7469 616c 5f69 6e64  .    partial_ind
+000014f0: 6578 3a20 696e 742c 0a29 202d 3e20 626f  ex: int,.) -> bo
+00001500: 6f6c 3a0a 2020 2020 6e75 6d5f 7461 6773  ol:.    num_tags
+00001510: 203d 206c 6f67 5f70 6f74 656e 7469 616c   = log_potential
+00001520: 732e 7369 7a65 282d 3129 0a20 2020 206c  s.size(-1).    l
+00001530: 656e 6774 6873 203d 206d 6173 6b2e 7375  engths = mask.su
+00001540: 6d28 6469 6d3d 2d31 290a 2020 2020 666f  m(dim=-1).    fo
+00001550: 7220 622c 2072 6561 6c5f 7365 7175 656e  r b, real_sequen
+00001560: 6365 5f6c 656e 6774 6820 696e 2065 6e75  ce_length in enu
+00001570: 6d65 7261 7465 286c 656e 6774 6873 293a  merate(lengths):
+00001580: 0a20 2020 2020 2020 2074 6167 7320 3d20  .        tags = 
+00001590: 7461 675f 696e 6469 6365 735b 622c 203a  tag_indices[b, :
+000015a0: 7265 616c 5f73 6571 7565 6e63 655f 6c65  real_sequence_le
+000015b0: 6e67 7468 5d2e 746f 6c69 7374 2829 0a20  ngth].tolist(). 
+000015c0: 2020 2020 2020 2074 6167 7320 3d20 5b74         tags = [t
+000015d0: 6167 735b 305d 5d20 2b20 7461 6773 0a20  ags[0]] + tags. 
+000015e0: 2020 2020 2020 2066 6f72 2070 6f73 2c20         for pos, 
+000015f0: 2869 2c20 6a29 2069 6e20 656e 756d 6572  (i, j) in enumer
+00001600: 6174 6528 7a69 7028 7461 6773 5b3a 2d31  ate(zip(tags[:-1
+00001610: 5d2c 2074 6167 735b 313a 5d2c 2073 7472  ], tags[1:], str
+00001620: 6963 743d 5472 7565 2929 3a0a 2020 2020  ict=True)):.    
+00001630: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
+00001640: 7061 7274 6961 6c5f 696e 6465 7820 616e  partial_index an
+00001650: 6420 6a20 3d3d 2070 6172 7469 616c 5f69  d j == partial_i
+00001660: 6e64 6578 3a0a 2020 2020 2020 2020 2020  ndex:.          
+00001670: 2020 2020 2020 7820 3d20 636f 6e73 7472        x = constr
+00001680: 6169 6e65 645f 6c6f 675f 706f 7465 6e74  ained_log_potent
+00001690: 6961 6c73 5b62 2c20 706f 735d 0a20 2020  ials[b, pos].   
+000016a0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+000016b0: 206c 6f67 5f70 6f74 656e 7469 616c 735b   log_potentials[
+000016c0: 622c 2070 6f73 5d0a 2020 2020 2020 2020  b, pos].        
+000016d0: 2020 2020 656c 6966 2069 203d 3d20 7061      elif i == pa
+000016e0: 7274 6961 6c5f 696e 6465 783a 0a20 2020  rtial_index:.   
+000016f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00001700: 206e 2069 6e20 7261 6e67 6528 6e75 6d5f   n in range(num_
+00001710: 7461 6773 293a 0a20 2020 2020 2020 2020  tags):.         
+00001720: 2020 2020 2020 2020 2020 2069 6620 6e20             if n 
+00001730: 3d3d 206a 3a0a 2020 2020 2020 2020 2020  == j:.          
+00001740: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001750: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00001760: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
+00001770: 3d20 636f 6e73 7472 6169 6e65 645f 6c6f  = constrained_lo
+00001780: 675f 706f 7465 6e74 6961 6c73 5b62 2c20  g_potentials[b, 
+00001790: 706f 732c 203a 2c20 6e5d 0a20 2020 2020  pos, :, n].     
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000017b0: 6620 6e6f 7420 746f 7263 682e 6571 7561  f not torch.equa
+000017c0: 6c28 7465 6d70 2c20 746f 7263 682e 6675  l(temp, torch.fu
+000017d0: 6c6c 5f6c 696b 6528 7465 6d70 2c20 4e49  ll_like(temp, NI
+000017e0: 4e46 2929 3a0a 2020 2020 2020 2020 2020  NF)):.          
+000017f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001800: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00001810: 2020 2020 2020 2020 2020 2078 203d 2063             x = c
+00001820: 6f6e 7374 7261 696e 6564 5f6c 6f67 5f70  onstrained_log_p
+00001830: 6f74 656e 7469 616c 735b 622c 2070 6f73  otentials[b, pos
+00001840: 2c20 3a2c 206a 5d0a 2020 2020 2020 2020  , :, j].        
+00001850: 2020 2020 2020 2020 7920 3d20 6c6f 675f          y = log_
+00001860: 706f 7465 6e74 6961 6c73 5b62 2c20 706f  potentials[b, po
+00001870: 732c 203a 2c20 6a5d 0a20 2020 2020 2020  s, :, j].       
+00001880: 2020 2020 2065 6c69 6620 6a20 3d3d 2070       elif j == p
+00001890: 6172 7469 616c 5f69 6e64 6578 3a0a 2020  artial_index:.  
+000018a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000018b0: 7220 6d20 696e 2072 616e 6765 286e 756d  r m in range(num
+000018c0: 5f74 6167 7329 3a0a 2020 2020 2020 2020  _tags):.        
+000018d0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+000018e0: 203d 3d20 693a 0a20 2020 2020 2020 2020   == i:.         
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001900: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00001910: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00001920: 203d 2063 6f6e 7374 7261 696e 6564 5f6c   = constrained_l
+00001930: 6f67 5f70 6f74 656e 7469 616c 735b 622c  og_potentials[b,
+00001940: 2070 6f73 2c20 6d5d 0a20 2020 2020 2020   pos, m].       
+00001950: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001960: 6e6f 7420 746f 7263 682e 6571 7561 6c28  not torch.equal(
+00001970: 7465 6d70 2c20 746f 7263 682e 6675 6c6c  temp, torch.full
+00001980: 5f6c 696b 6528 7465 6d70 2c20 4e49 4e46  _like(temp, NINF
+00001990: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000019a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000019b0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+000019c0: 2020 2020 2020 2020 2078 203d 2063 6f6e           x = con
+000019d0: 7374 7261 696e 6564 5f6c 6f67 5f70 6f74  strained_log_pot
+000019e0: 656e 7469 616c 735b 622c 2070 6f73 2c20  entials[b, pos, 
+000019f0: 695d 0a20 2020 2020 2020 2020 2020 2020  i].             
+00001a00: 2020 2079 203d 206c 6f67 5f70 6f74 656e     y = log_poten
+00001a10: 7469 616c 735b 622c 2070 6f73 2c20 695d  tials[b, pos, i]
+00001a20: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00001a30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00001a40: 2020 2066 6f72 206d 2069 6e20 7261 6e67     for m in rang
+00001a50: 6528 6e75 6d5f 7461 6773 293a 0a20 2020  e(num_tags):.   
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2066 6f72 206e 2069 6e20 7261 6e67 6528   for n in range(
+00001a80: 6e75 6d5f 7461 6773 293a 0a20 2020 2020  num_tags):.     
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2069 6620 6d20 3d3d 2069 2061 6e64     if m == i and
+00001ab0: 206e 203d 3d20 6a3a 0a20 2020 2020 2020   n == j:.       
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2020 2020 2020 6966 2063 6f6e 7374 7261        if constra
+00001b00: 696e 6564 5f6c 6f67 5f70 6f74 656e 7469  ined_log_potenti
+00001b10: 616c 735b 622c 2070 6f73 2c20 6d2c 206e  als[b, pos, m, n
+00001b20: 5d20 213d 204e 494e 463a 0a20 2020 2020  ] != NINF:.     
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00001b50: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00001b60: 2020 2020 7820 3d20 636f 6e73 7472 6169      x = constrai
+00001b70: 6e65 645f 6c6f 675f 706f 7465 6e74 6961  ned_log_potentia
+00001b80: 6c73 5b62 2c20 706f 732c 2069 2c20 6a5d  ls[b, pos, i, j]
 00001b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ba0: 2020 2020 2074 656d 7020 3d20 636f 6e73       temp = cons
-00001bb0: 7472 6169 6e65 645f 6c6f 675f 706f 7465  trained_log_pote
-00001bc0: 6e74 6961 6c73 5b62 2c20 706f 732c 203a  ntials[b, pos, :
-00001bd0: 2c20 6e5d 0a20 2020 2020 2020 2020 2020  , n].           
-00001be0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00001bf0: 746f 7263 682e 6571 7561 6c28 7465 6d70  torch.equal(temp
-00001c00: 2c20 746f 7263 682e 6675 6c6c 5f6c 696b  , torch.full_lik
-00001c10: 6528 7465 6d70 2c20 4e49 4e46 2929 3a0a  e(temp, NINF)):.
-00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c30: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00001c40: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00001c50: 2020 2020 2078 203d 2063 6f6e 7374 7261       x = constra
-00001c60: 696e 6564 5f6c 6f67 5f70 6f74 656e 7469  ined_log_potenti
-00001c70: 616c 735b 622c 2070 6f73 2c20 3a2c 206a  als[b, pos, :, j
-00001c80: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00001c90: 2020 7920 3d20 6c6f 675f 706f 7465 6e74    y = log_potent
-00001ca0: 6961 6c73 5b62 2c20 706f 732c 203a 2c20  ials[b, pos, :, 
-00001cb0: 6a5d 0a20 2020 2020 2020 2020 2020 2065  j].            e
-00001cc0: 6c69 6620 6a20 3d3d 2070 6172 7469 616c  lif j == partial
-00001cd0: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
-00001ce0: 2020 2020 2020 2020 666f 7220 6d20 696e          for m in
-00001cf0: 2072 616e 6765 286e 756d 5f74 6167 7329   range(num_tags)
-00001d00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001d10: 2020 2020 2020 6966 206d 203d 3d20 693a        if m == i:
-00001d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00001d40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00001d50: 2020 2020 2020 7465 6d70 203d 2063 6f6e        temp = con
-00001d60: 7374 7261 696e 6564 5f6c 6f67 5f70 6f74  strained_log_pot
-00001d70: 656e 7469 616c 735b 622c 2070 6f73 2c20  entials[b, pos, 
-00001d80: 6d5d 0a20 2020 2020 2020 2020 2020 2020  m].             
-00001d90: 2020 2020 2020 2069 6620 6e6f 7420 746f         if not to
-00001da0: 7263 682e 6571 7561 6c28 7465 6d70 2c20  rch.equal(temp, 
-00001db0: 746f 7263 682e 6675 6c6c 5f6c 696b 6528  torch.full_like(
-00001dc0: 7465 6d70 2c20 4e49 4e46 2929 3a0a 2020  temp, NINF)):.  
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001de0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00001df0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00001e00: 2020 2078 203d 2063 6f6e 7374 7261 696e     x = constrain
-00001e10: 6564 5f6c 6f67 5f70 6f74 656e 7469 616c  ed_log_potential
-00001e20: 735b 622c 2070 6f73 2c20 695d 0a20 2020  s[b, pos, i].   
-00001e30: 2020 2020 2020 2020 2020 2020 2079 203d               y =
-00001e40: 206c 6f67 5f70 6f74 656e 7469 616c 735b   log_potentials[
-00001e50: 622c 2070 6f73 2c20 695d 0a20 2020 2020  b, pos, i].     
-00001e60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00001e70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00001e80: 206d 2069 6e20 7261 6e67 6528 6e75 6d5f   m in range(num_
-00001e90: 7461 6773 293a 0a20 2020 2020 2020 2020  tags):.         
-00001ea0: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00001eb0: 2069 6e20 7261 6e67 6528 6e75 6d5f 7461   in range(num_ta
-00001ec0: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
-00001ed0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001ee0: 6d20 3d3d 2069 2061 6e64 206e 203d 3d20  m == i and n == 
-00001ef0: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001f10: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f30: 6966 2063 6f6e 7374 7261 696e 6564 5f6c  if constrained_l
-00001f40: 6f67 5f70 6f74 656e 7469 616c 735b 622c  og_potentials[b,
-00001f50: 2070 6f73 2c20 6d2c 206e 5d20 213d 204e   pos, m, n] != N
-00001f60: 494e 463a 0a20 2020 2020 2020 2020 2020  INF:.           
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00001f90: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-00001fa0: 3d20 636f 6e73 7472 6169 6e65 645f 6c6f  = constrained_lo
-00001fb0: 675f 706f 7465 6e74 6961 6c73 5b62 2c20  g_potentials[b, 
-00001fc0: 706f 732c 2069 2c20 6a5d 0a20 2020 2020  pos, i, j].     
-00001fd0: 2020 2020 2020 2020 2020 2079 203d 206c             y = l
-00001fe0: 6f67 5f70 6f74 656e 7469 616c 735b 622c  og_potentials[b,
-00001ff0: 2070 6f73 2c20 692c 206a 5d0a 0a20 2020   pos, i, j]..   
-00002000: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00002010: 746f 7263 682e 6571 7561 6c28 782c 2079  torch.equal(x, y
-00002020: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00002030: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00002040: 0a20 2020 2020 2020 2078 203d 2063 6f6e  .        x = con
-00002050: 7374 7261 696e 6564 5f6c 6f67 5f70 6f74  strained_log_pot
-00002060: 656e 7469 616c 735b 622c 2072 6561 6c5f  entials[b, real_
-00002070: 7365 7175 656e 6365 5f6c 656e 6774 683a  sequence_length:
-00002080: 5d0a 2020 2020 2020 2020 7920 3d20 6c6f  ].        y = lo
-00002090: 675f 706f 7465 6e74 6961 6c73 5b62 2c20  g_potentials[b, 
-000020a0: 7265 616c 5f73 6571 7565 6e63 655f 6c65  real_sequence_le
-000020b0: 6e67 7468 3a5d 0a20 2020 2020 2020 2069  ngth:].        i
-000020c0: 6620 6e6f 7420 746f 7263 682e 6571 7561  f not torch.equa
-000020d0: 6c28 782c 2079 293a 0a20 2020 2020 2020  l(x, y):.       
-000020e0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000020f0: 650a 2020 2020 7265 7475 726e 2054 7275  e.    return Tru
-00002100: 650a                                     e.
+00001ba0: 2079 203d 206c 6f67 5f70 6f74 656e 7469   y = log_potenti
+00001bb0: 616c 735b 622c 2070 6f73 2c20 692c 206a  als[b, pos, i, j
+00001bc0: 5d0a 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+00001bd0: 6620 6e6f 7420 746f 7263 682e 6571 7561  f not torch.equa
+00001be0: 6c28 782c 2079 293a 0a20 2020 2020 2020  l(x, y):.       
+00001bf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001c00: 4661 6c73 650a 0a20 2020 2020 2020 2078  False..        x
+00001c10: 203d 2063 6f6e 7374 7261 696e 6564 5f6c   = constrained_l
+00001c20: 6f67 5f70 6f74 656e 7469 616c 735b 622c  og_potentials[b,
+00001c30: 2072 6561 6c5f 7365 7175 656e 6365 5f6c   real_sequence_l
+00001c40: 656e 6774 683a 5d0a 2020 2020 2020 2020  ength:].        
+00001c50: 7920 3d20 6c6f 675f 706f 7465 6e74 6961  y = log_potentia
+00001c60: 6c73 5b62 2c20 7265 616c 5f73 6571 7565  ls[b, real_seque
+00001c70: 6e63 655f 6c65 6e67 7468 3a5d 0a20 2020  nce_length:].   
+00001c80: 2020 2020 2069 6620 6e6f 7420 746f 7263       if not torc
+00001c90: 682e 6571 7561 6c28 782c 2079 293a 0a20  h.equal(x, y):. 
+00001ca0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001cb0: 6e20 4661 6c73 650a 2020 2020 7265 7475  n False.    retu
+00001cc0: 726e 2054 7275 650a                      rn True.
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/4562057324d7e8a` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,220 +1,207 @@
-00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00000010: 1800 0000 0000 0000 5a69 7057 6974 686f  ........ZipWitho
-00000020: 7574 4578 706c 6963 6974 5374 7269 6374  utExplicitStrict
-00000030: 2f00 0000 0000 0000 607a 6970 2829 6020  /.......`zip()` 
-00000040: 7769 7468 6f75 7420 616e 2065 7870 6c69  without an expli
-00000050: 6369 7420 6073 7472 6963 743d 6020 7061  cit `strict=` pa
-00000060: 7261 6d65 7465 7200 0c09 0000 2b09 0000  rameter.....+...
-00000070: 0000 0000 0000 0000 000c 0900 0001 0000  ................
-00000080: 0000 0000 004c 0000 0000 0000 002f 5573  .....L......./Us
-00000090: 6572 732f 7961 7375 6675 6d69 2f57 6f72  ers/yasufumi/Wor
-000000a0: 6b73 7061 6365 2f70 7974 6f72 6368 2d70  kspace/pytorch-p
-000000b0: 6172 7469 616c 2d74 6167 6765 722f 7372  artial-tagger/sr
-000000c0: 632f 7061 7274 6961 6c5f 7461 6767 6572  c/partial_tagger
-000000d0: 2f75 7469 6c73 2e70 79dd 0c00 0000 0000  /utils.py.......
-000000e0: 0066 726f 6d20 7472 616e 7366 6f72 6d65  .from transforme
-000000f0: 7273 2069 6d70 6f72 7420 4175 746f 4d6f  rs import AutoMo
-00000100: 6465 6c2c 2041 7574 6f54 6f6b 656e 697a  del, AutoTokeniz
-00000110: 6572 0a0a 6672 6f6d 202e 6461 7461 2069  er..from .data i
-00000120: 6d70 6f72 7420 4c61 6265 6c53 6574 2c20  mport LabelSet, 
-00000130: 5370 616e 2c20 5461 670a 6672 6f6d 202e  Span, Tag.from .
-00000140: 6461 7461 2e62 6174 6368 2069 6d70 6f72  data.batch impor
-00000150: 7420 4368 6172 4261 7365 6454 6167 7343  t CharBasedTagsC
-00000160: 6f6c 6c65 6374 696f 6e2c 2043 6f6c 6c61  ollection, Colla
-00000170: 746f 722c 2054 7261 6e73 666f 726d 6572  tor, Transformer
-00000180: 4261 7463 6846 6163 746f 7279 0a66 726f  BatchFactory.fro
-00000190: 6d20 2e64 6563 6f64 6572 732e 7669 7465  m .decoders.vite
-000001a0: 7262 6920 696d 706f 7274 2043 6f6e 7472  rbi import Contr
-000001b0: 6169 6e65 722c 2056 6974 6572 6269 4465  ainer, ViterbiDe
-000001c0: 636f 6465 720a 6672 6f6d 202e 656d 6265  coder.from .embe
-000001d0: 6464 6572 7320 696d 706f 7274 2054 7261  dders import Tra
-000001e0: 6e73 666f 726d 6572 456d 6265 6464 6572  nsformerEmbedder
-000001f0: 0a66 726f 6d20 2e65 6e63 6f64 6572 732e  .from .encoders.
-00000200: 6c69 6e65 6172 2069 6d70 6f72 7420 4c69  linear import Li
-00000210: 6e65 6172 456e 636f 6465 720a 6672 6f6d  nearEncoder.from
-00000220: 202e 7461 6767 6572 2069 6d70 6f72 7420   .tagger import 
-00000230: 5365 7175 656e 6365 5461 6767 6572 0a0a  SequenceTagger..
-00000240: 0a64 6566 2063 7265 6174 655f 7461 6728  .def create_tag(
-00000250: 7374 6172 743a 2069 6e74 2c20 6c65 6e67  start: int, leng
-00000260: 7468 3a20 696e 742c 206c 6162 656c 3a20  th: int, label: 
-00000270: 7374 7229 202d 3e20 5461 673a 0a20 2020  str) -> Tag:.   
-00000280: 2022 2222 4372 6561 7465 7320 6120 7461   """Creates a ta
-00000290: 672e 0a0a 2020 2020 4172 6773 3a0a 2020  g...    Args:.  
-000002a0: 2020 2020 2020 7374 6172 743a 2041 6e20        start: An 
-000002b0: 696e 7465 6765 7220 7265 7072 6573 656e  integer represen
-000002c0: 7469 6e67 2061 2073 7461 7274 2069 6e64  ting a start ind
-000002d0: 6578 206f 6620 6120 7461 672e 0a20 2020  ex of a tag..   
-000002e0: 2020 2020 206c 656e 6774 683a 2041 6e20       length: An 
-000002f0: 696e 7465 6765 7220 7265 7072 6573 656e  integer represen
-00000300: 7469 6e67 206c 656e 6774 6820 6f66 2061  ting length of a
-00000310: 2074 6167 2e0a 2020 2020 2020 2020 6c61   tag..        la
-00000320: 6265 6c3a 2041 2073 7472 696e 6720 7265  bel: A string re
-00000330: 7072 6573 656e 7469 6e67 2061 206c 6162  presenting a lab
-00000340: 656c 206f 6620 6120 7461 672e 0a0a 2020  el of a tag...  
-00000350: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00000360: 2020 2041 2054 6167 2e0a 2020 2020 2222     A Tag..    ""
-00000370: 220a 2020 2020 7265 7475 726e 2054 6167  ".    return Tag
-00000380: 2853 7061 6e28 7374 6172 742c 206c 656e  (Span(start, len
-00000390: 6774 6829 2c20 6c61 6265 6c29 0a0a 0a64  gth), label)...d
-000003a0: 6566 2063 7265 6174 655f 7461 6767 6572  ef create_tagger
-000003b0: 280a 2020 2020 6d6f 6465 6c5f 6e61 6d65  (.    model_name
-000003c0: 3a20 7374 722c 206c 6162 656c 5f73 6574  : str, label_set
-000003d0: 3a20 4c61 6265 6c53 6574 2c20 7061 6464  : LabelSet, padd
-000003e0: 696e 675f 696e 6465 783a 2069 6e74 0a29  ing_index: int.)
-000003f0: 202d 3e20 5365 7175 656e 6365 5461 6767   -> SequenceTagg
-00000400: 6572 3a0a 2020 2020 2222 2243 7265 6174  er:.    """Creat
-00000410: 6573 2061 2054 7261 6e73 666f 726d 6572  es a Transformer
-00000420: 2074 6167 6765 722e 0a0a 2020 2020 4172   tagger...    Ar
-00000430: 6773 3a0a 2020 2020 2020 2020 6d6f 6465  gs:.        mode
-00000440: 6c5f 6e61 6d65 3a20 4120 7374 7269 6e67  l_name: A string
-00000450: 2072 6570 7265 7365 6e74 696e 6720 6120   representing a 
-00000460: 7472 616e 7366 6f72 6d65 7227 7320 6d6f  transformer's mo
-00000470: 6465 6c20 6e61 6d65 2e0a 2020 2020 2020  del name..      
-00000480: 2020 6c61 6265 6c5f 7365 743a 2041 204c    label_set: A L
-00000490: 6162 656c 5365 7420 6f62 6a65 6374 2e0a  abelSet object..
-000004a0: 2020 2020 2020 2020 7061 6464 696e 675f          padding_
-000004b0: 696e 6465 783a 2041 6e20 696e 7465 6765  index: An intege
-000004c0: 7220 7265 7072 6573 656e 7469 6e67 2061  r representing a
-000004d0: 6e20 696e 6465 7820 746f 2066 696c 6c20  n index to fill 
-000004e0: 7769 7468 2e0a 0a20 2020 2052 6574 7572  with...    Retur
-000004f0: 6e73 3a0a 2020 2020 2020 2020 4120 7461  ns:.        A ta
-00000500: 6767 6572 2e0a 2020 2020 2222 220a 2020  gger..    """.  
-00000510: 2020 6d6f 6465 6c20 3d20 4175 746f 4d6f    model = AutoMo
-00000520: 6465 6c2e 6672 6f6d 5f70 7265 7472 6169  del.from_pretrai
-00000530: 6e65 6428 6d6f 6465 6c5f 6e61 6d65 290a  ned(model_name).
-00000540: 2020 2020 7461 6767 6572 203d 2053 6571      tagger = Seq
-00000550: 7565 6e63 6554 6167 6765 7228 0a20 2020  uenceTagger(.   
-00000560: 2020 2020 2054 7261 6e73 666f 726d 6572       Transformer
-00000570: 456d 6265 6464 6572 286d 6f64 656c 292c  Embedder(model),
-00000580: 0a20 2020 2020 2020 204c 696e 6561 7245  .        LinearE
-00000590: 6e63 6f64 6572 286d 6f64 656c 2e63 6f6e  ncoder(model.con
-000005a0: 6669 672e 6869 6464 656e 5f73 697a 652c  fig.hidden_size,
-000005b0: 206c 6162 656c 5f73 6574 2e67 6574 5f74   label_set.get_t
-000005c0: 6167 5f73 697a 6528 2929 2c0a 2020 2020  ag_size()),.    
-000005d0: 2020 2020 5669 7465 7262 6944 6563 6f64      ViterbiDecod
-000005e0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-000005f0: 7061 6464 696e 675f 696e 6465 782c 0a20  padding_index,. 
-00000600: 2020 2020 2020 2020 2020 2043 6f6e 7472             Contr
-00000610: 6169 6e65 7228 0a20 2020 2020 2020 2020  ainer(.         
-00000620: 2020 2020 2020 206c 6162 656c 5f73 6574         label_set
-00000630: 2e67 6574 5f73 7461 7274 5f73 7461 7465  .get_start_state
-00000640: 7328 292c 0a20 2020 2020 2020 2020 2020  s(),.           
-00000650: 2020 2020 206c 6162 656c 5f73 6574 2e67       label_set.g
-00000660: 6574 5f65 6e64 5f73 7461 7465 7328 292c  et_end_states(),
-00000670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000680: 206c 6162 656c 5f73 6574 2e67 6574 5f74   label_set.get_t
-00000690: 7261 6e73 6974 696f 6e73 2829 2c0a 2020  ransitions(),.  
-000006a0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000006b0: 2020 2020 2029 2c0a 2020 2020 290a 2020       ),.    ).  
-000006c0: 2020 7265 7475 726e 2074 6167 6765 720a    return tagger.
-000006d0: 0a0a 6465 6620 6372 6561 7465 5f63 6f6c  ..def create_col
-000006e0: 6c61 746f 7228 0a20 2020 206d 6f64 656c  lator(.    model
-000006f0: 5f6e 616d 653a 2073 7472 2c20 6c61 6265  _name: str, labe
-00000700: 6c5f 7365 743a 204c 6162 656c 5365 742c  l_set: LabelSet,
-00000710: 2074 6f6b 656e 697a 6572 5f61 7267 733a   tokenizer_args:
-00000720: 2064 6963 7420 7c20 4e6f 6e65 203d 204e   dict | None = N
-00000730: 6f6e 650a 2920 2d3e 2043 6f6c 6c61 746f  one.) -> Collato
-00000740: 723a 0a20 2020 2022 2222 4372 6561 7465  r:.    """Create
-00000750: 7320 6120 636f 6c6c 6174 6f72 2e0a 0a20  s a collator... 
-00000760: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00000770: 206d 6f64 656c 5f6e 616d 653a 2041 2073   model_name: A s
-00000780: 7472 696e 6720 7265 7072 6573 656e 7469  tring representi
-00000790: 6e67 2061 2074 7261 6e73 666f 726d 6572  ng a transformer
-000007a0: 2773 206d 6f64 656c 206e 616d 652e 0a20  's model name.. 
-000007b0: 2020 2020 2020 206c 6162 656c 5f73 6574         label_set
-000007c0: 3a20 4120 4c61 6265 6c53 6574 206f 626a  : A LabelSet obj
-000007d0: 6563 742e 0a20 2020 2020 2020 2074 6f6b  ect..        tok
-000007e0: 656e 697a 6572 5f61 7267 733a 2041 2064  enizer_args: A d
-000007f0: 6963 7469 6f6e 6172 7920 7265 7072 6573  ictionary repres
-00000800: 656e 7469 6e67 2061 7267 756d 656e 7473  enting arguments
-00000810: 2070 6173 7365 6420 746f 2074 6f6b 656e   passed to token
-00000820: 697a 6572 2e0a 2020 2020 2222 220a 2020  izer..    """.  
-00000830: 2020 6261 7463 685f 6661 6374 6f72 7920    batch_factory 
-00000840: 3d20 5472 616e 7366 6f72 6d65 7242 6174  = TransformerBat
-00000850: 6368 4661 6374 6f72 7928 0a20 2020 2020  chFactory(.     
-00000860: 2020 2041 7574 6f54 6f6b 656e 697a 6572     AutoTokenizer
-00000870: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-00000880: 286d 6f64 656c 5f6e 616d 6529 2c20 6c61  (model_name), la
-00000890: 6265 6c5f 7365 742c 2074 6f6b 656e 697a  bel_set, tokeniz
-000008a0: 6572 5f61 7267 730a 2020 2020 290a 2020  er_args.    ).  
-000008b0: 2020 7265 7475 726e 2043 6f6c 6c61 746f    return Collato
-000008c0: 7228 6261 7463 685f 6661 6374 6f72 7929  r(batch_factory)
-000008d0: 0a0a 0a63 6c61 7373 204d 6574 7269 633a  ...class Metric:
-000008e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000008f0: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00000900: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-00000910: 7470 203d 2030 0a20 2020 2020 2020 2073  tp = 0.        s
-00000920: 656c 662e 5f5f 6670 203d 2030 0a20 2020  elf.__fp = 0.   
-00000930: 2020 2020 2073 656c 662e 5f5f 666e 203d       self.__fn =
-00000940: 2030 0a0a 2020 2020 6465 6620 5f5f 6361   0..    def __ca
-00000950: 6c6c 5f5f 280a 2020 2020 2020 2020 7365  ll__(.        se
-00000960: 6c66 2c0a 2020 2020 2020 2020 7072 6564  lf,.        pred
-00000970: 6963 7469 6f6e 733a 2043 6861 7242 6173  ictions: CharBas
-00000980: 6564 5461 6773 436f 6c6c 6563 7469 6f6e  edTagsCollection
-00000990: 2c0a 2020 2020 2020 2020 6772 6f75 6e64  ,.        ground
-000009a0: 5f74 7275 7468 733a 2043 6861 7242 6173  _truths: CharBas
-000009b0: 6564 5461 6773 436f 6c6c 6563 7469 6f6e  edTagsCollection
-000009c0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-000009d0: 0a20 2020 2020 2020 2066 6f72 2074 6167  .        for tag
-000009e0: 7331 2c20 7461 6773 3220 696e 207a 6970  s1, tags2 in zip
-000009f0: 2870 7265 6469 6374 696f 6e73 2c20 6772  (predictions, gr
-00000a00: 6f75 6e64 5f74 7275 7468 7329 3a0a 2020  ound_truths):.  
-00000a10: 2020 2020 2020 2020 2020 7461 675f 7365            tag_se
-00000a20: 7431 203d 207b 2874 6167 312e 7374 6172  t1 = {(tag1.star
-00000a30: 742c 2074 6167 312e 6c65 6e67 7468 2c20  t, tag1.length, 
-00000a40: 7461 6731 2e6c 6162 656c 2920 666f 7220  tag1.label) for 
-00000a50: 7461 6731 2069 6e20 7461 6773 317d 0a20  tag1 in tags1}. 
-00000a60: 2020 2020 2020 2020 2020 2074 6167 5f73             tag_s
-00000a70: 6574 3220 3d20 7b28 7461 6732 2e73 7461  et2 = {(tag2.sta
-00000a80: 7274 2c20 7461 6732 2e6c 656e 6774 682c  rt, tag2.length,
-00000a90: 2074 6167 322e 6c61 6265 6c29 2066 6f72   tag2.label) for
-00000aa0: 2074 6167 3220 696e 2074 6167 7332 7d0a   tag2 in tags2}.
-00000ab0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000ac0: 662e 5f5f 7470 202b 3d20 6c65 6e28 7461  f.__tp += len(ta
-00000ad0: 675f 7365 7431 2026 2074 6167 5f73 6574  g_set1 & tag_set
-00000ae0: 3229 0a20 2020 2020 2020 2020 2020 2073  2).            s
-00000af0: 656c 662e 5f5f 6670 202b 3d20 6c65 6e28  elf.__fp += len(
-00000b00: 7461 675f 7365 7431 202d 2074 6167 5f73  tag_set1 - tag_s
-00000b10: 6574 3229 0a20 2020 2020 2020 2020 2020  et2).           
-00000b20: 2073 656c 662e 5f5f 666e 202b 3d20 6c65   self.__fn += le
-00000b30: 6e28 7461 675f 7365 7432 202d 2074 6167  n(tag_set2 - tag
-00000b40: 5f73 6574 3129 0a0a 2020 2020 6465 6620  _set1)..    def 
-00000b50: 6765 745f 7363 6f72 6573 2873 656c 6629  get_scores(self)
-00000b60: 202d 3e20 6469 6374 5b73 7472 2c20 666c   -> dict[str, fl
-00000b70: 6f61 745d 3a0a 2020 2020 2020 2020 6966  oat]:.        if
-00000b80: 2073 656c 662e 5f5f 7470 202b 2073 656c   self.__tp + sel
-00000b90: 662e 5f5f 6670 2021 3d20 303a 0a20 2020  f.__fp != 0:.   
-00000ba0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
-00000bb0: 6f6e 203d 2073 656c 662e 5f5f 7470 202f  on = self.__tp /
-00000bc0: 2028 7365 6c66 2e5f 5f74 7020 2b20 7365   (self.__tp + se
-00000bd0: 6c66 2e5f 5f66 7029 0a20 2020 2020 2020  lf.__fp).       
-00000be0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00000bf0: 2020 2070 7265 6369 7369 6f6e 203d 2030     precision = 0
-00000c00: 2e30 0a0a 2020 2020 2020 2020 6966 2073  .0..        if s
-00000c10: 656c 662e 5f5f 7470 202b 2073 656c 662e  elf.__tp + self.
-00000c20: 5f5f 666e 2021 3d20 303a 0a20 2020 2020  __fn != 0:.     
-00000c30: 2020 2020 2020 2072 6563 616c 6c20 3d20         recall = 
-00000c40: 7365 6c66 2e5f 5f74 7020 2f20 2873 656c  self.__tp / (sel
-00000c50: 662e 5f5f 7470 202b 2073 656c 662e 5f5f  f.__tp + self.__
-00000c60: 666e 290a 2020 2020 2020 2020 656c 7365  fn).        else
-00000c70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00000c80: 6361 6c6c 203d 2030 2e30 0a0a 2020 2020  call = 0.0..    
-00000c90: 2020 2020 6966 2070 7265 6369 7369 6f6e      if precision
-00000ca0: 202b 2072 6563 616c 6c20 3d3d 2030 2e30   + recall == 0.0
-00000cb0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00000cc0: 7475 726e 207b 2266 315f 7363 6f72 6522  turn {"f1_score"
-00000cd0: 3a20 302e 302c 2022 7072 6563 6973 696f  : 0.0, "precisio
-00000ce0: 6e22 3a20 302e 302c 2022 7265 6361 6c6c  n": 0.0, "recall
-00000cf0: 223a 2030 2e30 7d0a 2020 2020 2020 2020  ": 0.0}.        
-00000d00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00000d10: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-00000d20: 2020 2020 2020 2020 2020 2022 6631 5f73             "f1_s
-00000d30: 636f 7265 223a 2032 202a 2070 7265 6369  core": 2 * preci
-00000d40: 7369 6f6e 202a 2072 6563 616c 6c20 2f20  sion * recall / 
-00000d50: 2870 7265 6369 7369 6f6e 202b 2072 6563  (precision + rec
-00000d60: 616c 6c29 2c0a 2020 2020 2020 2020 2020  all),.          
-00000d70: 2020 2020 2020 2270 7265 6369 7369 6f6e        "precision
-00000d80: 223a 2070 7265 6369 7369 6f6e 2c0a 2020  ": precision,.  
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00000da0: 6563 616c 6c22 3a20 7265 6361 6c6c 2c0a  ecall": recall,.
-00000db0: 2020 2020 2020 2020 2020 2020 7d0a                   }.
+00000000: 6672 6f6d 2074 7261 6e73 666f 726d 6572  from transformer
+00000010: 7320 696d 706f 7274 2041 7574 6f4d 6f64  s import AutoMod
+00000020: 656c 2c20 4175 746f 546f 6b65 6e69 7a65  el, AutoTokenize
+00000030: 720a 0a66 726f 6d20 2e64 6174 6120 696d  r..from .data im
+00000040: 706f 7274 204c 6162 656c 5365 742c 2053  port LabelSet, S
+00000050: 7061 6e2c 2054 6167 0a66 726f 6d20 2e64  pan, Tag.from .d
+00000060: 6174 612e 6261 7463 6820 696d 706f 7274  ata.batch import
+00000070: 2043 6861 7242 6173 6564 5461 6773 436f   CharBasedTagsCo
+00000080: 6c6c 6563 7469 6f6e 2c20 436f 6c6c 6174  llection, Collat
+00000090: 6f72 2c20 5472 616e 7366 6f72 6d65 7242  or, TransformerB
+000000a0: 6174 6368 4661 6374 6f72 790a 6672 6f6d  atchFactory.from
+000000b0: 202e 6465 636f 6465 7273 2e76 6974 6572   .decoders.viter
+000000c0: 6269 2069 6d70 6f72 7420 436f 6e74 7261  bi import Contra
+000000d0: 696e 6572 2c20 5669 7465 7262 6944 6563  iner, ViterbiDec
+000000e0: 6f64 6572 0a66 726f 6d20 2e65 6d62 6564  oder.from .embed
+000000f0: 6465 7273 2069 6d70 6f72 7420 5472 616e  ders import Tran
+00000100: 7366 6f72 6d65 7245 6d62 6564 6465 720a  sformerEmbedder.
+00000110: 6672 6f6d 202e 656e 636f 6465 7273 2e6c  from .encoders.l
+00000120: 696e 6561 7220 696d 706f 7274 204c 696e  inear import Lin
+00000130: 6561 7245 6e63 6f64 6572 0a66 726f 6d20  earEncoder.from 
+00000140: 2e74 6167 6765 7220 696d 706f 7274 2053  .tagger import S
+00000150: 6571 7565 6e63 6554 6167 6765 720a 0a0a  equenceTagger...
+00000160: 6465 6620 6372 6561 7465 5f74 6167 2873  def create_tag(s
+00000170: 7461 7274 3a20 696e 742c 206c 656e 6774  tart: int, lengt
+00000180: 683a 2069 6e74 2c20 6c61 6265 6c3a 2073  h: int, label: s
+00000190: 7472 2920 2d3e 2054 6167 3a0a 2020 2020  tr) -> Tag:.    
+000001a0: 2222 2243 7265 6174 6573 2061 2074 6167  """Creates a tag
+000001b0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000001c0: 2020 2020 2073 7461 7274 3a20 416e 2069       start: An i
+000001d0: 6e74 6567 6572 2072 6570 7265 7365 6e74  nteger represent
+000001e0: 696e 6720 6120 7374 6172 7420 696e 6465  ing a start inde
+000001f0: 7820 6f66 2061 2074 6167 2e0a 2020 2020  x of a tag..    
+00000200: 2020 2020 6c65 6e67 7468 3a20 416e 2069      length: An i
+00000210: 6e74 6567 6572 2072 6570 7265 7365 6e74  nteger represent
+00000220: 696e 6720 6c65 6e67 7468 206f 6620 6120  ing length of a 
+00000230: 7461 672e 0a20 2020 2020 2020 206c 6162  tag..        lab
+00000240: 656c 3a20 4120 7374 7269 6e67 2072 6570  el: A string rep
+00000250: 7265 7365 6e74 696e 6720 6120 6c61 6265  resenting a labe
+00000260: 6c20 6f66 2061 2074 6167 2e0a 0a20 2020  l of a tag...   
+00000270: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00000280: 2020 4120 5461 672e 0a20 2020 2022 2222    A Tag..    """
+00000290: 0a20 2020 2072 6574 7572 6e20 5461 6728  .    return Tag(
+000002a0: 5370 616e 2873 7461 7274 2c20 6c65 6e67  Span(start, leng
+000002b0: 7468 292c 206c 6162 656c 290a 0a0a 6465  th), label)...de
+000002c0: 6620 6372 6561 7465 5f74 6167 6765 7228  f create_tagger(
+000002d0: 0a20 2020 206d 6f64 656c 5f6e 616d 653a  .    model_name:
+000002e0: 2073 7472 2c20 6c61 6265 6c5f 7365 743a   str, label_set:
+000002f0: 204c 6162 656c 5365 742c 2070 6164 6469   LabelSet, paddi
+00000300: 6e67 5f69 6e64 6578 3a20 696e 740a 2920  ng_index: int.) 
+00000310: 2d3e 2053 6571 7565 6e63 6554 6167 6765  -> SequenceTagge
+00000320: 723a 0a20 2020 2022 2222 4372 6561 7465  r:.    """Create
+00000330: 7320 6120 5472 616e 7366 6f72 6d65 7220  s a Transformer 
+00000340: 7461 6767 6572 2e0a 0a20 2020 2041 7267  tagger...    Arg
+00000350: 733a 0a20 2020 2020 2020 206d 6f64 656c  s:.        model
+00000360: 5f6e 616d 653a 2041 2073 7472 696e 6720  _name: A string 
+00000370: 7265 7072 6573 656e 7469 6e67 2061 2074  representing a t
+00000380: 7261 6e73 666f 726d 6572 2773 206d 6f64  ransformer's mod
+00000390: 656c 206e 616d 652e 0a20 2020 2020 2020  el name..       
+000003a0: 206c 6162 656c 5f73 6574 3a20 4120 4c61   label_set: A La
+000003b0: 6265 6c53 6574 206f 626a 6563 742e 0a20  belSet object.. 
+000003c0: 2020 2020 2020 2070 6164 6469 6e67 5f69         padding_i
+000003d0: 6e64 6578 3a20 416e 2069 6e74 6567 6572  ndex: An integer
+000003e0: 2072 6570 7265 7365 6e74 696e 6720 616e   representing an
+000003f0: 2069 6e64 6578 2074 6f20 6669 6c6c 2077   index to fill w
+00000400: 6974 682e 0a0a 2020 2020 5265 7475 726e  ith...    Return
+00000410: 733a 0a20 2020 2020 2020 2041 2074 6167  s:.        A tag
+00000420: 6765 722e 0a20 2020 2022 2222 0a20 2020  ger..    """.   
+00000430: 206d 6f64 656c 203d 2041 7574 6f4d 6f64   model = AutoMod
+00000440: 656c 2e66 726f 6d5f 7072 6574 7261 696e  el.from_pretrain
+00000450: 6564 286d 6f64 656c 5f6e 616d 6529 0a20  ed(model_name). 
+00000460: 2020 2074 6167 6765 7220 3d20 5365 7175     tagger = Sequ
+00000470: 656e 6365 5461 6767 6572 280a 2020 2020  enceTagger(.    
+00000480: 2020 2020 5472 616e 7366 6f72 6d65 7245      TransformerE
+00000490: 6d62 6564 6465 7228 6d6f 6465 6c29 2c0a  mbedder(model),.
+000004a0: 2020 2020 2020 2020 4c69 6e65 6172 456e          LinearEn
+000004b0: 636f 6465 7228 6d6f 6465 6c2e 636f 6e66  coder(model.conf
+000004c0: 6967 2e68 6964 6465 6e5f 7369 7a65 2c20  ig.hidden_size, 
+000004d0: 6c61 6265 6c5f 7365 742e 6765 745f 7461  label_set.get_ta
+000004e0: 675f 7369 7a65 2829 292c 0a20 2020 2020  g_size()),.     
+000004f0: 2020 2056 6974 6572 6269 4465 636f 6465     ViterbiDecode
+00000500: 7228 0a20 2020 2020 2020 2020 2020 2070  r(.            p
+00000510: 6164 6469 6e67 5f69 6e64 6578 2c0a 2020  adding_index,.  
+00000520: 2020 2020 2020 2020 2020 436f 6e74 7261            Contra
+00000530: 696e 6572 280a 2020 2020 2020 2020 2020  iner(.          
+00000540: 2020 2020 2020 6c61 6265 6c5f 7365 742e        label_set.
+00000550: 6765 745f 7374 6172 745f 7374 6174 6573  get_start_states
+00000560: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00000570: 2020 2020 6c61 6265 6c5f 7365 742e 6765      label_set.ge
+00000580: 745f 656e 645f 7374 6174 6573 2829 2c0a  t_end_states(),.
+00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005a0: 6c61 6265 6c5f 7365 742e 6765 745f 7472  label_set.get_tr
+000005b0: 616e 7369 7469 6f6e 7328 292c 0a20 2020  ansitions(),.   
+000005c0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+000005d0: 2020 2020 292c 0a20 2020 2029 0a20 2020      ),.    ).   
+000005e0: 2072 6574 7572 6e20 7461 6767 6572 0a0a   return tagger..
+000005f0: 0a64 6566 2063 7265 6174 655f 636f 6c6c  .def create_coll
+00000600: 6174 6f72 280a 2020 2020 6d6f 6465 6c5f  ator(.    model_
+00000610: 6e61 6d65 3a20 7374 722c 206c 6162 656c  name: str, label
+00000620: 5f73 6574 3a20 4c61 6265 6c53 6574 2c20  _set: LabelSet, 
+00000630: 746f 6b65 6e69 7a65 725f 6172 6773 3a20  tokenizer_args: 
+00000640: 6469 6374 207c 204e 6f6e 6520 3d20 4e6f  dict | None = No
+00000650: 6e65 0a29 202d 3e20 436f 6c6c 6174 6f72  ne.) -> Collator
+00000660: 3a0a 2020 2020 2222 2243 7265 6174 6573  :.    """Creates
+00000670: 2061 2063 6f6c 6c61 746f 722e 0a0a 2020   a collator...  
+00000680: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00000690: 6d6f 6465 6c5f 6e61 6d65 3a20 4120 7374  model_name: A st
+000006a0: 7269 6e67 2072 6570 7265 7365 6e74 696e  ring representin
+000006b0: 6720 6120 7472 616e 7366 6f72 6d65 7227  g a transformer'
+000006c0: 7320 6d6f 6465 6c20 6e61 6d65 2e0a 2020  s model name..  
+000006d0: 2020 2020 2020 6c61 6265 6c5f 7365 743a        label_set:
+000006e0: 2041 204c 6162 656c 5365 7420 6f62 6a65   A LabelSet obje
+000006f0: 6374 2e0a 2020 2020 2020 2020 746f 6b65  ct..        toke
+00000700: 6e69 7a65 725f 6172 6773 3a20 4120 6469  nizer_args: A di
+00000710: 6374 696f 6e61 7279 2072 6570 7265 7365  ctionary represe
+00000720: 6e74 696e 6720 6172 6775 6d65 6e74 7320  nting arguments 
+00000730: 7061 7373 6564 2074 6f20 746f 6b65 6e69  passed to tokeni
+00000740: 7a65 722e 0a20 2020 2022 2222 0a20 2020  zer..    """.   
+00000750: 2062 6174 6368 5f66 6163 746f 7279 203d   batch_factory =
+00000760: 2054 7261 6e73 666f 726d 6572 4261 7463   TransformerBatc
+00000770: 6846 6163 746f 7279 280a 2020 2020 2020  hFactory(.      
+00000780: 2020 4175 746f 546f 6b65 6e69 7a65 722e    AutoTokenizer.
+00000790: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
+000007a0: 6d6f 6465 6c5f 6e61 6d65 292c 206c 6162  model_name), lab
+000007b0: 656c 5f73 6574 2c20 746f 6b65 6e69 7a65  el_set, tokenize
+000007c0: 725f 6172 6773 0a20 2020 2029 0a20 2020  r_args.    ).   
+000007d0: 2072 6574 7572 6e20 436f 6c6c 6174 6f72   return Collator
+000007e0: 2862 6174 6368 5f66 6163 746f 7279 290a  (batch_factory).
+000007f0: 0a0a 636c 6173 7320 4d65 7472 6963 3a0a  ..class Metric:.
+00000800: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000810: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00000820: 2020 2020 2020 2020 7365 6c66 2e5f 5f74          self.__t
+00000830: 7020 3d20 300a 2020 2020 2020 2020 7365  p = 0.        se
+00000840: 6c66 2e5f 5f66 7020 3d20 300a 2020 2020  lf.__fp = 0.    
+00000850: 2020 2020 7365 6c66 2e5f 5f66 6e20 3d20      self.__fn = 
+00000860: 300a 0a20 2020 2064 6566 205f 5f63 616c  0..    def __cal
+00000870: 6c5f 5f28 0a20 2020 2020 2020 2073 656c  l__(.        sel
+00000880: 662c 0a20 2020 2020 2020 2070 7265 6469  f,.        predi
+00000890: 6374 696f 6e73 3a20 4368 6172 4261 7365  ctions: CharBase
+000008a0: 6454 6167 7343 6f6c 6c65 6374 696f 6e2c  dTagsCollection,
+000008b0: 0a20 2020 2020 2020 2067 726f 756e 645f  .        ground_
+000008c0: 7472 7574 6873 3a20 4368 6172 4261 7365  truths: CharBase
+000008d0: 6454 6167 7343 6f6c 6c65 6374 696f 6e2c  dTagsCollection,
+000008e0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+000008f0: 2020 2020 2020 2020 666f 7220 7461 6773          for tags
+00000900: 312c 2074 6167 7332 2069 6e20 7a69 7028  1, tags2 in zip(
+00000910: 7072 6564 6963 7469 6f6e 732c 2067 726f  predictions, gro
+00000920: 756e 645f 7472 7574 6873 2c20 7374 7269  und_truths, stri
+00000930: 6374 3d54 7275 6529 3a0a 2020 2020 2020  ct=True):.      
+00000940: 2020 2020 2020 7461 675f 7365 7431 203d        tag_set1 =
+00000950: 207b 2874 6167 312e 7374 6172 742c 2074   {(tag1.start, t
+00000960: 6167 312e 6c65 6e67 7468 2c20 7461 6731  ag1.length, tag1
+00000970: 2e6c 6162 656c 2920 666f 7220 7461 6731  .label) for tag1
+00000980: 2069 6e20 7461 6773 317d 0a20 2020 2020   in tags1}.     
+00000990: 2020 2020 2020 2074 6167 5f73 6574 3220         tag_set2 
+000009a0: 3d20 7b28 7461 6732 2e73 7461 7274 2c20  = {(tag2.start, 
+000009b0: 7461 6732 2e6c 656e 6774 682c 2074 6167  tag2.length, tag
+000009c0: 322e 6c61 6265 6c29 2066 6f72 2074 6167  2.label) for tag
+000009d0: 3220 696e 2074 6167 7332 7d0a 0a20 2020  2 in tags2}..   
+000009e0: 2020 2020 2020 2020 2073 656c 662e 5f5f           self.__
+000009f0: 7470 202b 3d20 6c65 6e28 7461 675f 7365  tp += len(tag_se
+00000a00: 7431 2026 2074 6167 5f73 6574 3229 0a20  t1 & tag_set2). 
+00000a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000a20: 5f5f 6670 202b 3d20 6c65 6e28 7461 675f  __fp += len(tag_
+00000a30: 7365 7431 202d 2074 6167 5f73 6574 3229  set1 - tag_set2)
+00000a40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000a50: 662e 5f5f 666e 202b 3d20 6c65 6e28 7461  f.__fn += len(ta
+00000a60: 675f 7365 7432 202d 2074 6167 5f73 6574  g_set2 - tag_set
+00000a70: 3129 0a0a 2020 2020 6465 6620 6765 745f  1)..    def get_
+00000a80: 7363 6f72 6573 2873 656c 6629 202d 3e20  scores(self) -> 
+00000a90: 6469 6374 5b73 7472 2c20 666c 6f61 745d  dict[str, float]
+00000aa0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00000ab0: 662e 5f5f 7470 202b 2073 656c 662e 5f5f  f.__tp + self.__
+00000ac0: 6670 2021 3d20 303a 0a20 2020 2020 2020  fp != 0:.       
+00000ad0: 2020 2020 2070 7265 6369 7369 6f6e 203d       precision =
+00000ae0: 2073 656c 662e 5f5f 7470 202f 2028 7365   self.__tp / (se
+00000af0: 6c66 2e5f 5f74 7020 2b20 7365 6c66 2e5f  lf.__tp + self._
+00000b00: 5f66 7029 0a20 2020 2020 2020 2065 6c73  _fp).        els
+00000b10: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00000b20: 7265 6369 7369 6f6e 203d 2030 2e30 0a0a  recision = 0.0..
+00000b30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000b40: 5f5f 7470 202b 2073 656c 662e 5f5f 666e  __tp + self.__fn
+00000b50: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
+00000b60: 2020 2072 6563 616c 6c20 3d20 7365 6c66     recall = self
+00000b70: 2e5f 5f74 7020 2f20 2873 656c 662e 5f5f  .__tp / (self.__
+00000b80: 7470 202b 2073 656c 662e 5f5f 666e 290a  tp + self.__fn).
+00000b90: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000ba0: 2020 2020 2020 2020 2020 7265 6361 6c6c            recall
+00000bb0: 203d 2030 2e30 0a0a 2020 2020 2020 2020   = 0.0..        
+00000bc0: 6966 2070 7265 6369 7369 6f6e 202b 2072  if precision + r
+00000bd0: 6563 616c 6c20 3d3d 2030 2e30 3a0a 2020  ecall == 0.0:.  
+00000be0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000bf0: 207b 2266 315f 7363 6f72 6522 3a20 302e   {"f1_score": 0.
+00000c00: 302c 2022 7072 6563 6973 696f 6e22 3a20  0, "precision": 
+00000c10: 302e 302c 2022 7265 6361 6c6c 223a 2030  0.0, "recall": 0
+00000c20: 2e30 7d0a 2020 2020 2020 2020 656c 7365  .0}.        else
+00000c30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000c40: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
+00000c50: 2020 2020 2020 2022 6631 5f73 636f 7265         "f1_score
+00000c60: 223a 2032 202a 2070 7265 6369 7369 6f6e  ": 2 * precision
+00000c70: 202a 2072 6563 616c 6c20 2f20 2870 7265   * recall / (pre
+00000c80: 6369 7369 6f6e 202b 2072 6563 616c 6c29  cision + recall)
+00000c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000ca0: 2020 2270 7265 6369 7369 6f6e 223a 2070    "precision": p
+00000cb0: 7265 6369 7369 6f6e 2c0a 2020 2020 2020  recision,.      
+00000cc0: 2020 2020 2020 2020 2020 2272 6563 616c            "recal
+00000cd0: 6c22 3a20 7265 6361 6c6c 2c0a 2020 2020  l": recall,.    
+00000ce0: 2020 2020 2020 2020 7d0a                         }.
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/ddb4c8f62d6bd2f6` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/data/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,486 +1,464 @@
-00000000: 0100 0000 0000 0000 0900 0000 0000 0000  ................
-00000010: 6461 7461 2e63 6f72 6503 0000 0000 0000  data.core.......
-00000020: 0012 0000 0000 0000 0062 6973 6563 742e  .........bisect.
-00000030: 6269 7365 6374 5f6c 6566 7413 0000 001e  bisect_left.....
-00000040: 0000 0018 0000 0000 0000 0063 6f6c 6c65  ...........colle
-00000050: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
-00000060: 746f 723b 0000 0043 0000 0015 0000 0000  tor;...C........
-00000070: 0000 0064 6174 6163 6c61 7373 6573 2e64  ...dataclasses.d
-00000080: 6174 6163 6c61 7373 5c00 0000 6500 0000  ataclass\...e...
-00000090: 0100 0000 0000 0000 1800 0000 0000 0000  ................
-000000a0: 5a69 7057 6974 686f 7574 4578 706c 6963  ZipWithoutExplic
-000000b0: 6974 5374 7269 6374 2f00 0000 0000 0000  itStrict/.......
-000000c0: 607a 6970 2829 6020 7769 7468 6f75 7420  `zip()` without 
-000000d0: 616e 2065 7870 6c69 6369 7420 6073 7472  an explicit `str
-000000e0: 6963 743d 6020 7061 7261 6d65 7465 7200  ict=` parameter.
-000000f0: a010 0000 c810 0000 0000 0000 0000 0000  ................
-00000100: 00a0 1000 0001 0000 0000 0000 0050 0000  .............P..
-00000110: 0000 0000 002f 5573 6572 732f 7961 7375  ...../Users/yasu
-00000120: 6675 6d69 2f57 6f72 6b73 7061 6365 2f70  fumi/Workspace/p
-00000130: 7974 6f72 6368 2d70 6172 7469 616c 2d74  ytorch-partial-t
-00000140: 6167 6765 722f 7372 632f 7061 7274 6961  agger/src/partia
-00000150: 6c5f 7461 6767 6572 2f64 6174 612f 636f  l_tagger/data/co
-00000160: 7265 2e70 79ed 1c00 0000 0000 0066 726f  re.py........fro
-00000170: 6d20 6269 7365 6374 2069 6d70 6f72 7420  m bisect import 
-00000180: 6269 7365 6374 5f6c 6566 740a 6672 6f6d  bisect_left.from
-00000190: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-000001a0: 2069 6d70 6f72 7420 4974 6572 6174 6f72   import Iterator
-000001b0: 0a66 726f 6d20 6461 7461 636c 6173 7365  .from dataclasse
-000001c0: 7320 696d 706f 7274 2064 6174 6163 6c61  s import datacla
-000001d0: 7373 0a0a 0a40 6461 7461 636c 6173 7328  ss...@dataclass(
-000001e0: 6672 6f7a 656e 3d54 7275 652c 2065 713d  frozen=True, eq=
-000001f0: 5472 7565 290a 636c 6173 7320 5370 616e  True).class Span
-00000200: 3a0a 2020 2020 7374 6172 743a 2069 6e74  :.    start: int
-00000210: 0a20 2020 206c 656e 6774 683a 2069 6e74  .    length: int
-00000220: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
-00000230: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
-00000240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000250: 6861 7368 2828 7365 6c66 2e73 7461 7274  hash((self.start
-00000260: 2c20 7365 6c66 2e6c 656e 6774 6829 290a  , self.length)).
-00000270: 0a0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000280: 7a65 6e3d 5472 7565 2c20 6571 3d54 7275  zen=True, eq=Tru
-00000290: 6529 0a63 6c61 7373 2054 6167 3a0a 2020  e).class Tag:.  
-000002a0: 2020 7370 616e 3a20 5370 616e 0a20 2020    span: Span.   
-000002b0: 206c 6162 656c 3a20 7374 720a 0a20 2020   label: str..   
-000002c0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000002d0: 6566 2073 7461 7274 2873 656c 6629 202d  ef start(self) -
-000002e0: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
-000002f0: 6574 7572 6e20 7365 6c66 2e73 7061 6e2e  eturn self.span.
-00000300: 7374 6172 740a 0a20 2020 2040 7072 6f70  start..    @prop
-00000310: 6572 7479 0a20 2020 2064 6566 206c 656e  erty.    def len
-00000320: 6774 6828 7365 6c66 2920 2d3e 2069 6e74  gth(self) -> int
-00000330: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000340: 2073 656c 662e 7370 616e 2e6c 656e 6774   self.span.lengt
-00000350: 680a 0a0a 4064 6174 6163 6c61 7373 2866  h...@dataclass(f
-00000360: 726f 7a65 6e3d 5472 7565 2c20 6571 3d54  rozen=True, eq=T
-00000370: 7275 6529 0a63 6c61 7373 2043 6861 7242  rue).class CharB
-00000380: 6173 6564 5461 6773 3a0a 2020 2020 7461  asedTags:.    ta
-00000390: 6773 3a20 7475 706c 655b 5461 672c 202e  gs: tuple[Tag, .
-000003a0: 2e2e 5d0a 2020 2020 7465 7874 3a20 7374  ..].    text: st
-000003b0: 720a 0a20 2020 2064 6566 205f 5f69 7465  r..    def __ite
-000003c0: 725f 5f28 7365 6c66 2920 2d3e 2049 7465  r__(self) -> Ite
-000003d0: 7261 746f 725b 5461 675d 3a0a 2020 2020  rator[Tag]:.    
-000003e0: 2020 2020 7969 656c 6420 6672 6f6d 2073      yield from s
-000003f0: 656c 662e 7461 6773 0a0a 2020 2020 6465  elf.tags..    de
-00000400: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
-00000410: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00000420: 2074 6167 5f73 7472 7320 3d20 5b5d 0a20   tag_strs = []. 
-00000430: 2020 2020 2020 2066 6f72 2074 6167 2069         for tag i
-00000440: 6e20 7365 6c66 3a0a 2020 2020 2020 2020  n self:.        
-00000450: 2020 2020 7374 6172 7420 3d20 7461 672e      start = tag.
-00000460: 7374 6172 740a 2020 2020 2020 2020 2020  start.          
-00000470: 2020 656e 6420 3d20 7461 672e 7374 6172    end = tag.star
-00000480: 7420 2b20 7461 672e 6c65 6e67 7468 0a20  t + tag.length. 
-00000490: 2020 2020 2020 2020 2020 2074 6167 5f73             tag_s
-000004a0: 7472 203d 2066 227b 7365 6c66 2e74 6578  tr = f"{self.tex
-000004b0: 745b 7374 6172 743a 656e 645d 7d20 287b  t[start:end]} ({
-000004c0: 7461 672e 6c61 6265 6c7d 2922 0a20 2020  tag.label})".   
-000004d0: 2020 2020 2020 2020 2074 6167 5f73 7472           tag_str
-000004e0: 732e 6170 7065 6e64 2874 6167 5f73 7472  s.append(tag_str
-000004f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00000500: 2066 2228 7b27 2c20 272e 6a6f 696e 2874   f"({', '.join(t
-00000510: 6167 5f73 7472 7329 7d29 220a 0a0a 636c  ag_strs)})"...cl
-00000520: 6173 7320 546f 6b65 6e69 7a65 6454 6578  ass TokenizedTex
-00000530: 743a 0a20 2020 2064 6566 205f 5f69 6e69  t:.    def __ini
-00000540: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00000550: 662c 0a20 2020 2020 2020 2074 6578 743a  f,.        text:
-00000560: 2073 7472 2c0a 2020 2020 2020 2020 6368   str,.        ch
-00000570: 6172 5f73 7061 6e73 3a20 7475 706c 655b  ar_spans: tuple[
-00000580: 5370 616e 207c 204e 6f6e 652c 202e 2e2e  Span | None, ...
-00000590: 5d2c 0a20 2020 2020 2020 2074 6f6b 656e  ],.        token
-000005a0: 5f69 6e64 6963 6573 3a20 7475 706c 655b  _indices: tuple[
-000005b0: 696e 742c 202e 2e2e 5d2c 0a20 2020 2020  int, ...],.     
-000005c0: 2020 2061 6464 7469 6f6e 616c 5f74 6f6b     addtional_tok
-000005d0: 656e 3a20 7374 7220 3d20 225b 546f 6b65  en: str = "[Toke
-000005e0: 6e5d 222c 0a20 2020 2029 3a0a 2020 2020  n]",.    ):.    
-000005f0: 2020 2020 7365 6c66 2e5f 5f74 6578 7420      self.__text 
-00000600: 3d20 7465 7874 0a20 2020 2020 2020 2073  = text.        s
-00000610: 656c 662e 5f5f 6368 6172 5f73 7061 6e73  elf.__char_spans
-00000620: 203d 2063 6861 725f 7370 616e 730a 2020   = char_spans.  
-00000630: 2020 2020 2020 7365 6c66 2e5f 5f74 6f6b        self.__tok
-00000640: 656e 5f69 6e64 6963 6573 203d 2074 6f6b  en_indices = tok
-00000650: 656e 5f69 6e64 6963 6573 0a20 2020 2020  en_indices.     
-00000660: 2020 2073 656c 662e 5f5f 6164 6474 696f     self.__addtio
-00000670: 6e61 6c5f 746f 6b65 6e20 3d20 6164 6474  nal_token = addt
-00000680: 696f 6e61 6c5f 746f 6b65 6e0a 0a20 2020  ional_token..   
-00000690: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-000006a0: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
-000006b0: 2020 2020 7465 7874 203d 205b 5d0a 2020      text = [].  
-000006c0: 2020 2020 2020 666f 7220 7370 616e 2069        for span i
-000006d0: 6e20 7365 6c66 2e5f 5f63 6861 725f 7370  n self.__char_sp
-000006e0: 616e 733a 0a20 2020 2020 2020 2020 2020  ans:.           
-000006f0: 2069 6620 7370 616e 2069 7320 4e6f 6e65   if span is None
-00000700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000710: 2020 7465 7874 2e61 7070 656e 6428 7365    text.append(se
-00000720: 6c66 2e5f 5f61 6464 7469 6f6e 616c 5f74  lf.__addtional_t
-00000730: 6f6b 656e 290a 2020 2020 2020 2020 2020  oken).          
-00000740: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000750: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
-00000760: 7370 616e 2e73 7461 7274 0a20 2020 2020  span.start.     
-00000770: 2020 2020 2020 2020 2020 2065 6e64 203d             end =
-00000780: 2073 7461 7274 202b 2073 7061 6e2e 6c65   start + span.le
-00000790: 6e67 7468 0a20 2020 2020 2020 2020 2020  ngth.           
-000007a0: 2020 2020 2074 6578 742e 6170 7065 6e64       text.append
-000007b0: 2873 656c 662e 5f5f 7465 7874 5b73 7461  (self.__text[sta
-000007c0: 7274 3a65 6e64 5d29 0a20 2020 2020 2020  rt:end]).       
-000007d0: 2072 6574 7572 6e20 2220 222e 6a6f 696e   return " ".join
-000007e0: 2874 6578 7429 0a0a 2020 2020 4070 726f  (text)..    @pro
-000007f0: 7065 7274 790a 2020 2020 6465 6620 6e75  perty.    def nu
-00000800: 6d5f 746f 6b65 6e73 2873 656c 6629 202d  m_tokens(self) -
-00000810: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
-00000820: 6574 7572 6e20 6c65 6e28 7365 6c66 2e5f  eturn len(self._
-00000830: 5f63 6861 725f 7370 616e 7329 0a0a 2020  _char_spans)..  
-00000840: 2020 6465 6620 6765 745f 7465 7874 2873    def get_text(s
-00000850: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-00000860: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000870: 2e5f 5f74 6578 740a 0a20 2020 2064 6566  .__text..    def
-00000880: 2067 6574 5f74 6f6b 656e 2873 656c 662c   get_token(self,
-00000890: 2074 6f6b 656e 5f69 6e64 6578 3a20 696e   token_index: in
-000008a0: 7429 202d 3e20 7374 723a 0a20 2020 2020  t) -> str:.     
-000008b0: 2020 2063 6861 725f 7370 616e 203d 2073     char_span = s
-000008c0: 656c 662e 5f5f 6368 6172 5f73 7061 6e73  elf.__char_spans
-000008d0: 5b74 6f6b 656e 5f69 6e64 6578 5d0a 2020  [token_index].  
-000008e0: 2020 2020 2020 6966 2063 6861 725f 7370        if char_sp
-000008f0: 616e 2069 7320 4e6f 6e65 3a0a 2020 2020  an is None:.    
-00000900: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000910: 656c 662e 5f5f 6164 6474 696f 6e61 6c5f  elf.__addtional_
-00000920: 746f 6b65 6e0a 2020 2020 2020 2020 656c  token.        el
-00000930: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000940: 7374 6172 7420 3d20 6368 6172 5f73 7061  start = char_spa
-00000950: 6e2e 7374 6172 740a 2020 2020 2020 2020  n.start.        
-00000960: 2020 2020 656e 6420 3d20 7374 6172 7420      end = start 
-00000970: 2b20 6368 6172 5f73 7061 6e2e 6c65 6e67  + char_span.leng
-00000980: 7468 0a20 2020 2020 2020 2020 2020 2072  th.            r
-00000990: 6574 7572 6e20 7365 6c66 2e5f 5f74 6578  eturn self.__tex
-000009a0: 745b 7374 6172 743a 656e 645d 0a0a 2020  t[start:end]..  
-000009b0: 2020 6465 6620 6765 745f 6368 6172 5f73    def get_char_s
-000009c0: 7061 6e28 7365 6c66 2c20 746f 6b65 6e5f  pan(self, token_
-000009d0: 696e 6465 783a 2069 6e74 2920 2d3e 2053  index: int) -> S
-000009e0: 7061 6e20 7c20 4e6f 6e65 3a0a 2020 2020  pan | None:.    
-000009f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00000a00: 5f5f 6368 6172 5f73 7061 6e73 5b74 6f6b  __char_spans[tok
-00000a10: 656e 5f69 6e64 6578 5d0a 0a20 2020 2064  en_index]..    d
-00000a20: 6566 2063 6f6e 7665 7274 5f74 6f5f 746f  ef convert_to_to
-00000a30: 6b65 6e5f 696e 6465 7828 7365 6c66 2c20  ken_index(self, 
-00000a40: 6368 6172 5f69 6e64 6578 3a20 696e 7429  char_index: int)
-00000a50: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00000a60: 2072 6574 7572 6e20 7365 6c66 2e5f 5f74   return self.__t
-00000a70: 6f6b 656e 5f69 6e64 6963 6573 5b63 6861  oken_indices[cha
-00000a80: 725f 696e 6465 785d 0a0a 2020 2020 6465  r_index]..    de
-00000a90: 6620 636f 6e76 6572 745f 746f 5f63 6861  f convert_to_cha
-00000aa0: 725f 7370 616e 2873 656c 662c 2074 6f6b  r_span(self, tok
-00000ab0: 656e 5f73 7061 6e3a 2053 7061 6e29 202d  en_span: Span) -
-00000ac0: 3e20 5370 616e 207c 204e 6f6e 653a 0a20  > Span | None:. 
-00000ad0: 2020 2020 2020 2063 6861 725f 7370 616e         char_span
-00000ae0: 5f73 7461 7274 203d 2073 656c 662e 5f5f  _start = self.__
-00000af0: 6368 6172 5f73 7061 6e73 5b74 6f6b 656e  char_spans[token
-00000b00: 5f73 7061 6e2e 7374 6172 745d 0a20 2020  _span.start].   
-00000b10: 2020 2020 2063 6861 725f 7370 616e 5f65       char_span_e
-00000b20: 6e64 203d 2073 656c 662e 5f5f 6368 6172  nd = self.__char
-00000b30: 5f73 7061 6e73 5b74 6f6b 656e 5f73 7061  _spans[token_spa
-00000b40: 6e2e 7374 6172 7420 2b20 746f 6b65 6e5f  n.start + token_
-00000b50: 7370 616e 2e6c 656e 6774 6820 2d20 315d  span.length - 1]
-00000b60: 0a0a 2020 2020 2020 2020 6966 2063 6861  ..        if cha
-00000b70: 725f 7370 616e 5f73 7461 7274 2069 7320  r_span_start is 
-00000b80: 4e6f 6e65 206f 7220 6368 6172 5f73 7061  None or char_spa
-00000b90: 6e5f 656e 6420 6973 204e 6f6e 653a 0a20  n_end is None:. 
-00000ba0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000bb0: 6e20 4e6f 6e65 0a0a 2020 2020 2020 2020  n None..        
-00000bc0: 7265 7475 726e 2053 7061 6e28 0a20 2020  return Span(.   
-00000bd0: 2020 2020 2020 2020 2063 6861 725f 7370           char_sp
-00000be0: 616e 5f73 7461 7274 2e73 7461 7274 2c0a  an_start.start,.
-00000bf0: 2020 2020 2020 2020 2020 2020 6368 6172              char
-00000c00: 5f73 7061 6e5f 656e 642e 7374 6172 7420  _span_end.start 
-00000c10: 2b20 6368 6172 5f73 7061 6e5f 656e 642e  + char_span_end.
-00000c20: 6c65 6e67 7468 202d 2063 6861 725f 7370  length - char_sp
-00000c30: 616e 5f73 7461 7274 2e73 7461 7274 2c0a  an_start.start,.
-00000c40: 2020 2020 2020 2020 290a 0a0a 4064 6174          )...@dat
-00000c50: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
-00000c60: 7565 290a 636c 6173 7320 5375 6277 6f72  ue).class Subwor
-00000c70: 6442 6173 6564 5461 6773 3a0a 2020 2020  dBasedTags:.    
-00000c80: 7461 6773 3a20 7475 706c 655b 5461 672c  tags: tuple[Tag,
-00000c90: 202e 2e2e 5d0a 2020 2020 746f 6b65 6e69   ...].    tokeni
-00000ca0: 7a65 645f 7465 7874 3a20 546f 6b65 6e69  zed_text: Tokeni
-00000cb0: 7a65 6454 6578 740a 0a20 2020 2064 6566  zedText..    def
-00000cc0: 205f 5f69 7465 725f 5f28 7365 6c66 2920   __iter__(self) 
-00000cd0: 2d3e 2049 7465 7261 746f 725b 5461 675d  -> Iterator[Tag]
-00000ce0: 3a0a 2020 2020 2020 2020 7969 656c 6420  :.        yield 
-00000cf0: 6672 6f6d 2073 656c 662e 7461 6773 0a0a  from self.tags..
-00000d00: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00000d10: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-00000d20: 2020 2020 2020 2074 6167 5f73 7472 7320         tag_strs 
-00000d30: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-00000d40: 2074 6167 2069 6e20 7365 6c66 3a0a 2020   tag in self:.  
-00000d50: 2020 2020 2020 2020 2020 7374 6172 7420            start 
-00000d60: 3d20 7461 672e 7374 6172 740a 2020 2020  = tag.start.    
-00000d70: 2020 2020 2020 2020 656e 6420 3d20 7374          end = st
-00000d80: 6172 7420 2b20 7461 672e 6c65 6e67 7468  art + tag.length
-00000d90: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
-00000da0: 5f73 7472 203d 2022 2022 2e6a 6f69 6e28  _str = " ".join(
-00000db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000dc0: 2073 656c 662e 746f 6b65 6e69 7a65 645f   self.tokenized_
-00000dd0: 7465 7874 2e67 6574 5f74 6f6b 656e 2874  text.get_token(t
-00000de0: 6f6b 656e 5f69 6e64 6578 290a 2020 2020  oken_index).    
-00000df0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000e00: 746f 6b65 6e5f 696e 6465 7820 696e 2072  token_index in r
-00000e10: 616e 6765 2873 7461 7274 2c20 656e 6429  ange(start, end)
-00000e20: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00000e30: 2020 2020 2020 2020 2020 2074 6167 5f73             tag_s
-00000e40: 7472 732e 6170 7065 6e64 2866 227b 7461  trs.append(f"{ta
-00000e50: 675f 7374 727d 2028 7b74 6167 2e6c 6162  g_str} ({tag.lab
-00000e60: 656c 7d29 2229 0a20 2020 2020 2020 2072  el})").        r
-00000e70: 6574 7572 6e20 6622 287b 272c 2027 2e6a  eturn f"({', '.j
-00000e80: 6f69 6e28 7461 675f 7374 7273 297d 2922  oin(tag_strs)})"
-00000e90: 0a0a 2020 2020 6465 6620 6765 745f 6368  ..    def get_ch
-00000ea0: 6172 5f62 6173 6564 5f74 6167 7328 7365  ar_based_tags(se
-00000eb0: 6c66 2920 2d3e 2043 6861 7242 6173 6564  lf) -> CharBased
-00000ec0: 5461 6773 3a0a 2020 2020 2020 2020 7461  Tags:.        ta
-00000ed0: 6773 203d 205b 5d0a 2020 2020 2020 2020  gs = [].        
-00000ee0: 666f 7220 7461 6720 696e 2073 656c 662e  for tag in self.
-00000ef0: 7461 6773 3a0a 2020 2020 2020 2020 2020  tags:.          
-00000f00: 2020 6368 6172 5f73 7061 6e20 3d20 7365    char_span = se
-00000f10: 6c66 2e74 6f6b 656e 697a 6564 5f74 6578  lf.tokenized_tex
-00000f20: 742e 636f 6e76 6572 745f 746f 5f63 6861  t.convert_to_cha
-00000f30: 725f 7370 616e 2874 6167 2e73 7061 6e29  r_span(tag.span)
-00000f40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000f50: 6368 6172 5f73 7061 6e20 6973 206e 6f74  char_span is not
-00000f60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00000f70: 2020 2020 2020 2074 6167 732e 6170 7065         tags.appe
-00000f80: 6e64 2854 6167 2863 6861 725f 7370 616e  nd(Tag(char_span
-00000f90: 2c20 7461 672e 6c61 6265 6c29 290a 2020  , tag.label)).  
-00000fa0: 2020 2020 2020 7265 7475 726e 2043 6861        return Cha
-00000fb0: 7242 6173 6564 5461 6773 2874 7570 6c65  rBasedTags(tuple
-00000fc0: 2874 6167 7329 2c20 7365 6c66 2e74 6f6b  (tags), self.tok
-00000fd0: 656e 697a 6564 5f74 6578 742e 6765 745f  enized_text.get_
-00000fe0: 7465 7874 2829 290a 0a0a 636c 6173 7320  text())...class 
-00000ff0: 4c61 6265 6c53 6574 3a0a 2020 2020 6465  LabelSet:.    de
-00001000: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00001010: 206c 6162 656c 733a 2073 6574 5b73 7472   labels: set[str
-00001020: 5d29 3a0a 2020 2020 2020 2020 7365 6c66  ]):.        self
-00001030: 2e5f 5f6c 6162 656c 7320 3d20 5b2a 736f  .__labels = [*so
-00001040: 7274 6564 286c 6162 656c 7329 5d0a 2020  rted(labels)].  
-00001050: 2020 2020 2020 7365 6c66 2e5f 5f73 7461        self.__sta
-00001060: 7475 735f 6b69 6e64 203d 2034 2020 2320  tus_kind = 4  # 
-00001070: 7374 6172 742c 2069 6e73 6964 652c 2065  start, inside, e
-00001080: 6e64 2c20 756e 6974 0a0a 2020 2020 2020  nd, unit..      
-00001090: 2020 7365 6c66 2e5f 5f73 7461 7274 5f69    self.__start_i
-000010a0: 6e64 6963 6573 203d 205b 0a20 2020 2020  ndices = [.     
-000010b0: 2020 2020 2020 202a 7261 6e67 6528 0a20         *range(. 
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-000010d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000010e0: 2020 7365 6c66 2e67 6574 5f74 6167 5f73    self.get_tag_s
-000010f0: 697a 6528 292c 0a20 2020 2020 2020 2020  ize(),.         
-00001100: 2020 2020 2020 2073 656c 662e 5f5f 7374         self.__st
-00001110: 6174 7573 5f6b 696e 642c 0a20 2020 2020  atus_kind,.     
-00001120: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001130: 205d 0a20 2020 2020 2020 2073 656c 662e   ].        self.
-00001140: 5f5f 756e 6974 5f69 6e64 6963 6573 203d  __unit_indices =
-00001150: 205b 0a20 2020 2020 2020 2020 2020 202a   [.            *
-00001160: 7261 6e67 6528 0a20 2020 2020 2020 2020  range(.         
-00001170: 2020 2020 2020 2073 656c 662e 5f5f 7374         self.__st
-00001180: 6174 7573 5f6b 696e 642c 0a20 2020 2020  atus_kind,.     
-00001190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000011a0: 6765 745f 7461 675f 7369 7a65 2829 2c0a  get_tag_size(),.
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 7365 6c66 2e5f 5f73 7461 7475 735f 6b69  self.__status_ki
-000011d0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-000011e0: 290a 2020 2020 2020 2020 5d0a 0a20 2020  ).        ]..   
-000011f0: 2020 2020 2073 656c 662e 5f5f 6c61 6265       self.__labe
-00001200: 6c5f 6964 7320 3d20 6469 6374 287a 6970  l_ids = dict(zip
-00001210: 2873 656c 662e 5f5f 6c61 6265 6c73 2c20  (self.__labels, 
-00001220: 7365 6c66 2e5f 5f73 7461 7274 5f69 6e64  self.__start_ind
-00001230: 6963 6573 2929 0a0a 2020 2020 6465 6620  ices))..    def 
-00001240: 6765 745f 6f75 7473 6964 655f 696e 6465  get_outside_inde
-00001250: 7828 7365 6c66 2920 2d3e 2069 6e74 3a0a  x(self) -> int:.
-00001260: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
-00001270: 0a0a 2020 2020 6465 6620 6765 745f 7374  ..    def get_st
-00001280: 6172 745f 696e 6465 7828 7365 6c66 2c20  art_index(self, 
-00001290: 6c61 6265 6c3a 2073 7472 2920 2d3e 2069  label: str) -> i
-000012a0: 6e74 3a0a 2020 2020 2020 2020 6966 206c  nt:.        if l
-000012b0: 6162 656c 206e 6f74 2069 6e20 7365 6c66  abel not in self
-000012c0: 2e5f 5f6c 6162 656c 5f69 6473 3a0a 2020  .__label_ids:.  
-000012d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000012e0: 5661 6c75 6545 7272 6f72 2822 496e 7661  ValueError("Inva
-000012f0: 6c69 6420 6c61 6265 6c20 6973 2067 6976  lid label is giv
-00001300: 656e 2e22 290a 2020 2020 2020 2020 7265  en.").        re
-00001310: 7475 726e 2073 656c 662e 5f5f 6c61 6265  turn self.__labe
-00001320: 6c5f 6964 735b 6c61 6265 6c5d 0a0a 2020  l_ids[label]..  
-00001330: 2020 6465 6620 6765 745f 696e 7369 6465    def get_inside
-00001340: 5f69 6e64 6578 2873 656c 662c 206c 6162  _index(self, lab
-00001350: 656c 3a20 7374 7229 202d 3e20 696e 743a  el: str) -> int:
-00001360: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001370: 7365 6c66 2e67 6574 5f73 7461 7274 5f69  self.get_start_i
-00001380: 6e64 6578 286c 6162 656c 2920 2b20 310a  ndex(label) + 1.
-00001390: 0a20 2020 2064 6566 2067 6574 5f65 6e64  .    def get_end
-000013a0: 5f69 6e64 6578 2873 656c 662c 206c 6162  _index(self, lab
-000013b0: 656c 3a20 7374 7229 202d 3e20 696e 743a  el: str) -> int:
-000013c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000013d0: 7365 6c66 2e67 6574 5f73 7461 7274 5f69  self.get_start_i
-000013e0: 6e64 6578 286c 6162 656c 2920 2b20 320a  ndex(label) + 2.
-000013f0: 0a20 2020 2064 6566 2067 6574 5f75 6e69  .    def get_uni
-00001400: 745f 696e 6465 7828 7365 6c66 2c20 6c61  t_index(self, la
-00001410: 6265 6c3a 2073 7472 2920 2d3e 2069 6e74  bel: str) -> int
-00001420: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00001430: 2073 656c 662e 6765 745f 7374 6172 745f   self.get_start_
-00001440: 696e 6465 7828 6c61 6265 6c29 202b 2033  index(label) + 3
-00001450: 0a0a 2020 2020 6465 6620 6765 745f 6c61  ..    def get_la
-00001460: 6265 6c5f 7369 7a65 2873 656c 6629 202d  bel_size(self) -
-00001470: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
-00001480: 6574 7572 6e20 6c65 6e28 7365 6c66 2e5f  eturn len(self._
-00001490: 5f6c 6162 656c 7329 0a0a 2020 2020 6465  _labels)..    de
-000014a0: 6620 6765 745f 7461 675f 7369 7a65 2873  f get_tag_size(s
-000014b0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-000014c0: 2020 2020 2023 2028 7374 6172 742c 2069       # (start, i
-000014d0: 6e73 6964 652c 2065 6e64 2c20 756e 6974  nside, end, unit
-000014e0: 2920 2a20 6c61 6265 6c20 2b20 6f75 7473  ) * label + outs
-000014f0: 6964 6520 7374 6174 7573 0a20 2020 2020  ide status.     
-00001500: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00001510: 5f73 7461 7475 735f 6b69 6e64 202a 2073  _status_kind * s
-00001520: 656c 662e 6765 745f 6c61 6265 6c5f 7369  elf.get_label_si
-00001530: 7a65 2829 202b 2031 0a0a 2020 2020 6465  ze() + 1..    de
-00001540: 6620 6765 745f 6c61 6265 6c28 7365 6c66  f get_label(self
-00001550: 2c20 696e 6465 783a 2069 6e74 2920 2d3e  , index: int) ->
-00001560: 2073 7472 207c 204e 6f6e 653a 0a20 2020   str | None:.   
-00001570: 2020 2020 2069 6620 696e 6465 7820 3c20       if index < 
-00001580: 3020 6f72 2069 6e64 6578 203e 3d20 7365  0 or index >= se
-00001590: 6c66 2e67 6574 5f74 6167 5f73 697a 6528  lf.get_tag_size(
-000015a0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-000015b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000015c0: 2249 6e76 616c 6964 2069 6e64 6578 2e22  "Invalid index."
-000015d0: 290a 0a20 2020 2020 2020 2069 6620 696e  )..        if in
-000015e0: 6465 7820 3d3d 2073 656c 662e 6765 745f  dex == self.get_
-000015f0: 6f75 7473 6964 655f 696e 6465 7828 293a  outside_index():
-00001600: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001610: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-00001620: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00001630: 6c61 6265 6c73 5b62 6973 6563 745f 6c65  labels[bisect_le
-00001640: 6674 2873 656c 662e 5f5f 756e 6974 5f69  ft(self.__unit_i
-00001650: 6e64 6963 6573 2c20 696e 6465 7829 5d0a  ndices, index)].
-00001660: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
-00001670: 7274 5f73 7461 7465 7328 7365 6c66 2920  rt_states(self) 
-00001680: 2d3e 206c 6973 745b 626f 6f6c 5d3a 0a20  -> list[bool]:. 
-00001690: 2020 2020 2020 2073 7461 7465 7320 3d20         states = 
-000016a0: 5b46 616c 7365 5d20 2a20 7365 6c66 2e67  [False] * self.g
-000016b0: 6574 5f74 6167 5f73 697a 6528 290a 2020  et_tag_size().  
-000016c0: 2020 2020 2020 2320 416c 7761 7973 2061        # Always a
-000016d0: 6c6c 6f77 6564 2073 7461 7274 7320 6672  llowed starts fr
-000016e0: 6f6d 206f 7574 7369 6465 2073 7461 7475  om outside statu
-000016f0: 730a 2020 2020 2020 2020 7374 6174 6573  s.        states
-00001700: 5b73 656c 662e 6765 745f 6f75 7473 6964  [self.get_outsid
-00001710: 655f 696e 6465 7828 295d 203d 2054 7275  e_index()] = Tru
-00001720: 650a 0a20 2020 2020 2020 2066 6f72 206c  e..        for l
-00001730: 6162 656c 6564 5f73 7461 7274 5f69 6e64  abeled_start_ind
-00001740: 6578 2069 6e20 7365 6c66 2e5f 5f73 7461  ex in self.__sta
-00001750: 7274 5f69 6e64 6963 6573 3a0a 2020 2020  rt_indices:.    
-00001760: 2020 2020 2020 2020 6c61 6265 6c65 645f          labeled_
-00001770: 756e 6974 5f69 6e64 6578 203d 206c 6162  unit_index = lab
-00001780: 656c 6564 5f73 7461 7274 5f69 6e64 6578  eled_start_index
-00001790: 202b 2033 0a20 2020 2020 2020 2020 2020   + 3.           
-000017a0: 2073 7461 7465 735b 6c61 6265 6c65 645f   states[labeled_
-000017b0: 7374 6172 745f 696e 6465 785d 203d 2054  start_index] = T
-000017c0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-000017d0: 7374 6174 6573 5b6c 6162 656c 6564 5f75  states[labeled_u
-000017e0: 6e69 745f 696e 6465 785d 203d 2054 7275  nit_index] = Tru
-000017f0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00001800: 2073 7461 7465 730a 0a20 2020 2064 6566   states..    def
-00001810: 2067 6574 5f65 6e64 5f73 7461 7465 7328   get_end_states(
-00001820: 7365 6c66 2920 2d3e 206c 6973 745b 626f  self) -> list[bo
-00001830: 6f6c 5d3a 0a20 2020 2020 2020 2073 7461  ol]:.        sta
-00001840: 7465 7320 3d20 5b46 616c 7365 5d20 2a20  tes = [False] * 
-00001850: 7365 6c66 2e67 6574 5f74 6167 5f73 697a  self.get_tag_siz
-00001860: 6528 290a 2020 2020 2020 2020 2320 416c  e().        # Al
-00001870: 7761 7973 2061 6c6c 6f77 6564 2065 6e64  ways allowed end
-00001880: 7320 7769 7468 206f 7574 7369 6465 2073  s with outside s
-00001890: 7461 7475 730a 2020 2020 2020 2020 7374  tatus.        st
-000018a0: 6174 6573 5b73 656c 662e 6765 745f 6f75  ates[self.get_ou
-000018b0: 7473 6964 655f 696e 6465 7828 295d 203d  tside_index()] =
-000018c0: 2054 7275 650a 0a20 2020 2020 2020 2066   True..        f
-000018d0: 6f72 206c 6162 656c 6564 5f75 6e69 745f  or labeled_unit_
-000018e0: 696e 6465 7820 696e 2073 656c 662e 5f5f  index in self.__
-000018f0: 756e 6974 5f69 6e64 6963 6573 3a0a 2020  unit_indices:.  
-00001900: 2020 2020 2020 2020 2020 6c61 6265 6c65            labele
-00001910: 645f 656e 645f 696e 6465 7820 3d20 6c61  d_end_index = la
-00001920: 6265 6c65 645f 756e 6974 5f69 6e64 6578  beled_unit_index
-00001930: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
-00001940: 2073 7461 7465 735b 6c61 6265 6c65 645f   states[labeled_
-00001950: 656e 645f 696e 6465 785d 203d 2054 7275  end_index] = Tru
-00001960: 650a 2020 2020 2020 2020 2020 2020 7374  e.            st
-00001970: 6174 6573 5b6c 6162 656c 6564 5f75 6e69  ates[labeled_uni
-00001980: 745f 696e 6465 785d 203d 2054 7275 650a  t_index] = True.
-00001990: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000019a0: 7461 7465 730a 0a20 2020 2064 6566 2067  tates..    def g
-000019b0: 6574 5f74 7261 6e73 6974 696f 6e73 2873  et_transitions(s
-000019c0: 656c 6629 202d 3e20 6c69 7374 5b6c 6973  elf) -> list[lis
-000019d0: 745b 626f 6f6c 5d5d 3a0a 2020 2020 2020  t[bool]]:.      
-000019e0: 2020 7472 616e 7369 7469 6f6e 7320 3d20    transitions = 
-000019f0: 5b0a 2020 2020 2020 2020 2020 2020 5b46  [.            [F
-00001a00: 616c 7365 5d20 2a20 7365 6c66 2e67 6574  alse] * self.get
-00001a10: 5f74 6167 5f73 697a 6528 2920 666f 7220  _tag_size() for 
-00001a20: 5f20 696e 2072 616e 6765 2873 656c 662e  _ in range(self.
-00001a30: 6765 745f 7461 675f 7369 7a65 2829 290a  get_tag_size()).
-00001a40: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00001a50: 2020 6f75 7473 6964 655f 696e 6465 7820    outside_index 
-00001a60: 3d20 7365 6c66 2e67 6574 5f6f 7574 7369  = self.get_outsi
-00001a70: 6465 5f69 6e64 6578 2829 0a20 2020 2020  de_index().     
-00001a80: 2020 2074 7261 6e73 6974 696f 6e73 5b6f     transitions[o
-00001a90: 7574 7369 6465 5f69 6e64 6578 5d20 3d20  utside_index] = 
-00001aa0: 7365 6c66 2e67 6574 5f73 7461 7274 5f73  self.get_start_s
-00001ab0: 7461 7465 7328 290a 0a20 2020 2020 2020  tates()..       
-00001ac0: 2066 6f72 206c 6162 656c 6564 5f73 7461   for labeled_sta
-00001ad0: 7274 5f69 6e64 6578 2069 6e20 7365 6c66  rt_index in self
-00001ae0: 2e5f 5f73 7461 7274 5f69 6e64 6963 6573  .__start_indices
-00001af0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
-00001b00: 6265 6c65 645f 696e 7369 6465 5f69 6e64  beled_inside_ind
-00001b10: 6578 203d 206c 6162 656c 6564 5f73 7461  ex = labeled_sta
-00001b20: 7274 5f69 6e64 6578 202b 2031 0a20 2020  rt_index + 1.   
-00001b30: 2020 2020 2020 2020 206c 6162 656c 6564           labeled
-00001b40: 5f65 6e64 5f69 6e64 6578 203d 206c 6162  _end_index = lab
-00001b50: 656c 6564 5f73 7461 7274 5f69 6e64 6578  eled_start_index
-00001b60: 202b 2032 0a20 2020 2020 2020 2020 2020   + 2.           
-00001b70: 206c 6162 656c 6564 5f75 6e69 745f 696e   labeled_unit_in
-00001b80: 6465 7820 3d20 6c61 6265 6c65 645f 7374  dex = labeled_st
-00001b90: 6172 745f 696e 6465 7820 2b20 330a 0a20  art_index + 3.. 
-00001ba0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-00001bb0: 6974 696f 6e73 5b6c 6162 656c 6564 5f73  itions[labeled_s
-00001bc0: 7461 7274 5f69 6e64 6578 5d5b 6c61 6265  tart_index][labe
-00001bd0: 6c65 645f 696e 7369 6465 5f69 6e64 6578  led_inside_index
-00001be0: 5d20 3d20 5472 7565 0a20 2020 2020 2020  ] = True.       
-00001bf0: 2020 2020 2074 7261 6e73 6974 696f 6e73       transitions
-00001c00: 5b6c 6162 656c 6564 5f73 7461 7274 5f69  [labeled_start_i
-00001c10: 6e64 6578 5d5b 6c61 6265 6c65 645f 656e  ndex][labeled_en
-00001c20: 645f 696e 6465 785d 203d 2054 7275 650a  d_index] = True.
-00001c30: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00001c40: 6e73 6974 696f 6e73 5b6c 6162 656c 6564  nsitions[labeled
-00001c50: 5f69 6e73 6964 655f 696e 6465 785d 5b6c  _inside_index][l
-00001c60: 6162 656c 6564 5f69 6e73 6964 655f 696e  abeled_inside_in
-00001c70: 6465 785d 203d 2054 7275 650a 2020 2020  dex] = True.    
-00001c80: 2020 2020 2020 2020 7472 616e 7369 7469          transiti
-00001c90: 6f6e 735b 6c61 6265 6c65 645f 696e 7369  ons[labeled_insi
-00001ca0: 6465 5f69 6e64 6578 5d5b 6c61 6265 6c65  de_index][labele
-00001cb0: 645f 656e 645f 696e 6465 785d 203d 2054  d_end_index] = T
-00001cc0: 7275 650a 0a20 2020 2020 2020 2020 2020  rue..           
-00001cd0: 2074 7261 6e73 6974 696f 6e73 5b6c 6162   transitions[lab
-00001ce0: 656c 6564 5f65 6e64 5f69 6e64 6578 5d5b  eled_end_index][
-00001cf0: 6f75 7473 6964 655f 696e 6465 785d 203d  outside_index] =
-00001d00: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-00001d10: 2020 666f 7220 6920 696e 2073 656c 662e    for i in self.
-00001d20: 5f5f 7374 6172 745f 696e 6469 6365 7320  __start_indices 
-00001d30: 2b20 7365 6c66 2e5f 5f75 6e69 745f 696e  + self.__unit_in
-00001d40: 6469 6365 733a 0a20 2020 2020 2020 2020  dices:.         
-00001d50: 2020 2020 2020 2074 7261 6e73 6974 696f         transitio
-00001d60: 6e73 5b6c 6162 656c 6564 5f65 6e64 5f69  ns[labeled_end_i
-00001d70: 6e64 6578 5d5b 695d 203d 2054 7275 650a  ndex][i] = True.
-00001d80: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00001d90: 6e73 6974 696f 6e73 5b6c 6162 656c 6564  nsitions[labeled
-00001da0: 5f75 6e69 745f 696e 6465 785d 5b6f 7574  _unit_index][out
-00001db0: 7369 6465 5f69 6e64 6578 5d20 3d20 5472  side_index] = Tr
-00001dc0: 7565 0a20 2020 2020 2020 2020 2020 2066  ue.            f
-00001dd0: 6f72 2069 2069 6e20 7365 6c66 2e5f 5f73  or i in self.__s
-00001de0: 7461 7274 5f69 6e64 6963 6573 202b 2073  tart_indices + s
-00001df0: 656c 662e 5f5f 756e 6974 5f69 6e64 6963  elf.__unit_indic
-00001e00: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00001e10: 2020 2020 7472 616e 7369 7469 6f6e 735b      transitions[
-00001e20: 6c61 6265 6c65 645f 756e 6974 5f69 6e64  labeled_unit_ind
-00001e30: 6578 5d5b 695d 203d 2054 7275 650a 0a20  ex][i] = True.. 
-00001e40: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-00001e50: 616e 7369 7469 6f6e 730a                 ansitions.
+00000000: 6672 6f6d 2062 6973 6563 7420 696d 706f  from bisect impo
+00000010: 7274 2062 6973 6563 745f 6c65 6674 0a66  rt bisect_left.f
+00000020: 726f 6d20 636f 6c6c 6563 7469 6f6e 732e  rom collections.
+00000030: 6162 6320 696d 706f 7274 2049 7465 7261  abc import Itera
+00000040: 746f 720a 6672 6f6d 2064 6174 6163 6c61  tor.from datacla
+00000050: 7373 6573 2069 6d70 6f72 7420 6461 7461  sses import data
+00000060: 636c 6173 730a 0a0a 4064 6174 6163 6c61  class...@datacla
+00000070: 7373 2866 726f 7a65 6e3d 5472 7565 2c20  ss(frozen=True, 
+00000080: 6571 3d54 7275 6529 0a63 6c61 7373 2053  eq=True).class S
+00000090: 7061 6e3a 0a20 2020 2073 7461 7274 3a20  pan:.    start: 
+000000a0: 696e 740a 2020 2020 6c65 6e67 7468 3a20  int.    length: 
+000000b0: 696e 740a 0a20 2020 2064 6566 205f 5f68  int..    def __h
+000000c0: 6173 685f 5f28 7365 6c66 2920 2d3e 2069  ash__(self) -> i
+000000d0: 6e74 3a0a 2020 2020 2020 2020 7265 7475  nt:.        retu
+000000e0: 726e 2068 6173 6828 2873 656c 662e 7374  rn hash((self.st
+000000f0: 6172 742c 2073 656c 662e 6c65 6e67 7468  art, self.length
+00000100: 2929 0a0a 0a40 6461 7461 636c 6173 7328  ))...@dataclass(
+00000110: 6672 6f7a 656e 3d54 7275 652c 2065 713d  frozen=True, eq=
+00000120: 5472 7565 290a 636c 6173 7320 5461 673a  True).class Tag:
+00000130: 0a20 2020 2073 7061 6e3a 2053 7061 6e0a  .    span: Span.
+00000140: 2020 2020 6c61 6265 6c3a 2073 7472 0a0a      label: str..
+00000150: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00000160: 2020 6465 6620 7374 6172 7428 7365 6c66    def start(self
+00000170: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+00000180: 2020 7265 7475 726e 2073 656c 662e 7370    return self.sp
+00000190: 616e 2e73 7461 7274 0a0a 2020 2020 4070  an.start..    @p
+000001a0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000001b0: 6c65 6e67 7468 2873 656c 6629 202d 3e20  length(self) -> 
+000001c0: 696e 743a 0a20 2020 2020 2020 2072 6574  int:.        ret
+000001d0: 7572 6e20 7365 6c66 2e73 7061 6e2e 6c65  urn self.span.le
+000001e0: 6e67 7468 0a0a 0a40 6461 7461 636c 6173  ngth...@dataclas
+000001f0: 7328 6672 6f7a 656e 3d54 7275 652c 2065  s(frozen=True, e
+00000200: 713d 5472 7565 290a 636c 6173 7320 4368  q=True).class Ch
+00000210: 6172 4261 7365 6454 6167 733a 0a20 2020  arBasedTags:.   
+00000220: 2074 6167 733a 2074 7570 6c65 5b54 6167   tags: tuple[Tag
+00000230: 2c20 2e2e 2e5d 0a20 2020 2074 6578 743a  , ...].    text:
+00000240: 2073 7472 0a0a 2020 2020 6465 6620 5f5f   str..    def __
+00000250: 6974 6572 5f5f 2873 656c 6629 202d 3e20  iter__(self) -> 
+00000260: 4974 6572 6174 6f72 5b54 6167 5d3a 0a20  Iterator[Tag]:. 
+00000270: 2020 2020 2020 2079 6965 6c64 2066 726f         yield fro
+00000280: 6d20 7365 6c66 2e74 6167 730a 0a20 2020  m self.tags..   
+00000290: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+000002a0: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+000002b0: 2020 2020 7461 675f 7374 7273 203d 205b      tag_strs = [
+000002c0: 5d0a 2020 2020 2020 2020 666f 7220 7461  ].        for ta
+000002d0: 6720 696e 2073 656c 663a 0a20 2020 2020  g in self:.     
+000002e0: 2020 2020 2020 2073 7461 7274 203d 2074         start = t
+000002f0: 6167 2e73 7461 7274 0a20 2020 2020 2020  ag.start.       
+00000300: 2020 2020 2065 6e64 203d 2074 6167 2e73       end = tag.s
+00000310: 7461 7274 202b 2074 6167 2e6c 656e 6774  tart + tag.lengt
+00000320: 680a 2020 2020 2020 2020 2020 2020 7461  h.            ta
+00000330: 675f 7374 7220 3d20 6622 7b73 656c 662e  g_str = f"{self.
+00000340: 7465 7874 5b73 7461 7274 3a65 6e64 5d7d  text[start:end]}
+00000350: 2028 7b74 6167 2e6c 6162 656c 7d29 220a   ({tag.label})".
+00000360: 2020 2020 2020 2020 2020 2020 7461 675f              tag_
+00000370: 7374 7273 2e61 7070 656e 6428 7461 675f  strs.append(tag_
+00000380: 7374 7229 0a20 2020 2020 2020 2072 6574  str).        ret
+00000390: 7572 6e20 6622 287b 272c 2027 2e6a 6f69  urn f"({', '.joi
+000003a0: 6e28 7461 675f 7374 7273 297d 2922 0a0a  n(tag_strs)})"..
+000003b0: 0a63 6c61 7373 2054 6f6b 656e 697a 6564  .class Tokenized
+000003c0: 5465 7874 3a0a 2020 2020 6465 6620 5f5f  Text:.    def __
+000003d0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000003e0: 7365 6c66 2c0a 2020 2020 2020 2020 7465  self,.        te
+000003f0: 7874 3a20 7374 722c 0a20 2020 2020 2020  xt: str,.       
+00000400: 2063 6861 725f 7370 616e 733a 2074 7570   char_spans: tup
+00000410: 6c65 5b53 7061 6e20 7c20 4e6f 6e65 2c20  le[Span | None, 
+00000420: 2e2e 2e5d 2c0a 2020 2020 2020 2020 746f  ...],.        to
+00000430: 6b65 6e5f 696e 6469 6365 733a 2074 7570  ken_indices: tup
+00000440: 6c65 5b69 6e74 2c20 2e2e 2e5d 2c0a 2020  le[int, ...],.  
+00000450: 2020 2020 2020 6164 6474 696f 6e61 6c5f        addtional_
+00000460: 746f 6b65 6e3a 2073 7472 203d 2022 5b54  token: str = "[T
+00000470: 6f6b 656e 5d22 2c0a 2020 2020 293a 0a20  oken]",.    ):. 
+00000480: 2020 2020 2020 2073 656c 662e 5f5f 7465         self.__te
+00000490: 7874 203d 2074 6578 740a 2020 2020 2020  xt = text.      
+000004a0: 2020 7365 6c66 2e5f 5f63 6861 725f 7370    self.__char_sp
+000004b0: 616e 7320 3d20 6368 6172 5f73 7061 6e73  ans = char_spans
+000004c0: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+000004d0: 746f 6b65 6e5f 696e 6469 6365 7320 3d20  token_indices = 
+000004e0: 746f 6b65 6e5f 696e 6469 6365 730a 2020  token_indices.  
+000004f0: 2020 2020 2020 7365 6c66 2e5f 5f61 6464        self.__add
+00000500: 7469 6f6e 616c 5f74 6f6b 656e 203d 2061  tional_token = a
+00000510: 6464 7469 6f6e 616c 5f74 6f6b 656e 0a0a  ddtional_token..
+00000520: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00000530: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+00000540: 2020 2020 2020 2074 6578 7420 3d20 5b5d         text = []
+00000550: 0a20 2020 2020 2020 2066 6f72 2073 7061  .        for spa
+00000560: 6e20 696e 2073 656c 662e 5f5f 6368 6172  n in self.__char
+00000570: 5f73 7061 6e73 3a0a 2020 2020 2020 2020  _spans:.        
+00000580: 2020 2020 6966 2073 7061 6e20 6973 204e      if span is N
+00000590: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000005a0: 2020 2020 2074 6578 742e 6170 7065 6e64       text.append
+000005b0: 2873 656c 662e 5f5f 6164 6474 696f 6e61  (self.__addtiona
+000005c0: 6c5f 746f 6b65 6e29 0a20 2020 2020 2020  l_token).       
+000005d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000005e0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+000005f0: 203d 2073 7061 6e2e 7374 6172 740a 2020   = span.start.  
+00000600: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00000610: 6420 3d20 7374 6172 7420 2b20 7370 616e  d = start + span
+00000620: 2e6c 656e 6774 680a 2020 2020 2020 2020  .length.        
+00000630: 2020 2020 2020 2020 7465 7874 2e61 7070          text.app
+00000640: 656e 6428 7365 6c66 2e5f 5f74 6578 745b  end(self.__text[
+00000650: 7374 6172 743a 656e 645d 290a 2020 2020  start:end]).    
+00000660: 2020 2020 7265 7475 726e 2022 2022 2e6a      return " ".j
+00000670: 6f69 6e28 7465 7874 290a 0a20 2020 2040  oin(text)..    @
+00000680: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00000690: 206e 756d 5f74 6f6b 656e 7328 7365 6c66   num_tokens(self
+000006a0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+000006b0: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
+000006c0: 662e 5f5f 6368 6172 5f73 7061 6e73 290a  f.__char_spans).
+000006d0: 0a20 2020 2064 6566 2067 6574 5f74 6578  .    def get_tex
+000006e0: 7428 7365 6c66 2920 2d3e 2073 7472 3a0a  t(self) -> str:.
+000006f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000700: 656c 662e 5f5f 7465 7874 0a0a 2020 2020  elf.__text..    
+00000710: 6465 6620 6765 745f 746f 6b65 6e28 7365  def get_token(se
+00000720: 6c66 2c20 746f 6b65 6e5f 696e 6465 783a  lf, token_index:
+00000730: 2069 6e74 2920 2d3e 2073 7472 3a0a 2020   int) -> str:.  
+00000740: 2020 2020 2020 6368 6172 5f73 7061 6e20        char_span 
+00000750: 3d20 7365 6c66 2e5f 5f63 6861 725f 7370  = self.__char_sp
+00000760: 616e 735b 746f 6b65 6e5f 696e 6465 785d  ans[token_index]
+00000770: 0a20 2020 2020 2020 2069 6620 6368 6172  .        if char
+00000780: 5f73 7061 6e20 6973 204e 6f6e 653a 0a20  _span is None:. 
+00000790: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000007a0: 6e20 7365 6c66 2e5f 5f61 6464 7469 6f6e  n self.__addtion
+000007b0: 616c 5f74 6f6b 656e 0a20 2020 2020 2020  al_token.       
+000007c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000007d0: 2020 2073 7461 7274 203d 2063 6861 725f     start = char_
+000007e0: 7370 616e 2e73 7461 7274 0a20 2020 2020  span.start.     
+000007f0: 2020 2020 2020 2065 6e64 203d 2073 7461         end = sta
+00000800: 7274 202b 2063 6861 725f 7370 616e 2e6c  rt + char_span.l
+00000810: 656e 6774 680a 2020 2020 2020 2020 2020  ength.          
+00000820: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00000830: 7465 7874 5b73 7461 7274 3a65 6e64 5d0a  text[start:end].
+00000840: 0a20 2020 2064 6566 2067 6574 5f63 6861  .    def get_cha
+00000850: 725f 7370 616e 2873 656c 662c 2074 6f6b  r_span(self, tok
+00000860: 656e 5f69 6e64 6578 3a20 696e 7429 202d  en_index: int) -
+00000870: 3e20 5370 616e 207c 204e 6f6e 653a 0a20  > Span | None:. 
+00000880: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000890: 6c66 2e5f 5f63 6861 725f 7370 616e 735b  lf.__char_spans[
+000008a0: 746f 6b65 6e5f 696e 6465 785d 0a0a 2020  token_index]..  
+000008b0: 2020 6465 6620 636f 6e76 6572 745f 746f    def convert_to
+000008c0: 5f74 6f6b 656e 5f69 6e64 6578 2873 656c  _token_index(sel
+000008d0: 662c 2063 6861 725f 696e 6465 783a 2069  f, char_index: i
+000008e0: 6e74 2920 2d3e 2069 6e74 3a0a 2020 2020  nt) -> int:.    
+000008f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00000900: 5f5f 746f 6b65 6e5f 696e 6469 6365 735b  __token_indices[
+00000910: 6368 6172 5f69 6e64 6578 5d0a 0a20 2020  char_index]..   
+00000920: 2064 6566 2063 6f6e 7665 7274 5f74 6f5f   def convert_to_
+00000930: 6368 6172 5f73 7061 6e28 7365 6c66 2c20  char_span(self, 
+00000940: 746f 6b65 6e5f 7370 616e 3a20 5370 616e  token_span: Span
+00000950: 2920 2d3e 2053 7061 6e20 7c20 4e6f 6e65  ) -> Span | None
+00000960: 3a0a 2020 2020 2020 2020 6368 6172 5f73  :.        char_s
+00000970: 7061 6e5f 7374 6172 7420 3d20 7365 6c66  pan_start = self
+00000980: 2e5f 5f63 6861 725f 7370 616e 735b 746f  .__char_spans[to
+00000990: 6b65 6e5f 7370 616e 2e73 7461 7274 5d0a  ken_span.start].
+000009a0: 2020 2020 2020 2020 6368 6172 5f73 7061          char_spa
+000009b0: 6e5f 656e 6420 3d20 7365 6c66 2e5f 5f63  n_end = self.__c
+000009c0: 6861 725f 7370 616e 735b 746f 6b65 6e5f  har_spans[token_
+000009d0: 7370 616e 2e73 7461 7274 202b 2074 6f6b  span.start + tok
+000009e0: 656e 5f73 7061 6e2e 6c65 6e67 7468 202d  en_span.length -
+000009f0: 2031 5d0a 0a20 2020 2020 2020 2069 6620   1]..        if 
+00000a00: 6368 6172 5f73 7061 6e5f 7374 6172 7420  char_span_start 
+00000a10: 6973 204e 6f6e 6520 6f72 2063 6861 725f  is None or char_
+00000a20: 7370 616e 5f65 6e64 2069 7320 4e6f 6e65  span_end is None
+00000a30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000a40: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
+00000a50: 2020 2072 6574 7572 6e20 5370 616e 280a     return Span(.
+00000a60: 2020 2020 2020 2020 2020 2020 6368 6172              char
+00000a70: 5f73 7061 6e5f 7374 6172 742e 7374 6172  _span_start.star
+00000a80: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
+00000a90: 6861 725f 7370 616e 5f65 6e64 2e73 7461  har_span_end.sta
+00000aa0: 7274 202b 2063 6861 725f 7370 616e 5f65  rt + char_span_e
+00000ab0: 6e64 2e6c 656e 6774 6820 2d20 6368 6172  nd.length - char
+00000ac0: 5f73 7061 6e5f 7374 6172 742e 7374 6172  _span_start.star
+00000ad0: 742c 0a20 2020 2020 2020 2029 0a0a 0a40  t,.        )...@
+00000ae0: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000af0: 3d54 7275 6529 0a63 6c61 7373 2053 7562  =True).class Sub
+00000b00: 776f 7264 4261 7365 6454 6167 733a 0a20  wordBasedTags:. 
+00000b10: 2020 2074 6167 733a 2074 7570 6c65 5b54     tags: tuple[T
+00000b20: 6167 2c20 2e2e 2e5d 0a20 2020 2074 6f6b  ag, ...].    tok
+00000b30: 656e 697a 6564 5f74 6578 743a 2054 6f6b  enized_text: Tok
+00000b40: 656e 697a 6564 5465 7874 0a0a 2020 2020  enizedText..    
+00000b50: 6465 6620 5f5f 6974 6572 5f5f 2873 656c  def __iter__(sel
+00000b60: 6629 202d 3e20 4974 6572 6174 6f72 5b54  f) -> Iterator[T
+00000b70: 6167 5d3a 0a20 2020 2020 2020 2079 6965  ag]:.        yie
+00000b80: 6c64 2066 726f 6d20 7365 6c66 2e74 6167  ld from self.tag
+00000b90: 730a 0a20 2020 2064 6566 205f 5f72 6570  s..    def __rep
+00000ba0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
+00000bb0: 3a0a 2020 2020 2020 2020 7461 675f 7374  :.        tag_st
+00000bc0: 7273 203d 205b 5d0a 2020 2020 2020 2020  rs = [].        
+00000bd0: 666f 7220 7461 6720 696e 2073 656c 663a  for tag in self:
+00000be0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00000bf0: 7274 203d 2074 6167 2e73 7461 7274 0a20  rt = tag.start. 
+00000c00: 2020 2020 2020 2020 2020 2065 6e64 203d             end =
+00000c10: 2073 7461 7274 202b 2074 6167 2e6c 656e   start + tag.len
+00000c20: 6774 680a 2020 2020 2020 2020 2020 2020  gth.            
+00000c30: 7461 675f 7374 7220 3d20 2220 222e 6a6f  tag_str = " ".jo
+00000c40: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+00000c50: 2020 2020 7365 6c66 2e74 6f6b 656e 697a      self.tokeniz
+00000c60: 6564 5f74 6578 742e 6765 745f 746f 6b65  ed_text.get_toke
+00000c70: 6e28 746f 6b65 6e5f 696e 6465 7829 0a20  n(token_index). 
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000c90: 6f72 2074 6f6b 656e 5f69 6e64 6578 2069  or token_index i
+00000ca0: 6e20 7261 6e67 6528 7374 6172 742c 2065  n range(start, e
+00000cb0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+00000cc0: 290a 2020 2020 2020 2020 2020 2020 7461  ).            ta
+00000cd0: 675f 7374 7273 2e61 7070 656e 6428 6622  g_strs.append(f"
+00000ce0: 7b74 6167 5f73 7472 7d20 287b 7461 672e  {tag_str} ({tag.
+00000cf0: 6c61 6265 6c7d 2922 290a 2020 2020 2020  label})").      
+00000d00: 2020 7265 7475 726e 2066 2228 7b27 2c20    return f"({', 
+00000d10: 272e 6a6f 696e 2874 6167 5f73 7472 7329  '.join(tag_strs)
+00000d20: 7d29 220a 0a20 2020 2064 6566 2067 6574  })"..    def get
+00000d30: 5f63 6861 725f 6261 7365 645f 7461 6773  _char_based_tags
+00000d40: 2873 656c 6629 202d 3e20 4368 6172 4261  (self) -> CharBa
+00000d50: 7365 6454 6167 733a 0a20 2020 2020 2020  sedTags:.       
+00000d60: 2074 6167 7320 3d20 5b5d 0a20 2020 2020   tags = [].     
+00000d70: 2020 2066 6f72 2074 6167 2069 6e20 7365     for tag in se
+00000d80: 6c66 2e74 6167 733a 0a20 2020 2020 2020  lf.tags:.       
+00000d90: 2020 2020 2063 6861 725f 7370 616e 203d       char_span =
+00000da0: 2073 656c 662e 746f 6b65 6e69 7a65 645f   self.tokenized_
+00000db0: 7465 7874 2e63 6f6e 7665 7274 5f74 6f5f  text.convert_to_
+00000dc0: 6368 6172 5f73 7061 6e28 7461 672e 7370  char_span(tag.sp
+00000dd0: 616e 290a 2020 2020 2020 2020 2020 2020  an).            
+00000de0: 6966 2063 6861 725f 7370 616e 2069 7320  if char_span is 
+00000df0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00000e00: 2020 2020 2020 2020 2020 7461 6773 2e61            tags.a
+00000e10: 7070 656e 6428 5461 6728 6368 6172 5f73  ppend(Tag(char_s
+00000e20: 7061 6e2c 2074 6167 2e6c 6162 656c 2929  pan, tag.label))
+00000e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000e40: 4368 6172 4261 7365 6454 6167 7328 7475  CharBasedTags(tu
+00000e50: 706c 6528 7461 6773 292c 2073 656c 662e  ple(tags), self.
+00000e60: 746f 6b65 6e69 7a65 645f 7465 7874 2e67  tokenized_text.g
+00000e70: 6574 5f74 6578 7428 2929 0a0a 0a63 6c61  et_text())...cla
+00000e80: 7373 204c 6162 656c 5365 743a 0a20 2020  ss LabelSet:.   
+00000e90: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000ea0: 6c66 2c20 6c61 6265 6c73 3a20 7365 745b  lf, labels: set[
+00000eb0: 7374 725d 293a 0a20 2020 2020 2020 2073  str]):.        s
+00000ec0: 656c 662e 5f5f 6c61 6265 6c73 203d 205b  elf.__labels = [
+00000ed0: 2a73 6f72 7465 6428 6c61 6265 6c73 295d  *sorted(labels)]
+00000ee0: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00000ef0: 7374 6174 7573 5f6b 696e 6420 3d20 3420  status_kind = 4 
+00000f00: 2023 2073 7461 7274 2c20 696e 7369 6465   # start, inside
+00000f10: 2c20 656e 642c 2075 6e69 740a 0a20 2020  , end, unit..   
+00000f20: 2020 2020 2073 656c 662e 5f5f 7374 6172       self.__star
+00000f30: 745f 696e 6469 6365 7320 3d20 5b0a 2020  t_indices = [.  
+00000f40: 2020 2020 2020 2020 2020 2a72 616e 6765            *range
+00000f50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00000f60: 2020 312c 0a20 2020 2020 2020 2020 2020    1,.           
+00000f70: 2020 2020 2073 656c 662e 6765 745f 7461       self.get_ta
+00000f80: 675f 7369 7a65 2829 2c0a 2020 2020 2020  g_size(),.      
+00000f90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00000fa0: 5f73 7461 7475 735f 6b69 6e64 2c0a 2020  _status_kind,.  
+00000fb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00000fc0: 2020 2020 5d0a 2020 2020 2020 2020 7365      ].        se
+00000fd0: 6c66 2e5f 5f75 6e69 745f 696e 6469 6365  lf.__unit_indice
+00000fe0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+00000ff0: 2020 2a72 616e 6765 280a 2020 2020 2020    *range(.      
+00001000: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00001010: 5f73 7461 7475 735f 6b69 6e64 2c0a 2020  _status_kind,.  
+00001020: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001030: 6c66 2e67 6574 5f74 6167 5f73 697a 6528  lf.get_tag_size(
+00001040: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00001050: 2020 2073 656c 662e 5f5f 7374 6174 7573     self.__status
+00001060: 5f6b 696e 642c 0a20 2020 2020 2020 2020  _kind,.         
+00001070: 2020 2029 0a20 2020 2020 2020 205d 0a0a     ).        ]..
+00001080: 2020 2020 2020 2020 7365 6c66 2e5f 5f6c          self.__l
+00001090: 6162 656c 5f69 6473 203d 2064 6963 7428  abel_ids = dict(
+000010a0: 7a69 7028 7365 6c66 2e5f 5f6c 6162 656c  zip(self.__label
+000010b0: 732c 2073 656c 662e 5f5f 7374 6172 745f  s, self.__start_
+000010c0: 696e 6469 6365 732c 2073 7472 6963 743d  indices, strict=
+000010d0: 5472 7565 2929 0a0a 2020 2020 6465 6620  True))..    def 
+000010e0: 6765 745f 6f75 7473 6964 655f 696e 6465  get_outside_inde
+000010f0: 7828 7365 6c66 2920 2d3e 2069 6e74 3a0a  x(self) -> int:.
+00001100: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
+00001110: 0a0a 2020 2020 6465 6620 6765 745f 7374  ..    def get_st
+00001120: 6172 745f 696e 6465 7828 7365 6c66 2c20  art_index(self, 
+00001130: 6c61 6265 6c3a 2073 7472 2920 2d3e 2069  label: str) -> i
+00001140: 6e74 3a0a 2020 2020 2020 2020 6966 206c  nt:.        if l
+00001150: 6162 656c 206e 6f74 2069 6e20 7365 6c66  abel not in self
+00001160: 2e5f 5f6c 6162 656c 5f69 6473 3a0a 2020  .__label_ids:.  
+00001170: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00001180: 5661 6c75 6545 7272 6f72 2822 496e 7661  ValueError("Inva
+00001190: 6c69 6420 6c61 6265 6c20 6973 2067 6976  lid label is giv
+000011a0: 656e 2e22 290a 2020 2020 2020 2020 7265  en.").        re
+000011b0: 7475 726e 2073 656c 662e 5f5f 6c61 6265  turn self.__labe
+000011c0: 6c5f 6964 735b 6c61 6265 6c5d 0a0a 2020  l_ids[label]..  
+000011d0: 2020 6465 6620 6765 745f 696e 7369 6465    def get_inside
+000011e0: 5f69 6e64 6578 2873 656c 662c 206c 6162  _index(self, lab
+000011f0: 656c 3a20 7374 7229 202d 3e20 696e 743a  el: str) -> int:
+00001200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001210: 7365 6c66 2e67 6574 5f73 7461 7274 5f69  self.get_start_i
+00001220: 6e64 6578 286c 6162 656c 2920 2b20 310a  ndex(label) + 1.
+00001230: 0a20 2020 2064 6566 2067 6574 5f65 6e64  .    def get_end
+00001240: 5f69 6e64 6578 2873 656c 662c 206c 6162  _index(self, lab
+00001250: 656c 3a20 7374 7229 202d 3e20 696e 743a  el: str) -> int:
+00001260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001270: 7365 6c66 2e67 6574 5f73 7461 7274 5f69  self.get_start_i
+00001280: 6e64 6578 286c 6162 656c 2920 2b20 320a  ndex(label) + 2.
+00001290: 0a20 2020 2064 6566 2067 6574 5f75 6e69  .    def get_uni
+000012a0: 745f 696e 6465 7828 7365 6c66 2c20 6c61  t_index(self, la
+000012b0: 6265 6c3a 2073 7472 2920 2d3e 2069 6e74  bel: str) -> int
+000012c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000012d0: 2073 656c 662e 6765 745f 7374 6172 745f   self.get_start_
+000012e0: 696e 6465 7828 6c61 6265 6c29 202b 2033  index(label) + 3
+000012f0: 0a0a 2020 2020 6465 6620 6765 745f 6c61  ..    def get_la
+00001300: 6265 6c5f 7369 7a65 2873 656c 6629 202d  bel_size(self) -
+00001310: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
+00001320: 6574 7572 6e20 6c65 6e28 7365 6c66 2e5f  eturn len(self._
+00001330: 5f6c 6162 656c 7329 0a0a 2020 2020 6465  _labels)..    de
+00001340: 6620 6765 745f 7461 675f 7369 7a65 2873  f get_tag_size(s
+00001350: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+00001360: 2020 2020 2023 2028 7374 6172 742c 2069       # (start, i
+00001370: 6e73 6964 652c 2065 6e64 2c20 756e 6974  nside, end, unit
+00001380: 2920 2a20 6c61 6265 6c20 2b20 6f75 7473  ) * label + outs
+00001390: 6964 6520 7374 6174 7573 0a20 2020 2020  ide status.     
+000013a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000013b0: 5f73 7461 7475 735f 6b69 6e64 202a 2073  _status_kind * s
+000013c0: 656c 662e 6765 745f 6c61 6265 6c5f 7369  elf.get_label_si
+000013d0: 7a65 2829 202b 2031 0a0a 2020 2020 6465  ze() + 1..    de
+000013e0: 6620 6765 745f 6c61 6265 6c28 7365 6c66  f get_label(self
+000013f0: 2c20 696e 6465 783a 2069 6e74 2920 2d3e  , index: int) ->
+00001400: 2073 7472 207c 204e 6f6e 653a 0a20 2020   str | None:.   
+00001410: 2020 2020 2069 6620 696e 6465 7820 3c20       if index < 
+00001420: 3020 6f72 2069 6e64 6578 203e 3d20 7365  0 or index >= se
+00001430: 6c66 2e67 6574 5f74 6167 5f73 697a 6528  lf.get_tag_size(
+00001440: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00001450: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00001460: 2249 6e76 616c 6964 2069 6e64 6578 2e22  "Invalid index."
+00001470: 290a 0a20 2020 2020 2020 2069 6620 696e  )..        if in
+00001480: 6465 7820 3d3d 2073 656c 662e 6765 745f  dex == self.get_
+00001490: 6f75 7473 6964 655f 696e 6465 7828 293a  outside_index():
+000014a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000014b0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+000014c0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+000014d0: 6c61 6265 6c73 5b62 6973 6563 745f 6c65  labels[bisect_le
+000014e0: 6674 2873 656c 662e 5f5f 756e 6974 5f69  ft(self.__unit_i
+000014f0: 6e64 6963 6573 2c20 696e 6465 7829 5d0a  ndices, index)].
+00001500: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
+00001510: 7274 5f73 7461 7465 7328 7365 6c66 2920  rt_states(self) 
+00001520: 2d3e 206c 6973 745b 626f 6f6c 5d3a 0a20  -> list[bool]:. 
+00001530: 2020 2020 2020 2073 7461 7465 7320 3d20         states = 
+00001540: 5b46 616c 7365 5d20 2a20 7365 6c66 2e67  [False] * self.g
+00001550: 6574 5f74 6167 5f73 697a 6528 290a 2020  et_tag_size().  
+00001560: 2020 2020 2020 2320 416c 7761 7973 2061        # Always a
+00001570: 6c6c 6f77 6564 2073 7461 7274 7320 6672  llowed starts fr
+00001580: 6f6d 206f 7574 7369 6465 2073 7461 7475  om outside statu
+00001590: 730a 2020 2020 2020 2020 7374 6174 6573  s.        states
+000015a0: 5b73 656c 662e 6765 745f 6f75 7473 6964  [self.get_outsid
+000015b0: 655f 696e 6465 7828 295d 203d 2054 7275  e_index()] = Tru
+000015c0: 650a 0a20 2020 2020 2020 2066 6f72 206c  e..        for l
+000015d0: 6162 656c 6564 5f73 7461 7274 5f69 6e64  abeled_start_ind
+000015e0: 6578 2069 6e20 7365 6c66 2e5f 5f73 7461  ex in self.__sta
+000015f0: 7274 5f69 6e64 6963 6573 3a0a 2020 2020  rt_indices:.    
+00001600: 2020 2020 2020 2020 6c61 6265 6c65 645f          labeled_
+00001610: 756e 6974 5f69 6e64 6578 203d 206c 6162  unit_index = lab
+00001620: 656c 6564 5f73 7461 7274 5f69 6e64 6578  eled_start_index
+00001630: 202b 2033 0a20 2020 2020 2020 2020 2020   + 3.           
+00001640: 2073 7461 7465 735b 6c61 6265 6c65 645f   states[labeled_
+00001650: 7374 6172 745f 696e 6465 785d 203d 2054  start_index] = T
+00001660: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+00001670: 7374 6174 6573 5b6c 6162 656c 6564 5f75  states[labeled_u
+00001680: 6e69 745f 696e 6465 785d 203d 2054 7275  nit_index] = Tru
+00001690: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+000016a0: 2073 7461 7465 730a 0a20 2020 2064 6566   states..    def
+000016b0: 2067 6574 5f65 6e64 5f73 7461 7465 7328   get_end_states(
+000016c0: 7365 6c66 2920 2d3e 206c 6973 745b 626f  self) -> list[bo
+000016d0: 6f6c 5d3a 0a20 2020 2020 2020 2073 7461  ol]:.        sta
+000016e0: 7465 7320 3d20 5b46 616c 7365 5d20 2a20  tes = [False] * 
+000016f0: 7365 6c66 2e67 6574 5f74 6167 5f73 697a  self.get_tag_siz
+00001700: 6528 290a 2020 2020 2020 2020 2320 416c  e().        # Al
+00001710: 7761 7973 2061 6c6c 6f77 6564 2065 6e64  ways allowed end
+00001720: 7320 7769 7468 206f 7574 7369 6465 2073  s with outside s
+00001730: 7461 7475 730a 2020 2020 2020 2020 7374  tatus.        st
+00001740: 6174 6573 5b73 656c 662e 6765 745f 6f75  ates[self.get_ou
+00001750: 7473 6964 655f 696e 6465 7828 295d 203d  tside_index()] =
+00001760: 2054 7275 650a 0a20 2020 2020 2020 2066   True..        f
+00001770: 6f72 206c 6162 656c 6564 5f75 6e69 745f  or labeled_unit_
+00001780: 696e 6465 7820 696e 2073 656c 662e 5f5f  index in self.__
+00001790: 756e 6974 5f69 6e64 6963 6573 3a0a 2020  unit_indices:.  
+000017a0: 2020 2020 2020 2020 2020 6c61 6265 6c65            labele
+000017b0: 645f 656e 645f 696e 6465 7820 3d20 6c61  d_end_index = la
+000017c0: 6265 6c65 645f 756e 6974 5f69 6e64 6578  beled_unit_index
+000017d0: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
+000017e0: 2073 7461 7465 735b 6c61 6265 6c65 645f   states[labeled_
+000017f0: 656e 645f 696e 6465 785d 203d 2054 7275  end_index] = Tru
+00001800: 650a 2020 2020 2020 2020 2020 2020 7374  e.            st
+00001810: 6174 6573 5b6c 6162 656c 6564 5f75 6e69  ates[labeled_uni
+00001820: 745f 696e 6465 785d 203d 2054 7275 650a  t_index] = True.
+00001830: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00001840: 7461 7465 730a 0a20 2020 2064 6566 2067  tates..    def g
+00001850: 6574 5f74 7261 6e73 6974 696f 6e73 2873  et_transitions(s
+00001860: 656c 6629 202d 3e20 6c69 7374 5b6c 6973  elf) -> list[lis
+00001870: 745b 626f 6f6c 5d5d 3a0a 2020 2020 2020  t[bool]]:.      
+00001880: 2020 7472 616e 7369 7469 6f6e 7320 3d20    transitions = 
+00001890: 5b0a 2020 2020 2020 2020 2020 2020 5b46  [.            [F
+000018a0: 616c 7365 5d20 2a20 7365 6c66 2e67 6574  alse] * self.get
+000018b0: 5f74 6167 5f73 697a 6528 2920 666f 7220  _tag_size() for 
+000018c0: 5f20 696e 2072 616e 6765 2873 656c 662e  _ in range(self.
+000018d0: 6765 745f 7461 675f 7369 7a65 2829 290a  get_tag_size()).
+000018e0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000018f0: 2020 6f75 7473 6964 655f 696e 6465 7820    outside_index 
+00001900: 3d20 7365 6c66 2e67 6574 5f6f 7574 7369  = self.get_outsi
+00001910: 6465 5f69 6e64 6578 2829 0a20 2020 2020  de_index().     
+00001920: 2020 2074 7261 6e73 6974 696f 6e73 5b6f     transitions[o
+00001930: 7574 7369 6465 5f69 6e64 6578 5d20 3d20  utside_index] = 
+00001940: 7365 6c66 2e67 6574 5f73 7461 7274 5f73  self.get_start_s
+00001950: 7461 7465 7328 290a 0a20 2020 2020 2020  tates()..       
+00001960: 2066 6f72 206c 6162 656c 6564 5f73 7461   for labeled_sta
+00001970: 7274 5f69 6e64 6578 2069 6e20 7365 6c66  rt_index in self
+00001980: 2e5f 5f73 7461 7274 5f69 6e64 6963 6573  .__start_indices
+00001990: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+000019a0: 6265 6c65 645f 696e 7369 6465 5f69 6e64  beled_inside_ind
+000019b0: 6578 203d 206c 6162 656c 6564 5f73 7461  ex = labeled_sta
+000019c0: 7274 5f69 6e64 6578 202b 2031 0a20 2020  rt_index + 1.   
+000019d0: 2020 2020 2020 2020 206c 6162 656c 6564           labeled
+000019e0: 5f65 6e64 5f69 6e64 6578 203d 206c 6162  _end_index = lab
+000019f0: 656c 6564 5f73 7461 7274 5f69 6e64 6578  eled_start_index
+00001a00: 202b 2032 0a20 2020 2020 2020 2020 2020   + 2.           
+00001a10: 206c 6162 656c 6564 5f75 6e69 745f 696e   labeled_unit_in
+00001a20: 6465 7820 3d20 6c61 6265 6c65 645f 7374  dex = labeled_st
+00001a30: 6172 745f 696e 6465 7820 2b20 330a 0a20  art_index + 3.. 
+00001a40: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+00001a50: 6974 696f 6e73 5b6c 6162 656c 6564 5f73  itions[labeled_s
+00001a60: 7461 7274 5f69 6e64 6578 5d5b 6c61 6265  tart_index][labe
+00001a70: 6c65 645f 696e 7369 6465 5f69 6e64 6578  led_inside_index
+00001a80: 5d20 3d20 5472 7565 0a20 2020 2020 2020  ] = True.       
+00001a90: 2020 2020 2074 7261 6e73 6974 696f 6e73       transitions
+00001aa0: 5b6c 6162 656c 6564 5f73 7461 7274 5f69  [labeled_start_i
+00001ab0: 6e64 6578 5d5b 6c61 6265 6c65 645f 656e  ndex][labeled_en
+00001ac0: 645f 696e 6465 785d 203d 2054 7275 650a  d_index] = True.
+00001ad0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00001ae0: 6e73 6974 696f 6e73 5b6c 6162 656c 6564  nsitions[labeled
+00001af0: 5f69 6e73 6964 655f 696e 6465 785d 5b6c  _inside_index][l
+00001b00: 6162 656c 6564 5f69 6e73 6964 655f 696e  abeled_inside_in
+00001b10: 6465 785d 203d 2054 7275 650a 2020 2020  dex] = True.    
+00001b20: 2020 2020 2020 2020 7472 616e 7369 7469          transiti
+00001b30: 6f6e 735b 6c61 6265 6c65 645f 696e 7369  ons[labeled_insi
+00001b40: 6465 5f69 6e64 6578 5d5b 6c61 6265 6c65  de_index][labele
+00001b50: 645f 656e 645f 696e 6465 785d 203d 2054  d_end_index] = T
+00001b60: 7275 650a 0a20 2020 2020 2020 2020 2020  rue..           
+00001b70: 2074 7261 6e73 6974 696f 6e73 5b6c 6162   transitions[lab
+00001b80: 656c 6564 5f65 6e64 5f69 6e64 6578 5d5b  eled_end_index][
+00001b90: 6f75 7473 6964 655f 696e 6465 785d 203d  outside_index] =
+00001ba0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00001bb0: 2020 666f 7220 6920 696e 2073 656c 662e    for i in self.
+00001bc0: 5f5f 7374 6172 745f 696e 6469 6365 7320  __start_indices 
+00001bd0: 2b20 7365 6c66 2e5f 5f75 6e69 745f 696e  + self.__unit_in
+00001be0: 6469 6365 733a 0a20 2020 2020 2020 2020  dices:.         
+00001bf0: 2020 2020 2020 2074 7261 6e73 6974 696f         transitio
+00001c00: 6e73 5b6c 6162 656c 6564 5f65 6e64 5f69  ns[labeled_end_i
+00001c10: 6e64 6578 5d5b 695d 203d 2054 7275 650a  ndex][i] = True.
+00001c20: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00001c30: 6e73 6974 696f 6e73 5b6c 6162 656c 6564  nsitions[labeled
+00001c40: 5f75 6e69 745f 696e 6465 785d 5b6f 7574  _unit_index][out
+00001c50: 7369 6465 5f69 6e64 6578 5d20 3d20 5472  side_index] = Tr
+00001c60: 7565 0a20 2020 2020 2020 2020 2020 2066  ue.            f
+00001c70: 6f72 2069 2069 6e20 7365 6c66 2e5f 5f73  or i in self.__s
+00001c80: 7461 7274 5f69 6e64 6963 6573 202b 2073  tart_indices + s
+00001c90: 656c 662e 5f5f 756e 6974 5f69 6e64 6963  elf.__unit_indic
+00001ca0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00001cb0: 2020 2020 7472 616e 7369 7469 6f6e 735b      transitions[
+00001cc0: 6c61 6265 6c65 645f 756e 6974 5f69 6e64  labeled_unit_ind
+00001cd0: 6578 5d5b 695d 203d 2054 7275 650a 0a20  ex][i] = True.. 
+00001ce0: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
+00001cf0: 616e 7369 7469 6f6e 730a                 ansitions.
```

### Comparing `pytorch_partial_tagger-0.1.1/.ruff_cache/content/faeb112b154d577f` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/recognizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,77 @@
-00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00000010: 0f00 0000 0000 0000 556e 736f 7274 6564  ........Unsorted
-00000020: 496d 706f 7274 7329 0000 0000 0000 0049  Imports).......I
-00000030: 6d70 6f72 7420 626c 6f63 6b20 6973 2075  mport block is u
-00000040: 6e2d 736f 7274 6564 206f 7220 756e 2d66  n-sorted or un-f
-00000050: 6f72 6d61 7474 6564 0110 0000 0000 0000  ormatted........
-00000060: 004f 7267 616e 697a 6520 696d 706f 7274  .Organize import
-00000070: 7300 0000 00f5 0000 0001 0100 0000 0000  s...............
-00000080: 0000 0000 0000 f500 0000 01f4 0000 0000  ................
-00000090: 0000 0066 726f 6d20 7479 7069 6e67 2069  ...from typing i
-000000a0: 6d70 6f72 7420 6361 7374 0a0a 696d 706f  mport cast..impo
-000000b0: 7274 2074 6f72 6368 0a66 726f 6d20 7061  rt torch.from pa
-000000c0: 7274 6961 6c5f 7461 6767 6572 2e64 6174  rtial_tagger.dat
-000000d0: 612e 6261 7463 6820 696d 706f 7274 2028  a.batch import (
-000000e0: 0a20 2020 2042 6173 6542 6174 6368 4661  .    BaseBatchFa
-000000f0: 6374 6f72 792c 0a20 2020 2042 6174 6368  ctory,.    Batch
-00000100: 2c0a 2020 2020 4368 6172 4261 7365 6454  ,.    CharBasedT
-00000110: 6167 7343 6f6c 6c65 6374 696f 6e2c 0a20  agsCollection,. 
-00000120: 2020 2054 6578 7473 2c0a 290a 6672 6f6d     Texts,.).from
-00000130: 2070 6172 7469 616c 5f74 6167 6765 722e   partial_tagger.
-00000140: 7461 6767 6572 2069 6d70 6f72 7420 5365  tagger import Se
-00000150: 7175 656e 6365 5461 6767 6572 0a66 726f  quenceTagger.fro
-00000160: 6d20 746f 7263 682e 7574 696c 732e 6461  m torch.utils.da
-00000170: 7461 2069 6d70 6f72 7420 4461 7461 4c6f  ta import DataLo
-00000180: 6164 6572 0a0a 0a03 0000 0000 0000 0000  ader............
-00000190: 0000 0000 0000 0001 0000 0000 0000 0051  ...............Q
-000001a0: 0000 0000 0000 002f 5573 6572 732f 7961  ......./Users/ya
-000001b0: 7375 6675 6d69 2f57 6f72 6b73 7061 6365  sufumi/Workspace
-000001c0: 2f70 7974 6f72 6368 2d70 6172 7469 616c  /pytorch-partial
-000001d0: 2d74 6167 6765 722f 7372 632f 7061 7274  -tagger/src/part
-000001e0: 6961 6c5f 7461 6767 6572 2f72 6563 6f67  ial_tagger/recog
-000001f0: 6e69 7a65 722e 7079 fe04 0000 0000 0000  nizer.py........
-00000200: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000210: 7274 2063 6173 740a 0a69 6d70 6f72 7420  rt cast..import 
-00000220: 746f 7263 680a 6672 6f6d 2074 6f72 6368  torch.from torch
-00000230: 2e75 7469 6c73 2e64 6174 6120 696d 706f  .utils.data impo
-00000240: 7274 2044 6174 614c 6f61 6465 720a 0a66  rt DataLoader..f
-00000250: 726f 6d20 7061 7274 6961 6c5f 7461 6767  rom partial_tagg
-00000260: 6572 2e64 6174 612e 6261 7463 6820 696d  er.data.batch im
-00000270: 706f 7274 2028 0a20 2020 2042 6173 6542  port (.    BaseB
-00000280: 6174 6368 4661 6374 6f72 792c 0a20 2020  atchFactory,.   
-00000290: 2042 6174 6368 2c0a 2020 2020 4368 6172   Batch,.    Char
-000002a0: 4261 7365 6454 6167 7343 6f6c 6c65 6374  BasedTagsCollect
-000002b0: 696f 6e2c 0a20 2020 2054 6578 7473 2c0a  ion,.    Texts,.
-000002c0: 290a 6672 6f6d 2070 6172 7469 616c 5f74  ).from partial_t
-000002d0: 6167 6765 722e 7461 6767 6572 2069 6d70  agger.tagger imp
-000002e0: 6f72 7420 5365 7175 656e 6365 5461 6767  ort SequenceTagg
-000002f0: 6572 0a0a 0a63 6c61 7373 2052 6563 6f67  er...class Recog
-00000300: 6e69 7a65 723a 0a20 2020 2064 6566 205f  nizer:.    def _
-00000310: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00000320: 2073 656c 662c 0a20 2020 2020 2020 2074   self,.        t
-00000330: 6167 6765 723a 2053 6571 7565 6e63 6554  agger: SequenceT
-00000340: 6167 6765 722c 0a20 2020 2020 2020 2062  agger,.        b
-00000350: 6174 6368 5f66 6163 746f 7279 3a20 4261  atch_factory: Ba
-00000360: 7365 4261 7463 6846 6163 746f 7279 2c0a  seBatchFactory,.
-00000370: 2020 2020 2020 2020 7061 6464 696e 675f          padding_
-00000380: 696e 6465 783a 2069 6e74 2c0a 2020 2020  index: int,.    
-00000390: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000003a0: 5f5f 7461 6767 6572 203d 2074 6167 6765  __tagger = tagge
-000003b0: 720a 2020 2020 2020 2020 7365 6c66 2e5f  r.        self._
-000003c0: 5f62 6174 6368 5f66 6163 746f 7279 203d  _batch_factory =
-000003d0: 2062 6174 6368 5f66 6163 746f 7279 0a20   batch_factory. 
-000003e0: 2020 2020 2020 2073 656c 662e 5f5f 7061         self.__pa
-000003f0: 6464 696e 675f 696e 6465 7820 3d20 7061  dding_index = pa
-00000400: 6464 696e 675f 696e 6465 780a 0a20 2020  dding_index..   
-00000410: 2064 6566 205f 5f63 616c 6c5f 5f28 0a20   def __call__(. 
-00000420: 2020 2020 2020 2073 656c 662c 2074 6578         self, tex
-00000430: 7473 3a20 5465 7874 732c 2062 6174 6368  ts: Texts, batch
-00000440: 5f73 697a 653a 2069 6e74 2c20 6465 7669  _size: int, devi
-00000450: 6365 3a20 746f 7263 682e 6465 7669 6365  ce: torch.device
-00000460: 0a20 2020 2029 202d 3e20 4368 6172 4261  .    ) -> CharBa
-00000470: 7365 6454 6167 7343 6f6c 6c65 6374 696f  sedTagsCollectio
-00000480: 6e3a 0a20 2020 2020 2020 2064 6174 616c  n:.        datal
-00000490: 6f61 6465 7220 3d20 4461 7461 4c6f 6164  oader = DataLoad
-000004a0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-000004b0: 7465 7874 732c 2020 2320 7479 7065 3a20  texts,  # type: 
-000004c0: 6967 6e6f 7265 0a20 2020 2020 2020 2020  ignore.         
-000004d0: 2020 2063 6f6c 6c61 7465 5f66 6e3d 7365     collate_fn=se
-000004e0: 6c66 2e5f 5f62 6174 6368 5f66 6163 746f  lf.__batch_facto
-000004f0: 7279 2e63 7265 6174 652c 2020 2320 7479  ry.create,  # ty
-00000500: 7065 3a69 676e 6f72 650a 2020 2020 2020  pe:ignore.      
-00000510: 2020 2020 2020 6261 7463 685f 7369 7a65        batch_size
-00000520: 3d62 6174 6368 5f73 697a 652c 0a20 2020  =batch_size,.   
-00000530: 2020 2020 2020 2020 2073 6875 6666 6c65           shuffle
-00000540: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00000550: 290a 0a20 2020 2020 2020 2074 6167 6765  )..        tagge
-00000560: 7220 3d20 7365 6c66 2e5f 5f74 6167 6765  r = self.__tagge
-00000570: 722e 6576 616c 2829 0a0a 2020 2020 2020  r.eval()..      
-00000580: 2020 7072 6564 6963 7469 6f6e 7320 3d20    predictions = 
-00000590: 5b5d 0a20 2020 2020 2020 2066 6f72 2062  [].        for b
-000005a0: 6174 6368 2069 6e20 6461 7461 6c6f 6164  atch in dataload
-000005b0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-000005c0: 6261 7463 6820 3d20 6361 7374 2842 6174  batch = cast(Bat
-000005d0: 6368 2c20 6261 7463 6829 0a0a 2020 2020  ch, batch)..    
-000005e0: 2020 2020 2020 2020 7461 675f 696e 6469          tag_indi
-000005f0: 6365 7320 3d20 7461 6767 6572 2e70 7265  ces = tagger.pre
-00000600: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00000610: 2020 2020 2020 6261 7463 682e 6765 745f        batch.get_
-00000620: 7461 6767 6572 5f69 6e70 7574 7328 6465  tagger_inputs(de
-00000630: 7669 6365 292c 2062 6174 6368 2e67 6574  vice), batch.get
-00000640: 5f6d 6173 6b28 6465 7669 6365 290a 2020  _mask(device).  
-00000650: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00000660: 2020 2020 2020 2020 2070 7265 6469 6374           predict
-00000670: 696f 6e73 2e65 7874 656e 6428 0a20 2020  ions.extend(.   
-00000680: 2020 2020 2020 2020 2020 2020 2062 6174               bat
-00000690: 6368 2e63 7265 6174 655f 6368 6172 5f62  ch.create_char_b
-000006a0: 6173 6564 5f74 6167 7328 7461 675f 696e  ased_tags(tag_in
-000006b0: 6469 6365 732c 2073 656c 662e 5f5f 7061  dices, self.__pa
-000006c0: 6464 696e 675f 696e 6465 7829 0a20 2020  dding_index).   
-000006d0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000006e0: 2020 2020 7265 7475 726e 2074 7570 6c65      return tuple
-000006f0: 2870 7265 6469 6374 696f 6e73 290a       (predictions).
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 2063 6173 740a 0a69 6d70 6f72 7420  rt cast..import 
+00000020: 746f 7263 680a 6672 6f6d 2074 6f72 6368  torch.from torch
+00000030: 2e75 7469 6c73 2e64 6174 6120 696d 706f  .utils.data impo
+00000040: 7274 2044 6174 614c 6f61 6465 720a 0a66  rt DataLoader..f
+00000050: 726f 6d20 2e64 6174 612e 6261 7463 6820  rom .data.batch 
+00000060: 696d 706f 7274 2042 6173 6542 6174 6368  import BaseBatch
+00000070: 4661 6374 6f72 792c 2042 6174 6368 2c20  Factory, Batch, 
+00000080: 4368 6172 4261 7365 6454 6167 7343 6f6c  CharBasedTagsCol
+00000090: 6c65 6374 696f 6e2c 2054 6578 7473 0a66  lection, Texts.f
+000000a0: 726f 6d20 2e74 6167 6765 7220 696d 706f  rom .tagger impo
+000000b0: 7274 2053 6571 7565 6e63 6554 6167 6765  rt SequenceTagge
+000000c0: 720a 0a0a 636c 6173 7320 5265 636f 676e  r...class Recogn
+000000d0: 697a 6572 3a0a 2020 2020 6465 6620 5f5f  izer:.    def __
+000000e0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000000f0: 7365 6c66 2c0a 2020 2020 2020 2020 7461  self,.        ta
+00000100: 6767 6572 3a20 5365 7175 656e 6365 5461  gger: SequenceTa
+00000110: 6767 6572 2c0a 2020 2020 2020 2020 6261  gger,.        ba
+00000120: 7463 685f 6661 6374 6f72 793a 2042 6173  tch_factory: Bas
+00000130: 6542 6174 6368 4661 6374 6f72 792c 0a20  eBatchFactory,. 
+00000140: 2020 2020 2020 2070 6164 6469 6e67 5f69         padding_i
+00000150: 6e64 6578 3a20 696e 742c 0a20 2020 2029  ndex: int,.    )
+00000160: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00000170: 5f74 6167 6765 7220 3d20 7461 6767 6572  _tagger = tagger
+00000180: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00000190: 6261 7463 685f 6661 6374 6f72 7920 3d20  batch_factory = 
+000001a0: 6261 7463 685f 6661 6374 6f72 790a 2020  batch_factory.  
+000001b0: 2020 2020 2020 7365 6c66 2e5f 5f70 6164        self.__pad
+000001c0: 6469 6e67 5f69 6e64 6578 203d 2070 6164  ding_index = pad
+000001d0: 6469 6e67 5f69 6e64 6578 0a0a 2020 2020  ding_index..    
+000001e0: 6465 6620 5f5f 6361 6c6c 5f5f 280a 2020  def __call__(.  
+000001f0: 2020 2020 2020 7365 6c66 2c20 7465 7874        self, text
+00000200: 733a 2054 6578 7473 2c20 6261 7463 685f  s: Texts, batch_
+00000210: 7369 7a65 3a20 696e 742c 2064 6576 6963  size: int, devic
+00000220: 653a 2074 6f72 6368 2e64 6576 6963 650a  e: torch.device.
+00000230: 2020 2020 2920 2d3e 2043 6861 7242 6173      ) -> CharBas
+00000240: 6564 5461 6773 436f 6c6c 6563 7469 6f6e  edTagsCollection
+00000250: 3a0a 2020 2020 2020 2020 6461 7461 6c6f  :.        datalo
+00000260: 6164 6572 203d 2044 6174 614c 6f61 6465  ader = DataLoade
+00000270: 7228 0a20 2020 2020 2020 2020 2020 2074  r(.            t
+00000280: 6578 7473 2c20 2023 2074 7970 653a 2069  exts,  # type: i
+00000290: 676e 6f72 650a 2020 2020 2020 2020 2020  gnore.          
+000002a0: 2020 636f 6c6c 6174 655f 666e 3d73 656c    collate_fn=sel
+000002b0: 662e 5f5f 6261 7463 685f 6661 6374 6f72  f.__batch_factor
+000002c0: 792e 6372 6561 7465 2c20 2023 2074 7970  y.create,  # typ
+000002d0: 653a 6967 6e6f 7265 0a20 2020 2020 2020  e:ignore.       
+000002e0: 2020 2020 2062 6174 6368 5f73 697a 653d       batch_size=
+000002f0: 6261 7463 685f 7369 7a65 2c0a 2020 2020  batch_size,.    
+00000300: 2020 2020 2020 2020 7368 7566 666c 653d          shuffle=
+00000310: 4661 6c73 652c 0a20 2020 2020 2020 2029  False,.        )
+00000320: 0a0a 2020 2020 2020 2020 7461 6767 6572  ..        tagger
+00000330: 203d 2073 656c 662e 5f5f 7461 6767 6572   = self.__tagger
+00000340: 2e65 7661 6c28 290a 0a20 2020 2020 2020  .eval()..       
+00000350: 2070 7265 6469 6374 696f 6e73 203d 205b   predictions = [
+00000360: 5d0a 2020 2020 2020 2020 666f 7220 6261  ].        for ba
+00000370: 7463 6820 696e 2064 6174 616c 6f61 6465  tch in dataloade
+00000380: 723a 0a20 2020 2020 2020 2020 2020 2062  r:.            b
+00000390: 6174 6368 203d 2063 6173 7428 4261 7463  atch = cast(Batc
+000003a0: 682c 2062 6174 6368 290a 0a20 2020 2020  h, batch)..     
+000003b0: 2020 2020 2020 2074 6167 5f69 6e64 6963         tag_indic
+000003c0: 6573 203d 2074 6167 6765 722e 7072 6564  es = tagger.pred
+000003d0: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+000003e0: 2020 2020 2062 6174 6368 2e67 6574 5f74       batch.get_t
+000003f0: 6167 6765 725f 696e 7075 7473 2864 6576  agger_inputs(dev
+00000400: 6963 6529 2c20 6261 7463 682e 6765 745f  ice), batch.get_
+00000410: 6d61 736b 2864 6576 6963 6529 0a20 2020  mask(device).   
+00000420: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00000430: 2020 2020 2020 2020 7072 6564 6963 7469          predicti
+00000440: 6f6e 732e 6578 7465 6e64 280a 2020 2020  ons.extend(.    
+00000450: 2020 2020 2020 2020 2020 2020 6261 7463              batc
+00000460: 682e 6372 6561 7465 5f63 6861 725f 6261  h.create_char_ba
+00000470: 7365 645f 7461 6773 2874 6167 5f69 6e64  sed_tags(tag_ind
+00000480: 6963 6573 2c20 7365 6c66 2e5f 5f70 6164  ices, self.__pad
+00000490: 6469 6e67 5f69 6e64 6578 290a 2020 2020  ding_index).    
+000004a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000004b0: 2020 2072 6574 7572 6e20 7475 706c 6528     return tuple(
+000004c0: 7072 6564 6963 7469 6f6e 7329 0a         predictions).
```

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/embedders.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/embedders.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/tagger.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/training.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/decoders/viterbi.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/src/partial_tagger/encoders/linear.py` & `pytorch_partial_tagger-0.1.2/src/partial_tagger/encoders/linear.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/.gitignore` & `pytorch_partial_tagger-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/LICENSE` & `pytorch_partial_tagger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.1/pyproject.toml` & `pytorch_partial_tagger-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# Referred to
-# https://github.com/tiangolo/fastapi/blob/0.95.2/pyproject.toml
-
 [project]
 name = "pytorch-partial-tagger"
 description = "Sequence Tagger for Partially Annotated Dataset in PyTorch"
 authors = [
     {name = "Yasufumi Taniguchi", email = "yasufumi.taniguchi@gmail.com"},
 ]
 dependencies = [
@@ -41,15 +38,14 @@
 [tool.black]
 line-length = 88
 target-version = ["py310"]
 
 [tool.ruff]
 line-length = 88
 target-version = "py310"
-# https://beta.ruff.rs/docs/rules/
 select = [
   "E",  # pycodestyle errors
   "W",  # pycodestyle warnings
   "F",  # pyflakes
   "I",  # isort
   "C",  # flake8-comprehensions
   "B",  # flake8-bugbear
```

