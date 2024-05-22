# Comparing `tmp/mnt_nanoplacer-0.2.2.tar.gz` & `tmp/mnt_nanoplacer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnt_nanoplacer-0.2.2.tar", last modified: Mon May 13 09:45:59 2024, max compression
+gzip compressed data, was "mnt_nanoplacer-0.2.3.tar", last modified: Wed May 22 06:08:30 2024, max compression
```

## Comparing `mnt_nanoplacer-0.2.2.tar` & `mnt_nanoplacer-0.2.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.369051 mnt_nanoplacer-0.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    70113 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/docs/_static/lbr.png
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/docs/_static/mnt_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/docs/_static/mnt_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:45:59.413051 mnt_nanoplacer-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.369051 mnt_nanoplacer-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/src/mnt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.369051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.397051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/
--rw-r--r--   0 runner    (1001) docker     (127)    44749 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/adder.v
--rw-r--r--   0 runner    (1001) docker     (127)   491036 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v
--rw-r--r--   0 runner    (1001) docker     (127)   139420 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/bar.v
--rw-r--r--   0 runner    (1001) docker     (127)    30030 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v
--rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/dec.v
--rw-r--r--   0 runner    (1001) docker     (127)  2537203 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/div.v
--rw-r--r--   0 runner    (1001) docker     (127) 10153688 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v
--rw-r--r--   0 runner    (1001) docker     (127)    54911 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v
--rw-r--r--   0 runner    (1001) docker     (127)  1372592 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/log2.v
--rw-r--r--   0 runner    (1001) docker     (127)   132676 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/max.v
--rw-r--r--   0 runner    (1001) docker     (127)  1158136 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v
--rw-r--r--   0 runner    (1001) docker     (127)    38989 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/priority.v
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/router.v
--rw-r--r--   0 runner    (1001) docker     (127)   214688 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sin.v
--rw-r--r--   0 runner    (1001) docker     (127)  1087553 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v
--rw-r--r--   0 runner    (1001) docker     (127)   783980 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/square.v
--rw-r--r--   0 runner    (1001) docker     (127)   600136 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/voter.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.401051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c17.v
--rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v
--rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v
--rw-r--r--   0 runner    (1001) docker     (127)    37970 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v
--rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v
--rw-r--r--   0 runner    (1001) docker     (127)    70010 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v
--rw-r--r--   0 runner    (1001) docker     (127)    91913 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v
--rw-r--r--   0 runner    (1001) docker     (127)    83840 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v
--rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.405051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/
--rwxr-xr-x   0 runner    (1001) docker     (127)      222 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderAOIG.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderMaj.v
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/FA.v
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/FS.v
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/HA.v
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/HS.v
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/b1_r2.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/clpl.v
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/mux21.v
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/mux41.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/newtag.v
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/par_check.v
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/par_gen.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/t.v
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xnor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor2.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      560 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor5_r1.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderAOIG.v
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/b1_r2.v
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/c17.v
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority.v
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/parity.v
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/t.v
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/t_5.v
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor.v
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/FA.v
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/HA.v
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/mux21.v
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/par_check.v
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/par_gen.v
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/xnor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/xor2.v
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23940 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/nano_placement_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.384648 mnt_nanoplacer-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.384648 mnt_nanoplacer-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.380648 mnt_nanoplacer-0.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.384648 mnt_nanoplacer-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    70113 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/docs/_static/lbr.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/docs/_static/mnt_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/docs/_static/mnt_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.380648 mnt_nanoplacer-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.384648 mnt_nanoplacer-0.2.3/src/mnt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.388649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.384648 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.412649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/
+-rw-r--r--   0 runner    (1001) docker     (127)    44749 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/adder.v
+-rw-r--r--   0 runner    (1001) docker     (127)   491036 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v
+-rw-r--r--   0 runner    (1001) docker     (127)   139420 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/bar.v
+-rw-r--r--   0 runner    (1001) docker     (127)    30030 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v
+-rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/dec.v
+-rw-r--r--   0 runner    (1001) docker     (127)  2537203 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/div.v
+-rw-r--r--   0 runner    (1001) docker     (127) 10153688 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v
+-rw-r--r--   0 runner    (1001) docker     (127)    54911 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v
+-rw-r--r--   0 runner    (1001) docker     (127)  1372592 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/log2.v
+-rw-r--r--   0 runner    (1001) docker     (127)   132676 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/max.v
+-rw-r--r--   0 runner    (1001) docker     (127)  1158136 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v
+-rw-r--r--   0 runner    (1001) docker     (127)    38989 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/priority.v
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/router.v
+-rw-r--r--   0 runner    (1001) docker     (127)   214688 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/sin.v
+-rw-r--r--   0 runner    (1001) docker     (127)  1087553 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v
+-rw-r--r--   0 runner    (1001) docker     (127)   783980 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/square.v
+-rw-r--r--   0 runner    (1001) docker     (127)   600136 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/voter.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.416649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c17.v
+-rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v
+-rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v
+-rw-r--r--   0 runner    (1001) docker     (127)    37970 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v
+-rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v
+-rw-r--r--   0 runner    (1001) docker     (127)    70010 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v
+-rw-r--r--   0 runner    (1001) docker     (127)    91913 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v
+-rw-r--r--   0 runner    (1001) docker     (127)    83840 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.420649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      222 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderAOIG.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderMaj.v
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/FA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/FS.v
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/HA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/HS.v
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/b1_r2.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/clpl.v
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/mux21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/mux41.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/newtag.v
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/par_check.v
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/par_gen.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/t.v
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/xnor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/xor2.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      560 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/xor5_r1.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.420649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderAOIG.v
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/b1_r2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/c17.v
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/majority.v
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/parity.v
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/t.v
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/t_5.v
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/xor.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.420649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/FA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/HA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/mux21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/par_check.v
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/par_gen.v
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/xnor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/trindade16/xor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24192 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/nano_placement_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-22 06:08:30.000000 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-22 06:08:30.000000 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:08:30.000000 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 06:08:30.000000 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 06:08:30.000000 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 06:08:30.000000 mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:30.424649 mnt_nanoplacer-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-22 06:08:22.000000 mnt_nanoplacer-0.2.3/tests/test_utils.py
```

### Comparing `mnt_nanoplacer-0.2.2/.github/dependabot.yml` & `mnt_nanoplacer-0.2.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/.github/release-drafter.yml` & `mnt_nanoplacer-0.2.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/.github/workflows/codeql.yml` & `mnt_nanoplacer-0.2.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/.github/workflows/deploy.yml` & `mnt_nanoplacer-0.2.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/.gitignore` & `mnt_nanoplacer-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/.pre-commit-config.yaml` & `mnt_nanoplacer-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/LICENSE` & `mnt_nanoplacer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/PKG-INFO` & `mnt_nanoplacer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnt.nanoplacer
-Version: 0.2.2
+Version: 0.2.3
 Summary: NanoPlaceR - An open-source framework for placement and routing of Field-coupled Nanotechnologies based on reinforcement learning.
 Author-email: Simon Hofmann <simon.t.hofmann@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Chair for Design Automation, TU Munich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,30 +37,31 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: <=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: networkx>=3.1
-Requires-Dist: numpy>=1.24.3
-Requires-Dist: pre-commit>=3.3.3
-Requires-Dist: setuptools>=65.5.1
+Requires-Dist: networkx>=3.2.1
+Requires-Dist: numpy>=1.26.3
+Requires-Dist: pre-commit>=3.6.0
+Requires-Dist: setuptools>=68.2.0
 Requires-Dist: sb3_contrib>=2.2.1
-Requires-Dist: tensorboard>=2.13.0
+Requires-Dist: tensorboard>=2.15.1
 Requires-Dist: wheel>=0.38.0
-Requires-Dist: mnt.pyfiction>=0.5.0
+Requires-Dist: mnt.pyfiction>=0.6.1
 Provides-Extra: test
-Requires-Dist: pytest>=7.2; extra == "test"
+Requires-Dist: pytest>=8.2.1; extra == "test"
 Provides-Extra: coverage
 Requires-Dist: mnt.nanoplacer[test]; extra == "coverage"
 Requires-Dist: pytest-cov[toml]; extra == "coverage"
 
 [![PyPI](https://img.shields.io/pypi/v/mnt.nanoplacer?logo=pypi&style=flat-square)](https://pypi.org/project/mnt.nanoplacer/)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/mnt-nanoplacer/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/mnt-nanoplacer/actions/workflows/deploy.yml)
@@ -153,15 +154,15 @@
   -r,  --reset_model               If True, reset saved model and train from scratch (defautls to False).
   -v,  --verbosity                 0: No information. 1: Print layout after every new best placement. 2: Print training metrics. 3: 1 and 2 combined.
 ```
 
 For example to create the gate-level layout for the mux21 function from trindade16 on the 2DDWave clocking scheme using the best found layout dimensions (by training for a maximum of 10000 timesteps):
 
 ```
-mnt.nanoplacer -b "trindade16" -f "mux21" -c "2DDWave" -t "gate-level" -l -ts 10000 -v 1
+mnt.nanoplacer -b "trindade16" -f "mux21" -c "2DDWave" -t "Gate-level" -l -ts 10000 -v 1
 ```
 
 # Repository Structure
 
 ```
 .
 ├── docs/
```

### Comparing `mnt_nanoplacer-0.2.2/README.md` & `mnt_nanoplacer-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
   -r,  --reset_model               If True, reset saved model and train from scratch (defautls to False).
   -v,  --verbosity                 0: No information. 1: Print layout after every new best placement. 2: Print training metrics. 3: 1 and 2 combined.
 ```
 
 For example to create the gate-level layout for the mux21 function from trindade16 on the 2DDWave clocking scheme using the best found layout dimensions (by training for a maximum of 10000 timesteps):
 
 ```
-mnt.nanoplacer -b "trindade16" -f "mux21" -c "2DDWave" -t "gate-level" -l -ts 10000 -v 1
+mnt.nanoplacer -b "trindade16" -f "mux21" -c "2DDWave" -t "Gate-level" -l -ts 10000 -v 1
 ```
 
 # Repository Structure
 
 ```
 .
 ├── docs/
```

### Comparing `mnt_nanoplacer-0.2.2/docs/_static/lbr.png` & `mnt_nanoplacer-0.2.3/docs/_static/lbr.png`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/docs/_static/mnt_dark.svg` & `mnt_nanoplacer-0.2.3/docs/_static/mnt_dark.svg`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/docs/_static/mnt_light.svg` & `mnt_nanoplacer-0.2.3/docs/_static/mnt_light.svg`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/pyproject.toml` & `mnt_nanoplacer-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,43 +14,44 @@
 ]
 keywords = ["FCN",  "physical design"]
 license = { file = "LICENSE" }
 requires-python = "<=3.12"
 dynamic = ["version"]
 
 dependencies = [
-    "networkx>=3.1",
-    "numpy>=1.24.3",
-    "pre-commit>=3.3.3",
-    "setuptools>=65.5.1",
+    "networkx>=3.2.1",
+    "numpy>=1.26.3",
+    "pre-commit>=3.6.0",
+    "setuptools>=68.2.0",
     "sb3_contrib>=2.2.1",
-    "tensorboard>=2.13.0",
+    "tensorboard>=2.15.1",
     "wheel>=0.38.0",
-    "mnt.pyfiction>=0.5.0"
+    "mnt.pyfiction>=0.6.1"
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
 ]
 
 [project.optional-dependencies]
-test = ["pytest>=7.2"]
+test = ["pytest>=8.2.1"]
 coverage = ["mnt.nanoplacer[test]", "pytest-cov[toml]"]
 
 [project.scripts]
 "mnt.nanoplacer" = "mnt.nanoplacer.main:start"
 
 [project.urls]
 Homepage = "https://github.com/cda-tum/NanoPlaceR"
```

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/adder.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/adder.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/bar.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/bar.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/dec.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/dec.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/div.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/div.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/log2.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/log2.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/max.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/max.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/priority.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/priority.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/router.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/router.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sin.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/sin.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/square.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/square.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/voter.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/EPFL/voter.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/clpl.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/clpl.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/majority.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/parity.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/parity.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/main.py` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/main.py`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/nano_placement_env.py` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/nano_placement_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,19 @@
         verbose: int = 1,
         optimize: bool = True,
     ):
         """Constructor."""
 
         self.last_pos = None
         self.technology = technology
-        self.clocking_scheme = "2DDWave" if self.technology == "SiDB" else clocking_scheme
+        self.clocking_scheme = (
+            "2DDWave"
+            if (self.technology == "SiDB" or clocking_scheme.upper() == "2DDWAVE")
+            else clocking_scheme.upper()
+        )
 
         self.layout_width = layout_width
         self.layout_height = layout_height
 
         self.layout = pyfiction.cartesian_obstruction_layout(
             pyfiction.cartesian_gate_layout(
                 (self.layout_width - 1, self.layout_height - 1, 1),
@@ -67,15 +71,15 @@
         self.start = time()
         self.placement_times = []
         self.occupied_tiles = np.zeros([self.layout_width, self.layout_height], dtype=int)
         self.gates = np.zeros([self.layout_width, self.layout_height], dtype=int)
         self.verbose = verbose
         self.layout_mask_width = 4
         self.layout_mask_height = 4
-        self.optimize = optimize if self.clocking_scheme == "2DDWave" else False
+        self.optimize = optimize if self.clocking_scheme.upper() == "2DDWAVE" else False
 
     def reset(self, seed: int = None, options: dict = None) -> tuple[int, dict]:  # noqa: ARG002
         """Creates a new empty layout and resets all placement variables.
 
         :param seed:       Sets random seed (not implemented)
         :param options:    Additional options (not implemented)
 
@@ -253,33 +257,33 @@
 
     def save_layout(self):
         """Creates cell layout and saves it as .svg for QCA and .dot for SiDB.
         If technology is set to gate-level, it will be saved as an .fgl file."""
         if not Path.exists(Path("layouts")):
             Path.mkdir(Path("layouts"), parents=True)
 
-        if self.technology == "QCA":
+        if self.technology.lower() == "qca":
             try:
                 cell_layout = pyfiction.apply_qca_one_library(self.layout)
                 params = pyfiction.write_qca_layout_svg_params()
                 params.simple = len(self.actions) > 200
                 pyfiction.write_qca_layout_svg(
                     cell_layout,
                     os.path.join("layouts", f"{self.function}_{self.clocking_scheme}_qca.svg"),
                     params,
                 )
             finally:
                 pass
-        elif self.technology == "SiDB":
+        elif self.technology.lower() == "sidb":
             try:
                 hex_layout = pyfiction.hexagonalization(self.layout)
                 pyfiction.write_dot_layout(hex_layout, os.path.join("layouts", f"{self.function}_ROW_sidb.dot"))
             finally:
                 pass
-        elif self.technology == "Gate-level":
+        elif self.technology.lower() == "gate-level":
             pyfiction.write_fgl_layout(
                 self.layout,
                 os.path.join(
                     "layouts",
                     f"{self.function}_ONE_{self.clocking_scheme}_NanoPlaceR_{'Un' if not self.optimize else ''}Opt_UnOrd.fgl",
                 ),
             )
@@ -335,50 +339,53 @@
         possible_positions_nodes = np.ones([self.layout_width, self.layout_height], dtype=int)
 
         self.layout_mask_width = int(8 + ((self.current_node * (self.layout_width - 8)) / len(self.actions))) + 1
         self.layout_mask_height = int(8 + ((self.current_node * (self.layout_height - 8)) / len(self.actions))) + 1
         if (
             self.node_to_action[self.actions[self.current_node]] not in ["INPUT", "OUTPUT"]
             and len(preceding_nodes) != 1
-        ) and (self.node_to_action[self.actions[self.current_node]] != "OUTPUT" and self.clocking_scheme == "2DDWave"):
+        ) and (
+            self.node_to_action[self.actions[self.current_node]] != "OUTPUT"
+            and self.clocking_scheme.upper() == "2DDWAVE"
+        ):
             possible_positions_nodes[: self.layout_mask_width, : self.layout_mask_height] = 0
 
         if self.node_to_action[self.actions[self.current_node]] == "INPUT":
-            if self.clocking_scheme == "2DDWave":
+            if self.clocking_scheme.upper() == "2DDWAVE":
                 possible_positions_nodes[0, : self.layout_mask_height] = 0
                 possible_positions_nodes[: self.layout_mask_width, 0] = 0
-            elif self.clocking_scheme in ("USE", "RES", "ESR"):
+            elif self.clocking_scheme.upper() in ("USE", "RES", "ESR"):
                 possible_positions_nodes[0, :] = 0
                 possible_positions_nodes[self.layout_width - 1, :] = 0
                 possible_positions_nodes[:, 0] = 0
                 possible_positions_nodes[:, self.layout_height - 1] = 0
             else:
                 error_message = f"Unsupported clocking scheme: {self.clocking_scheme}"
                 raise Exception(error_message)
 
         elif self.node_to_action[self.actions[self.current_node]] == "OUTPUT":
-            if self.clocking_scheme == "2DDWave":
+            if self.clocking_scheme.upper() == "2DDWAVE":
                 node = self.node_dict[preceding_nodes[0]]
                 loc = self.layout.get_tile(node)
                 possible_positions_nodes[self.layout_width - 1, loc.y - 1 : self.layout_mask_height] = 0
                 possible_positions_nodes[loc.x - 1 : self.layout_mask_width, self.layout_height - 1] = 0
-            elif self.clocking_scheme in ("USE", "RES", "ESR"):
+            elif self.clocking_scheme.upper() in ("USE", "RES", "ESR"):
                 possible_positions_nodes[0][:] = 0
                 possible_positions_nodes[self.layout_width - 1, 0] = 0
                 possible_positions_nodes[:, 0] = 0
                 possible_positions_nodes[:, self.layout_height - 1] = 0
             else:
                 error_message = f"Unsupported clocking scheme: {self.clocking_scheme}"
                 raise Exception(error_message)
 
         elif len(preceding_nodes) == 1 and self.node_to_action[self.actions[self.current_node]] != "OUTPUT":
             node = self.node_dict[preceding_nodes[0]]
             loc = self.layout.get_tile(node)
             for zone in self.layout.outgoing_clocked_zones(loc):
-                if self.clocking_scheme == "2DDWave":
+                if self.clocking_scheme.upper() == "2DDWAVE":
                     if (
                         self.layout.is_empty_tile((zone.x, zone.y, 0))
                         and zone.x < self.layout_mask_width
                         and zone.y < self.layout_mask_height
                     ):
                         possible_positions_nodes[zone.x][zone.y] = 0
                 else:
@@ -393,15 +400,15 @@
                             self.layout.is_empty_tile((second_zone.x, second_zone.y, 0))
                             and second_zone.x in range(0, self.layout_width)
                             and second_zone.y in range(0, self.layout_height)
                         ):
                             possible_positions_nodes[second_zone.x][second_zone.y] = 0
 
         elif len(preceding_nodes) == 2:
-            if self.clocking_scheme == "2DDWave":
+            if self.clocking_scheme.upper() == "2DDWAVE":
                 node_1 = self.node_dict[preceding_nodes[0]]
                 loc_1 = self.layout.get_tile(node_1)
                 node_2 = self.node_dict[preceding_nodes[1]]
                 loc_2 = self.layout.get_tile(node_2)
                 min_x = max(loc_1.x, loc_2.x)
                 min_y = max(loc_1.y, loc_2.y)
                 if loc_1.x == loc_2.x:
@@ -436,21 +443,21 @@
                     ):
                         possible = True
                 params = pyfiction.a_star_params()
                 params.crossings = True
 
                 width = self.layout_width + 1
                 height = self.layout_height + 1
-                if self.clocking_scheme in ("RES", "ESR"):
+                if self.clocking_scheme.upper() in ("RES", "ESR"):
                     if ((self.layout_width + 1) % 4) == 1:
                         width += 1
                     elif ((self.layout_height + 1) % 4) == 2:
                         height += 1
                 self.layout.resize((width - 1, height - 1, 1))
-                if self.clocking_scheme in ("USE", "RES", "ESR"):
+                if self.clocking_scheme.upper() in ("USE", "RES", "ESR"):
                     goals = []
                     if (width % 2 == 0) and (height % 2 == 0):
                         goals.append((0, width - 1))
                     elif (width % 2 == 1) and (height % 2 == 1):
                         goals.append((width - 1, 0))
                     elif (width % 2 == 0) and (height % 2 == 1):
                         goals.append((width - 1, height - 1))
@@ -464,15 +471,15 @@
                         if len(pyfiction.a_star(self.layout, tile, goal, params)) == 0:
                             possible = False
                         else:
                             overall = True
                         if overall:
                             possible = True
                 elif (
-                    self.clocking_scheme == "2DDWave"
+                    self.clocking_scheme.upper() == "2DDWAVE"
                     and possible
                     and (
                         len(
                             pyfiction.a_star(
                                 self.layout,
                                 tile,
                                 (
@@ -510,15 +517,15 @@
         :param x:              X-coordinate of the placed gate
         :param y:              Y-coordinate of the placed gate
         :param placed_node:    Indicates whether a gate was placed or not
 
         :return:               Reward and termination indicator
         """
         reward = 10000 if self.current_node == len(self.actions) else placed_node
-        if placed_node and self.clocking_scheme == "2DDWave":
+        if placed_node and self.clocking_scheme.upper() == "2DDWAVE":
             reward *= 1 - ((x + y) / (self.layout_mask_width * self.layout_mask_height))
 
         done = bool(self.current_node == len(self.actions) or not self.placement_possible)
         if self.current_node > self.max_placed_nodes:
             print(f"New best placement: {self.current_node}/{len(self.actions)} ({time() - self.start:.2f}s)")
             if self.verbose == 1:
                 print(self.layout)
```

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py` & `mnt_nanoplacer-0.2.3/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import networkx as nx
+
 from mnt import pyfiction
 
 
 def map_to_multidiscrete(action: int, layout_width: int) -> tuple[int, int]:
     """Map a discrete action to the corresponding coordinate on a Cartesian grid.
 
     :param action:         Discrete action used by the RL agent
@@ -65,28 +66,28 @@
     """
 
     yield from topological_generations(dg)
 
 
 def create_action_list(
     benchmark, function
-) -> tuple[pyfiction.logic_network, dict[int, str], list[int], nx.DiGraph, list[str], list[str]]:
+) -> tuple[pyfiction.technology_network, dict[int, str], list[int], nx.DiGraph, list[str], list[str]]:
     """Create a topological odering of the network and a mapping of node to gate type.
 
     :param benchmark:    Benchmark set
     :param function:     Function in the benchmark set
 
     :return:    network:           Network of the logic function
     :return:    node_to_action:    Dictionary mapping node to gate type
     :return:    actions:           Topological sort of the network nodes
     :return:    dg:                Digraph representation of the logic network
     """
     dir_path = Path(__file__).parent.parent.parent.resolve()
     path = dir_path / "benchmarks" / benchmark / f"{function}.v"
-    network = pyfiction.read_logic_network(str(path))
+    network = pyfiction.read_technology_network(str(path))
 
     pi_names = [network.get_name(pi) for pi in network.pis()]
     po_names = [network.get_output_name(network.po_index(po)) for po in network.pos()]
 
     # mapping_params = pyfiction.and_or_not()
     # network = pyfiction.technology_mapping(network, mapping_params)
```

### Comparing `mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/PKG-INFO` & `mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnt.nanoplacer
-Version: 0.2.2
+Version: 0.2.3
 Summary: NanoPlaceR - An open-source framework for placement and routing of Field-coupled Nanotechnologies based on reinforcement learning.
 Author-email: Simon Hofmann <simon.t.hofmann@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Chair for Design Automation, TU Munich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,30 +37,31 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: <=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: networkx>=3.1
-Requires-Dist: numpy>=1.24.3
-Requires-Dist: pre-commit>=3.3.3
-Requires-Dist: setuptools>=65.5.1
+Requires-Dist: networkx>=3.2.1
+Requires-Dist: numpy>=1.26.3
+Requires-Dist: pre-commit>=3.6.0
+Requires-Dist: setuptools>=68.2.0
 Requires-Dist: sb3_contrib>=2.2.1
-Requires-Dist: tensorboard>=2.13.0
+Requires-Dist: tensorboard>=2.15.1
 Requires-Dist: wheel>=0.38.0
-Requires-Dist: mnt.pyfiction>=0.5.0
+Requires-Dist: mnt.pyfiction>=0.6.1
 Provides-Extra: test
-Requires-Dist: pytest>=7.2; extra == "test"
+Requires-Dist: pytest>=8.2.1; extra == "test"
 Provides-Extra: coverage
 Requires-Dist: mnt.nanoplacer[test]; extra == "coverage"
 Requires-Dist: pytest-cov[toml]; extra == "coverage"
 
 [![PyPI](https://img.shields.io/pypi/v/mnt.nanoplacer?logo=pypi&style=flat-square)](https://pypi.org/project/mnt.nanoplacer/)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/mnt-nanoplacer/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/mnt-nanoplacer/actions/workflows/deploy.yml)
@@ -153,15 +154,15 @@
   -r,  --reset_model               If True, reset saved model and train from scratch (defautls to False).
   -v,  --verbosity                 0: No information. 1: Print layout after every new best placement. 2: Print training metrics. 3: 1 and 2 combined.
 ```
 
 For example to create the gate-level layout for the mux21 function from trindade16 on the 2DDWave clocking scheme using the best found layout dimensions (by training for a maximum of 10000 timesteps):
 
 ```
-mnt.nanoplacer -b "trindade16" -f "mux21" -c "2DDWave" -t "gate-level" -l -ts 10000 -v 1
+mnt.nanoplacer -b "trindade16" -f "mux21" -c "2DDWave" -t "Gate-level" -l -ts 10000 -v 1
 ```
 
 # Repository Structure
 
 ```
 .
 ├── docs/
```

### Comparing `mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/SOURCES.txt` & `mnt_nanoplacer-0.2.3/src/mnt.nanoplacer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/tests/test_env.py` & `mnt_nanoplacer-0.2.3/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/tests/test_main.py` & `mnt_nanoplacer-0.2.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mnt_nanoplacer-0.2.2/tests/test_utils.py` & `mnt_nanoplacer-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

