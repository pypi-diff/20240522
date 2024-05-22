# Comparing `tmp/returnn-1.20240513.232708.tar.gz` & `tmp/returnn-1.20240522.175941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20240513.232708.tar", last modified: Mon May 13 21:38:21 2024, max compression
+gzip compressed data, was "dist/returnn-1.20240522.175941.tar", last modified: Wed May 22 16:18:46 2024, max compression
```

## Comparing `returnn-1.20240513.232708.tar` & `returnn-1.20240522.175941.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/
--rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      264 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (127)     2396 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3635 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (127)     2331 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1950 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    24864 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-rf-pt-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (127)    11615 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (127)     7287 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (127)    43239 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    43552 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    45111 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (127)    10194 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (127)   248580 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (127)    69536 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2804 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2966 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30829 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27474 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19602 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)    64342 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    25090 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (127)    99033 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (127)    65175 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    85507 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    77105 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (127)    55408 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23915 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 21:38:03.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (127)    51077 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-13 21:38:05.000000 returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19826 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (127)    29792 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (127)    26578 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    18723 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47607 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/frontend/_native/
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/backend.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/backend.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/module.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/module.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/py_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    70068 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/tensor_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_native/tensor_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_random_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (127)    40728 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/frontend/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/audio/mel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/audio/specaugment.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    22353 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/conv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/frontend/decoder/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/decoder/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15776 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)    34623 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   244419 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (127)    23542 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35134 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31142 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    23348 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    36521 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   116423 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)   164824 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)   147333 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46388 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (127)    72976 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/masked_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)    31611 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   152845 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   609993 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)   547403 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    52693 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    79729 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (127)   224930 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    71701 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   302712 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/data/extern_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/data/queued_data_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    56903 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89269 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/frontend/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/frontend/raw_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    26020 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/torch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/util/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/util/diagnose_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/torch/util/scaled_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   138774 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    60303 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (127)    17977 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    18562 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59177 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/multi_proc_non_daemonic_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/native_code_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/py_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/py_ext_mod_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/result_with_reason.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7273 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/task_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/train_proc_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/returnn/util/watch_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      461 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3386 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (127)    34282 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29203 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2960 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13634 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (127)    21403 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)   238450 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)   135447 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (127)   564103 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)   602155 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20306 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)   194602 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15016 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21080 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    26213 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9650 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3943 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      780 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6608 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18501 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5644 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10532 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1791 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10841 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6828 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4379 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    81620 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8500 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47001 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6048 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12596 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5770 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2576 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      719 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16425 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14986 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2936 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3900 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19622 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    49563 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31498 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:38:21.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (127)      800 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     5438 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6269 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1288 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/tf_inspect_summary_log.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4357 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/torch_avg_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/torch_export_to_onnx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8715 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/torch_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3090 2024-05-13 21:38:02.000000 returnn-1.20240513.232708/tools/torch_inspect_checkpoint_and_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      264 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2396 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3635 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2331 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1950 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24864 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-rf-pt-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11615 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7287 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43239 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43552 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45111 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10194 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)   248580 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    69536 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2804 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2966 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30829 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27474 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19602 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64342 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25090 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99033 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65175 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85507 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77105 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55408 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23915 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 16:18:33.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    51077 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-22 16:18:35.000000 returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19826 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29792 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26578 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18723 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47607 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/frontend/_native/
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/backend.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/backend.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/module.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/py_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    70068 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/tensor_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_native/tensor_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_random_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40728 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/frontend/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/audio/mel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/audio/specaugment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22353 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/conv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/frontend/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/decoder/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15776 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34623 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   244419 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23542 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35134 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31142 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23348 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36521 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116423 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164824 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147333 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46388 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72976 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/masked_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31611 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152845 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   609993 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   547403 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52693 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79729 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)   224930 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71701 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   302712 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/data/extern_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/data/queued_data_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56903 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89269 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/frontend/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/frontend/raw_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26020 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/torch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/util/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/util/diagnose_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/torch/util/scaled_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138774 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60303 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17977 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18562 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59177 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/multi_proc_non_daemonic_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/native_code_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/py_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/py_ext_mod_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/result_with_reason.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7273 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/task_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/train_proc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/returnn/util/watch_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      461 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3386 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (127)    34282 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29203 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2960 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13634 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21403 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238450 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135447 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   564103 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   602155 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20306 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194602 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15016 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21080 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26213 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9650 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3943 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      780 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6608 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18501 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5644 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10532 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1791 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10841 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6828 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4379 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    81620 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8500 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47001 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6048 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12596 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5770 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2576 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      719 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16425 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14986 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2936 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3900 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19622 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49563 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31498 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:18:46.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)      800 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5438 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6269 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1288 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/tf_inspect_summary_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4357 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/torch_avg_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/torch_export_to_onnx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8715 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/torch_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3090 2024-05-22 16:18:32.000000 returnn-1.20240522.175941/tools/torch_inspect_checkpoint_and_opt.py
```

### Comparing `returnn-1.20240513.232708/.gitignore` & `returnn-1.20240522.175941/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/.gitmodules` & `returnn-1.20240522.175941/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/CHANGELOG.md` & `returnn-1.20240522.175941/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/CODEOWNERS` & `returnn-1.20240522.175941/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/CONTRIBUTING.md` & `returnn-1.20240522.175941/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/LICENSE` & `returnn-1.20240522.175941/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/MANIFEST.in` & `returnn-1.20240522.175941/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/PKG-INFO` & `returnn-1.20240522.175941/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20240513.232708
+Version: 1.20240522.175941
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20240513.232708/README.rst` & `returnn-1.20240522.175941/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/__init__.py` & `returnn-1.20240522.175941/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/12AX.cluster_map` & `returnn-1.20240522.175941/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-fwd.config` & `returnn-1.20240522.175941/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-horovod-mpi.py` & `returnn-1.20240522.175941/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-horovod-mpi.py.sh` & `returnn-1.20240522.175941/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-hyper-param-tuning.config` & `returnn-1.20240522.175941/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-iter-dataset.py` & `returnn-1.20240522.175941/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-list-devices.py` & `returnn-1.20240522.175941/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-lua-torch-layer.config` & `returnn-1.20240522.175941/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20240522.175941/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-returnn-as-framework.py` & `returnn-1.20240522.175941/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-rf-pt-benchmark.py` & `returnn-1.20240522.175941/demos/demo-rf-pt-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-rf.config` & `returnn-1.20240522.175941/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-rhn-enwik8.config` & `returnn-1.20240522.175941/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-sprint-interface.py` & `returnn-1.20240522.175941/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-att-copy.config` & `returnn-1.20240522.175941/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-attention.config` & `returnn-1.20240522.175941/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-enc-dec.config` & `returnn-1.20240522.175941/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-hard-att-copy.config` & `returnn-1.20240522.175941/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20240522.175941/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20240522.175941/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20240522.175941/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20240522.175941/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-rec-self-att.config` & `returnn-1.20240522.175941/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20240522.175941/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20240522.175941/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-timit-lstm-ctc.config` & `returnn-1.20240522.175941/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-torch.config` & `returnn-1.20240522.175941/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20240522.175941/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/demo.sh` & `returnn-1.20240522.175941/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20240522.175941/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/README.txt` & `returnn-1.20240522.175941/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/config_demo` & `returnn-1.20240522.175941/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/config_fwd` & `returnn-1.20240522.175941/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/config_real` & `returnn-1.20240522.175941/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20240522.175941/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/decode.py` & `returnn-1.20240522.175941/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20240522.175941/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20240522.175941/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20240522.175941/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20240522.175941/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20240522.175941/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20240522.175941/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/artificial/trainconfig` & `returnn-1.20240522.175941/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20240522.175941/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/__init__.py` & `returnn-1.20240522.175941/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/__main__.py` & `returnn-1.20240522.175941/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/__old_mod_loader__.py` & `returnn-1.20240522.175941/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/__setup__.py` & `returnn-1.20240522.175941/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/config.py` & `returnn-1.20240522.175941/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/audio.py` & `returnn-1.20240522.175941/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/basic.py` & `returnn-1.20240522.175941/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/bundle_file.py` & `returnn-1.20240522.175941/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/cached.py` & `returnn-1.20240522.175941/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/cached2.py` & `returnn-1.20240522.175941/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/generating.py` & `returnn-1.20240522.175941/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/hdf.py` & `returnn-1.20240522.175941/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/lm.py` & `returnn-1.20240522.175941/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/map.py` & `returnn-1.20240522.175941/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/meta.py` & `returnn-1.20240522.175941/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/multi_proc.py` & `returnn-1.20240522.175941/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/normalization_data.py` & `returnn-1.20240522.175941/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/numpy_dump.py` & `returnn-1.20240522.175941/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/raw_wav.py` & `returnn-1.20240522.175941/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/sprint.py` & `returnn-1.20240522.175941/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/stereo.py` & `returnn-1.20240522.175941/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/util/feature_extraction.py` & `returnn-1.20240522.175941/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/datasets/util/vocabulary.py` & `returnn-1.20240522.175941/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/engine/base.py` & `returnn-1.20240522.175941/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/engine/batch.py` & `returnn-1.20240522.175941/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/__init__.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/__main__.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20240522.175941/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/__init__.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/edit.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/reroute.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/select.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/transform.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/extern/graph_editor/util.py` & `returnn-1.20240522.175941/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/forward_iface.py` & `returnn-1.20240522.175941/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/__init__.py` & `returnn-1.20240522.175941/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_backend.py` & `returnn-1.20240522.175941/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/__init__.py` & `returnn-1.20240522.175941/returnn/frontend/_native/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/backend.cpp` & `returnn-1.20240522.175941/returnn/frontend/_native/backend.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/backend.hpp` & `returnn-1.20240522.175941/returnn/frontend/_native/backend.hpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/module.cpp` & `returnn-1.20240522.175941/returnn/frontend/_native/module.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/module.hpp` & `returnn-1.20240522.175941/returnn/frontend/_native/module.hpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/py_utils.hpp` & `returnn-1.20240522.175941/returnn/frontend/_native/py_utils.hpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/tensor_ops.cpp` & `returnn-1.20240522.175941/returnn/frontend/_native/tensor_ops.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_native/tensor_ops.hpp` & `returnn-1.20240522.175941/returnn/frontend/_native/tensor_ops.hpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_numpy_backend.py` & `returnn-1.20240522.175941/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_random_journal.py` & `returnn-1.20240522.175941/returnn/frontend/_random_journal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/_utils.py` & `returnn-1.20240522.175941/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/array_.py` & `returnn-1.20240522.175941/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/attention.py` & `returnn-1.20240522.175941/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/audio/mel.py` & `returnn-1.20240522.175941/returnn/frontend/audio/mel.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/audio/specaugment.py` & `returnn-1.20240522.175941/returnn/frontend/audio/specaugment.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/backend.py` & `returnn-1.20240522.175941/returnn/frontend/backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/cond.py` & `returnn-1.20240522.175941/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/const.py` & `returnn-1.20240522.175941/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/container.py` & `returnn-1.20240522.175941/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/control_flow_ctx.py` & `returnn-1.20240522.175941/returnn/frontend/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/conv.py` & `returnn-1.20240522.175941/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/decoder/transformer.py` & `returnn-1.20240522.175941/returnn/frontend/decoder/transformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/device.py` & `returnn-1.20240522.175941/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/dims.py` & `returnn-1.20240522.175941/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/dropout.py` & `returnn-1.20240522.175941/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/dtype.py` & `returnn-1.20240522.175941/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/encoder/base.py` & `returnn-1.20240522.175941/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/encoder/conformer.py` & `returnn-1.20240522.175941/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/gradient.py` & `returnn-1.20240522.175941/returnn/frontend/gradient.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/graph.py` & `returnn-1.20240522.175941/returnn/frontend/graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/hooks.py` & `returnn-1.20240522.175941/returnn/frontend/hooks.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/init.py` & `returnn-1.20240522.175941/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/label_smoothing.py` & `returnn-1.20240522.175941/returnn/frontend/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/linear.py` & `returnn-1.20240522.175941/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/loop.py` & `returnn-1.20240522.175941/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/loss.py` & `returnn-1.20240522.175941/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/math_.py` & `returnn-1.20240522.175941/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/matmul.py` & `returnn-1.20240522.175941/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/module.py` & `returnn-1.20240522.175941/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/normalization.py` & `returnn-1.20240522.175941/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/parameter.py` & `returnn-1.20240522.175941/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/rand.py` & `returnn-1.20240522.175941/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/rec.py` & `returnn-1.20240522.175941/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/reduce.py` & `returnn-1.20240522.175941/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/run_ctx.py` & `returnn-1.20240522.175941/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/signal.py` & `returnn-1.20240522.175941/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/state.py` & `returnn-1.20240522.175941/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/tensor_array.py` & `returnn-1.20240522.175941/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/frontend/types.py` & `returnn-1.20240522.175941/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/import_/common.py` & `returnn-1.20240522.175941/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/import_/git.py` & `returnn-1.20240522.175941/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/import_/import_.py` & `returnn-1.20240522.175941/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/learning_rate_control.py` & `returnn-1.20240522.175941/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/log.py` & `returnn-1.20240522.175941/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/native_op.cpp` & `returnn-1.20240522.175941/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/native_op.py` & `returnn-1.20240522.175941/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/pretrain.py` & `returnn-1.20240522.175941/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/sprint/cache.py` & `returnn-1.20240522.175941/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/sprint/control.py` & `returnn-1.20240522.175941/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/sprint/error_signals.py` & `returnn-1.20240522.175941/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/sprint/extern_interface.py` & `returnn-1.20240522.175941/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/sprint/interface.py` & `returnn-1.20240522.175941/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/_dim_extra.py` & `returnn-1.20240522.175941/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/_tensor_extra.py` & `returnn-1.20240522.175941/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20240522.175941/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20240522.175941/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/control_flow_ctx.py` & `returnn-1.20240522.175941/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/dim.py` & `returnn-1.20240522.175941/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/marked_dim.py` & `returnn-1.20240522.175941/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/tensor.py` & `returnn-1.20240522.175941/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/tensor_dict.py` & `returnn-1.20240522.175941/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tensor/utils.py` & `returnn-1.20240522.175941/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/compat.py` & `returnn-1.20240522.175941/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/data_pipeline.py` & `returnn-1.20240522.175941/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/distributed.py` & `returnn-1.20240522.175941/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/engine.py` & `returnn-1.20240522.175941/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/README.md` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/cond.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/dims.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/layer.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/loop.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/masked_computation.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/masked_computation.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20240522.175941/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20240522.175941/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/horovod.py` & `returnn-1.20240522.175941/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/hyper_param_tuning.py` & `returnn-1.20240522.175941/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/layers/base.py` & `returnn-1.20240522.175941/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/layers/basic.py` & `returnn-1.20240522.175941/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/layers/rec.py` & `returnn-1.20240522.175941/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/layers/segmental_model.py` & `returnn-1.20240522.175941/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/layers/signal_processing.py` & `returnn-1.20240522.175941/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/layers/variable.py` & `returnn-1.20240522.175941/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/native_op.py` & `returnn-1.20240522.175941/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/network.py` & `returnn-1.20240522.175941/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/sprint.py` & `returnn-1.20240522.175941/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/updater.py` & `returnn-1.20240522.175941/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/util/basic.py` & `returnn-1.20240522.175941/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/util/data.py` & `returnn-1.20240522.175941/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20240522.175941/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/util/ken_lm.py` & `returnn-1.20240522.175941/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/tf/util/open_fst.py` & `returnn-1.20240522.175941/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/data/extern_data.py` & `returnn-1.20240522.175941/returnn/torch/data/extern_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/data/pipeline.py` & `returnn-1.20240522.175941/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/data/queued_data_iter.py` & `returnn-1.20240522.175941/returnn/torch/data/queued_data_iter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20240522.175941/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/data/tensor_utils.py` & `returnn-1.20240522.175941/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/distributed.py` & `returnn-1.20240522.175941/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/engine.py` & `returnn-1.20240522.175941/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/frontend/_backend.py` & `returnn-1.20240522.175941/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/frontend/_rand.py` & `returnn-1.20240522.175941/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/frontend/bridge.py` & `returnn-1.20240522.175941/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/updater.py` & `returnn-1.20240522.175941/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/util/diagnose_gpu.py` & `returnn-1.20240522.175941/returnn/torch/util/diagnose_gpu.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/torch/util/scaled_gradient.py` & `returnn-1.20240522.175941/returnn/torch/util/scaled_gradient.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/basic.py` & `returnn-1.20240522.175941/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/better_exchook.py` & `returnn-1.20240522.175941/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/bpe.py` & `returnn-1.20240522.175941/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/debug.py` & `returnn-1.20240522.175941/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/debug_helpers.py` & `returnn-1.20240522.175941/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/fsa.py` & `returnn-1.20240522.175941/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/literal_py_to_pickle.py` & `returnn-1.20240522.175941/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/multi_proc_non_daemonic_spawn.py` & `returnn-1.20240522.175941/returnn/util/multi_proc_non_daemonic_spawn.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/native_code_compiler.py` & `returnn-1.20240522.175941/returnn/util/native_code_compiler.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/pprint.py` & `returnn-1.20240522.175941/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/py-to-pickle.cpp` & `returnn-1.20240522.175941/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/py_ext_mod_compiler.py` & `returnn-1.20240522.175941/returnn/util/py_ext_mod_compiler.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/sig_proc.py` & `returnn-1.20240522.175941/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/task_system.py` & `returnn-1.20240522.175941/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/train_proc_manager.py` & `returnn-1.20240522.175941/returnn/util/train_proc_manager.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn/util/watch_memory.py` & `returnn-1.20240522.175941/returnn/util/watch_memory.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/returnn.egg-info/PKG-INFO` & `returnn-1.20240522.175941/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20240513.232708
+Version: 1.20240522.175941
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20240513.232708/returnn.egg-info/SOURCES.txt` & `returnn-1.20240522.175941/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/setup.py` & `returnn-1.20240522.175941/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/DummySprintExec.py` & `returnn-1.20240522.175941/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/PyCharm-inspection-profile.xml` & `returnn-1.20240522.175941/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20240522.175941/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20240522.175941/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/_set_num_threads1.py` & `returnn-1.20240522.175941/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/_setup_test_env.py` & `returnn-1.20240522.175941/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/bpe-unicode-demo.codes` & `returnn-1.20240522.175941/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/bpe-unicode-demo.vocab` & `returnn-1.20240522.175941/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/lexicon_opt.isyms` & `returnn-1.20240522.175941/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/lexicon_opt.jpg` & `returnn-1.20240522.175941/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/lint_common.py` & `returnn-1.20240522.175941/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/pycharm-inspect.py` & `returnn-1.20240522.175941/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/pylint.py` & `returnn-1.20240522.175941/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/returnn-as-framework.py` & `returnn-1.20240522.175941/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/rf_utils.py` & `returnn-1.20240522.175941/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/spelling.dic` & `returnn-1.20240522.175941/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_Config.py` & `returnn-1.20240522.175941/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_Dataset.py` & `returnn-1.20240522.175941/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_Fsa.py` & `returnn-1.20240522.175941/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_GeneratingDataset.py` & `returnn-1.20240522.175941/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_HDFDataset.py` & `returnn-1.20240522.175941/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_LearningRateControl.py` & `returnn-1.20240522.175941/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_Log.py` & `returnn-1.20240522.175941/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_MultiProcDataset.py` & `returnn-1.20240522.175941/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_Pretrain.py` & `returnn-1.20240522.175941/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_ResNet.py` & `returnn-1.20240522.175941/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_SprintDataset.py` & `returnn-1.20240522.175941/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_SprintInterface.py` & `returnn-1.20240522.175941/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFEngine.py` & `returnn-1.20240522.175941/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFNativeOp.py` & `returnn-1.20240522.175941/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFNetworkLayer.py` & `returnn-1.20240522.175941/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFNetworkRecLayer.py` & `returnn-1.20240522.175941/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20240522.175941/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFUpdater.py` & `returnn-1.20240522.175941/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TFUtil.py` & `returnn-1.20240522.175941/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TF_determinism.py` & `returnn-1.20240522.175941/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TaskSystem.py` & `returnn-1.20240522.175941/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20240522.175941/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_TranslationDataset.py` & `returnn-1.20240522.175941/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_Util.py` & `returnn-1.20240522.175941/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_demos.py` & `returnn-1.20240522.175941/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_fork_exec.py` & `returnn-1.20240522.175941/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_hdf_dump.py` & `returnn-1.20240522.175941/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_array.py` & `returnn-1.20240522.175941/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_attention.py` & `returnn-1.20240522.175941/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_base.py` & `returnn-1.20240522.175941/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_cond.py` & `returnn-1.20240522.175941/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_const.py` & `returnn-1.20240522.175941/tests/test_rf_const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_container.py` & `returnn-1.20240522.175941/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_conv.py` & `returnn-1.20240522.175941/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_encoder_conformer.py` & `returnn-1.20240522.175941/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_gradient.py` & `returnn-1.20240522.175941/tests/test_rf_gradient.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_label_smoothing.py` & `returnn-1.20240522.175941/tests/test_rf_label_smoothing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_loop.py` & `returnn-1.20240522.175941/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_math.py` & `returnn-1.20240522.175941/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_normalization.py` & `returnn-1.20240522.175941/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_rec.py` & `returnn-1.20240522.175941/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_reduce.py` & `returnn-1.20240522.175941/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_rf_signal.py` & `returnn-1.20240522.175941/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_tensor.py` & `returnn-1.20240522.175941/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_tools.py` & `returnn-1.20240522.175941/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_torch_dataset.py` & `returnn-1.20240522.175941/tests/test_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_torch_engine.py` & `returnn-1.20240522.175941/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_torch_frontend.py` & `returnn-1.20240522.175941/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tests/test_torch_internal_frontend.py` & `returnn-1.20240522.175941/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/analyze-dataset-batches.py` & `returnn-1.20240522.175941/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/bliss-collect-seq-lens.py` & `returnn-1.20240522.175941/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/bliss-dump-text.py` & `returnn-1.20240522.175941/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/bliss-get-segment-names.py` & `returnn-1.20240522.175941/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/bliss-to-ogg-zip.py` & `returnn-1.20240522.175941/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/bpe-create-lexicon.py` & `returnn-1.20240522.175941/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/calculate-word-error-rate.py` & `returnn-1.20240522.175941/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/cleanup-old-models.py` & `returnn-1.20240522.175941/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/collect-orth-symbols.py` & `returnn-1.20240522.175941/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/collect-words.py` & `returnn-1.20240522.175941/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/compile_native_op.py` & `returnn-1.20240522.175941/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/compile_tf_graph.py` & `returnn-1.20240522.175941/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/debug-dump-search-scores.py` & `returnn-1.20240522.175941/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/debug-plot-search-scores.py` & `returnn-1.20240522.175941/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/dump-dataset-raw-strings.py` & `returnn-1.20240522.175941/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/dump-dataset.py` & `returnn-1.20240522.175941/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/dump-forward-stats.py` & `returnn-1.20240522.175941/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/dump-forward.py` & `returnn-1.20240522.175941/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/dump-network-json.py` & `returnn-1.20240522.175941/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/dump-pickle.py` & `returnn-1.20240522.175941/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/extract_state_tying_from_dataset.py` & `returnn-1.20240522.175941/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/get-attention-weights.py` & `returnn-1.20240522.175941/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/get-best-model-epoch.py` & `returnn-1.20240522.175941/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/hdf_dump.py` & `returnn-1.20240522.175941/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/hdf_dump_translation_dataset.py` & `returnn-1.20240522.175941/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/import-blocks-mt-model.py` & `returnn-1.20240522.175941/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/import-t2t-mt-model.py` & `returnn-1.20240522.175941/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/Makefile` & `returnn-1.20240522.175941/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/README.md` & `returnn-1.20240522.175941/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/example/README.md` & `returnn-1.20240522.175941/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20240522.175941/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20240522.175941/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20240522.175941/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/file.h` & `returnn-1.20240522.175941/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20240522.175941/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20240522.175941/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/main.cc` & `returnn-1.20240522.175941/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/rescorer.h` & `returnn-1.20240522.175941/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20240522.175941/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20240522.175941/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/tf_avg_checkpoints.py` & `returnn-1.20240522.175941/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/tf_inspect_checkpoint.py` & `returnn-1.20240522.175941/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/tf_inspect_summary_log.py` & `returnn-1.20240522.175941/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/torch_avg_checkpoints.py` & `returnn-1.20240522.175941/tools/torch_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/torch_export_to_onnx.py` & `returnn-1.20240522.175941/tools/torch_export_to_onnx.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 - Input with sequence length are provided, output with sequence lengths:
     The input and output time dimensions are as usual, having `dyn_size_ext` of shape [B].
 """
 
 from __future__ import annotations
 import torch
-from typing import Callable, Optional, Dict
+from typing import Callable, Optional, Dict, List
 import argparse
 import os
 from random import random
 
 import _setup_returnn_env  # noqa
 from returnn.config import Config
 from returnn.log import log
@@ -153,15 +153,15 @@
     )
     assert all(v is not None for k, v in outputs_raw.items()), (
         f"Output raw keys from forward_step contain None values.\n"
         f"Output raw keys with None: {list(k for k, v in outputs_raw.items() if v is None)}"
     )
 
 
-def _get_model_outputs_raw_keys():
+def _get_model_outputs_raw_keys() -> List[str]:
     model_outputs = rf.get_run_ctx().expected_outputs
     model_outputs_raw_keys = []
     for k, v in model_outputs.data.items():
         model_outputs_raw_keys.append(k)
         for i, dim in enumerate(v.dims):
             if dim.dyn_size_ext and dim.dyn_size_ext.dims:
                 model_outputs_raw_keys.append(f"{k}:size{i}")
@@ -178,14 +178,16 @@
         type=str,
         help="Filename to config file. Must have `get_model()` and `forward_step()`. Can optionally have `export()`.",
     )
     parser.add_argument("checkpoint", type=str, help="Checkpoint to RF module, considering the backend.")
     parser.add_argument("out_onnx_filename", type=str, help="Filename of the final ONNX model.")
     parser.add_argument("--verbosity", default=4, type=int, help="5 for all seqs (default: 4)")
     parser.add_argument("--device", type=str, default="cpu", help="'cpu' (default) or 'gpu'.")
+    parser.add_argument("--input_names", type=str, help="Comma-separated list of input names.")
+    parser.add_argument("--output_names", type=str, help="Comma-separated list of output names.")
     args = parser.parse_args()
 
     init(config_filename=args.config, checkpoint=args.checkpoint, log_verbosity=args.verbosity, device=args.device)
 
     model_outputs_dict = config.typed_value("model_outputs")
     assert (
         model_outputs_dict is not None
@@ -246,24 +248,39 @@
             if dim.dyn_size_ext and dim.dyn_size_ext.dims == ():
                 continue
             if dim.dyn_size_ext:
                 dynamic_axes[f"{k}:size{i}"] = {
                     j: dim_.name for j, dim_ in enumerate(dim.dyn_size_ext.dims) if dim_.is_dynamic()
                 }
 
-    print("*** Input names:", list(extern_data_raw.keys()))
-    print("*** Output names:", model_outputs_raw_keys)
+    if args.input_names:
+        input_names = args.input_names.split(",")
+        assert set(extern_data_raw.keys()) == set(
+            input_names
+        ), f"missmatch between input_names {input_names} and extern_data keys {list(extern_data_raw.keys())}"
+    else:
+        input_names = list(extern_data_raw.keys())
+    if args.output_names:
+        output_names = args.output_names.split(",")
+        assert set(model_outputs_raw_keys) == set(
+            output_names
+        ), f"missmatch between output_names {output_names} and model_outputs keys {model_outputs_raw_keys}"
+    else:
+        output_names = model_outputs_raw_keys
+
+    print("*** Input names:", input_names)
+    print("*** Output names:", output_names)
     print("*** Dynamic axes:", dynamic_axes)
 
     export_func(
         pt_model_fwd,
         (extern_data_raw, {}),
         f=args.out_onnx_filename,
         verbose=True,
-        input_names=list(extern_data_raw.keys()),
-        output_names=model_outputs_raw_keys,
+        input_names=input_names,
+        output_names=output_names,
         dynamic_axes=dynamic_axes,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `returnn-1.20240513.232708/tools/torch_inspect_checkpoint.py` & `returnn-1.20240522.175941/tools/torch_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20240513.232708/tools/torch_inspect_checkpoint_and_opt.py` & `returnn-1.20240522.175941/tools/torch_inspect_checkpoint_and_opt.py`

 * *Files identical despite different names*

