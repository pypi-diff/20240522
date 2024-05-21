# Comparing `tmp/graspologic-3.3.1.dev14.tar.gz` & `tmp/graspologic-3.3.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graspologic-3.3.1.dev14.tar", max compression
+gzip compressed data, was "graspologic-3.3.1.dev9.tar", max compression
```

## Comparing `graspologic-3.3.1.dev14.tar` & `graspologic-3.3.1.dev9.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0     1074 2024-05-21 20:42:56.472530 graspologic-3.3.1.dev14/LICENSE.txt
--rw-r--r--   0        0        0     4172 2024-05-21 20:42:56.472530 graspologic-3.3.1.dev14/README.md
--rw-r--r--   0        0        0      605 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/__init__.py
--rw-r--r--   0        0        0      304 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/align/__init__.py
--rw-r--r--   0        0        0     4615 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/align/base.py
--rw-r--r--   0        0        0     4197 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/align/orthogonal_procrustes.py
--rw-r--r--   0        0        0    17718 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/align/seedless_procrustes.py
--rw-r--r--   0        0        0     3733 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/align/sign_flips.py
--rw-r--r--   0        0        0      328 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/cluster/__init__.py
--rw-r--r--   0        0        0    30149 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/cluster/autogmm.py
--rw-r--r--   0        0        0     2576 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/cluster/base.py
--rw-r--r--   0        0        0    16926 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/cluster/divisive_cluster.py
--rw-r--r--   0        0        0    11062 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/cluster/gclust.py
--rw-r--r--   0        0        0     4178 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/cluster/kclust.py
--rw-r--r--   0        0        0      238 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/__init__.py
--rw-r--r--   0        0        0     6898 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/base.py
--rw-r--r--   0        0        0    87769 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/drosophila/left_adjacency.csv
--rw-r--r--   0        0        0      418 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/drosophila/left_cell_labels.csv
--rw-r--r--   0        0        0    91164 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/drosophila/right_adjacency.csv
--rw-r--r--   0        0        0      426 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/drosophila/right_cell_labels.csv
--rw-r--r--   0        0        0    19847 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/mice/atlas.csv
--rw-r--r--   0        0        0      297 2024-05-21 20:42:56.488530 graspologic-3.3.1.dev14/graspologic/datasets/mice/blocks.csv
--rw-r--r--   0        0        0   465335 2024-05-21 20:42:56.492531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
--rw-r--r--   0        0        0   417268 2024-05-21 20:42:56.492531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
--rw-r--r--   0        0        0   481030 2024-05-21 20:42:56.496531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
--rw-r--r--   0        0        0   513067 2024-05-21 20:42:56.500531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
--rw-r--r--   0        0        0   486685 2024-05-21 20:42:56.500531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
--rw-r--r--   0        0        0   502512 2024-05-21 20:42:56.504531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
--rw-r--r--   0        0        0   501644 2024-05-21 20:42:56.504531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
--rw-r--r--   0        0        0   490182 2024-05-21 20:42:56.508531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
--rw-r--r--   0        0        0   423952 2024-05-21 20:42:56.508531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
--rw-r--r--   0        0        0   410522 2024-05-21 20:42:56.508531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
--rw-r--r--   0        0        0   418663 2024-05-21 20:42:56.512531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
--rw-r--r--   0        0        0   426113 2024-05-21 20:42:56.512531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
--rw-r--r--   0        0        0   459110 2024-05-21 20:42:56.516531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
--rw-r--r--   0        0        0   456778 2024-05-21 20:42:56.516531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
--rw-r--r--   0        0        0   500977 2024-05-21 20:42:56.520531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
--rw-r--r--   0        0        0   429240 2024-05-21 20:42:56.520531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
--rw-r--r--   0        0        0   412281 2024-05-21 20:42:56.524531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
--rw-r--r--   0        0        0   486497 2024-05-21 20:42:56.524531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
--rw-r--r--   0        0        0   466098 2024-05-21 20:42:56.528531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
--rw-r--r--   0        0        0   469626 2024-05-21 20:42:56.528531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
--rw-r--r--   0        0        0   431457 2024-05-21 20:42:56.532531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
--rw-r--r--   0        0        0   408031 2024-05-21 20:42:56.532531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
--rw-r--r--   0        0        0   450727 2024-05-21 20:42:56.532531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
--rw-r--r--   0        0        0   343162 2024-05-21 20:42:56.536531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
--rw-r--r--   0        0        0   451278 2024-05-21 20:42:56.536531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
--rw-r--r--   0        0        0   496115 2024-05-21 20:42:56.540531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
--rw-r--r--   0        0        0   493788 2024-05-21 20:42:56.540531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
--rw-r--r--   0        0        0   481678 2024-05-21 20:42:56.544531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
--rw-r--r--   0        0        0   479782 2024-05-21 20:42:56.544531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
--rw-r--r--   0        0        0   416610 2024-05-21 20:42:56.548531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
--rw-r--r--   0        0        0   363031 2024-05-21 20:42:56.548531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
--rw-r--r--   0        0        0   474339 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
--rwxr-xr-x   0        0        0    33536 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54776.csv
--rwxr-xr-x   0        0        0    33530 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54777.csv
--rwxr-xr-x   0        0        0    33537 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54779.csv
--rwxr-xr-x   0        0        0    33535 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54781.csv
--rwxr-xr-x   0        0        0    33544 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54790.csv
--rwxr-xr-x   0        0        0    33551 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54793.csv
--rwxr-xr-x   0        0        0    33549 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54794.csv
--rwxr-xr-x   0        0        0    33555 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54797.csv
--rwxr-xr-x   0        0        0    33519 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54811.csv
--rwxr-xr-x   0        0        0    33525 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54813.csv
--rwxr-xr-x   0        0        0    33530 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54815.csv
--rwxr-xr-x   0        0        0    33528 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54817.csv
--rwxr-xr-x   0        0        0    33501 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54821.csv
--rwxr-xr-x   0        0        0    33510 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54823.csv
--rwxr-xr-x   0        0        0    33536 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54829.csv
--rwxr-xr-x   0        0        0    33538 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54831.csv
--rwxr-xr-x   0        0        0    33530 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54833.csv
--rwxr-xr-x   0        0        0    33535 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54835.csv
--rwxr-xr-x   0        0        0    33505 2024-05-21 20:42:56.552531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54842.csv
--rwxr-xr-x   0        0        0    33508 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54847.csv
--rwxr-xr-x   0        0        0    33520 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54849.csv
--rwxr-xr-x   0        0        0    33520 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54851.csv
--rwxr-xr-x   0        0        0    33525 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54853.csv
--rwxr-xr-x   0        0        0    33527 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54855.csv
--rwxr-xr-x   0        0        0    33551 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54864.csv
--rwxr-xr-x   0        0        0    33551 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54866.csv
--rwxr-xr-x   0        0        0    33551 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54868.csv
--rwxr-xr-x   0        0        0    33552 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54870.csv
--rwxr-xr-x   0        0        0    33508 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54883.csv
--rwxr-xr-x   0        0        0    33514 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54885.csv
--rwxr-xr-x   0        0        0    33509 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54887.csv
--rwxr-xr-x   0        0        0    33496 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54890.csv
--rw-r--r--   0        0        0      684 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/datasets/mice/participants.csv
--rw-r--r--   0        0        0      699 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/__init__.py
--rw-r--r--   0        0        0     6965 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/ase.py
--rw-r--r--   0        0        0    17726 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/base.py
--rw-r--r--   0        0        0     8276 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/case.py
--rw-r--r--   0        0        0     7502 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/lse.py
--rw-r--r--   0        0        0    10447 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/mase.py
--rw-r--r--   0        0        0     8317 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/mds.py
--rw-r--r--   0        0        0     6972 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/mug2vec.py
--rw-r--r--   0        0        0    19443 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/n2v.py
--rw-r--r--   0        0        0    11479 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/omni.py
--rw-r--r--   0        0        0    11834 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/embed/svd.py
--rw-r--r--   0        0        0      429 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/__init__.py
--rw-r--r--   0        0        0     2880 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/binomial.py
--rw-r--r--   0        0        0     4564 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/density_test.py
--rw-r--r--   0        0        0    20564 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/group_connection_test.py
--rw-r--r--   0        0        0    20135 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/latent_distribution_test.py
--rw-r--r--   0        0        0     9837 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/latent_position_test.py
--rw-r--r--   0        0        0     2392 2024-05-21 20:42:56.556531 graspologic-3.3.1.dev14/graspologic/inference/utils.py
--rw-r--r--   0        0        0      428 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/__init__.py
--rw-r--r--   0        0        0    10697 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/__main__.py
--rw-r--r--   0        0        0    16074 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/auto.py
--rw-r--r--   0        0        0      345 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/classes.py
--rw-r--r--   0        0        0     6154 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/colors.py
--rw-r--r--   0        0        0    28486 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/include/colors-100.json
--rw-r--r--   0        0        0      174 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/__init__.py
--rw-r--r--   0        0        0     7029 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_grid.py
--rw-r--r--   0        0        0      860 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_node.py
--rw-r--r--   0        0        0    42453 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_quad_node.py
--rw-r--r--   0        0        0     2171 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_quad_tree.py
--rw-r--r--   0        0        0      964 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/nooverlap.py
--rw-r--r--   0        0        0    10077 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/layouts/render.py
--rw-r--r--   0        0        0      152 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/match/__init__.py
--rw-r--r--   0        0        0    26991 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/match/solver.py
--rw-r--r--   0        0        0      840 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/match/types.py
--rw-r--r--   0        0        0    14080 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/match/wrappers.py
--rw-r--r--   0        0        0      459 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/models/__init__.py
--rw-r--r--   0        0        0     7322 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/models/base.py
--rw-r--r--   0        0        0     7136 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/models/edge_swaps.py
--rw-r--r--   0        0        0     5488 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/models/er.py
--rw-r--r--   0        0        0     5906 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/models/rdpg.py
--rw-r--r--   0        0        0    19673 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/models/sbm_estimators.py
--rw-r--r--   0        0        0    16934 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/nominate/VNviaSGM.py
--rw-r--r--   0        0        0      234 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/nominate/__init__.py
--rw-r--r--   0        0        0    10972 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/nominate/spectralVN.py
--rw-r--r--   0        0        0      419 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/partition/__init__.py
--rw-r--r--   0        0        0    25165 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/partition/leiden.py
--rw-r--r--   0        0        0     5311 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/partition/modularity.py
--rw-r--r--   0        0        0     1091 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/__init__.py
--rw-r--r--   0        0        0      744 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/_elbow.py
--rw-r--r--   0        0        0       91 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/_types.py
--rw-r--r--   0        0        0     9212 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/adjacency_spectral_embedding.py
--rw-r--r--   0        0        0     4269 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/embeddings.py
--rw-r--r--   0        0        0     9918 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/laplacian_spectral_embedding.py
--rw-r--r--   0        0        0    12796 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/embed/omnibus_embedding.py
--rw-r--r--   0        0        0     4045 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/pipeline/graph_builder.py
--rw-r--r--   0        0        0      528 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/plot/__init__.py
--rw-r--r--   0        0        0    64195 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/plot/plot.py
--rw-r--r--   0        0        0    34806 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/plot/plot_matrix.py
--rw-r--r--   0        0        0     3456 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/preconditions.py
--rw-r--r--   0        0        0      604 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/preprocessing/__init__.py
--rw-r--r--   0        0        0    16315 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/preprocessing/graph_cuts.py
--rw-r--r--   0        0        0        0 2024-05-21 20:42:56.560531 graspologic-3.3.1.dev14/graspologic/py.typed
--rw-r--r--   0        0        0      482 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/simulations/__init__.py
--rw-r--r--   0        0        0     4904 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/simulations/rdpg_corr.py
--rw-r--r--   0        0        0    38533 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/simulations/simulations.py
--rw-r--r--   0        0        0    10269 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/simulations/simulations_corr.py
--rw-r--r--   0        0        0      153 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/subgraph/__init__.py
--rw-r--r--   0        0        0     8470 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/subgraph/sg.py
--rw-r--r--   0        0        0     1781 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/types.py
--rw-r--r--   0        0        0     1195 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/utils/__init__.py
--rw-r--r--   0        0        0     4201 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/utils/ptr.py
--rw-r--r--   0        0        0    40441 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/utils/utils.py
--rw-r--r--   0        0        0     1765 2024-05-21 20:42:56.564531 graspologic-3.3.1.dev14/graspologic/version.py
--rw-r--r--   0        0        0     4313 2024-05-21 20:43:42.388763 graspologic-3.3.1.dev14/pyproject.toml
--rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 graspologic-3.3.1.dev14/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-20 21:38:52.989539 graspologic-3.3.1.dev9/LICENSE.txt
+-rw-r--r--   0        0        0     4124 2024-05-20 21:38:52.989539 graspologic-3.3.1.dev9/README.md
+-rw-r--r--   0        0        0      605 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/__init__.py
+-rw-r--r--   0        0        0     4615 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/base.py
+-rw-r--r--   0        0        0     4197 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/orthogonal_procrustes.py
+-rw-r--r--   0        0        0    17718 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/seedless_procrustes.py
+-rw-r--r--   0        0        0     3733 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/sign_flips.py
+-rw-r--r--   0        0        0      328 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/cluster/__init__.py
+-rw-r--r--   0        0        0    30149 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/autogmm.py
+-rw-r--r--   0        0        0     2576 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/base.py
+-rw-r--r--   0        0        0    16926 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/divisive_cluster.py
+-rw-r--r--   0        0        0    11062 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/gclust.py
+-rw-r--r--   0        0        0     4178 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/kclust.py
+-rw-r--r--   0        0        0      238 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/__init__.py
+-rw-r--r--   0        0        0     6898 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/base.py
+-rw-r--r--   0        0        0    87769 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/left_adjacency.csv
+-rw-r--r--   0        0        0      418 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/left_cell_labels.csv
+-rw-r--r--   0        0        0    91164 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/right_adjacency.csv
+-rw-r--r--   0        0        0      426 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/right_cell_labels.csv
+-rw-r--r--   0        0        0    19847 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/mice/atlas.csv
+-rw-r--r--   0        0        0      297 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/mice/blocks.csv
+-rw-r--r--   0        0        0   465335 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   417268 2024-05-20 21:38:53.013539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   481030 2024-05-20 21:38:53.013539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   513067 2024-05-20 21:38:53.017539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   486685 2024-05-20 21:38:53.017539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   502512 2024-05-20 21:38:53.021539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   501644 2024-05-20 21:38:53.021539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   490182 2024-05-20 21:38:53.025539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   423952 2024-05-20 21:38:53.025539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   410522 2024-05-20 21:38:53.029539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   418663 2024-05-20 21:38:53.029539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   426113 2024-05-20 21:38:53.033539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   459110 2024-05-20 21:38:53.033539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   456778 2024-05-20 21:38:53.037539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   500977 2024-05-20 21:38:53.037539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   429240 2024-05-20 21:38:53.037539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   412281 2024-05-20 21:38:53.041539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   486497 2024-05-20 21:38:53.041539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   466098 2024-05-20 21:38:53.045539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   469626 2024-05-20 21:38:53.045539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   431457 2024-05-20 21:38:53.049539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   408031 2024-05-20 21:38:53.049539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   450727 2024-05-20 21:38:53.053540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   343162 2024-05-20 21:38:53.053540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   451278 2024-05-20 21:38:53.053540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   496115 2024-05-20 21:38:53.057540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   493788 2024-05-20 21:38:53.057540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   481678 2024-05-20 21:38:53.061540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   479782 2024-05-20 21:38:53.061540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   416610 2024-05-20 21:38:53.065540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   363031 2024-05-20 21:38:53.065540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   474339 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
+-rwxr-xr-x   0        0        0    33536 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54776.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54777.csv
+-rwxr-xr-x   0        0        0    33537 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54779.csv
+-rwxr-xr-x   0        0        0    33535 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54781.csv
+-rwxr-xr-x   0        0        0    33544 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54790.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54793.csv
+-rwxr-xr-x   0        0        0    33549 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54794.csv
+-rwxr-xr-x   0        0        0    33555 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54797.csv
+-rwxr-xr-x   0        0        0    33519 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54811.csv
+-rwxr-xr-x   0        0        0    33525 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54813.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54815.csv
+-rwxr-xr-x   0        0        0    33528 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54817.csv
+-rwxr-xr-x   0        0        0    33501 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54821.csv
+-rwxr-xr-x   0        0        0    33510 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54823.csv
+-rwxr-xr-x   0        0        0    33536 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54829.csv
+-rwxr-xr-x   0        0        0    33538 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54831.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54833.csv
+-rwxr-xr-x   0        0        0    33535 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54835.csv
+-rwxr-xr-x   0        0        0    33505 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54842.csv
+-rwxr-xr-x   0        0        0    33508 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54847.csv
+-rwxr-xr-x   0        0        0    33520 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54849.csv
+-rwxr-xr-x   0        0        0    33520 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54851.csv
+-rwxr-xr-x   0        0        0    33525 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54853.csv
+-rwxr-xr-x   0        0        0    33527 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54855.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54864.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54866.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54868.csv
+-rwxr-xr-x   0        0        0    33552 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54870.csv
+-rwxr-xr-x   0        0        0    33508 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54883.csv
+-rwxr-xr-x   0        0        0    33514 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54885.csv
+-rwxr-xr-x   0        0        0    33509 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54887.csv
+-rwxr-xr-x   0        0        0    33496 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54890.csv
+-rw-r--r--   0        0        0      684 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/participants.csv
+-rw-r--r--   0        0        0      699 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/__init__.py
+-rw-r--r--   0        0        0     6965 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/ase.py
+-rw-r--r--   0        0        0    17726 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/base.py
+-rw-r--r--   0        0        0     8276 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/case.py
+-rw-r--r--   0        0        0     7502 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/lse.py
+-rw-r--r--   0        0        0    10447 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/mase.py
+-rw-r--r--   0        0        0     8317 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/mds.py
+-rw-r--r--   0        0        0     6972 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/mug2vec.py
+-rw-r--r--   0        0        0    19443 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/n2v.py
+-rw-r--r--   0        0        0    11479 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/embed/omni.py
+-rw-r--r--   0        0        0    11834 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/embed/svd.py
+-rw-r--r--   0        0        0      429 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/binomial.py
+-rw-r--r--   0        0        0     4564 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/density_test.py
+-rw-r--r--   0        0        0    20564 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/group_connection_test.py
+-rw-r--r--   0        0        0    20135 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/latent_distribution_test.py
+-rw-r--r--   0        0        0     9837 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/latent_position_test.py
+-rw-r--r--   0        0        0     2392 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/utils.py
+-rw-r--r--   0        0        0      428 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/__init__.py
+-rw-r--r--   0        0        0    10697 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/__main__.py
+-rw-r--r--   0        0        0    16074 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/auto.py
+-rw-r--r--   0        0        0      345 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/classes.py
+-rw-r--r--   0        0        0     6154 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/colors.py
+-rw-r--r--   0        0        0    28486 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/include/colors-100.json
+-rw-r--r--   0        0        0      174 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/__init__.py
+-rw-r--r--   0        0        0     7029 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_grid.py
+-rw-r--r--   0        0        0      860 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_node.py
+-rw-r--r--   0        0        0    42453 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_node.py
+-rw-r--r--   0        0        0     2171 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_tree.py
+-rw-r--r--   0        0        0      964 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/nooverlap.py
+-rw-r--r--   0        0        0    10077 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/render.py
+-rw-r--r--   0        0        0      152 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/__init__.py
+-rw-r--r--   0        0        0    26991 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/solver.py
+-rw-r--r--   0        0        0      840 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/types.py
+-rw-r--r--   0        0        0    14080 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/wrappers.py
+-rw-r--r--   0        0        0      459 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/__init__.py
+-rw-r--r--   0        0        0     7322 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/base.py
+-rw-r--r--   0        0        0     7136 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/edge_swaps.py
+-rw-r--r--   0        0        0     5488 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/er.py
+-rw-r--r--   0        0        0     5906 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/rdpg.py
+-rw-r--r--   0        0        0    19673 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/sbm_estimators.py
+-rw-r--r--   0        0        0    16934 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/nominate/VNviaSGM.py
+-rw-r--r--   0        0        0      234 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/nominate/__init__.py
+-rw-r--r--   0        0        0    10972 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/nominate/spectralVN.py
+-rw-r--r--   0        0        0      419 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/partition/__init__.py
+-rw-r--r--   0        0        0    25153 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/partition/leiden.py
+-rw-r--r--   0        0        0     5311 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/partition/modularity.py
+-rw-r--r--   0        0        0     1091 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/__init__.py
+-rw-r--r--   0        0        0      744 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/_elbow.py
+-rw-r--r--   0        0        0       91 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/_types.py
+-rw-r--r--   0        0        0     9212 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/adjacency_spectral_embedding.py
+-rw-r--r--   0        0        0     4269 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/embeddings.py
+-rw-r--r--   0        0        0     9918 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/laplacian_spectral_embedding.py
+-rw-r--r--   0        0        0    12796 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/omnibus_embedding.py
+-rw-r--r--   0        0        0     4045 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/graph_builder.py
+-rw-r--r--   0        0        0      528 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/plot/__init__.py
+-rw-r--r--   0        0        0    64195 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/plot/plot.py
+-rw-r--r--   0        0        0    34806 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/plot/plot_matrix.py
+-rw-r--r--   0        0        0     3456 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/preconditions.py
+-rw-r--r--   0        0        0      604 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/preprocessing/__init__.py
+-rw-r--r--   0        0        0    16315 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/preprocessing/graph_cuts.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/py.typed
+-rw-r--r--   0        0        0      482 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/__init__.py
+-rw-r--r--   0        0        0     4904 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/rdpg_corr.py
+-rw-r--r--   0        0        0    38533 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/simulations.py
+-rw-r--r--   0        0        0    10269 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/simulations_corr.py
+-rw-r--r--   0        0        0      153 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/subgraph/__init__.py
+-rw-r--r--   0        0        0     8470 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/subgraph/sg.py
+-rw-r--r--   0        0        0     1781 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/types.py
+-rw-r--r--   0        0        0     1195 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/utils/__init__.py
+-rw-r--r--   0        0        0     4201 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/utils/ptr.py
+-rw-r--r--   0        0        0    40441 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/utils/utils.py
+-rw-r--r--   0        0        0     1765 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/version.py
+-rw-r--r--   0        0        0     4306 2024-05-20 21:39:33.610047 graspologic-3.3.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 graspologic-3.3.1.dev9/PKG-INFO
```

### Comparing `graspologic-3.3.1.dev14/LICENSE.txt` & `graspologic-3.3.1.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/README.md` & `graspologic-3.3.1.dev9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!-- omit in toc -->
 # graspologic
 [![Paper shield](https://img.shields.io/badge/JMLR-Paper-red)](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 [![PyPI version](https://img.shields.io/pypi/v/graspologic.svg)](https://pypi.org/project/graspologic/)
 [![Downloads shield](https://pepy.tech/badge/graspologic)](https://pepy.tech/project/graspologic)
-[![graspologic Build](https://github.com/graspologic-org/graspologic/actions/workflows/build.yml/badge.svg)](https://github.com/graspologic-org/graspologic/actions/workflows/build.yml)
+[![graspologic Build](https://github.com/microsoft/graspologic/actions/workflows/build.yml/badge.svg)](https://github.com/microsoft/graspologic/actions/workflows/build.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## `graspologic` is a package for graph statistical algorithms.
 <!-- no toc -->
 - [Overview](#overview)
 - [Documentation](#documentation)
 - [System Requirements](#system-requirements)
@@ -42,43 +42,43 @@
 And across the following **x86_64** versions of Python:
 - 3.9
 - 3.10
 - 3.11
 - 3.12
 
 If you try to use `graspologic` for a different platform than the ones listed and notice any unexpected behavior,
-please feel free to [raise an issue](https://github.com/graspologic-org/graspologic/issues/new).  It's better for ourselves and our users
+please feel free to [raise an issue](https://github.com/microsoft/graspologic/issues/new).  It's better for ourselves and our users
 if we have concrete examples of things not working!
 
 # Installation Guide
 <!-- omit in toc -->
 ## Install from pip
 ```
 pip install graspologic
 ```
 
 <!-- omit in toc -->
 ## Install from Github
 ```
-git clone https://github.com/graspologic-org/graspologic
+git clone https://github.com/microsoft/graspologic
 cd graspologic
 python3 -m venv venv
 source venv/bin/activate
 python3 setup.py install
 ```
 
 # Contributing
-We welcome contributions from anyone. Please see our [contribution guidelines](https://github.com/graspologic-org/graspologic/blob/dev/CONTRIBUTING.md) before making a pull request. Our
-[issues](https://github.com/graspologic-org/graspologic/issues) page is full of places we could use help!
+We welcome contributions from anyone. Please see our [contribution guidelines](https://github.com/microsoft/graspologic/blob/dev/CONTRIBUTING.md) before making a pull request. Our
+[issues](https://github.com/microsoft/graspologic/issues) page is full of places we could use help!
 If you have an idea for an improvement not listed there, please
-[make an issue](https://github.com/graspologic-org/graspologic/issues/new) first so you can discuss with the developers.
+[make an issue](https://github.com/microsoft/graspologic/issues/new) first so you can discuss with the developers.
 
 # License
 This project is covered under the MIT License.
 
 # Issues
-We appreciate detailed bug reports and feature requests (though we appreciate pull requests even more!). Please visit our [issues](https://github.com/graspologic-org/graspologic/issues) page if you have questions or ideas.
+We appreciate detailed bug reports and feature requests (though we appreciate pull requests even more!). Please visit our [issues](https://github.com/microsoft/graspologic/issues) page if you have questions or ideas.
 
 # Citing `graspologic`
 If you find `graspologic` useful in your work, please cite the package via the [GraSPy paper](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 
 > Chung, J., Pedigo, B. D., Bridgeford, E. W., Varjavand, B. K., Helm, H. S., & Vogelstein, J. T. (2019). GraSPy: Graph Statistics in Python. Journal of Machine Learning Research, 20(158), 1-7.
```

### Comparing `graspologic-3.3.1.dev14/graspologic/__init__.py` & `graspologic-3.3.1.dev9/graspologic/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/align/base.py` & `graspologic-3.3.1.dev9/graspologic/align/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/align/orthogonal_procrustes.py` & `graspologic-3.3.1.dev9/graspologic/align/orthogonal_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/align/seedless_procrustes.py` & `graspologic-3.3.1.dev9/graspologic/align/seedless_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/align/sign_flips.py` & `graspologic-3.3.1.dev9/graspologic/align/sign_flips.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/cluster/autogmm.py` & `graspologic-3.3.1.dev9/graspologic/cluster/autogmm.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/cluster/base.py` & `graspologic-3.3.1.dev9/graspologic/cluster/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/cluster/divisive_cluster.py` & `graspologic-3.3.1.dev9/graspologic/cluster/divisive_cluster.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/cluster/gclust.py` & `graspologic-3.3.1.dev9/graspologic/cluster/gclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/cluster/kclust.py` & `graspologic-3.3.1.dev9/graspologic/cluster/kclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/base.py` & `graspologic-3.3.1.dev9/graspologic/datasets/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/drosophila/left_adjacency.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/drosophila/left_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/drosophila/right_adjacency.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/drosophila/right_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/atlas.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/atlas.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54776.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54776.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54777.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54777.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54779.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54779.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54781.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54781.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54790.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54790.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54793.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54793.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54794.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54794.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54797.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54797.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54811.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54811.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54813.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54813.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54815.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54815.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54817.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54817.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54821.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54821.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54823.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54823.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54829.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54829.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54831.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54831.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54833.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54833.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54835.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54835.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54842.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54842.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54847.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54847.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54849.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54849.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54851.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54851.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54853.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54853.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54855.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54855.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54864.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54864.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54866.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54866.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54868.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54868.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54870.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54870.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54883.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54883.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54885.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54885.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54887.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54887.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/features/54890.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54890.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/datasets/mice/participants.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/participants.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/__init__.py` & `graspologic-3.3.1.dev9/graspologic/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/ase.py` & `graspologic-3.3.1.dev9/graspologic/embed/ase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/base.py` & `graspologic-3.3.1.dev9/graspologic/embed/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/case.py` & `graspologic-3.3.1.dev9/graspologic/embed/case.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/lse.py` & `graspologic-3.3.1.dev9/graspologic/embed/lse.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/mase.py` & `graspologic-3.3.1.dev9/graspologic/embed/mase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/mds.py` & `graspologic-3.3.1.dev9/graspologic/embed/mds.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/mug2vec.py` & `graspologic-3.3.1.dev9/graspologic/embed/mug2vec.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/n2v.py` & `graspologic-3.3.1.dev9/graspologic/embed/n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/omni.py` & `graspologic-3.3.1.dev9/graspologic/embed/omni.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/embed/svd.py` & `graspologic-3.3.1.dev9/graspologic/embed/svd.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/inference/binomial.py` & `graspologic-3.3.1.dev9/graspologic/inference/binomial.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/inference/density_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/density_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/inference/group_connection_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/group_connection_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/inference/latent_distribution_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/latent_distribution_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/inference/latent_position_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/latent_position_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/inference/utils.py` & `graspologic-3.3.1.dev9/graspologic/inference/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/__main__.py` & `graspologic-3.3.1.dev9/graspologic/layouts/__main__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/auto.py` & `graspologic-3.3.1.dev9/graspologic/layouts/auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/colors.py` & `graspologic-3.3.1.dev9/graspologic/layouts/colors.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/include/colors-100.json` & `graspologic-3.3.1.dev9/graspologic/layouts/include/colors-100.json`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_grid.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_grid.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_node.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_quad_node.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/_quad_tree.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_tree.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/nooverlap/nooverlap.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/nooverlap.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/layouts/render.py` & `graspologic-3.3.1.dev9/graspologic/layouts/render.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/match/solver.py` & `graspologic-3.3.1.dev9/graspologic/match/solver.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/match/types.py` & `graspologic-3.3.1.dev9/graspologic/match/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/match/wrappers.py` & `graspologic-3.3.1.dev9/graspologic/match/wrappers.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/models/base.py` & `graspologic-3.3.1.dev9/graspologic/models/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/models/edge_swaps.py` & `graspologic-3.3.1.dev9/graspologic/models/edge_swaps.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/models/er.py` & `graspologic-3.3.1.dev9/graspologic/models/er.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/models/rdpg.py` & `graspologic-3.3.1.dev9/graspologic/models/rdpg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/models/sbm_estimators.py` & `graspologic-3.3.1.dev9/graspologic/models/sbm_estimators.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/nominate/VNviaSGM.py` & `graspologic-3.3.1.dev9/graspologic/nominate/VNviaSGM.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/nominate/spectralVN.py` & `graspologic-3.3.1.dev9/graspologic/nominate/spectralVN.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/partition/leiden.py` & `graspologic-3.3.1.dev9/graspologic/partition/leiden.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
     --------
     graspologic.utils.is_unweighted
 
     References
     ----------
     .. [1] Traag, V.A.; Waltman, L.; Van, Eck N.J. "From Louvain to Leiden:
          guaranteeing well-connected communities", Scientific Reports, Vol. 9, 2019
-    .. [2] https://github.com/graspologic-org/graspologic-native
+    .. [2] https://github.com/microsoft/graspologic-native
 
     Notes
     -----
     No two different nodes are allowed to encode to the **same** str representation,
     e.g. node_a id of ``"1"`` and node_b id of ``1`` are different object types
     but str(node_a) == str(node_b). This collision will result in a ``ValueError``
 
@@ -544,15 +544,15 @@
     --------
     graspologic.utils.is_unweighted
 
     References
     ----------
     .. [1] Traag, V.A.; Waltman, L.; Van, Eck N.J. "From Louvain to Leiden:
         guaranteeing well-connected communities",Scientific Reports, Vol. 9, 2019
-    .. [2] https://github.com/graspologic-org/graspologic-native
+    .. [2] https://github.com/microsoft/graspologic-native
 
     Notes
     -----
     No two different nodes are allowed to encode to the **same** str representation,
     e.g. node_a id of ``"1"`` and node_b id of ``1`` are different object types
     but str(node_a) == str(node_b). This collision will result in a ``ValueError``
```

### Comparing `graspologic-3.3.1.dev14/graspologic/partition/modularity.py` & `graspologic-3.3.1.dev9/graspologic/partition/modularity.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/__init__.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/embed/__init__.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/embed/_elbow.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/_elbow.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/embed/adjacency_spectral_embedding.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/adjacency_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/embed/embeddings.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/embeddings.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/embed/laplacian_spectral_embedding.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/laplacian_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/embed/omnibus_embedding.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/omnibus_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/pipeline/graph_builder.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/graph_builder.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/plot/__init__.py` & `graspologic-3.3.1.dev9/graspologic/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/plot/plot.py` & `graspologic-3.3.1.dev9/graspologic/plot/plot.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/plot/plot_matrix.py` & `graspologic-3.3.1.dev9/graspologic/plot/plot_matrix.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/preconditions.py` & `graspologic-3.3.1.dev9/graspologic/preconditions.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/preprocessing/__init__.py` & `graspologic-3.3.1.dev9/graspologic/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/preprocessing/graph_cuts.py` & `graspologic-3.3.1.dev9/graspologic/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/simulations/rdpg_corr.py` & `graspologic-3.3.1.dev9/graspologic/simulations/rdpg_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/simulations/simulations.py` & `graspologic-3.3.1.dev9/graspologic/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/simulations/simulations_corr.py` & `graspologic-3.3.1.dev9/graspologic/simulations/simulations_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/subgraph/sg.py` & `graspologic-3.3.1.dev9/graspologic/subgraph/sg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/types.py` & `graspologic-3.3.1.dev9/graspologic/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/utils/__init__.py` & `graspologic-3.3.1.dev9/graspologic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/utils/ptr.py` & `graspologic-3.3.1.dev9/graspologic/utils/ptr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/utils/utils.py` & `graspologic-3.3.1.dev9/graspologic/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/graspologic/version.py` & `graspologic-3.3.1.dev9/graspologic/version.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.1.dev14/pyproject.toml` & `graspologic-3.3.1.dev9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "graspologic"
-version = "3.3.1.dev14"
+version = "3.3.1.dev9"
 description = "A set of Python modules for graph statistics"
-repository = "https://github.com/graspologic-org/graspologic"
+repository = "https://github.com/microsoft/graspologic"
 authors = [
     "Eric Bridgeford", 
     "Jaewon Chung <j1c@jhu.edu>", 
     "Benjamin Pedigo", 
     "Bijan Varjavand",
 ]
 maintainers = [
```

### Comparing `graspologic-3.3.1.dev14/PKG-INFO` & `graspologic-3.3.1.dev9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.3.1.dev14
+Version: 3.3.1.dev9
 Summary: A set of Python modules for graph statistics
-Home-page: https://github.com/graspologic-org/graspologic
+Home-page: https://github.com/microsoft/graspologic
 License: MIT
 Author: Eric Bridgeford
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -29,23 +29,23 @@
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (==1.12.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: umap-learn (>=0.5.6,<0.6.0)
-Project-URL: Repository, https://github.com/graspologic-org/graspologic
+Project-URL: Repository, https://github.com/microsoft/graspologic
 Description-Content-Type: text/markdown
 
 <!-- omit in toc -->
 # graspologic
 [![Paper shield](https://img.shields.io/badge/JMLR-Paper-red)](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 [![PyPI version](https://img.shields.io/pypi/v/graspologic.svg)](https://pypi.org/project/graspologic/)
 [![Downloads shield](https://pepy.tech/badge/graspologic)](https://pepy.tech/project/graspologic)
-[![graspologic Build](https://github.com/graspologic-org/graspologic/actions/workflows/build.yml/badge.svg)](https://github.com/graspologic-org/graspologic/actions/workflows/build.yml)
+[![graspologic Build](https://github.com/microsoft/graspologic/actions/workflows/build.yml/badge.svg)](https://github.com/microsoft/graspologic/actions/workflows/build.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## `graspologic` is a package for graph statistical algorithms.
 <!-- no toc -->
 - [Overview](#overview)
 - [Documentation](#documentation)
 - [System Requirements](#system-requirements)
@@ -80,44 +80,44 @@
 And across the following **x86_64** versions of Python:
 - 3.9
 - 3.10
 - 3.11
 - 3.12
 
 If you try to use `graspologic` for a different platform than the ones listed and notice any unexpected behavior,
-please feel free to [raise an issue](https://github.com/graspologic-org/graspologic/issues/new).  It's better for ourselves and our users
+please feel free to [raise an issue](https://github.com/microsoft/graspologic/issues/new).  It's better for ourselves and our users
 if we have concrete examples of things not working!
 
 # Installation Guide
 <!-- omit in toc -->
 ## Install from pip
 ```
 pip install graspologic
 ```
 
 <!-- omit in toc -->
 ## Install from Github
 ```
-git clone https://github.com/graspologic-org/graspologic
+git clone https://github.com/microsoft/graspologic
 cd graspologic
 python3 -m venv venv
 source venv/bin/activate
 python3 setup.py install
 ```
 
 # Contributing
-We welcome contributions from anyone. Please see our [contribution guidelines](https://github.com/graspologic-org/graspologic/blob/dev/CONTRIBUTING.md) before making a pull request. Our
-[issues](https://github.com/graspologic-org/graspologic/issues) page is full of places we could use help!
+We welcome contributions from anyone. Please see our [contribution guidelines](https://github.com/microsoft/graspologic/blob/dev/CONTRIBUTING.md) before making a pull request. Our
+[issues](https://github.com/microsoft/graspologic/issues) page is full of places we could use help!
 If you have an idea for an improvement not listed there, please
-[make an issue](https://github.com/graspologic-org/graspologic/issues/new) first so you can discuss with the developers.
+[make an issue](https://github.com/microsoft/graspologic/issues/new) first so you can discuss with the developers.
 
 # License
 This project is covered under the MIT License.
 
 # Issues
-We appreciate detailed bug reports and feature requests (though we appreciate pull requests even more!). Please visit our [issues](https://github.com/graspologic-org/graspologic/issues) page if you have questions or ideas.
+We appreciate detailed bug reports and feature requests (though we appreciate pull requests even more!). Please visit our [issues](https://github.com/microsoft/graspologic/issues) page if you have questions or ideas.
 
 # Citing `graspologic`
 If you find `graspologic` useful in your work, please cite the package via the [GraSPy paper](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 
 > Chung, J., Pedigo, B. D., Bridgeford, E. W., Varjavand, B. K., Helm, H. S., & Vogelstein, J. T. (2019). GraSPy: Graph Statistics in Python. Journal of Machine Learning Research, 20(158), 1-7.
```

