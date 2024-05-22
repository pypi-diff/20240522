# Comparing `tmp/pelita-2.3.2.tar.gz` & `tmp/pelita-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelita-2.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pelita-2.4.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pelita-2.3.2.tar` & `pelita-2.4.0rc1.tar`

### file list

```diff
@@ -1,402 +1,403 @@
--rw-r--r--   0        0        0      937 2023-10-16 22:16:14.499610 pelita-2.3.2/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1458 2023-10-16 22:16:14.499610 pelita-2.3.2/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     3116 2023-10-16 22:16:14.499610 pelita-2.3.2/.github/workflows/test_pytest.yml
--rw-r--r--   0        0        0      584 2023-10-16 22:16:14.499610 pelita-2.3.2/.gitignore
--rw-r--r--   0        0        0     1664 2023-10-16 22:16:14.499610 pelita-2.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     1381 2023-10-16 22:16:14.499610 pelita-2.3.2/COPYING
--rw-r--r--   0        0        0      190 2023-10-16 22:16:14.499610 pelita-2.3.2/MANIFEST.in
--rw-r--r--   0        0        0      572 2023-10-16 22:16:14.499610 pelita-2.3.2/README.md
--rw-r--r--   0        0        0     1855 2023-10-16 22:16:14.499610 pelita-2.3.2/README.tournament.md
--rwxr-xr-x   0        0        0      733 2023-10-16 22:16:14.499610 pelita-2.3.2/build-docs.sh
--rw-r--r--   0        0        0     1487 2023-10-16 22:16:14.499610 pelita-2.3.2/check_layout_consistency.py
--rw-r--r--   0        0        0      371 2023-10-16 22:16:14.499610 pelita-2.3.2/contrib/README.txt
--rw-r--r--   0        0        0      363 2023-10-16 22:16:14.499610 pelita-2.3.2/contrib/ci.cfg
--rwxr-xr-x   0        0        0    22092 2023-10-16 22:16:14.499610 pelita-2.3.2/contrib/ci_engine.py
--rw-r--r--   0        0        0     2671 2023-10-16 22:16:14.503611 pelita-2.3.2/demo/benchmark_game.py
--rwxr-xr-x   0        0        0      509 2023-10-16 22:16:14.503611 pelita-2.3.2/demo/demo_run_game.py
--rw-r--r--   0        0        0      638 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/Makefile
--rw-r--r--   0        0        0        9 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/.gitignore
--rw-r--r--   0        0        0        1 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/_static/pelita.css
--rw-r--r--   0        0        0     1980 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/conf.py
--rw-r--r--   0        0        0    93653 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/images/small-game.png
--rw-r--r--   0        0        0    30703 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/images/small-game@2x.png
--rw-r--r--   0        0        0      637 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/index.rst
--rw-r--r--   0        0        0     2299 2023-10-16 22:16:14.503611 pelita-2.3.2/doc/source/info.rst
--rw-r--r--   0        0        0      114 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/__init__.py
--rw-r--r--   0        0        0        0 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/__init__.py
--rw-r--r--   0        0        0     8239 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/_seeds
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/bad/nofood.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/bad/nowalls.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/bad/unreachable_food.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/bad/unreachable_initial.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/bad/wrong_side.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_001.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_002.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_003.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_004.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_005.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_006.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_007.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_008.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_009.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_010.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_011.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_012.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_013.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_014.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_015.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_016.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_017.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_018.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_019.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_020.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_021.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_022.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_023.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_024.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_025.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_026.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_027.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_028.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_029.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_030.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_031.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_032.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_033.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_034.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_035.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_036.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_037.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_038.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_039.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_040.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_041.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_042.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_043.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_044.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_045.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_046.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_047.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_048.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_049.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.503611 pelita-2.3.2/pelita/_layouts/big_050.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_051.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_052.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_053.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_054.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_055.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_056.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_057.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_058.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_059.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_060.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_061.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_062.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_063.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_064.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_065.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_066.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_067.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_068.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_069.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_070.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_071.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_072.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_073.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_074.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_075.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_076.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_077.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_078.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_079.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_080.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_081.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_082.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_083.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_084.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_085.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_086.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_087.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_088.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_089.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_090.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_091.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_092.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_093.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_094.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_095.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_096.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_097.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_098.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_099.layout
--rw-r--r--   0        0        0     2080 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/big_100.layout
--rwxr-xr-x   0        0        0      174 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/bot_replacer.sh
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_001.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_002.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_003.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_004.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_005.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_006.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_007.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_008.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_009.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_010.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_011.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_012.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_013.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_014.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_015.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_016.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_017.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_018.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_019.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_020.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_021.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_022.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_023.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_024.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_025.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_026.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_027.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_028.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_029.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_030.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_031.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_032.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_033.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_034.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_035.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_036.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_037.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_038.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.507611 pelita-2.3.2/pelita/_layouts/normal_039.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_040.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_041.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_042.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_043.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_044.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_045.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_046.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_047.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_048.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_049.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_050.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_051.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_052.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_053.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_054.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_055.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_056.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_057.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_058.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_059.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_060.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_061.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_062.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_063.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_064.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_065.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_066.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_067.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_068.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_069.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_070.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_071.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_072.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_073.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_074.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_075.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_076.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_077.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_078.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_079.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_080.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_081.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_082.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_083.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_084.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_085.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_086.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_087.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_088.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_089.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_090.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_091.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_092.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_093.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_094.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_095.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_096.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_097.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_098.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_099.layout
--rw-r--r--   0        0        0      528 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/normal_100.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_001.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_002.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_003.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_004.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_005.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_006.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_007.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_008.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_009.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_010.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_011.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_012.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_013.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_014.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_015.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_016.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_017.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_018.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_019.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_020.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_021.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_022.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_023.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_024.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_025.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_026.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_027.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_028.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_029.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_030.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_031.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_032.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_033.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_034.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_035.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_036.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_037.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_038.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_039.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_040.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_041.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_042.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_043.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_044.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_045.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_046.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_047.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_048.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_049.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_050.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.511611 pelita-2.3.2/pelita/_layouts/small_051.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_052.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_053.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_054.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_055.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_056.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_057.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_058.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_059.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_060.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_061.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_062.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_063.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_064.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_065.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_066.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_067.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_068.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_069.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_070.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_071.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_072.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_073.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_074.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_075.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_076.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_077.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_078.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_079.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_080.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_081.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_082.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_083.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_084.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_085.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_086.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_087.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_088.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_089.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_090.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_091.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_092.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_093.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_094.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_095.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_096.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_097.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_098.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_099.layout
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/_layouts/small_100.layout
--rw-r--r--   0        0        0      523 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/exceptions.py
--rw-r--r--   0        0        0    36940 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/game.py
--rw-r--r--   0        0        0     4544 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/gamestate_filters.py
--rw-r--r--   0        0        0    13254 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/layout.py
--rw-r--r--   0        0        0    13675 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/maze_generator.py
--rw-r--r--   0        0        0    12473 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/network.py
--rw-r--r--   0        0        0     1009 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/FoodEatingPlayer.py
--rw-r--r--   0        0        0      984 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/RandomExplorerPlayer.py
--rw-r--r--   0        0        0     1007 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/RandomPlayers.py
--rw-r--r--   0        0        0      711 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/SmartEatingPlayer.py
--rw-r--r--   0        0        0      845 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/SmartRandomPlayer.py
--rw-r--r--   0        0        0      157 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/StoppingPlayer.py
--rw-r--r--   0        0        0      628 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/__init__.py
--rw-r--r--   0        0        0     2347 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/player/base.py
--rw-r--r--   0        0        0        0 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/__init__.py
--rwxr-xr-x   0        0        0     2245 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/pelita_createlayout.py
--rwxr-xr-x   0        0        0    15446 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/pelita_main.py
--rwxr-xr-x   0        0        0    13877 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/pelita_player.py
--rwxr-xr-x   0        0        0     2072 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/pelita_tkviewer.py
--rwxr-xr-x   0        0        0    10172 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/pelita_tournament.py
--rw-r--r--   0        0        0      474 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/scripts/script_utils.py
--rw-r--r--   0        0        0    25810 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/team.py
--rw-r--r--   0        0        0    27155 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/tournament/__init__.py
--rw-r--r--   0        0        0    11066 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/tournament/knockout_mode.py
--rw-r--r--   0        0        0     5928 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/tournament/roundrobin.py
--rw-r--r--   0        0        0        0 2023-10-16 22:16:14.515612 pelita-2.3.2/pelita/ui/__init__.py
--rw-r--r--   0        0        0    40734 2023-10-16 22:16:14.519612 pelita-2.3.2/pelita/ui/tk_canvas.py
--rw-r--r--   0        0        0    15510 2023-10-16 22:16:14.519612 pelita-2.3.2/pelita/ui/tk_sprites.py
--rw-r--r--   0        0        0     1111 2023-10-16 22:16:14.519612 pelita-2.3.2/pelita/ui/tk_utils.py
--rw-r--r--   0        0        0     6198 2023-10-16 22:16:14.519612 pelita-2.3.2/pelita/ui/tk_viewer.py
--rw-r--r--   0        0        0    11726 2023-10-16 22:16:14.519612 pelita-2.3.2/pelita/utils.py
--rw-r--r--   0        0        0     6863 2023-10-16 22:16:14.519612 pelita-2.3.2/pelita/viewer.py
--rw-r--r--   0        0        0     1427 2023-10-16 22:16:14.519612 pelita-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      151 2023-10-16 22:16:14.519612 pelita-2.3.2/test/demo01_stopping.py
--rw-r--r--   0        0        0      286 2023-10-16 22:16:14.519612 pelita-2.3.2/test/demo02_random.py
--rw-r--r--   0        0        0      143 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_import_error.py
--rw-r--r--   0        0        0      108 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_bad_args.py
--rw-r--r--   0        0        0      118 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_bad_args_too_many.py
--rw-r--r--   0        0        0      102 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_bad_type.py
--rw-r--r--   0        0        0      107 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_bad_value.py
--rw-r--r--   0        0        0      126 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_division_by_zero.py
--rw-r--r--   0        0        0      147 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_import_error.py
--rw-r--r--   0        0        0      136 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_type_error.py
--rw-r--r--   0        0        0      140 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_move_value_error.py
--rw-r--r--   0        0        0       66 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_no_move.py
--rw-r--r--   0        0        0       67 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_no_name.py
--rw-r--r--   0        0        0       45 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/player_syntax_error.py
--rw-r--r--   0        0        0      153 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/remote_dumps_are_written_blue.py
--rw-r--r--   0        0        0      152 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/remote_dumps_are_written_red.py
--rw-r--r--   0        0        0      137 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/remote_dumps_with_failure_bad.py
--rw-r--r--   0        0        0       55 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/remote_dumps_with_failure_good.py
--rw-r--r--   0        0        0      100 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/remote_timeout_blue.py
--rw-r--r--   0        0        0      157 2023-10-16 22:16:14.519612 pelita-2.3.2/test/fixtures/remote_timeout_red.py
--rw-r--r--   0        0        0    20026 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_filter_gamestates.py
--rw-r--r--   0        0        0    45549 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_game.py
--rw-r--r--   0        0        0       35 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_layout.layout
--rw-r--r--   0        0        0    11712 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_layout.py
--rw-r--r--   0        0        0     3808 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_libpelita.py
--rw-r--r--   0        0        0    14939 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_maze_generation.py
--rw-r--r--   0        0        0     4333 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_network.py
--rw-r--r--   0        0        0     5534 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_pelita_player.py
--rw-r--r--   0        0        0     7677 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_player_base.py
--rw-r--r--   0        0        0     9003 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_players.py
--rw-r--r--   0        0        0     9783 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_remote_game.py
--rw-r--r--   0        0        0    20462 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_team.py
--rw-r--r--   0        0        0    14669 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_tournament.py
--rw-r--r--   0        0        0     2406 2023-10-16 22:16:14.519612 pelita-2.3.2/test/test_utils.py
--rw-r--r--   0        0        0      543 2023-10-16 22:16:14.519612 pelita-2.3.2/tournament.yaml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 pelita-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0      937 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1458 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     3266 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/.github/workflows/test_pytest.yml
+-rw-r--r--   0        0        0      584 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/.gitignore
+-rw-r--r--   0        0        0     1860 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1381 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/COPYING
+-rw-r--r--   0        0        0      190 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/MANIFEST.in
+-rw-r--r--   0        0        0      576 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/README.md
+-rw-r--r--   0        0        0     1855 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/README.tournament.md
+-rwxr-xr-x   0        0        0      740 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/build-docs.sh
+-rw-r--r--   0        0        0     1487 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/check_layout_consistency.py
+-rw-r--r--   0        0        0      371 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/contrib/README.txt
+-rw-r--r--   0        0        0      363 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/contrib/ci.cfg
+-rwxr-xr-x   0        0        0    22092 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/contrib/ci_engine.py
+-rw-r--r--   0        0        0     2671 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/demo/benchmark_game.py
+-rwxr-xr-x   0        0        0      509 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/demo/demo_run_game.py
+-rw-r--r--   0        0        0      638 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/doc/Makefile
+-rw-r--r--   0        0        0        9 2024-05-22 14:57:45.897736 pelita-2.4.0rc1/doc/source/.gitignore
+-rw-r--r--   0        0        0        1 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/doc/source/_static/pelita.css
+-rw-r--r--   0        0        0     1980 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/doc/source/conf.py
+-rw-r--r--   0        0        0    93653 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/doc/source/images/small-game.png
+-rw-r--r--   0        0        0    30703 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/doc/source/images/small-game@2x.png
+-rw-r--r--   0        0        0      637 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/doc/source/index.rst
+-rw-r--r--   0        0        0     2299 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/doc/source/info.rst
+-rw-r--r--   0        0        0      118 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/__init__.py
+-rw-r--r--   0        0        0     8239 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/_seeds
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/bad/nofood.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/bad/nowalls.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/bad/unreachable_food.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/bad/unreachable_initial.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/bad/wrong_side.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_001.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_002.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_003.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_004.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_005.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_006.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_007.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_008.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_009.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_010.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_011.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_012.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_013.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_014.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_015.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_016.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_017.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_018.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_019.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_020.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_021.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_022.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_023.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_024.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_025.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_026.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_027.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_028.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_029.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_030.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_031.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_032.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_033.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_034.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_035.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_036.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_037.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_038.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_039.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_040.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_041.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_042.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_043.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_044.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_045.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_046.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_047.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_048.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_049.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_050.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_051.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_052.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_053.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.901737 pelita-2.4.0rc1/pelita/_layouts/big_054.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_055.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_056.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_057.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_058.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_059.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_060.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_061.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_062.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_063.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_064.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_065.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_066.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_067.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_068.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_069.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_070.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_071.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_072.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_073.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_074.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_075.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_076.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_077.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_078.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_079.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_080.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_081.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_082.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_083.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_084.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_085.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_086.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_087.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_088.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_089.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_090.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_091.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_092.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_093.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_094.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_095.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_096.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_097.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_098.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_099.layout
+-rw-r--r--   0        0        0     2080 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/big_100.layout
+-rwxr-xr-x   0        0        0      174 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/bot_replacer.sh
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_001.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_002.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_003.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_004.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_005.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_006.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_007.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_008.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_009.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_010.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_011.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_012.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_013.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_014.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_015.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_016.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_017.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_018.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_019.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_020.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_021.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_022.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_023.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_024.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_025.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_026.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_027.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_028.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_029.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_030.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_031.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_032.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_033.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_034.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.905737 pelita-2.4.0rc1/pelita/_layouts/normal_035.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_036.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_037.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_038.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_039.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_040.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_041.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_042.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_043.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_044.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_045.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_046.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_047.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_048.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_049.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_050.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_051.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_052.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_053.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_054.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_055.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_056.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_057.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_058.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_059.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_060.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_061.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_062.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_063.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_064.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_065.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_066.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_067.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_068.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_069.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_070.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_071.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_072.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_073.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_074.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_075.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_076.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_077.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_078.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_079.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_080.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_081.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_082.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_083.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_084.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_085.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_086.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_087.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_088.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_089.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_090.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_091.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_092.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_093.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_094.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_095.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_096.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_097.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_098.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_099.layout
+-rw-r--r--   0        0        0      528 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/normal_100.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_001.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_002.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_003.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_004.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_005.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_006.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_007.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_008.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_009.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_010.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_011.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_012.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_013.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_014.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_015.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_016.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_017.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_018.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_019.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_020.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_021.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_022.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_023.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_024.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_025.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_026.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_027.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_028.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_029.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_030.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_031.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_032.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_033.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_034.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_035.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_036.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_037.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_038.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_039.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_040.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_041.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_042.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_043.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.909736 pelita-2.4.0rc1/pelita/_layouts/small_044.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_045.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_046.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_047.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_048.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_049.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_050.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_051.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_052.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_053.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_054.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_055.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_056.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_057.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_058.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_059.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_060.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_061.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_062.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_063.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_064.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_065.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_066.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_067.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_068.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_069.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_070.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_071.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_072.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_073.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_074.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_075.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_076.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_077.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_078.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_079.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_080.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_081.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_082.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_083.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_084.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_085.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_086.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_087.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_088.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_089.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_090.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_091.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_092.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_093.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_094.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_095.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_096.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_097.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_098.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_099.layout
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/_layouts/small_100.layout
+-rw-r--r--   0        0        0      523 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/exceptions.py
+-rw-r--r--   0        0        0    37304 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/game.py
+-rw-r--r--   0        0        0     4544 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/gamestate_filters.py
+-rw-r--r--   0        0        0    13254 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/layout.py
+-rw-r--r--   0        0        0    13675 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/maze_generator.py
+-rw-r--r--   0        0        0    11858 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/network.py
+-rw-r--r--   0        0        0     1009 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/FoodEatingPlayer.py
+-rw-r--r--   0        0        0      984 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/RandomExplorerPlayer.py
+-rw-r--r--   0        0        0     1007 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/RandomPlayers.py
+-rw-r--r--   0        0        0      711 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/SmartEatingPlayer.py
+-rw-r--r--   0        0        0      845 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/SmartRandomPlayer.py
+-rw-r--r--   0        0        0      157 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/StoppingPlayer.py
+-rw-r--r--   0        0        0      628 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/player/base.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/__init__.py
+-rwxr-xr-x   0        0        0     2245 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/pelita_createlayout.py
+-rwxr-xr-x   0        0        0    18390 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/pelita_main.py
+-rwxr-xr-x   0        0        0    10258 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/pelita_player.py
+-rwxr-xr-x   0        0        0    21455 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/pelita_server.py
+-rwxr-xr-x   0        0        0     2072 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/pelita_tkviewer.py
+-rwxr-xr-x   0        0        0    10172 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/pelita_tournament.py
+-rw-r--r--   0        0        0      474 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/scripts/script_utils.py
+-rw-r--r--   0        0        0    28344 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/team.py
+-rw-r--r--   0        0        0    27155 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/tournament/__init__.py
+-rw-r--r--   0        0        0    11066 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/tournament/knockout_mode.py
+-rw-r--r--   0        0        0     5928 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/tournament/roundrobin.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:57:45.913736 pelita-2.4.0rc1/pelita/ui/__init__.py
+-rw-r--r--   0        0        0    40734 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pelita/ui/tk_canvas.py
+-rw-r--r--   0        0        0    15510 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pelita/ui/tk_sprites.py
+-rw-r--r--   0        0        0     1111 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pelita/ui/tk_utils.py
+-rw-r--r--   0        0        0     6198 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pelita/ui/tk_viewer.py
+-rw-r--r--   0        0        0    10277 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pelita/utils.py
+-rw-r--r--   0        0        0     7478 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pelita/viewer.py
+-rw-r--r--   0        0        0     1492 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      151 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/demo01_stopping.py
+-rw-r--r--   0        0        0      286 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/demo02_random.py
+-rw-r--r--   0        0        0      143 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_import_error.py
+-rw-r--r--   0        0        0      108 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_bad_args.py
+-rw-r--r--   0        0        0      118 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_bad_args_too_many.py
+-rw-r--r--   0        0        0      102 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_bad_type.py
+-rw-r--r--   0        0        0      107 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_bad_value.py
+-rw-r--r--   0        0        0      126 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_division_by_zero.py
+-rw-r--r--   0        0        0      147 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_import_error.py
+-rw-r--r--   0        0        0      136 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_type_error.py
+-rw-r--r--   0        0        0      140 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_move_value_error.py
+-rw-r--r--   0        0        0       66 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_no_move.py
+-rw-r--r--   0        0        0       67 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_no_name.py
+-rw-r--r--   0        0        0       45 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/player_syntax_error.py
+-rw-r--r--   0        0        0      153 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/remote_dumps_are_written_blue.py
+-rw-r--r--   0        0        0      152 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/remote_dumps_are_written_red.py
+-rw-r--r--   0        0        0      137 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/remote_dumps_with_failure_bad.py
+-rw-r--r--   0        0        0       55 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/remote_dumps_with_failure_good.py
+-rw-r--r--   0        0        0      100 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/remote_timeout_blue.py
+-rw-r--r--   0        0        0      157 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/fixtures/remote_timeout_red.py
+-rw-r--r--   0        0        0    20026 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_filter_gamestates.py
+-rw-r--r--   0        0        0    45549 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_game.py
+-rw-r--r--   0        0        0       35 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_layout.layout
+-rw-r--r--   0        0        0    11712 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_layout.py
+-rw-r--r--   0        0        0     3808 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_libpelita.py
+-rw-r--r--   0        0        0    14939 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_maze_generation.py
+-rw-r--r--   0        0        0     3511 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_network.py
+-rw-r--r--   0        0        0     5534 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_pelita_player.py
+-rw-r--r--   0        0        0     7677 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_player_base.py
+-rw-r--r--   0        0        0     9003 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_players.py
+-rw-r--r--   0        0        0     9508 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_remote_game.py
+-rw-r--r--   0        0        0    22889 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_team.py
+-rw-r--r--   0        0        0    14669 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_tournament.py
+-rw-r--r--   0        0        0     2406 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/test/test_utils.py
+-rw-r--r--   0        0        0      543 2024-05-22 14:57:45.917737 pelita-2.4.0rc1/tournament.yaml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 pelita-2.4.0rc1/PKG-INFO
```

### Comparing `pelita-2.3.2/.github/workflows/build_docs.yml` & `pelita-2.4.0rc1/.github/workflows/build_docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   deploy_docs:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0 # fetch all history and tags (needed for git describe)
     - name: Set up Python 3.12
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.12'
     - name: Install sphinx and prepare repo
       run: |
         python -m pip install --upgrade pip
         python -m pip install sphinx
         pip install -e .
```

### Comparing `pelita-2.3.2/.github/workflows/pypi_release.yml` & `pelita-2.4.0rc1/.github/workflows/pypi_release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   build-and-publish:
     name: Build and publish Python distributions to PyPI and TestPyPI
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python 3.12
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.12'
 
     - name: Install flit
       run: python -m pip install flit
 
     - name: Build a binary wheel and a source tarball
```

### Comparing `pelita-2.3.2/.github/workflows/test_pytest.yml` & `pelita-2.4.0rc1/.github/workflows/test_pytest.yml`

 * *Files 13% similar despite different names*

```diff
@@ -7,39 +7,44 @@
     branches: [ main ]
 
 jobs:
   pytest:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.9, "3.10", "3.11", "3.12"]
+        os: [ubuntu-latest, macos-latest, windows-latest, macos-13]
+        python-version: ['3.9', '3.10', '3.11', '3.12']
+        exclude:
+          - os: macos-latest
+            python-version: '3.9'
+          - os: macos-13
+            python-version: '3.10'
+          - os: macos-13
+            python-version: '3.11'
+          - os: macos-13
+            python-version: '3.12'
     timeout-minutes: 15
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest-cov
         python -m pip install pytest-timestamper # this plugin adds timestamps to the output
         python -m pip install -e .
         python -c "import zmq; print('Using pyzmq {} and zmq {}.'.format(zmq.pyzmq_version(), zmq.zmq_version()))"
     - name: Test with pytest
       run: |
         python -m pytest -v -s --cov=./pelita/ test/
       timeout-minutes: 8
-    - name: "Upload coverage to Codecov"
-      uses: codecov/codecov-action@v3
-      with:
-        fail_ci_if_error: true
 
     - name: Upload coverage data to coveralls.io
       uses: AndreMiras/coveralls-python-action@develop
       if: runner.os == 'Linux' # Only works on Linux
       with:
         github-token: ${{ secrets.github_token }}
         flag-name: run-${{ matrix.os }}-py-${{ matrix.python-version }}
@@ -79,15 +84,15 @@
         os: [ubuntu-latest, macos-latest]
         python-version: ["3.10", "3.11", "3.12"]
     timeout-minutes: 15
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .
         python -c "import zmq; print('Using pyzmq {} and zmq {}.'.format(zmq.pyzmq_version(), zmq.zmq_version()))"
```

### Comparing `pelita-2.3.2/.gitignore` & `pelita-2.4.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/CHANGELOG.md` & `pelita-2.4.0rc1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Pelita changelog
 
+  * v2.4.0 (xx. May 2024)
+
+     - Greatly improved server mode
+     - Bot.legal_positions becomes a static attribute
+     - Bot has a new cached attribute graph
+     - Small timeout improvements
+
   * v2.3.2 (16. Oct 2023)
 
      - Give advice when tkinter is not available
      - Fix colours in --ascii mode on Windows
      - Improved --progress bar
 
   * v2.3.1 (2. Sep 2023)
```

### Comparing `pelita-2.3.2/COPYING` & `pelita-2.4.0rc1/COPYING`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/README.md` & `pelita-2.4.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pelita
 
-[![Build Status](https://github.com/ASPP/pelita/actions/workflows/push_ci.yml/badge.svg?branch=main)](https://github.com/ASPP/pelita/actions)
+[![Build Status](https://github.com/ASPP/pelita/actions/workflows/test_pytest.yml/badge.svg?branch=main)](https://github.com/ASPP/pelita/actions)
 
 ## Description
 
 Pelita is a programmable game that lets you play against your opponent by writing code in Python.
 
 ![](doc/source/images/small-game.png)
```

### Comparing `pelita-2.3.2/README.tournament.md` & `pelita-2.4.0rc1/README.tournament.md`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/build-docs.sh` & `pelita-2.4.0rc1/build-docs.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 
 set -Eeuo pipefail
 
 # get the 'git describe' output
-git_describe=$(git describe)
+git_describe=$(git describe --tags)
 
 # make the documentation, hope it doesn't fail
 echo "Generating doc from $git_describe"
 
 # Generate _contributors.rst
 CONTRIBUTORS=doc/source/_contributors.rst
```

### Comparing `pelita-2.3.2/check_layout_consistency.py` & `pelita-2.4.0rc1/check_layout_consistency.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/contrib/ci_engine.py` & `pelita-2.4.0rc1/contrib/ci_engine.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/demo/benchmark_game.py` & `pelita-2.4.0rc1/demo/benchmark_game.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/doc/Makefile` & `pelita-2.4.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/doc/source/conf.py` & `pelita-2.4.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/doc/source/images/small-game.png` & `pelita-2.4.0rc1/doc/source/images/small-game.png`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/doc/source/images/small-game@2x.png` & `pelita-2.4.0rc1/doc/source/images/small-game@2x.png`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/doc/source/index.rst` & `pelita-2.4.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/doc/source/info.rst` & `pelita-2.4.0rc1/doc/source/info.rst`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/_seeds` & `pelita-2.4.0rc1/pelita/_layouts/_seeds`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/bad/nowalls.layout` & `pelita-2.4.0rc1/pelita/_layouts/bad/nowalls.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/bad/unreachable_food.layout` & `pelita-2.4.0rc1/pelita/_layouts/bad/unreachable_food.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/bad/unreachable_initial.layout` & `pelita-2.4.0rc1/pelita/_layouts/bad/unreachable_initial.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/bad/wrong_side.layout` & `pelita-2.4.0rc1/pelita/_layouts/bad/wrong_side.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_001.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_001.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_002.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_002.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_003.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_003.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_004.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_004.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_005.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_005.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_006.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_006.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_007.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_007.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_008.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_008.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_009.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_009.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_010.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_010.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_011.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_011.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_012.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_012.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_013.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_013.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_014.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_014.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_015.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_015.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_016.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_016.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_017.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_017.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_018.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_018.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_019.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_019.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_020.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_020.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_021.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_021.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_022.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_022.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_023.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_023.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_024.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_024.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_025.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_025.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_026.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_026.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_027.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_027.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_028.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_028.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_029.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_029.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_030.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_030.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_031.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_031.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_032.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_032.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_033.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_033.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_034.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_034.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_035.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_035.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_036.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_036.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_037.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_037.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_038.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_038.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_039.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_039.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_040.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_040.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_041.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_041.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_042.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_042.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_043.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_043.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_044.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_044.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_045.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_045.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_046.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_046.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_047.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_047.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_048.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_048.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_049.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_049.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_050.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_050.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_051.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_051.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_052.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_052.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_053.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_053.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_054.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_054.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_055.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_055.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_056.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_056.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_057.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_057.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_058.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_058.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_059.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_059.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_060.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_060.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_061.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_061.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_062.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_062.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_063.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_063.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_064.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_064.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_065.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_065.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_066.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_066.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_067.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_067.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_068.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_068.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_069.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_069.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_070.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_070.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_071.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_071.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_072.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_072.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_073.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_073.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_074.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_074.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_075.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_075.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_076.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_076.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_077.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_077.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_078.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_078.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_079.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_079.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_080.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_080.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_081.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_081.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_082.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_082.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_083.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_083.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_084.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_084.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_085.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_085.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_086.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_086.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_087.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_087.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_088.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_088.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_089.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_089.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_090.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_090.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_091.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_091.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_092.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_092.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_093.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_093.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_094.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_094.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_095.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_095.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_096.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_096.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_097.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_097.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_098.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_098.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_099.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_099.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/big_100.layout` & `pelita-2.4.0rc1/pelita/_layouts/big_100.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_001.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_001.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_002.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_002.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_003.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_003.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_004.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_004.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_005.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_005.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_006.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_006.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_007.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_007.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_008.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_008.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_009.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_009.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_010.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_010.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_011.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_011.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_012.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_012.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_013.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_013.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_014.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_014.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_015.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_015.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_016.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_016.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_017.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_017.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_018.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_018.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_019.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_019.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_020.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_020.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_021.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_021.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_022.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_022.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_023.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_023.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_024.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_024.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_025.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_025.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_026.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_026.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_027.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_027.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_028.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_028.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_029.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_029.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_030.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_030.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_031.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_031.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_032.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_032.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_033.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_033.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_034.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_034.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_035.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_035.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_036.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_036.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_037.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_037.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_038.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_038.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_039.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_039.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_040.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_040.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_041.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_041.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_042.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_042.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_043.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_043.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_044.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_044.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_045.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_045.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_046.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_046.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_047.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_047.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_048.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_048.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_049.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_049.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_050.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_050.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_051.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_051.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_052.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_052.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_053.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_053.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_054.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_054.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_055.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_055.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_056.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_056.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_057.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_057.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_058.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_058.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_059.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_059.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_060.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_060.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_061.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_061.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_062.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_062.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_063.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_063.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_064.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_064.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_065.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_065.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_066.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_066.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_067.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_067.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_068.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_068.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_069.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_069.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_070.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_070.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_071.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_071.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_072.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_072.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_073.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_073.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_074.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_074.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_075.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_075.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_076.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_076.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_077.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_077.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_078.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_078.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_079.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_079.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_080.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_080.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_081.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_081.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_082.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_082.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_083.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_083.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_084.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_084.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_085.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_085.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_086.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_086.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_087.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_087.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_088.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_088.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_089.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_089.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_090.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_090.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_091.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_091.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_092.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_092.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_093.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_093.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_094.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_094.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_095.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_095.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_096.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_096.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_097.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_097.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_098.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_098.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_099.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_099.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/_layouts/normal_100.layout` & `pelita-2.4.0rc1/pelita/_layouts/normal_100.layout`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/exceptions.py` & `pelita-2.4.0rc1/pelita/exceptions.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/game.py` & `pelita-2.4.0rc1/pelita/game.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             viewer_state['viewers'].append(ProgressViewer())
         elif len(viewer) == 2 and viewer[0] == 'reply-to':
             viewer_state['viewers'].append(ReplyToViewer(viewer[1]))
         elif len(viewer) == 2 and viewer[0] == 'write-replay-to':
             viewer_state['viewers'].append(ReplayWriter(open(viewer[1], 'w')))
         elif viewer in ('tk', 'tk-no-sync'):
             if not zmq_publisher:
-                zmq_publisher = ZMQPublisher(address='tcp://127.0.0.1:*')
+                zmq_publisher = ZMQPublisher(address='tcp://127.0.0.1')
                 viewer_state['viewers'].append(zmq_publisher)
             if viewer == 'tk':
                 viewer_state['controller'] = setup_controller()
             if viewer_state['controller']:
                 proc = TkViewer(address=zmq_publisher.socket_addr, controller=viewer_state['controller'].socket_addr,
                                 stop_after=options.get('stop_at'),
                                 geometry=options.get('geometry'),
@@ -502,20 +502,26 @@
 
 def prepare_bot_state(game_state, idx=None):
     """ Prepares the bot’s game state for the current bot.
 
     """
 
     bot_initialization = game_state.get('turn') is None and idx is not None
+    bot_finalization = game_state.get('turn') is not None and idx is not None
 
     if bot_initialization:
         # We assume that we are in get_initial phase
         turn = idx
         bot_turn = None
         seed = game_state['rnd'].randint(0, sys.maxsize)
+    elif bot_finalization:
+        # Called for remote players in _exit
+        turn = idx
+        bot_turn = None
+        seed = None
     else:
         turn = game_state['turn']
         bot_turn = game_state['turn'] // 2
         seed = None
 
     bot_position = game_state['bots'][turn]
     own_team = turn % 2
@@ -566,15 +572,16 @@
     }
 
     bot_state = {
         'team': team_state,
         'enemy': enemy_state,
         'round': game_state['round'],
         'bot_turn': bot_turn,
-        'timeout_length': game_state['timeout_length']
+        'timeout_length': game_state['timeout_length'],
+        'max_rounds': game_state['max_rounds'],
     }
 
     if bot_initialization:
         bot_state.update({
             'walls': game_state['walls'], # only in initial round
             'shape': game_state['shape'], # only in initial round
             'seed': seed # only used in set_initial phase
@@ -972,17 +979,18 @@
     return { 'whowins' : None, 'gameover' : False}
 
 
 def check_exit_remote_teams(game_state):
     """ If the we are gameover, we want the remote teams to shut down. """
     if game_state['gameover']:
         _logger.info("Gameover. Telling teams to exit.")
-        for team in game_state['teams']:
+        for idx, team in enumerate(game_state['teams']):
             try:
-                team._exit()
+                team_game_state = prepare_bot_state(game_state, idx=idx)
+                team._exit(team_game_state)
             except AttributeError:
                 pass
 
 
 def game_print(turn, msg):
     allow_unicode = not _mswindows
     if turn % 2 == 0:
```

### Comparing `pelita-2.3.2/pelita/gamestate_filters.py` & `pelita-2.4.0rc1/pelita/gamestate_filters.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/layout.py` & `pelita-2.4.0rc1/pelita/layout.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/maze_generator.py` & `pelita-2.4.0rc1/pelita/maze_generator.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/network.py` & `pelita-2.4.0rc1/pelita/network.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 
 import json
 import logging
-import re
 import sys
 import time
+from urllib.parse import urlparse
 import uuid
 
 import zmq
 
 _logger = logging.getLogger(__name__)
 
+# 41736 is the word PELI(T)A when read upside down in reverse without glasses
+# The missing T stands for tcp
+PELITA_PORT = 41736
+
 ## Pelita network data structures
 
 # ControlRequest
 # {__action__}
 
 # ViewerUpdate
 # {__action__, __data__}
@@ -45,50 +49,28 @@
         super().__init__(message, error_type, *args)
 
 
 #: The timeout to use during sending
 DEAD_CONNECTION_TIMEOUT = 3.0
 
 
-def extract_port_range(address):
-    """ We additionally allow for setting a port range in rectangular brackets:
-        tcp://127.0.0.1:[50100:50120]
-    """
-    range_pattern = re.compile(r"(?P<addr>.*?):\[(?P<port_min>\d+):(?P<port_max>\d+)\]")
-    random_pattern = re.compile(r"(?P<addr>.*?):\*")
-    port_pattern = re.compile(r"(?P<addr>.*?):(?P<port>\d+)")
-
-    m = range_pattern.match(address)
-    if m:
-        return {"addr": m.group(1), "port_min": int(m.group(2)), "port_max": int(m.group(3))}
-    m = random_pattern.match(address)
-    if m:
-        return {"addr": m.group(1), "port_min": None, "port_max": None}
-    m = port_pattern.match(address)
-    if m:
-        return {"addr": address}
-    return {"addr": address}
+def bind_socket(socket: zmq.Socket, address, option_hint=None):
+    parsed_address = urlparse(address)
 
-def bind_socket(socket, address, option_hint=None):
-    try:
-        address_range = extract_port_range(address)
-        addr = address_range["addr"]
-        try:
-            port_min = address_range["port_min"]
-            port_max = address_range["port_max"]
-            if port_min and port_max:
-                port = socket.bind_to_random_port(addr, port_min, port_max)
-            else:
-                port = socket.bind_to_random_port(addr)
-            bind_addr = "{0}:{1}".format(addr, port)
-            return bind_addr
+    # NB: We cannot use parsed_address.geturl() to generate a nice url for zmq
+    # as this will eat the empty hostname in a file path and zmq does not like that.
+    # file:///tmp/a -> file:/tmp/a
 
-        except KeyError:
-            socket.bind(addr)
-            return addr
+    try:
+        if parsed_address.scheme == 'tcp' and parsed_address.port is None:
+            port = socket.bind_to_random_port(address)
+            return f'tcp://{parsed_address.hostname}:{port}'
+        else:
+            socket.bind(address)
+            return address
 
     except (zmq.ZMQError, zmq.ZMQBindError) as e:
         print('error binding to address %s: %s' % (address, e), file=sys.stderr)
         if option_hint:
             print('use %s <address> to specify a different port' %\
                 (option_hint,), file=sys.stderr)
         raise
@@ -311,15 +293,15 @@
         self.socket.send_unicode(as_json)
 
     def show_state(self, game_state):
         self._send(action="observe", data=game_state)
 
 
 class Controller:
-    def __init__(self, address='tcp://127.0.0.1:*', zmq_context=None):
+    def __init__(self, address='tcp://127.0.0.1', zmq_context=None):
         self.address = address
         if zmq_context:
             self.context = zmq_context
         else:
             self.context = zmq.Context()
         # We use a ROUTER which we bind.
         # This means other DEALERs can connect and
```

### Comparing `pelita-2.3.2/pelita/player/FoodEatingPlayer.py` & `pelita-2.4.0rc1/pelita/player/FoodEatingPlayer.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/player/RandomExplorerPlayer.py` & `pelita-2.4.0rc1/pelita/player/RandomExplorerPlayer.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/player/RandomPlayers.py` & `pelita-2.4.0rc1/pelita/player/RandomPlayers.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/player/SmartEatingPlayer.py` & `pelita-2.4.0rc1/pelita/player/SmartEatingPlayer.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/player/SmartRandomPlayer.py` & `pelita-2.4.0rc1/pelita/player/SmartRandomPlayer.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/player/__init__.py` & `pelita-2.4.0rc1/pelita/player/__init__.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/player/base.py` & `pelita-2.4.0rc1/pelita/player/base.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/scripts/pelita_createlayout.py` & `pelita-2.4.0rc1/pelita/scripts/pelita_createlayout.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/scripts/pelita_main.py` & `pelita-2.4.0rc1/pelita/scripts/pelita_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import argparse
 import json
 import logging
 from pathlib import Path
 import random
 import sys
+from urllib.parse import urlparse
 
 from rich.console import Console
+from rich.markup import escape
 from rich.prompt import Prompt
+import zmq
 
 import pelita
 from .script_utils import start_logging
 
+from pelita.network import PELITA_PORT
 # TODO: The check_team option
 from pelita.tournament import check_team
 
 # silence stupid warnings from logging module
 logging.root.manager.emittedNoHandlerWarning = 1
 _logger = logging.getLogger(__name__)
 
@@ -25,29 +29,35 @@
     if team_spec != "SCAN":
         return team_spec
     from zeroconf import ServiceBrowser, ServiceStateChange, Zeroconf
     from queue import Queue, Empty
 
     SCAN_TIME = 5 # seconds
 
-    q = Queue(maxsize=5)
+    q = Queue(maxsize=20)
 
     def on_service_state_change(
         zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange
     ) -> None:
 
         if state_change is ServiceStateChange.Added:
             info = zeroconf.get_service_info(service_type, name)
 
+            def make_url(addr, port):
+                if port == PELITA_PORT:
+                    return f"pelita://{addr}"
+                else:
+                    return f"pelita://{addr}:{port}"
+
             if info:
-                addresses = ["%s:%d" % (addr, info.port) for addr in info.parsed_scoped_addresses()]
+                addresses = [make_url(addr, info.port) for addr in info.parsed_scoped_addresses()]
 
-                addr = f"tcp://{addresses[0]}"
                 team_name = info.properties[b"team_name"].decode()
-                q.put((addr, team_name), timeout=5)
+                path = info.properties[b"path"].decode()
+                q.put((addresses[0] + path, team_name), timeout=5)
 
     zeroconf = Zeroconf()
     services = ["_pelita-player._tcp.local."]
     console = Console()
 
     console.print(f"[bold]Remote player requested. Scanning network for players ({SCAN_TIME}s).")
     with console.status("[red bold]Searching for other players …") as status:
@@ -89,25 +99,88 @@
         elif answer in choices.keys():
             console.print(f"Choosing [blue]{choices[answer]}[/]", highlight=False)
             return choices[answer]
         else:
             return None
 
 
+def scan_server(team_spec):
+    parsed_url = urlparse(team_spec)
+    if parsed_url.port:
+        port = parsed_url.port
+    else:
+        port = PELITA_PORT
+
+    send_addr = f"tcp://{parsed_url.hostname}:{port}"
+
+    zmq_context = zmq.Context()
+    socket = zmq_context.socket(zmq.DEALER)
+    socket.setsockopt(zmq.LINGER, 0)
+    socket.connect(send_addr)
+    socket.send_json({"SCAN": team_spec})
+
+    console = Console()
+
+    console.print(f"[bold]Remote player requested. Scanning server for players.")
+
+    WAIT_TIMEOUT = 5000
+    incoming = socket.poll(timeout=WAIT_TIMEOUT)
+    if incoming == zmq.POLLIN:
+        teams = json.loads(socket.recv().decode('utf8'))
+        if not teams:
+            console.print("No teams found on the server :(")
+            return None
+        else:
+            print("Server has the following teams available")
+    else:
+        console.print(f"Server did not reply in {WAIT_TIMEOUT} ms.")
+        return None
+
+    players = []
+    for addr, team_name in teams.items():
+        console.print(f"  [blue]{len(players)})[/] {team_name} \\[[blue]{addr}[/]]", highlight=False)
+        players.append(addr)
+
+    if players:
+        console.print(f"  [blue]r)[/] Random team")
+        console.print(f"  [blue]s)[/] Server default")
+        console.print(f"  [blue]x)[/] Exit")
+        console.print()
+        console.print(f"Found {len(players)} player{'s' if len(players) != 1 else ''}.")
+
+        choices = {str(i): player for i, player in enumerate(players)}
+
+        answer = Prompt.ask("[bold]Select player to play against (r for random, s server’s choice, x to exit)",
+                            choices=list(choices) + ["r", "s", "x"],
+                            default="r")
+
+        if answer == "r":
+            console.print("Choosing random player.")
+            return random.choice(players)
+        if answer == "s":
+            console.print("Letting the server choose.")
+            return team_spec
+        elif answer in choices.keys():
+            console.print(f"Choosing [blue]{choices[answer]}[/]", highlight=False)
+            return choices[answer]
+        else:
+            return None
+
+
 def geometry_string(s):
     """Get a X-style geometry definition and return a tuple.
 
     600x400 -> (600,400)
     """
     try:
         x_string, y_string = s.split('x')
         geometry = (int(x_string), int(y_string))
     except ValueError:
         msg = "%s is not a valid geometry specification" %s
-        raise argparse.ArgumentTypeError(msg)
+        raise argparse.ArgumentTypeError(msg) from None
     return geometry
 
 
 def long_help(s):
     return s if '--long-help' in sys.argv else argparse.SUPPRESS
 
 parser = argparse.ArgumentParser(description='Run a single pelita game',
@@ -194,17 +267,17 @@
                                help=long_help('Communicate the result of the game on this channel.'))
 
 publisher_opt = advanced_settings.add_mutually_exclusive_group()
 publisher_opt.add_argument('--publish', type=str, metavar='URL', dest='publish_to',
                            help=long_help('Publish the game to this zmq socket.'))
 publisher_opt.add_argument('--no-publish', const=False, action='store_const', dest='publish_to',
                            help=long_help('Do not publish.'))
-parser.set_defaults(publish_to="tcp://127.0.0.1:*")
+parser.set_defaults(publish_to="tcp://127.0.0.1")
 
-advanced_settings.add_argument('--controller', type=str, metavar='URL', default="tcp://127.0.0.1:*",
+advanced_settings.add_argument('--controller', type=str, metavar='URL', default="tcp://127.0.0.1",
                                help=long_help('Channel for controlling the game.'))
 advanced_settings.add_argument('--external-controller', const=True, action='store_const',
                                help=long_help('Force control by an external controller.'))
 
 parser.epilog = """\
 Team Specification:
     A team consists of a path to a .py file or to a Python module
@@ -331,14 +404,24 @@
         if team_spec == "SCAN":
             scanned_spec = scan(team_spec)
             if scanned_spec:
                 team_specs[idx] = scanned_spec
             else:
                 print("No remote team found. Exiting.")
                 return
+        elif team_spec.startswith("pelita://"):
+            # check if we need to send a server scan request
+            parsed_url = urlparse(team_spec)
+            if parsed_url.path in ('', '/'):
+                scanned_spec = scan_server(team_spec)
+                if scanned_spec:
+                    team_specs[idx] = scanned_spec
+                else:
+                    print("No remote team selected. Exiting.")
+                    return
 
     if args.seed is None:
         seed = random.randint(0, sys.maxsize)
         print("Replay this game with --seed {seed}".format(seed=seed))
     else:
         seed = args.seed
```

### Comparing `pelita-2.3.2/pelita/scripts/pelita_player.py` & `pelita-2.4.0rc1/pelita/scripts/pelita_player.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 #!/usr/bin/env python3
 
-import argparse
 import contextlib
 import importlib
 import json
 import logging
 from pathlib import Path
-import signal
-import subprocess
 import sys
-from urllib.parse import urlparse
 
-import zeroconf
+import click
 import zmq
 
 import pelita
 from ..team import make_team
 from ..network import json_default_handler
 from .script_utils import start_logging
 
 _logger = logging.getLogger(__name__)
 
 
-zeroconf.log.setLevel(logging.DEBUG)
-zeroconf.log.addHandler(_logger)
-
 @contextlib.contextmanager
 def with_sys_path(dirname):
     sys.path.insert(0, dirname)
     try:
         yield
     finally:
         sys.path.remove(dirname)
 
-
-def run_player(team_spec, address, color=None):
+def run_player(team_spec, address, team_name_override=False, silent_bots=False):
     """ Creates a team from `team_spec` and runs
     a game through the zmq PAIR socket on `address`.
 
     Parameters
     ----------
     team_spec : str
         path to the module that declares the team
     address : address to zmq PAIR socket
         the address of the remote team socket
-    color : string, optional
-        the color of the team (for nicer output)
 
     """
 
     address = address.replace('*', 'localhost')
     # Connect to the given address
     context = zmq.Context()
     socket = context.socket(zmq.PAIR)
@@ -80,32 +70,23 @@
             raise IOError('failed to connect the client to address %s: %s'
                           % (address, e))
         # TODO: Do not raise here but wait for zmq to return a sensible error message
         # We need a way to distinguish between syntax errors in the client
         # and general zmq disconnects
         raise
 
-    if color == 'blue':
-        pie = '\033[94m' + 'ᗧ' + '\033[0m'
-    elif color == 'red':
-        pie = '\033[91m' + 'ᗧ' + '\033[0m'
-    else:
-        pie = 'ᗧ'
-    if pelita.game._mswindows:
-        print(f"{color} team '{team_spec}' -> '{team.team_name}'")
-    else:
-        print(f"{pie} {color} team '{team_spec}' -> '{team.team_name}'")
+    _logger.info(f"Running player '{team_spec}' ({team.team_name})")
 
     while True:
-        cont = player_handle_request(socket, team)
+        cont = player_handle_request(socket, team, team_name_override=team_name_override, silent_bots=silent_bots)
         if not cont:
             return
 
 
-def player_handle_request(socket, team):
+def player_handle_request(socket, team, team_name_override=False, silent_bots=False):
     """ Awaits a new request on `socket` and dispatches it
     to `team`.
 
     Parameters
     ----------
     socket : zmq PAIR socket
         the connection to the main pelita game
@@ -131,16 +112,28 @@
         _logger.debug("<o-- %r [%s]", action, msg_id)
 
         # feed client actor here …
         if action == "set_initial":
             retval = team.set_initial(**data)
         elif action == "get_move":
             retval = team.get_move(**data)
+            if silent_bots:
+                # We want to remove a speak attribute
+                # but we don’t care if it fails at all
+                try:
+                    retval.pop('say')
+                except:
+                    pass
+
         elif action == "team_name":
-            retval = team.team_name
+            if isinstance(team_name_override, str):
+                retval = team_name_override
+            else:
+                retval = team.team_name
+            # TODO: Log team name override
         elif action == "exit":
             # quit and don’t return anything
             message_obj = {
                 "__uuid__": msg_id,
                 "__return__": None
             }
             return False
@@ -290,155 +283,51 @@
 
 
 def team_from_module(module):
     """ Looks for a move function and a team name in
     `module` and returns a team.
     """
     # look for a new-style team
-    move = getattr(module, "move")
-    name = getattr(module, "TEAM_NAME")
+    move = module.move
+    name = module.TEAM_NAME
     if not callable(move):
         raise TypeError("move is not a function")
-    if type(name) is not str:
+    if not isinstance(name, str):
         raise TypeError("TEAM_NAME is not a string")
     team, _ = make_team(move, team_name=name)
     return team
 
 
-def zeroconf_advertise(address, team_spec):
-    parsed_url = urlparse(address)
-    if parsed_url.scheme != "tcp":
-        _logger.warning("Can only advertise to tcp addresses.")
-        return
-    if parsed_url.hostname == "0.0.0.0":
-        _logger.warning("Can only advertise to a specific interface.")
-        return
-
-    # TODO: This should only be done once
-    team = load_team(team_spec)
-    name = team.team_name
-
-    desc = {
-        'spec': team_spec,
-        'team_name': name,
-        'proto_version': 0.1
-        }
-    info = zeroconf.ServiceInfo(
-        "_pelita-player._tcp.local.",
-        f"{name}._pelita-player._tcp.local.",
-        parsed_addresses=[parsed_url.hostname],
-        server='mynewserver.local',
-        port=parsed_url.port,
-        properties=desc,
-    )
-
-    # protocol versoin ...
-    zc = zeroconf.Zeroconf()
-    zc.engine._listen_socket
-    print("Registration of a service, press Ctrl-C to exit...")
-    zc.register_service(info)
-
-
-def with_zmq_router(team_spec, address, *, advertise: bool):
-    dealer_pair_mapping = {}
-    pair_dealer_mapping = {}
-    proc_dealer_mapping = {}
-
-    def cleanup(signum, frame):
-        for proc in proc_dealer_mapping:
-            proc.terminate()
-        sys.exit()
-
-    signal.signal(signal.SIGTERM, cleanup)
-
-    ctx = zmq.Context()
-    sock = ctx.socket(zmq.ROUTER)
-    sock.bind(address)
-
-    if advertise:
-        zeroconf_advertise(address, team_spec)
-
-    poll = zmq.Poller()
-    poll.register(sock, zmq.POLLIN)
+@click.group()
+@click.option('--log',
+              is_flag=False, flag_value="-", default=None, metavar='LOGFILE',
+              help="print debugging log information to LOGFILE (default 'stderr')")
+def main(log):
+    if log is not None:
+        start_logging(log)
+
+
+@main.command(help="Load team and connect to the specified address.")
+@click.argument('team')
+@click.argument('address')
+@click.option('--team-name-override',
+              default=None,
+              help='Override the team name')
+@click.option('--silent-bots',
+              is_flag=True,
+              default=False,
+              help='Filter bot speak')
+def remote_game(team, address, team_name_override, silent_bots):
+    run_player(team, address, team_name_override=team_name_override, silent_bots=silent_bots)
+
+
+@main.command("check-team", help="Load team and print its name.")
+@click.argument('team')
+def cli_check_team(team):
+    return check_team(team)
 
-    while True:
-        evts = dict(poll.poll(1000))
-        if sock in evts:
-            id_ = sock.recv()
-            msg = sock.recv_json()
-            if "REQUEST" in msg:
-                pair_sock = ctx.socket(zmq.PAIR)
-                port = pair_sock.bind_to_random_port('tcp://127.0.0.1')
-                pair_addr = 'tcp://127.0.0.1:{}'.format(port)
-
-                poll.register(pair_sock, zmq.POLLIN)
-
-                _logger.info("Starting match for team {}. ({} already running.)".format(team_spec, len(proc_dealer_mapping)))
-                sub = play_remote(team_spec, pair_addr)
-
-                dealer_pair_mapping[id_] = pair_sock
-                pair_dealer_mapping[pair_sock] = id_
-                proc_dealer_mapping[sub] = (id_, pair_sock)
-
-                assert len(dealer_pair_mapping) == len(pair_dealer_mapping)
-            elif id_ in dealer_pair_mapping:
-                dealer_pair_mapping[id_].send_json(msg)
-            else:
-                _logger.info("Unknown incoming DEALER and not a request.")
-
-        elif len(evts):
-            for pair_sock, id_ in pair_dealer_mapping.items():
-                if pair_sock in evts:
-                    msg = pair_sock.recv()
-                    sock.send_multipart([id_, msg])
-
-        old_procs = list(proc_dealer_mapping.keys())
-        count = 0
-        for proc in old_procs:
-            if proc.poll() is not None:
-                id_, pair_sock = proc_dealer_mapping[proc]
-                del dealer_pair_mapping[id_]
-                del pair_dealer_mapping[pair_sock]
-                del proc_dealer_mapping[proc]
-                count += 1
-        if count:
-            _logger.debug("Cleaned up {} process(es). ({} still running.)".format(count, len(proc_dealer_mapping)))
-
-
-def play_remote(team_spec, pair_addr):
-    external_call = [sys.executable,
-                    '-m',
-                    'pelita.scripts.pelita_player',
-                    team_spec,
-                    pair_addr]
-    _logger.debug("Executing: %r", external_call)
-    sub = subprocess.Popen(external_call)
-    return sub
-
-
-def main():
-    parser = argparse.ArgumentParser(description="Runs a Python pelita module.")
-    parser.add_argument('--log', help='print debugging log information to LOGFILE (default \'stderr\')',
-                        metavar='LOGFILE', default=argparse.SUPPRESS, nargs='?')
-    parser.add_argument('--remote', help='bind to a zmq.ROUTER socket at the given address which forks subprocesses on demand',
-                        action='store_const', const=True)
-    parser.add_argument('--advertise', help='advertise player on zeroconf',
-                        action='store_const', const=True)
-    parser.add_argument('--color', help='which color your team will have in the game', default=None)
-    parser.add_argument('team')
-    parser.add_argument('address')
-
-    args = parser.parse_args()
-
-    try:
-        start_logging(args.log)
-    except AttributeError:
-        pass
-
-    if args.remote:
-        with_zmq_router(args.team, args.address, advertise=args.advertise)
-    else:
-        run_player(args.team, args.address, args.color)
+def check_team(team):
+    print(load_team(team).team_name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pelita-2.3.2/pelita/scripts/pelita_tkviewer.py` & `pelita-2.4.0rc1/pelita/scripts/pelita_tkviewer.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/scripts/pelita_tournament.py` & `pelita-2.4.0rc1/pelita/scripts/pelita_tournament.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/team.py` & `pelita-2.4.0rc1/pelita/team.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import os
 import random
 import subprocess
 import sys
 import traceback
 from io import StringIO
 from pathlib import Path
+from urllib.parse import urlparse
 
 import zmq
+import networkx as nx
 
 from . import layout
 from .exceptions import PlayerDisconnected, PlayerTimeout
-from .layout import layout_as_str, BOT_I2N
-from .network import ZMQClientError, ZMQConnection, ZMQReplyTimeout, ZMQUnreachablePeer
+from .layout import layout_as_str, BOT_I2N, wall_dimensions
+from .network import ZMQClientError, ZMQConnection, ZMQReplyTimeout, ZMQUnreachablePeer, PELITA_PORT
 
 _logger = logging.getLogger(__name__)
 
 
 def _ensure_list_tuples(list):
     """ Ensures that an iterable is a list of position tuples. """
     return [tuple(item) for item in list]
@@ -32,23 +34,70 @@
     return [
         tuple((x, y) for x in range(0, width // 2)
                      for y in range(0, height) if (x, y) not in walls),
         tuple((x, y) for x in range(width // 2, width)
                      for y in range(0, height) if (x, y) not in walls)
     ]
 
+def walls_to_graph(walls):
+    """Return a networkx Graph object given the walls of a maze.
+
+    Parameters
+    ----------
+    walls : set[(x0,y0), (x1,y1), ...]
+         a set of wall coordinates
+
+    Returns
+    -------
+    graph : networkx.Graph
+         a networkx Graph representing the free squares in the maze and their
+         connections. Note that 'free' in this context means that the corresponding
+         square in the maze is not a wall (but can contain food or bots).
+
+    Notes
+    -----
+    Nodes in the graph are (x,y) coordinates representing squares in the maze
+    which are not walls.
+    Edges in the graph are ((x1,y1), (x2,y2)) tuples of coordinates of two
+    adjacent squares. Adjacent means that you can go from one square to one of
+    its adjacent squares by making ore single step (up, down, left, or right).
+    """
+    graph = nx.Graph()
+    width, height = wall_dimensions(walls)
+
+    for x in range(width):
+        for y in range(height):
+            if (x, y) not in walls:
+                # this is a free position, get its neighbors
+                for delta_x, delta_y in ((1,0), (-1,0), (0,1), (0,-1)):
+                    neighbor = (x + delta_x, y + delta_y)
+                    # we don't need to check for getting neighbors out of the maze
+                    # because our mazes are all surrounded by walls, i.e. our
+                    # deltas will not put us out of the maze
+                    if neighbor not in walls:
+                        # this is a genuine neighbor, add an edge in the graph
+                        graph.add_edge((x, y), neighbor)
+    return graph
+
+
 
 class Team:
     """
     Wraps a move function and forwards it the `set_initial`
     and `get_move` requests.
 
     The Team class holds the team’s state between turns, the team’s
     random number generator and the bot track (resets every time a bot
-    is killed).
+    is killed). This class is also caching bot attributes that do not
+    change during the game. Currently cached attributes:
+        - bot.walls
+        - bot.shape
+        - bot._initial_position
+        - bot.homezone
+        - bot.graph
 
     Parameters
     ----------
     team_move : function with (bot, state) -> position
         the team’s move function
     team_name :
         the name of the team (optional)
@@ -102,14 +151,19 @@
 
         # Cache the initial positions so that we don’t have to calculate them at each step
         self._initial_positions = layout.initial_positions(self._walls, self._shape)
 
         # Cache the homezone so that we don’t have to create it at each step
         self._homezone = create_homezones(self._shape, self._walls)
 
+        # Cache the graph representation of the maze -> stores a read-only view of the
+        # graph, so that local modifications in the move function are not carried
+        # over
+        self._graph = walls_to_graph(self._walls).copy(as_view=True)
+
         return self.team_name
 
     def get_move(self, game_state):
         """ Requests a move from the Player who controls the Bot with id `bot_id`.
 
         This method returns a dict with a key `move` and a value specifying the direction
         in a tuple. Additionally, a key `say` can be added with a textual value.
@@ -127,15 +181,16 @@
                        shape=self._shape,
                        initial_positions=self._initial_positions,
                        homezone=self._homezone,
                        team=game_state['team'],
                        enemy=game_state['enemy'],
                        round=game_state['round'],
                        bot_turn=game_state['bot_turn'],
-                       rng=self._random)
+                       rng=self._random,
+                       graph=self._graph)
 
         team = me._team
 
         for idx, mybot in enumerate(team):
             # If a bot has been killed, we reset its bot track
             if mybot.was_killed:
                 self._bot_track[idx] = []
@@ -174,15 +229,15 @@
             }
 
         return {
             "move": move,
             "say": me._say
         }
 
-    def _exit(self):
+    def _exit(self, game_state=None):
         """ Dummy function. Only needed for `RemoteTeam`. """
         pass
 
     def __repr__(self):
         return f'Team({self._team_move!r}, {self.team_name!r})'
 
 
@@ -217,33 +272,47 @@
 
         self._team_spec = team_spec
         self._team_name = team_name
 
         #: Default timeout for a request, unless specified in the game_state
         self._request_timeout = 3
 
-        if team_spec.startswith('remote:tcp://'):
+        if team_spec.startswith('pelita://'):
             # We connect to a remote player that is listening
             # on the given team_spec address.
             # We create a new DEALER socket and send a single
             # REQUEST message to the remote address.
             # The remote player will then create a new instance
             # of a player and forward all of our zmq traffic
             # to that player.
 
-            # remove the "remote:" part from the address
-            send_addr = team_spec[len("remote:"):]
+            # given a url pelita://hostname:port/path we extract hostname and port and
+            # convert it to tcp://hostname:port that we use for the zmq connection
+            parsed_url = urlparse(team_spec)
+            if parsed_url.port:
+                port = parsed_url.port
+            else:
+                port = PELITA_PORT
+            send_addr = f"tcp://{parsed_url.hostname}:{port}"
             address = "tcp://*"
             self.bound_to_address = address
 
             socket = zmq_context.socket(zmq.DEALER)
             socket.setsockopt(zmq.LINGER, 0)
             socket.connect(send_addr)
             _logger.info("Connecting zmq.DEALER to remote player at {}.".format(send_addr))
-            socket.send_json({"REQUEST": address})
+
+            socket.send_json({"REQUEST": team_spec})
+            WAIT_TIMEOUT = 5000
+            incoming = socket.poll(timeout=WAIT_TIMEOUT)
+            if incoming == zmq.POLLIN:
+                ok = socket.recv()
+            else:
+                # Server did not respond
+                raise PlayerTimeout()
             self.proc = None
 
         else:
             # We bind to a local tcp port with a zmq PAIR socket
             # and start a new subprocess of pelita_player.py
             # that includes the address of that socket and the
             # team_spec as command line arguments.
@@ -269,18 +338,17 @@
         the same start script (pelitagame) and runs `team_spec`
         as a standalone client on URL `addr`.
         """
         player = 'pelita.scripts.pelita_player'
         external_call = [sys.executable,
                          '-m',
                          player,
+                         'remote-game',
                          team_spec,
-                         address,
-                         '--color',
-                         color]
+                         address]
 
         _logger.debug("Executing: %r", external_call)
         if store_output == subprocess.DEVNULL:
             return (subprocess.Popen(external_call, stdout=store_output), None, None)
         elif store_output:
             store_path = Path(store_output)
             stdout = (store_path / f"{color or team_spec}.out").open('w')
@@ -352,25 +420,32 @@
             return None
         except ZMQUnreachablePeer:
             # if the remote connection is closed
             raise PlayerDisconnected()
         except ZMQClientError:
             raise
 
-    def _exit(self):
+    def _exit(self, game_state=None):
         # We only want to exit once.
         if getattr(self, '_sent_exit', False):
             return
+
+        if game_state:
+            payload = {'game_state': game_state}
+        else:
+            payload = {}
+
         try:
             # TODO: make zmqconnection stateful. set flag when already disconnected
             # For now, we simply check the state of the socket so that we do not send
             # over an already closed socket.
             if self.zmqconnection.socket.closed:
                 return
-            self.zmqconnection.send("exit", {}, timeout=1)
+            # TODO: Include final state with exit message
+            self.zmqconnection.send("exit", payload, timeout=1)
             self._sent_exit = True
         except ZMQUnreachablePeer:
             _logger.info("Remote Player %r is already dead during exit. Ignoring.", self)
 
     def __del__(self):
         try:
             self._exit()
@@ -438,14 +513,15 @@
                           homezone,
                           food,
                           score,
                           kills,
                           deaths,
                           was_killed,
                           random,
+                          graph,
                           round,
                           bot_char,
                           is_blue,
                           team_name,
                           error_count,
                           is_noisy,
                           bot_turn=None):
@@ -473,47 +549,30 @@
         self._bot_index  = bot_index
         self.round = round
         self.char = bot_char
         self.is_blue = is_blue
         self.team_name = team_name
         self.error_count = error_count
         self.is_noisy = is_noisy
+        self.graph = graph
 
-        # Attributes for Bot
-        if self._is_on_team:
-            assert bot_turn is not None
-            self._bot_turn = bot_turn
-
-    # @property
-    # def legal_directions(self):
-        # """ The legal moves that the bot can make from its current position,
-        # including no move at all.
-        # """
-        # legal_directions = [(0, 0)]
-
-        # for move in [(-1, 0), (1, 0), (0, 1), (0, -1)]:
-            # new_pos = (self.position[0] + move[0], self.position[1] + move[1])
-            # if not new_pos in self.walls:
-                # legal_directions.append(move)
-
-        # return legal_directions
-
-    @property
-    def legal_positions(self):
-        """ The legal positions that the bot can reach from its current position,
-        including the current position.
-        """
-        legal_positions = []
+        # The legal positions that the bot can reach from its current position,
+        # including the current position.
+        self.legal_positions = []
 
         for direction in [(0, 0), (-1, 0), (1, 0), (0, 1), (0, -1)]:
-            new_pos = (self.position[0] + direction[0], self.position[1] + direction[1])
+            new_pos = (position[0] + direction[0],
+                       position[1] + direction[1])
             if not new_pos in self.walls:
-                legal_positions.append(new_pos)
+                self.legal_positions.append(new_pos)
 
-        return legal_positions
+        # Attributes for Bot
+        if self._is_on_team:
+            assert bot_turn is not None
+            self._bot_turn = bot_turn
 
     @property
     def _team(self):
        """ Both of our bots.
        """
        if self._is_on_team:
            return self._bots['team']
@@ -651,15 +710,15 @@
 
             out.write(str(layout))
             out.write(footer)
             return out.getvalue()
 
 
 # def __init__(self, *, bot_index, position, initial_position, walls, homezone, food, is_noisy, score, random, round, is_blue):
-def make_bots(*, walls, shape, initial_positions, homezone, team, enemy, round, bot_turn, rng):
+def make_bots(*, walls, shape, initial_positions, homezone, team, enemy, round, bot_turn, rng, graph):
     bots = {}
 
     team_index = team['team_index']
     enemy_index = enemy['team_index']
 
     team_initial_positions = initial_positions[team_index::2]
     enemy_initial_positions = initial_positions[enemy_index::2]
@@ -677,14 +736,15 @@
             food=_ensure_list_tuples(team['food']),
             walls=walls,
             shape=shape,
             round=round,
             bot_turn=bot_turn,
             bot_char=BOT_I2N[team_index + idx*2],
             random=rng,
+            graph=graph,
             position=team['bot_positions'][idx],
             initial_position=team_initial_positions[idx],
             is_blue=team_index % 2 == 0,
             homezone=homezone[team_index],
             team_name=team['name'])
         b._bots = bots
         team_bots.append(b)
@@ -701,14 +761,15 @@
             error_count=enemy['error_count'],
             food=_ensure_list_tuples(enemy['food']),
             walls=walls,
             shape=shape,
             round=round,
             bot_char = BOT_I2N[team_index + idx*2],
             random=rng,
+            graph=graph,
             position=enemy['bot_positions'][idx],
             initial_position=enemy_initial_positions[idx],
             is_blue=enemy_index % 2 == 0,
             homezone=homezone[enemy_index],
             team_name=enemy['name'])
         b._bots = bots
         enemy_bots.append(b)
```

### Comparing `pelita-2.3.2/pelita/tournament/__init__.py` & `pelita-2.4.0rc1/pelita/tournament/__init__.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/tournament/knockout_mode.py` & `pelita-2.4.0rc1/pelita/tournament/knockout_mode.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/tournament/roundrobin.py` & `pelita-2.4.0rc1/pelita/tournament/roundrobin.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/ui/tk_canvas.py` & `pelita-2.4.0rc1/pelita/ui/tk_canvas.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/ui/tk_sprites.py` & `pelita-2.4.0rc1/pelita/ui/tk_sprites.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/ui/tk_utils.py` & `pelita-2.4.0rc1/pelita/ui/tk_utils.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/ui/tk_viewer.py` & `pelita-2.4.0rc1/pelita/ui/tk_viewer.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/pelita/utils.py` & `pelita-2.4.0rc1/pelita/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,22 @@
 import random
 
 import networkx as nx
 
 
 from .team import make_bots, create_homezones
 from .layout import (get_random_layout, get_layout_by_name, get_available_layouts,
-                     parse_layout, BOT_N2I, initial_positions, wall_dimensions)
+                     parse_layout, BOT_N2I, initial_positions)
 
-RNG = random.Random()
-
-def walls_to_graph(walls):
-    """Return a networkx Graph object given the walls of a maze.
-
-    Parameters
-    ----------
-    walls : set[(x0,y0), (x1,y1), ...]
-         a set of wall coordinates
-
-    Returns
-    -------
-    graph : networkx.Graph
-         a networkx Graph representing the free squares in the maze and their
-         connections. Note that 'free' in this context means that the corresponding
-         square in the maze is not a wall (but can contain food or bots).
+# this import is needed for backward compatibility, do not remove or you'll break
+# older clients!
+from .team import walls_to_graph
 
-    Notes
-    -----
-    Nodes in the graph are (x,y) coordinates representing squares in the maze
-    which are not walls.
-    Edges in the graph are ((x1,y1), (x2,y2)) tuples of coordinates of two
-    adjacent squares. Adjacent means that you can go from one square to one of
-    its adjacent squares by making ore single step (up, down, left, or right).
-    """
-    graph = nx.Graph()
-    width, height = wall_dimensions(walls)
+RNG = random.Random()
 
-    for x in range(width):
-        for y in range(height):
-            if (x, y) not in walls:
-                # this is a free position, get its neighbors
-                for delta_x, delta_y in ((1,0), (-1,0), (0,1), (0,-1)):
-                    neighbor = (x + delta_x, y + delta_y)
-                    # we don't need to check for getting neighbors out of the maze
-                    # because our mazes are all surrounded by walls, i.e. our
-                    # deltas will not put us out of the maze
-                    if neighbor not in walls:
-                        # this is a genuine neighbor, add an edge in the graph
-                        graph.add_edge((x, y), neighbor)
-    return graph
 
 def _parse_layout_arg(*, layout=None, food=None, bots=None, seed=None):
 
     # prepare layout argument to be passed to pelita.game.run_game
     if layout is None:
         layout_name, layout_str = get_random_layout(size='normal', seed=seed)
         layout_dict = parse_layout(layout_str)
@@ -299,10 +264,11 @@
                     shape=layout['shape'],
                     initial_positions=initial_positions(layout['walls'], layout['shape']),
                     homezone=create_homezones(layout['shape'], layout['walls']),
                     team=team,
                     enemy=enemy,
                     round=round,
                     bot_turn=0,
-                    rng=rng)
+                    rng=rng,
+                    graph=walls_to_graph(layout['walls']))
     return bot
```

### Comparing `pelita-2.3.2/pelita/viewer.py` & `pelita-2.4.0rc1/pelita/viewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """ The observers. """
 
 import json
 import logging
+import sys
 
 import zmq
 from rich.console import Console
 from rich.progress import (BarColumn, MofNCompleteColumn, Progress,
                            SpinnerColumn, TextColumn, TimeElapsedColumn)
 
 from . import layout
 from .network import SetEncoder
 
 _logger = logging.getLogger(__name__)
+_mswindows = (sys.platform == "win32")
 
 # Only highlight explicit markup
 pprint = Console(highlight=False).print
 
 class ProgressViewer:
     def __init__(self) -> None:
         self.progress = Progress(
@@ -179,17 +181,31 @@
 
     def show_state(self, game_state):
         self._send(game_state)
 
 
 class ResultPrinter:
     def show_state(self, state):
+        if (state['turn'] is None and
+            state['round'] is None):
+            # TODO: We must ensure that this is only printed once
+            self.print_team_names(state['team_names'])
+
         if state["gameover"]:
             self.print_possible_winner(state)
 
+    def print_team_names(self, team_names):
+        # TODO: The team_spec is missing in the state.
+        # Should we print it here?
+        pie = '' if _mswindows else 'ᗧ'
+
+        for col, team_name in zip(['blue', 'red'], team_names):
+            if team_name is not None:
+                pprint(f"[bright_{col}]{pie}[/bright_{col}] {col} team: '{team_name}'")
+
     def print_possible_winner(self, state):
         """ Checks the game state for a winner.
 
         This is needed for pelita.scripts parsing the output.
         """
         winning_team = state.get("whowins")
         if state['round'] == 1:
```

### Comparing `pelita-2.3.2/pyproject.toml` & `pelita-2.4.0rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,26 +26,28 @@
     "pyzmq",
     "PyYAML",
     "numpy",
     "networkx",
     "pytest>=4",
     "zeroconf",
     "rich",
+    "click",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
 pelita = "pelita.scripts.pelita_main:main"
 pelita-tournament = "pelita.scripts.pelita_tournament:main"
 pelita-tkviewer = "pelita.scripts.pelita_tkviewer:main"
 pelita-player = "pelita.scripts.pelita_player:main"
+pelita-server = "pelita.scripts.pelita_server:main"
 pelita-createlayout = "pelita.scripts.pelita_createlayout:main"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
 # addopts = --verbose
```

### Comparing `pelita-2.3.2/test/test_filter_gamestates.py` & `pelita-2.4.0rc1/test/test_filter_gamestates.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_game.py` & `pelita-2.4.0rc1/test/test_game.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_layout.py` & `pelita-2.4.0rc1/test/test_layout.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_libpelita.py` & `pelita-2.4.0rc1/test/test_libpelita.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_maze_generation.py` & `pelita-2.4.0rc1/test/test_maze_generation.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_network.py` & `pelita-2.4.0rc1/test/test_network.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 import uuid
 import sys
 
 import zmq
 
-from pelita.network import bind_socket, extract_port_range
+from pelita.network import bind_socket
 from pelita.team import make_team
 from pelita.scripts.pelita_player import player_handle_request
 
 _mswindows = (sys.platform == "win32")
 
 
 @pytest.fixture(scope="module")
@@ -26,30 +26,14 @@
 
 def test_bind_socket_fail(zmq_context):
     socket = zmq_context.socket(zmq.PUB)
     with pytest.raises(zmq.ZMQError):
         bind_socket(socket, "bad-address", '--publish')
     socket.close()
 
-def test_extract_port_range():
-    test_cases = [
-        ("tcp://*",                     dict(addr="tcp://*")),
-        ("tcp://*:",                    dict(addr="tcp://*:")),
-        ("tcp://*:*",                   dict(addr="tcp://*", port_min=None, port_max=None)),
-        ("tcp://*:123",                 dict(addr="tcp://*:123")),
-        ("tcp://*:[123:124]",           dict(addr="tcp://*", port_min=123, port_max=124)),
-        ("tcp://*:123:[124:125]]",      dict(addr="tcp://*:123", port_min=124, port_max=125)),
-        ("tcp://*:123[124:125]]",       dict(addr="tcp://*:123[124:125]]")),
-        ("ipc:///tmp/pelita-publisher", dict(addr="ipc:///tmp/pelita-publisher"))
-    ]
-
-    for test in test_cases:
-        extracted = extract_port_range(test[0])
-        assert extracted == test[1]
-
 
 def test_simpleclient(zmq_context):
     res = []
     def stopping(bot, state):
         print(bot)
         res.append(True)
         print(res)
```

### Comparing `pelita-2.3.2/test/test_pelita_player.py` & `pelita-2.4.0rc1/test/test_pelita_player.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_player_base.py` & `pelita-2.4.0rc1/test/test_player_base.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_players.py` & `pelita-2.4.0rc1/test/test_players.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_remote_game.py` & `pelita-2.4.0rc1/test/test_remote_game.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 
 @pytest.fixture(scope="module")
 def remote_teams():
     # get random port numbers within the range of dynamic ports
     port_stopping = RNG.randint(49153,65534)
     port_food_eater = port_stopping+1
 
-    addr_stopping = f'tcp://127.0.0.1:{port_stopping}'
-    addr_food_eater = f'tcp://127.0.0.1:{port_food_eater}'
-    remote = [sys.executable, '-m', 'pelita.scripts.pelita_player', '--remote']
+    addr_stopping = "127.0.0.1"
+    addr_food_eater = "127.0.0.1"
+    remote = [sys.executable, '-m', 'pelita.scripts.pelita_server', 'remote-server', '--address', '127.0.0.1']
 
-    remote_stopping = remote + ['pelita/player/StoppingPlayer', addr_stopping ]
-    remote_food_eater = remote + ['pelita/player/FoodEatingPlayer', addr_food_eater]
+    remote_stopping = remote + ['--port', str(port_stopping), '--team', 'pelita/player/StoppingPlayer']
+    remote_food_eater = remote + ['--port', str(port_food_eater), '--team', 'pelita/player/FoodEatingPlayer']
 
-    teams = [f'remote:{addr_stopping}', f'remote:{addr_food_eater}']
+    teams = [f'pelita://127.0.0.1:{port_stopping}/Stopping_Players', f'pelita://127.0.0.1:{port_food_eater}/Food_Eating_Players']
     with run_and_terminate_process(remote_stopping):
         with run_and_terminate_process(remote_food_eater):
             yield teams
 
 
 def test_remote_call_pelita(remote_teams):
     res, stdout, stderr = call_pelita(remote_teams, rounds=30, size='small', viewer='null', seed='1')
@@ -117,20 +117,17 @@
     assert state['whowins'] == 2
     assert state['fatal_errors'] == [[], []]
     assert state['errors'] == [{}, {}]
 
     path = Path(out_folder.name)
     blue_lines = (path / 'blue.out').read_text().split('\n')
     red_lines = (path / 'red.out').read_text().split('\n')
-    # The first line contains the welcome message 'blue team 'path' -> 'name''
-    assert 'blue team' in blue_lines[0]
-    assert 'red team' in red_lines[0]
     # now check what has been printed
-    assert blue_lines[1:] == ['1 0 p1', '1 1 p1', '2 0 p1', '2 1 p1', '']
-    assert red_lines[1:] == ['1 0 p2', '1 1 p2', '2 0 p2', '2 1 p2', '']
+    assert blue_lines == ['1 0 p1', '1 1 p1', '2 0 p1', '2 1 p1', '']
+    assert red_lines == ['1 0 p2', '1 1 p2', '2 0 p2', '2 1 p2', '']
 
     assert (path / 'blue.err').read_text() == 'p1err\np1err\np1err\np1err\n'
     assert (path / 'red.err').read_text() == 'p2err\np2err\np2err\np2err\n'
 
 
 @pytest.mark.parametrize("failing_team", [0, 1])
 def test_remote_dumps_with_failure(failing_team):
@@ -172,20 +169,16 @@
 
     path = Path(out_folder.name)
 
     # stdout is still the same for both teams
 
     blue_lines = (path / 'blue.out').read_text().split('\n')
     red_lines = (path / 'red.out').read_text().split('\n')
-    # The first line contains the welcome message 'blue team 'path' -> 'name''
-    assert 'blue team' in blue_lines[0]
-    assert 'red team' in red_lines[0]
-    # now check what has been printed
-    assert blue_lines[1:] == ['']
-    assert red_lines[1:] == ['']
+    assert blue_lines == ['']
+    assert red_lines == ['']
 
     blue_err = (path / 'blue.err').read_text()
     red_err = (path / 'red.err').read_text()
 
     if failing_team == 0:
         fail_err = blue_err
         good_err = red_err
```

### Comparing `pelita-2.3.2/test/test_team.py` & `pelita-2.4.0rc1/test/test_team.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+import networkx
 
 from pelita.layout import parse_layout, get_random_layout, initial_positions
 from pelita.game import run_game, setup_game, play_turn
 
 def stopping(bot, state):
     return bot.position
 
@@ -403,14 +404,89 @@
 
     state = run_game([asserting_team, asserting_team], max_rounds=1, layout_dict=parsed)
     # assertions might have been caught in run_game
     # check that all is good
     assert state['errors'] == [{}, {}]
     assert state['fatal_errors'] == [[], []]
 
+def test_bot_graph():
+    layout = """
+    ########
+    #  ax  #
+    #  by  #
+    #......#
+    ########
+    """
+    def rough_bot(bot, state):
+        # check that we have this node in the graph at the beginning
+        assert (1, 1) in bot.graph
+        # check that we can't remove a node
+        with pytest.raises(networkx.NetworkXError):
+            bot.graph.remove_node((1, 1))
+        # check that we can't add a node
+        with pytest.raises(networkx.NetworkXError):
+            bot.graph.add_node((100, 100))
+        # check that I can create my own copy of the graph and that this copy is
+        # writable
+        my_graph = bot.graph.copy()
+        my_graph.remove_node((1, 1))
+        assert (1, 1) not in my_graph
+        return bot.position
+
+    state  = run_game([rough_bot, stopping], max_rounds=1, layout_dict=parse_layout(layout))
+    # assertions might have been caught in run_game
+    # check that all is good
+    assert state['errors'] == [{}, {}]
+    assert state['fatal_errors'] == [[], []]
+
+def test_bot_graph_is_half_mutable():
+    # Test that a bot can change the weights of the graph
+    # Changing the weights affects the future self of the bot
+    # Changing the weights does affect the other bot in the team
+    # Changing the weights does not affect the other team
+    layout = """
+    ########
+    #  ax  #
+    #  by  #
+    #......#
+    ########
+    """
+
+    observer = []
+    
+    def blue(bot, state):
+        if bot.turn == 0 and bot.round == 1:
+            assert bot.graph[1, 1][1, 2].get('weight') is None
+            bot.graph[1, 1][1, 2]['weight'] = 1
+            observer.append('B')
+        else:
+            assert bot.graph[1, 1][1, 2].get('weight') == 1
+            observer.append('b')
+
+        return bot.position
+
+    def red(bot, state):
+        if bot.turn == 0 and bot.round == 1:
+            assert bot.graph[1, 1][1, 2].get('weight') is None
+            bot.graph[1, 1][1, 2]['weight'] = 2
+            observer.append('R')
+        else:
+            assert bot.graph[1, 1][1, 2].get('weight') == 2
+            observer.append('r')
+
+        return bot.position
+
+    state  = run_game([blue, red], max_rounds=2, layout_dict=parse_layout(layout))
+    # assertions might have been caught in run_game
+    # check that all is good
+    assert state['errors'] == [{}, {}]
+    assert state['fatal_errors'] == [[], []]
+    assert "".join(observer) == 'BRbrbrbr'
+
+
 def test_team_names():
     test_layout = (
     """ ##################
         #a#.  .  # .     #
         #b#####    #####x#
         #     . #  .  .#y#
         ################## """)
```

### Comparing `pelita-2.3.2/test/test_tournament.py` & `pelita-2.4.0rc1/test/test_tournament.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/test/test_utils.py` & `pelita-2.4.0rc1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/tournament.yaml` & `pelita-2.4.0rc1/tournament.yaml`

 * *Files identical despite different names*

### Comparing `pelita-2.3.2/PKG-INFO` & `pelita-2.4.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelita
-Version: 2.3.2
+Version: 2.4.0rc1
 Summary: Pelita
 Keywords: education
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -16,19 +16,20 @@
 Requires-Dist: pyzmq
 Requires-Dist: PyYAML
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: pytest>=4
 Requires-Dist: zeroconf
 Requires-Dist: rich
+Requires-Dist: click
 Project-URL: Homepage, https://github.com/ASPP/pelita
 
 # Pelita
 
-[![Build Status](https://github.com/ASPP/pelita/actions/workflows/push_ci.yml/badge.svg?branch=main)](https://github.com/ASPP/pelita/actions)
+[![Build Status](https://github.com/ASPP/pelita/actions/workflows/test_pytest.yml/badge.svg?branch=main)](https://github.com/ASPP/pelita/actions)
 
 ## Description
 
 Pelita is a programmable game that lets you play against your opponent by writing code in Python.
 
 ![](doc/source/images/small-game.png)
```

