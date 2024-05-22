# Comparing `tmp/vsensebox_ultralytics-8.2.15.tar.gz` & `tmp/vsensebox_ultralytics-8.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox_ultralytics-8.2.15.tar", last modified: Tue May 14 14:11:06 2024, max compression
+gzip compressed data, was "vsensebox_ultralytics-8.2.18.tar", last modified: Wed May 22 10:09:34 2024, max compression
```

## Comparing `vsensebox_ultralytics-8.2.15.tar` & `vsensebox_ultralytics-8.2.18.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.292057 vsensebox_ultralytics-8.2.15/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.296057 vsensebox_ultralytics-8.2.15/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.296057 vsensebox_ultralytics-8.2.15/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.296057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.288057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.300057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.304057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.304057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.304057 vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57665 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    31051 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58122 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40103 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30919 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    35048 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.308057 vsensebox_ultralytics-8.2.15/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.312057 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.316057 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30866 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/parking_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.320057 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.324057 vsensebox_ultralytics-8.2.15/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    23552 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    28375 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15654 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    48466 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-14 14:11:01.000000 vsensebox_ultralytics-8.2.15/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:06.328057 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-14 14:11:06.000000 vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.175881 vsensebox_ultralytics-8.2.18/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-22 10:09:34.175881 vsensebox_ultralytics-8.2.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-22 10:09:34.175881 vsensebox_ultralytics-8.2.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.135881 vsensebox_ultralytics-8.2.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.135881 vsensebox_ultralytics-8.2.18/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.135881 vsensebox_ultralytics-8.2.18/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.135881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.143881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.131881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.143881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.143881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.143881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.143881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.147881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.147881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.147881 vsensebox_ultralytics-8.2.18/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.151881 vsensebox_ultralytics-8.2.18/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57665 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.151881 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.151881 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31051 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.151881 vsensebox_ultralytics-8.2.18/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58122 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40103 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30975 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.151881 vsensebox_ultralytics-8.2.18/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.151881 vsensebox_ultralytics-8.2.18/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.155881 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-22 10:09:28.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.155881 vsensebox_ultralytics-8.2.18/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.155881 vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.155881 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.159881 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.159881 vsensebox_ultralytics-8.2.18/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.159881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.159881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.159881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.159881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.163881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.163881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.163881 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.163881 vsensebox_ultralytics-8.2.18/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30866 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.163881 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.167881 vsensebox_ultralytics-8.2.18/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/parking_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.167881 vsensebox_ultralytics-8.2.18/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.167881 vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.171881 vsensebox_ultralytics-8.2.18/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23552 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.171881 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28436 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15654 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48207 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-22 10:09:29.000000 vsensebox_ultralytics-8.2.18/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:09:34.175881 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-22 10:09:34.000000 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-22 10:09:34.000000 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:09:34.000000 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 10:09:34.000000 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-22 10:09:34.000000 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-22 10:09:34.000000 vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/top_level.txt
```

### Comparing `vsensebox_ultralytics-8.2.15/LICENSE` & `vsensebox_ultralytics-8.2.18/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/PKG-INFO` & `vsensebox_ultralytics-8.2.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vsensebox-ultralytics
-Version: 8.2.15
+Version: 8.2.18
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
-Home-page: https://github.com/rathaumons/ultralytics-for-vsensebox
+Home-page: https://github.com/numediart/ultralytics-for-vsensebox
 License: AGPL-3.0
-Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-vsensebox/issues
-Project-URL: Funding, https://ultralytics.com
-Project-URL: Source, https://github.com/rathaumons/ultralytics-for-vsensebox
+Project-URL: Bug Reports, https://github.com/numediart/ultralytics-for-vsensebox/issues
+Project-URL: Source, https://github.com/numediart/ultralytics-for-vsensebox
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -47,43 +46,43 @@
 Requires-Dist: coremltools>=7.0; extra == "export"
 Requires-Dist: openvino>=2024.0.0; extra == "export"
 Provides-Extra: explorer
 Requires-Dist: lancedb; extra == "explorer"
 Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 
-[![Test Build](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
+[![Test Build](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
 
 # Customized Ultralytics for VSenseBox
 
-* Updated: **May 14, 2024**
-* Synced with: v8.2.15 -> [[590002f]](https://github.com/ultralytics/ultralytics/commit/590002ff6d3a936b0cb1aeb582ea2daa26fcdbb6)
+* Updated: **May 22, 2024**
+* Synced with: v8.2.18 -> [[c8b6a8b]](https://github.com/ultralytics/ultralytics/commit/c8b6a8bc37ce196a6b7e0c153539402db4383c16)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
-* Customized for [`VSenseBox`](https://github.com/rathaumons/vsensebox):
+* Customized for [`VSenseBox`](https://github.com/numediart/vsensebox):
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
 
 ## Installation
 
 * Install from [PyPI](https://pypi.org/project/vsensebox-ultralytics/):
     ```
     pip install vsensebox-ultralytics
     ``` 
 * Or install from GitHub directly:
     ```
-    pip install git+https://github.com/rathaumons/ultralytics-for-vsensebox.git
+    pip install git+https://github.com/numediart/ultralytics-for-vsensebox.git
     ```
 * Or build from source:
 
     <details><summary><ins>Click here to expand!</ins></summary>
     
     ```
-    git clone https://github.com/rathaumons/ultralytics-for-vsensebox.git
+    git clone https://github.com/numediart/ultralytics-for-vsensebox.git
     cd ultralytics-for-vsensebox
     python -m pip install --upgrade pip
     python -m pip install -U pip setuptools
     pip install wheel build
     python -m build --wheel --skip-dependency-check --no-isolatio
     cd dist
     ```
```

### Comparing `vsensebox_ultralytics-8.2.15/README.md` & `vsensebox_ultralytics-8.2.18/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[![Test Build](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
+[![Test Build](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
 
 # Customized Ultralytics for VSenseBox
 
-* Updated: **May 14, 2024**
-* Synced with: v8.2.15 -> [[590002f]](https://github.com/ultralytics/ultralytics/commit/590002ff6d3a936b0cb1aeb582ea2daa26fcdbb6)
+* Updated: **May 22, 2024**
+* Synced with: v8.2.18 -> [[c8b6a8b]](https://github.com/ultralytics/ultralytics/commit/c8b6a8bc37ce196a6b7e0c153539402db4383c16)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
-* Customized for [`VSenseBox`](https://github.com/rathaumons/vsensebox):
+* Customized for [`VSenseBox`](https://github.com/numediart/vsensebox):
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
 
 ## Installation
 
 * Install from [PyPI](https://pypi.org/project/vsensebox-ultralytics/):
     ```
     pip install vsensebox-ultralytics
     ``` 
 * Or install from GitHub directly:
     ```
-    pip install git+https://github.com/rathaumons/ultralytics-for-vsensebox.git
+    pip install git+https://github.com/numediart/ultralytics-for-vsensebox.git
     ```
 * Or build from source:
 
     <details><summary><ins>Click here to expand!</ins></summary>
     
     ```
-    git clone https://github.com/rathaumons/ultralytics-for-vsensebox.git
+    git clone https://github.com/numediart/ultralytics-for-vsensebox.git
     cd ultralytics-for-vsensebox
     python -m pip install --upgrade pip
     python -m pip install -U pip setuptools
     pip install wheel build
     python -m build --wheel --skip-dependency-check --no-isolatio
     cd dist
     ```
```

### Comparing `vsensebox_ultralytics-8.2.15/requirements.txt` & `vsensebox_ultralytics-8.2.18/requirements.txt`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/setup.cfg` & `vsensebox_ultralytics-8.2.18/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/setup.py` & `vsensebox_ultralytics-8.2.18/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,19 +46,18 @@
     version=get_version(),  # version of pypi package
     python_requires='>=3.8',
     license='AGPL-3.0',
     description=('Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, '
                  'pose estimation and image classification.'),
     long_description=README,
     long_description_content_type='text/markdown',
-    url='https://github.com/rathaumons/ultralytics-for-vsensebox',
+    url='https://github.com/numediart/ultralytics-for-vsensebox',
     project_urls={
-        'Bug Reports': 'https://github.com/rathaumons/ultralytics-for-vsensebox/issues',
-        'Funding': 'https://ultralytics.com',
-        'Source': 'https://github.com/rathaumons/ultralytics-for-vsensebox'},
+        'Bug Reports': 'https://github.com/numediart/ultralytics-for-vsensebox/issues',
+        'Source': 'https://github.com/numediart/ultralytics-for-vsensebox'},
     packages=['ultralytics'] + [str(x) for x in Path('ultralytics').rglob('*/') if x.is_dir() and '__' not in str(x)],
     package_data={
         '': ['*.yaml'],
         'ultralytics.assets': ['*.jpg']},
     include_package_data=True,
     install_requires=parse_requirements(PARENT / 'requirements.txt'),
     extras_require={
```

### Comparing `vsensebox_ultralytics-8.2.15/tests/__init__.py` & `vsensebox_ultralytics-8.2.18/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/conftest.py` & `vsensebox_ultralytics-8.2.18/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_cli.py` & `vsensebox_ultralytics-8.2.18/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_cuda.py` & `vsensebox_ultralytics-8.2.18/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_engine.py` & `vsensebox_ultralytics-8.2.18/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_explorer.py` & `vsensebox_ultralytics-8.2.18/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_exports.py` & `vsensebox_ultralytics-8.2.18/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_integrations.py` & `vsensebox_ultralytics-8.2.18/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/tests/test_python.py` & `vsensebox_ultralytics-8.2.18/tests/test_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,16 @@
     ONLINE,
     ROOT,
     WEIGHTS_DIR,
     WINDOWS,
     Retry,
     checks,
 )
-from ultralytics.utils.downloads import download
+from ultralytics.utils.downloads import download, is_url
 from ultralytics.utils.torch_utils import TORCH_1_9
-
 from . import CFG, IS_TMP_WRITEABLE, MODEL, SOURCE, TMP
 
 
 def test_model_forward():
     """Test the forward pass of the YOLO model."""
     model = YOLO(CFG)
     model(source=None, imgsz=32, augment=True)  # also test no source and augment
@@ -98,15 +97,15 @@
     assert len(model(batch, imgsz=32)) == len(batch)  # multiple sources in a batch
 
 
 @pytest.mark.parametrize("model", MODELS)
 def test_predict_visualize(model):
     """Test model predict methods with 'visualize=True' arguments."""
     YOLO(WEIGHTS_DIR / model)(SOURCE, imgsz=32, visualize=True)
-    
+
 
 def test_predict_grey_and_4ch():
     """Test YOLO prediction on SOURCE converted to greyscale and 4-channel images."""
     im = Image.open(SOURCE)
     directory = TMP / "im4"
     directory.mkdir(parents=True, exist_ok=True)
 
@@ -127,14 +126,15 @@
             results = model(source, save=True, verbose=True, imgsz=32)
             assert len(results) == 1  # verify that an image was run
         f.unlink()  # cleanup
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not ONLINE, reason="environment is offline")
+@pytest.mark.skipif(not is_url("https://youtu.be/G17sBkb38XQ"), reason="YouTube URL issue")
 @Retry(times=3, delay=10)
 def test_youtube():
     """
     Test YouTube inference.
 
     Marked --slow to reduce YouTube API rate limits risk.
     """
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.2.15"
+__version__ = "8.2.18"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/assets/bus.jpg` & `vsensebox_ultralytics-8.2.18/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/assets/zidane.jpg` & `vsensebox_ultralytics-8.2.18/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Argoverse.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/DOTAv1.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/ImageNet.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/Objects365.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/SKU-110K.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VOC.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/VisDrone.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/african-wildlife.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/brain-tumor.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/carparts-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco-pose.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco128.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-pose.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/coco8.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/crack-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/dota8.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/lvis.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/open-images-v7.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/package-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/tiger-pose.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/datasets/xView.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/default.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v3/yolov3.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v5/yolov5.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v6/yolov6.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-world.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v8/yolov8.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 # YOLOv9c-seg
 # 654 layers, 27897120 parameters, 159.4 GFLOPs
 
 # parameters
-nc: 80  # number of classes
+nc: 80 # number of classes
 
 # gelan backbone
 backbone:
-  - [-1, 1, Conv, [64, 3, 2]]  # 0-P1/2
-  - [-1, 1, Conv, [128, 3, 2]]  # 1-P2/4
-  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 1]]  # 2
-  - [-1, 1, ADown, [256]]  # 3-P3/8
-  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 1]]  # 4
-  - [-1, 1, ADown, [512]]  # 5-P4/16
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 6
-  - [-1, 1, ADown, [512]]  # 7-P5/32
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 8
-  - [-1, 1, SPPELAN, [512, 256]]  # 9
+  - [-1, 1, Conv, [64, 3, 2]] # 0-P1/2
+  - [-1, 1, Conv, [128, 3, 2]] # 1-P2/4
+  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 1]] # 2
+  - [-1, 1, ADown, [256]] # 3-P3/8
+  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 1]] # 4
+  - [-1, 1, ADown, [512]] # 5-P4/16
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 6
+  - [-1, 1, ADown, [512]] # 7-P5/32
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 8
+  - [-1, 1, SPPELAN, [512, 256]] # 9
 
 head:
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 6], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 12
-
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 4], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 1]]  # 15 (P3/8-small)
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 6], 1, Concat, [1]] # cat backbone P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 12
+
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 4], 1, Concat, [1]] # cat backbone P3
+  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 1]] # 15 (P3/8-small)
 
   - [-1, 1, ADown, [256]]
-  - [[-1, 12], 1, Concat, [1]]  # cat head P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 18 (P4/16-medium)
+  - [[-1, 12], 1, Concat, [1]] # cat head P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 18 (P4/16-medium)
 
   - [-1, 1, ADown, [512]]
-  - [[-1, 9], 1, Concat, [1]]  # cat head P5
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 21 (P5/32-large)
+  - [[-1, 9], 1, Concat, [1]] # cat head P5
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 21 (P5/32-large)
 
-  - [[15, 18, 21], 1, Segment, [nc, 32, 256]]  # Segment(P3, P4, P5)
+  - [[15, 18, 21], 1, Segment, [nc, 32, 256]] # Segment(P3, P4, P5)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9c.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 # YOLOv9c
 # 618 layers, 25590912 parameters, 104.0 GFLOPs
 
 # parameters
-nc: 80  # number of classes
+nc: 80 # number of classes
 
 # gelan backbone
 backbone:
-  - [-1, 1, Conv, [64, 3, 2]]  # 0-P1/2
-  - [-1, 1, Conv, [128, 3, 2]]  # 1-P2/4
-  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 1]]  # 2
-  - [-1, 1, ADown, [256]]  # 3-P3/8
-  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 1]]  # 4
-  - [-1, 1, ADown, [512]]  # 5-P4/16
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 6
-  - [-1, 1, ADown, [512]]  # 7-P5/32
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 8
-  - [-1, 1, SPPELAN, [512, 256]]  # 9
+  - [-1, 1, Conv, [64, 3, 2]] # 0-P1/2
+  - [-1, 1, Conv, [128, 3, 2]] # 1-P2/4
+  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 1]] # 2
+  - [-1, 1, ADown, [256]] # 3-P3/8
+  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 1]] # 4
+  - [-1, 1, ADown, [512]] # 5-P4/16
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 6
+  - [-1, 1, ADown, [512]] # 7-P5/32
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 8
+  - [-1, 1, SPPELAN, [512, 256]] # 9
 
 head:
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 6], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 12
-
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 4], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 1]]  # 15 (P3/8-small)
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 6], 1, Concat, [1]] # cat backbone P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 12
+
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 4], 1, Concat, [1]] # cat backbone P3
+  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 1]] # 15 (P3/8-small)
 
   - [-1, 1, ADown, [256]]
-  - [[-1, 12], 1, Concat, [1]]  # cat head P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 18 (P4/16-medium)
+  - [[-1, 12], 1, Concat, [1]] # cat head P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 18 (P4/16-medium)
 
   - [-1, 1, ADown, [512]]
-  - [[-1, 9], 1, Concat, [1]]  # cat head P5
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]]  # 21 (P5/32-large)
+  - [[-1, 9], 1, Concat, [1]] # cat head P5
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 1]] # 21 (P5/32-large)
 
-  - [[15, 18, 21], 1, Detect, [nc]]  # Detect(P3, P4, P5)
+  - [[15, 18, 21], 1, Detect, [nc]] # Detect(P3, P4, P5)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
-# YOLOv9c-seg
-# 1261 layers, 60512800 parameters, 248.4 GFLOPs
+# YOLOv9e
+# 1225 layers, 58206592 parameters, 193.0 GFLOPs
 
 # parameters
-nc: 80  # number of classes
+nc: 80 # number of classes
 
 # gelan backbone
 backbone:
   - [-1, 1, Silence, []]
-  - [-1, 1, Conv, [64, 3, 2]]  # 1-P1/2
-  - [-1, 1, Conv, [128, 3, 2]]  # 2-P2/4
-  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]]  # 3
-  - [-1, 1, ADown, [256]]  # 4-P3/8
-  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]]  # 5
-  - [-1, 1, ADown, [512]]  # 6-P4/16
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 7
-  - [-1, 1, ADown, [1024]]  # 8-P5/32
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 9
+  - [-1, 1, Conv, [64, 3, 2]] # 1-P1/2
+  - [-1, 1, Conv, [128, 3, 2]] # 2-P2/4
+  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]] # 3
+  - [-1, 1, ADown, [256]] # 4-P3/8
+  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]] # 5
+  - [-1, 1, ADown, [512]] # 6-P4/16
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 7
+  - [-1, 1, ADown, [1024]] # 8-P5/32
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 9
 
   - [1, 1, CBLinear, [[64]]] # 10
   - [3, 1, CBLinear, [[64, 128]]] # 11
   - [5, 1, CBLinear, [[64, 128, 256]]] # 12
   - [7, 1, CBLinear, [[64, 128, 256, 512]]] # 13
   - [9, 1, CBLinear, [[64, 128, 256, 512, 1024]]] # 14
 
-  - [0, 1, Conv, [64, 3, 2]]  # 15-P1/2
+  - [0, 1, Conv, [64, 3, 2]] # 15-P1/2
   - [[10, 11, 12, 13, 14, -1], 1, CBFuse, [[0, 0, 0, 0, 0]]] # 16
-  - [-1, 1, Conv, [128, 3, 2]]  # 17-P2/4
-  - [[11, 12, 13, 14, -1], 1, CBFuse, [[1, 1, 1, 1]]] # 18  
-  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]]  # 19
-  - [-1, 1, ADown, [256]]  # 20-P3/8
-  - [[12, 13, 14, -1], 1, CBFuse, [[2, 2, 2]]] # 21  
-  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]]  # 22
-  - [-1, 1, ADown, [512]]  # 23-P4/16
-  - [[13, 14, -1], 1, CBFuse, [[3, 3]]] # 24 
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 25
-  - [-1, 1, ADown, [1024]]  # 26-P5/32
+  - [-1, 1, Conv, [128, 3, 2]] # 17-P2/4
+  - [[11, 12, 13, 14, -1], 1, CBFuse, [[1, 1, 1, 1]]] # 18
+  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]] # 19
+  - [-1, 1, ADown, [256]] # 20-P3/8
+  - [[12, 13, 14, -1], 1, CBFuse, [[2, 2, 2]]] # 21
+  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]] # 22
+  - [-1, 1, ADown, [512]] # 23-P4/16
+  - [[13, 14, -1], 1, CBFuse, [[3, 3]]] # 24
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 25
+  - [-1, 1, ADown, [1024]] # 26-P5/32
   - [[14, -1], 1, CBFuse, [[4]]] # 27
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 28
-  - [-1, 1, SPPELAN, [512, 256]]  # 29
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 28
+  - [-1, 1, SPPELAN, [512, 256]] # 29
 
 # gelan head
 head:
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 25], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]]  # 32
-
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 22], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 2]]  # 35 (P3/8-small)
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 25], 1, Concat, [1]] # cat backbone P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]] # 32
+
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 22], 1, Concat, [1]] # cat backbone P3
+  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 2]] # 35 (P3/8-small)
 
   - [-1, 1, ADown, [256]]
-  - [[-1, 32], 1, Concat, [1]]  # cat head P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]]  # 38 (P4/16-medium)
+  - [[-1, 32], 1, Concat, [1]] # cat head P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]] # 38 (P4/16-medium)
 
   - [-1, 1, ADown, [512]]
-  - [[-1, 29], 1, Concat, [1]]  # cat head P5
-  - [-1, 1, RepNCSPELAN4, [512, 1024, 512, 2]]  # 41 (P5/32-large)
+  - [[-1, 29], 1, Concat, [1]] # cat head P5
+  - [-1, 1, RepNCSPELAN4, [512, 1024, 512, 2]] # 41 (P5/32-large)
 
-  - [[35, 38, 41], 1, Segment, [nc, 32, 256]]  # Segment (P3, P4, P5)
+  - [[35, 38, 41], 1, Detect, [nc]] # Detect(P3, P4, P5)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/models/v9/yolov9e.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
-# YOLOv9e
-# 1225 layers, 58206592 parameters, 193.0 GFLOPs
+# YOLOv9c-seg
+# 1261 layers, 60512800 parameters, 248.4 GFLOPs
 
 # parameters
-nc: 80  # number of classes
+nc: 80 # number of classes
 
 # gelan backbone
 backbone:
   - [-1, 1, Silence, []]
-  - [-1, 1, Conv, [64, 3, 2]]  # 1-P1/2
-  - [-1, 1, Conv, [128, 3, 2]]  # 2-P2/4
-  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]]  # 3
-  - [-1, 1, ADown, [256]]  # 4-P3/8
-  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]]  # 5
-  - [-1, 1, ADown, [512]]  # 6-P4/16
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 7
-  - [-1, 1, ADown, [1024]]  # 8-P5/32
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 9
+  - [-1, 1, Conv, [64, 3, 2]] # 1-P1/2
+  - [-1, 1, Conv, [128, 3, 2]] # 2-P2/4
+  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]] # 3
+  - [-1, 1, ADown, [256]] # 4-P3/8
+  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]] # 5
+  - [-1, 1, ADown, [512]] # 6-P4/16
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 7
+  - [-1, 1, ADown, [1024]] # 8-P5/32
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 9
 
   - [1, 1, CBLinear, [[64]]] # 10
   - [3, 1, CBLinear, [[64, 128]]] # 11
   - [5, 1, CBLinear, [[64, 128, 256]]] # 12
   - [7, 1, CBLinear, [[64, 128, 256, 512]]] # 13
   - [9, 1, CBLinear, [[64, 128, 256, 512, 1024]]] # 14
 
-  - [0, 1, Conv, [64, 3, 2]]  # 15-P1/2
+  - [0, 1, Conv, [64, 3, 2]] # 15-P1/2
   - [[10, 11, 12, 13, 14, -1], 1, CBFuse, [[0, 0, 0, 0, 0]]] # 16
-  - [-1, 1, Conv, [128, 3, 2]]  # 17-P2/4
-  - [[11, 12, 13, 14, -1], 1, CBFuse, [[1, 1, 1, 1]]] # 18  
-  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]]  # 19
-  - [-1, 1, ADown, [256]]  # 20-P3/8
-  - [[12, 13, 14, -1], 1, CBFuse, [[2, 2, 2]]] # 21  
-  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]]  # 22
-  - [-1, 1, ADown, [512]]  # 23-P4/16
-  - [[13, 14, -1], 1, CBFuse, [[3, 3]]] # 24 
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 25
-  - [-1, 1, ADown, [1024]]  # 26-P5/32
+  - [-1, 1, Conv, [128, 3, 2]] # 17-P2/4
+  - [[11, 12, 13, 14, -1], 1, CBFuse, [[1, 1, 1, 1]]] # 18
+  - [-1, 1, RepNCSPELAN4, [256, 128, 64, 2]] # 19
+  - [-1, 1, ADown, [256]] # 20-P3/8
+  - [[12, 13, 14, -1], 1, CBFuse, [[2, 2, 2]]] # 21
+  - [-1, 1, RepNCSPELAN4, [512, 256, 128, 2]] # 22
+  - [-1, 1, ADown, [512]] # 23-P4/16
+  - [[13, 14, -1], 1, CBFuse, [[3, 3]]] # 24
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 25
+  - [-1, 1, ADown, [1024]] # 26-P5/32
   - [[14, -1], 1, CBFuse, [[4]]] # 27
-  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]]  # 28
-  - [-1, 1, SPPELAN, [512, 256]]  # 29
+  - [-1, 1, RepNCSPELAN4, [1024, 512, 256, 2]] # 28
+  - [-1, 1, SPPELAN, [512, 256]] # 29
 
 # gelan head
 head:
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 25], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]]  # 32
-
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 22], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 2]]  # 35 (P3/8-small)
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 25], 1, Concat, [1]] # cat backbone P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]] # 32
+
+  - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
+  - [[-1, 22], 1, Concat, [1]] # cat backbone P3
+  - [-1, 1, RepNCSPELAN4, [256, 256, 128, 2]] # 35 (P3/8-small)
 
   - [-1, 1, ADown, [256]]
-  - [[-1, 32], 1, Concat, [1]]  # cat head P4
-  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]]  # 38 (P4/16-medium)
+  - [[-1, 32], 1, Concat, [1]] # cat head P4
+  - [-1, 1, RepNCSPELAN4, [512, 512, 256, 2]] # 38 (P4/16-medium)
 
   - [-1, 1, ADown, [512]]
-  - [[-1, 29], 1, Concat, [1]]  # cat head P5
-  - [-1, 1, RepNCSPELAN4, [512, 1024, 512, 2]]  # 41 (P5/32-large)
+  - [[-1, 29], 1, Concat, [1]] # cat head P5
+  - [-1, 1, RepNCSPELAN4, [512, 1024, 512, 2]] # 41 (P5/32-large)
 
-  - [[35, 38, 41], 1, Detect, [nc]]  # Detect(P3, P4, P5)
+  - [[35, 38, 41], 1, Segment, [nc, 32, 256]] # Segment (P3, P4, P5)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/botsort.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/cfg/trackers/bytetrack.yaml` & `vsensebox_ultralytics-8.2.18/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/annotator.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/augment.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/base.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/build.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/converter.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/dataset.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/explorer.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/gui/dash.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/explorer/utils.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/loaders.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/split_dota.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/data/utils.py` & `vsensebox_ultralytics-8.2.18/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/exporter.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/model.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/predictor.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/results.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         save(filename): Save annotated results to file.
         verbose(): Returns a log string for each task, detailing detections and classifications.
         save_txt(txt_file, save_conf=False): Saves detection results to a text file.
         save_crop(save_dir, file_name=Path("im.jpg")): Saves cropped detection images.
         tojson(normalize=False): Converts detection results to JSON format.
     """
 
-    def __init__(self, orig_img, path, names, boxes=None, masks=None, probs=None, keypoints=None, obb=None) -> None:
+    def __init__(
+        self, orig_img, path, names, boxes=None, masks=None, probs=None, keypoints=None, obb=None, speed=None
+    ) -> None:
         """
         Initialize the Results class.
 
         Args:
             orig_img (numpy.ndarray): The original image as a numpy array.
             path (str): The path to the image file.
             names (dict): A dictionary of class names.
@@ -111,15 +113,15 @@
         self.orig_img = orig_img
         self.orig_shape = orig_img.shape[:2]
         self.boxes = Boxes(boxes, self.orig_shape) if boxes is not None else None  # native size boxes
         self.masks = Masks(masks, self.orig_shape) if masks is not None else None  # native size or imgsz masks
         self.probs = Probs(probs) if probs is not None else None
         self.keypoints = Keypoints(keypoints, self.orig_shape) if keypoints is not None else None
         self.obb = OBB(obb, self.orig_shape) if obb is not None else None
-        self.speed = {"preprocess": None, "inference": None, "postprocess": None}  # milliseconds per image
+        self.speed = speed if speed is not None else {"preprocess": None, "inference": None, "postprocess": None}
         self.names = names
         self.path = path
         self.save_dir = None
         self._keys = "boxes", "masks", "probs", "keypoints", "obb"
 
     def __getitem__(self, idx):
         """Return a Results object for the specified index."""
@@ -176,16 +178,16 @@
         return self._apply("cuda")
 
     def to(self, *args, **kwargs):
         """Return a copy of the Results object with tensors on the specified device and dtype."""
         return self._apply("to", *args, **kwargs)
 
     def new(self):
-        """Return a new Results object with the same image, path, and names."""
-        return Results(orig_img=self.orig_img, path=self.path, names=self.names)
+        """Return a new Results object with the same image, path, names and speed."""
+        return Results(orig_img=self.orig_img, path=self.path, names=self.names, speed=self.speed)
 
     def plot(
         self,
         conf=True,
         line_width=None,
         font_size=None,
         font="Arial.ttf",
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/trainer.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,21 +523,21 @@
         return data["train"], data.get("val") or data.get("test")
 
     def setup_model(self):
         """Load/create/download model for any task."""
         if isinstance(self.model, torch.nn.Module):  # if model is loaded beforehand. No setup needed
             return
 
-        model, weights = self.model, None
+        cfg, weights = self.model, None
         ckpt = None
-        if str(model).endswith(".pt"):
-            weights, ckpt = attempt_load_one_weight(model)
+        if str(self.model).endswith(".pt"):
+            weights, ckpt = attempt_load_one_weight(self.model)
             cfg = weights.yaml
-        else:
-            cfg = model
+        elif isinstance(self.args.pretrained, (str, Path)):
+            weights, _ = attempt_load_one_weight(self.args.pretrained)
         self.model = self.get_model(cfg=cfg, weights=weights, verbose=RANK == -1)  # calls Model(cfg, weights)
         return ckpt
 
     def optimizer_step(self):
         """Perform a single step of the training optimizer with gradient clipping and EMA update."""
         self.scaler.unscale_(self.optimizer)  # unscale gradients
         torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=10.0)  # clip gradients
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/tuner.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/engine/validator.py` & `vsensebox_ultralytics-8.2.18/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/hub/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/hub/auth.py` & `vsensebox_ultralytics-8.2.18/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/hub/session.py` & `vsensebox_ultralytics-8.2.18/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/hub/utils.py` & `vsensebox_ultralytics-8.2.18/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/model.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/prompt.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/utils.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/fastsam/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/nas/model.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/nas/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/nas/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/model.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/rtdetr/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/amg.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/build.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/model.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/decoders.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/encoders.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/sam.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/tiny_encoder.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/modules/transformer.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/sam/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/utils/loss.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/utils/ops.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/classify/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/detect/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/model.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/obb/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/pose/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/predict.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/segment/val.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/models/yolo/world/train_world.py` & `vsensebox_ultralytics-8.2.18/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/autobackend.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/block.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/conv.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/head.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/transformer.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/modules/utils.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/nn/tasks.py` & `vsensebox_ultralytics-8.2.18/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/solutions/distance_calculation.py` & `vsensebox_ultralytics-8.2.18/ultralytics/solutions/distance_calculation.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,177 +5,172 @@
 import cv2
 
 from ultralytics.utils.checks import check_imshow
 from ultralytics.utils.plotting import Annotator, colors
 
 
 class DistanceCalculation:
-    """A class to calculate distance between two objects in real-time video stream based on their tracks."""
+    """A class to calculate distance between two objects in a real-time video stream based on their tracks."""
 
-    def __init__(self):
-        """Initializes the distance calculation class with default values for Visual, Image, track and distance
-        parameters.
+    def __init__(
+        self,
+        names,
+        pixels_per_meter=10,
+        view_img=False,
+        line_thickness=2,
+        line_color=(255, 255, 0),
+        centroid_color=(255, 0, 255),
+    ):
         """
+        Initializes the DistanceCalculation class with the given parameters.
 
-        # Visual & im0 information
+        Args:
+            names (dict): Dictionary mapping class indices to class names.
+            pixels_per_meter (int, optional): Conversion factor from pixels to meters. Defaults to 10.
+            view_img (bool, optional): Flag to indicate if the video stream should be displayed. Defaults to False.
+            line_thickness (int, optional): Thickness of the lines drawn on the image. Defaults to 2.
+            line_color (tuple, optional): Color of the lines drawn on the image (BGR format). Defaults to (255, 255, 0).
+            centroid_color (tuple, optional): Color of the centroids drawn (BGR format). Defaults to (255, 0, 255).
+        """
+        # Visual & image information
         self.im0 = None
         self.annotator = None
-        self.view_img = False
-        self.line_color = (255, 255, 0)
-        self.centroid_color = (255, 0, 255)
+        self.view_img = view_img
+        self.line_color = line_color
+        self.centroid_color = centroid_color
 
-        # Predict/track information
+        # Prediction & tracking information
         self.clss = None
-        self.names = None
+        self.names = names
         self.boxes = None
-        self.line_thickness = 2
+        self.line_thickness = line_thickness
         self.trk_ids = None
 
         # Distance calculation information
         self.centroids = []
-        self.pixel_per_meter = 10
+        self.pixel_per_meter = pixels_per_meter
 
-        # Mouse event
+        # Mouse event information
         self.left_mouse_count = 0
         self.selected_boxes = {}
 
-        # Check if environment support imshow
+        # Check if environment supports imshow
         self.env_check = check_imshow(warn=True)
 
-    def set_args(
-        self,
-        names,
-        pixels_per_meter=10,
-        view_img=False,
-        line_thickness=2,
-        line_color=(255, 255, 0),
-        centroid_color=(255, 0, 255),
-    ):
-        """
-        Configures the distance calculation and display parameters.
-
-        Args:
-            names (dict): object detection classes names
-            pixels_per_meter (int): Number of pixels in meter
-            view_img (bool): Flag indicating frame display
-            line_thickness (int): Line thickness for bounding boxes.
-            line_color (RGB): color of centroids line
-            centroid_color (RGB): colors of bbox centroids
-        """
-        self.names = names
-        self.pixel_per_meter = pixels_per_meter
-        self.view_img = view_img
-        self.line_thickness = line_thickness
-        self.line_color = line_color
-        self.centroid_color = centroid_color
-
     def mouse_event_for_distance(self, event, x, y, flags, param):
         """
-        This function is designed to move region with mouse events in a real-time video stream.
+        Handles mouse events to select regions in a real-time video stream.
 
         Args:
-            event (int): The type of mouse event (e.g., cv2.EVENT_MOUSEMOVE, cv2.EVENT_LBUTTONDOWN, etc.).
-            x (int): The x-coordinate of the mouse pointer.
-            y (int): The y-coordinate of the mouse pointer.
-            flags (int): Any flags associated with the event (e.g., cv2.EVENT_FLAG_CTRLKEY,
-                cv2.EVENT_FLAG_SHIFTKEY, etc.).
-            param (dict): Additional parameters you may want to pass to the function.
+            event (int): Type of mouse event (e.g., cv2.EVENT_MOUSEMOVE, cv2.EVENT_LBUTTONDOWN, etc.).
+            x (int): X-coordinate of the mouse pointer.
+            y (int): Y-coordinate of the mouse pointer.
+            flags (int): Flags associated with the event (e.g., cv2.EVENT_FLAG_CTRLKEY, cv2.EVENT_FLAG_SHIFTKEY, etc.).
+            param (dict): Additional parameters passed to the function.
         """
-        global selected_boxes
-        global left_mouse_count
         if event == cv2.EVENT_LBUTTONDOWN:
             self.left_mouse_count += 1
             if self.left_mouse_count <= 2:
                 for box, track_id in zip(self.boxes, self.trk_ids):
                     if box[0] < x < box[2] and box[1] < y < box[3] and track_id not in self.selected_boxes:
-                        self.selected_boxes[track_id] = []
                         self.selected_boxes[track_id] = box
 
-        if event == cv2.EVENT_RBUTTONDOWN:
+        elif event == cv2.EVENT_RBUTTONDOWN:
             self.selected_boxes = {}
             self.left_mouse_count = 0
 
     def extract_tracks(self, tracks):
         """
-        Extracts results from the provided data.
+        Extracts tracking results from the provided data.
 
         Args:
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.boxes = tracks[0].boxes.xyxy.cpu()
         self.clss = tracks[0].boxes.cls.cpu().tolist()
         self.trk_ids = tracks[0].boxes.id.int().cpu().tolist()
 
-    def calculate_centroid(self, box):
+    @staticmethod
+    def calculate_centroid(box):
         """
-        Calculate the centroid of bounding box.
+        Calculates the centroid of a bounding box.
 
         Args:
-            box (list): Bounding box data
+            box (list): Bounding box coordinates [x1, y1, x2, y2].
+
+        Returns:
+            (tuple): Centroid coordinates (x, y).
         """
         return int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2)
 
     def calculate_distance(self, centroid1, centroid2):
         """
-        Calculate distance between two centroids.
+        Calculates the distance between two centroids.
 
         Args:
-            centroid1 (point): First bounding box data
-            centroid2 (point): Second bounding box data
+            centroid1 (tuple): Coordinates of the first centroid (x, y).
+            centroid2 (tuple): Coordinates of the second centroid (x, y).
+
+        Returns:
+            (tuple): Distance in meters and millimeters.
         """
         pixel_distance = math.sqrt((centroid1[0] - centroid2[0]) ** 2 + (centroid1[1] - centroid2[1]) ** 2)
-        return pixel_distance / self.pixel_per_meter, (pixel_distance / self.pixel_per_meter) * 1000
+        distance_m = pixel_distance / self.pixel_per_meter
+        distance_mm = distance_m * 1000
+        return distance_m, distance_mm
 
     def start_process(self, im0, tracks):
         """
-        Calculate distance between two bounding boxes based on tracking data.
+        Processes the video frame and calculates the distance between two bounding boxes.
 
         Args:
-            im0 (nd array): Image
+            im0 (ndarray): The image frame.
             tracks (list): List of tracks obtained from the object tracking process.
+
+        Returns:
+            (ndarray): The processed image frame.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img:
                 self.display_frames()
-            return
-        self.extract_tracks(tracks)
+            return im0
 
-        self.annotator = Annotator(self.im0, line_width=2)
+        self.extract_tracks(tracks)
+        self.annotator = Annotator(self.im0, line_width=self.line_thickness)
 
         for box, cls, track_id in zip(self.boxes, self.clss, self.trk_ids):
             self.annotator.box_label(box, color=colors(int(cls), True), label=self.names[int(cls)])
 
             if len(self.selected_boxes) == 2:
-                for trk_id, _ in self.selected_boxes.items():
+                for trk_id in self.selected_boxes.keys():
                     if trk_id == track_id:
                         self.selected_boxes[track_id] = box
 
         if len(self.selected_boxes) == 2:
-            for trk_id, box in self.selected_boxes.items():
-                centroid = self.calculate_centroid(self.selected_boxes[trk_id])
-                self.centroids.append(centroid)
+            self.centroids = [self.calculate_centroid(self.selected_boxes[trk_id]) for trk_id in self.selected_boxes]
 
             distance_m, distance_mm = self.calculate_distance(self.centroids[0], self.centroids[1])
             self.annotator.plot_distance_and_line(
                 distance_m, distance_mm, self.centroids, self.line_color, self.centroid_color
             )
 
         self.centroids = []
 
         if self.view_img and self.env_check:
             self.display_frames()
 
         return im0
 
     def display_frames(self):
-        """Display frame."""
+        """Displays the current frame with annotations."""
         cv2.namedWindow("Ultralytics Distance Estimation")
         cv2.setMouseCallback("Ultralytics Distance Estimation", self.mouse_event_for_distance)
         cv2.imshow("Ultralytics Distance Estimation", self.im0)
 
         if cv2.waitKey(1) & 0xFF == ord("q"):
             return
 
 
 if __name__ == "__main__":
-    DistanceCalculation()
+    names = {0: "person", 1: "car"}  # example class names
+    distance_calculation = DistanceCalculation(names)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/solutions/heatmap.py` & `vsensebox_ultralytics-8.2.18/ultralytics/solutions/heatmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,150 +12,106 @@
 
 from shapely.geometry import LineString, Point, Polygon
 
 
 class Heatmap:
     """A class to draw heatmaps in real-time video stream based on their tracks."""
 
-    def __init__(self):
+    def __init__(
+        self,
+        classes_names,
+        imw=0,
+        imh=0,
+        colormap=cv2.COLORMAP_JET,
+        heatmap_alpha=0.5,
+        view_img=False,
+        view_in_counts=True,
+        view_out_counts=True,
+        count_reg_pts=None,
+        count_txt_color=(0, 0, 0),
+        count_bg_color=(255, 255, 255),
+        count_reg_color=(255, 0, 255),
+        region_thickness=5,
+        line_dist_thresh=15,
+        line_thickness=2,
+        decay_factor=0.99,
+        shape="circle",
+    ):
         """Initializes the heatmap class with default values for Visual, Image, track, count and heatmap parameters."""
 
         # Visual information
         self.annotator = None
-        self.view_img = False
-        self.shape = "circle"
+        self.view_img = view_img
+        self.shape = shape
 
-        self.names = None  # Classes names
+        self.initialized = False
+        self.names = classes_names  # Classes names
 
         # Image information
-        self.imw = None
-        self.imh = None
+        self.imw = imw
+        self.imh = imh
         self.im0 = None
-        self.tf = 2
-        self.view_in_counts = True
-        self.view_out_counts = True
+        self.tf = line_thickness
+        self.view_in_counts = view_in_counts
+        self.view_out_counts = view_out_counts
 
         # Heatmap colormap and heatmap np array
-        self.colormap = None
+        self.colormap = colormap
         self.heatmap = None
-        self.heatmap_alpha = 0.5
+        self.heatmap_alpha = heatmap_alpha
 
         # Predict/track information
         self.boxes = None
         self.track_ids = None
         self.clss = None
         self.track_history = defaultdict(list)
 
         # Region & Line Information
-        self.count_reg_pts = None
         self.counting_region = None
-        self.line_dist_thresh = 15
-        self.region_thickness = 5
-        self.region_color = (255, 0, 255)
+        self.line_dist_thresh = line_dist_thresh
+        self.region_thickness = region_thickness
+        self.region_color = count_reg_color
 
         # Object Counting Information
         self.in_counts = 0
         self.out_counts = 0
         self.count_ids = []
         self.class_wise_count = {}
-        self.count_txt_color = (0, 0, 0)
-        self.count_bg_color = (255, 255, 255)
+        self.count_txt_color = count_txt_color
+        self.count_bg_color = count_bg_color
         self.cls_txtdisplay_gap = 50
 
         # Decay factor
-        self.decay_factor = 0.99
+        self.decay_factor = decay_factor
 
-        # Check if environment support imshow
+        # Check if environment supports imshow
         self.env_check = check_imshow(warn=True)
 
-    def set_args(
-        self,
-        imw,
-        imh,
-        classes_names=None,
-        colormap=cv2.COLORMAP_JET,
-        heatmap_alpha=0.5,
-        view_img=False,
-        view_in_counts=True,
-        view_out_counts=True,
-        count_reg_pts=None,
-        count_txt_color=(0, 0, 0),
-        count_bg_color=(255, 255, 255),
-        count_reg_color=(255, 0, 255),
-        region_thickness=5,
-        line_dist_thresh=15,
-        line_thickness=2,
-        decay_factor=0.99,
-        shape="circle",
-    ):
-        """
-        Configures the heatmap colormap, width, height and display parameters.
-
-        Args:
-            colormap (cv2.COLORMAP): The colormap to be set.
-            imw (int): The width of the frame.
-            imh (int): The height of the frame.
-            classes_names (dict): Classes names
-            line_thickness (int): Line thickness for bounding boxes.
-            heatmap_alpha (float): alpha value for heatmap display
-            view_img (bool): Flag indicating frame display
-            view_in_counts (bool): Flag to control whether to display the incounts on video stream.
-            view_out_counts (bool): Flag to control whether to display the outcounts on video stream.
-            count_reg_pts (list): Object counting region points
-            count_txt_color (RGB color): count text color value
-            count_bg_color (RGB color): count highlighter line color
-            count_reg_color (RGB color): Color of object counting region
-            region_thickness (int): Object counting Region thickness
-            line_dist_thresh (int): Euclidean Distance threshold for line counter
-            decay_factor (float): value for removing heatmap area after object passed
-            shape (str): Heatmap shape, rect or circle shape supported
-        """
-        self.tf = line_thickness
-        self.names = classes_names
-        self.imw = imw
-        self.imh = imh
-        self.heatmap_alpha = heatmap_alpha
-        self.view_img = view_img
-        self.view_in_counts = view_in_counts
-        self.view_out_counts = view_out_counts
-        self.colormap = colormap
-
         # Region and line selection
-        if count_reg_pts is not None:
-            if len(count_reg_pts) == 2:
+        self.count_reg_pts = count_reg_pts
+        print(self.count_reg_pts)
+        if self.count_reg_pts is not None:
+            if len(self.count_reg_pts) == 2:
                 print("Line Counter Initiated.")
-                self.count_reg_pts = count_reg_pts
                 self.counting_region = LineString(self.count_reg_pts)
-            elif len(count_reg_pts) >= 3:
+            elif len(self.count_reg_pts) >= 3:
                 print("Polygon Counter Initiated.")
-                self.count_reg_pts = count_reg_pts
                 self.counting_region = Polygon(self.count_reg_pts)
             else:
                 print("Invalid Region points provided, region_points must be 2 for lines or >= 3 for polygons.")
                 print("Using Line Counter Now")
                 self.counting_region = LineString(self.count_reg_pts)
 
-        # Heatmap new frame
-        self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
-
-        self.count_txt_color = count_txt_color
-        self.count_bg_color = count_bg_color
-        self.region_color = count_reg_color
-        self.region_thickness = region_thickness
-        self.decay_factor = decay_factor
-        self.line_dist_thresh = line_dist_thresh
-        self.shape = shape
-
-        # shape of heatmap, if not selected
+        # Shape of heatmap, if not selected
         if self.shape not in {"circle", "rect"}:
             print("Unknown shape value provided, 'circle' & 'rect' supported")
             print("Using Circular shape now")
             self.shape = "circle"
 
-    def extract_results(self, tracks):
+    def extract_results(self, tracks, _intialized=False):
         """
         Extracts results from the provided data.
 
         Args:
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.boxes = tracks[0].boxes.xyxy.cpu()
@@ -167,26 +123,28 @@
         Generate heatmap based on tracking data.
 
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0
-        if tracks[0].boxes.id is None:
-            self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
-            if self.view_img and self.env_check:
-                self.display_frames()
-            return im0
+
+        # Initialize heatmap only once
+        if not self.initialized:
+            self.heatmap = np.zeros((int(self.im0.shape[0]), int(self.im0.shape[1])), dtype=np.float32)
+            self.initialized = True
+
         self.heatmap *= self.decay_factor  # decay factor
+
         self.extract_results(tracks)
         self.annotator = Annotator(self.im0, self.tf, None)
 
-        if self.count_reg_pts is not None:
+        if self.track_ids is not None:
             # Draw counting region
-            if self.view_in_counts or self.view_out_counts:
+            if self.count_reg_pts is not None:
                 self.annotator.draw_region(
                     reg_pts=self.count_reg_pts, color=self.region_color, thickness=self.region_thickness
                 )
 
             for box, cls, track_id in zip(self.boxes, self.clss, self.track_ids):
                 # Store class info
                 if self.names[cls] not in self.class_wise_count:
@@ -210,42 +168,45 @@
                 track_line = self.track_history[track_id]
                 track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
                 if len(track_line) > 30:
                     track_line.pop(0)
 
                 prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
 
-                # Count objects in any polygon
-                if len(self.count_reg_pts) >= 3:
-                    is_inside = self.counting_region.contains(Point(track_line[-1]))
-
-                    if prev_position is not None and is_inside and track_id not in self.count_ids:
-                        self.count_ids.append(track_id)
-
-                        if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
-                            self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["IN"] += 1
-                        else:
-                            self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["OUT"] += 1
-
-                # Count objects using line
-                elif len(self.count_reg_pts) == 2:
-                    if prev_position is not None and track_id not in self.count_ids:
-                        distance = Point(track_line[-1]).distance(self.counting_region)
-                        if distance < self.line_dist_thresh and track_id not in self.count_ids:
+                if self.count_reg_pts is not None:
+                    # Count objects in any polygon
+                    if len(self.count_reg_pts) >= 3:
+                        is_inside = self.counting_region.contains(Point(track_line[-1]))
+
+                        if prev_position is not None and is_inside and track_id not in self.count_ids:
                             self.count_ids.append(track_id)
 
                             if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                                 self.in_counts += 1
                                 self.class_wise_count[self.names[cls]]["IN"] += 1
                             else:
                                 self.out_counts += 1
                                 self.class_wise_count[self.names[cls]]["OUT"] += 1
 
+                    # Count objects using line
+                    elif len(self.count_reg_pts) == 2:
+                        if prev_position is not None and track_id not in self.count_ids:
+                            distance = Point(track_line[-1]).distance(self.counting_region)
+                            if distance < self.line_dist_thresh and track_id not in self.count_ids:
+                                self.count_ids.append(track_id)
+
+                                if (box[0] - prev_position[0]) * (
+                                    self.counting_region.centroid.x - prev_position[0]
+                                ) > 0:
+                                    self.in_counts += 1
+                                    self.class_wise_count[self.names[cls]]["IN"] += 1
+                                else:
+                                    self.out_counts += 1
+                                    self.class_wise_count[self.names[cls]]["OUT"] += 1
+
         else:
             for box, cls in zip(self.boxes, self.clss):
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
@@ -254,34 +215,34 @@
                     self.heatmap[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])] += (
                         2 * mask[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])]
                     )
 
                 else:
                     self.heatmap[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])] += 2
 
-        # Normalize, apply colormap to heatmap and combine with original image
-        heatmap_normalized = cv2.normalize(self.heatmap, None, 0, 255, cv2.NORM_MINMAX)
-        heatmap_colored = cv2.applyColorMap(heatmap_normalized.astype(np.uint8), self.colormap)
-
-        labels_dict = {}
+        if self.count_reg_pts is not None:
+            labels_dict = {}
 
-        for key, value in self.class_wise_count.items():
-            if value["IN"] != 0 or value["OUT"] != 0:
-                if not self.view_in_counts and not self.view_out_counts:
-                    continue
-                elif not self.view_in_counts:
-                    labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
-                elif not self.view_out_counts:
-                    labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
-                else:
-                    labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
+            for key, value in self.class_wise_count.items():
+                if value["IN"] != 0 or value["OUT"] != 0:
+                    if not self.view_in_counts and not self.view_out_counts:
+                        continue
+                    elif not self.view_in_counts:
+                        labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
+                    elif not self.view_out_counts:
+                        labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
+                    else:
+                        labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
 
-        if labels_dict is not None:
-            self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
+            if labels_dict is not None:
+                self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
 
+        # Normalize, apply colormap to heatmap and combine with original image
+        heatmap_normalized = cv2.normalize(self.heatmap, None, 0, 255, cv2.NORM_MINMAX)
+        heatmap_colored = cv2.applyColorMap(heatmap_normalized.astype(np.uint8), self.colormap)
         self.im0 = cv2.addWeighted(self.im0, 1 - self.heatmap_alpha, heatmap_colored, self.heatmap_alpha, 0)
 
         if self.env_check and self.view_img:
             self.display_frames()
 
         return self.im0
 
@@ -290,8 +251,9 @@
         cv2.imshow("Ultralytics Heatmap", self.im0)
 
         if cv2.waitKey(1) & 0xFF == ord("q"):
             return
 
 
 if __name__ == "__main__":
-    Heatmap()
+    classes_names = {0: "person", 1: "car"}  # example class names
+    heatmap = Heatmap(classes_names)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/solutions/object_counter.py` & `vsensebox_ultralytics-8.2.18/ultralytics/solutions/object_counter.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,63 +11,18 @@
 
 from shapely.geometry import LineString, Point, Polygon
 
 
 class ObjectCounter:
     """A class to manage the counting of objects in a real-time video stream based on their tracks."""
 
-    def __init__(self):
-        """Initializes the Counter with default values for various tracking and counting parameters."""
-
-        # Mouse events
-        self.is_drawing = False
-        self.selected_point = None
-
-        # Region & Line Information
-        self.reg_pts = [(20, 400), (1260, 400)]
-        self.line_dist_thresh = 15
-        self.counting_region = None
-        self.region_color = (255, 0, 255)
-        self.region_thickness = 5
-
-        # Image and annotation Information
-        self.im0 = None
-        self.tf = None
-        self.view_img = False
-        self.view_in_counts = True
-        self.view_out_counts = True
-
-        self.names = None  # Classes names
-        self.annotator = None  # Annotator
-        self.window_name = "Ultralytics YOLOv8 Object Counter"
-
-        # Object counting Information
-        self.in_counts = 0
-        self.out_counts = 0
-        self.count_ids = []
-        self.class_wise_count = {}
-        self.count_txt_thickness = 0
-        self.count_txt_color = (255, 255, 255)
-        self.count_bg_color = (255, 255, 255)
-        self.cls_txtdisplay_gap = 50
-        self.fontsize = 0.6
-
-        # Tracks info
-        self.track_history = defaultdict(list)
-        self.track_thickness = 2
-        self.draw_tracks = False
-        self.track_color = None
-
-        # Check if environment support imshow
-        self.env_check = check_imshow(warn=True)
-
-    def set_args(
+    def __init__(
         self,
         classes_names,
-        reg_pts,
+        reg_pts=None,
         count_reg_color=(255, 0, 255),
         count_txt_color=(0, 0, 0),
         count_bg_color=(255, 255, 255),
         line_thickness=2,
         track_thickness=2,
         view_img=False,
         view_in_counts=True,
@@ -75,74 +30,98 @@
         draw_tracks=False,
         track_color=None,
         region_thickness=5,
         line_dist_thresh=15,
         cls_txtdisplay_gap=50,
     ):
         """
-        Configures the Counter's image, bounding box line thickness, and counting region points.
+        Initializes the ObjectCounter with various tracking and counting parameters.
 
         Args:
+            classes_names (dict): Dictionary of class names.
+            reg_pts (list): List of points defining the counting region.
+            count_reg_color (tuple): RGB color of the counting region.
+            count_txt_color (tuple): RGB color of the count text.
+            count_bg_color (tuple): RGB color of the count text background.
             line_thickness (int): Line thickness for bounding boxes.
+            track_thickness (int): Thickness of the track lines.
             view_img (bool): Flag to control whether to display the video stream.
-            view_in_counts (bool): Flag to control whether to display the incounts on video stream.
-            view_out_counts (bool): Flag to control whether to display the outcounts on video stream.
-            reg_pts (list): Initial list of points defining the counting region.
-            classes_names (dict): Classes names
-            track_thickness (int): Track thickness
-            draw_tracks (Bool): draw tracks
-            count_txt_color (RGB color): count text color value
-            count_bg_color (RGB color): count highlighter line color
-            count_reg_color (RGB color): Color of object counting region
-            track_color (RGB color): color for tracks
-            region_thickness (int): Object counting Region thickness
-            line_dist_thresh (int): Euclidean Distance threshold for line counter
-            cls_txtdisplay_gap (int): Display gap between each class count
+            view_in_counts (bool): Flag to control whether to display the in counts on the video stream.
+            view_out_counts (bool): Flag to control whether to display the out counts on the video stream.
+            draw_tracks (bool): Flag to control whether to draw the object tracks.
+            track_color (tuple): RGB color of the tracks.
+            region_thickness (int): Thickness of the object counting region.
+            line_dist_thresh (int): Euclidean distance threshold for line counter.
+            cls_txtdisplay_gap (int): Display gap between each class count.
         """
+
+        # Mouse events
+        self.is_drawing = False
+        self.selected_point = None
+
+        # Region & Line Information
+        self.reg_pts = [(20, 400), (1260, 400)] if reg_pts is None else reg_pts
+        self.line_dist_thresh = line_dist_thresh
+        self.counting_region = None
+        self.region_color = count_reg_color
+        self.region_thickness = region_thickness
+
+        # Image and annotation Information
+        self.im0 = None
         self.tf = line_thickness
         self.view_img = view_img
         self.view_in_counts = view_in_counts
         self.view_out_counts = view_out_counts
+
+        self.names = classes_names  # Classes names
+        self.annotator = None  # Annotator
+        self.window_name = "Ultralytics YOLOv8 Object Counter"
+
+        # Object counting Information
+        self.in_counts = 0
+        self.out_counts = 0
+        self.count_ids = []
+        self.class_wise_count = {}
+        self.count_txt_thickness = 0
+        self.count_txt_color = count_txt_color
+        self.count_bg_color = count_bg_color
+        self.cls_txtdisplay_gap = cls_txtdisplay_gap
+        self.fontsize = 0.6
+
+        # Tracks info
+        self.track_history = defaultdict(list)
         self.track_thickness = track_thickness
         self.draw_tracks = draw_tracks
+        self.track_color = track_color
+
+        # Check if environment supports imshow
+        self.env_check = check_imshow(warn=True)
 
-        # Region and line selection
-        if len(reg_pts) == 2:
+        # Initialize counting region
+        if len(self.reg_pts) == 2:
             print("Line Counter Initiated.")
-            self.reg_pts = reg_pts
             self.counting_region = LineString(self.reg_pts)
-        elif len(reg_pts) >= 3:
+        elif len(self.reg_pts) >= 3:
             print("Polygon Counter Initiated.")
-            self.reg_pts = reg_pts
             self.counting_region = Polygon(self.reg_pts)
         else:
             print("Invalid Region points provided, region_points must be 2 for lines or >= 3 for polygons.")
             print("Using Line Counter Now")
             self.counting_region = LineString(self.reg_pts)
 
-        self.names = classes_names
-        self.track_color = track_color
-        self.count_txt_color = count_txt_color
-        self.count_bg_color = count_bg_color
-        self.region_color = count_reg_color
-        self.region_thickness = region_thickness
-        self.line_dist_thresh = line_dist_thresh
-        self.cls_txtdisplay_gap = cls_txtdisplay_gap
-
     def mouse_event_for_region(self, event, x, y, flags, params):
         """
-        This function is designed to move region with mouse events in a real-time video stream.
+        Handles mouse events for defining and moving the counting region in a real-time video stream.
 
         Args:
             event (int): The type of mouse event (e.g., cv2.EVENT_MOUSEMOVE, cv2.EVENT_LBUTTONDOWN, etc.).
             x (int): The x-coordinate of the mouse pointer.
             y (int): The y-coordinate of the mouse pointer.
-            flags (int): Any flags associated with the event (e.g., cv2.EVENT_FLAG_CTRLKEY,
-                cv2.EVENT_FLAG_SHIFTKEY, etc.).
-            params (dict): Additional parameters you may want to pass to the function.
+            flags (int): Any associated event flags (e.g., cv2.EVENT_FLAG_CTRLKEY,  cv2.EVENT_FLAG_SHIFTKEY, etc.).
+            params (dict): Additional parameters for the function.
         """
         if event == cv2.EVENT_LBUTTONDOWN:
             for i, point in enumerate(self.reg_pts):
                 if (
                     isinstance(point, (tuple, list))
                     and len(point) >= 2
                     and (abs(x - point[0]) < 10 and abs(y - point[1]) < 10)
@@ -236,19 +215,19 @@
                 elif not self.view_in_counts:
                     labels_dict[str.capitalize(key)] = f"OUT {value['OUT']}"
                 elif not self.view_out_counts:
                     labels_dict[str.capitalize(key)] = f"IN {value['IN']}"
                 else:
                     labels_dict[str.capitalize(key)] = f"IN {value['IN']} OUT {value['OUT']}"
 
-        if labels_dict is not None:
+        if labels_dict:
             self.annotator.display_analytics(self.im0, labels_dict, self.count_txt_color, self.count_bg_color, 10)
 
     def display_frames(self):
-        """Display frame."""
+        """Displays the current frame with annotations and regions in a window."""
         if self.env_check:
             cv2.namedWindow(self.window_name)
             if len(self.reg_pts) == 4:  # only add mouse event If user drawn region
                 cv2.setMouseCallback(self.window_name, self.mouse_event_for_region, {"region_points": self.reg_pts})
             cv2.imshow(self.window_name, self.im0)
             # Break Window
             if cv2.waitKey(1) & 0xFF == ord("q"):
@@ -267,8 +246,9 @@
 
         if self.view_img:
             self.display_frames()
         return self.im0
 
 
 if __name__ == "__main__":
-    ObjectCounter()
+    classes_names = {0: "person", 1: "car"}  # example class names
+    ObjectCounter(classes_names)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/solutions/parking_management.py` & `vsensebox_ultralytics-8.2.18/ultralytics/solutions/parking_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,30 @@
 import cv2
 import numpy as np
 from PIL import Image, ImageTk
 
 from ultralytics.utils.checks import check_imshow, check_requirements
 from ultralytics.utils.plotting import Annotator
 
-check_requirements("tkinter")
-import tkinter as tk
-
 
 class ParkingPtsSelection:
     def __init__(self, master):
-        """Initializes the UI for selecting parking zone points in a tkinter window."""
+        """
+        Initializes the UI for selecting parking zone points in a tkinter window.
+
+        Args:
+            master (tk.Tk): The main tkinter window object.
+        """
+        check_requirements("tkinter")
+        import tkinter as tk
+
         self.master = master
         master.title("Ultralytics Parking Zones Points Selector")
 
-        # Resizable false
+        # Disable window resizing
         master.resizable(False, False)
 
         # Setup canvas for image display
         self.canvas = tk.Canvas(master, bg="white")
 
         # Setup buttons
         button_frame = tk.Frame(master)
@@ -32,15 +37,14 @@
         tk.Button(button_frame, text="Remove Last BBox", command=self.remove_last_bounding_box).grid(row=0, column=1)
         tk.Button(button_frame, text="Save", command=self.save_to_json).grid(row=0, column=2)
 
         # Initialize properties
         self.image_path = None
         self.image = None
         self.canvas_image = None
-        self.canvas = None
         self.bounding_boxes = []
         self.current_box = []
         self.img_width = 0
         self.img_height = 0
 
         # Constants
         self.canvas_max_width = 1280
@@ -97,15 +101,14 @@
     def draw_bounding_box(self, box):
         """
         Draw bounding box on canvas.
 
         Args:
             box (list): Bounding box data
         """
-
         for i in range(4):
             x1, y1 = box[i]
             x2, y2 = box[(i + 1) % 4]
             self.canvas.create_line(x1, y1, x2, y2, fill="blue", width=2)
 
     def remove_last_bounding_box(self):
         """Remove the last drawn bounding box from canvas."""
@@ -147,14 +150,25 @@
         model_path,
         txt_color=(0, 0, 0),
         bg_color=(255, 255, 255),
         occupied_region_color=(0, 255, 0),
         available_region_color=(0, 0, 255),
         margin=10,
     ):
+        """
+        Initializes the parking management system with a YOLOv8 model and visualization settings.
+
+        Args:
+            model_path (str): Path to the YOLOv8 model.
+            txt_color (tuple): RGB color tuple for text.
+            bg_color (tuple): RGB color tuple for background.
+            occupied_region_color (tuple): RGB color tuple for occupied regions.
+            available_region_color (tuple): RGB color tuple for available regions.
+            margin (int): Margin for text display.
+        """
         # Model path and initialization
         self.model_path = model_path
         self.model = self.load_model()
 
         # Labels dictionary
         self.labels_dict = {"Occupancy": 0, "Available": 0}
 
@@ -162,15 +176,15 @@
         self.margin = margin
         self.bg_color = bg_color
         self.txt_color = txt_color
         self.occupied_region_color = occupied_region_color
         self.available_region_color = available_region_color
 
         self.window_name = "Ultralytics YOLOv8 Parking Management System"
-        # Check if environment support imshow
+        # Check if environment supports imshow
         self.env_check = check_imshow(warn=True)
 
     def load_model(self):
         """Load the Ultralytics YOLOv8 model for inference and analytics."""
         from ultralytics import YOLO
 
         self.model = YOLO(self.model_path)
@@ -180,15 +194,14 @@
     def parking_regions_extraction(json_file):
         """
         Extract parking regions from json file.
 
         Args:
             json_file (str): file that have all parking slot points
         """
-
         with open(json_file, "r") as json_file:
             return json.load(json_file)
 
     def process_data(self, json_data, im0, boxes, clss):
         """
         Process the model data for parking lot management.
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/solutions/queue_management.py` & `vsensebox_ultralytics-8.2.18/ultralytics/solutions/queue_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,179 +9,160 @@
 
 check_requirements("shapely>=2.0.0")
 
 from shapely.geometry import Point, Polygon
 
 
 class QueueManager:
-    """A class to manage the queue management in real-time video stream based on their tracks."""
+    """A class to manage the queue in a real-time video stream based on object tracks."""
 
-    def __init__(self):
-        """Initializes the queue manager with default values for various tracking and counting parameters."""
-
-        # Mouse events
-        self.is_drawing = False
-        self.selected_point = None
-
-        # Region & Line Information
-        self.reg_pts = [(20, 60), (20, 680), (1120, 680), (1120, 60)]
-        self.counting_region = None
-        self.region_color = (255, 0, 255)
-        self.region_thickness = 5
-
-        # Image and annotation Information
-        self.im0 = None
-        self.tf = None
-        self.view_img = False
-        self.view_queue_counts = True
-        self.fontsize = 0.6
-
-        self.names = None  # Classes names
-        self.annotator = None  # Annotator
-        self.window_name = "Ultralytics YOLOv8 Queue Manager"
-
-        # Object counting Information
-        self.counts = 0
-        self.count_txt_color = (255, 255, 255)
-
-        # Tracks info
-        self.track_history = defaultdict(list)
-        self.track_thickness = 2
-        self.draw_tracks = False
-        self.track_color = None
-
-        # Check if environment support imshow
-        self.env_check = check_imshow(warn=True)
-
-    def set_args(
+    def __init__(
         self,
         classes_names,
-        reg_pts,
+        reg_pts=None,
         line_thickness=2,
         track_thickness=2,
         view_img=False,
         region_color=(255, 0, 255),
         view_queue_counts=True,
         draw_tracks=False,
         count_txt_color=(255, 255, 255),
         track_color=None,
         region_thickness=5,
         fontsize=0.7,
     ):
         """
-        Configures the Counter's image, bounding box line thickness, and counting region points.
+        Initializes the QueueManager with specified parameters for tracking and counting objects.
 
         Args:
-            line_thickness (int): Line thickness for bounding boxes.
-            view_img (bool): Flag to control whether to display the video stream.
-            view_queue_counts (bool): Flag to control whether to display the counts on video stream.
-            reg_pts (list): Initial list of points defining the counting region.
-            classes_names (dict): Classes names
-            region_color (RGB color): Color of queue region
-            track_thickness (int): Track thickness
-            draw_tracks (Bool): draw tracks
-            count_txt_color (RGB color): count text color value
-            track_color (RGB color): color for tracks
-            region_thickness (int): Object counting Region thickness
-            fontsize (float): Text display font size
+            classes_names (dict): A dictionary mapping class IDs to class names.
+            reg_pts (list of tuples, optional): Points defining the counting region polygon. Defaults to a predefined
+                rectangle.
+            line_thickness (int, optional): Thickness of the annotation lines. Defaults to 2.
+            track_thickness (int, optional): Thickness of the track lines. Defaults to 2.
+            view_img (bool, optional): Whether to display the image frames. Defaults to False.
+            region_color (tuple, optional): Color of the counting region lines (BGR). Defaults to (255, 0, 255).
+            view_queue_counts (bool, optional): Whether to display the queue counts. Defaults to True.
+            draw_tracks (bool, optional): Whether to draw tracks of the objects. Defaults to False.
+            count_txt_color (tuple, optional): Color of the count text (BGR). Defaults to (255, 255, 255).
+            track_color (tuple, optional): Color of the tracks. If None, different colors will be used for different
+                tracks. Defaults to None.
+            region_thickness (int, optional): Thickness of the counting region lines. Defaults to 5.
+            fontsize (float, optional): Font size for the text annotations. Defaults to 0.7.
         """
+
+        # Mouse events state
+        self.is_drawing = False
+        self.selected_point = None
+
+        # Region & Line Information
+        self.reg_pts = reg_pts if reg_pts is not None else [(20, 60), (20, 680), (1120, 680), (1120, 60)]
+        self.counting_region = (
+            Polygon(self.reg_pts) if len(self.reg_pts) >= 3 else Polygon([(20, 60), (20, 680), (1120, 680), (1120, 60)])
+        )
+        self.region_color = region_color
+        self.region_thickness = region_thickness
+
+        # Image and annotation Information
+        self.im0 = None
         self.tf = line_thickness
         self.view_img = view_img
         self.view_queue_counts = view_queue_counts
-        self.track_thickness = track_thickness
-        self.draw_tracks = draw_tracks
-        self.region_color = region_color
+        self.fontsize = fontsize
 
-        if len(reg_pts) >= 3:
-            print("Queue region initiated...")
-            self.reg_pts = reg_pts
-            self.counting_region = Polygon(self.reg_pts)
-        else:
-            print("Invalid region points provided...")
-            print("Using default region now....")
-            self.counting_region = Polygon(self.reg_pts)
+        self.names = classes_names  # Class names
+        self.annotator = None  # Annotator
+        self.window_name = "Ultralytics YOLOv8 Queue Manager"
 
-        self.names = classes_names
-        self.track_color = track_color
+        # Object counting Information
+        self.counts = 0
         self.count_txt_color = count_txt_color
-        self.region_thickness = region_thickness
-        self.fontsize = fontsize
+
+        # Tracks info
+        self.track_history = defaultdict(list)
+        self.track_thickness = track_thickness
+        self.draw_tracks = draw_tracks
+        self.track_color = track_color
+
+        # Check if environment supports imshow
+        self.env_check = check_imshow(warn=True)
 
     def extract_and_process_tracks(self, tracks):
         """Extracts and processes tracks for queue management in a video stream."""
 
-        # Annotator Init and queue region drawing
+        # Initialize annotator and draw the queue region
         self.annotator = Annotator(self.im0, self.tf, self.names)
 
         if tracks[0].boxes.id is not None:
             boxes = tracks[0].boxes.xyxy.cpu()
             clss = tracks[0].boxes.cls.cpu().tolist()
             track_ids = tracks[0].boxes.id.int().cpu().tolist()
 
             # Extract tracks
             for box, track_id, cls in zip(boxes, track_ids, clss):
                 # Draw bounding box
                 self.annotator.box_label(box, label=f"{self.names[cls]}#{track_id}", color=colors(int(track_id), True))
 
-                # Draw Tracks
+                # Update track history
                 track_line = self.track_history[track_id]
                 track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
                 if len(track_line) > 30:
                     track_line.pop(0)
 
-                # Draw track trails
+                # Draw track trails if enabled
                 if self.draw_tracks:
                     self.annotator.draw_centroid_and_tracks(
                         track_line,
-                        color=self.track_color if self.track_color else colors(int(track_id), True),
+                        color=self.track_color or colors(int(track_id), True),
                         track_thickness=self.track_thickness,
                     )
 
                 prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
 
+                # Check if the object is inside the counting region
                 if len(self.reg_pts) >= 3:
                     is_inside = self.counting_region.contains(Point(track_line[-1]))
                     if prev_position is not None and is_inside:
                         self.counts += 1
 
-        label = "Queue Counts : " + str(self.counts)
-
+        # Display queue counts
+        label = f"Queue Counts : {str(self.counts)}"
         if label is not None:
             self.annotator.queue_counts_display(
                 label,
                 points=self.reg_pts,
                 region_color=self.region_color,
                 txt_color=self.count_txt_color,
-                fontsize=self.fontsize,
             )
 
-        self.counts = 0
+        self.counts = 0  # Reset counts after displaying
         self.display_frames()
 
     def display_frames(self):
-        """Display frame."""
+        """Displays the current frame with annotations."""
         if self.env_check:
             self.annotator.draw_region(reg_pts=self.reg_pts, thickness=self.region_thickness, color=self.region_color)
             cv2.namedWindow(self.window_name)
             cv2.imshow(self.window_name, self.im0)
-            # Break Window
+            # Close window on 'q' key press
             if cv2.waitKey(1) & 0xFF == ord("q"):
                 return
 
     def process_queue(self, im0, tracks):
         """
         Main function to start the queue management process.
 
         Args:
             im0 (ndarray): Current frame from the video stream.
             tracks (list): List of tracks obtained from the object tracking process.
         """
-        self.im0 = im0  # store image
-        self.extract_and_process_tracks(tracks)  # draw region even if no objects
+        self.im0 = im0  # Store the current frame
+        self.extract_and_process_tracks(tracks)  # Extract and process tracks
 
         if self.view_img:
-            self.display_frames()
+            self.display_frames()  # Display the frame if enabled
         return self.im0
 
 
 if __name__ == "__main__":
-    QueueManager()
+    classes_names = {0: "person", 1: "car"}  # example class names
+    queue_manager = QueueManager(classes_names)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/solutions/speed_estimation.py` & `vsensebox_ultralytics-8.2.18/ultralytics/solutions/speed_estimation.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,174 +7,155 @@
 import numpy as np
 
 from ultralytics.utils.checks import check_imshow
 from ultralytics.utils.plotting import Annotator, colors
 
 
 class SpeedEstimator:
-    """A class to estimation speed of objects in real-time video stream based on their tracks."""
+    """A class to estimate the speed of objects in a real-time video stream based on their tracks."""
 
-    def __init__(self):
-        """Initializes the speed-estimator class with default values for Visual, Image, track and speed parameters."""
+    def __init__(self, names, reg_pts=None, view_img=False, line_thickness=2, region_thickness=5, spdl_dist_thresh=10):
+        """
+        Initializes the SpeedEstimator with the given parameters.
 
-        # Visual & im0 information
+        Args:
+            names (dict): Dictionary of class names.
+            reg_pts (list, optional): List of region points for speed estimation. Defaults to [(20, 400), (1260, 400)].
+            view_img (bool, optional): Whether to display the image with annotations. Defaults to False.
+            line_thickness (int, optional): Thickness of the lines for drawing boxes and tracks. Defaults to 2.
+            region_thickness (int, optional): Thickness of the region lines. Defaults to 5.
+            spdl_dist_thresh (int, optional): Distance threshold for speed calculation. Defaults to 10.
+        """
+        # Visual & image information
         self.im0 = None
         self.annotator = None
-        self.view_img = False
+        self.view_img = view_img
 
         # Region information
-        self.reg_pts = [(20, 400), (1260, 400)]
-        self.region_thickness = 3
+        self.reg_pts = reg_pts if reg_pts is not None else [(20, 400), (1260, 400)]
+        self.region_thickness = region_thickness
 
-        # Predict/track information
+        # Tracking information
         self.clss = None
-        self.names = None
+        self.names = names
         self.boxes = None
         self.trk_ids = None
         self.trk_pts = None
-        self.line_thickness = 2
+        self.line_thickness = line_thickness
         self.trk_history = defaultdict(list)
 
-        # Speed estimator information
+        # Speed estimation information
         self.current_time = 0
         self.dist_data = {}
         self.trk_idslist = []
-        self.spdl_dist_thresh = 10
+        self.spdl_dist_thresh = spdl_dist_thresh
         self.trk_previous_times = {}
         self.trk_previous_points = {}
 
-        # Check if environment support imshow
+        # Check if the environment supports imshow
         self.env_check = check_imshow(warn=True)
 
-    def set_args(
-        self,
-        reg_pts,
-        names,
-        view_img=False,
-        line_thickness=2,
-        region_thickness=5,
-        spdl_dist_thresh=10,
-    ):
-        """
-        Configures the speed estimation and display parameters.
-
-        Args:
-            reg_pts (list): Initial list of points defining the speed calculation region.
-            names (dict): object detection classes names
-            view_img (bool): Flag indicating frame display
-            line_thickness (int): Line thickness for bounding boxes.
-            region_thickness (int): Speed estimation region thickness
-            spdl_dist_thresh (int): Euclidean distance threshold for speed line
-        """
-        if reg_pts is None:
-            print("Region points not provided, using default values")
-        else:
-            self.reg_pts = reg_pts
-        self.names = names
-        self.view_img = view_img
-        self.line_thickness = line_thickness
-        self.region_thickness = region_thickness
-        self.spdl_dist_thresh = spdl_dist_thresh
-
     def extract_tracks(self, tracks):
         """
-        Extracts results from the provided data.
+        Extracts results from the provided tracking data.
 
         Args:
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.boxes = tracks[0].boxes.xyxy.cpu()
         self.clss = tracks[0].boxes.cls.cpu().tolist()
         self.trk_ids = tracks[0].boxes.id.int().cpu().tolist()
 
     def store_track_info(self, track_id, box):
         """
-        Store track data.
+        Stores track data.
 
         Args:
-            track_id (int): object track id.
-            box (list): object bounding box data
+            track_id (int): Object track id.
+            box (list): Object bounding box data.
+
+        Returns:
+            (list): Updated tracking history for the given track_id.
         """
         track = self.trk_history[track_id]
         bbox_center = (float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2))
         track.append(bbox_center)
 
         if len(track) > 30:
             track.pop(0)
 
         self.trk_pts = np.hstack(track).astype(np.int32).reshape((-1, 1, 2))
         return track
 
     def plot_box_and_track(self, track_id, box, cls, track):
         """
-        Plot track and bounding box.
+        Plots track and bounding box.
 
         Args:
-            track_id (int): object track id.
-            box (list): object bounding box data
-            cls (str): object class name
-            track (list): tracking history for tracks path drawing
+            track_id (int): Object track id.
+            box (list): Object bounding box data.
+            cls (str): Object class name.
+            track (list): Tracking history for drawing tracks path.
         """
-        speed_label = f"{int(self.dist_data[track_id])}km/ph" if track_id in self.dist_data else self.names[int(cls)]
+        speed_label = f"{int(self.dist_data[track_id])} km/h" if track_id in self.dist_data else self.names[int(cls)]
         bbox_color = colors(int(track_id)) if track_id in self.dist_data else (255, 0, 255)
 
         self.annotator.box_label(box, speed_label, bbox_color)
-
         cv2.polylines(self.im0, [self.trk_pts], isClosed=False, color=(0, 255, 0), thickness=1)
         cv2.circle(self.im0, (int(track[-1][0]), int(track[-1][1])), 5, bbox_color, -1)
 
     def calculate_speed(self, trk_id, track):
         """
-        Calculation of object speed.
+        Calculates the speed of an object.
 
         Args:
-            trk_id (int): object track id.
-            track (list): tracking history for tracks path drawing
+            trk_id (int): Object track id.
+            track (list): Tracking history for drawing tracks path.
         """
-
         if not self.reg_pts[0][0] < track[-1][0] < self.reg_pts[1][0]:
             return
         if self.reg_pts[1][1] - self.spdl_dist_thresh < track[-1][1] < self.reg_pts[1][1] + self.spdl_dist_thresh:
             direction = "known"
-
         elif self.reg_pts[0][1] - self.spdl_dist_thresh < track[-1][1] < self.reg_pts[0][1] + self.spdl_dist_thresh:
             direction = "known"
-
         else:
             direction = "unknown"
 
-        if self.trk_previous_times[trk_id] != 0 and direction != "unknown" and trk_id not in self.trk_idslist:
+        if self.trk_previous_times.get(trk_id) != 0 and direction != "unknown" and trk_id not in self.trk_idslist:
             self.trk_idslist.append(trk_id)
 
             time_difference = time() - self.trk_previous_times[trk_id]
             if time_difference > 0:
                 dist_difference = np.abs(track[-1][1] - self.trk_previous_points[trk_id][1])
                 speed = dist_difference / time_difference
                 self.dist_data[trk_id] = speed
 
         self.trk_previous_times[trk_id] = time()
         self.trk_previous_points[trk_id] = track[-1]
 
     def estimate_speed(self, im0, tracks, region_color=(255, 0, 0)):
         """
-        Calculate object based on tracking data.
+        Estimates the speed of objects based on tracking data.
 
         Args:
-            im0 (nd array): Image
+            im0 (ndarray): Image.
             tracks (list): List of tracks obtained from the object tracking process.
-            region_color (tuple): Color to use when drawing regions.
+            region_color (tuple, optional): Color to use when drawing regions. Defaults to (255, 0, 0).
+
+        Returns:
+            (ndarray): The image with annotated boxes and tracks.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img and self.env_check:
                 self.display_frames()
             return im0
-        self.extract_tracks(tracks)
 
-        self.annotator = Annotator(self.im0, line_width=2)
+        self.extract_tracks(tracks)
+        self.annotator = Annotator(self.im0, line_width=self.line_thickness)
         self.annotator.draw_region(reg_pts=self.reg_pts, color=region_color, thickness=self.region_thickness)
 
         for box, trk_id, cls in zip(self.boxes, self.trk_ids, self.clss):
             track = self.store_track_info(trk_id, box)
 
             if trk_id not in self.trk_previous_times:
                 self.trk_previous_times[trk_id] = 0
@@ -184,15 +165,16 @@
 
         if self.view_img and self.env_check:
             self.display_frames()
 
         return im0
 
     def display_frames(self):
-        """Display frame."""
+        """Displays the current frame."""
         cv2.imshow("Ultralytics Speed Estimation", self.im0)
         if cv2.waitKey(1) & 0xFF == ord("q"):
             return
 
 
 if __name__ == "__main__":
-    SpeedEstimator()
+    names = {0: "person", 1: "car"}  # example class names
+    speed_estimator = SpeedEstimator(names)
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/basetrack.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/bot_sort.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/byte_tracker.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/track.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/gmc.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/kalman_filter.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/trackers/utils/matching.py` & `vsensebox_ultralytics-8.2.18/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/__init__.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,15 @@
         (bool): True if connection is successful, False otherwise.
     """
     with contextlib.suppress(Exception):
         assert str(os.getenv("YOLO_OFFLINE", "")).lower() != "true"  # check if ENV var YOLO_OFFLINE="True"
         import socket
 
         for dns in ("1.1.1.1", "8.8.8.8"):  # check Cloudflare and Google DNS
-            socket.create_connection(address=(dns, 80), timeout=1.0).close()
+            socket.create_connection(address=(dns, 80), timeout=2.0).close()
             return True
     return False
 
 
 def is_pip_package(filepath: str = __name__) -> bool:
     """
     Determines if the file at the given filepath is part of a pip package.
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/autobatch.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/benchmarks.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/base.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/clearml.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/comet.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/dvc.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/hub.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/mlflow.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/neptune.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/raytune.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/tensorboard.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/callbacks/wb.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/callbacks/wb.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             y_log.extend(np.interp(x_new, x, yi))  # interpolate y to new x
             classes.extend([names[i]] * len(x_new))  # add class names
         wb.log({id: _custom_table(x_log, y_log, classes, title, x_title, y_title)}, commit=False)
 
 
 def _log_plots(plots, step):
     """Logs plots from the input dictionary if they haven't been logged already at the specified step."""
-    for name, params in plots.items():
+    for name, params in plots.copy().items():  # shallow copy to prevent plots dict changing during iteration
         timestamp = params["timestamp"]
         if _processed_plots.get(name) != timestamp:
             wb.run.log({name.stem: wb.Image(str(name))}, step=step)
             _processed_plots[name] = timestamp
 
 
 def on_pretrain_routine_start(trainer):
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/checks.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,34 +249,34 @@
         if hard:
             raise ModuleNotFoundError(emojis(warning))  # assert version requirements met
         if verbose:
             LOGGER.warning(warning)
     return result
 
 
-def check_latest_pypi_version(package_name="pyppbox-ultralytics"):
+def check_latest_pypi_version(package_name="vsensebox-ultralytics"):
     """
     Returns the latest version of a PyPI package without downloading or installing it.
 
     Parameters:
         package_name (str): The name of the package to find the latest version for.
 
     Returns:
         (str): The latest version of the package.
     """
-    if package_name == 'pyppbox-ultralytics':
+    if package_name == 'vsensebox-ultralytics':
         with contextlib.suppress(Exception):
             requests.packages.urllib3.disable_warnings()  # Disable the InsecureRequestWarning
             response = requests.get(f'https://pypi.org/pypi/{package_name}/json', timeout=3)
             if response.status_code == 200:
                 return response.json()['info']['version']
     else:
         LOGGER.info(
-        f'This is custom pyppbox-ultralytics for pyppbox 😃 '
-        f"🌐 Check for the update here: https://github.com/rathaumons/ultralytics-for-pyppbox")
+        f'This is custom vsensebox-ultralytics for vsensebox 😃 '
+        f"🌐 Check for the update here: https://github.com/numediart/ultralytics-for-vsensebox")
     return None
 
 
 def check_pip_update_available():
     """
     Checks if a new version of the ultralytics package is available on PyPI.
 
@@ -286,16 +286,16 @@
     if ONLINE and IS_PIP_PACKAGE:
         with contextlib.suppress(Exception):
             from ultralytics import __version__
 
             latest = check_latest_pypi_version()
             if check_version(__version__, f"<{latest}"):  # check if current version is < latest version
                 LOGGER.info(
-                    f"New https://pypi.org/project/pyppbox-ultralytics/{latest} available 😃 "
-                    f"Update with 'pip install -U pyppbox-ultralytics'"
+                    f"New https://pypi.org/project/vsensebox-ultralytics/{latest} available 😃 "
+                    f"Update with 'pip install -U vsensebox-ultralytics'"
                 )
                 return True
     return False
 
 
 @ThreadingLocked()
 def check_font(font="Arial.ttf"):
@@ -393,15 +393,15 @@
         if install and AUTOINSTALL:  # check environment variable
             n = len(pkgs)  # number of packages updates
             LOGGER.info(f"{prefix} Ultralytics requirement{'s' * (n > 1)} {pkgs} not found, attempting AutoUpdate...")
             try:
                 t = time.time()
                 assert ONLINE, "AutoUpdate skipped (offline)"
                 with Retry(times=2, delay=1):  # run up to 2 times with 1-second retry delay
-                    LOGGER.info(subprocess.check_output(f"pip install --no-cache {s} {cmds}", shell=True).decode())
+                    LOGGER.info(subprocess.check_output(f"pip install --no-cache-dir {s} {cmds}", shell=True).decode())
                 dt = time.time() - t
                 LOGGER.info(
                     f"{prefix} AutoUpdate success ✅ {dt:.1f}s, installed {n} package{'s' * (n > 1)}: {pkgs}\n"
                     f"{prefix} ⚠️ {colorstr('bold', 'Restart runtime or rerun command for updates to take effect')}\n"
                 )
             except Exception as e:
                 LOGGER.warning(f"{prefix} ❌ {e}")
@@ -537,15 +537,16 @@
     return path_resolved.exists() and path_resolved.parts[: len(base_dir_resolved.parts)] == base_dir_resolved.parts
 
 
 def check_imshow(warn=False):
     """Check if environment supports image displays."""
     try:
         if LINUX:
-            assert "DISPLAY" in os.environ and not IS_DOCKER and not IS_COLAB and not IS_KAGGLE
+            assert not IS_COLAB and not IS_KAGGLE
+            assert "DISPLAY" in os.environ, "The DISPLAY environment variable isn't set."
         cv2.imshow("test", np.zeros((8, 8, 3), dtype=np.uint8))  # show a small 8-pixel image
         cv2.waitKey(1)
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         return True
     except Exception as e:
         if warn:
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/dist.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/downloads.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/errors.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/files.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/instance.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/loss.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/metrics.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/ops.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/patches.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/plotting.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,31 +374,31 @@
             color (tuple): tracks line color
             track_thickness (int): track line thickness value
         """
         points = np.hstack(track).astype(np.int32).reshape((-1, 1, 2))
         cv2.polylines(self.im, [points], isClosed=False, color=color, thickness=track_thickness)
         cv2.circle(self.im, (int(track[-1][0]), int(track[-1][1])), track_thickness * 2, color, -1)
 
-    def queue_counts_display(self, label, points=None, region_color=(255, 255, 255), txt_color=(0, 0, 0), fontsize=0.7):
+    def queue_counts_display(self, label, points=None, region_color=(255, 255, 255), txt_color=(0, 0, 0)):
         """
         Displays queue counts on an image centered at the points with customizable font size and colors.
 
         Args:
             label (str): queue counts label
             points (tuple): region points for center point calculation to display text
             region_color (RGB): queue region color
             txt_color (RGB): text display color
-            fontsize (float): text fontsize
         """
+
         x_values = [point[0] for point in points]
         y_values = [point[1] for point in points]
         center_x = sum(x_values) // len(points)
         center_y = sum(y_values) // len(points)
 
-        text_size = cv2.getTextSize(label, 0, fontScale=fontsize, thickness=self.tf)[0]
+        text_size = cv2.getTextSize(label, 0, fontScale=self.sf, thickness=self.tf)[0]
         text_width = text_size[0]
         text_height = text_size[1]
 
         rect_width = text_width + 20
         rect_height = text_height + 20
         rect_top_left = (center_x - rect_width // 2, center_y - rect_height // 2)
         rect_bottom_right = (center_x + rect_width // 2, center_y + rect_height // 2)
@@ -409,21 +409,20 @@
 
         # Draw text
         cv2.putText(
             self.im,
             label,
             (text_x, text_y),
             0,
-            fontScale=fontsize,
+            fontScale=self.sf,
             color=txt_color,
             thickness=self.tf,
             lineType=cv2.LINE_AA,
         )
 
-    ### Parking management utils
     def display_objects_labels(self, im0, text, txt_color, bg_color, x_center, y_center, margin):
         """
         Display the bounding boxes labels in parking management app.
 
         Args:
             im0 (ndarray): inference image
             text (str): object/class name
@@ -441,44 +440,41 @@
         rect_x1 = text_x - margin
         rect_y1 = text_y - text_size[1] - margin
         rect_x2 = text_x + text_size[0] + margin
         rect_y2 = text_y + margin
         cv2.rectangle(im0, (rect_x1, rect_y1), (rect_x2, rect_y2), bg_color, -1)
         cv2.putText(im0, text, (text_x, text_y), 0, self.sf, txt_color, self.tf, lineType=cv2.LINE_AA)
 
-    # Parking lot and object counting app
     def display_analytics(self, im0, text, txt_color, bg_color, margin):
         """
         Display the overall statistics for parking lots
         Args:
             im0 (ndarray): inference image
             text (dict): labels dictionary
             txt_color (bgr color): display color for text foreground
             bg_color (bgr color): display color for text background
             margin (int): gap between text and rectangle for better display
         """
 
         horizontal_gap = int(im0.shape[1] * 0.02)
         vertical_gap = int(im0.shape[0] * 0.01)
-
         text_y_offset = 0
-
         for label, value in text.items():
             txt = f"{label}: {value}"
-            text_size = cv2.getTextSize(txt, 0, int(self.sf * 1.5), int(self.tf * 1.5))[0]
+            text_size = cv2.getTextSize(txt, 0, self.sf, self.tf)[0]
+            if text_size[0] < 5 or text_size[1] < 5:
+                text_size = (5, 5)
             text_x = im0.shape[1] - text_size[0] - margin * 2 - horizontal_gap
             text_y = text_y_offset + text_size[1] + margin * 2 + vertical_gap
             rect_x1 = text_x - margin * 2
             rect_y1 = text_y - text_size[1] - margin * 2
             rect_x2 = text_x + text_size[0] + margin * 2
             rect_y2 = text_y + margin * 2
             cv2.rectangle(im0, (rect_x1, rect_y1), (rect_x2, rect_y2), bg_color, -1)
-            cv2.putText(
-                im0, txt, (text_x, text_y), 0, int(self.sf * 1.5), txt_color, int(self.tf * 1.5), lineType=cv2.LINE_AA
-            )
+            cv2.putText(im0, txt, (text_x, text_y), 0, self.sf, txt_color, self.tf, lineType=cv2.LINE_AA)
             text_y_offset = rect_y2
 
     @staticmethod
     def estimate_pose_angle(a, b, c):
         """
         Calculate the pose angle for object.
 
@@ -514,83 +510,86 @@
                     if len(k) == 3:
                         conf = k[2]
                         if conf < conf_thres:
                             continue
                     cv2.circle(self.im, (int(x_coord), int(y_coord)), radius, (0, 255, 0), -1, lineType=cv2.LINE_AA)
         return self.im
 
-    def plot_angle_and_count_and_stage(self, angle_text, count_text, stage_text, center_kpt, line_thickness=2):
+    def plot_angle_and_count_and_stage(
+        self, angle_text, count_text, stage_text, center_kpt, color=(104, 31, 17), txt_color=(255, 255, 255)
+    ):
         """
         Plot the pose angle, count value and step stage.
 
         Args:
             angle_text (str): angle value for workout monitoring
             count_text (str): counts value for workout monitoring
             stage_text (str): stage decision for workout monitoring
             center_kpt (int): centroid pose index for workout monitoring
-            line_thickness (int): thickness for text display
+            color (tuple): text background color for workout monitoring
+            txt_color (tuple): text foreground color for workout monitoring
         """
+
         angle_text, count_text, stage_text = (f" {angle_text:.2f}", f"Steps : {count_text}", f" {stage_text}")
-        font_scale = 0.6 + (line_thickness / 10.0)
 
         # Draw angle
-        (angle_text_width, angle_text_height), _ = cv2.getTextSize(angle_text, 0, font_scale, line_thickness)
+        (angle_text_width, angle_text_height), _ = cv2.getTextSize(angle_text, 0, self.sf, self.tf)
         angle_text_position = (int(center_kpt[0]), int(center_kpt[1]))
         angle_background_position = (angle_text_position[0], angle_text_position[1] - angle_text_height - 5)
-        angle_background_size = (angle_text_width + 2 * 5, angle_text_height + 2 * 5 + (line_thickness * 2))
+        angle_background_size = (angle_text_width + 2 * 5, angle_text_height + 2 * 5 + (self.tf * 2))
         cv2.rectangle(
             self.im,
             angle_background_position,
             (
                 angle_background_position[0] + angle_background_size[0],
                 angle_background_position[1] + angle_background_size[1],
             ),
-            (255, 255, 255),
+            color,
             -1,
         )
-        cv2.putText(self.im, angle_text, angle_text_position, 0, font_scale, (0, 0, 0), line_thickness)
+        cv2.putText(self.im, angle_text, angle_text_position, 0, self.sf, txt_color, self.tf)
 
         # Draw Counts
-        (count_text_width, count_text_height), _ = cv2.getTextSize(count_text, 0, font_scale, line_thickness)
+        (count_text_width, count_text_height), _ = cv2.getTextSize(count_text, 0, self.sf, self.tf)
         count_text_position = (angle_text_position[0], angle_text_position[1] + angle_text_height + 20)
         count_background_position = (
             angle_background_position[0],
             angle_background_position[1] + angle_background_size[1] + 5,
         )
-        count_background_size = (count_text_width + 10, count_text_height + 10 + (line_thickness * 2))
+        count_background_size = (count_text_width + 10, count_text_height + 10 + self.tf)
 
         cv2.rectangle(
             self.im,
             count_background_position,
             (
                 count_background_position[0] + count_background_size[0],
                 count_background_position[1] + count_background_size[1],
             ),
-            (255, 255, 255),
+            color,
             -1,
         )
-        cv2.putText(self.im, count_text, count_text_position, 0, font_scale, (0, 0, 0), line_thickness)
+        cv2.putText(self.im, count_text, count_text_position, 0, self.sf, txt_color, self.tf)
 
         # Draw Stage
-        (stage_text_width, stage_text_height), _ = cv2.getTextSize(stage_text, 0, font_scale, line_thickness)
+        (stage_text_width, stage_text_height), _ = cv2.getTextSize(stage_text, 0, self.sf, self.tf)
         stage_text_position = (int(center_kpt[0]), int(center_kpt[1]) + angle_text_height + count_text_height + 40)
         stage_background_position = (stage_text_position[0], stage_text_position[1] - stage_text_height - 5)
         stage_background_size = (stage_text_width + 10, stage_text_height + 10)
 
         cv2.rectangle(
             self.im,
             stage_background_position,
             (
                 stage_background_position[0] + stage_background_size[0],
                 stage_background_position[1] + stage_background_size[1],
             ),
-            (255, 255, 255),
+            color,
             -1,
         )
-        cv2.putText(self.im, stage_text, stage_text_position, 0, font_scale, (0, 0, 0), line_thickness)
+        cv2.putText(self.im, stage_text, stage_text_position, 0, self.sf, txt_color, self.tf)
 
     def seg_bbox(self, mask, mask_color=(255, 0, 255), det_label=None, track_label=None):
         """
         Function for drawing segmented object in bounding box shape.
 
         Args:
             mask (list): masks data list for instance segmentation area plotting
@@ -622,60 +621,59 @@
         Args:
             distance_m (float): Distance between two bbox centroids in meters.
             distance_mm (float): Distance between two bbox centroids in millimeters.
             centroids (list): Bounding box centroids data.
             line_color (RGB): Distance line color.
             centroid_color (RGB): Bounding box centroid color.
         """
-        (text_width_m, text_height_m), _ = cv2.getTextSize(f"Distance M: {distance_m:.2f}m", 0, 0.8, 2)
-        cv2.rectangle(self.im, (15, 25), (15 + text_width_m + 10, 25 + text_height_m + 20), (255, 255, 255), -1)
+
+        (text_width_m, text_height_m), _ = cv2.getTextSize(f"Distance M: {distance_m:.2f}m", 0, self.sf, self.tf)
+        cv2.rectangle(self.im, (15, 25), (15 + text_width_m + 10, 25 + text_height_m + 20), line_color, -1)
         cv2.putText(
             self.im,
             f"Distance M: {distance_m:.2f}m",
             (20, 50),
             0,
-            0.8,
-            (0, 0, 0),
-            2,
+            self.sf,
+            centroid_color,
+            self.tf,
             cv2.LINE_AA,
         )
 
-        (text_width_mm, text_height_mm), _ = cv2.getTextSize(f"Distance MM: {distance_mm:.2f}mm", 0, 0.8, 2)
-        cv2.rectangle(self.im, (15, 75), (15 + text_width_mm + 10, 75 + text_height_mm + 20), (255, 255, 255), -1)
+        (text_width_mm, text_height_mm), _ = cv2.getTextSize(f"Distance MM: {distance_mm:.2f}mm", 0, self.sf, self.tf)
+        cv2.rectangle(self.im, (15, 75), (15 + text_width_mm + 10, 75 + text_height_mm + 20), line_color, -1)
         cv2.putText(
             self.im,
             f"Distance MM: {distance_mm:.2f}mm",
             (20, 100),
             0,
-            0.8,
-            (0, 0, 0),
-            2,
+            self.sf,
+            centroid_color,
+            self.tf,
             cv2.LINE_AA,
         )
 
         cv2.line(self.im, centroids[0], centroids[1], line_color, 3)
         cv2.circle(self.im, centroids[0], 6, centroid_color, -1)
         cv2.circle(self.im, centroids[1], 6, centroid_color, -1)
 
-    def visioneye(self, box, center_point, color=(235, 219, 11), pin_color=(255, 0, 255), thickness=2, pins_radius=10):
+    def visioneye(self, box, center_point, color=(235, 219, 11), pin_color=(255, 0, 255)):
         """
         Function for pinpoint human-vision eye mapping and plotting.
 
         Args:
             box (list): Bounding box coordinates
             center_point (tuple): center point for vision eye view
             color (tuple): object centroid and line color value
             pin_color (tuple): visioneye point color value
-            thickness (int): int value for line thickness
-            pins_radius (int): visioneye point radius value
         """
         center_bbox = int((box[0] + box[2]) / 2), int((box[1] + box[3]) / 2)
-        cv2.circle(self.im, center_point, pins_radius, pin_color, -1)
-        cv2.circle(self.im, center_bbox, pins_radius, color, -1)
-        cv2.line(self.im, center_point, center_bbox, color, thickness)
+        cv2.circle(self.im, center_point, self.tf * 2, pin_color, -1)
+        cv2.circle(self.im, center_bbox, self.tf * 2, color, -1)
+        cv2.line(self.im, center_point, center_bbox, color, self.tf)
 
 
 @TryExcept()  # known issue https://github.com/ultralytics/yolov5/issues/5395
 @plt_settings()
 def plot_labels(boxes, cls, names=(), save_dir=Path(""), on_plot=None):
     """Plot training labels including class histograms and box statistics."""
     import pandas  # scope for faster 'import ultralytics'
```

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/tal.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/torch_utils.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/triton.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/ultralytics/utils/tuner.py` & `vsensebox_ultralytics-8.2.18/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/PKG-INFO` & `vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vsensebox-ultralytics
-Version: 8.2.15
+Version: 8.2.18
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
-Home-page: https://github.com/rathaumons/ultralytics-for-vsensebox
+Home-page: https://github.com/numediart/ultralytics-for-vsensebox
 License: AGPL-3.0
-Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-vsensebox/issues
-Project-URL: Funding, https://ultralytics.com
-Project-URL: Source, https://github.com/rathaumons/ultralytics-for-vsensebox
+Project-URL: Bug Reports, https://github.com/numediart/ultralytics-for-vsensebox/issues
+Project-URL: Source, https://github.com/numediart/ultralytics-for-vsensebox
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -47,43 +46,43 @@
 Requires-Dist: coremltools>=7.0; extra == "export"
 Requires-Dist: openvino>=2024.0.0; extra == "export"
 Provides-Extra: explorer
 Requires-Dist: lancedb; extra == "explorer"
 Requires-Dist: duckdb<=0.9.2; extra == "explorer"
 Requires-Dist: streamlit; extra == "explorer"
 
-[![Test Build](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
+[![Test Build](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/test_build.yaml) [![PyPI](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/publish.yaml/badge.svg)](https://github.com/numediart/ultralytics-for-vsensebox/actions/workflows/publish.yaml)
 
 # Customized Ultralytics for VSenseBox
 
-* Updated: **May 14, 2024**
-* Synced with: v8.2.15 -> [[590002f]](https://github.com/ultralytics/ultralytics/commit/590002ff6d3a936b0cb1aeb582ea2daa26fcdbb6)
+* Updated: **May 22, 2024**
+* Synced with: v8.2.18 -> [[c8b6a8b]](https://github.com/ultralytics/ultralytics/commit/c8b6a8bc37ce196a6b7e0c153539402db4383c16)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
-* Customized for [`VSenseBox`](https://github.com/rathaumons/vsensebox):
+* Customized for [`VSenseBox`](https://github.com/numediart/vsensebox):
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
 
 ## Installation
 
 * Install from [PyPI](https://pypi.org/project/vsensebox-ultralytics/):
     ```
     pip install vsensebox-ultralytics
     ``` 
 * Or install from GitHub directly:
     ```
-    pip install git+https://github.com/rathaumons/ultralytics-for-vsensebox.git
+    pip install git+https://github.com/numediart/ultralytics-for-vsensebox.git
     ```
 * Or build from source:
 
     <details><summary><ins>Click here to expand!</ins></summary>
     
     ```
-    git clone https://github.com/rathaumons/ultralytics-for-vsensebox.git
+    git clone https://github.com/numediart/ultralytics-for-vsensebox.git
     cd ultralytics-for-vsensebox
     python -m pip install --upgrade pip
     python -m pip install -U pip setuptools
     pip install wheel build
     python -m build --wheel --skip-dependency-check --no-isolatio
     cd dist
     ```
```

### Comparing `vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/SOURCES.txt` & `vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vsensebox_ultralytics-8.2.15/vsensebox_ultralytics.egg-info/top_level.txt` & `vsensebox_ultralytics-8.2.18/vsensebox_ultralytics.egg-info/top_level.txt`

 * *Files identical despite different names*

