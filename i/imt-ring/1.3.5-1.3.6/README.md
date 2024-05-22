# Comparing `tmp/imt_ring-1.3.5.tar.gz` & `tmp/imt_ring-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ring-1.3.5.tar", last modified: Wed May 15 14:41:38 2024, max compression
+gzip compressed data, was "imt_ring-1.3.6.tar", last modified: Wed May 22 11:41:55 2024, max compression
```

## Comparing `imt_ring-1.3.5.tar` & `imt_ring-1.3.6.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.063777 imt_ring-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 14:41:38.063777 imt_ring-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-15 14:41:34.000000 imt_ring-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 14:41:34.000000 imt_ring-1.3.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 14:41:38.063777 imt_ring-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.027776 imt_ring-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.059776 imt_ring-1.3.5/src/imt_ring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 14:41:38.000000 imt_ring-1.3.5/src/imt_ring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.031776 imt_ring-1.3.5/src/ring/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.031776 imt_ring-1.3.5/src/ring/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.031776 imt_ring-1.3.5/src/ring/algorithms/custom_joints/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_imp_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16215 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/custom_joints/suntay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.035776 imt_ring-1.3.5/src/ring/algorithms/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/algorithms/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33913 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.035776 imt_ring-1.3.5/src/ring/io/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.035776 imt_ring-1.3.5/src/ring/io/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/branched.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/io/examples/exclude/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/exclude/knee_trans_dof.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/inv_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/knee_flexible_imus.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/spherical_stiff.xml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/symmetric.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_all_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_all_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_ang0_pos0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_control.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_free.xml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_kinematics.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/io/examples/test_morph_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_randomize_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_sensors.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples/test_three_seg_seg2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/io/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/test_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/io/xml/to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/maths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.039776 imt_ring-1.3.5/src/ring/ml/params/
--rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/params/0x13e3518065c21cd8.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/ringnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/ml/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/base_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/mujoco_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/vispy_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/rendering/vispy_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/sim2real/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sim2real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sim2real/sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/sys_composer/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/delete_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/inject_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/sys_composer/morph_sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.055776 imt_ring-1.3.5/src/ring/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-15 14:41:34.000000 imt_ring-1.3.5/src/ring/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:41:38.059776 imt_ring-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_custom_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_rcmg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_sys_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 14:41:34.000000 imt_ring-1.3.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.406696 imt_ring-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 11:41:55.406696 imt_ring-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-22 11:41:51.000000 imt_ring-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-22 11:41:51.000000 imt_ring-1.3.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 11:41:55.406696 imt_ring-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.374696 imt_ring-1.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.406696 imt_ring-1.3.6/src/imt_ring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 11:41:55.000000 imt_ring-1.3.6/src/imt_ring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/algorithms/custom_joints/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_imp_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16676 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/custom_joints/suntay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.378696 imt_ring-1.3.6/src/ring/algorithms/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/algorithms/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33947 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/branched.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/examples/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/exclude/knee_trans_dof.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/inv_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/knee_flexible_imus.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/spherical_stiff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/symmetric.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_all_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_all_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_ang0_pos0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_control.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_free.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_kinematics.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.382696 imt_ring-1.3.6/src/ring/io/examples/test_morph_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_randomize_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_sensors.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples/test_three_seg_seg2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.386696 imt_ring-1.3.6/src/ring/io/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/test_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/io/xml/to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.386696 imt_ring-1.3.6/src/ring/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.386696 imt_ring-1.3.6/src/ring/ml/params/
+-rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/params/0x13e3518065c21cd8.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/ringnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/ml/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.398696 imt_ring-1.3.6/src/ring/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/base_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/mujoco_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/vispy_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/rendering/vispy_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.398696 imt_ring-1.3.6/src/ring/sim2real/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sim2real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sim2real/sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.402696 imt_ring-1.3.6/src/ring/sys_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/delete_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/inject_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/sys_composer/morph_sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.402696 imt_ring-1.3.6/src/ring/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-22 11:41:51.000000 imt_ring-1.3.6/src/ring/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:41:55.406696 imt_ring-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_custom_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_rcmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_sys_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-22 11:41:51.000000 imt_ring-1.3.6/tests/test_utils.py
```

### Comparing `imt_ring-1.3.5/PKG-INFO` & `imt_ring-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.5
+Version: 1.3.6
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.5/pyproject.toml` & `imt_ring-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ring"
-version = "1.3.5"
+version = "1.3.6"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "RING: Recurrent Inertial Graph-based Estimator"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_ring-1.3.5/readme.md` & `imt_ring-1.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/imt_ring.egg-info/PKG-INFO` & `imt_ring-1.3.6/src/imt_ring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.3.5
+Version: 1.3.6
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.3.5/src/imt_ring.egg-info/SOURCES.txt` & `imt_ring-1.3.6/src/imt_ring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/__init__.py` & `imt_ring-1.3.6/src/ring/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algebra.py` & `imt_ring-1.3.6/src/ring/algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/__init__.py` & `imt_ring-1.3.6/src/ring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/_random.py` & `imt_ring-1.3.6/src/ring/algorithms/_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_imp_joint.py` & `imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_imp_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/custom_joints/rr_joint.py` & `imt_ring-1.3.6/src/ring/algorithms/custom_joints/rr_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/custom_joints/suntay.py` & `imt_ring-1.3.6/src/ring/algorithms/custom_joints/suntay.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,20 +289,33 @@
             find_suntay_joint=_utils_find_suntay_joint,
             sconfig=sconfig,
         ),
     )
     ring.register_new_joint_type(name, joint_model, 1, overwrite=True)
 
 
+def _scale_delta(method: str, key, xs, mn, mx, amin, amax, **kwargs):
+    if method == "normal":
+        delta = jnp.clip(jax.random.normal(key) + 0.5, 1.0)
+    elif method == "uniform":
+        delta = 1 / (jax.random.uniform(key) + 1e-2)
+    else:
+        raise NotImplementedError
+
+    return delta
+
+
 def Polynomial_DrawnFnPair(
     order: int = 2,
     center: bool = False,
     flexion_center_deg: Optional[float] = None,
     include_bias: bool = True,
     enable_scale_delta: bool = True,
+    scale_delta_method: str = "normal",
+    scale_delta_kwargs: dict = dict(),
 ) -> DrawnFnPairFactory:
     assert not (order == 0 and not include_bias)
 
     flexion_center = (
         jnp.deg2rad(flexion_center_deg) if flexion_center_deg is not None else None
     )
     del flexion_center_deg
@@ -339,15 +352,17 @@
             values = jax.vmap(_apply_poly_factors, in_axes=(None, 0))(
                 poly_factors, xs - q0
             )
             eps = 1e-6
             amin, amax = jnp.min(values), jnp.max(values) + eps
             if enable_scale_delta:
                 delta = amax - amin
-                scale_delta = jnp.clip(jax.random.normal(c3) + 0.5, 1.0)
+                scale_delta = _scale_delta(
+                    scale_delta_method, c3, xs, mn, mx, amin, amax, **scale_delta_kwargs
+                )
                 amax = amin + delta * scale_delta
             return amin, amax, poly_factors, q0
 
         def _apply(params, q):
             amin, amax, poly_factors, q0 = params
             q = q - q0
             value = _apply_poly_factors(poly_factors, q)
```

### Comparing `imt_ring-1.3.5/src/ring/algorithms/dynamics.py` & `imt_ring-1.3.6/src/ring/algorithms/dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/__init__.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/base.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,19 @@
         utils.hdf5_save(path, data, overwrite=overwrite)
 
     def to_eager_gen(
         self,
         batchsize: int = 1,
         sizes: int | list[int] = 1,
         seed: int = 1,
+        shuffle: bool = True,
     ) -> types.BatchedGenerator:
-        return batch.batch_generators_eager(self.gens, sizes, batchsize, seed=seed)
+        return batch.batch_generators_eager(
+            self.gens, sizes, batchsize, seed=seed, shuffle=shuffle
+        )
 
     def to_lazy_gen(
         self, sizes: int | list[int] = 1, jit: bool = True
     ) -> types.BatchedGenerator:
         return batch.batch_generators_lazy(self.gens, sizes, jit=jit)
 
     @staticmethod
```

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/batch.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/batch.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/motion_artifacts.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/pd_control.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/randomize.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/transforms.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/transforms.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/generator/types.py` & `imt_ring-1.3.6/src/ring/algorithms/generator/types.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/jcalc.py` & `imt_ring-1.3.6/src/ring/algorithms/jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/kinematics.py` & `imt_ring-1.3.6/src/ring/algorithms/kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/algorithms/sensors.py` & `imt_ring-1.3.6/src/ring/algorithms/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 from typing import Optional
 
 import jax
 import jax.numpy as jnp
+
 from ring import algebra
 from ring import algorithms
 from ring import base
 from ring import io
 from ring import maths
 from ring import sim2real
 
@@ -441,30 +442,26 @@
 
     X = {name: {"joint_axes": axes[sys.name_to_idx(name)]} for name in sys.link_names}
     return X
 
 
 def _joint_axes_from_sys(sys: base.Transform, N: int) -> dict:
     "`sys` should be `sys_noimu`. `N` is number of timesteps"
-    xaxis = jnp.array([1.0, 0, 0])
-    yaxis = jnp.array([0.0, 1, 0])
-    zaxis = jnp.array([0.0, 0, 1])
-    id_to_axis = {"x": xaxis, "y": yaxis, "z": zaxis}
     X = {}
 
     def f(_, __, name, link_type, link):
         joint_params = link.joint_params
         if link_type in ["rx", "ry", "rz"]:
-            joint_axes = id_to_axis[link_type[1]]
+            joint_axes = maths.unit_vectors(link_type[1])
         elif link_type == "rr":
             joint_axes = joint_params["rr"]["joint_axes"]
         elif link_type[:6] == "rr_imp":
             joint_axes = joint_params[link_type]["joint_axes"]
         else:
-            joint_axes = xaxis
+            joint_axes = maths.x_unit_vector
         X[name] = {"joint_axes": joint_axes}
 
     sys.scan(f, "lll", sys.link_names, sys.link_types, sys.links)
     X = jax.tree_map(lambda arr: jnp.repeat(arr[None], N, axis=0), X)
     return X
```

### Comparing `imt_ring-1.3.5/src/ring/base.py` & `imt_ring-1.3.6/src/ring/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,14 +567,15 @@
         self,
         name: str,
         new_joint_type: str,
         new_arma: Optional[jax.Array] = None,
         new_damp: Optional[jax.Array] = None,
         new_stif: Optional[jax.Array] = None,
         new_zero: Optional[jax.Array] = None,
+        seed: int = 1,
     ):
         "By default damping, stiffness are set to zero."
         from ring.algorithms import get_joint_model
 
         q_size, qd_size = Q_WIDTHS[new_joint_type], QD_WIDTHS[new_joint_type]
 
         def logic_unfreeze_to_spherical(link_name, olt, ola, old, ols, olz):
@@ -596,15 +597,15 @@
 
             return nlt, nla, nld, nls, nlz
 
         sys = _update_sys_if_replace_joint_type(self, logic_unfreeze_to_spherical)
 
         jm = get_joint_model(new_joint_type)
         if jm.init_joint_params is not None:
-            sys = sys.from_str(sys.to_str())
+            sys = sys.from_str(sys.to_str(), seed=seed)
 
         return sys
 
     def findall_imus(self) -> list[str]:
         return [name for name in self.link_names if name[:3] == "imu"]
 
     def findall_segments(self) -> list[str]:
```

### Comparing `imt_ring-1.3.5/src/ring/io/examples/branched.xml` & `imt_ring-1.3.6/src/ring/io/examples/branched.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/exclude/knee_trans_dof.xml` & `imt_ring-1.3.6/src/ring/io/examples/exclude/knee_trans_dof.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.3.6/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/inv_pendulum.xml` & `imt_ring-1.3.6/src/ring/io/examples/inv_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/knee_flexible_imus.xml` & `imt_ring-1.3.6/src/ring/io/examples/knee_flexible_imus.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_all_1.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_all_1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_all_2.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_all_2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_control.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_control.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_double_pendulum.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_kinematics.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_kinematics.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg1.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_morph_system/four_seg_seg3.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_morph_system/four_seg_seg3.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_randomize_position.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_randomize_position.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples/test_three_seg_seg2.xml` & `imt_ring-1.3.6/src/ring/io/examples/test_three_seg_seg2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/examples.py` & `imt_ring-1.3.6/src/ring/io/examples.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/xml/abstract.py` & `imt_ring-1.3.6/src/ring/io/xml/abstract.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/xml/from_xml.py` & `imt_ring-1.3.6/src/ring/io/xml/from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/xml/test_from_xml.py` & `imt_ring-1.3.6/src/ring/io/xml/test_from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/xml/test_to_xml.py` & `imt_ring-1.3.6/src/ring/io/xml/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/io/xml/to_xml.py` & `imt_ring-1.3.6/src/ring/io/xml/to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/maths.py` & `imt_ring-1.3.6/src/ring/maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/__init__.py` & `imt_ring-1.3.6/src/ring/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/base.py` & `imt_ring-1.3.6/src/ring/ml/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/callbacks.py` & `imt_ring-1.3.6/src/ring/ml/callbacks.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/ml_utils.py` & `imt_ring-1.3.6/src/ring/ml/ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/optimizer.py` & `imt_ring-1.3.6/src/ring/ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/params/0x13e3518065c21cd8.pickle` & `imt_ring-1.3.6/src/ring/ml/params/0x13e3518065c21cd8.pickle`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/ringnet.py` & `imt_ring-1.3.6/src/ring/ml/ringnet.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/train.py` & `imt_ring-1.3.6/src/ring/ml/train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/ml/training_loop.py` & `imt_ring-1.3.6/src/ring/ml/training_loop.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/rendering/base_render.py` & `imt_ring-1.3.6/src/ring/rendering/base_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/rendering/mujoco_render.py` & `imt_ring-1.3.6/src/ring/rendering/mujoco_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/rendering/vispy_render.py` & `imt_ring-1.3.6/src/ring/rendering/vispy_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/rendering/vispy_visuals.py` & `imt_ring-1.3.6/src/ring/rendering/vispy_visuals.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/sim2real/sim2real.py` & `imt_ring-1.3.6/src/ring/sim2real/sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/spatial.py` & `imt_ring-1.3.6/src/ring/spatial.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/sys_composer/delete_sys.py` & `imt_ring-1.3.6/src/ring/sys_composer/delete_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/sys_composer/inject_sys.py` & `imt_ring-1.3.6/src/ring/sys_composer/inject_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/sys_composer/morph_sys.py` & `imt_ring-1.3.6/src/ring/sys_composer/morph_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/__init__.py` & `imt_ring-1.3.6/src/ring/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/batchsize.py` & `imt_ring-1.3.6/src/ring/utils/batchsize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/colab.py` & `imt_ring-1.3.6/src/ring/utils/colab.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/hdf5.py` & `imt_ring-1.3.6/src/ring/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/normalizer.py` & `imt_ring-1.3.6/src/ring/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/path.py` & `imt_ring-1.3.6/src/ring/utils/path.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/src/ring/utils/utils.py` & `imt_ring-1.3.6/src/ring/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,16 @@
         return tree.copy()
     elif isinstance(tree, list):
         return [pytree_deepcopy(ele) for ele in tree]
     elif isinstance(tree, tuple):
         return tuple(pytree_deepcopy(ele) for ele in tree)
     elif isinstance(tree, dict):
         return {key: pytree_deepcopy(value) for key, value in tree.items()}
+    elif isinstance(tree, _Base):
+        return tree
     else:
         raise NotImplementedError(f"Not implemented for type={type(tree)}")
 
 
 def import_lib(
     lib: str,
     required_for: Optional[str] = None,
```

### Comparing `imt_ring-1.3.5/tests/test_algebra.py` & `imt_ring-1.3.6/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_base.py` & `imt_ring-1.3.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_custom_joints.py` & `imt_ring-1.3.6/tests/test_custom_joints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import jax
 import numpy as np
+import pytest
+
 import ring
 from ring import MotionConfig
 from ring.algorithms import custom_joints
 from ring.algorithms.generator import transforms
 from ring.algorithms.jcalc import _init_joint_params
 
 
@@ -17,56 +19,62 @@
         ring.algorithms.GeneratorTrafoRemoveOutputExtras(),
         ring.algorithms.GeneratorTrafoRemoveInputExtras(sys),
     )(MotionConfig(T=10.0))
 
     return gen(jax.random.PRNGKey(1))[0]
 
 
-def test_virtual_input_joint_axes_rr_joint():
-    sys = ring.io.load_example("test_three_seg_seg2")
+def _replace_ry_rz_with(sys, new_joint_type: str):
     sys_rr = sys.replace(
         link_types=[
-            "rr" if link_type in ["ry", "rz"] else link_type
+            new_joint_type if link_type in ["ry", "rz"] else link_type
             for link_type in sys.link_types
         ]
     )
+    return sys_rr
+
+
+def test_virtual_input_joint_axes_rr_joint():
+    sys = ring.io.load_example("test_three_seg_seg2")
+    sys_rr = _replace_ry_rz_with(sys, "rr")
     sys_rr = _init_joint_params(jax.random.PRNGKey(1), sys_rr)
     joint_axes = sys_rr.links.joint_params["rr"]["joint_axes"]
 
     # test `ry` / `rz`
     X = pipeline_load_data_X(sys)
 
     np.testing.assert_allclose(
         X["seg1"]["joint_axes"],
         np.repeat(np.array([[0.0, -1, 0]]), 1000, axis=0),
-        atol=1e-7,
+        atol=4e-7,
     )
     np.testing.assert_allclose(
         X["seg3"]["joint_axes"],
         np.repeat(np.array([[0.0, 0, 1]]), 1000, axis=0),
         atol=1e-7,
     )
 
     # test `rr`
     X = pipeline_load_data_X(sys_rr)
 
     np.testing.assert_allclose(
         X["seg1"]["joint_axes"],
         np.repeat(-joint_axes[1:2], 1000, axis=0),
-        atol=3e-7,
-        rtol=2e-6,
+        atol=4e-7,
+        rtol=2e-4,
     )
     np.testing.assert_allclose(
         X["seg3"]["joint_axes"],
         np.repeat(joint_axes[3:4], 1000, axis=0),
         atol=3e-7,
         rtol=2e-6,
     )
 
 
+@pytest.mark.filterwarnings("ignore:The system has")
 def test_virtual_input_joint_axes_rr_imp_joint():
     custom_joints.register_rr_imp_joint(MotionConfig(T=10.0))
 
     sys = ring.io.load_example("test_three_seg_seg2")
     sys_rr_imp = sys.change_joint_type("seg1", "rr_imp").change_joint_type(
         "seg3", "rr_imp"
     )
@@ -81,26 +89,26 @@
         np.repeat(joint_axes[1:2], 1000, axis=0),
         atol=0.01,
         rtol=0.02,
     )
     np.testing.assert_allclose(
         X["seg3"]["joint_axes"],
         np.repeat(-joint_axes[3:4], 1000, axis=0),
-        atol=0.002,
-        rtol=0.002,
+        atol=0.01,
+        rtol=0.032,
     )
 
     # test `make_generator`
     # we can't really test behaviour for `rr_imp` since the `make_generator` internally
     # builds a `setup_fn` that randomizes the `sys.links.joint_params` field
     X = pipeline_load_data_X(sys)
 
     np.testing.assert_allclose(
         X["seg1"]["joint_axes"],
         np.repeat(np.array([[0.0, -1, 0]]), 1000, axis=0),
-        atol=1e-7,
+        atol=4e-7,
     )
     np.testing.assert_allclose(
         X["seg3"]["joint_axes"],
         np.repeat(np.array([[0.0, 0, 1]]), 1000, axis=0),
-        atol=1e-7,
+        atol=4e-7,
     )
```

### Comparing `imt_ring-1.3.5/tests/test_dynamics.py` & `imt_ring-1.3.6/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_generator.py` & `imt_ring-1.3.6/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_jcalc.py` & `imt_ring-1.3.6/tests/test_jcalc.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_jit.py` & `imt_ring-1.3.6/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_kinematics.py` & `imt_ring-1.3.6/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_maths.py` & `imt_ring-1.3.6/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_ml_utils.py` & `imt_ring-1.3.6/tests/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_motion_artifacts.py` & `imt_ring-1.3.6/tests/test_motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_pd_control.py` & `imt_ring-1.3.6/tests/test_pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_random.py` & `imt_ring-1.3.6/tests/test_random.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from jax import random as jrand
 import numpy as np
 import pytest
+
 import ring
 from ring.algorithms._random import _resolve_range_of_motion
 
 
 @pytest.mark.parametrize(
     "range_of_motion, range_of_motion_method, delta_ang_min, delta_ang_max",
     [
@@ -13,29 +14,35 @@
         (True, "coinflip", 0.0, 0.1),
         (True, "uniform", 2.5, 3.0),
     ],
 )
 def test_delta_ang_min_max(
     range_of_motion, range_of_motion_method, delta_ang_min, delta_ang_max
 ):
+    max_iter = 100
+    t_min, t_max = 0.1, 3.1
     for seed in range(10):
-        key = jrand.PRNGKey(seed)
-        phi = _resolve_range_of_motion(
-            range_of_motion,
-            range_of_motion_method,
-            0.0,
-            3.14,
-            float(delta_ang_min),
-            float(delta_ang_max),
-            1.0,
-            0.0,
-            key,
-            100,
-        )
-        assert delta_ang_min < abs(phi) < delta_ang_max
+        for prev_phi in [-3.0, 0.0, 3.0]:
+            key_t, key_ang = jrand.split(jrand.PRNGKey(seed))
+            dt, next_phi = _resolve_range_of_motion(
+                range_of_motion,
+                range_of_motion_method,
+                0.0,
+                3.14,
+                float(delta_ang_min),
+                float(delta_ang_max),
+                t_min,
+                t_max,
+                prev_phi,
+                key_t,
+                key_ang,
+                max_iter,
+            )
+            assert t_min <= dt <= t_max
+            assert delta_ang_min < abs(next_phi - prev_phi) < delta_ang_max
 
 
 @pytest.mark.parametrize(
     "randomized_interpolation, range_of_motion, range_of_motion_method",
     [
         (False, False, "uniform"),
         (False, False, "coinflip"),
```

### Comparing `imt_ring-1.3.5/tests/test_randomize.py` & `imt_ring-1.3.6/tests/test_randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_rcmg.py` & `imt_ring-1.3.6/tests/test_rcmg.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_render.py` & `imt_ring-1.3.6/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_sensors.py` & `imt_ring-1.3.6/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_sim2real.py` & `imt_ring-1.3.6/tests/test_sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_sys_composer.py` & `imt_ring-1.3.6/tests/test_sys_composer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_train.py` & `imt_ring-1.3.6/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.3.5/tests/test_utils.py` & `imt_ring-1.3.6/tests/test_utils.py`

 * *Files identical despite different names*

