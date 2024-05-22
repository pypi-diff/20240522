# Comparing `tmp/shenfun-4.1.4.tar.gz` & `tmp/shenfun-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shenfun-4.1.4.tar", last modified: Wed Nov  8 13:08:39 2023, max compression
+gzip compressed data, was "shenfun-4.2.0.tar", last modified: Wed May 22 06:51:01 2024, max compression
```

## Comparing `shenfun-4.1.4.tar` & `shenfun-4.2.0.tar`

### file list

```diff
@@ -1,129 +1,126 @@
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.417874 shenfun-4.1.4/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       89 2023-04-27 11:17:36.000000 shenfun-4.1.4/.codacy.yml
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1321 2019-12-10 14:07:27.000000 shenfun-4.1.4/LICENSE
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       81 2019-12-10 14:07:27.000000 shenfun-4.1.4/MANIFEST.in
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     8156 2023-11-08 13:08:39.417624 shenfun-4.1.4/PKG-INFO
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7347 2023-03-14 09:32:55.000000 shenfun-4.1.4/README.rst
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2720 2023-10-20 19:03:57.000000 shenfun-4.1.4/azure-pipelines.yml
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      848 2022-11-24 15:41:09.000000 shenfun-4.1.4/leg2chebX.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      208 2021-09-17 07:57:46.000000 shenfun-4.1.4/readthedocs.yml
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       63 2021-08-27 18:22:41.000000 shenfun-4.1.4/requirements.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       38 2023-11-08 13:08:39.417954 shenfun-4.1.4/setup.cfg
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4717 2022-12-07 11:26:25.000000 shenfun-4.1.4/setup.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.351784 shenfun-4.1.4/shenfun/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2123 2023-11-08 13:01:42.000000 shenfun-4.1.4/shenfun/__init__.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.355586 shenfun-4.1.4/shenfun/bessel/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       45 2022-08-18 13:39:44.000000 shenfun-4.1.4/shenfun/bessel/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    10493 2022-09-01 07:19:30.000000 shenfun-4.1.4/shenfun/bessel/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1066 2022-09-01 07:20:07.000000 shenfun-4.1.4/shenfun/bessel/matrices.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.358766 shenfun-4.1.4/shenfun/chebyshev/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      115 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/chebyshev/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    74772 2023-10-17 14:15:45.000000 shenfun-4.1.4/shenfun/chebyshev/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    18730 2022-09-21 09:08:14.000000 shenfun-4.1.4/shenfun/chebyshev/la.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    53585 2023-10-17 13:46:56.000000 shenfun-4.1.4/shenfun/chebyshev/matrices.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.361627 shenfun-4.1.4/shenfun/chebyshevu/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      113 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/chebyshevu/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    47603 2023-03-09 14:32:05.000000 shenfun-4.1.4/shenfun/chebyshevu/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     6819 2022-08-17 08:02:46.000000 shenfun-4.1.4/shenfun/chebyshevu/matrices.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2877 2023-04-13 06:41:35.000000 shenfun-4.1.4/shenfun/config.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11025 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/coordinates.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.365965 shenfun-4.1.4/shenfun/forms/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      129 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/forms/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    73188 2023-04-27 11:43:11.000000 shenfun-4.1.4/shenfun/forms/arguments.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    25050 2023-10-16 19:23:27.000000 shenfun-4.1.4/shenfun/forms/inner.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     9896 2022-09-22 14:19:28.000000 shenfun-4.1.4/shenfun/forms/operators.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    10048 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/forms/project.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.368074 shenfun-4.1.4/shenfun/fourier/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2968 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/fourier/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    23031 2022-08-25 07:50:09.000000 shenfun-4.1.4/shenfun/fourier/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     6388 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/fourier/matrices.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.369875 shenfun-4.1.4/shenfun/hermite/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       45 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/hermite/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5827 2022-08-15 15:26:27.000000 shenfun-4.1.4/shenfun/hermite/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3342 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/hermite/matrices.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.371136 shenfun-4.1.4/shenfun/io/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4191 2023-01-31 09:18:01.000000 shenfun-4.1.4/shenfun/io/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11789 2023-01-31 15:13:16.000000 shenfun-4.1.4/shenfun/io/generate_xdmf.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.374079 shenfun-4.1.4/shenfun/jacobi/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       45 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/jacobi/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    43811 2023-03-09 14:55:30.000000 shenfun-4.1.4/shenfun/jacobi/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      725 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/jacobi/matrices.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    18706 2023-10-16 19:29:06.000000 shenfun-4.1.4/shenfun/jacobi/recursions.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    48864 2023-02-22 15:20:15.000000 shenfun-4.1.4/shenfun/la.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.375984 shenfun-4.1.4/shenfun/laguerre/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       45 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/laguerre/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    12895 2022-08-17 07:19:20.000000 shenfun-4.1.4/shenfun/laguerre/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2368 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/laguerre/matrices.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.381742 shenfun-4.1.4/shenfun/legendre/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      166 2022-09-15 13:42:41.000000 shenfun-4.1.4/shenfun/legendre/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    55822 2023-10-17 12:16:10.000000 shenfun-4.1.4/shenfun/legendre/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    50866 2023-04-27 11:14:42.000000 shenfun-4.1.4/shenfun/legendre/dlt.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.383236 shenfun-4.1.4/shenfun/legendre/fastgl/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       45 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/legendre/fastgl/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1290 2023-10-05 08:41:25.000000 shenfun-4.1.4/shenfun/legendre/fastgl/fastgl_wrap.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5589 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/legendre/la.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      482 2022-10-26 07:16:08.000000 shenfun-4.1.4/shenfun/legendre/leg2chebX.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1036 2023-03-10 07:22:12.000000 shenfun-4.1.4/shenfun/legendre/lobatto.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    32598 2023-02-23 17:59:15.000000 shenfun-4.1.4/shenfun/legendre/matrices.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    81027 2023-10-17 12:16:17.000000 shenfun-4.1.4/shenfun/matrixbase.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.383860 shenfun-4.1.4/shenfun/optimization/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2374 2022-11-25 14:08:37.000000 shenfun-4.1.4/shenfun/optimization/__init__.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.393462 shenfun-4.1.4/shenfun/optimization/cython/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1820 2023-02-23 16:18:26.000000 shenfun-4.1.4/shenfun/optimization/cython/Cheb.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    33021 2022-12-06 13:35:42.000000 shenfun-4.1.4/shenfun/optimization/cython/Matvec.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      942 2023-04-03 14:32:44.000000 shenfun-4.1.4/shenfun/optimization/cython/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5564 2019-12-10 14:07:27.000000 shenfun-4.1.4/shenfun/optimization/cython/applymask.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2057 2019-12-10 14:07:27.000000 shenfun-4.1.4/shenfun/optimization/cython/convolve.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1107 2022-06-13 09:50:19.000000 shenfun-4.1.4/shenfun/optimization/cython/cross.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    38733 2021-06-01 05:18:36.000000 shenfun-4.1.4/shenfun/optimization/cython/evaluate.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    84138 2022-11-25 15:11:54.000000 shenfun-4.1.4/shenfun/optimization/cython/la.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     9597 2023-04-03 14:40:24.000000 shenfun-4.1.4/shenfun/optimization/cython/leg2chebm.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2697 2019-12-10 14:07:27.000000 shenfun-4.1.4/shenfun/optimization/cython/outer.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    34893 2023-05-02 10:49:13.000000 shenfun-4.1.4/shenfun/optimization/cython/transforms.pyx
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.400375 shenfun-4.1.4/shenfun/optimization/numba/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     8420 2022-09-15 12:00:59.000000 shenfun-4.1.4/shenfun/optimization/numba/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    18663 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/biharmonic.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1115 2023-01-02 14:35:35.000000 shenfun-4.1.4/shenfun/optimization/numba/chebyshev.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      752 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/diagma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1398 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/fdma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    17997 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/helmholtz.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2392 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/heptadma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3015 2022-10-13 08:37:19.000000 shenfun-4.1.4/shenfun/optimization/numba/la.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1782 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/pdma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2279 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/tdma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1056 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/threedma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    13085 2023-02-15 15:33:01.000000 shenfun-4.1.4/shenfun/optimization/numba/transforms.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      914 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/optimization/numba/twodma.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    82359 2023-10-19 17:13:15.000000 shenfun-4.1.4/shenfun/spectralbase.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    78537 2023-04-27 11:32:27.000000 shenfun-4.1.4/shenfun/tensorproductspace.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.402369 shenfun-4.1.4/shenfun/ultraspherical/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       45 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/ultraspherical/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    41658 2023-03-09 14:52:13.000000 shenfun-4.1.4/shenfun/ultraspherical/bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      950 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/ultraspherical/matrices.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.404985 shenfun-4.1.4/shenfun/utilities/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    21595 2023-10-06 14:02:53.000000 shenfun-4.1.4/shenfun/utilities/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4004 2023-03-10 09:20:08.000000 shenfun-4.1.4/shenfun/utilities/findbasis.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    27937 2023-07-11 11:56:31.000000 shenfun-4.1.4/shenfun/utilities/integrators.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3514 2022-08-15 12:15:32.000000 shenfun-4.1.4/shenfun/utilities/lagrangian_particles.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.354201 shenfun-4.1.4/shenfun.egg-info/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     8156 2023-11-08 13:08:38.000000 shenfun-4.1.4/shenfun.egg-info/PKG-INFO
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3939 2023-11-08 13:08:39.000000 shenfun-4.1.4/shenfun.egg-info/SOURCES.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)        1 2023-11-08 13:08:38.000000 shenfun-4.1.4/shenfun.egg-info/dependency_links.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       37 2023-11-08 13:08:38.000000 shenfun-4.1.4/shenfun.egg-info/requires.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)        8 2023-11-08 13:08:38.000000 shenfun-4.1.4/shenfun.egg-info/top_level.txt
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-11-08 13:08:39.416304 shenfun-4.1.4/tests/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     8877 2023-02-23 14:39:35.000000 shenfun-4.1.4/tests/test_backward.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1971 2022-08-15 15:33:38.000000 shenfun-4.1.4/tests/test_bases.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5226 2022-08-15 12:15:32.000000 shenfun-4.1.4/tests/test_curl.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3176 2022-08-15 12:15:32.000000 shenfun-4.1.4/tests/test_curvilinear.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1168 2023-02-23 19:42:22.000000 shenfun-4.1.4/tests/test_demos.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2393 2022-08-23 10:47:28.000000 shenfun-4.1.4/tests/test_dot.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     6393 2022-08-15 12:15:32.000000 shenfun-4.1.4/tests/test_forms.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      902 2022-08-15 12:15:32.000000 shenfun-4.1.4/tests/test_fourier.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     6345 2023-01-31 09:21:09.000000 shenfun-4.1.4/tests/test_io.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1261 2023-02-22 15:28:07.000000 shenfun-4.1.4/tests/test_la.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1208 2022-08-15 12:15:32.000000 shenfun-4.1.4/tests/test_lagrangian_particles.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    27588 2023-10-19 18:21:04.000000 shenfun-4.1.4/tests/test_matrices.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4435 2022-08-15 12:15:32.000000 shenfun-4.1.4/tests/test_spectralbase.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    22163 2023-02-18 15:53:39.000000 shenfun-4.1.4/tests/test_tensorproductspace.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    22410 2023-03-09 14:56:36.000000 shenfun-4.1.4/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.704492 shenfun-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 06:50:50.000000 shenfun-4.2.0/.codacy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 06:50:50.000000 shenfun-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 06:50:50.000000 shenfun-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-22 06:51:01.704492 shenfun-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-22 06:50:50.000000 shenfun-4.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 06:50:51.000000 shenfun-4.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-22 06:50:51.000000 shenfun-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:51:01.704492 shenfun-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-22 06:50:51.000000 shenfun-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.688492 shenfun-4.2.0/shenfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.688492 shenfun-4.2.0/shenfun/chebyshev/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75410 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshev/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshev/la.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53585 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshev/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/chebyshevu/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshevu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47603 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshevu/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/chebyshevu/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73193 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/forms/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25335 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/forms/inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/forms/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/forms/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/fourier/
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/fourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/fourier/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/fourier/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/hermite/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/hermite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/hermite/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/hermite/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/io/generate_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/jacobi/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/jacobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43811 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/jacobi/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/jacobi/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18706 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/jacobi/recursions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48874 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/la.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.692492 shenfun-4.2.0/shenfun/laguerre/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/laguerre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12895 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/laguerre/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/laguerre/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.696492 shenfun-4.2.0/shenfun/legendre/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55830 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50928 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/dlt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.696492 shenfun-4.2.0/shenfun/legendre/fastgl/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/fastgl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173232 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/fastgl/fastgl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/fastgl/fastgl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/fastgl/fastgl_wrap.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/fastgl/fastgl_wrap.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/la.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/lobatto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32598 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/legendre/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81468 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/matrixbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.696492 shenfun-4.2.0/shenfun/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.700492 shenfun-4.2.0/shenfun/optimization/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/Cheb.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    33021 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/Matvec.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/applymask.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/convolve.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/cross.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/evaluate.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    84138 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/la.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/leg2chebm.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/outer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/transforms.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    34893 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/cython/transforms.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.700492 shenfun-4.2.0/shenfun/optimization/numba/
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/biharmonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/diagma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/fdma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17997 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/helmholtz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/heptadma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/la.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/pdma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/tdma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/threedma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/optimization/numba/twodma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83484 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/spectralbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78999 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/tensorproductspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.700492 shenfun-4.2.0/shenfun/ultraspherical/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/ultraspherical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41658 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/ultraspherical/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/ultraspherical/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.700492 shenfun-4.2.0/shenfun/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/utilities/findbasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/utilities/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-22 06:50:51.000000 shenfun-4.2.0/shenfun/utilities/lagrangian_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.704492 shenfun-4.2.0/shenfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-22 06:51:01.000000 shenfun-4.2.0/shenfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-22 06:51:01.000000 shenfun-4.2.0/shenfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:51:01.000000 shenfun-4.2.0/shenfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 06:51:01.000000 shenfun-4.2.0/shenfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 06:51:01.000000 shenfun-4.2.0/shenfun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:51:01.704492 shenfun-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_backward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_curvilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_la.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_lagrangian_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27588 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_spectralbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_tensorproductspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-05-22 06:50:51.000000 shenfun-4.2.0/tests/test_transforms.py
```

### Comparing `shenfun-4.1.4/LICENSE` & `shenfun-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/PKG-INFO` & `shenfun-4.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 Metadata-Version: 2.1
 Name: shenfun
-Version: 4.1.4
+Version: 4.2.0
 Summary: Shenfun -- Automated Spectral-Galerkin framework
 Home-page: https://github.com/spectralDNS/shenfun
 Author: Mikael Mortensen
 Author-email: mikaem@math.uio.no
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: mpi4py-fft
+Requires-Dist: mpi4py
+Requires-Dist: cython
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 Shenfun
 =======
 .. image:: https://app.codacy.com/project/badge/Grade/bd772b3ca7134651a9225d8051db8c41
     :target: https://www.codacy.com/gh/spectralDNS/shenfun/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=spectralDNS/shenfun&amp;utm_campaign=Badge_Grade
 .. image:: https://dev.azure.com/spectralDNS/shenfun/_apis/build/status/spectralDNS.shenfun?branchName=master
     :target: https://dev.azure.com/spectralDNS/shenfun
 .. image:: https://github.com/spectralDNS/shenfun/workflows/github-CI/badge.svg?branch=master
     :target: https://github.com/spectralDNS/shenfun
 .. image:: https://codecov.io/gh/spectralDNS/shenfun/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/spectralDNS/shenfun
 .. image:: https://anaconda.org/conda-forge/shenfun/badges/platforms.svg
     :target: https://anaconda.org/conda-forge/shenfun
-.. |binder| image:: https://mybinder.org/badge_logo.svg
-    :target: https://mybinder.org/v2/gh/spectralDNS/shenfun/master?filepath=binder
-
-
-Try it in a jupyter hub using Binder
-
-|binder|
 
 Description
 -----------
 Shenfun is a high performance computing platform for solving partial differential equations (PDEs) by the spectral Galerkin method. The user interface to shenfun is very similar to `FEniCS <https://fenicsproject.org>`_, but applications are limited to multidimensional tensor product grids, using either Cartesian or curvilinear grids (e.g., but not limited to, polar, cylindrical, spherical or parabolic). The code is parallelized with MPI through the `mpi4py-fft <https://bitbucket.org/mpi4py/mpi4py-fft>`_ package.
 
 Shenfun enables fast development of efficient and accurate PDE solvers (spectral order and accuracy), in the comfortable high-level Python language. The spectral accuracy is ensured by using high-order *global* orthogonal basis functions (Fourier, Legendre, Chebyshev first and second kind, Ultraspherical, Jacobi, Laguerre and Hermite), as opposed to finite element codes that are using low-order *local* basis functions. Efficiency is ensured through vectorization (`Numpy <https://www.numpy.org/>`_), parallelization (`mpi4py <https://bitbucket.org/mpi4py/mpi4py>`_) and by moving critical routines to `Cython <https://cython.org/>`_ or `Numba <https://numba.pydata.org>`_. Shenfun has been used to run turbulence simulations (Direct Numerical Simulations) on thousands of processors on high-performance supercomputers, see the `spectralDNS <https://github.com/spectralDNS/spectralDNS>`_ repository.
 
 The demo folder contains several examples for the Poisson, Helmholtz and Biharmonic equations. For extended documentation and installation instructions see `ReadTheDocs <http://shenfun.readthedocs.org>`_. For interactive demos, see the `jupyter book <https://mikaem.github.io/shenfun-demos>`_. Note that shenfun currently comes with the possibility to use two non-periodic directions (see `biharmonic demo <https://github.com/spectralDNS/shenfun/blob/master/demo/biharmonic2D_2nonperiodic.py>`_), and equations may be solved coupled and implicit (see `MixedPoisson.py <https://github.com/spectralDNS/shenfun/blob/master/demo/MixedPoisson.py>`_).
 
-Note that shenfun works with curvilinear coordinates. For example, it is possible to solve equations on a `sphere <https://github.com/spectralDNS/shenfun/blob/master/demo/sphere_helmholtz.py>`_ (using spherical coordinates), on the surface of a `torus <https://github.com/spectralDNS/shenfun/blob/master/binder/Torus.ipynb>`_, on a `Möbius strip <https://mikaem.github.io/shenfun-demos/content/moebius.html>`_ or along any `curved line in 2D/3D <https://github.com/spectralDNS/shenfun/blob/master/demo/curvilinear_poisson1D.py>`_. Actually, any new coordinates may be defined by the user as long as the coordinates lead to a system of equations with separable coefficients. After defining new coordinates, operators like div, grad and curl work automatically with the new curvilinear coordinates. See also `this notebook on the sphere <https://github.com/spectralDNS/shenfun/blob/master/binder/sphere-helmholtz.ipynb>`_ or an illustration of the `vector Laplacian <https://github.com/spectralDNS/shenfun/blob/master/binder/vector-laplacian.ipynb>`_.
+Note that shenfun works with curvilinear coordinates. For example, it is possible to solve equations on a `sphere <https://github.com/spectralDNS/shenfun/blob/master/demo/sphere_helmholtz.py>`_ (using spherical coordinates), on the surface of a `torus <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/Torus.ipynb>`_, on a `Möbius strip <https://mikaem.github.io/shenfun-demos/content/moebius.html>`_ or along any `curved line in 2D/3D <https://github.com/spectralDNS/shenfun/blob/master/demo/curvilinear_poisson1D.py>`_. Actually, any new coordinates may be defined by the user as long as the coordinates lead to a system of equations with separable coefficients. After defining new coordinates, operators like div, grad and curl work automatically with the new curvilinear coordinates. See also `this notebook on the sphere <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/sphere-helmholtz.ipynb>`_ or an illustration of the `vector Laplacian <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/vector-laplacian.ipynb>`_.
 
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/moebius8_trans.png
     :target: https://mikaem.github.io/shenfun-demos/content/moebius.html
     :alt: The eigenvector of the 8'th smallest eigvalue on a Möbius strip
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/smallcoil2.png
     :alt: Solution of Poisson's equation on a Coil
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/spherewhite4.png
     :target: https://mikaem.github.io/shenfun-demos/content/sphericalhelmholtz.html
     :alt: Solution of Poisson's equation on a spherical shell
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/torus2.png
-    :target: https://github.com/spectralDNS/shenfun/blob/master/binder/Torus.ipynb
+    :target: https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/Torus.ipynb
     :alt: Solution of Poisson's equation on the surface of a torus
 
 
 For a more psychedelic experience, have a look at the `simulation <https://github.com/spectralDNS/shenfun/blob/master/demo/Ginzburg_Landau_sphere_IRK3.py>`_ of the Ginzburg-Landau equation on the sphere (click for Youtube-video):
 
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/GLimage.png
     :target: https://youtu.be/odsIoHVcqek
@@ -99,9 +95,7 @@
 
     Mikael Mortensen
     mikaem at math.uio.no
     https://mikaem.github.io/
     Department of Mathematics
     University of Oslo
     Norway
-
-
```

### Comparing `shenfun-4.1.4/README.rst` & `shenfun-4.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,42 +6,35 @@
     :target: https://dev.azure.com/spectralDNS/shenfun
 .. image:: https://github.com/spectralDNS/shenfun/workflows/github-CI/badge.svg?branch=master
     :target: https://github.com/spectralDNS/shenfun
 .. image:: https://codecov.io/gh/spectralDNS/shenfun/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/spectralDNS/shenfun
 .. image:: https://anaconda.org/conda-forge/shenfun/badges/platforms.svg
     :target: https://anaconda.org/conda-forge/shenfun
-.. |binder| image:: https://mybinder.org/badge_logo.svg
-    :target: https://mybinder.org/v2/gh/spectralDNS/shenfun/master?filepath=binder
-
-
-Try it in a jupyter hub using Binder
-
-|binder|
 
 Description
 -----------
 Shenfun is a high performance computing platform for solving partial differential equations (PDEs) by the spectral Galerkin method. The user interface to shenfun is very similar to `FEniCS <https://fenicsproject.org>`_, but applications are limited to multidimensional tensor product grids, using either Cartesian or curvilinear grids (e.g., but not limited to, polar, cylindrical, spherical or parabolic). The code is parallelized with MPI through the `mpi4py-fft <https://bitbucket.org/mpi4py/mpi4py-fft>`_ package.
 
 Shenfun enables fast development of efficient and accurate PDE solvers (spectral order and accuracy), in the comfortable high-level Python language. The spectral accuracy is ensured by using high-order *global* orthogonal basis functions (Fourier, Legendre, Chebyshev first and second kind, Ultraspherical, Jacobi, Laguerre and Hermite), as opposed to finite element codes that are using low-order *local* basis functions. Efficiency is ensured through vectorization (`Numpy <https://www.numpy.org/>`_), parallelization (`mpi4py <https://bitbucket.org/mpi4py/mpi4py>`_) and by moving critical routines to `Cython <https://cython.org/>`_ or `Numba <https://numba.pydata.org>`_. Shenfun has been used to run turbulence simulations (Direct Numerical Simulations) on thousands of processors on high-performance supercomputers, see the `spectralDNS <https://github.com/spectralDNS/spectralDNS>`_ repository.
 
 The demo folder contains several examples for the Poisson, Helmholtz and Biharmonic equations. For extended documentation and installation instructions see `ReadTheDocs <http://shenfun.readthedocs.org>`_. For interactive demos, see the `jupyter book <https://mikaem.github.io/shenfun-demos>`_. Note that shenfun currently comes with the possibility to use two non-periodic directions (see `biharmonic demo <https://github.com/spectralDNS/shenfun/blob/master/demo/biharmonic2D_2nonperiodic.py>`_), and equations may be solved coupled and implicit (see `MixedPoisson.py <https://github.com/spectralDNS/shenfun/blob/master/demo/MixedPoisson.py>`_).
 
-Note that shenfun works with curvilinear coordinates. For example, it is possible to solve equations on a `sphere <https://github.com/spectralDNS/shenfun/blob/master/demo/sphere_helmholtz.py>`_ (using spherical coordinates), on the surface of a `torus <https://github.com/spectralDNS/shenfun/blob/master/binder/Torus.ipynb>`_, on a `Möbius strip <https://mikaem.github.io/shenfun-demos/content/moebius.html>`_ or along any `curved line in 2D/3D <https://github.com/spectralDNS/shenfun/blob/master/demo/curvilinear_poisson1D.py>`_. Actually, any new coordinates may be defined by the user as long as the coordinates lead to a system of equations with separable coefficients. After defining new coordinates, operators like div, grad and curl work automatically with the new curvilinear coordinates. See also `this notebook on the sphere <https://github.com/spectralDNS/shenfun/blob/master/binder/sphere-helmholtz.ipynb>`_ or an illustration of the `vector Laplacian <https://github.com/spectralDNS/shenfun/blob/master/binder/vector-laplacian.ipynb>`_.
+Note that shenfun works with curvilinear coordinates. For example, it is possible to solve equations on a `sphere <https://github.com/spectralDNS/shenfun/blob/master/demo/sphere_helmholtz.py>`_ (using spherical coordinates), on the surface of a `torus <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/Torus.ipynb>`_, on a `Möbius strip <https://mikaem.github.io/shenfun-demos/content/moebius.html>`_ or along any `curved line in 2D/3D <https://github.com/spectralDNS/shenfun/blob/master/demo/curvilinear_poisson1D.py>`_. Actually, any new coordinates may be defined by the user as long as the coordinates lead to a system of equations with separable coefficients. After defining new coordinates, operators like div, grad and curl work automatically with the new curvilinear coordinates. See also `this notebook on the sphere <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/sphere-helmholtz.ipynb>`_ or an illustration of the `vector Laplacian <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/vector-laplacian.ipynb>`_.
 
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/moebius8_trans.png
     :target: https://mikaem.github.io/shenfun-demos/content/moebius.html
     :alt: The eigenvector of the 8'th smallest eigvalue on a Möbius strip
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/smallcoil2.png
     :alt: Solution of Poisson's equation on a Coil
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/spherewhite4.png
     :target: https://mikaem.github.io/shenfun-demos/content/sphericalhelmholtz.html
     :alt: Solution of Poisson's equation on a spherical shell
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/torus2.png
-    :target: https://github.com/spectralDNS/shenfun/blob/master/binder/Torus.ipynb
+    :target: https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/Torus.ipynb
     :alt: Solution of Poisson's equation on the surface of a torus
 
 
 For a more psychedelic experience, have a look at the `simulation <https://github.com/spectralDNS/shenfun/blob/master/demo/Ginzburg_Landau_sphere_IRK3.py>`_ of the Ginzburg-Landau equation on the sphere (click for Youtube-video):
 
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/GLimage.png
     :target: https://youtu.be/odsIoHVcqek
```

### Comparing `shenfun-4.1.4/setup.py` & `shenfun-4.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import os
 import re
 import subprocess
-from setuptools import setup, Extension
+from setuptools import setup
+from setuptools.extension import Extension
 from setuptools.command.build_ext import build_ext
 from numpy import get_include
 
 cwd = os.path.abspath(os.path.dirname(__file__))
 cdir = os.path.join(cwd, "shenfun", "optimization", "cython")
 
 def has_flag(compiler, flagname):
@@ -18,46 +19,49 @@
     p = subprocess.Popen([compiler.compiler[0], '-E', '-'] + [flagname],
                          stdin=subprocess.PIPE, stdout=devnull, stderr=devnull)
     p.communicate("")
     return True if p.returncode == 0 else False
 
 class build_ext_subclass(build_ext):
     def build_extensions(self):
-        extra_compile_args = ['-g0']
+        extra_compile_args = []
         if os.environ.get("READTHEDOCS", None) == "True":
             extra_compile_args.append('-O0')
         else:
             extra_compile_args.append('-O3')
             if not os.environ.get('CONDA_BUILD', 0):
-                for c in ['-w', '-Ofast', '-ffast-math', '-march=native']:
+                for c in ['-w', '-Ofast']:
                     if has_flag(self.compiler, c):
                         extra_compile_args.append(c)
 
         for e in self.extensions:
-            e.extra_compile_args += extra_compile_args
+            #e.extra_compile_args += extra_compile_args
             e.include_dirs.extend([get_include()])
         build_ext.build_extensions(self)
 
 def get_extensions():
-    ext = []
-    for s in ("Matvec", "la", "evaluate", "transforms", "leg2chebm"):
+    ext = [Extension("shenfun.legendre.fastgl.fastgl_wrap",
+                         libraries=["m"],
+                         language="c++",
+                         sources=[os.path.join(cwd, "shenfun", "legendre", "fastgl", "fastgl_wrap.pyx")],
+                         define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')])]
+    for s in ("transforms", "leg2chebm", "Matvec", "la", "evaluate"):
         ext.append(Extension("shenfun.optimization.cython.{0}".format(s),
-                             libraries=['m'],
-                             sources=[os.path.join(cdir, '{0}.pyx'.format(s))],
-                             language="c++"))  # , define_macros=define_macros
-    ext.append(Extension("shenfun.legendre.fastgl.fastgl_wrap",
-                         libraries=['m'],
-                         language='c++',
-                         sources=[os.path.join(cwd, "shenfun", "legendre", "fastgl", "fastgl_wrap.pyx")]))
+                             libraries=["m"],
+                             sources=[os.path.join(cdir, "{0}.pyx".format(s))],
+                             language="c++",
+                             define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')]))  # , define_macros=define_macros
+    
     [e.extra_link_args.extend(["-std=c++11"]) for e in ext]
     #[e.extra_link_args.extend(["-std=c++11", "-fopenmp"]) for e in ext]
     for s in ("Cheb", "convolve", "outer", "applymask", "cross"):
         ext.append(Extension("shenfun.optimization.cython.{0}".format(s),
-                             libraries=['m'],
-                             sources=[os.path.join(cdir, '{0}.pyx'.format(s))]))
+                             libraries=["m"],
+                             sources=[os.path.join(cdir, "{0}.pyx".format(s))],
+                             define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')]))
 
     return ext
 
 def version():
     srcdir = os.path.join(cwd, 'shenfun')
     with open(os.path.join(srcdir, '__init__.py')) as f:
         m = re.search(r"__version__\s*=\s*'(.*)'", f.read())
@@ -102,13 +106,10 @@
                     "shenfun.jacobi",
                     "shenfun.forms",
                     "shenfun.utilities",
                     "shenfun.io"
                    ],
           package_dir={"shenfun": "shenfun"},
           install_requires=["mpi4py-fft", "mpi4py", "cython", "numpy", "scipy"],
-          setup_requires=["numpy>=1.9",
-                          "cython>=0.25",
-                          "setuptools>=18.0"],
           ext_modules=get_extensions(),
           cmdclass={"build_ext": build_ext_subclass}
          )
```

### Comparing `shenfun-4.1.4/shenfun/__init__.py` & `shenfun-4.2.0/shenfun/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ``Shenfun`` has support for solving scalar and vector equations in curvilinear
 coordinates, like polar or spherical coordinates.
 
 """
 #pylint: disable=wildcard-import,no-name-in-module
 
-__version__ = '4.1.4'
+__version__ = '4.2.0'
 __author__ = 'Mikael Mortensen'
 
 import numpy as np
 from mpi4py import MPI
 from .config import config, dumpconfig
 from . import chebyshev
 from . import chebyshevu
```

### Comparing `shenfun-4.1.4/shenfun/bessel/bases.py` & `shenfun-4.2.0/shenfun/laguerre/bases.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import sympy as sp
 import numpy as np
-import scipy.special as sc
-from scipy.special import jv
+from numpy.polynomial import laguerre as lag
+from scipy.special import eval_laguerre
 from shenfun.matrixbase import SparseMatrix
+from shenfun.jacobi.recursions import n
 from shenfun.spectralbase import SpectralBase, getCompositeBase, getBCGeneric, BoundaryConditions
 
 #pylint: disable=method-hidden,no-else-return,not-callable,abstract-method,no-member,cyclic-import
 
 bases = ['Orthogonal',
-         'CompactDirichlet']
-bcbases = []
+         'CompactDirichlet',
+         'CompactNeumann',
+         'Generic']
+bcbases = ['BCGeneric']
 testbases = []
 __all__ = bases + bcbases
 
 xp = sp.Symbol('x', real=True)
 
 
 class Orthogonal(SpectralBase):
-    r"""Function space for a regular Bessel series
+    r"""Function space for a regular Laguerre series
 
-    The orthogonal basis is the Fourier-Bessel function of order 0
+    The orthogonal basis is the Laguerre function
 
     .. math::
 
-        \phi_k(x) = J_0(\lambda_k x/b), \quad k = 0, 1, \ldots, N-1,
+        \phi_k = La_k \exp(-x/2), \quad k = 0, 1, \ldots, N-1,
 
-    where :math:`\lambda_k` is the :math:`k`'th root of :math:`J_0(x)`
-    and the domain is :math:`x\in [0, b]`.
+    where :math:`La_k` is the :math:`k`'th Laguerre polynomial.
 
     Parameters
     ----------
     N : int
         Number of quadrature points
     padding_factor : float, optional
         Factor for padding backward transforms.
@@ -40,84 +42,155 @@
         Type of input data in real physical space. Will be overloaded when
         basis is part of a :class:`.TensorProductSpace`.
     coordinates: 2- or 3-tuple (coordinate, position vector (, sympy assumptions)), optional
         Map for curvilinear coordinatesystem, and parameters to :class:`~shenfun.coordinates.Coordinates`
 
     Note
     ----
-    We are using Fourier-Bessel functions and not the regular Bessel functions.
-
+    We are using Laguerre functions and not the regular Laguerre polynomials
+    as basis functions.
     """
     def __init__(self, N, dtype=float, padding_factor=1, dealias_direct=False,
-                 domain=(0, 1), coordinates=None, **kw):
-        SpectralBase.__init__(self, N, quad="BG", domain=domain, dtype=dtype,
+                 coordinates=None, **kw):
+        SpectralBase.__init__(self, N, quad="LG", domain=(0, sp.S.Infinity), dtype=dtype,
                               padding_factor=padding_factor, dealias_direct=dealias_direct,
                               coordinates=coordinates)
-        self.zeros = np.array([sc.jn_zeros(n, N) for n in range(N)])
         self.plan(int(N*padding_factor), 0, dtype, {})
 
     @staticmethod
     def family():
-        return 'bessel'
+        return 'laguerre'
 
     def reference_domain(self):
-        return (0, 1)
+        return (0, sp.S.Infinity)
+
+    def domain_factor(self):
+        return 1
 
     def points_and_weights(self, N=None, map_true_domain=False, weighted=True, **kw):
         if N is None:
             N = self.shape(False)
-        assert self.quad == "BG"
-        points = np.linspace(0, 1, self.N)
-        weights = None
-
-        if weighted:
-            pass
+        if self.quad == "LG":
+            points, weights = lag.laggauss(N)
+            if weighted:
+                weights *= np.exp(points)
         else:
             raise NotImplementedError
 
         return points, weights
 
     def vandermonde(self, x):
+        V = lag.lagvander(x, int(self.N*self.padding_factor)-1)
+        V *= np.exp(-x/2)[:, None]
+        return V
+
+    def evaluate_basis(self, x, i=0, output_array=None):
+        x = np.atleast_1d(x)
+        if output_array is None:
+            output_array = np.zeros(x.shape)
+        output_array = eval_laguerre(i, x, out=output_array)
+        output_array *= np.exp(-x/2)
+        return output_array
+
+    def evaluate_basis_derivative(self, x=None, i=0, k=0, output_array=None):
         if x is None:
             x = self.mesh(False, False)
-        V = np.zeros((x.shape[0], self.N))
-        for i in range(self.dim()):
-            f = self.orthogonal_basis_function(i, x=xp)
-            V[:, i] = sp.lambdify(xp, f)(x)
-        return V
+        if output_array is None:
+            output_array = np.zeros(x.shape)
+        x = np.atleast_1d(x)
+        basis = np.zeros(self.shape(True))
+        basis[i] = 1
+        basis = lag.Laguerre(basis)
+        if k == 1:
+            basis = basis.deriv(k)-0.5*basis
+        elif k == 2:
+            basis = basis.deriv(2)-basis.deriv(1)+0.25*basis
+        elif k == 3:
+            basis = basis.deriv(3)-1.5*basis.deriv(2)+0.75*basis.deriv(1)-basis/8
+        elif k == 4:
+            basis = basis.deriv(4)-2*basis.deriv(3)+1.5*basis.deriv(2)-0.5*basis.deriv(1)+basis/16
+        output_array[:] = basis(x)*np.exp(-x/2)
+        return output_array
 
     @staticmethod
     def bnd_values(k=0, **kw):
         if k == 0:
-            return (lambda i: int(i==0), None)
+            return (lambda i: 1, None)
         elif k == 1:
-            return (lambda i: 0, None)
+            return (lambda i: -i-sp.S.Half, None)
         raise NotImplementedError
 
     def stencil_matrix(self, N=None):
         N = self.N if N is None else N
         return SparseMatrix({0: 1}, (N, N))
 
+    def evaluate_basis_derivative_all(self, x=None, k=0, argument=0):
+        if x is None:
+            x = self.mesh(False, False)
+        V = lag.lagvander(x, int(self.N*self.padding_factor)-1)
+        M = V.shape[1]
+        if k == 1:
+            D = np.zeros((M, M))
+            D[:-1, :] = lag.lagder(np.eye(M), 1)
+            W = np.dot(V, D)
+            W -= 0.5*V
+            V = W*np.exp(-x/2)[:, np.newaxis]
+
+        elif k == 2:
+            D = np.zeros((M, M))
+            D[:-2, :] = lag.lagder(np.eye(M), 2)
+            D[:-1, :] -= lag.lagder(np.eye(M), 1)
+            W = np.dot(V, D)
+            W += 0.25*V
+            V = W*np.exp(-x/2)[:, np.newaxis]
+
+        elif k == 3:
+            D = np.zeros((M, M))
+            D[:-3, :] = lag.lagder(np.eye(M), 3)
+            D[:-2, :] -= lag.lagder(np.eye(M), 2)*3/2
+            D[:-1, :] += lag.lagder(np.eye(M), 1)*3/4
+            W = np.dot(V, D)
+            W += V/8
+            V = W*np.exp(-x/2)[:, np.newaxis]
+
+        elif k == 4:
+            D = np.zeros((M, M))
+            D[:-4, :] = lag.lagder(np.eye(M), 4)
+            D[:-3, :] -= lag.lagder(np.eye(M), 3)*2
+            D[:-2, :] += lag.lagder(np.eye(M), 2)*3/2
+            D[:-1, :] -= lag.lagder(np.eye(M), 1)/2
+            W = np.dot(V, D)
+            W += V/16
+            V = W*np.exp(-x/2)[:, np.newaxis]
+
+        elif k == 0:
+            V *= np.exp(-x/2)[:, np.newaxis]
+
+        else:
+            raise NotImplementedError
+
+        return V
+
     def eval(self, x, u, output_array=None):
         x = np.atleast_1d(x)
-        raise NotImplementedError
+        if output_array is None:
+            output_array = np.zeros(x.shape, dtype=self.dtype)
+        output_array[:] = lag.lagval(x, u)*np.exp(-x/2)
+        return output_array
 
-    def orthogonal_basis_function(self, i=0, x=xp):
-        lambdai = self.zeros[i, -1]
-        return sp.besselj(i, x*lambdai/self.domain[1])
+    def orthogonal_basis_function(self, i=0, x=sp.symbols('x')):
+        return sp.laguerre(i, x)*sp.exp(-x/2)
 
     def L2_norm_sq(self, i):
-        lambdai = self.zeros[i, -1]
-        return sp.Rational(1, 2)*sp.besselj(i+1, lambdai)**2
+        return 1
 
     def l2_norm_sq(self, i=None):
-        raise NotImplementedError
-
-    def weight(self, x=xp):
-        return x
+        if i is None:
+            return np.ones(self.N)
+        return 1
 
     @property
     def is_orthogonal(self):
         return True
 
     def get_orthogonal(self, **kwargs):
         d = dict(quad=self.quad,
@@ -127,24 +200,24 @@
                  dealias_direct=self.dealias_direct,
                  coordinates=self.coors.coordinates)
         d.update(kwargs)
         return Orthogonal(self.N, **d)
 
     @staticmethod
     def short_name():
-        return 'Jn'
+        return 'La'
 
-    #def get_bc_space(self):
-    #    if self._bc_space:
-    #        return self._bc_space
-    #    self._bc_space = BCGeneric(self.N, bc=self.bcs)
-    #    return self._bc_space
+    def get_bc_space(self):
+        if self._bc_space:
+            return self._bc_space
+        self._bc_space = BCGeneric(self.N, bc=self.bcs)
+        return self._bc_space
 
 CompositeBase = getCompositeBase(Orthogonal)
-#BCGeneric = getBCGeneric(CompositeBase)
+BCGeneric = getBCGeneric(CompositeBase)
 
 class CompactDirichlet(CompositeBase):
     r"""Laguerre function space for Dirichlet boundary conditions
 
     The basis :math:`\{\phi_k\}_{k=0}^{N-1}` is
 
     .. math::
@@ -193,119 +266,119 @@
     def boundary_condition():
         return 'Dirichlet'
 
     @staticmethod
     def short_name():
         return 'SD'
 
-#
-#class CompactNeumann(CompositeBase):
-#    r"""Laguerre function space for Dirichlet boundary conditions
-#
-#    The basis :math:`\{\phi_k\}_{k=0}^{N-1}` is
-#
-#    .. math::
-#        \phi_k &= (La_k - \frac{2k+1}{2k+3}La_{k+1})\exp(-x/2), \, k=0, 1, \ldots, N-2, \\
-#        \phi_{N-1} &= La_0\exp(-x/2),
-#
-#    such that
-#
-#    .. math::
-#        u(x) &= \sum_{k=0}^{N-1} \hat{u}_k \phi_k(x), \\
-#        u'(0) &= a
-#
-#    Parameters
-#    ----------
-#    N : int
-#        Number of quadrature points
-#    quad : str, optional
-#        Type of quadrature
-#
-#        - LG - Laguerre-Gauss
-#    bc : 1-tuple of number (a,)
-#        Boundary value a = u'(0)
-#    padding_factor : float, optional
-#        Factor for padding backward transforms.
-#    dealias_direct : bool, optional
-#        Set upper 1/3 of coefficients to zero before backward transform
-#    dtype : data-type, optional
-#        Type of input data in real physical space. Will be overloaded when
-#        basis is part of a :class:`.TensorProductSpace`.
-#    coordinates: 2- or 3-tuple (coordinate, position vector (, sympy assumptions)), optional
-#        Map for curvilinear coordinatesystem, and parameters to :class:`~shenfun.coordinates.Coordinates`
-#
-#    """
-#    def __init__(self, N, bc=(0,), dtype=float, padding_factor=1,
-#                 dealias_direct=False, coordinates=None, **kw):
-#        if isinstance(bc, (tuple, list)):
-#            assert len(bc) == 1
-#            bc = BoundaryConditions({'left': {'N': bc[0]}, 'right': {}}, domain=(0, np.inf))
-#        CompositeBase.__init__(self, N, dtype=dtype, quad='LG', padding_factor=padding_factor,
-#                               bc=bc, dealias_direct=dealias_direct, domain=(0, sp.S.Infinity),
-#                               coordinates=coordinates)
-#        self._stencil = {0: 1, 1: -(2*n+1)/(2*n+3)}
-#
-#    @staticmethod
-#    def boundary_condition():
-#        return 'Neumann'
-#
-#    @staticmethod
-#    def short_name():
-#        return 'CN'
-#
-#
-#class Generic(CompositeBase):
-#    r"""Function space for Laguerre space with any boundary conditions
-#
-#    Any combination of Dirichlet and Neumann is possible.
-#
-#    Parameters
-#    ----------
-#    N : int, optional
-#        Number of quadrature points
-#    quad : str, optional
-#        Type of quadrature
-#
-#        - LG - Laguerre-Gauss
-#
-#    bc : dict, optional
-#        The dictionary must have key 'left' (not 'right'), to describe boundary
-#        conditions on the left boundary. Specify Dirichlet with
-#
-#            {'left': {'D': a}}
-#
-#        for some value `a`, that will be neglected in the current
-#        function. Specify mixed Neumann and Dirichlet as
-#
-#            {'left': {'D': a, 'N': b}}
-#
-#        See :class:`~shenfun.spectralbase.BoundaryConditions`.
-#    domain : 2-tuple of floats, optional
-#        The computational domain
-#    dtype : data-type, optional
-#        Type of input data in real physical space. Will be overloaded when
-#        basis is part of a :class:`.TensorProductSpace`.
-#    padding_factor : float, optional
-#        Factor for padding backward transforms.
-#    dealias_direct : bool, optional
-#        Set upper 1/3 of coefficients to zero before backward transform
-#    coordinates: 2- or 3-tuple (coordinate, position vector (, sympy assumptions)), optional
-#        Map for curvilinear coordinatesystem, and parameters to :class:`~shenfun.coordinates.Coordinates`
-#
-#    """
-#    def __init__(self, N, quad="LG", bc={}, domain=(0, sp.S.Infinity), dtype=float,
-#                 padding_factor=1, dealias_direct=False, coordinates=None, **kw):
-#        from shenfun.utilities.findbasis import get_stencil_matrix
-#        self._stencil = get_stencil_matrix(bc, 'laguerre')
-#        if not isinstance(bc, BoundaryConditions):
-#            bc = BoundaryConditions(bc, domain=domain)
-#        CompositeBase.__init__(self, N, quad=quad, domain=domain, dtype=dtype, bc=bc,
-#                               padding_factor=padding_factor, dealias_direct=dealias_direct,
-#                               coordinates=coordinates)
-#
-#    @staticmethod
-#    def boundary_condition():
-#        return 'Generic'
-#
-#    @staticmethod
-#    def short_name():
-#        return 'GL'
+
+class CompactNeumann(CompositeBase):
+    r"""Laguerre function space for Dirichlet boundary conditions
+
+    The basis :math:`\{\phi_k\}_{k=0}^{N-1}` is
+
+    .. math::
+        \phi_k &= (La_k - \frac{2k+1}{2k+3}La_{k+1})\exp(-x/2), \, k=0, 1, \ldots, N-2, \\
+        \phi_{N-1} &= La_0\exp(-x/2),
+
+    such that
+
+    .. math::
+        u(x) &= \sum_{k=0}^{N-1} \hat{u}_k \phi_k(x), \\
+        u'(0) &= a
+
+    Parameters
+    ----------
+    N : int
+        Number of quadrature points
+    quad : str, optional
+        Type of quadrature
+
+        - LG - Laguerre-Gauss
+    bc : 1-tuple of number (a,)
+        Boundary value a = u'(0)
+    padding_factor : float, optional
+        Factor for padding backward transforms.
+    dealias_direct : bool, optional
+        Set upper 1/3 of coefficients to zero before backward transform
+    dtype : data-type, optional
+        Type of input data in real physical space. Will be overloaded when
+        basis is part of a :class:`.TensorProductSpace`.
+    coordinates: 2- or 3-tuple (coordinate, position vector (, sympy assumptions)), optional
+        Map for curvilinear coordinatesystem, and parameters to :class:`~shenfun.coordinates.Coordinates`
+
+    """
+    def __init__(self, N, bc=(0,), dtype=float, padding_factor=1,
+                 dealias_direct=False, coordinates=None, **kw):
+        if isinstance(bc, (tuple, list)):
+            assert len(bc) == 1
+            bc = BoundaryConditions({'left': {'N': bc[0]}, 'right': {}}, domain=(0, np.inf))
+        CompositeBase.__init__(self, N, dtype=dtype, quad='LG', padding_factor=padding_factor,
+                               bc=bc, dealias_direct=dealias_direct, domain=(0, sp.S.Infinity),
+                               coordinates=coordinates)
+        self._stencil = {0: 1, 1: -(2*n+1)/(2*n+3)}
+
+    @staticmethod
+    def boundary_condition():
+        return 'Neumann'
+
+    @staticmethod
+    def short_name():
+        return 'CN'
+
+
+class Generic(CompositeBase):
+    r"""Function space for Laguerre space with any boundary conditions
+
+    Any combination of Dirichlet and Neumann is possible.
+
+    Parameters
+    ----------
+    N : int, optional
+        Number of quadrature points
+    quad : str, optional
+        Type of quadrature
+
+        - LG - Laguerre-Gauss
+
+    bc : dict, optional
+        The dictionary must have key 'left' (not 'right'), to describe boundary
+        conditions on the left boundary. Specify Dirichlet with
+
+            {'left': {'D': a}}
+
+        for some value `a`, that will be neglected in the current
+        function. Specify mixed Neumann and Dirichlet as
+
+            {'left': {'D': a, 'N': b}}
+
+        See :class:`~shenfun.spectralbase.BoundaryConditions`.
+    domain : 2-tuple of floats, optional
+        The computational domain
+    dtype : data-type, optional
+        Type of input data in real physical space. Will be overloaded when
+        basis is part of a :class:`.TensorProductSpace`.
+    padding_factor : float, optional
+        Factor for padding backward transforms.
+    dealias_direct : bool, optional
+        Set upper 1/3 of coefficients to zero before backward transform
+    coordinates: 2- or 3-tuple (coordinate, position vector (, sympy assumptions)), optional
+        Map for curvilinear coordinatesystem, and parameters to :class:`~shenfun.coordinates.Coordinates`
+
+    """
+    def __init__(self, N, quad="LG", bc={}, domain=(0, sp.S.Infinity), dtype=float,
+                 padding_factor=1, dealias_direct=False, coordinates=None, **kw):
+        from shenfun.utilities.findbasis import get_stencil_matrix
+        self._stencil = get_stencil_matrix(bc, 'laguerre')
+        if not isinstance(bc, BoundaryConditions):
+            bc = BoundaryConditions(bc, domain=domain)
+        CompositeBase.__init__(self, N, quad=quad, domain=domain, dtype=dtype, bc=bc,
+                               padding_factor=padding_factor, dealias_direct=dealias_direct,
+                               coordinates=coordinates)
+
+    @staticmethod
+    def boundary_condition():
+        return 'Generic'
+
+    @staticmethod
+    def short_name():
+        return 'GL'
```

### Comparing `shenfun-4.1.4/shenfun/bessel/matrices.py` & `shenfun-4.2.0/shenfun/jacobi/matrices.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from shenfun.matrixbase import SpectralMatrix, SpectralMatDict
 from shenfun.spectralbase import get_norm_sq
 from . import bases
 
-CD = bases.CompactDirichlet
-J = bases.Orthogonal
+J  = bases.Orthogonal
 
 class BJJmat(SpectralMatrix):
     r"""Mass matrix :math:`B=(b_{kj}) \in \mathbb{R}^{M \times N}`, where
 
     .. math::
 
-        b_{kj}=(J_k(x \lambda_k), J_k(x \lambda_j))_w,
+        b_{kj}=(J_j, J_k)_w,
 
-    where the Bessel function :math:`J_k(x \lambda_k) \in` :class:`.bases.Orthogonal`,
-    and test and trial spaces have dimensions of M and N, respectively.
+    :math:`J_k \in` :class:`.jacobi.bases.Orthogonal` and test and trial spaces have
+    dimensions of M and N, respectively.
 
     """
-    def __init__(self, test, trial, scale=1, measure=1, assemble=None, kind=None, fixed_resolution=None):
-        assert isinstance(test[0], J)
-        assert isinstance(trial[0], J)
-        SpectralMatrix.__init__(self, test, trial, scale=scale, measure=measure, assemble=assemble, kind=kind, fixed_resolution=fixed_resolution)
-
     def assemble(self, method):
         test, trial = self.testfunction, self.trialfunction
+        assert isinstance(test[0], J)
+        assert isinstance(trial[0], J)
         return {0: get_norm_sq(test[0], trial[0], method)}
 
-
 mat = SpectralMatDict({
-    ((J, 0), (J, 0)): BJJmat
-    })
+    ((J,  0), (J,  0)): BJJmat,
+})
```

### Comparing `shenfun-4.1.4/shenfun/chebyshev/bases.py` & `shenfun-4.2.0/shenfun/chebyshev/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1930,14 +1930,28 @@
         self._stencil = {
             0: 1,
             2: -(4*n + 8)/(n + 5),
             4: 6*(n + 1)*(n + 4)/((n + 5)*(n + 6)),
             6: -4*(n + 1)*(n + 2)/((n + 5)*(n + 7)),
             8: (n + 1)*(n + 2)*(n + 3)/((n + 5)*(n + 6)*(n + 7))
         }
+        #self._stencil = {
+        #    0: 1/(8*sp.pi*(n + 1)*(n + 2)),
+        #    2: -1/(2*sp.pi*(n + 1)*(n + 5)),
+        #    4: 3*(n + 4)/(4*sp.pi*(n + 2)*(n + 5)*(n + 6)),
+        #    6: -1/(2*sp.pi*(n + 5)*(n + 7)),
+        #    8: (n + 3)/(8*sp.pi*(n + 5)*(n + 6)*(n + 7))
+        #}
+        #self._stencil = {
+        #    0: 1/(8*sp.pi*(n + 1)*(n + 2)*(n + 3)*(n + 4)),
+        #    2: -1/(2*sp.pi*(n + 1)*(n + 3)*(n + 4)*(n + 5)),
+        #    4: 3/(4*sp.pi*(n + 2)*(n + 3)*(n + 5)*(n + 6)),
+        #    6: -1/(2*sp.pi*(n + 3)*(n + 4)*(n + 5)*(n + 7)),
+        #    8: 1/(8*sp.pi*(n + 4)*(n + 5)*(n + 6)*(n + 7))
+        #}
 
     @staticmethod
     def boundary_condition():
         return '8th order'
 
     @staticmethod
     def short_name():
```

### Comparing `shenfun-4.1.4/shenfun/chebyshev/la.py` & `shenfun-4.2.0/shenfun/chebyshev/la.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/chebyshev/matrices.py` & `shenfun-4.2.0/shenfun/chebyshev/matrices.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/chebyshevu/bases.py` & `shenfun-4.2.0/shenfun/chebyshevu/bases.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/chebyshevu/matrices.py` & `shenfun-4.2.0/shenfun/chebyshevu/matrices.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/config.py` & `shenfun-4.2.0/shenfun/config.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/coordinates.py` & `shenfun-4.2.0/shenfun/coordinates.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/forms/arguments.py` & `shenfun-4.2.0/shenfun/forms/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from itertools import product
 from collections import defaultdict
 import copy
 from scipy.special import sph_harm, erf, airy, jn, gammaln
 import numpy as np
 import sympy as sp
 from shenfun.config import config
-from shenfun.optimization.cython import evaluate
+from shenfun.optimization import cython
 from shenfun.spectralbase import BoundaryConditions
 from mpi4py_fft import DistArray
 
 __all__ = ('Expr', 'BasisFunction', 'TestFunction', 'TrialFunction', 'Function',
            'Array', 'FunctionSpace')
 
 # Define some special functions required for spherical harmonics
@@ -771,18 +771,18 @@
 
                 bv = basis if basis.tensor_rank == 0 else basis[ind[base_j]]
                 work.fill(0)
                 if len(x) == 1:
                     work = np.dot(P, bv)
 
                 elif len(x) == 2:
-                    work = evaluate.evaluate_2D(work, bv, M, r2c, last_conj_index, sl)
+                    work = cython.evaluate.evaluate_2D(work, bv, M, r2c, last_conj_index, sl)
 
                 elif len(x) == 3:
-                    work = evaluate.evaluate_3D(work, bv, M, r2c, last_conj_index, sl)
+                    work = cython.evaluate.evaluate_3D(work, bv, M, r2c, last_conj_index, sl)
 
                 sc = self.scales()[vec][base_j]
                 if not hasattr(sc, 'free_symbols'):
                     sc = float(sc)
                 else:
                     sym0 = tuple(sc.free_symbols)
                     m = []
```

### Comparing `shenfun-4.1.4/shenfun/forms/inner.py` & `shenfun-4.2.0/shenfun/forms/inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,40 +233,47 @@
         result = 0.0
         for e0i, e1i in zip(expr0, expr1):
             result += inner(e0i, e1i)
         return result
 
     if isinstance(expr0, sp.Expr) or isinstance(expr1, sp.Expr):
         # Special linear form using sympy expression
+        expr_is_test = False
         if isinstance(expr0, sp.Expr):
-            assert isinstance(expr1, TestFunction)
+            if isinstance(expr1, TestFunction):
+                expr_is_test = True
             test = expr1
             trial = expr0
         else:
-            assert isinstance(expr0, TestFunction)
+            if isinstance(expr0, TestFunction):
+                expr_is_test = True
             test = expr0
             trial = expr1
 
-        if output_array is None:
-            output_array = Function(test.function_space())
+        if expr_is_test:
+            if output_array is None:
+                output_array = Function(test.function_space())
 
-        if assemble in ('exact', 'adaptive'):
-            output_array = scalar_product(test, trial, output_array, assemble=assemble)
+            if assemble in ('exact', 'adaptive'):
+                output_array = scalar_product(test, trial, output_array, assemble=assemble)
 
-        else: # quadrature
-            if fixed_resolution is not None:
-                from shenfun import comm
-                assert comm.Get_size() == 1
-                M = fixed_resolution
-                testM = test.function_space().get_refined(M)
-                outM = testM.scalar_product(Array(testM, buffer=trial), kind=kind)
-                output_array[test.function_space().slice()] = outM[test.function_space().slice()]
-            else:
-                output_array = test.function_space().scalar_product(Array(test.function_space(), buffer=trial), output_array, kind=kind)
-        return output_array
+            else: # quadrature
+                if fixed_resolution is not None:
+                    from shenfun import comm
+                    assert comm.Get_size() == 1
+                    M = fixed_resolution
+                    testM = test.function_space().get_refined(M)
+                    outM = testM.scalar_product(Array(testM, buffer=trial), kind=kind)
+                    output_array[test.function_space().slice()] = outM[test.function_space().slice()]
+                else:
+                    output_array = test.function_space().scalar_product(Array(test.function_space(), buffer=trial), output_array, kind=kind)
+            return output_array
+        else:
+            expr0 = test
+            expr1 = Function(test.function_space(), buffer=trial)
 
     assert np.all([hasattr(e, 'argument') for e in (expr0, expr1)])
     t0 = expr0.argument
     t1 = expr1.argument
     if t0 == 0:
         assert t1 in (1, 2)
         test = expr0
```

### Comparing `shenfun-4.1.4/shenfun/forms/operators.py` & `shenfun-4.2.0/shenfun/forms/operators.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/forms/project.py` & `shenfun-4.2.0/shenfun/forms/project.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/fourier/__init__.py` & `shenfun-4.2.0/shenfun/fourier/__init__.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/fourier/bases.py` & `shenfun-4.2.0/shenfun/fourier/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 where :math:`\overline{v}` is the complex conjugate of :math:`v`, and
 :math:`L` is the length of the (periodic) domain.
 """
 import sympy as sp
 import numpy as np
 from mpi4py_fft import fftw
 from shenfun.spectralbase import SpectralBase, Transform, islicedict, slicedict
-from shenfun.optimization.cython import convolve
+from shenfun.optimization import cython
 from shenfun.config import config
 
 bases = ['R2C', 'C2C']
 bcbases = []
 testbases = []
 __all__ = bases
 
@@ -466,15 +466,15 @@
             uv = self.forward(u2*u3, uv)
 
         else:
             if uv is None:
                 uv = np.zeros(N+1, dtype=u.dtype)
             Np = N if not N % 2 == 0 else N+1
             k1 = np.fft.fftfreq(Np, 1./Np).astype(int)
-            convolve.convolve_real_1D(u, v, uv, k1)
+            cython.convolve.convolve_real_1D(u, v, uv, k1)
 
         return uv
 
 
 class C2C(FourierBase):
     r"""Fourier function space for complex to complex transforms
 
@@ -632,10 +632,10 @@
         else:
 
             if uv is None:
                 uv = np.zeros(2*N, dtype=u.dtype)
 
             Np = N if not N % 2 == 0 else N+1
             k = np.fft.fftfreq(Np, 1./Np).astype(int)
-            convolve.convolve_1D(u, v, uv, k)
+            cython.convolve.convolve_1D(u, v, uv, k)
 
         return uv
```

### Comparing `shenfun-4.1.4/shenfun/fourier/matrices.py` & `shenfun-4.2.0/shenfun/fourier/matrices.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/hermite/bases.py` & `shenfun-4.2.0/shenfun/hermite/bases.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/hermite/matrices.py` & `shenfun-4.2.0/shenfun/hermite/matrices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from shenfun.matrixbase import SpectralMatrix, SpectralMatDict
-from shenfun.optimization.cython import Matvec
+from shenfun.optimization import cython
 from shenfun.la import TDMA
 from . import bases
 
 H = bases.Orthogonal
 
 
 class BHHmat(SpectralMatrix):
@@ -70,23 +70,23 @@
         return TDMA
 
     def matvec(self, v, c, format='cython', axis=0):
         N, M = self.shape
         c.fill(0)
         if format == 'cython' and v.ndim == 3:
             ld = self[-2]*np.ones(M-2)
-            Matvec.Tridiagonal_matvec3D_ptr(v, c, ld, self[0], ld, axis)
+            cython.Matvec.Tridiagonal_matvec3D_ptr(v, c, ld, self[0], ld, axis)
             self.scale_array(c, self.scale)
         elif format == 'cython' and v.ndim == 2:
             ld = self[-2]*np.ones(M-2)
-            Matvec.Tridiagonal_matvec2D_ptr(v, c, ld, self[0], ld, axis)
+            cython.Matvec.Tridiagonal_matvec2D_ptr(v, c, ld, self[0], ld, axis)
             self.scale_array(c, self.scale)
         elif format == 'cython' and v.ndim == 1:
             ld = self[-2]*np.ones(M-2)
-            Matvec.Tridiagonal_matvec(v, c, ld, self[0], ld)
+            cython.Matvec.Tridiagonal_matvec(v, c, ld, self[0], ld)
             self.scale_array(c, self.scale)
         elif format == 'self':
             if axis > 0:
                 v = np.moveaxis(v, axis, 0)
                 c = np.moveaxis(c, axis, 0)
             s = (slice(None),)+(np.newaxis,)*(v.ndim-1) # broadcasting
             c[:(N-2)] = self[2][s]*v[2:N]
```

### Comparing `shenfun-4.1.4/shenfun/io/__init__.py` & `shenfun-4.2.0/shenfun/io/__init__.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/io/generate_xdmf.py` & `shenfun-4.2.0/shenfun/io/generate_xdmf.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/jacobi/bases.py` & `shenfun-4.2.0/shenfun/jacobi/bases.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/jacobi/matrices.py` & `shenfun-4.2.0/shenfun/ultraspherical/matrices.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 from shenfun.matrixbase import SpectralMatrix, SpectralMatDict
 from shenfun.spectralbase import get_norm_sq
 from . import bases
 
-J  = bases.Orthogonal
+Q  = bases.Orthogonal
+CB = bases.CompositeBase
+CD = bases.CompactDirichlet
+CN = bases.CompactNeumann
+UD = bases.UpperDirichlet
+LD = bases.LowerDirichlet
+P1 = bases.Phi1
+P2 = bases.Phi2
+P3 = bases.Phi3
+P4 = bases.Phi4
+BCG = bases.BCGeneric
 
-class BJJmat(SpectralMatrix):
+
+class BQQmat(SpectralMatrix):
     r"""Mass matrix :math:`B=(b_{kj}) \in \mathbb{R}^{M \times N}`, where
 
     .. math::
 
-        b_{kj}=(J_j, J_k)_w,
+        b_{kj}=(Q_j, Q_k)_w,
 
-    :math:`J_k \in` :class:`.jacobi.bases.Orthogonal` and test and trial spaces have
-    dimensions of M and N, respectively.
+    :math:`Q_k \in` :class:`.ultraspherical.bases.Orthogonal` and test and
+    trial spaces have dimensions of M and N, respectively.
 
     """
     def assemble(self, method):
         test, trial = self.testfunction, self.trialfunction
-        assert isinstance(test[0], J)
-        assert isinstance(trial[0], J)
+        assert isinstance(test[0], Q)
+        assert isinstance(trial[0], Q)
         return {0: get_norm_sq(test[0], trial[0], method)}
 
+
 mat = SpectralMatDict({
-    ((J,  0), (J,  0)): BJJmat,
+    ((Q, 0), (Q, 0)): BQQmat,
 })
```

### Comparing `shenfun-4.1.4/shenfun/jacobi/recursions.py` & `shenfun-4.2.0/shenfun/jacobi/recursions.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/la.py` & `shenfun-4.2.0/shenfun/la.py`

 * *Files 0% similar despite different names*

```diff
@@ -1496,18 +1496,18 @@
         if len(daxes) == space.dimensions:
             # Only Fourier spaces, all diagonal
             assert len(daxes) == space.dimensions
             Ai = self.mat._Ai[0]
             gi = b.flatten()
             if isinstance(self._lu, dict):
                 for con in constraints:
-                    Ai, gi = self.apply_constraint(Ai, gi, np.sum(np.array(space.dims()[:con[0]])), 0, con)
+                    Ai, gi = self.apply_constraint(Ai, gi, int(np.sum(np.array(space.dims()[:con[0]]))), 0, con)
             else:
                 for con in constraints:
-                    _, gi = self.apply_constraint(None, gi, np.sum(np.array(space.dims()[:con[0]])), 0, con)
+                    _, gi = self.apply_constraint(None, gi, int(np.sum(np.array(space.dims()[:con[0]]))), 0, con)
             lu = sp.linalg.splu(Ai, permc_spec=config['matrix']['block']['permc_spec'])
             self._lu = lu
             u[:] = lu.solve(gi).reshape(u.shape)
 
         else:
             sl, dims = space._get_ndiag_slices_and_dims()
             gi = np.zeros(dims[-1], dtype=b.dtype)
```

### Comparing `shenfun-4.1.4/shenfun/laguerre/matrices.py` & `shenfun-4.2.0/shenfun/laguerre/matrices.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/legendre/bases.py` & `shenfun-4.2.0/shenfun/legendre/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 from shenfun.config import config
 from shenfun.spectralbase import Transform, getCompositeBase, getBCGeneric, \
     BoundaryConditions, islicedict, slicedict
 from shenfun.matrixbase import SparseMatrix
 from shenfun.utilities import n
 from shenfun.jacobi import JacobiBase
 from .lobatto import legendre_lobatto_nodes_and_weights
-from . import fastgl
 
 
 bases = ['Orthogonal',
          'ShenDirichlet',
          'ShenNeumann',
          'ShenBiharmonic',
          'ShenBiPolar',
@@ -116,14 +115,15 @@
         self.plan(int(padding_factor*N), 0, dtype, {})
 
     @staticmethod
     def family():
         return 'legendre'
 
     def points_and_weights(self, N=None, map_true_domain=False, weighted=True, **kw):
+        from . import fastgl
         if N is None:
             N = self.shape(False)
         if self.quad == "LG":
             points, weights = fastgl.leggauss(N)
 
         elif self.quad == "GL":
             points, weights = legendre_lobatto_nodes_and_weights(N)
```

### Comparing `shenfun-4.1.4/shenfun/legendre/dlt.py` & `shenfun-4.2.0/shenfun/legendre/dlt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from scipy.special import gammaln
 import numpy as np
 from numpy.polynomial import chebyshev as n_cheb
 from mpi4py import MPI
 from mpi4py_fft import fftw
 from mpi4py_fft.fftw.utilities import FFTW_MEASURE, FFTW_PRESERVE_INPUT
 from shenfun.optimization import runtimeoptimizer
-from shenfun.optimization.cython import Leg2Cheb, Cheb2Leg, Lambda
+from shenfun.optimization import cython
 from shenfun.spectralbase import islicedict, slicedict
-from shenfun.forms.arguments import FunctionSpace
-from . import fastgl
 
 __all__ = ['DLT', 'leg2cheb', 'cheb2leg', 'Leg2chebHaleTownsend',
            'Leg2Cheb', 'Cheb2Leg', 'FMMLeg2Cheb', 'FMMCheb2Leg']
 
+Leg2Cheb = getattr(cython, 'Leg2Cheb', None)
+Cheb2Leg = getattr(cython, 'Cheb2Leg', None)
+Lambda = getattr(cython, 'Lambda', None)
 
 class DLT:
     r"""Discrete Legendre Transform
 
     A class for performing fast FFT-based discrete Legendre transforms, both
     forwards and backwards. Based on::
 
@@ -93,14 +94,15 @@
     >>> u[:] = 1
     >>> np.alltrue(np.abs(u - u.backward().forward()) < 1e-12)
     True
 
     """
     def __init__(self, input_array, s=None, axes=(-1,), threads=1, kind='backward',
                  flags=(FFTW_MEASURE, FFTW_PRESERVE_INPUT), output_array=None):
+        from . import fastgl
         if isinstance(axes, tuple):
             assert len(axes) == 1
             axis = axes[-1]
         elif isinstance(axes, int):
             axis = axes
         self.axis = axis
         assert kind in ('forward', 'scalar product', 'backward')
```

### Comparing `shenfun-4.1.4/shenfun/legendre/fastgl/fastgl_wrap.pyx` & `shenfun-4.2.0/shenfun/legendre/fastgl/fastgl_wrap.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # distutils: language = c++
 #cython: boundscheck=False
 #cython: wraparound=False
-#cython: language_level=3
+#cython: language_level=3str
 from . cimport fastgl_wrap
 
 import numpy as np
 
 def getGLPair(int N, int k):
     """Return point and weight k for N-point Gauss-Legendre rule
```

### Comparing `shenfun-4.1.4/shenfun/legendre/la.py` & `shenfun-4.2.0/shenfun/legendre/la.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/legendre/lobatto.py` & `shenfun-4.2.0/shenfun/legendre/lobatto.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/legendre/matrices.py` & `shenfun-4.2.0/shenfun/legendre/matrices.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/matrixbase.py` & `shenfun-4.2.0/shenfun/matrixbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,15 @@
             if kind is not None:
                 # Specified method of assembly, mainly for testing
                 if kind == 'implemented':
                     d = self.assemble(assemble)
                     _assembly_method += '_implemented'
                 elif kind == 'stencil':
                     assert sp.sympify(measure).is_polynomial(), 'Cannot use `stencil` with non-polynomial coefficients'
-                    if test[0].short_name() in ('P1', 'P2', 'P3', 'P4'):
+                    if test[0].short_name() in ('P1', 'P2', 'P3', 'P4') and test[0].N != trial[0].N:
                         d = assemble_phi(test, trial, measure)
                         _assembly_method += '_phi'
                     else:
                         d = assemble_stencil(test, trial, measure)
                         _assembly_method += '_stencil'
                 elif kind == 'vandermonde':
                     d = _get_matrix(test, trial, measure, assemble='quadrature', fixed_resolution=fixed_resolution)
@@ -1863,36 +1863,33 @@
         v = test[0].evaluate_basis_derivative_all(x=x, k=test[1])[:, :K0]
         V = np.dot(np.conj(v.T)*ws[np.newaxis, :], u)
 
     else: # exact or adaptive
 
         x = sp.Symbol('x', real=True)
 
-        if not measure == 1:
-            if isinstance(measure, sp.Expr):
-                s = measure.free_symbols
-                assert len(s) == 1
-                x = s.pop()
-                xm = test[0].map_true_domain(x)
-                if test[0].family() == 'chebyshev':
-                    measure = measure.subs(x, sp.cos(xm))
-                else:
-                    measure = measure.subs(x, xm)
-            else:
-                assert isinstance(measure, Number)
-
         # Exact integration is much more expensive than quadrature and
         # as such we use quadrature first simply to get the sparsity pattern.
         try:
             R = _get_matrix(test, trial, measure=measure, assemble='quadrature')
         except:
             R = {k: None for k in np.arange(-test[0].dim(), test[0].dim()+1)}
+
         V = np.zeros((K0, K1), dtype=test[0].forward.output_array.dtype)
-        if test[0].family() == 'chebyshev':
+        if test[0].family() == 'chebyshev' and assemble == 'exact':
             # Transform integral using x=cos(theta)
+            if not measure == 1:
+                if isinstance(measure, sp.Expr):
+                    s = measure.free_symbols
+                    assert len(s) == 1
+                    x = s.pop()
+                    xm = test[0].map_true_domain(x)
+                    measure = measure.subs(x, sp.cos(xm))
+                else:
+                    assert isinstance(measure, Number)
             assert test[1] == 0
             S0 = test[0].stencil_matrix().diags('csr')
             S1 = trial[0].stencil_matrix().diags('csr')
             for i in range(test[0].slice().start, test[0].slice().stop):
                 M0 = S0.getrow(i)
                 pi = sp.S(0)
                 for ind, d in zip(M0.indices, M0.data):
@@ -1906,41 +1903,53 @@
                     for ind, d in zip(M1.indices, M1.data):
                         pj += d*sp.cos(ind*x)
 
                     # df(theta)/dx = df/dtheta*dtheta/dx - apply recursively
                     for _ in range(trial[1]):
                         pj = -pj.diff(x, 1)/sp.sin(x)
 
-                    integrand = measure*pi*pj
-                    if assemble == 'exact':
-                        V[i, j] = sp.integrate(integrand, (x, 0, sp.pi))
-                    elif assemble == 'adaptive':
-                        if isinstance(integrand, Number):
-                            V[i, j] = integrand*np.pi
-                        else:
-                            V[i, j] = quad(sp.lambdify(x, integrand), 0, np.pi)[0]
+                    V[i, j] = sp.integrate(measure*pi*pj, (x, 0, sp.pi))
 
         else:
-            measure *= test[0].weight() # Weight of weighted space (in reference domain)
+            if not measure == 1:
+                if isinstance(measure, sp.Expr):
+                    s = measure.free_symbols
+                    assert len(s) == 1
+                    x = s.pop()
+                    xm = test[0].map_true_domain(x)
+                    measure = measure.subs(x, xm)
+                else:
+                    assert isinstance(measure, Number)
+
+            cheb = test[0].family() == 'chebyshev'
+            if cheb: # use adaptive quadrature with weight incorporated
+                w = {'weight': 'alg',
+                     'wvar': (-0.5, -0.5)}
+            else:
+                w = {}
+                measure *= test[0].weight() # Weight of weighted space (in reference domain)
             domain = test[0].reference_domain()
             for i in range(test[0].slice().start, test[0].slice().stop):
                 pi = np.conj(test[0].basis_function(i, x=x))
                 for jq in R.keys():
                     j = i+jq
                     if j < 0 or j >= K1:
                         continue
                     pj = trial[0].basis_function(j, x=x)
                     integrand = measure*pi.diff(x, test[1])*pj.diff(x, trial[1])
                     if assemble == 'exact':
                         V[i, j] = integrate_sympy(integrand, (x, domain[0], domain[1]))
                     elif assemble == 'adaptive':
                         if isinstance(integrand, Number):
-                            V[i, j] = integrand*float(domain[1]-domain[0])
+                            if cheb:
+                                V[i, j] = integrand*np.pi
+                            else:
+                                V[i, j] = integrand*float(domain[1]-domain[0])
                         else:
-                            V[i, j] = quad(sp.lambdify(x, integrand), float(domain[0]), float(domain[1]))[0]
+                            V[i, j] = quad(sp.lambdify(x, integrand), float(domain[0]), float(domain[1]), **w)[0]
 
     if V.dtype.char in 'FDG':
         ni = np.linalg.norm(V.imag)
         if ni == 0:
             V = V.real.copy()
         elif np.linalg.norm(V.real) / ni > 1e14:
             V = V.real.copy()
@@ -2064,14 +2073,15 @@
     k = (test[0].N-test[0].dim())//2
     l = k-trial[1]
     assert l >= 0
     D = sp.S(0)
     for dv in split(measure, expand=True):
         sc = dv['coeff']
         msi = dv['x']
+        assert sp.sympify(msi).is_polynomial()
         qi = sp.degree(msi)
         Ax = Lmat(k, qi, l, test[0].dim(), trial[0].N, alpha, beta, gn)
         D = D + sc*Ax
     if trial[0].is_orthogonal:
         d = extract_diagonal_matrix(D, lowerband=q-k+l, upperband=q+k+l)
     else:
         K = trial[0].stencil_matrix()
@@ -2097,19 +2107,19 @@
     l = k-trial[1]
     assert l >= 0
     D = sp.S(0)
     if k <= N:
         for dv in split(measure, expand=True):
             sc = dv['coeff']
             msi = dv['x']
+            assert sp.sympify(msi).is_polynomial()
             qi = sp.degree(msi)
             Ax = Lmat(k, qi, l, M, N, alpha, beta, gn)
             D = D + sc*Ax
     if D is sp.S.Zero:
-        scale = 0
         d = {0: 1}
     else:
         K = trial[0].stencil_matrix()
         d = extract_diagonal_matrix(D*extract_diagonal_matrix(K).diags('csr').T, lowerband=N+q, upperband=N)
         d = d._storage
     return d
```

### Comparing `shenfun-4.1.4/shenfun/optimization/__init__.py` & `shenfun-4.2.0/shenfun/optimization/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 module we place optimized functions that are to be used instead of default
 Python methods. Some methods are implemented solely in Cython and only called
 from within the regular Python modules.
 
 """
 import importlib
 from functools import wraps
-from . import cython
 from shenfun.config import config
 
 try:
-    from . import numba
+    from . import cython
 except ModuleNotFoundError:
-    numba = None
+    cython = None
+#try:
+from . import numba
+#except ModuleNotFoundError:
+#    numba = None
 
 
 """
 
 runtimeoptimizer
 
 A decorator that chooses optimized function at runtime
```

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/Cheb.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/Cheb.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/Matvec.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/Matvec.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/__init__.py` & `shenfun-4.2.0/shenfun/optimization/cython/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 from .outer import outer2D, outer3D
 from .applymask import apply_mask
 from .Cheb import chebval
 from .transforms import evaluate_expansion_all, scalar_product, leg2cheb, cheb2leg, \
     restricted_product, FMMcheb, FMMdirect1, FMMdirect2, FMMdirect3, FMMdirect4, \
     _leg2cheb, _cheb2leg, FMMcheb, Lambda
 from .leg2chebm import Leg2Cheb, Cheb2Leg
+from .evaluate import evaluate_2D, evaluate_3D, evaluate_lm_2D, evaluate_lm_3D
+from .convolve import convolve_1D, convolve_real_1D
```

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/applymask.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/applymask.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/convolve.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/convolve.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/cross.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/cross.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/evaluate.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/evaluate.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/la.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/la.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/leg2chebm.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/leg2chebm.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,31 @@
 cimport cython
 import cython
 from libc.stdlib cimport malloc, free
 from copy import copy
 from numpy.polynomial import chebyshev as n_cheb
 from .transforms import FMMdirect1, FMMcheb, FMMdirect2, FMMdirect3, \
     FMMdirect4, _leg2cheb, _cheb2leg, _Lambda
-from .transforms cimport get_number_of_blocks
+#from .transforms cimport get_number_of_blocks
 
 np.import_array()
 
+cdef int get_number_of_blocks(int level, long* D, int N):
+    cdef:
+        int s = 1
+        int nd = 1
+        int i, j
+    if level > 0:
+        for i in range(level):
+            nd = 1
+            for j in range(i+1):
+                nd *= D[level-j-1]
+            s += nd
+    return s
+
 cdef class FMMLevel:
     cdef public int N
     cdef public int Nn
     cdef public int diags
     cdef public int L
     cdef public int s
     cdef public int maxs
```

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/outer.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/outer.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/cython/transforms.pyx` & `shenfun-4.2.0/shenfun/optimization/cython/transforms.pyx`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/__init__.py` & `shenfun-4.2.0/shenfun/optimization/numba/__init__.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/biharmonic.py` & `shenfun-4.2.0/shenfun/optimization/numba/biharmonic.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/chebyshev.py` & `shenfun-4.2.0/shenfun/optimization/numba/chebyshev.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/diagma.py` & `shenfun-4.2.0/shenfun/optimization/numba/diagma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/fdma.py` & `shenfun-4.2.0/shenfun/optimization/numba/fdma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/helmholtz.py` & `shenfun-4.2.0/shenfun/optimization/numba/helmholtz.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/heptadma.py` & `shenfun-4.2.0/shenfun/optimization/numba/heptadma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/la.py` & `shenfun-4.2.0/shenfun/optimization/numba/la.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/pdma.py` & `shenfun-4.2.0/shenfun/optimization/numba/pdma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/tdma.py` & `shenfun-4.2.0/shenfun/optimization/numba/tdma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/threedma.py` & `shenfun-4.2.0/shenfun/optimization/numba/threedma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/transforms.py` & `shenfun-4.2.0/shenfun/optimization/numba/transforms.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/optimization/numba/twodma.py` & `shenfun-4.2.0/shenfun/optimization/numba/twodma.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/spectralbase.py` & `shenfun-4.2.0/shenfun/spectralbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1854,14 +1854,15 @@
 
     domain : 2-tuple of numbers, optional
         The domain, if different than (-1, 1).
 
     """
     def __init__(self, bc, domain=None):
         bcs = {'left': {}, 'right': {}}
+
         if isinstance(bc, str):
             # Boundary conditions given in single string with boundary conditions separated by &&
             for bci in bc.split('&&'):
                 # Check for Dirichlet
                 x = re.search(r"u\((.*)\)=(.*)", bci)
                 if x:
                     if np.abs(float(x.group(1))-domain[0]) < 1e-8:
@@ -1948,31 +1949,32 @@
         elif isinstance(bc, dict):
             if isinstance(bc.get("left", {}) or bc.get("right", {}), (tuple, list)):
                 # old form {'left': [('D', 0), ('N', 0)], 'right': [('D', 0)]}
                 bc = {k.lower(): list(v) if isinstance(v[0], (tuple, list)) else [v] for k, v in bc.items()}
                 for key, val in bc.items():
                     bcs[key] = {v[0]: copy.deepcopy(v[1]) for v in val}
             else:
-                bcs.update(copy.deepcopy(bc))
+                #bcs.update(copy.deepcopy(bc))
+                bcs.update(bc)
 
         # Take care of non-standard domain size
         df = 1
         if domain is not None:
             assert isinstance(domain, (tuple, list))
             if np.isfinite(float(domain[0]*domain[1])):
                 df = 2/float(domain[1]-domain[0])
 
         for key, val in bcs.items():
             for bc, v in val.items():
                 if bc == 'N':
-                    bcs[key][bc] = bcs[key][bc]/df
+                    val[bc] /= df
                 elif bc == 'N2':
-                    bcs[key][bc] = bcs[key][bc]/df**2
+                    val[bc] /= df**2
                 elif bc == 'N3':
-                    bcs[key][bc] = bcs[key][bc]/df**3
+                    val[bc] /= df**3
         dict.__init__(self, bcs)
 
     def orderednames(self):
         return ['L'+bci for bci in sorted(self['left'].keys())] + ['R'+bci for bci in sorted(self['right'].keys())]
 
     def orderedvals(self):
         ls = []
@@ -2097,14 +2099,40 @@
         return np.array(self.slice())
 
     def _get_ndiag_slices_and_dims(self, j=()):
         sl = self._get_ndiag_slices(j)
         dims = self._get_ndiag_cum_dofs()
         return sl, dims
 
+    def __len__(self):
+        return len(self.bases)
+
+    def get_dealiased(self, padding_factor=1.5, dealias_direct=False):
+        """Return space (otherwise as self) to be used for dealiasing
+
+        Parameters
+        ----------
+        padding_factor : number or tuple, optional
+            Scale the number of quadrature points in self with this number, or
+            tuple of numbers, one for each dimension.
+        dealias_direct : bool, optional
+            Used only if ``padding_factor=1``. Sets the 1/3 highest frequencies
+            to zeros.
+        """
+        if padding_factor == 1 and dealias_direct is False:
+            return self
+        if isinstance(padding_factor, Number):
+            padding_factor = (padding_factor,)*len(self)
+        elif isinstance(padding_factor, (tuple, list, np.ndarray)):
+            assert len(padding_factor) == len(self)
+        padded_bases = [base.get_dealiased(padding_factor=padding_factor[i],
+                                           dealias_direct=dealias_direct)
+                        for i, base in enumerate(self.bases)]
+        return MixedFunctionSpace(padded_bases)
+
 class VectorBasisTransform:
 
     __slots__ = ('_transforms',)
 
     def __init__(self, transforms):
         self._transforms = []
         for transform in transforms:
```

### Comparing `shenfun-4.1.4/shenfun/tensorproductspace.py` & `shenfun-4.2.0/shenfun/tensorproductspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mpi4py_fft.mpifft import Transform, PFFT
 from mpi4py_fft.pencil import Subcomm, Pencil
 from mpi4py import MPI
 from shenfun import config
 from shenfun.fourier.bases import R2C, C2C
 from shenfun.utilities import apply_mask
 from shenfun.forms.arguments import Function, Array
-from shenfun.optimization.cython import evaluate
+from shenfun.optimization import cython
 from shenfun.spectralbase import slicedict, islicedict, SpectralBase
 from shenfun.coordinates import Coordinates
 
 comm = MPI.COMM_WORLD
 
 __all__ = ('TensorProductSpace', 'VectorSpace', 'TensorSpace',
            'CompositeSpace', 'Convolve')
@@ -460,15 +460,15 @@
                 self.pencil, self)
 
         else:
             self.configure_backwards(backward_from_pencil, dtype, kw)
 
         for i, base in enumerate(self.bases):
             base.axis = i
-            if base.has_nonhomogeneous_bcs:
+            if isinstance(base.bc, BoundaryValues):
                 base.bc.set_tensor_bcs(base, self)
 
     def configure_backwards(self, pencil, dtype, kw):
         """Configure transforms starting from spectral space
 
         Parameters
         ----------
@@ -795,18 +795,18 @@
                 else:
                     last_conj_index = M
                 sl = self.local_slice()[axis].start
             x.append(base.map_reference_domain(points[axis]))
             w.append(base.wavenumbers(bcast=False)[self.local_slice()[axis]].astype(float))
 
         if len(self) == 2:
-            output_array = evaluate.evaluate_lm_2D(list(self.bases), output_array, coefficients, x[0], x[1], w[0], w[1], r2c, last_conj_index, sl)
+            output_array = cython.evaluate.evaluate_lm_2D(list(self.bases), output_array, coefficients, x[0], x[1], w[0], w[1], r2c, last_conj_index, sl)
 
         elif len(self) == 3:
-            output_array = evaluate.evaluate_lm_3D(list(self.bases), output_array, coefficients, x[0], x[1], x[2], w[0], w[1], w[2], r2c, last_conj_index, sl)
+            output_array = cython.evaluate.evaluate_lm_3D(list(self.bases), output_array, coefficients, x[0], x[1], x[2], w[0], w[1], w[2], r2c, last_conj_index, sl)
 
         output_array = np.atleast_1d(output_array)
         output_array = comm.allreduce(output_array)
         return output_array
 
     def _eval_cython(self, points, coefficients, output_array):
         """Evaluate Function at points, given expansion coefficients
@@ -833,18 +833,18 @@
                 M = base.N//2+1
                 if base.N % 2 == 0:
                     last_conj_index = M-1
                 else:
                     last_conj_index = M
                 sl = self.local_slice()[axis].start
         if len(self) == 2:
-            output_array = evaluate.evaluate_2D(output_array, coefficients, P, r2c, last_conj_index, sl)
+            output_array = cython.evaluate.evaluate_2D(output_array, coefficients, P, r2c, last_conj_index, sl)
 
         elif len(self) == 3:
-            output_array = evaluate.evaluate_3D(output_array, coefficients, P, r2c, last_conj_index, sl)
+            output_array = cython.evaluate.evaluate_3D(output_array, coefficients, P, r2c, last_conj_index, sl)
 
         output_array = np.atleast_1d(output_array)
         output_array = comm.allreduce(output_array)
         return output_array
 
     def wavenumbers(self, scaled=False, eliminate_highest_freq=False):
         """Return list of wavenumbers
@@ -1826,34 +1826,43 @@
 
 class BoundaryValues:
     """Class for setting nonhomogeneous boundary conditions inside a multi-
     dimensional :class:`.TensorProductSpace`.
 
     Parameters
     ----------
-    T : :class:`.TensorProductSpace`
+    T : :class:`.SpectralBase`
     bc : :class:`.BoundaryConditions`
     """
     # pylint: disable=protected-access, redefined-outer-name, dangerous-default-value, unsubscriptable-object
 
     def __init__(self, T, bc):
         self.base = T
         self.tensorproductspace = None
         self.bc = bc
         self.bcs = bc.orderedvals()       # Processed bc
         self.bcs_final = bc.orderedvals() # Data. May differ from bcs only for TensorProductSpaces
         self.axis = 0
         self.bc_time = 0
 
-    def update(self, time=None):
+    def update(self, time=None, update_tensor=False):
+        """Update boundary values
+
+        Parameters
+        ----------
+        time : number
+            For boundary condition depending on time. Update with new time.
+        update_tensor : bool
+            Whether or not to update tensor if inhomogeneous 1D space is part
+            of a tensorproductspace
+        """
         from shenfun.forms.project import Project
-        tt = sp.symbols('t', real=True)
         bcs = self.bc.orderedvals()
-        update_tensor = False
         if self.has_nonhomogeneous_bcs:
+            tt = sp.symbols('t', real=True)
             for i, bci in enumerate(bcs):
                 if isinstance(bci, Project):
                     bci()
                     update_tensor = True
                 elif isinstance(bci, sp.Expr) and time is not None:
                     if tt in bci.free_symbols:
                         self.bc_time = time
@@ -2083,17 +2092,20 @@
             for i in range(M):
                 u[self.base.si[-(M)+i]] = self.bcs_final[i]
         else:
             for i in range(M):
                 u[self.base.si[-(M)+i]] = self.bcs[i]
 
     def has_nonhomogeneous_bcs(self):
+        from shenfun.forms.project import Project
         for bc in self.bc.orderedvals():
             if isinstance(bc, Number):
                 if not bc == 0:
                     return True
+            elif isinstance(bc, Project):
+                return True
             elif isinstance(bc, np.ndarray):
                 if not np.all(bc == 0):
                     return True
             elif isinstance(bc, sp.Expr):
                 return True
         return False
```

### Comparing `shenfun-4.1.4/shenfun/ultraspherical/bases.py` & `shenfun-4.2.0/shenfun/ultraspherical/bases.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/utilities/__init__.py` & `shenfun-4.2.0/shenfun/utilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 except ImportError:
     from collections import MutableMapping
 from collections import defaultdict
 import numpy as np
 import sympy as sp
 from scipy.fftpack import dct
 from scipy.integrate import quad
-from shenfun.optimization import runtimeoptimizer
-from shenfun.optimization.cython import Lambda
+from shenfun.optimization import runtimeoptimizer, cython
 from shenfun.config import config
 from .findbasis import get_bc_basis, get_stencil_matrix, n
 
 __all__ = ['dx', 'clenshaw_curtis1D', 'CachedArrayDict', 'surf3D',
            'wrap_periodic', 'outer', 'dot', 'apply_mask', 'integrate_sympy',
            'mayavi_show', 'quiver3D', 'get_bc_basis', 'get_stencil_matrix',
            'scalar_product', 'n', 'cross', 'reset_profile', 'Lambda']
 
+Lambda = getattr(cython, 'Lambda', None)
+
 def dx(u, weighted=False):
     r"""Compute integral of u over domain
 
     .. math::
 
         \int_{\Omega} u dx
 
@@ -720,25 +721,25 @@
 
     if T.is_composite_space:
         for vi, xi in zip(v, output_array):
             xi = scalar_product(vi, f, xi)
         return output_array
 
     x = sp.Symbol('x', real=True)
+    cheb = T.family() == 'chebyshev'
+
     if not isinstance(f, Number):
         s = f.free_symbols
         assert len(s) == 1
         x = s.pop()
-        xm = T.map_true_domain(x)
-        if T.family() == 'chebyshev':
-            f = f.subs(x, sp.cos(xm))
-        else:
-            f = f.subs(x, xm)
+        f = T.map_expression_true_domain(f, x=x)
+        if cheb:
+            f = f.subs(x, sp.cos(x))
 
-    if T.family() == 'chebyshev':
+    if cheb:
         S = T.stencil_matrix().diags('csr')
         for i in range(T.slice().start, T.slice().stop):
             M = S.getrow(i)
             integrand = sp.S(0)
             for ind, d in zip(M.indices, M.data):
                 integrand += d*sp.cos(ind*x)
             integrand = f*integrand
@@ -754,13 +755,16 @@
         f *= T.weight()
         for i in range(T.slice().start, T.slice().stop):
             integrand = f*sp.conjugate(T.basis_function(i, x=x))
             if assemble == 'exact':
                 output_array[i] = sp.integrate(integrand, (x, (domain[0], domain[1])))
             elif assemble == 'adaptive':
                 if len(integrand.free_symbols) == 0:
-                    output_array[i] = integrand*float(domain[1]-domain[0])
+                    if cheb:
+                        output_array[i] = integrand*np.pi
+                    else:
+                        output_array[i] = integrand*float(domain[1]-domain[0])
                 else:
                     output_array[i] = quad(sp.lambdify(x, integrand), float(domain[0]), float(domain[1]))[0]
     if T.domain_factor() != 1:
         output_array /= float(T.domain_factor())
     return output_array
```

### Comparing `shenfun-4.1.4/shenfun/utilities/findbasis.py` & `shenfun-4.2.0/shenfun/utilities/findbasis.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun/utilities/integrators.py` & `shenfun-4.2.0/shenfun/utilities/integrators.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import types
 import numpy as np
 from shenfun import Function, TPMatrix, TrialFunction, TestFunction,\
     inner, la, Expr, CompositeSpace, BlockMatrix, SparseMatrix, \
     get_simplified_tpmatrices, ScipyMatrix, Inner, SpectralMatrix
 
 __all__ = ('IRK3', 'BackwardEuler', 'RK4', 'ETDRK4', 'ETD',
-           'IMEXRK3', 'IMEXRK111', 'IMEXRK222', 'IMEXRK443')
+           'IMEXRK3', 'IMEXRK011', 'IMEXRK111', 'IMEXRK222', 'IMEXRK443')
 
 #pylint: disable=unused-variable
 
 class IntegratorBase:
     """Abstract base class for integrators
 
     Parameters
@@ -812,14 +812,31 @@
             self.T.mask_nyquist(self.rhs, self.mask)
         return self.rhs
 
     def solve_step(self, rk=0):
         # only one solver since the diagonal of a is constant
         return self.solvers[0](self.rhs, self.u_)
 
+class IMEXRK011(PDEIMEXRK):
+
+    @classmethod
+    def steps(cls):
+        return 1
+
+    def stages(self):
+        a = np.array([
+            [0, 0],
+            [0, 0]])
+        b = np.array([
+            [0, 0],
+            [1, 0]])
+        c = (1, 0)
+        return a, b, c
+
+
 class IMEXRK111(PDEIMEXRK):
 
     @classmethod
     def steps(cls):
         return 1
 
     def stages(self):
```

### Comparing `shenfun-4.1.4/shenfun/utilities/lagrangian_particles.py` & `shenfun-4.2.0/shenfun/utilities/lagrangian_particles.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/shenfun.egg-info/PKG-INFO` & `shenfun-4.2.0/shenfun.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 Metadata-Version: 2.1
 Name: shenfun
-Version: 4.1.4
+Version: 4.2.0
 Summary: Shenfun -- Automated Spectral-Galerkin framework
 Home-page: https://github.com/spectralDNS/shenfun
 Author: Mikael Mortensen
 Author-email: mikaem@math.uio.no
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: mpi4py-fft
+Requires-Dist: mpi4py
+Requires-Dist: cython
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 Shenfun
 =======
 .. image:: https://app.codacy.com/project/badge/Grade/bd772b3ca7134651a9225d8051db8c41
     :target: https://www.codacy.com/gh/spectralDNS/shenfun/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=spectralDNS/shenfun&amp;utm_campaign=Badge_Grade
 .. image:: https://dev.azure.com/spectralDNS/shenfun/_apis/build/status/spectralDNS.shenfun?branchName=master
     :target: https://dev.azure.com/spectralDNS/shenfun
 .. image:: https://github.com/spectralDNS/shenfun/workflows/github-CI/badge.svg?branch=master
     :target: https://github.com/spectralDNS/shenfun
 .. image:: https://codecov.io/gh/spectralDNS/shenfun/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/spectralDNS/shenfun
 .. image:: https://anaconda.org/conda-forge/shenfun/badges/platforms.svg
     :target: https://anaconda.org/conda-forge/shenfun
-.. |binder| image:: https://mybinder.org/badge_logo.svg
-    :target: https://mybinder.org/v2/gh/spectralDNS/shenfun/master?filepath=binder
-
-
-Try it in a jupyter hub using Binder
-
-|binder|
 
 Description
 -----------
 Shenfun is a high performance computing platform for solving partial differential equations (PDEs) by the spectral Galerkin method. The user interface to shenfun is very similar to `FEniCS <https://fenicsproject.org>`_, but applications are limited to multidimensional tensor product grids, using either Cartesian or curvilinear grids (e.g., but not limited to, polar, cylindrical, spherical or parabolic). The code is parallelized with MPI through the `mpi4py-fft <https://bitbucket.org/mpi4py/mpi4py-fft>`_ package.
 
 Shenfun enables fast development of efficient and accurate PDE solvers (spectral order and accuracy), in the comfortable high-level Python language. The spectral accuracy is ensured by using high-order *global* orthogonal basis functions (Fourier, Legendre, Chebyshev first and second kind, Ultraspherical, Jacobi, Laguerre and Hermite), as opposed to finite element codes that are using low-order *local* basis functions. Efficiency is ensured through vectorization (`Numpy <https://www.numpy.org/>`_), parallelization (`mpi4py <https://bitbucket.org/mpi4py/mpi4py>`_) and by moving critical routines to `Cython <https://cython.org/>`_ or `Numba <https://numba.pydata.org>`_. Shenfun has been used to run turbulence simulations (Direct Numerical Simulations) on thousands of processors on high-performance supercomputers, see the `spectralDNS <https://github.com/spectralDNS/spectralDNS>`_ repository.
 
 The demo folder contains several examples for the Poisson, Helmholtz and Biharmonic equations. For extended documentation and installation instructions see `ReadTheDocs <http://shenfun.readthedocs.org>`_. For interactive demos, see the `jupyter book <https://mikaem.github.io/shenfun-demos>`_. Note that shenfun currently comes with the possibility to use two non-periodic directions (see `biharmonic demo <https://github.com/spectralDNS/shenfun/blob/master/demo/biharmonic2D_2nonperiodic.py>`_), and equations may be solved coupled and implicit (see `MixedPoisson.py <https://github.com/spectralDNS/shenfun/blob/master/demo/MixedPoisson.py>`_).
 
-Note that shenfun works with curvilinear coordinates. For example, it is possible to solve equations on a `sphere <https://github.com/spectralDNS/shenfun/blob/master/demo/sphere_helmholtz.py>`_ (using spherical coordinates), on the surface of a `torus <https://github.com/spectralDNS/shenfun/blob/master/binder/Torus.ipynb>`_, on a `Möbius strip <https://mikaem.github.io/shenfun-demos/content/moebius.html>`_ or along any `curved line in 2D/3D <https://github.com/spectralDNS/shenfun/blob/master/demo/curvilinear_poisson1D.py>`_. Actually, any new coordinates may be defined by the user as long as the coordinates lead to a system of equations with separable coefficients. After defining new coordinates, operators like div, grad and curl work automatically with the new curvilinear coordinates. See also `this notebook on the sphere <https://github.com/spectralDNS/shenfun/blob/master/binder/sphere-helmholtz.ipynb>`_ or an illustration of the `vector Laplacian <https://github.com/spectralDNS/shenfun/blob/master/binder/vector-laplacian.ipynb>`_.
+Note that shenfun works with curvilinear coordinates. For example, it is possible to solve equations on a `sphere <https://github.com/spectralDNS/shenfun/blob/master/demo/sphere_helmholtz.py>`_ (using spherical coordinates), on the surface of a `torus <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/Torus.ipynb>`_, on a `Möbius strip <https://mikaem.github.io/shenfun-demos/content/moebius.html>`_ or along any `curved line in 2D/3D <https://github.com/spectralDNS/shenfun/blob/master/demo/curvilinear_poisson1D.py>`_. Actually, any new coordinates may be defined by the user as long as the coordinates lead to a system of equations with separable coefficients. After defining new coordinates, operators like div, grad and curl work automatically with the new curvilinear coordinates. See also `this notebook on the sphere <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/sphere-helmholtz.ipynb>`_ or an illustration of the `vector Laplacian <https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/vector-laplacian.ipynb>`_.
 
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/moebius8_trans.png
     :target: https://mikaem.github.io/shenfun-demos/content/moebius.html
     :alt: The eigenvector of the 8'th smallest eigvalue on a Möbius strip
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/smallcoil2.png
     :alt: Solution of Poisson's equation on a Coil
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/spherewhite4.png
     :target: https://mikaem.github.io/shenfun-demos/content/sphericalhelmholtz.html
     :alt: Solution of Poisson's equation on a spherical shell
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/torus2.png
-    :target: https://github.com/spectralDNS/shenfun/blob/master/binder/Torus.ipynb
+    :target: https://github.com/spectralDNS/shenfun/blob/master/docs/notebooks/Torus.ipynb
     :alt: Solution of Poisson's equation on the surface of a torus
 
 
 For a more psychedelic experience, have a look at the `simulation <https://github.com/spectralDNS/shenfun/blob/master/demo/Ginzburg_Landau_sphere_IRK3.py>`_ of the Ginzburg-Landau equation on the sphere (click for Youtube-video):
 
 .. image:: https://cdn.jsdelivr.net/gh/spectralDNS/spectralutilities@master/figures/GLimage.png
     :target: https://youtu.be/odsIoHVcqek
@@ -99,9 +95,7 @@
 
     Mikael Mortensen
     mikaem at math.uio.no
     https://mikaem.github.io/
     Department of Mathematics
     University of Oslo
     Norway
-
-
```

### Comparing `shenfun-4.1.4/shenfun.egg-info/SOURCES.txt` & `shenfun-4.2.0/shenfun.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 .codacy.yml
 LICENSE
 MANIFEST.in
 README.rst
-azure-pipelines.yml
-leg2chebX.py
-readthedocs.yml
-requirements.txt
+environment.yml
+pyproject.toml
 setup.py
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/legendre/fastgl/fastgl_wrap.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/Cheb.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/Matvec.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/applymask.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/convolve.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/cross.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/evaluate.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/la.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/leg2chebm.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/outer.pyx
-/Users/mikaelmortensen/MySoftware/shenfun/shenfun/optimization/cython/transforms.pyx
+/home/runner/work/shenfun/shenfun/shenfun/legendre/fastgl/fastgl_wrap.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/Cheb.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/Matvec.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/applymask.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/convolve.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/cross.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/evaluate.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/la.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/leg2chebm.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/outer.pyx
+/home/runner/work/shenfun/shenfun/shenfun/optimization/cython/transforms.pyx
 shenfun/__init__.py
 shenfun/config.py
 shenfun/coordinates.py
 shenfun/la.py
 shenfun/matrixbase.py
 shenfun/spectralbase.py
 shenfun/tensorproductspace.py
 shenfun.egg-info/PKG-INFO
 shenfun.egg-info/SOURCES.txt
 shenfun.egg-info/dependency_links.txt
 shenfun.egg-info/requires.txt
 shenfun.egg-info/top_level.txt
-shenfun/bessel/__init__.py
-shenfun/bessel/bases.py
-shenfun/bessel/matrices.py
 shenfun/chebyshev/__init__.py
 shenfun/chebyshev/bases.py
 shenfun/chebyshev/la.py
 shenfun/chebyshev/matrices.py
 shenfun/chebyshevu/__init__.py
 shenfun/chebyshevu/bases.py
 shenfun/chebyshevu/matrices.py
@@ -60,30 +55,33 @@
 shenfun/laguerre/__init__.py
 shenfun/laguerre/bases.py
 shenfun/laguerre/matrices.py
 shenfun/legendre/__init__.py
 shenfun/legendre/bases.py
 shenfun/legendre/dlt.py
 shenfun/legendre/la.py
-shenfun/legendre/leg2chebX.py
 shenfun/legendre/lobatto.py
 shenfun/legendre/matrices.py
 shenfun/legendre/fastgl/__init__.py
+shenfun/legendre/fastgl/fastgl.cpp
+shenfun/legendre/fastgl/fastgl.h
+shenfun/legendre/fastgl/fastgl_wrap.pxd
 shenfun/legendre/fastgl/fastgl_wrap.pyx
 shenfun/optimization/__init__.py
 shenfun/optimization/cython/Cheb.pyx
 shenfun/optimization/cython/Matvec.pyx
 shenfun/optimization/cython/__init__.py
 shenfun/optimization/cython/applymask.pyx
 shenfun/optimization/cython/convolve.pyx
 shenfun/optimization/cython/cross.pyx
 shenfun/optimization/cython/evaluate.pyx
 shenfun/optimization/cython/la.pyx
 shenfun/optimization/cython/leg2chebm.pyx
 shenfun/optimization/cython/outer.pyx
+shenfun/optimization/cython/transforms.pxd
 shenfun/optimization/cython/transforms.pyx
 shenfun/optimization/numba/__init__.py
 shenfun/optimization/numba/biharmonic.py
 shenfun/optimization/numba/chebyshev.py
 shenfun/optimization/numba/diagma.py
 shenfun/optimization/numba/fdma.py
 shenfun/optimization/numba/helmholtz.py
```

### Comparing `shenfun-4.1.4/tests/test_backward.py` & `shenfun-4.2.0/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_bases.py` & `shenfun-4.2.0/tests/test_bases.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_curl.py` & `shenfun-4.2.0/tests/test_curl.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 def allclose(a, b):
     atol = tol[a.dtype.char.lower()]
     return np.allclose(a, b, rtol=0, atol=atol)
 
 @pytest.mark.parametrize('typecode', 'fdg')
 def test_curl(typecode):
+    from mpi4py_fft.fftw import fftlib
+    if typecode.upper() not in fftlib:
+        return
     K0 = FunctionSpace(N[0], 'F', dtype=typecode.upper())
     K1 = FunctionSpace(N[1], 'F', dtype=typecode.upper())
     K2 = FunctionSpace(N[2], 'F', dtype=typecode)
     T = TensorProductSpace(comm, (K0, K1, K2), dtype=typecode)
     X = T.local_mesh(True)
     K = T.local_wavenumbers()
     Tk = VectorSpace(T)
```

### Comparing `shenfun-4.1.4/tests/test_curvilinear.py` & `shenfun-4.2.0/tests/test_curvilinear.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_demos.py` & `shenfun-4.2.0/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_dot.py` & `shenfun-4.2.0/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_forms.py` & `shenfun-4.2.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_fourier.py` & `shenfun-4.2.0/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_io.py` & `shenfun-4.2.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_la.py` & `shenfun-4.2.0/tests/test_la.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_lagrangian_particles.py` & `shenfun-4.2.0/tests/test_lagrangian_particles.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_matrices.py` & `shenfun-4.2.0/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_spectralbase.py` & `shenfun-4.2.0/tests/test_spectralbase.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_tensorproductspace.py` & `shenfun-4.2.0/tests/test_tensorproductspace.py`

 * *Files identical despite different names*

### Comparing `shenfun-4.1.4/tests/test_transforms.py` & `shenfun-4.2.0/tests/test_transforms.py`

 * *Files identical despite different names*

