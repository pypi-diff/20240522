# Comparing `tmp/imap_box_up-0.0.4.tar.gz` & `tmp/imap_box_up-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_box_up-0.0.4.tar", last modified: Wed Apr 24 11:36:58 2024, max compression
+gzip compressed data, was "imap_box_up-0.0.5.tar", last modified: Wed May 22 08:54:46 2024, max compression
```

## Comparing `imap_box_up-0.0.4.tar` & `imap_box_up-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.930940 imap_box_up-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-24 11:36:58.930940 imap_box_up-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.922939 imap_box_up-0.0.4/imap/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/global_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.926939 imap_box_up-0.0.4/imap/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    32951 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/convex_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/odr_spiral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.926939 imap_box_up-0.0.4/imap/lib/opendrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/junction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/lanes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/plan_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/road.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/polynoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/proj_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.926939 imap_box_up-0.0.4/imap_box_up.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:36:58.930940 imap_box_up-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:46.215440 imap_box_up-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-22 08:54:46.215440 imap_box_up-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:46.211440 imap_box_up-0.0.5/imap/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/global_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:46.211440 imap_box_up-0.0.5/imap/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27871 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/odr_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:46.215440 imap_box_up-0.0.5/imap/lib/opendrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/lanes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/plan_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/road.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/opendrive/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/polynoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/proj_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/lib/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/imap/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:54:46.215440 imap_box_up-0.0.5/imap_box_up.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-22 08:54:46.000000 imap_box_up-0.0.5/imap_box_up.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-22 08:54:46.000000 imap_box_up-0.0.5/imap_box_up.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:54:46.000000 imap_box_up-0.0.5/imap_box_up.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 08:54:46.000000 imap_box_up-0.0.5/imap_box_up.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-22 08:54:46.000000 imap_box_up-0.0.5/imap_box_up.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 08:54:46.000000 imap_box_up-0.0.5/imap_box_up.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:54:46.215440 imap_box_up-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 08:54:06.000000 imap_box_up-0.0.5/setup.py
```

### Comparing `imap_box_up-0.0.4/LICENSE` & `imap_box_up-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/PKG-INFO` & `imap_box_up-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,46 @@
-Metadata-Version: 2.1
-Name: imap_box_up
-Version: 0.0.4
-Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
-Home-page: https://github.com/porterpan/imap_box_up
-Author: porter
-Author-email: porter.pan@outlook.com
-Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: protobuf<=3.19.4
-Requires-Dist: matplotlib
-Requires-Dist: pyproj
-Requires-Dist: record_msg<=0.1.1
-Requires-Dist: concave-hull<=0.0.7
-Requires-Dist: scipy<=1.13.0
-
 # imap_box_up
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
 **[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap/releases/tag/v0.1.7), the imap tool is very useful. 
 
-The name of **imap_box_up** , Just to modified from imap_box
-
-The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
+The name of **imap_box_up** , Just to modified from imap_box and just to distinguish it from **imap_box**
 
 imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-- the map road lane attribution should have curb, if not have curb, task will random selection shouler, stop, walking to create apoolo map.
+- the map road lane attribution should have curb, if not have curb, task will random selection shouler ~~, stop, walking to create apoolo map.~~
 
 - The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to my appollo hdmap code for perception work. 
+
 
+## 新特性1（junction apollo map 显示使用 curbe or shoulder道路属性进行显示，可以实现弧形的显示，而不是原先的box显示junction hd map)
 
-## fix junction bug
+该功能使用默认参数将生成沿着curb或者shoulder绘制的路口地图
 
 ![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
 
-**Supported features**:
-1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
-2. Find lane by id
-3. Convert format: Opendrive to Apollo format.
+如果你要使用原先的box形状显示路口，可以使用参数 -b 即可生成box形状的路口。
 
-| os      | support                 | remark |
-|---------|-------------------------|--------|
-| ubuntu  | :heavy_check_mark:      |        |
-| mac     | :heavy_check_mark:      |        |
-| windows | :heavy_check_mark:      |        |
+## new 2 （添加新的参数-r 以转换为不带有地理坐标的地图数据)
 
-## Related work
-- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
-- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
-- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
+## 地图绘制说明
+
+绘制路口时，确保路口存在curb或者shoulder元素，因为默认非box的junction路口apollo hdmap 需要有这两种元素中的一种或者两种才能正常生成，否则转换后的apollo hdmap 将丢失junction 元素。检查是否有curb属性如下图
+
+![](roadmap_have_junction_or_shoulder.png)
 
 ## Quick start
 
 #### Install
+
 You can install imap by following cmd.
 ```shell
 pip3 install imap_box_up
 ```
 
 ## Example
 #### 1. Visualization
@@ -132,7 +106,24 @@
 ```shell
 sudo chmod 777 data/your_map_file
 ```
 2. Map data permission checking has no problem, still nothing display and no errors!
 A: It's better to install imap_box by running "sudo pip3 install imap_box", then run "imap -m xxx.txt".
 
 > If you have any questions, please feel free to contact me.
+
+
+**Supported features**:
+1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
+2. Find lane by id
+3. Convert format: Opendrive to Apollo format.
+
+| os      | support                 | remark |
+|---------|-------------------------|--------|
+| ubuntu  | :heavy_check_mark:      |        |
+| mac     | :heavy_check_mark:      |        |
+| windows | :heavy_check_mark:      |        |
+
+## Related work
+- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
+- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
+- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imap_box_up-0.0.4/README.md` & `imap_box_up-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,67 @@
+Metadata-Version: 2.1
+Name: imap_box_up
+Version: 0.0.5
+Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
+Home-page: https://github.com/porterpan/imap_box_up
+Author: porter
+Author-email: porter.pan@outlook.com
+Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: protobuf<=3.19.4
+Requires-Dist: matplotlib
+Requires-Dist: pyproj
+Requires-Dist: record_msg<=0.1.1
+Requires-Dist: concave-hull<=0.0.7
+Requires-Dist: scipy<=1.13.0
+
 # imap_box_up
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
 **[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap/releases/tag/v0.1.7), the imap tool is very useful. 
 
-The name of **imap_box_up** , Just to modified from imap_box
-
-The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
+The name of **imap_box_up** , Just to modified from imap_box and just to distinguish it from **imap_box**
 
 imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-- the map road lane attribution should have curb, if not have curb, task will random selection shouler, stop, walking to create apoolo map.
+- the map road lane attribution should have curb, if not have curb, task will random selection shouler ~~, stop, walking to create apoolo map.~~
 
 - The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to my appollo hdmap code for perception work. 
+
 
+## 新特性1（junction apollo map 显示使用 curbe or shoulder道路属性进行显示，可以实现弧形的显示，而不是原先的box显示junction hd map)
 
-## fix junction bug
+该功能使用默认参数将生成沿着curb或者shoulder绘制的路口地图
 
 ![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
 
-**Supported features**:
-1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
-2. Find lane by id
-3. Convert format: Opendrive to Apollo format.
+如果你要使用原先的box形状显示路口，可以使用参数 -b 即可生成box形状的路口。
 
-| os      | support                 | remark |
-|---------|-------------------------|--------|
-| ubuntu  | :heavy_check_mark:      |        |
-| mac     | :heavy_check_mark:      |        |
-| windows | :heavy_check_mark:      |        |
+## new 2 （添加新的参数-r 以转换为不带有地理坐标的地图数据)
 
-## Related work
-- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
-- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
-- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
+## 地图绘制说明
+
+绘制路口时，确保路口存在curb或者shoulder元素，因为默认非box的junction路口apollo hdmap 需要有这两种元素中的一种或者两种才能正常生成，否则转换后的apollo hdmap 将丢失junction 元素。检查是否有curb属性如下图
+
+![](roadmap_have_junction_or_shoulder.png)
 
 ## Quick start
 
 #### Install
+
 You can install imap by following cmd.
 ```shell
 pip3 install imap_box_up
 ```
 
 ## Example
 #### 1. Visualization
@@ -110,8 +126,25 @@
 A: Check the permissions of the map file, if the current user does not have permissions, modify the permissions with the following commands.
 ```shell
 sudo chmod 777 data/your_map_file
 ```
 2. Map data permission checking has no problem, still nothing display and no errors!
 A: It's better to install imap_box by running "sudo pip3 install imap_box", then run "imap -m xxx.txt".
 
-> If you have any questions, please feel free to contact me.
+> If you have any questions, please feel free to contact me.
+
+
+**Supported features**:
+1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
+2. Find lane by id
+3. Convert format: Opendrive to Apollo format.
+
+| os      | support                 | remark |
+|---------|-------------------------|--------|
+| ubuntu  | :heavy_check_mark:      |        |
+| mac     | :heavy_check_mark:      |        |
+| windows | :heavy_check_mark:      |        |
+
+## Related work
+- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
+- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
+- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imap_box_up-0.0.4/imap/editor.py` & `imap_box_up-0.0.5/imap/editor.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/global_var.py` & `imap_box_up-0.0.5/imap/global_var.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/common.py` & `imap_box_up-0.0.5/imap/lib/common.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/convertor.py` & `imap_box_up-0.0.5/imap/lib/convertor.py`

 * *Files 14% similar despite different names*

```diff
@@ -601,169 +601,81 @@
         return aabb_box(points)
       else:
         return convex_hull(points)
     
     elif type == "boundry": 
       left_incomroadlist = []  
       right_incomroadlist = []  
- 
+      junction_mark_list= ["curb", "shoulder"]
       boundary_point_temp=[]
       for junction_connecting_lane in xodr_junction.connections:  
-        # connecting_road 
-        for lanesection_ in self.xodr_map.roads[junction_connecting_lane.connecting_road].lanes.lane_sections: 
-          junction_id = self.xodr_map.roads[junction_connecting_lane.connecting_road].junction_id 
-          if junction_id == "-1":
-            continue 
-          link_name = self.xodr_map.roads[junction_connecting_lane.connecting_road].link
-          # print("junction_id: ", junction_id)
-          # print("pre: {} sub: {}".format(link_name.predecessor.contact_point, link_name.successor.contact_point))          
-          incomRoadID = junction_connecting_lane.connecting_road #incoming_road
+        print("junction: {} connected_road: {}, incoming_road: {}.".format(xodr_junction.name, junction_connecting_lane.connecting_road, junction_connecting_lane.incoming_road))
+
+        incomRoadID = junction_connecting_lane.connecting_road #incoming_road
+        junction_id = self.xodr_map.roads[incomRoadID].junction_id 
+        if junction_id == "-1":
+          continue 
+        
+        link_name = self.xodr_map.roads[incomRoadID].link
+        # 每个id对应的road下的section
+        for lanesection_ in self.xodr_map.roads[incomRoadID].lanes.lane_sections:   
           left_boundary_points = []
           right_boundary_points = []  
-          
-          have_right_curb = False           
-          for lanesectionright in lanesection_.right:
-              for roadmark in lanesectionright.road_marks:
-                if roadmark.roadmark_type == "curb":
-                  have_right_curb = True
-
-          for lanesectionright in lanesection_.right: # -            
-            if have_right_curb==True:
-              record_right = False
-              for roadmark in lanesectionright.road_marks:
-                if roadmark.roadmark_type == "curb":
-                  record_right = True
-              if record_right == True:   
-                if incomRoadID in right_incomroadlist:
-                  break
-                right_incomroadlist.append(incomRoadID) 
-                # if len(lanesection_.right)>0 and len(lanesection_.left)>0: 
-                if len(lanesectionright.right_boundary) >0:   
-                  print("__curbe__") 
-                  for points in lanesectionright.right_boundary:              
-                      right_boundary_points.append([points.x, points.y])  
-                # else:
-                #   for points in lanesectionright.right_boundary:              
-                #         right_boundary_points.append([points.x, points.y])   
-                    
-            elif  lanesectionright.lane_type != "driving":# and lanesectionright.lane_type != "shoulder": 
-              # print("laneleft.lane_id.right: ", lanesectionright.lane_id)
-              # print("laneleft.type: ", lanesectionright.lane_type)
+
+          for lanesectionright in lanesection_.right: # driving  shoulder  curb sidewalk
+            if lanesectionright.road_marks[0].roadmark_type in junction_mark_list:                      
               if incomRoadID in right_incomroadlist:
                 break
               right_incomroadlist.append(incomRoadID) 
-              # if len(lanesection_.right)>0 and len(lanesection_.left)>0:  
-              if len(lanesectionright.right_boundary) >0: 
-                print("__tyep__:", lanesectionright.lane_type) 
+              # if len(lanesection_.right)>0 and len(lanesection_.left)>0: 
+              if len(lanesectionright.right_boundary) >0:   
                 for points in lanesectionright.right_boundary:              
                     right_boundary_points.append([points.x, points.y])  
-              # else:
-              #   for points in lanesectionright.right_boundary:              
-              #         right_boundary_points.append([points.x, points.y])          
-
-          # if lanesectionleft.road_marks[0].roadmark_type == "curb":
-          have_left_curb = False           
-          for lanesectionleft in lanesection_.left:
-              for roadmark in lanesectionleft.road_marks:
-                if roadmark.roadmark_type == "curb":
-                  have_left_curb = True
-
-          for lanesectionleft in lanesection_.left: # + 
-            # if lanesectionleft.road_marks[0].roadmark_type == "curb":
-            if have_left_curb==True:
-              record = False
-              for roadmark in lanesectionleft.road_marks:
-                if roadmark.roadmark_type == "curb":
-                  record = True
-              if record == True:   
-                if incomRoadID in left_incomroadlist:
-                  break
-                left_incomroadlist.append(incomRoadID)
-                # if len(lanesection_.right)>0 and len(lanesection_.left)>0:   
-                if len(lanesectionleft.left_boundary) >0:  
-                  print("__curbe__")           
-                  for points in lanesectionleft.left_boundary:                           
-                    left_boundary_points.append([points.x, points.y])
-                # else:
-                #   for points in lanesectionleft.left_boundary:                           
-                #       left_boundary_points.append([points.x, points.y])
-            elif lanesectionleft.lane_type != "driving": # and lanesectionleft.lane_type != "shoulder":
-              # print("laneleft.lane_id.left: ", lanesectionleft.lane_id)
-              # print("laneleft.type: ", lanesectionleft.lane_type)  
+                    
+          for lanesectionleft in lanesection_.left: #  sidewalk curb shoulder driving
+            if lanesectionleft.road_marks[0].roadmark_type in junction_mark_list:  
               if incomRoadID in left_incomroadlist:
                 break
               left_incomroadlist.append(incomRoadID)
-              # if len(lanesection_.right)>0 and len(lanesection_.left)>0:    
-              if len(lanesectionleft.left_boundary) >0:       
-                print("__tyep__:", lanesectionleft.lane_type)      
+              if len(lanesectionleft.left_boundary) >0:           
                 for points in lanesectionleft.left_boundary:                           
                   left_boundary_points.append([points.x, points.y])
-              # else:
-              #   for points in lanesectionleft.left_boundary:                           
-              #       left_boundary_points.append([points.x, points.y])
+                
           
           if len(right_boundary_points)>3:
             boundary_point_temp.append([right_boundary_points, link_name, "right"])
-          elif len(left_boundary_points)>3:  
+          if len(left_boundary_points)>3:  
             boundary_point_temp.append([left_boundary_points, link_name, "left"])
 
-      if len(boundary_point_temp)==3:
-        for i in range(0,len(boundary_point_temp)):
-          point_list_temp,link_name_temp, side = boundary_point_temp[i]
-          if side == "left":
-            if link_name_temp.successor.contact_point == "start" and link_name_temp.predecessor.contact_point == "end":
-              boundary_point_temp[i][0]=point_list_temp[::-1]
-            else:
-              boundary_point_temp[i][0]=point_list_temp
-          # else:
-          #   if link_name_temp.successor.contact_point == "start" and link_name_temp.predecessor.contact_point == "end":
-          #     boundary_point_temp[i][0]=point_list_temp[::-1]
-          #   else:
-          #     boundary_point_temp[i][0]=point_list_temp
-
-      boundary_points = []  
-      point_list_ = []    
-      # for point_list,link_name_ in boundary_point_temp:
-      if len(boundary_point_temp) == 3:
-        point_list_ = boundary_point_temp[0][0]
-        for i in range(1,3):
-          if boundary_point_temp[0][1].successor.element_id == boundary_point_temp[i][1].predecessor.element_id:
-            point_list_.extend(boundary_point_temp[i][0])
-            point_list_.extend(boundary_point_temp[3-i][0])
-            break
-        boundary_points = point_list_
-      elif len(boundary_point_temp) == 4:        
-        for i in range(0,3):          
-          for j in range (i+1, 4):
-            if boundary_point_temp[i][1].successor.element_id == boundary_point_temp[j][1].predecessor.element_id:
-              temp_point_ = boundary_point_temp[i+1][0]
-              temp_name_ = boundary_point_temp[i+1][1]
-              boundary_point_temp[i+1][0] = boundary_point_temp[j][0]
-              boundary_point_temp[j][0] = temp_point_
-
-              boundary_point_temp[i+1][1] = boundary_point_temp[j][1]
-              boundary_point_temp[j][1] = temp_name_
-          boundary_points.extend(boundary_point_temp[i][0])
-        boundary_points.extend(boundary_point_temp[3][0])
-      else:
-        for points, _, _ in boundary_point_temp:
-          boundary_points.extend(points)
+
+      boundary_points = []        
+      for points, _, _ in boundary_point_temp:
+        boundary_points.extend(points)
+
+      if len(boundary_points)<3:
+        return
       
       hull = ConvexHull_lib(np.array(boundary_points))
 
-
       # return boundary_points
       return concave_hull_lib(boundary_points, length_threshold=0, concavity=5, convex_hull_indexes=hull.vertices)
     else:
       print("---------------------convert method error---------------------")
       return   
 
+
+
+
   def convert_junctions(self, method="boundry"):
     for _, xodr_junction in self.xodr_map.junctions.items():
       polygon = self.construct_junction_polygon(xodr_junction, method)
+      if polygon == None:
+        logging.warning(
+          "junction {} polygon is None.".format(xodr_junction.junction_id))
+        continue
       if len(polygon) < 3:
         logging.warning(
           "junction {} polygon size < 3.".format(xodr_junction.junction_id))
         continue
 
       pb_junction = self.pb_map.junction.add()
       pb_junction.id.id = xodr_junction.junction_id
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imap_box_up-0.0.4/imap/lib/convex_hull.py` & `imap_box_up-0.0.5/imap/lib/convex_hull.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/draw.py` & `imap_box_up-0.0.5/imap/lib/draw.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/odr_spiral.py` & `imap_box_up-0.0.5/imap/lib/odr_spiral.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/common.py` & `imap_box_up-0.0.5/imap/lib/opendrive/common.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/header.py` & `imap_box_up-0.0.5/imap/lib/opendrive/header.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/junction.py` & `imap_box_up-0.0.5/imap/lib/opendrive/junction.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/lanes.py` & `imap_box_up-0.0.5/imap/lib/opendrive/lanes.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/map.py` & `imap_box_up-0.0.5/imap/lib/opendrive/map.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/plan_view.py` & `imap_box_up-0.0.5/imap/lib/opendrive/plan_view.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/profile.py` & `imap_box_up-0.0.5/imap/lib/opendrive/profile.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/road.py` & `imap_box_up-0.0.5/imap/lib/opendrive/road.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/signals.py` & `imap_box_up-0.0.5/imap/lib/opendrive/signals.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/opendrive/user_data.py` & `imap_box_up-0.0.5/imap/lib/opendrive/user_data.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/polynoms.py` & `imap_box_up-0.0.5/imap/lib/polynoms.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/proj_helper.py` & `imap_box_up-0.0.5/imap/lib/proj_helper.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/proto_utils.py` & `imap_box_up-0.0.5/imap/lib/proto_utils.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/lib/transform.py` & `imap_box_up-0.0.5/imap/lib/transform.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap/main.py` & `imap_box_up-0.0.5/imap/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,21 @@
     parser = argparse.ArgumentParser(
         description="Imap is a tool to display hdmap info on a map.",
         prog="imap_box_up",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog='eg:\n \
     1.show appollo map by id: imap_box_up -m data/borregas_ave.txt -l lane_35 \n \
     2.Format conversion with UTM map(opendrive->appollo): imap_box_up -f -i data/town.xodr -o data/apollo_map.txt \n \
-    3.Format conversion with relative map(opendrive->appollo.relative map, recommend): imap_box_up -f -r -i data/town.xodr -o data/apollo_map.txt \n \
-    4.if you want convert map junction with box(not recommend): imap_box_up -f -r -b -i data/town.xodr -o data/apollo_map.txt \n \
-    Notice:\n \
+    3.if you want convert map junction with box: imap_box_up -f -r -b -i data/town.xodr -o data/apollo_map.txt \n \
+    4.Format conversion with relative map(opendrive->appollo.relative map): \n \
+    \t \t imap_box_up -f -r -i data/town.xodr -o data/apollo_map.txt \n \
+    \nNotice:\n \
     1.After running the command imap -m data/your_map_file, nothing display and no errors!!! \n \
         step1:Check the permissions: sudo chmod 777 data/your_map_file \n \
-    if step1 no solve the problem, you can try sudo pip install xxx again. \n \
-    2.Other Problem you can contact porter.pan@outlook.com \n \
-    3.code modified from: https://github.com/daohu527/imap '
+    2.Make sure you junction section have curb or shoulder type when not use -b.'
         )
 
     parser.add_argument(
         "-m", "--map", action="store", type=str, required=False,
         help="Specify the map(appollo hdmap) file in txt or binary format, to show")
     parser.add_argument(
         "--save_fig", action="store", type=bool, required=False,
```

### Comparing `imap_box_up-0.0.4/imap/map.py` & `imap_box_up-0.0.5/imap/map.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/imap_box_up.egg-info/PKG-INFO` & `imap_box_up-0.0.5/imap_box_up.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap_box_up
-Version: 0.0.4
+Version: 0.0.5
 Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
 Home-page: https://github.com/porterpan/imap_box_up
 Author: porter
 Author-email: porter.pan@outlook.com
 Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,52 +21,47 @@
 
 # imap_box_up
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
 **[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap/releases/tag/v0.1.7), the imap tool is very useful. 
 
-The name of **imap_box_up** , Just to modified from imap_box
-
-The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
+The name of **imap_box_up** , Just to modified from imap_box and just to distinguish it from **imap_box**
 
 imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-- the map road lane attribution should have curb, if not have curb, task will random selection shouler, stop, walking to create apoolo map.
+- the map road lane attribution should have curb, if not have curb, task will random selection shouler ~~, stop, walking to create apoolo map.~~
 
 - The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to my appollo hdmap code for perception work. 
+
 
+## 新特性1（junction apollo map 显示使用 curbe or shoulder道路属性进行显示，可以实现弧形的显示，而不是原先的box显示junction hd map)
 
-## fix junction bug
+该功能使用默认参数将生成沿着curb或者shoulder绘制的路口地图
 
 ![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
 
-**Supported features**:
-1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
-2. Find lane by id
-3. Convert format: Opendrive to Apollo format.
+如果你要使用原先的box形状显示路口，可以使用参数 -b 即可生成box形状的路口。
 
-| os      | support                 | remark |
-|---------|-------------------------|--------|
-| ubuntu  | :heavy_check_mark:      |        |
-| mac     | :heavy_check_mark:      |        |
-| windows | :heavy_check_mark:      |        |
+## new 2 （添加新的参数-r 以转换为不带有地理坐标的地图数据)
 
-## Related work
-- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
-- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
-- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
+## 地图绘制说明
+
+绘制路口时，确保路口存在curb或者shoulder元素，因为默认非box的junction路口apollo hdmap 需要有这两种元素中的一种或者两种才能正常生成，否则转换后的apollo hdmap 将丢失junction 元素。检查是否有curb属性如下图
+
+![](roadmap_have_junction_or_shoulder.png)
 
 ## Quick start
 
 #### Install
+
 You can install imap by following cmd.
 ```shell
 pip3 install imap_box_up
 ```
 
 ## Example
 #### 1. Visualization
@@ -132,7 +127,24 @@
 ```shell
 sudo chmod 777 data/your_map_file
 ```
 2. Map data permission checking has no problem, still nothing display and no errors!
 A: It's better to install imap_box by running "sudo pip3 install imap_box", then run "imap -m xxx.txt".
 
 > If you have any questions, please feel free to contact me.
+
+
+**Supported features**:
+1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
+2. Find lane by id
+3. Convert format: Opendrive to Apollo format.
+
+| os      | support                 | remark |
+|---------|-------------------------|--------|
+| ubuntu  | :heavy_check_mark:      |        |
+| mac     | :heavy_check_mark:      |        |
+| windows | :heavy_check_mark:      |        |
+
+## Related work
+- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
+- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
+- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imap_box_up-0.0.4/imap_box_up.egg-info/SOURCES.txt` & `imap_box_up-0.0.5/imap_box_up.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.4/setup.py` & `imap_box_up-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imap_box_up",
-    version="0.0.4",
+    version="0.0.5",
     author="porter",
     author_email="porter.pan@outlook.com",
     description="High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/porterpan/imap_box_up",
     project_urls={
```

