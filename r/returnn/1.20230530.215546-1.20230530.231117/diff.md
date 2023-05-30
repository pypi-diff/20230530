# Comparing `tmp/returnn-1.20230530.215546.tar.gz` & `tmp/returnn-1.20230530.231117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230530.215546.tar", last modified: Tue May 30 20:22:11 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230530.231117.tar", last modified: Tue May 30 21:27:13 2023, max compression
```

## Comparing `returnn-1.20230530.215546.tar` & `returnn-1.20230530.231117.tar`

### file list

```diff
@@ -1,445 +1,445 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-30 20:21:56.000000 returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157391 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151459 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   585937 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:22:11.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-30 20:21:53.000000 returnn-1.20230530.215546/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 21:26:56.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-30 21:26:58.000000 returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157552 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151459 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   585937 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551354 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187644 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:27:13.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-30 21:26:55.000000 returnn-1.20230530.231117/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230530.215546/.gitignore` & `returnn-1.20230530.231117/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/.gitmodules` & `returnn-1.20230530.231117/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/CHANGELOG.md` & `returnn-1.20230530.231117/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/CODEOWNERS` & `returnn-1.20230530.231117/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/CONTRIBUTING.md` & `returnn-1.20230530.231117/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/LICENSE` & `returnn-1.20230530.231117/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/MANIFEST.in` & `returnn-1.20230530.231117/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/PKG-INFO` & `returnn-1.20230530.231117/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230530.215546
+Version: 1.20230530.231117
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230530.215546/README.rst` & `returnn-1.20230530.231117/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/__init__.py` & `returnn-1.20230530.231117/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/12AX.cluster_map` & `returnn-1.20230530.231117/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-fwd.config` & `returnn-1.20230530.231117/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-horovod-mpi.py` & `returnn-1.20230530.231117/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230530.231117/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-hyper-param-tuning.config` & `returnn-1.20230530.231117/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-iter-dataset.py` & `returnn-1.20230530.231117/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-list-devices.py` & `returnn-1.20230530.231117/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-lua-torch-layer.config` & `returnn-1.20230530.231117/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230530.231117/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-returnn-as-framework.py` & `returnn-1.20230530.231117/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-rf.config` & `returnn-1.20230530.231117/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-rhn-enwik8.config` & `returnn-1.20230530.231117/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-sprint-interface.py` & `returnn-1.20230530.231117/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-att-copy.config` & `returnn-1.20230530.231117/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-attention.config` & `returnn-1.20230530.231117/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-enc-dec.config` & `returnn-1.20230530.231117/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230530.231117/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230530.231117/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230530.231117/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230530.231117/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230530.231117/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-rec-self-att.config` & `returnn-1.20230530.231117/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230530.231117/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230530.231117/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230530.231117/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-torch.config` & `returnn-1.20230530.231117/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230530.231117/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/demo.sh` & `returnn-1.20230530.231117/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230530.231117/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/README.txt` & `returnn-1.20230530.231117/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/config_demo` & `returnn-1.20230530.231117/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230530.231117/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/config_real` & `returnn-1.20230530.231117/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230530.231117/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/decode.py` & `returnn-1.20230530.231117/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230530.231117/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230530.231117/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230530.231117/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230530.231117/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230530.231117/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230530.231117/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230530.231117/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230530.231117/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/__init__.py` & `returnn-1.20230530.231117/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/__main__.py` & `returnn-1.20230530.231117/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/__old_mod_loader__.py` & `returnn-1.20230530.231117/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/__setup__.py` & `returnn-1.20230530.231117/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/config.py` & `returnn-1.20230530.231117/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/audio.py` & `returnn-1.20230530.231117/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/basic.py` & `returnn-1.20230530.231117/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/bundle_file.py` & `returnn-1.20230530.231117/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/cached.py` & `returnn-1.20230530.231117/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/cached2.py` & `returnn-1.20230530.231117/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/generating.py` & `returnn-1.20230530.231117/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/hdf.py` & `returnn-1.20230530.231117/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/lm.py` & `returnn-1.20230530.231117/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/map.py` & `returnn-1.20230530.231117/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/meta.py` & `returnn-1.20230530.231117/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/multi_proc.py` & `returnn-1.20230530.231117/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/normalization_data.py` & `returnn-1.20230530.231117/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/numpy_dump.py` & `returnn-1.20230530.231117/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/raw_wav.py` & `returnn-1.20230530.231117/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/sprint.py` & `returnn-1.20230530.231117/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/stereo.py` & `returnn-1.20230530.231117/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230530.231117/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/datasets/util/vocabulary.py` & `returnn-1.20230530.231117/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/engine/base.py` & `returnn-1.20230530.231117/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/engine/batch.py` & `returnn-1.20230530.231117/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230530.231117/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/edit.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/select.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/transform.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/extern/graph_editor/util.py` & `returnn-1.20230530.231117/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/__init__.py` & `returnn-1.20230530.231117/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/_backend.py` & `returnn-1.20230530.231117/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/_numpy_backend.py` & `returnn-1.20230530.231117/returnn/frontend/_numpy_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,20 @@
     def executing_eagerly() -> bool:
         """executing eagerly"""
         return True
 
     @staticmethod
     def get_dtype_name_raw(raw_tensor: numpy.ndarray) -> str:
         """
-        :return: dtype of raw tensor, as string
+        :return: dtype of raw tensor, as string. e.g. "int64" etc.
         """
-        return raw_tensor.dtype.name
+        dtype_name = raw_tensor.dtype.name
+        if dtype_name.startswith("str"):
+            return "string"  # ignore the bit-length, it supports variable length
+        return dtype_name
 
     @staticmethod
     def as_dtype_raw(dtype_name: str) -> numpy.dtype:
         """
         :param dtype_name: e.g. "float32"
         :return: dtype object
         """
```

### Comparing `returnn-1.20230530.215546/returnn/frontend/_utils.py` & `returnn-1.20230530.231117/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/array_.py` & `returnn-1.20230530.231117/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/attention.py` & `returnn-1.20230530.231117/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/cond.py` & `returnn-1.20230530.231117/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/const.py` & `returnn-1.20230530.231117/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/container.py` & `returnn-1.20230530.231117/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/conv.py` & `returnn-1.20230530.231117/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/device.py` & `returnn-1.20230530.231117/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/dims.py` & `returnn-1.20230530.231117/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/dropout.py` & `returnn-1.20230530.231117/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/dtype.py` & `returnn-1.20230530.231117/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/encoder/base.py` & `returnn-1.20230530.231117/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/encoder/conformer.py` & `returnn-1.20230530.231117/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/init.py` & `returnn-1.20230530.231117/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/linear.py` & `returnn-1.20230530.231117/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/loop.py` & `returnn-1.20230530.231117/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/loss.py` & `returnn-1.20230530.231117/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/math_.py` & `returnn-1.20230530.231117/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/matmul.py` & `returnn-1.20230530.231117/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/module.py` & `returnn-1.20230530.231117/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/normalization.py` & `returnn-1.20230530.231117/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/parameter.py` & `returnn-1.20230530.231117/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/rand.py` & `returnn-1.20230530.231117/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/rec.py` & `returnn-1.20230530.231117/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/reduce.py` & `returnn-1.20230530.231117/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/run_ctx.py` & `returnn-1.20230530.231117/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/signal.py` & `returnn-1.20230530.231117/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/state.py` & `returnn-1.20230530.231117/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/tensor_array.py` & `returnn-1.20230530.231117/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/frontend/types.py` & `returnn-1.20230530.231117/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/import_/common.py` & `returnn-1.20230530.231117/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/import_/git.py` & `returnn-1.20230530.231117/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/import_/import_.py` & `returnn-1.20230530.231117/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/learning_rate_control.py` & `returnn-1.20230530.231117/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/log.py` & `returnn-1.20230530.231117/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/native_op.cpp` & `returnn-1.20230530.231117/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/native_op.py` & `returnn-1.20230530.231117/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/pretrain.py` & `returnn-1.20230530.231117/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/sprint/cache.py` & `returnn-1.20230530.231117/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/sprint/control.py` & `returnn-1.20230530.231117/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/sprint/error_signals.py` & `returnn-1.20230530.231117/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/sprint/extern_interface.py` & `returnn-1.20230530.231117/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/sprint/interface.py` & `returnn-1.20230530.231117/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/_dim_extra.py` & `returnn-1.20230530.231117/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/_tensor_extra.py` & `returnn-1.20230530.231117/returnn/tensor/_tensor_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,18 @@
                     continue  # we allow anything in the placeholder
                 if raw_shape[i] != self.batch_shape[i]:
                     raise Exception(
                         f"Mismatching shape: Raw tensor {raw_shape} vs Tensor {self};\n"
                         + backend.format_graph_output(self._raw_tensor, max_depth=3)
                     )
             backend.set_known_shape_raw(self._raw_tensor, self.batch_shape)
-            assert backend.get_dtype_name_raw(self._raw_tensor) == self.dtype
+            assert backend.get_dtype_name_raw(self._raw_tensor) == self.dtype, (
+                f"{self} dtype {self.dtype} does not match "
+                f"raw tensor dtype {backend.get_dtype_name_raw(self._raw_tensor)}"
+            )
         if assume_complete:
             for tag in self.dim_tags:
                 if tag.is_batch_dim():
                     continue
                 if tag.is_dynamic():
                     assert tag.dyn_size_ext, "%s sanity_check: dynamic dim %s undefined" % (self, tag)
                     if not ignore_placeholder:
```

### Comparing `returnn-1.20230530.215546/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230530.231117/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230530.231117/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230530.231117/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/dim.py` & `returnn-1.20230530.231117/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/marked_dim.py` & `returnn-1.20230530.231117/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/tensor.py` & `returnn-1.20230530.231117/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/tensor_dict.py` & `returnn-1.20230530.231117/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tensor/utils.py` & `returnn-1.20230530.231117/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/compat.py` & `returnn-1.20230530.231117/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/data_pipeline.py` & `returnn-1.20230530.231117/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/distributed.py` & `returnn-1.20230530.231117/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/engine.py` & `returnn-1.20230530.231117/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230530.231117/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230530.231117/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/horovod.py` & `returnn-1.20230530.231117/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230530.231117/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/layers/base.py` & `returnn-1.20230530.231117/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/layers/basic.py` & `returnn-1.20230530.231117/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/layers/rec.py` & `returnn-1.20230530.231117/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/layers/segmental_model.py` & `returnn-1.20230530.231117/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/layers/signal_processing.py` & `returnn-1.20230530.231117/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/layers/variable.py` & `returnn-1.20230530.231117/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/native_op.py` & `returnn-1.20230530.231117/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/network.py` & `returnn-1.20230530.231117/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/sprint.py` & `returnn-1.20230530.231117/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/updater.py` & `returnn-1.20230530.231117/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/util/basic.py` & `returnn-1.20230530.231117/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/util/data.py` & `returnn-1.20230530.231117/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/util/ken_lm.py` & `returnn-1.20230530.231117/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/tf/util/open_fst.py` & `returnn-1.20230530.231117/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/data/pipeline.py` & `returnn-1.20230530.231117/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230530.231117/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/data/tensor_utils.py` & `returnn-1.20230530.231117/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/engine.py` & `returnn-1.20230530.231117/returnn/torch/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 """
 
 from __future__ import annotations
 from typing import Optional, Union, Callable, Dict
 from contextlib import nullcontext
 
 import os
+import numpy
 import torch
 import torch.utils.data.datapipes as dp
 from torch import autocast
 from torch.cuda import amp
 from torchdata.dataloader2 import DataLoader2
 from random import random
 
 from returnn.config import Config
 from returnn.log import log
 from returnn.engine.base import EngineBase
 import returnn.frontend as rf
-from returnn.tensor import TensorDict, Tensor
+from returnn.tensor import TensorDict, Tensor, Dim
 from returnn.datasets.basic import init_dataset, Dataset
 from returnn.util import basic as util
 from returnn.util import NumbersDict
 from returnn.util.basic import NotSpecified
 from .updater import Updater
 from .data import pipeline as data_pipeline
 from .data import returnn_dataset_wrapper
@@ -114,14 +115,17 @@
         if config.has("eval_datasets"):
             for dataset_name, dataset_opts in config.typed_value("eval_datasets", {}).items():
                 self.eval_datasets[dataset_name] = init_dataset(dataset_opts, default_kwargs={"name": dataset_name})
 
         extern_data = TensorDict()
         extern_data_dict = self.config.typed_value("extern_data")
         extern_data.update(extern_data_dict, auto_convert=True)
+        if "seq_tag" not in extern_data.data:
+            batch_dim = _get_batch_dim_from_extern_data(extern_data)
+            extern_data.data["seq_tag"] = Tensor(name="seq_tag", dtype="string", dims=[batch_dim])
         self.extern_data = extern_data
 
         self._train_dataloader = self._create_data_loader(train_data) if train_data else None
         for dataset_name, dataset in self.eval_datasets.items():
             self._eval_dataloaders[dataset_name] = self._create_data_loader(dataset)
 
         self._start_epoch = self.get_train_start_epoch(self.config)
@@ -494,41 +498,60 @@
     """
     :param extern_data_raw: This comes out of the DataLoader.
     :param extern_data_template: Specified via `extern_data` in the config.
     :param device: E.g. the GPU.
     :return: tensor dict, like extern_data_template, but with raw tensors set to Torch tensors, on the right device.
     """
     assert isinstance(extern_data_raw, dict) and extern_data_raw
-    batch_dim = next(iter(extern_data_template.data.values())).dims[0]
+    batch_dim = _get_batch_dim_from_extern_data(extern_data_template)
     batch_dim.dyn_size_ext = None  # if it is dynamic, reset now, and set it below
     extern_data = TensorDict()
     for k, data in extern_data_template.data.items():
         data = data.copy_template()
-        raw_tensor = extern_data_raw[k].to(device)
-        data.dtype = str(raw_tensor.dtype).split(".")[-1]  # just overwrite for now...
-        data.raw_tensor = raw_tensor
+        raw_tensor = extern_data_raw[k]
+        if isinstance(raw_tensor, torch.Tensor):
+            data.dtype = str(raw_tensor.dtype).split(".")[-1]  # just overwrite for now...
+            data.raw_tensor = raw_tensor.to(device)
+        elif isinstance(raw_tensor, numpy.ndarray):
+            data.raw_tensor = raw_tensor  # leave it as it is
+        else:
+            raise TypeError(f"Unexpected type {type(raw_tensor)} for {k} in extern_data_raw.")
 
         if batch_dim.size is None and batch_dim.dyn_size_ext is None:
             batch_dim.dyn_size_ext = Tensor(batch_dim.name or "batch", dims=[], dtype="int32")
             batch_dim.dyn_size_ext.raw_tensor = torch.tensor(extern_data_raw[k].shape[0], dtype=torch.int32)
 
-        if k + ":seq_len" in extern_data_raw:
+        # This has certain assumptions on the dataset, the data pipeline and collate_batch.
+        # Namely, we expect that we get the batch dim in the first dim (see collate_batch).
+        # We also expect that the sequence lengths are in the second dim, if it is dynamic.
+        if len(data.dims) >= 2 and data.dims[1].dimension is None:
+            assert k + ":seq_len" in extern_data_raw, (
+                f"extern_data {data}, dyn spatial dim, missing {k}:seq_len in raw dict, "
+                f"check dataset or collate_batch"
+            )
             # Sequence lengths have to be on CPU for the later call to rnn.pack_padded_sequence
             size = extern_data_raw[k + ":seq_len"].cpu()
             size_dtype = str(size.dtype).split(".")[-1]
             if data.dims[1].dyn_size_ext is None:
                 data.dims[1].dyn_size_ext = Tensor(data.dims[1].name or "time", dims=[batch_dim], dtype=size_dtype)
             data.dims[1].dyn_size_ext.dtype = size_dtype
             data.dims[1].dyn_size_ext.raw_tensor = size
 
         extern_data.data[k] = data
 
     return extern_data
 
 
+def _get_batch_dim_from_extern_data(extern_data: TensorDict) -> Dim:
+    # We expect that the batch dim is the first dim in any of the tensors.
+    # See collate_batch.
+    batch_dim = next(iter(extern_data.data.values())).dims[0]
+    return batch_dim
+
+
 def _print_process(report_prefix, step, eval_info):
     """
     Similar but simplified from TF engine _print_process.
 
     :param str report_prefix:
     :param int step:
     :param dict[str] eval_info: via :func:`_collect_eval_info`
```

### Comparing `returnn-1.20230530.215546/returnn/torch/frontend/_backend.py` & `returnn-1.20230530.231117/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/frontend/_rand.py` & `returnn-1.20230530.231117/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/frontend/bridge.py` & `returnn-1.20230530.231117/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/torch/updater.py` & `returnn-1.20230530.231117/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/basic.py` & `returnn-1.20230530.231117/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/better_exchook.py` & `returnn-1.20230530.231117/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/bpe.py` & `returnn-1.20230530.231117/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/debug.py` & `returnn-1.20230530.231117/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/debug_helpers.py` & `returnn-1.20230530.231117/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/fsa.py` & `returnn-1.20230530.231117/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230530.231117/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/pprint.py` & `returnn-1.20230530.231117/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/py-to-pickle.cpp` & `returnn-1.20230530.231117/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/sig_proc.py` & `returnn-1.20230530.231117/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn/util/task_system.py` & `returnn-1.20230530.231117/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/returnn.egg-info/PKG-INFO` & `returnn-1.20230530.231117/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230530.215546
+Version: 1.20230530.231117
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230530.215546/returnn.egg-info/SOURCES.txt` & `returnn-1.20230530.231117/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/setup.py` & `returnn-1.20230530.231117/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/DummySprintExec.py` & `returnn-1.20230530.231117/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230530.231117/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230530.231117/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230530.231117/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/_set_num_threads1.py` & `returnn-1.20230530.231117/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/_setup_test_env.py` & `returnn-1.20230530.231117/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/bpe-unicode-demo.codes` & `returnn-1.20230530.231117/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/bpe-unicode-demo.vocab` & `returnn-1.20230530.231117/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/lexicon_opt.isyms` & `returnn-1.20230530.231117/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/lexicon_opt.jpg` & `returnn-1.20230530.231117/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/lint_common.py` & `returnn-1.20230530.231117/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/pycharm-inspect.py` & `returnn-1.20230530.231117/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/pylint.py` & `returnn-1.20230530.231117/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/returnn-as-framework.py` & `returnn-1.20230530.231117/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/rf_utils.py` & `returnn-1.20230530.231117/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/spelling.dic` & `returnn-1.20230530.231117/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_Config.py` & `returnn-1.20230530.231117/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_Dataset.py` & `returnn-1.20230530.231117/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_Fsa.py` & `returnn-1.20230530.231117/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_GeneratingDataset.py` & `returnn-1.20230530.231117/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_HDFDataset.py` & `returnn-1.20230530.231117/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_LearningRateControl.py` & `returnn-1.20230530.231117/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_Log.py` & `returnn-1.20230530.231117/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_MultiProcDataset.py` & `returnn-1.20230530.231117/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_PTDataset.py` & `returnn-1.20230530.231117/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_Pretrain.py` & `returnn-1.20230530.231117/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_ResNet.py` & `returnn-1.20230530.231117/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_SprintDataset.py` & `returnn-1.20230530.231117/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_SprintInterface.py` & `returnn-1.20230530.231117/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFEngine.py` & `returnn-1.20230530.231117/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFNativeOp.py` & `returnn-1.20230530.231117/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFNetworkLayer.py` & `returnn-1.20230530.231117/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230530.231117/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230530.231117/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFUpdater.py` & `returnn-1.20230530.231117/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TFUtil.py` & `returnn-1.20230530.231117/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TF_determinism.py` & `returnn-1.20230530.231117/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TaskSystem.py` & `returnn-1.20230530.231117/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230530.231117/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_TranslationDataset.py` & `returnn-1.20230530.231117/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_Util.py` & `returnn-1.20230530.231117/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_demos.py` & `returnn-1.20230530.231117/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_fork_exec.py` & `returnn-1.20230530.231117/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_hdf_dump.py` & `returnn-1.20230530.231117/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_array.py` & `returnn-1.20230530.231117/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_attention.py` & `returnn-1.20230530.231117/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_base.py` & `returnn-1.20230530.231117/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_cond.py` & `returnn-1.20230530.231117/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_container.py` & `returnn-1.20230530.231117/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_conv.py` & `returnn-1.20230530.231117/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_encoder_conformer.py` & `returnn-1.20230530.231117/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_loop.py` & `returnn-1.20230530.231117/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_math.py` & `returnn-1.20230530.231117/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_normalization.py` & `returnn-1.20230530.231117/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_rec.py` & `returnn-1.20230530.231117/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_reduce.py` & `returnn-1.20230530.231117/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_rf_signal.py` & `returnn-1.20230530.231117/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_tensor.py` & `returnn-1.20230530.231117/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_tools.py` & `returnn-1.20230530.231117/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_torch_frontend.py` & `returnn-1.20230530.231117/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tests/test_torch_internal_frontend.py` & `returnn-1.20230530.231117/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/analyze-dataset-batches.py` & `returnn-1.20230530.231117/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/bliss-collect-seq-lens.py` & `returnn-1.20230530.231117/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/bliss-dump-text.py` & `returnn-1.20230530.231117/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/bliss-get-segment-names.py` & `returnn-1.20230530.231117/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/bliss-to-ogg-zip.py` & `returnn-1.20230530.231117/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/bpe-create-lexicon.py` & `returnn-1.20230530.231117/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/calculate-word-error-rate.py` & `returnn-1.20230530.231117/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/cleanup-old-models.py` & `returnn-1.20230530.231117/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/collect-orth-symbols.py` & `returnn-1.20230530.231117/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/collect-words.py` & `returnn-1.20230530.231117/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/compile_native_op.py` & `returnn-1.20230530.231117/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/compile_tf_graph.py` & `returnn-1.20230530.231117/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/debug-dump-search-scores.py` & `returnn-1.20230530.231117/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/debug-plot-search-scores.py` & `returnn-1.20230530.231117/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/dump-dataset-raw-strings.py` & `returnn-1.20230530.231117/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/dump-dataset.py` & `returnn-1.20230530.231117/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/dump-forward-stats.py` & `returnn-1.20230530.231117/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/dump-forward.py` & `returnn-1.20230530.231117/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/dump-network-json.py` & `returnn-1.20230530.231117/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/dump-pickle.py` & `returnn-1.20230530.231117/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230530.231117/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/get-attention-weights.py` & `returnn-1.20230530.231117/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/get-best-model-epoch.py` & `returnn-1.20230530.231117/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/hdf_dump.py` & `returnn-1.20230530.231117/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230530.231117/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/import-blocks-mt-model.py` & `returnn-1.20230530.231117/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/import-t2t-mt-model.py` & `returnn-1.20230530.231117/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/Makefile` & `returnn-1.20230530.231117/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/README.md` & `returnn-1.20230530.231117/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/example/README.md` & `returnn-1.20230530.231117/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230530.231117/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230530.231117/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230530.231117/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/file.h` & `returnn-1.20230530.231117/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230530.231117/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230530.231117/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/main.cc` & `returnn-1.20230530.231117/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230530.231117/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230530.231117/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230530.231117/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/tf_avg_checkpoints.py` & `returnn-1.20230530.231117/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/tf_inspect_checkpoint.py` & `returnn-1.20230530.231117/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/tf_inspect_summary_log.py` & `returnn-1.20230530.231117/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230530.215546/tools/torch_export_to_onnx.py` & `returnn-1.20230530.231117/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

