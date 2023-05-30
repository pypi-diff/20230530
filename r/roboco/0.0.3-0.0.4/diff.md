# Comparing `tmp/roboco-0.0.3.tar.gz` & `tmp/roboco-0.0.4.tar.gz`

## Comparing `roboco-0.0.3.tar` & `roboco-0.0.4.tar`

### file list

```diff
@@ -1,146 +1,155 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 roboco-0.0.3/Dockerfile.example
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 roboco-0.0.3/Dockerfile.pytorch.snippet
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 roboco-0.0.3/TROUBLESHOOTING.md
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 roboco-0.0.3/robot_notes.md
--rwxr-xr-x   0        0        0     6782 2020-02-02 00:00:00.000000 roboco-0.0.3/run.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 roboco-0.0.3/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 roboco-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/10ac7116675be068
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/11dac970d9d29490
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/12a4ae5ba9877db3
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/134820b5f2a573ee
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/157c05ab3ece0a11
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/1964284c5ee28918
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/26edf2930d594dc3
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/2845a52de8470b9d
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/2f5807a633f5b81e
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/338074ba5479eead
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/349538cc06055dfb
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/3644ba7928607a0b
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/36657aa7e3a97f2c
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/36a62fce8458bb4b
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/3aa89a3cf1f4fd2c
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/3f6dac4702b204d8
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/40bffd2ceb95e330
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/43491f137b65d21d
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/46cefab02d6edf15
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/4c3c9a70062d71db
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/518d9b4760433cdc
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/530fbb809a6861d5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/53c95475027057e5
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/545c0bc5448c5eca
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/56e813d9a318018
--rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/582050854505ee31
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/585f3ca6285969b7
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/58e1f565d5753409
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/5b7cd585fd0b0a93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/5baacda8438403d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/603f5a3573c6cc66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/605af05ab1a000ff
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/653e542defa9aeee
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/69bc0a5d26a53f1f
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/6a20f72b0835d9b6
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/6ac3af4d5c1f9bdd
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/6ae7aaa8b214285c
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/6b2a4534ad8c52ff
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/6f53bb332d8fdab3
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/6feda24645941437
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/70b5adb5e7bd521
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/72307ce0427bae49
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/7991d18a2bc2b658
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/79d1d136cc5e038e
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/7a4106e8e18ef937
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/7eaaa343b9aa199a
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/826e032f7ae37401
--rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/846c2437e951ec7d
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/84c53cda7566070b
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/861fccb5205732e3
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/871bbfc438f6eff
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/890abbb627cc88ac
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/89777f3ecc7cf78d
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/8c97ddb266702bdc
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/8df1ca1d7533df23
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/8e37abca3cb4b071
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/98b5c20a6adfe257
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/99a5e62fcb9da3ea
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/a064faed8e120643
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/a25f4c9ccfae7dde
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/ad117982b9e3370f
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/af7a656f77f7719d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/af869ac835256569
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/afb06438bdd28f4b
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b0fb03ffb51824fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b125d935287432e6
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b3bcbfcfda7c321e
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b4766f6368382bde
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b52395c3c74782a2
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b79787da3068774b
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/b7d20649b3300bdf
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/ba19b847a1a94e0d
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/bb1a4e4498e9b8ab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/bc54aeb7666b500d
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/c0e134d6d72fa129
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/c9f54f81b7e34ac6
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/cabe1f69183bad36
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/ccc7213449d99d32
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/cef5b634045d652d
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/cf7b0767148a6756
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/cf893669271a02da
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/d011bc589989879b
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/d320c90d3ec67938
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/d4d3b77b8607825c
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/d5f5e82542c8b4a4
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/d7cfc16d4ed32fcd
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/db1defe56e170052
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/dc233b2e79429be2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/dd76c40a396897ca
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/ddf08ec1c315b512
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/df1aa0dc85d3e406
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/e1adf56cb7a0b8dc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/e1b21fd7f3acc882
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/e3496a654d9b8755
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/e381e52f132f57ee
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/e4341beee9707dc9
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/e95a43dfcbe6d014
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/ebbf12f591c2353e
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/ecd6294df376ee93
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/f2f43a3f0408a250
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/f7574bc2eaf2d77a
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/f7d6ff750e40a8e8
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/fa2d67a5010838f0
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/fc657ff8f13e68ca
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/fd13edf66f7e64aa
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/fdd0c9381df73cfc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.3/.ruff_cache/content/febd26cfb4fcf504
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 roboco-0.0.3/snippets/Dockerfile.pytorch.snippet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roboco-0.0.3/snippets/Dockerfile.realsense.em
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roboco-0.0.3/snippets/Dockerfile.robotiq.em
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 roboco-0.0.3/src/roboco/__init__.py
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 roboco-0.0.3/src/roboco/__main__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 roboco-0.0.3/src/roboco/configurations.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 roboco-0.0.3/src/roboco/template.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/abb_yumi/Dockerfile.melodic
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/abb_yumi/Dockerfile.noetic
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/baxter/Dockerfile.kinetic
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/baxter/Dockerfile.noetic
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/fetch/Dockerfile.noetic
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/jackal/Dockerfile.foxy
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/jackal/Dockerfile.humble
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/jackal/Dockerfile.noetic
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/panda/Dockerfile.noetic
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ridgeback/Dockerfile.noetic
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ros/Dockerfile.foxy
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ros/Dockerfile.galactic
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ros/Dockerfile.humble
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ros/Dockerfile.kinetic
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ros/Dockerfile.melodic
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ros/Dockerfile.noetic
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ur5/Dockerfile.humble
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 roboco-0.0.3/templates/ur5/Dockerfile.noetic
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 roboco-0.0.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 roboco-0.0.3/LICENSE
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 roboco-0.0.3/README.md
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 roboco-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 roboco-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 roboco-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 roboco-0.0.4/Dockerfile.example
+-rwxr-xr-x   0        0        0     6782 2020-02-02 00:00:00.000000 roboco-0.0.4/run.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 roboco-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 roboco-0.0.4/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/10ac7116675be068
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/11dac970d9d29490
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/12a4ae5ba9877db3
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/134820b5f2a573ee
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/157c05ab3ece0a11
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/1964284c5ee28918
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/26edf2930d594dc3
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/2845a52de8470b9d
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/2f5807a633f5b81e
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/338074ba5479eead
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/349538cc06055dfb
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/3644ba7928607a0b
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/36657aa7e3a97f2c
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/36a62fce8458bb4b
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/3714faab6e6f7883
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/37e1a6cea87bbf8e
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/3aa89a3cf1f4fd2c
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/3dcd71be8c392e12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/3f3c8a71e0bba2cc
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/3f6dac4702b204d8
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/40bffd2ceb95e330
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/43491f137b65d21d
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/46cefab02d6edf15
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/4c3c9a70062d71db
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/516335490e2fb8ee
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/518d9b4760433cdc
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/530fbb809a6861d5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/53c95475027057e5
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/545c0bc5448c5eca
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/56e813d9a318018
+-rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/582050854505ee31
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/585f3ca6285969b7
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/58e1f565d5753409
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/5b7cd585fd0b0a93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/5baacda8438403d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/603f5a3573c6cc66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/605af05ab1a000ff
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/653e542defa9aeee
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/69bc0a5d26a53f1f
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/6a20f72b0835d9b6
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/6ac3af4d5c1f9bdd
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/6ae7aaa8b214285c
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/6b2a4534ad8c52ff
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/6f53bb332d8fdab3
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/6feda24645941437
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/70129ae628c98a8a
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/70b5adb5e7bd521
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/72307ce0427bae49
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/7991d18a2bc2b658
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/79d1d136cc5e038e
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/7a4106e8e18ef937
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/7eaaa343b9aa199a
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/826e032f7ae37401
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/846c2437e951ec7d
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/84c53cda7566070b
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/861fccb5205732e3
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/871bbfc438f6eff
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/890abbb627cc88ac
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/89777f3ecc7cf78d
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/8c97ddb266702bdc
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/8df1ca1d7533df23
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/8e37abca3cb4b071
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/97c423c30dcbb142
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/98b5c20a6adfe257
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/99a5e62fcb9da3ea
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/a064faed8e120643
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/a25f4c9ccfae7dde
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ad117982b9e3370f
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ad5eda74ffa82a85
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/af0050a1e4b571e6
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/af7a656f77f7719d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/af869ac835256569
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/afb06438bdd28f4b
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b0fb03ffb51824fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b125d935287432e6
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b1c13b6ed45664a4
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b3bcbfcfda7c321e
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b4766f6368382bde
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b52395c3c74782a2
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b79787da3068774b
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/b7d20649b3300bdf
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ba19b847a1a94e0d
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/bb1a4e4498e9b8ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/bc54aeb7666b500d
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/c0e134d6d72fa129
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/c9f54f81b7e34ac6
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/cabe1f69183bad36
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ccc7213449d99d32
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/cef5b634045d652d
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/cf7b0767148a6756
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/cf893669271a02da
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/d011bc589989879b
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/d320c90d3ec67938
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/d4d3b77b8607825c
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/d5f5e82542c8b4a4
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/d7cfc16d4ed32fcd
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/db1defe56e170052
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/dc233b2e79429be2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/dd76c40a396897ca
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ddf08ec1c315b512
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/df1aa0dc85d3e406
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/e1adf56cb7a0b8dc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/e1b21fd7f3acc882
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/e3496a654d9b8755
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/e381e52f132f57ee
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/e4341beee9707dc9
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/e95a43dfcbe6d014
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ebbf12f591c2353e
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/ecd6294df376ee93
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/f2f43a3f0408a250
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/f7574bc2eaf2d77a
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/f7d6ff750e40a8e8
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/fa2d67a5010838f0
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/fc657ff8f13e68ca
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/fd13edf66f7e64aa
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/fdd0c9381df73cfc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 roboco-0.0.4/.ruff_cache/content/febd26cfb4fcf504
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 roboco-0.0.4/docs/troubleshooting.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 roboco-0.0.4/snippets/Dockerfile.pytorch.snippet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roboco-0.0.4/snippets/Dockerfile.realsense.em
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roboco-0.0.4/snippets/Dockerfile.robotiq.em
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 roboco-0.0.4/src/roboco/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 roboco-0.0.4/src/roboco/__main__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 roboco-0.0.4/src/roboco/configurations.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 roboco-0.0.4/src/roboco/template.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/abb_yumi/Dockerfile.melodic
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/abb_yumi/Dockerfile.noetic
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/baxter/Dockerfile.kinetic
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/baxter/Dockerfile.noetic
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/fetch/Dockerfile.noetic
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/jackal/Dockerfile.foxy
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/jackal/Dockerfile.humble
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/jackal/Dockerfile.noetic
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/panda/Dockerfile.noetic
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ridgeback/Dockerfile.noetic
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ros/Dockerfile.foxy
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ros/Dockerfile.galactic
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ros/Dockerfile.humble
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ros/Dockerfile.kinetic
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ros/Dockerfile.melodic
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ros/Dockerfile.noetic
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ur5/Dockerfile.humble
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 roboco-0.0.4/templates/ur5/Dockerfile.noetic
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 roboco-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 roboco-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 roboco-0.0.4/README.md
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 roboco-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 roboco-0.0.4/PKG-INFO
```

### Comparing `roboco-0.0.3/TROUBLESHOOTING.md` & `roboco-0.0.4/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/run.py` & `roboco-0.0.4/run.py`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.github/workflows/docker-publish.yml` & `roboco-0.0.4/.github/workflows/docker-publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 on:
   workflow_dispatch:
   push:
     branches:
       - 'main'
     tags:
       - 'v*'
+    paths:
+      - '.github/workflows/docker-publish.yml'
+      - 'templates/**'
   pull_request:
     branches:
       - 'main'
+    paths:
+      - '.github/workflows/docker-publish.yml'
+      - 'templates/**'
 
 env:
   REGISTRY: ghcr.io
   IMAGE_NAME: ${{ github.repository }}
 
 jobs:
   build-and-push-image:
```

### Comparing `roboco-0.0.3/.ruff_cache/content/10ac7116675be068` & `roboco-0.0.4/.ruff_cache/content/10ac7116675be068`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/11dac970d9d29490` & `roboco-0.0.4/.ruff_cache/content/11dac970d9d29490`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/157c05ab3ece0a11` & `roboco-0.0.4/.ruff_cache/content/157c05ab3ece0a11`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/1964284c5ee28918` & `roboco-0.0.4/.ruff_cache/content/1964284c5ee28918`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/2f5807a633f5b81e` & `roboco-0.0.4/.ruff_cache/content/2f5807a633f5b81e`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/338074ba5479eead` & `roboco-0.0.4/.ruff_cache/content/338074ba5479eead`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/349538cc06055dfb` & `roboco-0.0.4/.ruff_cache/content/349538cc06055dfb`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/3644ba7928607a0b` & `roboco-0.0.4/.ruff_cache/content/3644ba7928607a0b`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/36657aa7e3a97f2c` & `roboco-0.0.4/.ruff_cache/content/36657aa7e3a97f2c`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/36a62fce8458bb4b` & `roboco-0.0.4/.ruff_cache/content/36a62fce8458bb4b`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/3aa89a3cf1f4fd2c` & `roboco-0.0.4/.ruff_cache/content/3aa89a3cf1f4fd2c`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/40bffd2ceb95e330` & `roboco-0.0.4/.ruff_cache/content/40bffd2ceb95e330`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/46cefab02d6edf15` & `roboco-0.0.4/.ruff_cache/content/46cefab02d6edf15`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/4c3c9a70062d71db` & `roboco-0.0.4/.ruff_cache/content/4c3c9a70062d71db`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/518d9b4760433cdc` & `roboco-0.0.4/.ruff_cache/content/518d9b4760433cdc`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/56e813d9a318018` & `roboco-0.0.4/.ruff_cache/content/56e813d9a318018`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/582050854505ee31` & `roboco-0.0.4/.ruff_cache/content/582050854505ee31`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/58e1f565d5753409` & `roboco-0.0.4/.ruff_cache/content/58e1f565d5753409`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/69bc0a5d26a53f1f` & `roboco-0.0.4/.ruff_cache/content/69bc0a5d26a53f1f`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/6a20f72b0835d9b6` & `roboco-0.0.4/.ruff_cache/content/6a20f72b0835d9b6`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/6ac3af4d5c1f9bdd` & `roboco-0.0.4/.ruff_cache/content/6ac3af4d5c1f9bdd`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/6ae7aaa8b214285c` & `roboco-0.0.4/.ruff_cache/content/6ae7aaa8b214285c`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/6b2a4534ad8c52ff` & `roboco-0.0.4/.ruff_cache/content/6b2a4534ad8c52ff`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/6feda24645941437` & `roboco-0.0.4/.ruff_cache/content/6feda24645941437`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/72307ce0427bae49` & `roboco-0.0.4/.ruff_cache/content/72307ce0427bae49`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/79d1d136cc5e038e` & `roboco-0.0.4/.ruff_cache/content/3714faab6e6f7883`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/7eaaa343b9aa199a` & `roboco-0.0.4/.ruff_cache/content/7eaaa343b9aa199a`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/826e032f7ae37401` & `roboco-0.0.4/.ruff_cache/content/826e032f7ae37401`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/846c2437e951ec7d` & `roboco-0.0.4/.ruff_cache/content/846c2437e951ec7d`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/871bbfc438f6eff` & `roboco-0.0.4/.ruff_cache/content/871bbfc438f6eff`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/89777f3ecc7cf78d` & `roboco-0.0.4/.ruff_cache/content/89777f3ecc7cf78d`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/8c97ddb266702bdc` & `roboco-0.0.4/.ruff_cache/content/8c97ddb266702bdc`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/8e37abca3cb4b071` & `roboco-0.0.4/.ruff_cache/content/8e37abca3cb4b071`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/99a5e62fcb9da3ea` & `roboco-0.0.4/.ruff_cache/content/99a5e62fcb9da3ea`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/ad117982b9e3370f` & `roboco-0.0.4/.ruff_cache/content/ad117982b9e3370f`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/af7a656f77f7719d` & `roboco-0.0.4/.ruff_cache/content/af7a656f77f7719d`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/b79787da3068774b` & `roboco-0.0.4/.ruff_cache/content/b79787da3068774b`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/b7d20649b3300bdf` & `roboco-0.0.4/.ruff_cache/content/b7d20649b3300bdf`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/ba19b847a1a94e0d` & `roboco-0.0.4/.ruff_cache/content/ba19b847a1a94e0d`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/bb1a4e4498e9b8ab` & `roboco-0.0.4/.ruff_cache/content/bb1a4e4498e9b8ab`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/cabe1f69183bad36` & `roboco-0.0.4/.ruff_cache/content/cabe1f69183bad36`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/ccc7213449d99d32` & `roboco-0.0.4/.ruff_cache/content/ccc7213449d99d32`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/cef5b634045d652d` & `roboco-0.0.4/.ruff_cache/content/cef5b634045d652d`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/cf7b0767148a6756` & `roboco-0.0.4/.ruff_cache/content/cf7b0767148a6756`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/d011bc589989879b` & `roboco-0.0.4/.ruff_cache/content/d011bc589989879b`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/d320c90d3ec67938` & `roboco-0.0.4/.ruff_cache/content/d320c90d3ec67938`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/d5f5e82542c8b4a4` & `roboco-0.0.4/.ruff_cache/content/d5f5e82542c8b4a4`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/ddf08ec1c315b512` & `roboco-0.0.4/.ruff_cache/content/ddf08ec1c315b512`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/e1adf56cb7a0b8dc` & `roboco-0.0.4/.ruff_cache/content/e1adf56cb7a0b8dc`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/e3496a654d9b8755` & `roboco-0.0.4/.ruff_cache/content/e3496a654d9b8755`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/e381e52f132f57ee` & `roboco-0.0.4/.ruff_cache/content/e381e52f132f57ee`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/e4341beee9707dc9` & `roboco-0.0.4/.ruff_cache/content/e4341beee9707dc9`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/e95a43dfcbe6d014` & `roboco-0.0.4/.ruff_cache/content/e95a43dfcbe6d014`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/ebbf12f591c2353e` & `roboco-0.0.4/.ruff_cache/content/ebbf12f591c2353e`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/ecd6294df376ee93` & `roboco-0.0.4/.ruff_cache/content/ecd6294df376ee93`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/f7574bc2eaf2d77a` & `roboco-0.0.4/.ruff_cache/content/f7574bc2eaf2d77a`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/fa2d67a5010838f0` & `roboco-0.0.4/.ruff_cache/content/fa2d67a5010838f0`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/fc657ff8f13e68ca` & `roboco-0.0.4/.ruff_cache/content/fc657ff8f13e68ca`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.ruff_cache/content/fd13edf66f7e64aa` & `roboco-0.0.4/.ruff_cache/content/fd13edf66f7e64aa`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/src/roboco/__main__.py` & `roboco-0.0.4/src/roboco/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,37 @@
 blue = "#61afef"
 style = get_style(
     {"input": blue, "questionmark": yellow, "answermark": f"{green} bold"},
     style_override=False,
 )
 tick = "\u2714"
 
-# This template makes heavy use of https://inquirerpy.readthedocs.io/en/latest/
-
 
 def main():
     parser = argparse.ArgumentParser(description="Create a container for your robotics project")
     parser.add_argument("-V", "--version", action="store_true", default=False, help="display version")
+    subparsers = parser.add_subparsers(dest="command")
+    subparsers.add_parser("init", help="generate a Dockerfile and run script for your project")
+    subparsers.add_parser("snippet", help="display snippets to add to your Dockerfile")
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         sys.exit()
 
+    if args.command is None:
+        parser.print_help()
+        sys.exit()
+    elif args.command == "init":
+        init()
+    elif args.command == "snippet":
+        snippet()
+
+
+def init():
     if os.path.exists("run.py") or os.path.exists("Dockerfile"):
         warn_message = "Warning: run.py and/or Dockerfile already exist(s) in this directory."
         color_print([(yellow, warn_message)])
         overwrite_message = "Overwrite these files and continue?"
         overwrite = inquirer.confirm(message=overwrite_message, default=False, style=style, amark=tick).execute()
         if not overwrite:
             print("Operation cancelled.")
@@ -104,9 +115,13 @@
         f"""
         cd {name}
         ./run.py
     """
     )
 
 
+def snippet():
+    color_print([(yellow, "Snippets not implemented yet.")])
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `roboco-0.0.3/src/roboco/configurations.py` & `roboco-0.0.4/src/roboco/configurations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import Literal
+
+from typing_extensions import Literal
 
 ROSDistro = Literal["kinetic", "melodic", "noetic", "foxy", "galactic", "humble"]
 
 
 @dataclass
 class HardwareOption:
     key: str  # a unique identifier for the hardware option
```

### Comparing `roboco-0.0.3/src/roboco/template.py` & `roboco-0.0.4/src/roboco/template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # ruff: noqa: T201
 import os
 import shutil
-from importlib.resources import files
+
+try:
+    # Python < 3.9
+    import importlib_resources as ilr
+except ImportError:
+    # Python >= 3.9
+    import importlib.resources as ilr
 from pathlib import Path
 
 from roboco import __version__
 from roboco.configurations import ProjectConfiguration, realsense_camera, ur5
 
 
 def generate_from_template(configuration: ProjectConfiguration):
     dockerfile_template = f"{configuration.robot.key}/Dockerfile.{configuration.ros_distro}"
     print(f"Generating from {dockerfile_template}")
-    package_dir = files("roboco")
+    package_dir = ilr.files("roboco")
     run_script_dest = "./run.py"
     dockerfile_dest = "./Dockerfile"
     run_script_src = f"{package_dir}/run.py"
     dockerfile_src = f"{package_dir}/templates/{dockerfile_template}"
 
     shutil.copyfile(dockerfile_src, dockerfile_dest)
     shutil.copyfile(run_script_src, run_script_dest)
```

### Comparing `roboco-0.0.3/templates/abb_yumi/Dockerfile.melodic` & `roboco-0.0.4/templates/abb_yumi/Dockerfile.melodic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/baxter/Dockerfile.kinetic` & `roboco-0.0.4/templates/baxter/Dockerfile.kinetic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/baxter/Dockerfile.noetic` & `roboco-0.0.4/templates/baxter/Dockerfile.noetic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/jackal/Dockerfile.foxy` & `roboco-0.0.4/templates/jackal/Dockerfile.foxy`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/jackal/Dockerfile.humble` & `roboco-0.0.4/templates/jackal/Dockerfile.humble`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/panda/Dockerfile.noetic` & `roboco-0.0.4/templates/panda/Dockerfile.noetic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ros/Dockerfile.foxy` & `roboco-0.0.4/templates/ros/Dockerfile.foxy`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ros/Dockerfile.galactic` & `roboco-0.0.4/templates/ros/Dockerfile.galactic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ros/Dockerfile.humble` & `roboco-0.0.4/templates/ros/Dockerfile.humble`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ros/Dockerfile.kinetic` & `roboco-0.0.4/templates/ros/Dockerfile.kinetic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ros/Dockerfile.melodic` & `roboco-0.0.4/templates/ros/Dockerfile.melodic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ros/Dockerfile.noetic` & `roboco-0.0.4/templates/ros/Dockerfile.noetic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/templates/ur5/Dockerfile.noetic` & `roboco-0.0.4/templates/ur5/Dockerfile.noetic`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/.gitignore` & `roboco-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/LICENSE` & `roboco-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `roboco-0.0.3/pyproject.toml` & `roboco-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "inquirerpy~=0.3.4",
+  "typing_extensions~=4.6.2",
+  "importlib-resources==3.0.0;python_version<'3.9'",
 ]
 
 [project.scripts]
 roboco = "roboco.__main__:main"
 
 [project.urls]
 Documentation = "https://github.com/monashrobotics/robot_containers#readme"
```

