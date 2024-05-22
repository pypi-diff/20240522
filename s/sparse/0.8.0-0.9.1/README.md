# Comparing `tmp/sparse-0.8.0.tar.gz` & `tmp/sparse-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparse-0.8.0.tar", last modified: Mon Aug 26 18:00:36 2019, max compression
+gzip compressed data, was "dist/sparse-0.9.1.tar", last modified: Thu Jan 23 10:13:28 2020, max compression
```

## Comparing `sparse-0.8.0.tar` & `sparse-0.9.1.tar`

### file list

```diff
@@ -1,157 +1,165 @@
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     1517 2018-07-18 03:53:44.000000 sparse-0.8.0/LICENSE
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      324 2019-03-14 22:16:04.000000 sparse-0.8.0/MANIFEST.in
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     2271 2019-08-26 18:00:36.000000 sparse-0.8.0/PKG-INFO
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      971 2019-04-02 09:02:27.000000 sparse-0.8.0/README.rst
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/docs/
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/docs/_templates/
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/docs/_templates/autosummary/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      105 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      527 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      428 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     7938 2019-08-26 17:57:26.000000 sparse-0.8.0/docs/changelog.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     6142 2019-08-26 17:35:29.000000 sparse-0.8.0/docs/conf.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     5821 2018-07-18 16:18:44.000000 sparse-0.8.0/docs/construct.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     4668 2019-08-26 17:13:30.000000 sparse-0.8.0/docs/contributing.rst
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/docs/generated/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.T.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2018-08-05 14:24:36.000000 sparse-0.8.0/docs/generated/sparse.COO.all.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2018-08-05 14:24:36.000000 sparse-0.8.0/docs/generated/sparse.COO.any.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       82 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.COO.asformat.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       78 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.astype.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       98 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.broadcast_to.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.COO.clip.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2018-10-16 20:38:45.000000 sparse-0.8.0/docs/generated/sparse.COO.conj.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.COO.copy.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       85 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.COO.density.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.dot.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       78 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.dtype.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      104 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.enable_caching.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       87 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.COO.from_iter.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       92 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.from_numpy.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      115 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.from_scipy_sparse.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2018-10-16 20:38:45.000000 sparse-0.8.0/docs/generated/sparse.COO.imag.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       92 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.linear_loc.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.max.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      101 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.maybe_densify.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.COO.mean.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.min.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.nbytes.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.ndim.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.nnz.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       79 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.COO.nonzero.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.prod.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2018-10-16 20:38:45.000000 sparse-0.8.0/docs/generated/sparse.COO.real.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       78 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.reduce.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.reshape.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2019-07-08 13:11:00.000000 sparse-0.8.0/docs/generated/sparse.COO.resize.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.round.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     1527 2019-07-08 13:11:00.000000 sparse-0.8.0/docs/generated/sparse.COO.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.COO.size.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2019-03-31 01:28:16.000000 sparse-0.8.0/docs/generated/sparse.COO.std.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.sum.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      109 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.to_scipy_sparse.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.tocsc.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.tocsr.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.todense.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       87 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.COO.transpose.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2019-03-31 01:28:16.000000 sparse-0.8.0/docs/generated/sparse.COO.var.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       82 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.DOK.asformat.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       84 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.density.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       86 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.from_coo.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       92 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.from_numpy.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.ndim.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.nnz.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      401 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.DOK.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.size.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       80 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.to_coo.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.DOK.todense.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      106 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.asformat.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      108 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.density.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       99 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.ndim.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       96 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.nnz.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      352 2019-03-01 08:19:39.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       99 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.size.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      103 2019-03-01 08:19:39.000000 sparse-0.8.0/docs/generated/sparse.SparseArray.todense.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2019-03-14 22:16:04.000000 sparse-0.8.0/docs/generated/sparse.argwhere.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       68 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.as_coo.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.concatenate.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       57 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.dot.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2018-03-03 09:50:45.000000 sparse-0.8.0/docs/generated/sparse.elemwise.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       58 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.eye.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       61 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.full.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.full_like.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2019-07-08 13:11:00.000000 sparse-0.8.0/docs/generated/sparse.isneginf.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2019-07-08 13:11:00.000000 sparse-0.8.0/docs/generated/sparse.isposinf.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       61 2018-09-20 16:29:05.000000 sparse-0.8.0/docs/generated/sparse.kron.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       74 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.load_npz.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2018-11-11 18:11:44.000000 sparse-0.8.0/docs/generated/sparse.matmul.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2018-03-03 09:50:45.000000 sparse-0.8.0/docs/generated/sparse.nanmax.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       70 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.nanmean.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2018-03-03 09:50:45.000000 sparse-0.8.0/docs/generated/sparse.nanmin.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2018-03-03 09:50:45.000000 sparse-0.8.0/docs/generated/sparse.nanprod.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-04-20 05:25:09.000000 sparse-0.8.0/docs/generated/sparse.nanreduce.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2018-03-03 09:50:45.000000 sparse-0.8.0/docs/generated/sparse.nansum.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       61 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.ones.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.ones_like.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.random.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2019-08-22 07:06:08.000000 sparse-0.8.0/docs/generated/sparse.result_type.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       60 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.roll.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      630 2019-08-22 07:06:08.000000 sparse-0.8.0/docs/generated/sparse.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       74 2018-07-18 03:53:44.000000 sparse-0.8.0/docs/generated/sparse.save_npz.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       63 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.stack.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.tensordot.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       60 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.tril.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       60 2018-02-27 07:44:51.000000 sparse-0.8.0/docs/generated/sparse.triu.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       63 2018-03-03 09:50:45.000000 sparse-0.8.0/docs/generated/sparse.where.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       64 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.zeros.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       79 2018-09-20 08:53:25.000000 sparse-0.8.0/docs/generated/sparse.zeros_like.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     2946 2019-03-01 08:19:39.000000 sparse-0.8.0/docs/index.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      499 2018-02-27 07:45:21.000000 sparse-0.8.0/docs/install.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)   226597 2019-03-01 08:19:39.000000 sparse-0.8.0/docs/logo.png
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     8754 2019-03-01 08:19:39.000000 sparse-0.8.0/docs/operations.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     1823 2018-07-18 16:18:44.000000 sparse-0.8.0/docs/quickstart.rst
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     3548 2019-03-01 08:19:39.000000 sparse-0.8.0/docs/roadmap.rst
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/requirements/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       22 2019-03-14 22:16:04.000000 sparse-0.8.0/requirements/all.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       23 2019-03-14 22:16:04.000000 sparse-0.8.0/requirements/docs.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       36 2019-03-14 22:16:04.000000 sparse-0.8.0/requirements/tests.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       16 2019-03-14 22:16:04.000000 sparse-0.8.0/requirements/tox.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       30 2019-08-26 16:27:16.000000 sparse-0.8.0/requirements.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      296 2019-08-26 18:00:36.000000 sparse-0.8.0/setup.cfg
--rwxr-xr-x   0 hameerabbasi   (501) staff       (20)     2166 2019-03-14 22:16:04.000000 sparse-0.8.0/setup.py
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/sparse/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      237 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/__init__.py
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/sparse/_compressed/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)       29 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_compressed/__init__.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    13639 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_compressed/compressed.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     2179 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_compressed/convert.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     6483 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_compressed/indexing.py
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/sparse/_coo/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      717 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_coo/__init__.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    39116 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_coo/common.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    72353 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_coo/core.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    17748 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_coo/indexing.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    22939 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_coo/umath.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    10658 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_dok.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     2859 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_io.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      425 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_settings.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     8765 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_slicing.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     6262 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_sparse_array.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     9939 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/_utils.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      497 2019-08-26 18:00:36.000000 sparse-0.8.0/sparse/_version.py
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/sparse/tests/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      133 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/tests/conftest.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     1695 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/tests/test_array_function.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     4482 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/tests/test_compressed.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    57886 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/tests/test_coo.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     3589 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/tests/test_dok.py
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      847 2019-08-26 17:13:30.000000 sparse-0.8.0/sparse/tests/test_io.py
-drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2019-08-26 18:00:36.000000 sparse-0.8.0/sparse.egg-info/
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     2271 2019-08-26 18:00:35.000000 sparse-0.8.0/sparse.egg-info/PKG-INFO
--rw-r--r--   0 hameerabbasi   (501) staff       (20)     4511 2019-08-26 18:00:35.000000 sparse-0.8.0/sparse.egg-info/SOURCES.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)        1 2019-08-26 18:00:35.000000 sparse-0.8.0/sparse.egg-info/dependency_links.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)        1 2019-03-04 00:12:57.000000 sparse-0.8.0/sparse.egg-info/not-zip-safe
--rw-r--r--   0 hameerabbasi   (501) staff       (20)      228 2019-08-26 18:00:35.000000 sparse-0.8.0/sparse.egg-info/requires.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)        7 2019-08-26 18:00:35.000000 sparse-0.8.0/sparse.egg-info/top_level.txt
--rw-r--r--   0 hameerabbasi   (501) staff       (20)    68611 2018-04-20 05:25:09.000000 sparse-0.8.0/versioneer.py
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     1517 2020-01-23 10:12:50.000000 sparse-0.9.1/LICENSE
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      324 2020-01-23 10:12:50.000000 sparse-0.9.1/MANIFEST.in
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     2271 2020-01-23 10:13:28.000000 sparse-0.9.1/PKG-INFO
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      971 2020-01-23 10:12:50.000000 sparse-0.9.1/README.rst
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/docs/
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/docs/_templates/
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/docs/_templates/autosummary/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      105 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      527 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      428 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     8719 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/changelog.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     6164 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/conf.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     5821 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/construct.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     4668 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/contributing.rst
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/docs/generated/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.T.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.all.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.any.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       82 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.asformat.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       78 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.astype.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       98 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.broadcast_to.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.clip.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.conj.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.copy.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       85 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.density.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.dot.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       78 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.dtype.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      104 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.enable_caching.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       87 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.from_iter.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       92 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.from_numpy.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      115 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.from_scipy_sparse.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.imag.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       92 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.linear_loc.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.max.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      101 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.maybe_densify.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       73 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.mean.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.min.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.nbytes.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.ndim.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.nnz.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       79 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.nonzero.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.prod.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.real.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       78 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.reduce.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.reshape.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.resize.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.round.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     1527 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.size.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.std.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.sum.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      109 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.to_scipy_sparse.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.tocsc.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.tocsr.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.todense.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       87 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.transpose.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.COO.var.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       82 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.asformat.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       84 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.density.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       86 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.from_coo.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       92 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.from_numpy.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.ndim.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.nnz.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      397 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.size.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       80 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.to_coo.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.DOK.todense.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      106 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.asformat.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      108 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.density.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       99 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.ndim.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       96 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.nnz.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      352 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       99 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.size.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      103 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.SparseArray.todense.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.argwhere.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       68 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.as_coo.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.concatenate.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       77 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.diagonal.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.diagonalize.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       57 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.dot.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.elemwise.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       58 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.eye.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       61 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.full.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.full_like.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.isneginf.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       72 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.isposinf.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       61 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.kron.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       74 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.load_npz.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.matmul.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.nanmax.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       70 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.nanmean.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.nanmin.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       69 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.nanprod.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.nanreduce.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.nansum.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       61 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.ones.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       76 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.ones_like.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       66 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.random.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       81 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.result_type.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       60 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.roll.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      661 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       74 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.save_npz.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       63 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.stack.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       75 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.tensordot.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       60 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.tril.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       60 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.triu.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       63 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.where.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       64 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.zeros.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       79 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/generated/sparse.zeros_like.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     2946 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/index.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      499 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/install.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)   226597 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/logo.png
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     8754 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/operations.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     1823 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/quickstart.rst
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     3548 2020-01-23 10:12:50.000000 sparse-0.9.1/docs/roadmap.rst
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/requirements/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       22 2020-01-23 10:12:50.000000 sparse-0.9.1/requirements/all.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       23 2020-01-23 10:12:50.000000 sparse-0.9.1/requirements/docs.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       35 2020-01-23 10:12:50.000000 sparse-0.9.1/requirements/tests.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       16 2020-01-23 10:12:50.000000 sparse-0.9.1/requirements/tox.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       30 2020-01-23 10:12:50.000000 sparse-0.9.1/requirements.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      296 2020-01-23 10:13:28.000000 sparse-0.9.1/setup.cfg
+-rwxr-xr-x   0 hameerabbasi   (501) staff       (20)     2284 2020-01-23 10:12:50.000000 sparse-0.9.1/setup.py
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      263 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/__init__.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    11543 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_common.py
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse/_compressed/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       68 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_compressed/__init__.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     3557 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_compressed/common.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    14970 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_compressed/compressed.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     2068 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_compressed/convert.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     6053 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_compressed/indexing.py
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse/_coo/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      746 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_coo/__init__.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    37015 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_coo/common.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    72752 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_coo/core.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    18012 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_coo/indexing.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     9215 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_coo/numba_extension.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    23745 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_coo/umath.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    10798 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_dok.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     2977 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_io.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      165 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_numba_extension.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      424 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_settings.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     8913 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_slicing.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     6706 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_sparse_array.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    12641 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/_utils.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      497 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse/_version.py
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse/tests/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      133 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/conftest.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     1882 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/test_array_function.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     7133 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/test_compressed.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    59228 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/test_coo.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     1759 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/test_coo_numba.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     3523 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/test_dok.py
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      848 2020-01-23 10:12:50.000000 sparse-0.9.1/sparse/tests/test_io.py
+drwxr-xr-x   0 hameerabbasi   (501) staff       (20)        0 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     2271 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/PKG-INFO
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)     4753 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/SOURCES.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)        1 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/dependency_links.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)       67 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/entry_points.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)        1 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/not-zip-safe
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)      225 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/requires.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)        7 2020-01-23 10:13:28.000000 sparse-0.9.1/sparse.egg-info/top_level.txt
+-rw-r--r--   0 hameerabbasi   (501) staff       (20)    68751 2020-01-23 10:12:50.000000 sparse-0.9.1/versioneer.py
```

### Comparing `sparse-0.8.0/LICENSE` & `sparse-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/PKG-INFO` & `sparse-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse
-Version: 0.8.0
+Version: 0.9.1
 Summary: Sparse n-dimensional arrays
 Home-page: https://github.com/pydata/sparse/
 Maintainer: Hameer Abbasi
 Maintainer-email: hameerabbasi@yahoo.com
 License: BSD 3-Clause License (Revised)
 Project-URL: Documentation, https://sparse.pydata.org/
 Project-URL: Source, https://github.com/pydata/sparse/
@@ -42,11 +42,11 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.5, <4
+Provides-Extra: docs
 Provides-Extra: tests
-Provides-Extra: all
 Provides-Extra: tox
-Provides-Extra: docs
+Provides-Extra: all
```

### Comparing `sparse-0.8.0/README.rst` & `sparse-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/_templates/autosummary/class.rst` & `sparse-0.9.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/changelog.rst` & `sparse-0.9.1/docs/changelog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 Changelog
 =========
 
+.. currentmodule:: sparse
+
+0.9.1 / 2020-01-23
+------------------
+
+* Fixed a bug where indexing with an empty list could lead
+  to issues. (:issue:`281`, :pr:`282`)
+* Change code formatter to black. (:pr:`284`)
+* Add the :obj:`diagonal` and :obj:`diagonalize` functions.
+  (:issue:`288`, :pr:`289`, thanks :ghuser:`pettni`)
+* Add HTML repr for notebooks. (:pr:`283`, thanks :ghuser:`daletovar`)
+* Avoid making copy of ``coords`` when making a new :obj:`COO`
+  array.
+* Add stack and concatenate for GCXS. (:issue:`301`, :pr:`303`, thanks
+  :ghuser:`daletovar`).
+* Fix issue where functions dispatching to an attribute access wouldn't
+  work with ``__array_function__``. (:issue:`308`, :pr:`309`).
+* Add partial support for constructing and mirroring :obj:`COO` objects to
+  Numba.
+
 0.8.0 / 2019-08-26
 ------------------
 
 This release switches to Numba's new typed lists, a lot of
 back-end work with the CI infrastructure, so Linux, macOS
 and Windows are officially tested. It also includes bug fixes.
```

### Comparing `sparse-0.8.0/docs/conf.py` & `sparse-0.9.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,58 +16,60 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-sys.path.insert(0, os.path.abspath('..'))
+sys.path.insert(0, os.path.abspath(".."))
 from sparse import __version__  # flake8: noqa E402
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.inheritance_diagram',
-    'sphinx.ext.extlinks',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.inheritance_diagram",
+    "sphinx.ext.extlinks",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
-mathjax_path = "https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
+mathjax_path = (
+    "https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
+)
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'sparse'
-copyright = '2018, Sparse developers'
-author = 'Sparse Developers'
+project = "sparse"
+copyright = "2018, Sparse developers"
+author = "Sparse Developers"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = __version__
@@ -80,19 +82,18 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', '**tests**', '**setup**', '**extern**',
-                    '**data**']
+exclude_patterns = ["_build", "**tests**", "**setup**", "**extern**", "**data**"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 autosummary_generate = True
 
 # -- Options for HTML output ----------------------------------------------
@@ -126,69 +127,68 @@
 #         'searchbox.html',
 #     ]
 # }
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'sparsedoc'
+htmlhelp_basename = "sparsedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'sparse.tex', 'sparse Documentation',
-     'Sparse Developers', 'manual'),
+    (master_doc, "sparse.tex", "sparse Documentation", "Sparse Developers", "manual")
 ]
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'sparse', 'sparse Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "sparse", "sparse Documentation", [author], 1)]
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'sparse', 'sparse Documentation',
-     author, 'sparse', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "sparse",
+        "sparse Documentation",
+        author,
+        "sparse",
+        "One line description of project.",
+        "Miscellaneous",
+    )
 ]
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3/', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None)
+    "python": ("https://docs.python.org/3/", None),
+    "numpy": ("https://docs.scipy.org/doc/numpy/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference/", None),
 }
 
 extlinks = {
-    'issue': ('https://github.com/pydata/sparse/issues/%s', 'Issue #'),
-    'pr': ('https://github.com/pydata/sparse/pull/%s', 'PR #'),
-    'ghuser': ('https://github.com/%s', '@')
+    "issue": ("https://github.com/pydata/sparse/issues/%s", "Issue #"),
+    "pr": ("https://github.com/pydata/sparse/pull/%s", "PR #"),
+    "ghuser": ("https://github.com/%s", "@"),
 }
```

### Comparing `sparse-0.8.0/docs/construct.rst` & `sparse-0.9.1/docs/construct.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/contributing.rst` & `sparse-0.9.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/generated/sparse.COO.rst` & `sparse-0.9.1/docs/generated/sparse.COO.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/generated/sparse.rst` & `sparse-0.9.1/docs/generated/sparse.rst`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
     argwhere
 
     as_coo
 
     concatenate
 
+    diagonal
+
+    diagonalize
+
     dot
 
     elemwise
 
     eye
 
     full
```

### Comparing `sparse-0.8.0/docs/index.rst` & `sparse-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/logo.png` & `sparse-0.9.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/operations.rst` & `sparse-0.9.1/docs/operations.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/quickstart.rst` & `sparse-0.9.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/docs/roadmap.rst` & `sparse-0.9.1/docs/roadmap.rst`

 * *Files identical despite different names*

### Comparing `sparse-0.8.0/sparse/_compressed/compressed.py` & `sparse-0.9.1/sparse/_compressed/compressed.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 from functools import reduce
 from operator import mul
 from collections.abc import Iterable
 import scipy.sparse as ss
 
 from .._sparse_array import SparseArray
 from .._coo.common import linear_loc
-from .._utils import normalize_axis, check_zero_fill_value
+from .._utils import normalize_axis, check_zero_fill_value, check_compressed_axes
 from .._coo.core import COO
 from .convert import uncompress_dimension
 from .indexing import getitem
 
 
 def _from_coo(x, compressed_axes=None):
 
     if x.ndim == 0:
         if compressed_axes is not None:
-            raise ValueError('no axes to compress for 0d array')
-        return (
-            x.data, x.coords, []), x.shape, None, (), None, None, None, x.fill_value
+            raise ValueError("no axes to compress for 0d array")
+        return (x.data, x.coords, []), x.shape, None, (), None, None, None, x.fill_value
 
     if x.ndim == 1:
         if compressed_axes is not None:
-            raise ValueError('no axes to compress for 1d array')
+            raise ValueError("no axes to compress for 1d array")
         return (
-            x.data, x.coords[0], []), x.shape, None, None, None, None, None, x.fill_value
+            (x.data, x.coords[0], ()),
+            x.shape,
+            None,
+            None,
+            None,
+            None,
+            None,
+            x.fill_value,
+        )
 
     compressed_axes = normalize_axis(compressed_axes, x.ndim)
     if compressed_axes is None:
         # defaults to best compression ratio
         compressed_axes = (np.argmin(x.shape),)
 
-    if not isinstance(compressed_axes, Iterable):
-        raise ValueError('compressed_axes must be an iterable')
-    if len(compressed_axes) == len(x.shape):
-        raise ValueError('cannot compress all axes')
-    if not np.array_equal(
-            np.unique(compressed_axes), sorted(
-            np.array(compressed_axes))):
-        raise ValueError('repeated axis in compressed_axes')
+    check_compressed_axes(x.shape, compressed_axes)
 
     axis_order = list(compressed_axes)
     # array location where the uncompressed dimensions start
     axisptr = len(compressed_axes)
     axis_order.extend(np.setdiff1d(np.arange(len(x.shape)), compressed_axes))
     new_shape = np.array(x.shape)[axis_order]
     row_size = np.prod(new_shape[:axisptr])
@@ -57,179 +57,261 @@
     # linearizing twice is unnecessary, fix needed
     coords = x.reshape((compressed_shape)).coords
     indptr = np.empty(row_size + 1, dtype=np.intp)
     indptr[0] = 0
     np.cumsum(np.bincount(coords[0], minlength=row_size), out=indptr[1:])
     indices = coords[1]
     data = x.data[order]
-    return ((data, indices, indptr), shape, compressed_shape, compressed_axes, axis_order,
-            new_shape, axisptr, x.fill_value)
+    return (
+        (data, indices, indptr),
+        shape,
+        compressed_shape,
+        compressed_axes,
+        axis_order,
+        new_shape,
+        axisptr,
+        x.fill_value,
+    )
 
 
-class GXCS(SparseArray, NDArrayOperatorsMixin):
+class GCXS(SparseArray, NDArrayOperatorsMixin):
 
     __array_priority__ = 12
 
     def __init__(self, arg, shape=None, compressed_axes=None, fill_value=0):
 
         if isinstance(arg, np.ndarray):
-            arg, shape, compressed_shape, compressed_axes, axis_order, reordered_shape, axisptr, fill_value = _from_coo(
-                COO(arg), compressed_axes)
+            (
+                arg,
+                shape,
+                compressed_shape,
+                compressed_axes,
+                axis_order,
+                reordered_shape,
+                axisptr,
+                fill_value,
+            ) = _from_coo(COO(arg), compressed_axes)
 
         elif isinstance(arg, COO):
-            arg, shape, compressed_shape, compressed_axes, axis_order, reordered_shape, axisptr, fill_value = _from_coo(
-                arg, compressed_axes)
+            (
+                arg,
+                shape,
+                compressed_shape,
+                compressed_axes,
+                axis_order,
+                reordered_shape,
+                axisptr,
+                fill_value,
+            ) = _from_coo(arg, compressed_axes)
 
         if shape is None:
-            raise ValueError('missing `shape` argument')
+            raise ValueError("missing `shape` argument")
 
         if len(shape) != 1:
 
             # if initializing directly with (data,indices,indptr)
             compressed_axes = normalize_axis(compressed_axes, len(shape))
 
             if compressed_axes is None:
-                raise ValueError('missing `compressed_axes` argument')
+                raise ValueError("missing `compressed_axes` argument")
             elif compressed_axes != () and len(compressed_axes) >= len(shape):
-                raise ValueError('cannot compress all axes')
+                raise ValueError("cannot compress all axes")
             if not np.array_equal(
-                np.unique(compressed_axes), sorted(
-                    np.array(compressed_axes))):
-                raise ValueError('repeated axis in compressed_axes')
+                np.unique(compressed_axes), sorted(np.array(compressed_axes))
+            ):
+                raise ValueError("repeated axis in compressed_axes")
 
             axis_order = list(compressed_axes)
             # array location where the uncompressed dimensions start
             axisptr = len(compressed_axes)
-            axis_order.extend(
-                np.setdiff1d(
-                    np.arange(
-                        len(shape)),
-                    compressed_axes))
+            axis_order.extend(np.setdiff1d(np.arange(len(shape)), compressed_axes))
             reordered_shape = np.array(shape)[axis_order]
             row_size = np.prod(reordered_shape[:axisptr])
             col_size = np.prod(reordered_shape[axisptr:])
             compressed_shape = (row_size, col_size)
         else:
-            compressed_axes = compressed_shape = axis_order = reordered_shape = axisptr = None
+            compressed_axes = (
+                compressed_shape
+            ) = axis_order = reordered_shape = axisptr = None
 
         self.data, self.indices, self.indptr = arg
         self.shape = shape
         self.compressed_shape = compressed_shape
         self.compressed_axes = compressed_axes
         self.axis_order = axis_order
         self.axisptr = axisptr
         self.reordered_shape = reordered_shape
         self.fill_value = fill_value
-        self.dtype = self.data.dtype
 
     @classmethod
     def from_numpy(cls, x, compressed_axes=None, fill_value=0):
         coo = COO(x, fill_value=fill_value)
         return cls.from_coo(coo, compressed_axes)
 
     @classmethod
     def from_coo(cls, x, compressed_axes=None):
-        arg, shape, compressed_shape, compressed_axes, axis_order, reordered_shape, axisptr, fill_value = _from_coo(
-            x, compressed_axes)
-        return cls(
+        (
             arg,
-            shape=shape,
-            compressed_axes=compressed_axes,
-            fill_value=fill_value)
+            shape,
+            compressed_shape,
+            compressed_axes,
+            axis_order,
+            reordered_shape,
+            axisptr,
+            fill_value,
+        ) = _from_coo(x, compressed_axes)
+        return cls(
+            arg, shape=shape, compressed_axes=compressed_axes, fill_value=fill_value
+        )
 
     @classmethod
     def from_scipy_sparse(cls, x):
-        if x.format == 'csc':
-            return cls((x.data, x.indices, x.indptr),
-                       shape=x.shape, compressed_axes=(1,))
+        if x.format == "csc":
+            return cls(
+                (x.data, x.indices, x.indptr), shape=x.shape, compressed_axes=(1,)
+            )
         else:
-            x = x.asformat('csr')
-            return cls((x.data, x.indices, x.indptr),
-                       shape=x.shape, compressed_axes=(0,))
+            x = x.asformat("csr")
+            return cls(
+                (x.data, x.indices, x.indptr), shape=x.shape, compressed_axes=(0,)
+            )
 
     @classmethod
     def from_iter(cls, x, shape=None, compressed_axes=None, fill_value=None):
         return cls.from_coo(
-            COO.from_iter(
-                x,
-                shape,
-                fill_value),
-            compressed_axes=compressed_axes)
+            COO.from_iter(x, shape, fill_value), compressed_axes=compressed_axes
+        )
+
+    @property
+    def dtype(self):
+        """
+        The datatype of this array.
+        
+        Returns
+        -------
+        numpy.dtype
+            The datatype of this array.
+            
+        See Also
+        --------
+        numpy.ndarray.dtype : Numpy equivalent property.
+        scipy.sparse.csr_matrix.dtype : Scipy equivalent property.
+        """
+        return self.data.dtype
 
     @property
     def nnz(self):
+        """
+        The number of nonzero elements in this array.
+        
+        Returns
+        -------
+        int
+            The number of nonzero elements in this array.
+            
+        See Also
+        --------
+        COO.nnz : Equivalent :obj:`COO` array property.
+        DOK.nnz : Equivalent :obj:`DOK` array property.
+        numpy.count_nonzero : A similar Numpy function.
+        scipy.sparse.csr_matrix.nnz : The Scipy equivalent property.
+        """
         return self.data.shape[0]
 
     @property
     def nbytes(self):
-        return self.data.nbytes + self.indices.nbytes + self.indptr.nbytes
-
-    @property
-    def density(self):
-        return self.nnz / reduce(mul, self.shape, 1)
-
-    @property
-    def ndim(self):
-        return len(self.shape)
+        """
+        The number of bytes taken up by this object. Note that for small arrays,
+        this may undercount the number of bytes due to the large constant overhead.
+        
+        Returns
+        -------
+        int
+            The approximate bytes of memory taken by this object.
+        
+        See Also
+        --------
+        numpy.ndarray.nbytes : The equivalent Numpy property.
+        """
+        nbytes = self.data.nbytes + self.indices.nbytes
+        if self.indptr != ():
+            nbytes += self.indptr.nbytes
+        return nbytes
 
     def __str__(self):
-        return '<GXCS: shape={}, dtype={}, nnz={}, fill_value={}, compressed_axes={}>'.format(
-            self.shape, self.dtype, self.nnz, self.fill_value, self.compressed_axes)
+        return "<GCXS: shape={}, dtype={}, nnz={}, fill_value={}, compressed_axes={}>".format(
+            self.shape, self.dtype, self.nnz, self.fill_value, self.compressed_axes
+        )
 
     __repr__ = __str__
 
     __getitem__ = getitem
 
     def change_compressed_axes(self, new_compressed_axes):
         """
-        changes the compressed axes in-place.
-        right now the space complexity feels a little high
+        changes the compressed axes of an array.
         """
         if self.ndim == 1:
-            raise NotImplementedError('no axes to compress for 1d array')
+            raise NotImplementedError("no axes to compress for 1d array")
 
-        new_compressed_axes = tuple(normalize_axis(new_compressed_axes[i],
-                                                   self.ndim) for i in range(len(new_compressed_axes)))
+        new_compressed_axes = tuple(
+            normalize_axis(new_compressed_axes[i], self.ndim)
+            for i in range(len(new_compressed_axes))
+        )
 
         if len(new_compressed_axes) >= len(self.shape):
-            raise ValueError('cannot compress all axes')
+            raise ValueError("cannot compress all axes")
         if len(set(new_compressed_axes)) != len(new_compressed_axes):
-            raise ValueError('repeated axis in compressed_axes')
+            raise ValueError("repeated axis in compressed_axes")
         coo = self.tocoo()
-        arg, shape, compressed_shape, compressed_axes, axis_order, reordered_shape, axisptr, fill_value = _from_coo(
-            coo, new_compressed_axes)
-        self.data, self.indices, self.indptr = arg
-        self.compressed_shape = compressed_shape
-        self.compressed_axes = new_compressed_axes
-        self.axis_order = axis_order
-        self.reordered_shape = reordered_shape
-        self.axisptr = axisptr
+        (
+            arg,
+            shape,
+            compressed_shape,
+            compressed_axes,
+            axis_order,
+            reordered_shape,
+            axisptr,
+            fill_value,
+        ) = _from_coo(coo, new_compressed_axes)
+        return GCXS(
+            arg, shape=shape, compressed_axes=compressed_axes, fill_value=fill_value
+        )
 
     def tocoo(self):
         if self.ndim == 1:
-            return COO(self.indices[None, :], self.data,
-                       shape=self.shape, fill_value=self.fill_value)
+            return COO(
+                self.indices[None, :],
+                self.data,
+                shape=self.shape,
+                fill_value=self.fill_value,
+            )
         uncompressed = uncompress_dimension(self.indptr)
         coords = np.vstack((uncompressed, self.indices))
         order = np.argsort(self.axis_order)
-        return COO(
-            coords,
-            self.data,
-            shape=self.compressed_shape,
-            fill_value=self.fill_value).reshape(
-            self.reordered_shape).transpose(order)
+        return (
+            COO(
+                coords,
+                self.data,
+                shape=self.compressed_shape,
+                fill_value=self.fill_value,
+            )
+            .reshape(self.reordered_shape)
+            .transpose(order)
+        )
 
     def todense(self):
         if self.compressed_axes == ():
             return np.full(self.shape, self.fill_value, self.dtype)
         return self.tocoo().todense()
 
     def todok(self):
 
         from ..dok import DOK
+
         return DOK.from_coo(self.tocoo())  # probably a temporary solution
 
     def to_scipy_sparse(self):
         """
         Converts this :obj:`CSD` object into a :obj:`scipy.sparse.csr_matrix` or `scipy.sparse.csc_matrix`.
         Returns
         -------
@@ -243,22 +325,25 @@
             If all the array doesn't zero fill-values.
         """
 
         check_zero_fill_value(self)
 
         if self.ndim != 2:
             raise ValueError(
-                "Can only convert a 2-dimensional array to a Scipy sparse matrix.")
+                "Can only convert a 2-dimensional array to a Scipy sparse matrix."
+            )
 
         if 0 in self.compressed_axes:
             return ss.csr_matrix(
-                (self.data, self.indices, self.indptr), shape=self.shape)
+                (self.data, self.indices, self.indptr), shape=self.shape
+            )
         else:
             return ss.csc_matrix(
-                (self.data, self.indices, self.indptr), shape=self.shape)
+                (self.data, self.indices, self.indptr), shape=self.shape
+            )
 
     def asformat(self, format):
         """
         Convert this sparse array to a given format.
         Parameters
         ----------
         format : str
@@ -269,20 +354,20 @@
             The converted array.
         Raises
         ------
         NotImplementedError
             If the format isn't supported.
         """
 
-        if format == 'coo':
+        if format == "coo":
             return self.tocoo()
-        elif format == 'dok':
+        elif format == "dok":
             return self.todok()
 
-        raise NotImplementedError('The given format is not supported.')
+        raise NotImplementedError("The given format is not supported.")
 
     def maybe_densify(self, max_size=1000, min_density=0.25):
         """
         Converts this :obj:`CSR` or `CSC` array to a :obj:`numpy.ndarray` if not too
         costly.
         Parameters
         ----------
@@ -299,18 +384,19 @@
         ValueError
             If the returned array would be too large.
         """
 
         if self.size <= max_size or self.density >= min_density:
             return self.todense()
         else:
-            raise ValueError("Operation would require converting "
-                             "large sparse array to dense")
+            raise ValueError(
+                "Operation would require converting " "large sparse array to dense"
+            )
 
-    def reshape(self, shape, order='C', compressed_axes=None):
+    def reshape(self, shape, order="C", compressed_axes=None):
         """
         Returns a new :obj:`CSR` or `CSC` array that is a reshaped version of this array.
         Parameters
         ----------
         shape : tuple[int]
             The desired shape of the output array.
         Returns
@@ -324,32 +410,31 @@
         Notes
         -----
         The :code:`order` parameter is provided just for compatibility with
         Numpy and isn't actually supported.
 
         """
 
-        if order not in {'C', None}:
+        if order not in {"C", None}:
             raise NotImplementedError("The 'order' parameter is not supported")
         if any(d == -1 for d in shape):
-            extra = int(self.size /
-                        np.prod([d for d in shape if d != -1]))
+            extra = int(self.size / np.prod([d for d in shape if d != -1]))
             shape = tuple([d if d != -1 else extra for d in shape])
 
         if self.shape == shape:
             return self
 
         if self.size != reduce(mul, shape, 1):
             raise ValueError(
-                'cannot reshape array of size {} into shape {}'.format(
-                    self.size, shape))
+                "cannot reshape array of size {} into shape {}".format(self.size, shape)
+            )
 
         # there's likely a way to do this without decompressing to COO
         coo = self.tocoo().reshape(shape)
-        return GXCS.from_coo(coo, compressed_axes)
+        return GCXS.from_coo(coo, compressed_axes)
 
     def resize(self, *args, refcheck=True, compressed_axes=None):
         """
         This method changes the shape and size of an array in-place.
 
         Parameters
         ----------
@@ -363,27 +448,35 @@
         """
 
         if len(args) == 1 and isinstance(args[0], tuple):
             shape = args[0]
         elif all(isinstance(arg, int) for arg in args):
             shape = tuple(args)
         else:
-            raise ValueError('Invalid input')
+            raise ValueError("Invalid input")
 
         if any(d < 0 for d in shape):
-            raise ValueError('negative dimensions not allowed')
+            raise ValueError("negative dimensions not allowed")
 
         if self.shape == shape:
             return
 
         # there's likely a way to do this without decompressing to COO
         coo = self.tocoo()
         coo.resize(shape)
-        arg, shape, compressed_shape, compressed_axes, axis_order, reordered_shape, axisptr, fill_value = _from_coo(
-            coo, compressed_axes)
+        (
+            arg,
+            shape,
+            compressed_shape,
+            compressed_axes,
+            axis_order,
+            reordered_shape,
+            axisptr,
+            fill_value,
+        ) = _from_coo(coo, compressed_axes)
         self.data, self.indices, self.indptr = arg
         self.shape = shape
         self.compressed_shape = compressed_shape
         self.compressed_axes = compressed_axes
         self.axis_order = axis_order
         self.reordered_shape = reordered_shape
         self.axisptr = axisptr
```

### Comparing `sparse-0.8.0/sparse/_compressed/convert.py` & `sparse-0.9.1/sparse/_compressed/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 import numpy as np
 import numba
 from numba.typed import List
 
 
-def convert_to_flat(inds, shape, axisptr):
+def convert_to_flat(inds, shape):
     inds = [np.array(ind) for ind in inds]
     if any(ind.ndim > 1 for ind in inds):
-        raise IndexError('Only one-dimensional iterable indices supported.')
-    uncompressed_inds = inds[axisptr:]
-    cols = np.empty(
-        np.prod([ind.size for ind in uncompressed_inds]), dtype=np.intp)
-    shape_bins = transform_shape(shape[axisptr:])
+        raise IndexError("Only one-dimensional iterable indices supported.")
+    cols = np.empty(np.prod([ind.size for ind in inds]), dtype=np.intp)
+    shape_bins = transform_shape(shape)
     increments = List()
-    for i in range(len(uncompressed_inds)):
-        increments.append(
-            (uncompressed_inds[i] * shape_bins[i]).astype(np.int32))
+    for i in range(len(inds)):
+        increments.append((inds[i] * shape_bins[i]).astype(np.int32))
     operations = np.prod([ind.shape[0] for ind in increments[:-1]])
     return compute_flat(increments, cols, operations)
 
 
 @numba.jit(nopython=True, nogil=True)
 def compute_flat(increments, cols, operations):  # pragma: no cover
     start = 0
     end = increments[-1].shape[0]
-    positions = np.zeros(len(increments)-1, dtype=np.intp)
-    pos = len(increments)-2
+    positions = np.zeros(len(increments) - 1, dtype=np.intp)
+    pos = len(increments) - 2
     for i in range(operations):
         if i != 0 and positions[pos] == increments[pos].shape[0]:
             positions[pos] = 0
             pos -= 1
             positions[pos] += 1
             pos += 1
-        to_add = np.array([increments[i][positions[i]]
-                           for i in range(len(increments)-1)]).sum()
+        to_add = np.array(
+            [increments[i][positions[i]] for i in range(len(increments) - 1)]
+        ).sum()
         cols[start:end] = increments[-1] + to_add
         positions[pos] += 1
         start += increments[-1].shape[0]
         end += increments[-1].shape[0]
     return cols
 
 
@@ -44,19 +42,19 @@
     """
     turns a shape into the linearized increments that
     it represents. For example, given (5,5,5), it returns
     np.array([25,5,1]).
     """
     shape_bins = np.empty(len(shape), dtype=np.intp)
     shape_bins[-1] = 1
-    for i in range(len(shape)-2, -1, -1):
-        shape_bins[i] = np.prod(shape[i+1:])
+    for i in range(len(shape) - 2, -1, -1):
+        shape_bins[i] = np.prod(shape[i + 1 :])
     return shape_bins
 
 
 @numba.jit(nopython=True, nogil=True)
 def uncompress_dimension(indptr):  # pragma: no cover
     """converts an index pointer array into an array of coordinates"""
     uncompressed = np.empty(indptr[-1], dtype=np.intp)
     for i in range(len(indptr) - 1):
-        uncompressed[indptr[i]:indptr[i + 1]] = i
+        uncompressed[indptr[i] : indptr[i + 1]] = i
     return uncompressed
```

### Comparing `sparse-0.8.0/sparse/_compressed/indexing.py` & `sparse-0.9.1/sparse/_compressed/indexing.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,33 +8,35 @@
 
 
 def getitem(x, key):
     """
 
 
     """
-    from .compressed import GXCS
+    from .compressed import GCXS
 
     if x.ndim == 1:
         coo = x.tocoo()[key]
-        return GXCS.from_coo(coo)
+        return GCXS.from_coo(coo)
 
     key = list(normalize_index(key, x.shape))
 
     # zip_longest so things like x[..., None] are picked up.
-    if len(key) != 0 and all(isinstance(k, slice) and k == slice(0, dim, 1)
-                             for k, dim in zip_longest(key, x.shape)):
+    if len(key) != 0 and all(
+        isinstance(k, slice) and k == slice(0, dim, 1)
+        for k, dim in zip_longest(key, x.shape)
+    ):
         return x
 
     # return a single element
     if all(isinstance(k, int) for k in key):  # indexing for a single element
         key = np.array(key)[x.axis_order]  # reordering the input
         ind = np.ravel_multi_index(key, x.reordered_shape)
         row, col = np.unravel_index(ind, x.compressed_shape)
-        current_row = x.indices[x.indptr[row]:x.indptr[row + 1]]
+        current_row = x.indices[x.indptr[row] : x.indptr[row + 1]]
         item = np.searchsorted(current_row, col)
         if not (item >= current_row.size or current_row[item] != col):
             item += x.indptr[row]
             return x.data[item]
         return x.fill_value
 
     shape = []
@@ -64,35 +66,27 @@
                 compressed_inds[i] = True
             else:
                 uncompressed_inds[i] = True
         count += 1
 
     reordered_key = [Nones_removed[i] for i in x.axis_order]
 
-    # prepare for converting to flat indices
-    for i, ind in enumerate(reordered_key[:x.axisptr]):
-        if isinstance(ind, slice):
-            reordered_key[i] = range(ind.start, ind.stop, ind.step)
-    for i, ind in enumerate(reordered_key[x.axisptr:]):
+    for i, ind in enumerate(reordered_key):
         if isinstance(ind, Integral):
-            reordered_key[i + x.axisptr] = [ind]
+            reordered_key[i] = [ind]
         elif isinstance(ind, slice):
-            reordered_key[i +
-                          x.axisptr] = np.arange(ind.start, ind.stop, ind.step)
-
-    # find starts and ends of rows
-    a = x.indptr[:-1].reshape(x.reordered_shape[:x.axisptr])
-    b = x.indptr[1:].reshape(x.reordered_shape[:x.axisptr])
-    starts = a[tuple(reordered_key[:x.axisptr])].flatten()
-    ends = b[tuple(reordered_key[:x.axisptr])].flatten()
+            reordered_key[i] = np.arange(ind.start, ind.stop, ind.step)
 
     shape = np.array(shape)
 
-    cols = convert_to_flat(reordered_key, x.reordered_shape, x.axisptr)
+    rows = convert_to_flat(reordered_key[: x.axisptr], x.reordered_shape[: x.axisptr])
+    cols = convert_to_flat(reordered_key[x.axisptr :], x.reordered_shape[x.axisptr :])
 
+    starts = x.indptr[:-1][rows]
+    ends = x.indptr[1:][rows]
     if np.any(compressed_inds):
         compressed_axes = shape_key[compressed_inds]
 
         if len(compressed_axes) == 1:
             row_size = shape[compressed_axes]
         else:
             row_size = np.prod(shape[compressed_axes])
@@ -117,26 +111,26 @@
         if len(shape) == 1:
             indices = uncompressed
             indptr = None
         else:
             indices = uncompressed % size
             indptr = np.empty(shape[0] + 1, dtype=np.intp)
             indptr[0] = 0
-            np.cumsum(np.bincount(uncompressed //
-                                  size, minlength=shape[0]), out=indptr[1:])
+            np.cumsum(
+                np.bincount(uncompressed // size, minlength=shape[0]), out=indptr[1:]
+            )
     if not np.any(compressed_inds):
 
         if len(shape) == 1:
             indptr = None
         else:
             uncompressed = indices // size
             indptr = np.empty(shape[0] + 1, dtype=np.intp)
             indptr[0] = 0
-            np.cumsum(np.bincount(uncompressed,
-                                  minlength=shape[0]), out=indptr[1:])
+            np.cumsum(np.bincount(uncompressed, minlength=shape[0]), out=indptr[1:])
             indices = indices % size
 
     arg = (data, indices, indptr)
 
     compressed_axes = np.array(compressed_axes)
     shape = shape.tolist()
     for i in range(len(key)):
@@ -146,23 +140,23 @@
 
     compressed_axes = tuple(compressed_axes)
     shape = tuple(shape)
 
     if len(shape) == 1:
         compressed_axes = None
 
-    return GXCS(
-        arg,
-        shape=shape,
-        compressed_axes=compressed_axes,
-        fill_value=x.fill_value)
+    return GCXS(
+        arg, shape=shape, compressed_axes=compressed_axes, fill_value=x.fill_value
+    )
 
 
 @numba.jit(nopython=True, nogil=True)
-def get_array_selection(arr_data, arr_indices, indptr, starts, ends, col):  # pragma: no cover
+def get_array_selection(
+    arr_data, arr_indices, indptr, starts, ends, col
+):  # pragma: no cover
     """
     This is a very general algorithm to be used when more optimized methods don't apply.
     It performs a binary search for each of the requested elements.
     Consequently it roughly scales by O(n log nnz per row) where n is the number of requested elements and
     nnz per row is the number of nonzero elements in that row.
     """
     indices = []
```

### Comparing `sparse-0.8.0/sparse/_coo/common.py` & `sparse-0.9.1/sparse/_coo/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 from collections.abc import Iterable
 
 import numpy as np
 import scipy.sparse
 import numba
 
 from .._sparse_array import SparseArray
-from .._utils import isscalar, normalize_axis, check_zero_fill_value, check_consistent_fill_value
+from .._utils import (
+    isscalar,
+    normalize_axis,
+    check_zero_fill_value,
+    check_consistent_fill_value,
+)
 
 
-def asCOO(x, name='asCOO', check=True):
+def asCOO(x, name="asCOO", check=True):
     """
     Convert the input to :obj:`COO`. Passes through :obj:`COO` objects as-is.
 
     Parameters
     ----------
     x : Union[SparseArray, scipy.sparse.spmatrix, numpy.ndarray]
         The input array to convert.
@@ -34,15 +39,17 @@
     ------
     ValueError
         If ``check`` is true and a dense input is supplied.
     """
     from .core import COO
 
     if check and not isinstance(x, (SparseArray, scipy.sparse.spmatrix)):
-        raise ValueError('Performing this operation would produce a dense result: %s' % name)
+        raise ValueError(
+            "Performing this operation would produce a dense result: %s" % name
+        )
 
     if not isinstance(x, COO):
         x = COO(x)
 
     return x
 
 
@@ -182,18 +189,18 @@
 
     See Also
     --------
     numpy.matmul : NumPy equivalent function.
     COO.__matmul__ : Equivalent function for COO objects.
     """
     check_zero_fill_value(a, b)
-    if not hasattr(a, 'ndim') or not hasattr(b, 'ndim'):
+    if not hasattr(a, "ndim") or not hasattr(b, "ndim"):
         raise TypeError(
-            "Cannot perform dot product on types %s, %s" %
-            (type(a), type(b)))
+            "Cannot perform dot product on types %s, %s" % (type(a), type(b))
+        )
 
     # When b is 2-d, it is equivalent to dot
     if b.ndim <= 2:
         return dot(a, b)
 
     # when a is 2-d, we need to transpose result after dot
     if a.ndim <= 2:
@@ -215,31 +222,31 @@
 
     if a.ndim < b.ndim:
         a = a[(None,) * (b.ndim - a.ndim)]
     if a.ndim > b.ndim:
         b = b[(None,) * (a.ndim - b.ndim)]
     for i, j in zip(a.shape[:-2], b.shape[:-2]):
         if i != 1 and j != 1 and i != j:
-            raise ValueError('shapes of a and b are not broadcastable')
+            raise ValueError("shapes of a and b are not broadcastable")
 
     def _matmul_recurser(a, b):
         if a.ndim == 2:
             return dot(a, b)
         res = []
         for i in range(max(a.shape[0], b.shape[0])):
             a_i = a[0] if a.shape[0] == 1 else a[i]
             b_i = b[0] if b.shape[0] == 1 else b[i]
             res.append(_matmul_recurser(a_i, b_i))
         mask = [isinstance(x, SparseArray) for x in res]
         if all(mask):
             return stack(res)
         else:
-            res = [x.todense() if isinstance(x, SparseArray) else x
-                   for x in res]
+            res = [x.todense() if isinstance(x, SparseArray) else x for x in res]
             return np.stack(res)
+
     return _matmul_recurser(a, b)
 
 
 def dot(a, b):
     """
     Perform the equivalent of :obj:`numpy.dot` on two arrays.
 
@@ -260,36 +267,39 @@
 
     See Also
     --------
     numpy.dot : NumPy equivalent function.
     COO.dot : Equivalent function for COO objects.
     """
     check_zero_fill_value(a, b)
-    if not hasattr(a, 'ndim') or not hasattr(b, 'ndim'):
+    if not hasattr(a, "ndim") or not hasattr(b, "ndim"):
         raise TypeError(
-            "Cannot perform dot product on types %s, %s" %
-            (type(a), type(b)))
+            "Cannot perform dot product on types %s, %s" % (type(a), type(b))
+        )
 
     if a.ndim == 1 and b.ndim == 1:
         return (a * b).sum()
 
     a_axis = -1
     b_axis = -2
 
     if b.ndim == 1:
         b_axis = -1
     return tensordot(a, b, axes=(a_axis, b_axis))
 
 
 def _dot(a, b):
     from .core import COO
+
     out_shape = (a.shape[0], b.shape[1])
     if isinstance(a, COO) and isinstance(b, COO):
         b = b.T
-        coords, data = _dot_coo_coo_type(a.dtype, b.dtype)(a.coords, a.data, b.coords, b.data)
+        coords, data = _dot_coo_coo_type(a.dtype, b.dtype)(
+            a.coords, a.data, b.coords, b.data
+        )
 
         return COO(coords, data, shape=out_shape, has_duplicates=False, sorted=True)
 
     if isinstance(a, COO) and isinstance(b, np.ndarray):
         b = b.view(type=np.ndarray).T
         return _dot_coo_ndarray_type(a.dtype, b.dtype)(a.coords, a.data, b, out_shape)
 
@@ -315,34 +325,37 @@
     Raises
     ------
     ValueError
         If all arguments are dense or arguments have nonzero fill-values.
 
     Examples
     --------
+    >>> from sparse import eye
     >>> a = eye(3, dtype='i8')
     >>> b = np.array([1, 2, 3], dtype='i8')
     >>> res = kron(a, b)
     >>> res.todense()  # doctest: +SKIP
     array([[1, 2, 3, 0, 0, 0, 0, 0, 0],
            [0, 0, 0, 1, 2, 3, 0, 0, 0],
            [0, 0, 0, 0, 0, 0, 1, 2, 3]], dtype=int64)
     """
     from .core import COO
     from .umath import _cartesian_product
+
     check_zero_fill_value(a, b)
 
     a_sparse = isinstance(a, (SparseArray, scipy.sparse.spmatrix))
     b_sparse = isinstance(b, (SparseArray, scipy.sparse.spmatrix))
     a_ndim = np.ndim(a)
     b_ndim = np.ndim(b)
 
     if not (a_sparse or b_sparse):
-        raise ValueError('Performing this operation would produce a dense '
-                         'result: kron')
+        raise ValueError(
+            "Performing this operation would produce a dense " "result: kron"
+        )
 
     if a_ndim == 0 or b_ndim == 0:
         return a * b
 
     a = asCOO(a, check=False)
     b = asCOO(b, check=False)
 
@@ -384,38 +397,47 @@
         If all elements of :code:`arrays` don't have the same fill-value.
 
     See Also
     --------
     numpy.concatenate : NumPy equivalent function
     """
     from .core import COO
+
     check_consistent_fill_value(arrays)
 
     arrays = [x if isinstance(x, COO) else COO(x) for x in arrays]
     axis = normalize_axis(axis, arrays[0].ndim)
-    assert all(x.shape[ax] == arrays[0].shape[ax]
-               for x in arrays
-               for ax in set(range(arrays[0].ndim)) - {axis})
+    assert all(
+        x.shape[ax] == arrays[0].shape[ax]
+        for x in arrays
+        for ax in set(range(arrays[0].ndim)) - {axis}
+    )
     nnz = 0
     dim = sum(x.shape[axis] for x in arrays)
     shape = list(arrays[0].shape)
     shape[axis] = dim
 
     data = np.concatenate([x.data for x in arrays])
     coords = np.concatenate([x.coords for x in arrays], axis=1)
 
     dim = 0
     for x in arrays:
         if dim:
-            coords[axis, nnz:x.nnz + nnz] += dim
+            coords[axis, nnz : x.nnz + nnz] += dim
         dim += x.shape[axis]
         nnz += x.nnz
 
-    return COO(coords, data, shape=shape, has_duplicates=False,
-               sorted=(axis == 0), fill_value=arrays[0].fill_value)
+    return COO(
+        coords,
+        data,
+        shape=shape,
+        has_duplicates=False,
+        sorted=(axis == 0),
+        fill_value=arrays[0].fill_value,
+    )
 
 
 def stack(arrays, axis=0):
     """
     Stack the input arrays along the given dimension.
 
     Parameters
@@ -436,38 +458,45 @@
         If all elements of :code:`arrays` don't have the same fill-value.
 
     See Also
     --------
     numpy.stack : NumPy equivalent function
     """
     from .core import COO
+
     check_consistent_fill_value(arrays)
 
     assert len({x.shape for x in arrays}) == 1
     arrays = [x if isinstance(x, COO) else COO(x) for x in arrays]
     axis = normalize_axis(axis, arrays[0].ndim + 1)
     data = np.concatenate([x.data for x in arrays])
     coords = np.concatenate([x.coords for x in arrays], axis=1)
     shape = list(arrays[0].shape)
     shape.insert(axis, len(arrays))
 
     nnz = 0
     dim = 0
     new = np.empty(shape=(coords.shape[1],), dtype=np.intp)
     for x in arrays:
-        new[nnz:x.nnz + nnz] = dim
+        new[nnz : x.nnz + nnz] = dim
         dim += 1
         nnz += x.nnz
 
     coords = [coords[i] for i in range(coords.shape[0])]
     coords.insert(axis, new)
     coords = np.stack(coords, axis=0)
 
-    return COO(coords, data, shape=shape, has_duplicates=False,
-               sorted=(axis == 0), fill_value=arrays[0].fill_value)
+    return COO(
+        coords,
+        data,
+        shape=shape,
+        has_duplicates=False,
+        sorted=(axis == 0),
+        fill_value=arrays[0].fill_value,
+    )
 
 
 def triu(x, k=0):
     """
     Returns an array with all elements below the k-th diagonal set to zero.
 
     Parameters
@@ -489,18 +518,21 @@
         If :code:`x` doesn't have zero fill-values.
 
     See Also
     --------
     numpy.triu : NumPy equivalent function
     """
     from .core import COO
+
     check_zero_fill_value(x)
 
     if not x.ndim >= 2:
-        raise NotImplementedError('sparse.triu is not implemented for scalars or 1-D arrays.')
+        raise NotImplementedError(
+            "sparse.triu is not implemented for scalars or 1-D arrays."
+        )
 
     mask = x.coords[-2] + k <= x.coords[-1]
 
     coords = x.coords[:, mask]
     data = x.data[mask]
 
     return COO(coords, data, shape=x.shape, has_duplicates=False, sorted=True)
@@ -529,18 +561,21 @@
         If :code:`x` doesn't have zero fill-values.
 
     See Also
     --------
     numpy.tril : NumPy equivalent function
     """
     from .core import COO
+
     check_zero_fill_value(x)
 
     if not x.ndim >= 2:
-        raise NotImplementedError('sparse.tril is not implemented for scalars or 1-D arrays.')
+        raise NotImplementedError(
+            "sparse.tril is not implemented for scalars or 1-D arrays."
+        )
 
     mask = x.coords[-2] + k >= x.coords[-1]
 
     coords = x.coords[:, mask]
     data = x.data[mask]
 
     return COO(coords, data, shape=x.shape, has_duplicates=False, sorted=True)
@@ -568,15 +603,15 @@
 
     See Also
     --------
     :obj:`COO.sum` : Function without ``NaN`` skipping.
     numpy.nansum : Equivalent Numpy function.
     """
     assert out is None
-    x = asCOO(x, name='nansum')
+    x = asCOO(x, name="nansum")
     return nanreduce(x, np.add, axis=axis, keepdims=keepdims, dtype=dtype)
 
 
 def nanmean(x, axis=None, keepdims=False, dtype=None, out=None):
     """
     Performs a ``NaN`` skipping mean operation along the given axes. Uses all axes by default.
 
@@ -598,39 +633,39 @@
 
     See Also
     --------
     :obj:`COO.mean` : Function without ``NaN`` skipping.
     numpy.nanmean : Equivalent Numpy function.
     """
     assert out is None
-    x = asCOO(x, name='nanmean')
+    x = asCOO(x, name="nanmean")
 
     if not np.issubdtype(x.dtype, np.floating):
         return x.mean(axis=axis, keepdims=keepdims, dtype=dtype)
 
     mask = np.isnan(x)
     x2 = where(mask, 0, x)
 
     # Count the number non-nan elements along axis
-    nancount = mask.sum(axis=axis, dtype='i8', keepdims=keepdims)
+    nancount = mask.sum(axis=axis, dtype="i8", keepdims=keepdims)
     if axis is None:
         axis = tuple(range(x.ndim))
     elif not isinstance(axis, tuple):
         axis = (axis,)
     den = reduce(operator.mul, (x.shape[i] for i in axis), 1)
     den -= nancount
 
     if (den == 0).any():
         warnings.warn("Mean of empty slice", RuntimeWarning, stacklevel=2)
 
     num = np.sum(x2, axis=axis, dtype=dtype, keepdims=keepdims)
 
-    with np.errstate(invalid='ignore', divide='ignore'):
+    with np.errstate(invalid="ignore", divide="ignore"):
         if num.ndim:
-            return np.true_divide(num, den, casting='unsafe')
+            return np.true_divide(num, den, casting="unsafe")
         return (num / den).astype(dtype)
 
 
 def nanmax(x, axis=None, keepdims=False, dtype=None, out=None):
     """
     Maximize along the given axes, skipping ``NaN`` values. Uses all axes by default.
 
@@ -652,18 +687,17 @@
 
     See Also
     --------
     :obj:`COO.max` : Function without ``NaN`` skipping.
     numpy.nanmax : Equivalent Numpy function.
     """
     assert out is None
-    x = asCOO(x, name='nanmax')
+    x = asCOO(x, name="nanmax")
 
-    ar = x.reduce(np.fmax, axis=axis, keepdims=keepdims,
-                  dtype=dtype)
+    ar = x.reduce(np.fmax, axis=axis, keepdims=keepdims, dtype=dtype)
 
     if (isscalar(ar) and np.isnan(ar)) or np.isnan(ar.data).any():
         warnings.warn("All-NaN slice encountered", RuntimeWarning, stacklevel=2)
 
     return ar
 
 
@@ -689,18 +723,17 @@
 
     See Also
     --------
     :obj:`COO.min` : Function without ``NaN`` skipping.
     numpy.nanmin : Equivalent Numpy function.
     """
     assert out is None
-    x = asCOO(x, name='nanmin')
+    x = asCOO(x, name="nanmin")
 
-    ar = x.reduce(np.fmin, axis=axis, keepdims=keepdims,
-                  dtype=dtype)
+    ar = x.reduce(np.fmin, axis=axis, keepdims=keepdims, dtype=dtype)
 
     if (isscalar(ar) and np.isnan(ar)) or np.isnan(ar.data).any():
         warnings.warn("All-NaN slice encountered", RuntimeWarning, stacklevel=2)
 
     return ar
 
 
@@ -775,15 +808,15 @@
     y_given = y is not None
 
     if not (x_given or y_given):
         condition = asCOO(condition, name=str(np.where))
         return tuple(condition.coords)
 
     if x_given != y_given:
-        raise ValueError('either both or neither of x and y should be given')
+        raise ValueError("either both or neither of x and y should be given")
 
     return elemwise(np.where, condition, x, y)
 
 
 def argwhere(a):
     """
     Find the indices of array elements that are non-zero, grouped by element.
@@ -897,14 +930,15 @@
 
     Returns
     -------
     res : ndarray
         Output array, with the same shape as a.
     """
     from .core import COO, as_coo
+
     a = as_coo(a)
 
     # roll flattened array
     if axis is None:
         return roll(a.reshape((-1,)), shift, 0).reshape(a.shape)
 
     # roll across specified axis
@@ -915,266 +949,160 @@
             axis = (axis,)
 
         # make shift iterable
         if not isinstance(shift, Iterable):
             shift = (shift,)
 
         elif np.ndim(shift) > 1:
-            raise ValueError(
-                "'shift' and 'axis' must be integers or 1D sequences.")
+            raise ValueError("'shift' and 'axis' must be integers or 1D sequences.")
 
         # handle broadcasting
         if len(shift) == 1:
             shift = np.full(len(axis), shift)
 
         # check if dimensions are consistent
         if len(axis) != len(shift):
             raise ValueError(
-                "If 'shift' is a 1D sequence, "
-                "'axis' must have equal length.")
+                "If 'shift' is a 1D sequence, " "'axis' must have equal length."
+            )
 
         # shift elements
         coords, data = np.copy(a.coords), np.copy(a.data)
         for sh, ax in zip(shift, axis):
             coords[ax] += sh
             coords[ax] %= a.shape[ax]
 
-        return COO(coords, data=data, shape=a.shape, has_duplicates=False, fill_value=a.fill_value)
-
-
-def eye(N, M=None, k=0, dtype=float):
-    """Return a 2-D COO array with ones on the diagonal and zeros elsewhere.
+        return COO(
+            coords,
+            data=data,
+            shape=a.shape,
+            has_duplicates=False,
+            fill_value=a.fill_value,
+        )
+
+
+def diagonal(a, offset=0, axis1=0, axis2=1):
+    """
+    Extract diagonal from a COO array. The equivalent of :obj:`numpy.diagonal`.
 
     Parameters
     ----------
-    N : int
-        Number of rows in the output.
-    M : int, optional
-        Number of columns in the output. If None, defaults to `N`.
-    k : int, optional
-        Index of the diagonal: 0 (the default) refers to the main diagonal,
-        a positive value refers to an upper diagonal, and a negative value
-        to a lower diagonal.
-    dtype : data-type, optional
-        Data-type of the returned array.
-
-    Returns
-    -------
-    I : COO array of shape (N, M)
-        An array where all elements are equal to zero, except for the `k`-th
-        diagonal, whose values are equal to one.
+    a: COO
+        The array to perform the operation on.
+    offset: int, optional
+        Offset of the diagonal from the main diagonal. Defaults to main diagonal (0).
+    axis1: int, optional
+        First axis from which the diagonals should be taken.  
+        Defaults to first axis (0).
+    axis2 : int, optional
+        Second axis from which the diagonals should be taken.  
+        Defaults to second axis (1).
 
     Examples
     --------
-    >>> eye(2, dtype=int).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([[1, 0],
-           [0, 1]])
-    >>> eye(3, k=1).todense()  # doctest: +SKIP
-    array([[0., 1., 0.],
-           [0., 0., 1.],
-           [0., 0., 0.]])
-    """
-    from .core import COO
-
-    if M is None:
-        M = N
-
-    N = int(N)
-    M = int(M)
-    k = int(k)
-
-    data_length = min(N, M)
-
-    if k > 0:
-        data_length = max(min(data_length, M - k), 0)
-        n_coords = np.arange(data_length, dtype=np.intp)
-        m_coords = n_coords + k
-    elif k < 0:
-        data_length = max(min(data_length, N + k), 0)
-        m_coords = np.arange(data_length, dtype=np.intp)
-        n_coords = m_coords - k
-    else:
-        n_coords = m_coords = np.arange(data_length, dtype=np.intp)
-
-    coords = np.stack([n_coords, m_coords])
-    data = np.array(1, dtype=dtype)
-
-    return COO(coords, data=data, shape=(N, M), has_duplicates=False,
-               sorted=True)
-
-
-def full(shape, fill_value, dtype=None):
-    """Return a COO array of given shape and type, filled with `fill_value`.
-
-    Parameters
-    ----------
-    shape : int or tuple of ints
-        Shape of the new array, e.g., ``(2, 3)`` or ``2``.
-    fill_value : scalar
-        Fill value.
-    dtype : data-type, optional
-        The desired data-type for the array. The default, `None`, means
-        `np.array(fill_value).dtype`.
+    >>> import sparse
+    >>> x = sparse.as_coo(np.arange(9).reshape(3,3))
+    >>> sparse.diagonal(x).todense()
+    array([0, 4, 8])
+    >>> sparse.diagonal(x,offset=1).todense()
+    array([1, 5])
+
+    >>> x = sparse.as_coo(np.arange(12).reshape((2,3,2)))
+    >>> x_diag = sparse.diagonal(x, axis1=0, axis2=2)
+    >>> x_diag.shape
+    (3, 2)
+    >>> x_diag.todense()
+    array([[ 0,  7],
+           [ 2,  9],
+           [ 4, 11]])
 
     Returns
     -------
-    out : COO
-        Array of `fill_value` with the given shape and dtype.
+    out: COO
+        The result of the operation.
 
-    Examples
-    --------
-    >>> full(5, 9).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([9, 9, 9, 9, 9])
+    Raises
+    ------
+    ValueError
+        If a.shape[axis1] != a.shape[axis2]
 
-    >>> full((2, 2), 9, dtype=float).todense()  # doctest: +SKIP
-    array([[9., 9.],
-           [9., 9.]])
+    See Also
+    --------
+    :obj:`numpy.diagonal`: NumPy equivalent function
     """
     from .core import COO
 
-    if dtype is None:
-        dtype = np.array(fill_value).dtype
-    if not isinstance(shape, tuple):
-        shape = (shape,)
-    data = np.empty(0, dtype=dtype)
-    coords = np.empty((len(shape), 0), dtype=np.intp)
-    return COO(coords, data=data, shape=shape,
-               fill_value=fill_value, has_duplicates=False,
-               sorted=True)
+    if a.shape[axis1] != a.shape[axis2]:
+        raise ValueError("a.shape[axis1] != a.shape[axis2]")
 
+    diag_axes = [
+        axis for axis in range(len(a.shape)) if axis != axis1 and axis != axis2
+    ] + [axis1]
+    diag_shape = [a.shape[axis] for axis in diag_axes]
+    diag_shape[-1] -= abs(offset)
 
-def full_like(a, fill_value, dtype=None):
-    """Return a full array with the same shape and type as a given array.
+    diag_idx = _diagonal_idx(a.coords, axis1, axis2, offset)
 
-    Parameters
-    ----------
-    a : array_like
-        The shape and data-type of the result will match those of `a`.
-    dtype : data-type, optional
-        Overrides the data type of the result.
+    diag_coords = [a.coords[axis][diag_idx] for axis in diag_axes]
+    diag_data = a.data[diag_idx]
 
-    Returns
-    -------
-    out : COO
-        Array of `fill_value` with the same shape and type as `a`.
+    return COO(diag_coords, diag_data, diag_shape)
 
-    Examples
-    --------
-    >>> x = np.ones((2, 3), dtype='i8')
-    >>> full_like(x, 9.0).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([[9, 9, 9],
-           [9, 9, 9]])
-    """
-    return full(a.shape, fill_value, dtype=(a.dtype if dtype is None else dtype))
-
-
-def zeros(shape, dtype=float):
-    """Return a COO array of given shape and type, filled with zeros.
 
-    Parameters
-    ----------
-    shape : int or tuple of ints
-        Shape of the new array, e.g., ``(2, 3)`` or ``2``.
-    dtype : data-type, optional
-        The desired data-type for the array, e.g., `numpy.int8`.  Default is
-        `numpy.float64`.
-
-    Returns
-    -------
-    out : COO
-        Array of zeros with the given shape and dtype.
-
-    Examples
-    --------
-    >>> zeros(5).todense()  # doctest: +SKIP
-    array([0., 0., 0., 0., 0.])
-
-    >>> zeros((2, 2), dtype=int).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([[0, 0],
-           [0, 0]])
+def diagonalize(a, axis=0):
     """
-    return full(shape, 0, np.dtype(dtype))
-
+    Diagonalize a COO array. The new dimension is appended at the end.
 
-def zeros_like(a, dtype=None):
-    """Return a COO array of zeros with the same shape and type as ``a``.
+    .. WARNING:: :obj:`diagonalize` is not :obj:`numpy` compatible as there is no direct :obj:`numpy` equivalent. The API may change in the future.
 
     Parameters
     ----------
-    a : array_like
-        The shape and data-type of the result will match those of `a`.
-    dtype : data-type, optional
-        Overrides the data type of the result.
-
-    Returns
-    -------
-    out : COO
-        Array of zeros with the same shape and type as `a`.
+    a: Union[COO, np.ndarray, scipy.sparse.spmatrix]
+        The array to diagonalize.    
+    axis: int, optional
+        The axis to diagonalize. Defaults to first axis (0).
 
     Examples
     --------
-    >>> x = np.ones((2, 3), dtype='i8')
-    >>> zeros_like(x).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([[0, 0, 0],
-           [0, 0, 0]])
-    """
-    return zeros(a.shape, dtype=(a.dtype if dtype is None else dtype))
-
-
-def ones(shape, dtype=float):
-    """Return a COO array of given shape and type, filled with ones.
-
-    Parameters
-    ----------
-    shape : int or tuple of ints
-        Shape of the new array, e.g., ``(2, 3)`` or ``2``.
-    dtype : data-type, optional
-        The desired data-type for the array, e.g., `numpy.int8`.  Default is
-        `numpy.float64`.
+    >>> import sparse
+    >>> x = sparse.as_coo(np.arange(1,4))
+    >>> sparse.diagonalize(x).todense()
+    array([[1, 0, 0],
+           [0, 2, 0],
+           [0, 0, 3]])
+
+    >>> x = sparse.as_coo(np.arange(24).reshape((2,3,4)))
+    >>> x_diag = sparse.diagonalize(x, axis=1)
+    >>> x_diag.shape
+    (2, 3, 4, 3)
+
+    :obj:`diagonalize` is the inverse of :obj:`diagonal`
+
+    >>> a = sparse.random((3,3,3,3,3), density=0.3)
+    >>> a_diag = sparse.diagonalize(a, axis=2)
+    >>> (sparse.diagonal(a_diag, axis1=2, axis2=5) == a.transpose([0,1,3,4,2])).all()
+    True
 
     Returns
     -------
-    out : COO
-        Array of ones with the given shape and dtype.
+    out: COO
+        The result of the operation.
 
-    Examples
+    See Also
     --------
-    >>> ones(5).todense()  # doctest: +SKIP
-    array([1., 1., 1., 1., 1.])
-
-    >>> ones((2, 2), dtype=int).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([[1, 1],
-           [1, 1]])
+    :obj:`numpy.diag`: NumPy equivalent for 1D array
     """
-    return full(shape, 1, np.dtype(dtype))
-
-
-def ones_like(a, dtype=None):
-    """Return a COO array of ones with the same shape and type as ``a``.
+    from .core import COO, as_coo
 
-    Parameters
-    ----------
-    a : array_like
-        The shape and data-type of the result will match those of `a`.
-    dtype : data-type, optional
-        Overrides the data type of the result.
+    a = as_coo(a)
 
-    Returns
-    -------
-    out : COO
-        Array of ones with the same shape and type as `a`.
+    diag_shape = a.shape + (a.shape[axis],)
+    diag_coords = np.vstack([a.coords, a.coords[axis]])
 
-    Examples
-    --------
-    >>> x = np.ones((2, 3), dtype='i8')
-    >>> ones_like(x).todense()  # doctest: +NORMALIZE_WHITESPACE
-    array([[1, 1, 1],
-           [1, 1, 1]])
-    """
-    return ones(a.shape, dtype=(a.dtype if dtype is None else dtype))
+    return COO(diag_coords, a.data, diag_shape)
 
 
 def _memoize_dtype(f):
     """
     Memoizes a function taking in NumPy dtypes.
 
     Parameters
@@ -1210,16 +1138,19 @@
     return wrapped
 
 
 @_memoize_dtype
 def _dot_coo_coo_type(dt1, dt2):
     dtr = np.result_type(dt1, dt2)
 
-    @numba.jit(nopython=True, nogil=True,
-               locals={'data_curr': numba.numpy_support.from_dtype(dtr)})
+    @numba.jit(
+        nopython=True,
+        nogil=True,
+        locals={"data_curr": numba.numpy_support.from_dtype(dtr)},
+    )
     def _dot_coo_coo(coords1, data1, coords2, data2):  # pragma: no cover
         """
         Utility function taking in two ``COO`` objects and calculating a "sense"
         of their dot product. Acually computes ``s1 @ s2.T``.
 
         Parameters
         ----------
@@ -1234,20 +1165,26 @@
         didx1 = 0
 
         while didx1 < len(data1):
             oidx1 = coords1[0, didx1]
             didx2 = 0
             didx1_curr = didx1
 
-            while didx2 < len(data2) and didx1 < len(data1) and coords1[0, didx1] == oidx1:
+            while (
+                didx2 < len(data2) and didx1 < len(data1) and coords1[0, didx1] == oidx1
+            ):
                 oidx2 = coords2[0, didx2]
                 data_curr = 0
 
-                while didx2 < len(data2) and didx1 < len(data1) and \
-                        coords2[0, didx2] == oidx2 and coords1[0, didx1] == oidx1:
+                while (
+                    didx2 < len(data2)
+                    and didx1 < len(data1)
+                    and coords2[0, didx2] == oidx2
+                    and coords1[0, didx1] == oidx1
+                ):
                     if coords1[1, didx1] < coords2[1, didx2]:
                         didx1 += 1
                     elif coords1[1, didx1] > coords2[1, didx2]:
                         didx2 += 1
                     else:
                         data_curr += data1[didx1] * data2[didx2]
                         didx1 += 1
@@ -1366,14 +1303,15 @@
     array([ True])
 
     See Also
     --------
     numpy.isposinf : The NumPy equivalent
     """
     from .core import elemwise
+
     return elemwise(lambda x, out=None, dtype=None: np.isposinf(x, out=out), x, out=out)
 
 
 def isneginf(x, out=None):
     """
     Test element-wise for negative infinity, return result as sparse ``bool`` array.
 
@@ -1392,14 +1330,15 @@
     array([ True])
 
     See Also
     --------
     numpy.isneginf : The NumPy equivalent
     """
     from .core import elemwise
+
     return elemwise(lambda x, out=None, dtype=None: np.isneginf(x, out=out), x, out=out)
 
 
 def result_type(*arrays_and_dtypes):
     """Returns the type that results from applying the NumPy type promotion rules to the
     arguments.
 
@@ -1413,7 +1352,33 @@
 def _as_result_type_arg(x):
     if not isinstance(x, SparseArray):
         return x
     if x.ndim > 0:
         return x.dtype
     # 0-dimensional arrays give different result_type outputs than their dtypes
     return x.todense()
+
+
+@numba.jit(nopython=True, nogil=True)
+def _diagonal_idx(coordlist, axis1, axis2, offset):
+    """
+    Utility function that returns all indices that correspond to a diagonal element.
+
+    Parameters
+    ----------
+    coordlist : list of lists
+        Coordinate indices.
+
+    axis1, axis2 : int
+        The axes of the diagonal.
+
+    offset : int
+        Offset of the diagonal from the main diagonal. Defaults to main diagonal (0).
+
+    """
+    return np.array(
+        [
+            i
+            for i in range(len(coordlist[axis1]))
+            if coordlist[axis1][i] + offset == coordlist[axis2][i]
+        ]
+    )
```

### Comparing `sparse-0.8.0/sparse/_coo/core.py` & `sparse-0.9.1/sparse/_coo/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 from .common import dot, matmul
 from .indexing import getitem
 from .umath import elemwise, broadcast_to
 from .._sparse_array import SparseArray
 from .._utils import normalize_axis, equivalent, check_zero_fill_value, _zero_of_dtype
 
 
-_reduce_super_ufunc = {
-    np.add: np.multiply,
-    np.multiply: np.power,
-}
+_reduce_super_ufunc = {np.add: np.multiply, np.multiply: np.power}
 
 
 class COO(SparseArray, NDArrayOperatorsMixin):  # lgtm [py/missing-equals]
     """
     A sparse multidimensional array.
 
     This is stored in COO format.  It depends on NumPy and Scipy.sparse for
@@ -194,18 +191,28 @@
     >>> s7.todense()  # doctest: +NORMALIZE_WHITESPACE
     array([[0, 0, 0, 0, 0],
            [0, 4, 5, 0, 0],
            [0, 6, 7, 0, 0],
            [0, 0, 0, 0, 0],
            [0, 0, 0, 0, 0]])
     """
+
     __array_priority__ = 12
 
-    def __init__(self, coords, data=None, shape=None, has_duplicates=True,
-                 sorted=False, prune=False, cache=False, fill_value=None):
+    def __init__(
+        self,
+        coords,
+        data=None,
+        shape=None,
+        has_duplicates=True,
+        sorted=False,
+        prune=False,
+        cache=False,
+        fill_value=None,
+    ):
         self._cache = None
         if cache:
             self.enable_caching()
 
         if data is None:
             arr = as_coo(coords, shape=shape, fill_value=fill_value)
             self._make_shallow_copy_of(arr)
@@ -217,44 +224,53 @@
         if self.coords.ndim == 1:
             self.coords = self.coords[None, :]
 
         if self.data.ndim == 0:
             self.data = np.broadcast_to(self.data, self.coords.shape[1])
 
         if shape and not self.coords.size:
-            self.coords = np.zeros((len(shape) if isinstance(
-                shape, Iterable) else 1, 0), dtype=np.uint64)
+            self.coords = np.zeros(
+                (len(shape) if isinstance(shape, Iterable) else 1, 0), dtype=np.uint64
+            )
 
         if shape is None:
             if self.coords.nbytes:
                 shape = tuple((self.coords.max(axis=1) + 1))
             else:
                 shape = ()
 
         super().__init__(shape, fill_value=fill_value)
-        self.coords = self.coords.astype(np.intp)
+        self.coords = self.coords.astype(np.intp, copy=False)
 
         if self.shape:
             if len(self.data) != self.coords.shape[1]:
-                msg = ('The data length does not match the coordinates '
-                       'given.\nlen(data) = {}, but {} coords specified.')
+                msg = (
+                    "The data length does not match the coordinates "
+                    "given.\nlen(data) = {}, but {} coords specified."
+                )
                 raise ValueError(msg.format(len(data), self.coords.shape[1]))
             if len(self.shape) != self.coords.shape[0]:
-                msg = ("Shape specified by `shape` doesn't match the "
-                       "shape of `coords`; len(shape)={} != coords.shape[0]={}"
-                       "(and coords.shape={})")
-                raise ValueError(msg.format(len(shape),
-                                            self.coords.shape[0],
-                                            self.coords.shape))
+                msg = (
+                    "Shape specified by `shape` doesn't match the "
+                    "shape of `coords`; len(shape)={} != coords.shape[0]={}"
+                    "(and coords.shape={})"
+                )
+                raise ValueError(
+                    msg.format(len(shape), self.coords.shape[0], self.coords.shape)
+                )
 
         from .._settings import WARN_ON_TOO_DENSE
+
         if WARN_ON_TOO_DENSE and self.nbytes >= self.size * self.data.itemsize:
-            warnings.warn("Attempting to create a sparse array that takes no less "
-                          "memory than than an equivalent dense array. You may want to "
-                          "use a dense array here instead.", RuntimeWarning)
+            warnings.warn(
+                "Attempting to create a sparse array that takes no less "
+                "memory than than an equivalent dense array. You may want to "
+                "use a dense array here instead.",
+                RuntimeWarning,
+            )
 
         if not sorted:
             self._sort_indices()
 
         if has_duplicates:
             self._sum_duplicates()
 
@@ -344,16 +360,22 @@
         if x.shape:
             coords = np.where(~equivalent(x, fill_value))
             data = x[coords]
             coords = np.vstack(coords)
         else:
             coords = np.empty((0, 1), dtype=np.uint8)
             data = np.array(x, ndmin=1)
-        return cls(coords, data, shape=x.shape, has_duplicates=False,
-                   sorted=True, fill_value=fill_value)
+        return cls(
+            coords,
+            data,
+            shape=x.shape,
+            has_duplicates=False,
+            sorted=True,
+            fill_value=fill_value,
+        )
 
     def todense(self):
         """
         Convert this :obj:`COO` array to a dense :obj:`numpy.ndarray`. Note that
         this may take a large amount of memory if the :obj:`COO` object's :code:`shape`
         is large.
 
@@ -406,21 +428,25 @@
         Examples
         --------
         >>> x = scipy.sparse.rand(6, 3, density=0.2)
         >>> s = COO.from_scipy_sparse(x)
         >>> np.array_equal(x.todense(), s.todense())
         True
         """
-        x = x.asformat('coo')
+        x = x.asformat("coo")
         coords = np.empty((2, x.nnz), dtype=x.row.dtype)
         coords[0, :] = x.row
         coords[1, :] = x.col
-        return COO(coords, x.data, shape=x.shape,
-                   has_duplicates=not x.has_canonical_format,
-                   sorted=x.has_canonical_format)
+        return COO(
+            coords,
+            x.data,
+            shape=x.shape,
+            has_duplicates=not x.has_canonical_format,
+            sorted=x.has_canonical_format,
+        )
 
     @classmethod
     def from_iter(cls, x, shape=None, fill_value=None):
         """
         Converts an iterable in certain formats to a :obj:`COO` array. See examples
         for details.
 
@@ -476,32 +502,36 @@
         if isinstance(x, dict):
             x = list(x.items())
 
         if not isinstance(x, Sized):
             x = list(x)
 
         if len(x) != 2 and not all(len(item) == 2 for item in x):
-            raise ValueError('Invalid iterable to convert to COO.')
+            raise ValueError("Invalid iterable to convert to COO.")
 
         if not x:
             ndim = 0 if shape is None else len(shape)
             coords = np.empty((ndim, 0), dtype=np.uint8)
             data = np.empty((0,))
             shape = () if shape is None else shape
 
         elif not isinstance(x[0][0], Iterable):
             coords = np.stack(x[1], axis=0)
             data = np.asarray(x[0])
         else:
             coords = np.array([item[0] for item in x]).T
             data = np.array([item[1] for item in x])
 
-        if not (coords.ndim == 2 and data.ndim == 1 and
-                np.issubdtype(coords.dtype, np.integer) and np.all(coords >= 0)):
-            raise ValueError('Invalid iterable to convert to COO.')
+        if not (
+            coords.ndim == 2
+            and data.ndim == 1
+            and np.issubdtype(coords.dtype, np.integer)
+            and np.all(coords >= 0)
+        ):
+            raise ValueError("Invalid iterable to convert to COO.")
 
         return COO(coords, data, shape=shape, fill_value=fill_value)
 
     @property
     def dtype(self):
         """
         The datatype of this array.
@@ -607,15 +637,15 @@
 
     def __sizeof__(self):
         return self.nbytes
 
     __getitem__ = getitem
 
     def __str__(self):
-        return '<COO: shape={!s}, dtype={!s}, nnz={:d}, fill_value={!s}>'.format(
+        return "<COO: shape={!s}, dtype={!s}, nnz={:d}, fill_value={!s}>".format(
             self.shape, self.dtype, self.nnz, self.fill_value
         )
 
     __repr__ = __str__
 
     @staticmethod
     def _reduce(method, *args, **kwargs):
@@ -689,56 +719,69 @@
 
         By default, this reduces the array by only the first axis.
 
         >>> s.reduce(np.add)
         <COO: shape=(5,), dtype=int64, nnz=5, fill_value=0>
         """
         axis = normalize_axis(axis, self.ndim)
-        zero_reduce_result = method.reduce(
-            [self.fill_value, self.fill_value], **kwargs)
+        zero_reduce_result = method.reduce([self.fill_value, self.fill_value], **kwargs)
         reduce_super_ufunc = None
 
         if not equivalent(zero_reduce_result, self.fill_value):
             reduce_super_ufunc = _reduce_super_ufunc.get(method, None)
 
             if reduce_super_ufunc is None:
-                raise ValueError("Performing this reduction operation would produce "
-                                 "a dense result: %s" % str(method))
+                raise ValueError(
+                    "Performing this reduction operation would produce "
+                    "a dense result: %s" % str(method)
+                )
 
         if axis is None:
             axis = tuple(range(self.ndim))
 
         if not isinstance(axis, tuple):
             axis = (axis,)
 
         axis = tuple(a if a >= 0 else a + self.ndim for a in axis)
 
         neg_axis = tuple(ax for ax in range(self.ndim) if ax not in set(axis))
 
         a = self.transpose(neg_axis + axis)
-        a = a.reshape((np.prod([self.shape[d] for d in neg_axis], dtype=np.intp),
-                       np.prod([self.shape[d] for d in axis], dtype=np.intp)))
+        a = a.reshape(
+            (
+                np.prod([self.shape[d] for d in neg_axis], dtype=np.intp),
+                np.prod([self.shape[d] for d in axis], dtype=np.intp),
+            )
+        )
 
-        result, inv_idx, counts = _grouped_reduce(
-            a.data, a.coords[0], method, **kwargs)
+        result, inv_idx, counts = _grouped_reduce(a.data, a.coords[0], method, **kwargs)
 
         result_fill_value = self.fill_value
 
         if reduce_super_ufunc is None:
             missing_counts = counts != a.shape[1]
-            result[missing_counts] = method(result[missing_counts],
-                                            self.fill_value, **kwargs)
+            result[missing_counts] = method(
+                result[missing_counts], self.fill_value, **kwargs
+            )
         else:
-            result = method(result, reduce_super_ufunc(
-                self.fill_value, a.shape[1] - counts)).astype(result.dtype)
+            result = method(
+                result, reduce_super_ufunc(self.fill_value, a.shape[1] - counts)
+            ).astype(result.dtype)
             result_fill_value = reduce_super_ufunc(self.fill_value, a.shape[1])
         coords = a.coords[0:1, inv_idx]
 
-        a = COO(coords, result, shape=(a.shape[0],),
-                has_duplicates=False, sorted=True, prune=True, fill_value=result_fill_value)
+        a = COO(
+            coords,
+            result,
+            shape=(a.shape[0],),
+            has_duplicates=False,
+            sorted=True,
+            prune=True,
+            fill_value=result_fill_value,
+        )
 
         a = a.reshape(tuple(self.shape[d] for d in neg_axis))
         result = a
 
         if keepdims:
             result = _keepdims(self, result, axis)
 
@@ -1090,15 +1133,17 @@
         dtype('float16')
 
         By default, this reduces the array down to one number, multiplying along all axes.
 
         >>> s.prod()
         0
         """
-        return np.multiply.reduce(self, out=out, axis=axis, keepdims=keepdims, dtype=dtype)
+        return np.multiply.reduce(
+            self, out=out, axis=axis, keepdims=keepdims, dtype=dtype
+        )
 
     def mean(self, axis=None, keepdims=False, dtype=None, out=None):
         """
         Compute the mean along the given axes. Uses all axes by default.
 
         Parameters
         ----------
@@ -1161,27 +1206,27 @@
             axis = tuple(range(self.ndim))
         elif not isinstance(axis, tuple):
             axis = (axis,)
         den = reduce(operator.mul, (self.shape[i] for i in axis), 1)
 
         if dtype is None:
             if issubclass(self.dtype.type, (np.integer, np.bool_)):
-                dtype = inter_dtype = np.dtype('f8')
+                dtype = inter_dtype = np.dtype("f8")
             else:
                 dtype = self.dtype
-                inter_dtype = (np.dtype('f4')
-                               if issubclass(dtype.type, np.float16)
-                               else dtype)
+                inter_dtype = (
+                    np.dtype("f4") if issubclass(dtype.type, np.float16) else dtype
+                )
         else:
             inter_dtype = dtype
 
         num = self.sum(axis=axis, keepdims=keepdims, dtype=inter_dtype)
 
         if num.ndim:
-            out = np.true_divide(num, den, casting='unsafe')
+            out = np.true_divide(num, den, casting="unsafe")
             return out.astype(dtype) if out.dtype != dtype else out
         return np.divide(num, den, dtype=dtype, out=out)
 
     def var(self, axis=None, dtype=None, out=None, ddof=0, keepdims=False):
         """
         Compute the variance along the gi66ven axes. Uses all axes by default.
 
@@ -1254,15 +1299,15 @@
         rcount = reduce(operator.mul, (self.shape[a] for a in axis), 1)
         # Make this warning show up on top.
         if ddof >= rcount:
             warnings.warn("Degrees of freedom <= 0 for slice", RuntimeWarning)
 
         # Cast bool, unsigned int, and int to float64 by default
         if dtype is None and issubclass(self.dtype.type, (np.integer, np.bool_)):
-            dtype = np.dtype('f8')
+            dtype = np.dtype("f8")
 
         arrmean = self.sum(axis, dtype=dtype, keepdims=True)
         np.divide(arrmean, rcount, out=arrmean)
         x = self - arrmean
         if issubclass(self.dtype.type, np.complexfloating):
             x = x.real * x.real + x.imag * x.imag
         else:
@@ -1270,15 +1315,15 @@
 
         ret = x.sum(axis=axis, dtype=dtype, out=out, keepdims=keepdims)
 
         # Compute degrees of freedom and make sure it is not negative.
         rcount = max([rcount - ddof, 0])
 
         ret = ret[...]
-        np.divide(ret, rcount, out=ret, casting='unsafe')
+        np.divide(ret, rcount, out=ret, casting="unsafe")
         return ret[()]
 
     def std(self, axis=None, dtype=None, out=None, ddof=0, keepdims=False):
         """
         Compute the standard deviation along the given axes. Uses all axes by default.
 
         Parameters
@@ -1336,16 +1381,15 @@
 
         By default, this reduces the array down to one number, computing the
         standard deviation along all axes.
 
         >>> s.std()  # doctest: +SKIP
         0.7071067811865476
         """
-        ret = self.var(axis=axis, dtype=dtype, out=out, ddof=ddof,
-                       keepdims=keepdims)
+        ret = self.var(axis=axis, dtype=dtype, out=out, ddof=ddof, keepdims=keepdims)
 
         ret = np.sqrt(ret)
         return ret
 
     def transpose(self, axes=None):
         """
         Returns a new array which has the order of the axes switched.
@@ -1408,26 +1452,30 @@
 
         axes = tuple(axes)
 
         if axes == tuple(range(self.ndim)):
             return self
 
         if self._cache is not None:
-            for ax, value in self._cache['transpose']:
+            for ax, value in self._cache["transpose"]:
                 if ax == axes:
                     return value
 
         shape = tuple(self.shape[ax] for ax in axes)
-        result = COO(self.coords[axes, :], self.data, shape,
-                     has_duplicates=False,
-                     cache=self._cache is not None,
-                     fill_value=self.fill_value)
+        result = COO(
+            self.coords[axes, :],
+            self.data,
+            shape,
+            has_duplicates=False,
+            cache=self._cache is not None,
+            fill_value=self.fill_value,
+        )
 
         if self._cache is not None:
-            self._cache['transpose'].append((axes, result))
+            self._cache["transpose"].append((axes, result))
         return result
 
     @property
     def T(self):
         """
         Returns a new array which has the order of the axes reversed.
 
@@ -1491,15 +1539,15 @@
             is complex, the output dtype is float.
 
         See Also
         --------
         numpy.ndarray.real : NumPy equivalent attribute.
         numpy.real : NumPy equivalent function.
         """
-        return self.__array_ufunc__(np.real, '__call__', self)
+        return self.__array_ufunc__(np.real, "__call__", self)
 
     @property
     def imag(self):
         """The imaginary part of the array.
 
         Examples
         --------
@@ -1517,15 +1565,15 @@
             array is complex, the output dtype is float.
 
         See Also
         --------
         numpy.ndarray.imag : NumPy equivalent attribute.
         numpy.imag : NumPy equivalent function.
         """
-        return self.__array_ufunc__(np.imag, '__call__', self)
+        return self.__array_ufunc__(np.imag, "__call__", self)
 
     def conj(self):
         """Return the complex conjugate, element-wise.
 
         The complex conjugate of a complex number is obtained by changing the
         sign of its imaginary part.
 
@@ -1595,36 +1643,38 @@
     def __rmatmul__(self, other):
         try:
             return matmul(other, self)
         except NotImplementedError:
             return NotImplemented
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
-        out = kwargs.pop('out', None)
+        out = kwargs.pop("out", None)
         if out is not None and not all(isinstance(x, COO) for x in out):
             return NotImplemented
 
-        if getattr(ufunc, 'signature', None) is not None:
+        if getattr(ufunc, "signature", None) is not None:
             return self.__array_function__(ufunc, (np.ndarray, COO), inputs, kwargs)
 
         if out is not None:
-            kwargs['dtype'] = out[0].dtype
+            kwargs["dtype"] = out[0].dtype
 
-        if method == '__call__':
+        if method == "__call__":
             result = elemwise(ufunc, *inputs, **kwargs)
-        elif method == 'reduce':
+        elif method == "reduce":
             result = COO._reduce(ufunc, *inputs, **kwargs)
         else:
             return NotImplemented
 
         if out is not None:
             (out,) = out
             if out.shape != result.shape:
-                raise ValueError('non-broadcastable output operand with shape %s '
-                                 'doesn\'t match the broadcast shape %s' % (out.shape, result.shape))
+                raise ValueError(
+                    "non-broadcastable output operand with shape %s "
+                    "doesn't match the broadcast shape %s" % (out.shape, result.shape)
+                )
 
             out._make_shallow_copy_of(result)
             return out
 
         return result
 
     def linear_loc(self):
@@ -1653,17 +1703,18 @@
         >>> s = COO.from_numpy(x)
         >>> s.linear_loc()  # doctest: +NORMALIZE_WHITESPACE
         array([ 0,  6, 12, 18, 24])
         >>> np.array_equal(np.flatnonzero(x), s.linear_loc())
         True
         """
         from .common import linear_loc
+
         return linear_loc(self.coords, self.shape)
 
-    def reshape(self, shape, order='C'):
+    def reshape(self, shape, order="C"):
         """
         Returns a new :obj:`COO` array that is a reshaped version of this array.
         Parameters
         ----------
         shape : tuple[int]
             The desired shape of the output array.
         Returns
@@ -1689,52 +1740,57 @@
                [20, 21, 22, 23, 24]])
         """
         if isinstance(shape, Iterable):
             shape = tuple(shape)
         else:
             shape = (shape,)
 
-        if order not in {'C', None}:
+        if order not in {"C", None}:
             raise NotImplementedError("The `order` parameter is not supported")
 
         if self.shape == shape:
             return self
         if any(d == -1 for d in shape):
-            extra = int(self.size /
-                        np.prod([d for d in shape if d != -1]))
+            extra = int(self.size / np.prod([d for d in shape if d != -1]))
             shape = tuple([d if d != -1 else extra for d in shape])
 
         if self.shape == shape:
             return self
 
         if self.size != reduce(operator.mul, shape, 1):
             raise ValueError(
-                'cannot reshape array of size {} into shape {}'.format(self.size, shape))
+                "cannot reshape array of size {} into shape {}".format(self.size, shape)
+            )
 
         if self._cache is not None:
-            for sh, value in self._cache['reshape']:
+            for sh, value in self._cache["reshape"]:
                 if sh == shape:
                     return value
 
         # TODO: this self.size enforces a 2**64 limit to array size
         linear_loc = self.linear_loc()
 
         coords = np.empty((len(shape), self.nnz), dtype=np.intp)
         strides = 1
         for i, d in enumerate(shape[::-1]):
             coords[-(i + 1), :] = (linear_loc // strides) % d
             strides *= d
 
-        result = COO(coords, self.data, shape,
-                     has_duplicates=False,
-                     sorted=True, cache=self._cache is not None,
-                     fill_value=self.fill_value)
+        result = COO(
+            coords,
+            self.data,
+            shape,
+            has_duplicates=False,
+            sorted=True,
+            cache=self._cache is not None,
+            fill_value=self.fill_value,
+        )
 
         if self._cache is not None:
-            self._cache['reshape'].append((shape, result))
+            self._cache["reshape"].append((shape, result))
         return result
 
     def resize(self, *args, refcheck=True):
         """
         This method changes the shape and size of an array in-place.
         Parameters
         ----------
@@ -1747,24 +1803,24 @@
 
         """
         if len(args) == 1 and isinstance(args[0], tuple):
             shape = args[0]
         elif all(isinstance(arg, int) for arg in args):
             shape = tuple(args)
         else:
-            raise ValueError('Invalid input')
+            raise ValueError("Invalid input")
 
         if any(d < 0 for d in shape):
-            raise ValueError('negative dimensions not allowed')
+            raise ValueError("negative dimensions not allowed")
 
         new_size = reduce(operator.mul, shape, 1)
 
         # TODO: this self.size enforces a 2**64 limit to array size
         linear_loc = self.linear_loc()
-        end_idx = np.searchsorted(linear_loc, new_size, side='left')
+        end_idx = np.searchsorted(linear_loc, new_size, side="left")
         linear_loc = linear_loc[:end_idx]
 
         coords = np.empty((len(shape), len(linear_loc)), dtype=np.intp)
         strides = 1
         for i, d in enumerate(shape[::-1]):
             coords[-(i + 1), :] = (linear_loc // strides) % d
             strides *= d
@@ -1797,27 +1853,28 @@
         COO.tocsr : Convert to a :obj:`scipy.sparse.csr_matrix`.
         COO.tocsc : Convert to a :obj:`scipy.sparse.csc_matrix`.
         """
         check_zero_fill_value(self)
 
         if self.ndim != 2:
             raise ValueError(
-                "Can only convert a 2-dimensional array to a Scipy sparse matrix.")
+                "Can only convert a 2-dimensional array to a Scipy sparse matrix."
+            )
 
-        result = scipy.sparse.coo_matrix((self.data,
-                                          (self.coords[0],
-                                           self.coords[1])),
-                                         shape=self.shape)
+        result = scipy.sparse.coo_matrix(
+            (self.data, (self.coords[0], self.coords[1])), shape=self.shape
+        )
         result.has_canonical_format = True
         return result
 
     def _tocsr(self):
         if self.ndim != 2:
-            raise ValueError('This array must be two-dimensional for this conversion '
-                             'to work.')
+            raise ValueError(
+                "This array must be two-dimensional for this conversion " "to work."
+            )
         row, col = self.coords
 
         # Pass 3: count nonzeros in each row
         indptr = np.zeros(self.shape[0] + 1, dtype=np.int64)
         np.cumsum(np.bincount(row, minlength=self.shape[0]), out=indptr[1:])
 
         return scipy.sparse.csr_matrix((self.data, col, indptr), shape=self.shape)
@@ -1922,15 +1979,15 @@
         array([3, 4, 1], dtype=uint8)
         """
         linear = self.linear_loc()
 
         if (np.diff(linear) >= 0).all():  # already sorted
             return
 
-        order = np.argsort(linear, kind='mergesort')
+        order = np.argsort(linear, kind="mergesort")
         self.coords = self.coords[:, order]
         self.data = self.data[order]
 
     def _sum_duplicates(self):
         """
         Sums data corresponding to duplicates in :obj:`COO.coords`.
 
@@ -2018,15 +2075,17 @@
         --------
         :obj:`numpy.round` : NumPy equivalent ufunc.
         :obj:`COO.elemwise`: Apply an arbitrary element-wise function to one or two
             arguments.
         """
         if out is not None and not isinstance(out, tuple):
             out = (out,)
-        return self.__array_ufunc__(np.round, '__call__', self, decimals=decimals, out=out)
+        return self.__array_ufunc__(
+            np.round, "__call__", self, decimals=decimals, out=out
+        )
 
     round_ = round
 
     def clip(self, min=None, max=None, out=None):
         """Clip (limit) the values in the array.
 
         Return an array whose values are limited to ``[min, max]``. One of min
@@ -2061,29 +2120,32 @@
         >>> x.clip(min=1, max=2).todense() # doctest: +NORMALIZE_WHITESPACE
         array([1, 1, 1, 1, 2, 2])
         """
         if min is None and max is None:
             raise ValueError("One of max or min must be given.")
         if out is not None and not isinstance(out, tuple):
             out = (out,)
-        return self.__array_ufunc__(np.clip, '__call__', self, a_min=min,
-                                    a_max=max, out=out)
+        return self.__array_ufunc__(
+            np.clip, "__call__", self, a_min=min, a_max=max, out=out
+        )
 
     def astype(self, dtype, copy=True):
         """
         Copy of the array, cast to a specified type.
 
         See also
         --------
         scipy.sparse.coo_matrix.astype : SciPy sparse equivalent function
         numpy.ndarray.astype : NumPy equivalent ufunc.
         :obj:`COO.elemwise`: Apply an arbitrary element-wise function to one or two
             arguments.
         """
-        return self.__array_ufunc__(np.ndarray.astype, '__call__', self, dtype=dtype, copy=copy)
+        return self.__array_ufunc__(
+            np.ndarray.astype, "__call__", self, dtype=dtype, copy=copy
+        )
 
     def maybe_densify(self, max_size=1000, min_density=0.25):
         """
         Converts this :obj:`COO` array to a :obj:`numpy.ndarray` if not too
         costly.
 
         Parameters
@@ -2123,16 +2185,17 @@
         Traceback (most recent call last):
             ...
         ValueError: Operation would require converting large sparse array to dense
         """
         if self.size <= max_size or self.density >= min_density:
             return self.todense()
         else:
-            raise ValueError("Operation would require converting "
-                             "large sparse array to dense")
+            raise ValueError(
+                "Operation would require converting " "large sparse array to dense"
+            )
 
     def nonzero(self):
         """
         Get the indices where this array is nonzero.
 
         Returns
         -------
@@ -2172,29 +2235,33 @@
             The converted array.
 
         Raises
         ------
         NotImplementedError
             If the format isn't supported.
         """
-        from .._compressed import GXCS
-        if format == 'gxcs' or format is GXCS:
-            return GXCS.from_coo(self, compressed_axes=compressed_axes)
+        from .._compressed import GCXS
+
+        if format == "gcxs" or format is GCXS:
+            return GCXS.from_coo(self, compressed_axes=compressed_axes)
+
         elif compressed_axes is not None:
             raise ValueError(
-                'compressed_axes is not supported for {} format'.format(format))
+                "compressed_axes is not supported for {} format".format(format)
+            )
 
-        if format == 'coo' or format is COO:
+        if format == "coo" or format is COO:
             return self
 
         from .._dok import DOK
-        if format == 'dok' or format is DOK:
+
+        if format == "dok" or format is DOK:
             return DOK.from_coo(self)
 
-        raise NotImplementedError('The given format is not supported.')
+        raise NotImplementedError("The given format is not supported.")
 
 
 def as_coo(x, shape=None, fill_value=None):
     """
     Converts any given format to :obj:`COO`. See the "See Also" section for details.
 
     Parameters
@@ -2212,36 +2279,42 @@
     See Also
     --------
     SparseArray.asformat : A utility function to convert between formats in this library.
     COO.from_numpy : Convert a Numpy array to :obj:`COO`.
     COO.from_scipy_sparse : Convert a SciPy sparse matrix to :obj:`COO`.
     COO.from_iter : Convert an iterable to :obj:`COO`.
     """
-    if hasattr(x, 'shape') and shape is not None:
-        raise ValueError('Cannot provide a shape in combination with something '
-                         'that already has a shape.')
-
-    if hasattr(x, 'fill_value') and fill_value is not None:
-        raise ValueError('Cannot provide a fill-value in combination with something '
-                         'that already has a fill-value.')
+    if hasattr(x, "shape") and shape is not None:
+        raise ValueError(
+            "Cannot provide a shape in combination with something "
+            "that already has a shape."
+        )
+
+    if hasattr(x, "fill_value") and fill_value is not None:
+        raise ValueError(
+            "Cannot provide a fill-value in combination with something "
+            "that already has a fill-value."
+        )
 
     if isinstance(x, SparseArray):
-        return x.asformat('coo')
+        return x.asformat("coo")
 
     if isinstance(x, np.ndarray):
         return COO.from_numpy(x, fill_value=fill_value)
 
     if isinstance(x, scipy.sparse.spmatrix):
         return COO.from_scipy_sparse(x)
 
     if isinstance(x, (Iterable, Iterator)):
         return COO.from_iter(x, shape=shape, fill_value=fill_value)
 
-    raise NotImplementedError('Format not supported for conversion. Supplied type is '
-                              '%s, see help(sparse.as_coo) for supported formats.' % type(x))
+    raise NotImplementedError(
+        "Format not supported for conversion. Supplied type is "
+        "%s, see help(sparse.as_coo) for supported formats." % type(x)
+    )
 
 
 def _keepdims(original, new, axis):
     shape = list(original.shape)
     for ax in axis:
         shape[ax] = 1
     return new.reshape(shape)
@@ -2249,30 +2322,31 @@
 
 @numba.jit(nopython=True, nogil=True)  # pragma: no cover
 def _calc_counts_invidx(groups):
     inv_idx = []
     counts = []
 
     if len(groups) == 0:
-        return (np.array(inv_idx, dtype=groups.dtype),
-                np.array(counts, dtype=groups.dtype))
+        return (
+            np.array(inv_idx, dtype=groups.dtype),
+            np.array(counts, dtype=groups.dtype),
+        )
 
     inv_idx.append(0)
 
     last_group = groups[0]
     for i in range(1, len(groups)):
         if groups[i] != last_group:
             counts.append(i - inv_idx[-1])
             inv_idx.append(i)
             last_group = groups[i]
 
     counts.append(len(groups) - inv_idx[-1])
 
-    return (np.array(inv_idx, dtype=groups.dtype),
-            np.array(counts, dtype=groups.dtype))
+    return (np.array(inv_idx, dtype=groups.dtype), np.array(counts, dtype=groups.dtype))
 
 
 def _grouped_reduce(x, groups, method, **kwargs):
     """
     Performs a :code:`ufunc` grouped reduce.
 
     Parameters
```

### Comparing `sparse-0.8.0/sparse/_coo/indexing.py` & `sparse-0.9.1/sparse/_coo/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,37 +35,45 @@
         data = x.data[index]
         idx = np.where(data)
         data = data[idx].flatten()
         coords = list(x.coords[:, idx[0]])
         coords.extend(idx[1:])
 
         fill_value_idx = np.asarray(x.fill_value[index]).flatten()
-        fill_value = fill_value_idx[0] if fill_value_idx.size else _zero_of_dtype(data.dtype)[()]
+        fill_value = (
+            fill_value_idx[0] if fill_value_idx.size else _zero_of_dtype(data.dtype)[()]
+        )
 
         if not equivalent(fill_value, fill_value_idx).all():
-            raise ValueError('Fill-values in the array are inconsistent.')
+            raise ValueError("Fill-values in the array are inconsistent.")
 
-        return COO(coords, data,
-                   shape=x.shape + x.data.dtype[index].shape,
-                   has_duplicates=False,
-                   sorted=True, fill_value=fill_value)
+        return COO(
+            coords,
+            data,
+            shape=x.shape + x.data.dtype[index].shape,
+            has_duplicates=False,
+            sorted=True,
+            fill_value=fill_value,
+        )
 
     # Otherwise, convert into a tuple.
     if not isinstance(index, tuple):
         index = (index,)
 
     # Check if the last index is an ellipsis.
     last_ellipsis = len(index) > 0 and index[-1] is Ellipsis
 
     # Normalize the index into canonical form.
     index = normalize_index(index, x.shape)
 
     # zip_longest so things like x[..., None] are picked up.
-    if len(index) != 0 and all(isinstance(ind, slice) and ind == slice(0, dim, 1)
-                               for ind, dim in zip_longest(index, x.shape)):
+    if len(index) != 0 and all(
+        isinstance(ind, slice) and ind == slice(0, dim, 1)
+        for ind, dim in zip_longest(index, x.shape)
+    ):
         return x
 
     # Get the mask
     mask, adv_idx = _mask(x.coords, index, x.shape)
 
     # Get the length of the mask
     if isinstance(mask, slice):
@@ -113,34 +121,43 @@
                 return x.data[mask][0]
             else:
                 return x.fill_value
 
     shape = tuple(shape)
     data = x.data[mask]
 
-    return COO(coords, data, shape=shape,
-               has_duplicates=False,
-               sorted=sorted, fill_value=x.fill_value)
+    return COO(
+        coords,
+        data,
+        shape=shape,
+        has_duplicates=False,
+        sorted=sorted,
+        fill_value=x.fill_value,
+    )
 
 
 def _mask(coords, indices, shape):
     indices = _prune_indices(indices, shape)
     indices, adv_idx, adv_idx_pos = _separate_adv_indices(indices)
 
     if len(adv_idx) != 0:
         if len(adv_idx) != 1:
-            raise IndexError('Only indices with at most one iterable index are supported.')
+            raise IndexError(
+                "Only indices with at most one iterable index are supported."
+            )
 
         adv_idx = adv_idx[0]
         adv_idx_pos = adv_idx_pos[0]
 
         if adv_idx.ndim != 1:
-            raise IndexError('Only one-dimensional iterable indices supported.')
+            raise IndexError("Only one-dimensional iterable indices supported.")
 
-        mask, aidxs = _compute_multi_mask(coords, _ind_ar_from_indices(indices), adv_idx, adv_idx_pos)
+        mask, aidxs = _compute_multi_mask(
+            coords, _ind_ar_from_indices(indices), adv_idx, adv_idx_pos
+        )
         return mask, _AdvIdxInfo(aidxs, adv_idx_pos, len(adv_idx))
 
     mask, is_slice = _compute_mask(coords, _ind_ar_from_indices(indices))
 
     if is_slice:
         return slice(mask[0], mask[1], 1), None
     else:
@@ -284,15 +301,15 @@
         The advanced array index.
     """
     mask = numba.typed.List.empty_list(numba.types.intp)
     a_indices = numba.typed.List.empty_list(numba.types.intp)
     full_idx = np.empty((len(indices) + 1, 3), dtype=np.intp)
 
     full_idx[:adv_idx_pos] = indices[:adv_idx_pos]
-    full_idx[adv_idx_pos + 1:] = indices[adv_idx_pos:]
+    full_idx[adv_idx_pos + 1 :] = indices[adv_idx_pos:]
 
     for i, aidx in enumerate(adv_idx):
         full_idx[adv_idx_pos] = [aidx, aidx + 1, 1]
         partial_mask, is_slice = _compute_mask(coords, full_idx)
         if is_slice:
             slice_mask = numba.typed.List.empty_list(numba.types.intp)
             for j in range(partial_mask[0], partial_mask[1]):
@@ -373,17 +390,21 @@
     while i < len(indices):
         # Guesstimate whether working with pairs is more efficient or
         # working with the mask directly.
         # One side is the estimate of time taken for binary searches
         # (n_searches * log(avg_length))
         # The other is an estimated time of a linear filter for the mask.
         n_pairs = len(starts)
-        n_current_slices = len(range(indices[i, 0], indices[i, 1], indices[i, 2])) * n_pairs + 2
-        if n_current_slices * np.log(n_current_slices / max(n_pairs, 1)) > \
-                n_matches + n_pairs:
+        n_current_slices = (
+            len(range(indices[i, 0], indices[i, 1], indices[i, 2])) * n_pairs + 2
+        )
+        if (
+            n_current_slices * np.log(n_current_slices / max(n_pairs, 1))
+            > n_matches + n_pairs
+        ):
             break
 
         # For each of the pairs, search inside the coordinates for other
         # matching sub-pairs.
         # This gets the start-end coordinates in coords for each 'sub-array'
         # Which would come out of indexing a single integer.
         starts, stops, n_matches = _get_mask_pairs(starts, stops, coords[i], indices[i])
@@ -445,16 +466,22 @@
     stops = numba.typed.List.empty_list(numba.types.intp)
     n_matches = np.intp(0)
 
     for j in range(len(starts_old)):
         # For each matching "integer" in the slice, search within the "sub-coords"
         # Using binary search.
         for p_match in range(idx[0], idx[1], idx[2]):
-            start = np.searchsorted(c[starts_old[j]:stops_old[j]], p_match, side='left') + starts_old[j]
-            stop = np.searchsorted(c[starts_old[j]:stops_old[j]], p_match, side='right') + starts_old[j]
+            start = (
+                np.searchsorted(c[starts_old[j] : stops_old[j]], p_match, side="left")
+                + starts_old[j]
+            )
+            stop = (
+                np.searchsorted(c[starts_old[j] : stops_old[j]], p_match, side="right")
+                + starts_old[j]
+            )
 
             if start != stop:
                 starts.append(start)
                 stops.append(stop)
                 n_matches += stop - start
 
     return starts, stops, n_matches
@@ -500,17 +527,18 @@
             match = True
 
             # Check if it matches all indices
             for k in range(len(indices)):
                 idx = indices[k]
                 elem = coords[k, j]
 
-                match &= ((elem - idx[0]) % idx[2] == 0 and
-                          ((idx[2] > 0 and idx[0] <= elem < idx[1]) or
-                           (idx[2] < 0 and idx[0] >= elem > idx[1])))
+                match &= (elem - idx[0]) % idx[2] == 0 and (
+                    (idx[2] > 0 and idx[0] <= elem < idx[1])
+                    or (idx[2] < 0 and idx[0] >= elem > idx[1])
+                )
 
             # and append to the mask if so.
             if match:
                 mask.append(j)
 
     return mask
```

### Comparing `sparse-0.8.0/sparse/_coo/umath.py` & `sparse-0.9.1/sparse/_coo/umath.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,17 +111,18 @@
     """
     result_shape = ()
 
     for shape in shapes:
         try:
             result_shape = _get_broadcast_shape(shape, result_shape)
         except ValueError:
-            shapes_str = ', '.join(str(shape) for shape in shapes)
-            raise ValueError('operands could not be broadcast together with shapes %s'
-                             % shapes_str)
+            shapes_str = ", ".join(str(shape) for shape in shapes)
+            raise ValueError(
+                "operands could not be broadcast together with shapes %s" % shapes_str
+            )
 
     return result_shape
 
 
 def _get_broadcast_shape(shape1, shape2, is_result=False):
     """
     Get the overall broadcasted shape.
@@ -140,21 +141,27 @@
 
     Raises
     ------
     ValueError
         If the two shapes cannot be broadcast together.
     """
     # https://stackoverflow.com/a/47244284/774273
-    if not all((l1 == l2) or (l1 == 1) or ((l2 == 1) and not is_result) for l1, l2 in
-               zip(shape1[::-1], shape2[::-1])):
-        raise ValueError('operands could not be broadcast together with shapes %s, %s' %
-                         (shape1, shape2))
+    if not all(
+        (l1 == l2) or (l1 == 1) or ((l2 == 1) and not is_result)
+        for l1, l2 in zip(shape1[::-1], shape2[::-1])
+    ):
+        raise ValueError(
+            "operands could not be broadcast together with shapes %s, %s"
+            % (shape1, shape2)
+        )
 
-    result_shape = tuple(l1 if l1 != 1 else l2 for l1, l2 in
-                         zip_longest(shape1[::-1], shape2[::-1], fillvalue=1))[::-1]
+    result_shape = tuple(
+        l1 if l1 != 1 else l2
+        for l1, l2 in zip_longest(shape1[::-1], shape2[::-1], fillvalue=1)
+    )[::-1]
 
     return result_shape
 
 
 def _get_broadcast_parameters(shape, broadcast_shape):
     """
     Get the broadcast parameters.
@@ -168,16 +175,18 @@
 
     Returns
     -------
     params : list
         A list containing None if the dimension isn't in the original array, False if
         it needs to be broadcast, and True if it doesn't.
     """
-    params = [None if l1 is None else l1 == l2 for l1, l2
-              in zip_longest(shape[::-1], broadcast_shape[::-1], fillvalue=None)][::-1]
+    params = [
+        None if l1 is None else l1 == l2
+        for l1, l2 in zip_longest(shape[::-1], broadcast_shape[::-1], fillvalue=None)
+    ][::-1]
 
     return params
 
 
 def _get_reduced_coords(coords, params):
     """
     Gets only those dimensions of the coordinates that don't need to be broadcast.
@@ -375,19 +384,27 @@
 
     result_shape = _get_broadcast_shape(x.shape, shape, is_result=True)
     params = _get_broadcast_parameters(x.shape, result_shape)
     coords, data = _get_expanded_coords_data(x.coords, x.data, params, result_shape)
 
     # Check if all the non-broadcast axes are next to each other
     nonbroadcast_idx = [idx for idx, p in enumerate(params) if p]
-    diff_nonbroadcast_idx = [a - b for a, b in zip(nonbroadcast_idx[1:], nonbroadcast_idx[:-1])]
+    diff_nonbroadcast_idx = [
+        a - b for a, b in zip(nonbroadcast_idx[1:], nonbroadcast_idx[:-1])
+    ]
     sorted = all(d == 1 for d in diff_nonbroadcast_idx)
 
-    return COO(coords, data, shape=result_shape, has_duplicates=False,
-               sorted=sorted, fill_value=x.fill_value)
+    return COO(
+        coords,
+        data,
+        shape=result_shape,
+        has_duplicates=False,
+        sorted=sorted,
+        fill_value=x.fill_value,
+    )
 
 
 class _Elemwise:
     def __init__(self, func, *args, **kwargs):
         """
         Initialize the element-wise function calculator.
 
@@ -417,86 +434,116 @@
                 self.args = None
                 return
             else:
                 processed_args.append(arg)
 
         self.args = tuple(processed_args)
         self.func = func
-        self.dtype = kwargs.pop('dtype', None)
+        self.dtype = kwargs.pop("dtype", None)
         self.kwargs = kwargs
         self.cache = {}
 
         self._check_broadcast()
         self._get_fill_value()
 
     def get_result(self):
         from .core import COO
+
         if self.args is None:
             return NotImplemented
 
         if self.shape == self.ndarray_shape:
             args = [a.todense() if isinstance(a, COO) else a for a in self.args]
             return self.func(*args, **self.kwargs)
 
         if any(s == 0 for s in self.shape):
             data = np.empty((0,), dtype=self.fill_value.dtype)
             coords = np.empty((0, len(self.shape)), dtype=np.intp)
-            return COO(coords, data, shape=self.shape, has_duplicates=False, fill_value=self.fill_value)
+            return COO(
+                coords,
+                data,
+                shape=self.shape,
+                has_duplicates=False,
+                fill_value=self.fill_value,
+            )
 
         data_list = []
         coords_list = []
 
-        for mask in itertools.product(*[[True, False] if isinstance(arg, COO)
-                                        else [None] for arg in self.args]):
+        for mask in itertools.product(
+            *[[True, False] if isinstance(arg, COO) else [None] for arg in self.args]
+        ):
             if not any(mask):
                 continue
 
             r = self._get_func_coords_data(mask)
 
             if r is not None:
                 coords_list.append(r[0])
                 data_list.append(r[1])
 
         # Concatenate matches and mismatches
-        data = np.concatenate(data_list) if len(data_list) else np.empty((0,), dtype=self.fill_value.dtype)
-        coords = np.concatenate(coords_list, axis=1) if len(coords_list) else \
-            np.empty((0, len(self.shape)), dtype=np.intp)
+        data = (
+            np.concatenate(data_list)
+            if len(data_list)
+            else np.empty((0,), dtype=self.fill_value.dtype)
+        )
+        coords = (
+            np.concatenate(coords_list, axis=1)
+            if len(coords_list)
+            else np.empty((0, len(self.shape)), dtype=np.intp)
+        )
 
-        return COO(coords, data, shape=self.shape, has_duplicates=False, fill_value=self.fill_value)
+        return COO(
+            coords,
+            data,
+            shape=self.shape,
+            has_duplicates=False,
+            fill_value=self.fill_value,
+        )
 
     def _get_fill_value(self):
         """
         A function that finds and returns the fill-value.
 
         Raises
         ------
         ValueError
             If the fill-value is inconsistent.
         """
         from .core import COO
 
-        zero_args = tuple(arg.fill_value[...] if isinstance(arg, COO) else arg for arg in self.args)
+        zero_args = tuple(
+            arg.fill_value[...] if isinstance(arg, COO) else arg for arg in self.args
+        )
 
         # Some elemwise functions require a dtype argument, some abhorr it.
         try:
             fill_value_array = self.func(*zero_args, dtype=self.dtype, **self.kwargs)
             self.dtype = None
         except TypeError:
             fill_value_array = self.func(*zero_args, **self.kwargs)
 
         try:
             fill_value = fill_value_array[(0,) * fill_value_array.ndim]
         except IndexError:
             zero_args = tuple(
-                arg.fill_value if isinstance(arg, COO) else _zero_of_dtype(arg.dtype) for arg in self.args)
+                arg.fill_value if isinstance(arg, COO) else _zero_of_dtype(arg.dtype)
+                for arg in self.args
+            )
             fill_value = self.func(*zero_args, **self.kwargs)[()]
 
-        if not equivalent(fill_value, fill_value_array).all() and self.shape != self.ndarray_shape:
-            raise ValueError('Performing a mixed sparse-dense operation that would result in a dense array. '
-                             'Please make sure that func(sparse_fill_values, ndarrays) is a constant array.')
+        if (
+            not equivalent(fill_value, fill_value_array).all()
+            and self.shape != self.ndarray_shape
+        ):
+            raise ValueError(
+                "Performing a mixed sparse-dense operation that would result in a dense array. "
+                "Please make sure that func(sparse_fill_values, ndarrays) is a constant array."
+            )
 
         # Store dtype separately if needed.
         if self.dtype is not None:
             fill_value = fill_value.astype(self.dtype)
 
         self.fill_value = fill_value
         self.dtype = self.fill_value.dtype
@@ -507,25 +554,28 @@
 
         Raises
         ------
         ValueError
             If the check fails.
         """
         from .core import COO
+
         full_shape = _get_nary_broadcast_shape(*tuple(arg.shape for arg in self.args))
         non_ndarray_shape = _get_nary_broadcast_shape(
             *tuple(arg.shape for arg in self.args if isinstance(arg, COO))
         )
         ndarray_shape = _get_nary_broadcast_shape(
             *tuple(arg.shape for arg in self.args if isinstance(arg, np.ndarray))
         )
 
         if full_shape != non_ndarray_shape:
-            raise ValueError('Please make sure that the broadcast shape of just the sparse arrays is '
-                             'the same as the broadcast shape of all the operands.')
+            raise ValueError(
+                "Please make sure that the broadcast shape of just the sparse arrays is "
+                "the same as the broadcast shape of all the operands."
+            )
 
         self.shape = full_shape
         self.ndarray_shape = ndarray_shape
         self.non_ndarray_shape = non_ndarray_shape
 
     def _get_func_coords_data(self, mask):
         """
@@ -540,31 +590,37 @@
         -------
         None or tuple
             The coords/data tuple for the given mask.
         """
         from .core import COO
 
         matched_args = [arg for arg, m in zip(self.args, mask) if m is not None and m]
-        unmatched_args = [arg for arg, m in zip(self.args, mask) if m is not None and not m]
+        unmatched_args = [
+            arg for arg, m in zip(self.args, mask) if m is not None and not m
+        ]
         ndarray_args = [arg for arg, m in zip(self.args, mask) if m is None]
 
         matched_broadcast_shape = _get_nary_broadcast_shape(
             *tuple(arg.shape for arg in itertools.chain(matched_args, ndarray_args))
         )
 
-        matched_arrays = self._match_coo(*matched_args,
-                                         cache=self.cache,
-                                         broadcast_shape=matched_broadcast_shape)
+        matched_arrays = self._match_coo(
+            *matched_args, cache=self.cache, broadcast_shape=matched_broadcast_shape
+        )
 
         func_args = []
 
         m_arg = 0
         for arg, m in zip(self.args, mask):
             if m is None:
-                func_args.append(np.broadcast_to(arg, matched_broadcast_shape)[tuple(matched_arrays[0].coords)])
+                func_args.append(
+                    np.broadcast_to(arg, matched_broadcast_shape)[
+                        tuple(matched_arrays[0].coords)
+                    ]
+                )
                 continue
 
             if m:
                 func_args.append(matched_arrays[m_arg].data)
                 m_arg += 1
             else:
                 func_args.append(arg.fill_value)
@@ -586,30 +642,34 @@
             return None
 
         func_coords = matched_arrays[0].coords[:, unmatched_mask]
         func_data = func_data[unmatched_mask]
 
         if matched_arrays[0].shape != self.shape:
             params = _get_broadcast_parameters(matched_arrays[0].shape, self.shape)
-            func_coords, func_data = _get_expanded_coords_data(func_coords, func_data, params, self.shape)
+            func_coords, func_data = _get_expanded_coords_data(
+                func_coords, func_data, params, self.shape
+            )
 
         if all(m is None or m for m in mask):
             return func_coords, func_data
 
         # Not really sorted but we need the sortedness.
-        func_array = COO(func_coords, func_data, self.shape, has_duplicates=False, sorted=True)
+        func_array = COO(
+            func_coords, func_data, self.shape, has_duplicates=False, sorted=True
+        )
 
         unmatched_mask = np.ones(func_array.nnz, dtype=np.bool)
 
         for arg in unmatched_args:
             matched_idx = self._match_coo(func_array, arg, return_midx=True)[0]
             unmatched_mask[matched_idx] = False
 
-        coords = np.asarray(func_array.coords[:, unmatched_mask], order='C')
-        data = np.asarray(func_array.data[unmatched_mask], order='C')
+        coords = np.asarray(func_array.coords[:, unmatched_mask], order="C")
+        data = np.asarray(func_array.data[unmatched_mask], order="C")
 
         return coords, data
 
     @staticmethod
     def _match_coo(*args, **kwargs):
         """
         Matches the coordinates for any number of input :obj:`COO` arrays.
@@ -633,78 +693,97 @@
         matched_arrays : List[COO]
             The expanded, matched :obj:`COO` objects. Only returned if
             ``return_midx`` is ``False``.
         """
         from .core import COO
         from .common import linear_loc
 
-        cache = kwargs.pop('cache', None)
-        return_midx = kwargs.pop('return_midx', False)
-        broadcast_shape = kwargs.pop('broadcast_shape', None)
+        cache = kwargs.pop("cache", None)
+        return_midx = kwargs.pop("return_midx", False)
+        broadcast_shape = kwargs.pop("broadcast_shape", None)
 
         if kwargs:
-            raise ValueError('Unknown kwargs: {}'.format(kwargs.keys()))
+            raise ValueError("Unknown kwargs: {}".format(kwargs.keys()))
 
         if return_midx and (len(args) != 2 or cache is not None):
-            raise NotImplementedError('Matching indices only supported for two args, and no cache.')
+            raise NotImplementedError(
+                "Matching indices only supported for two args, and no cache."
+            )
 
         matched_arrays = [args[0]]
         cache_key = [id(args[0])]
         for arg2 in args[1:]:
             cache_key.append(id(arg2))
             key = tuple(cache_key)
             if cache is not None and key in cache:
                 matched_arrays = cache[key]
                 continue
 
             cargs = [matched_arrays[0], arg2]
             current_shape = _get_broadcast_shape(matched_arrays[0].shape, arg2.shape)
-            params = [_get_broadcast_parameters(arg.shape, current_shape) for arg in cargs]
+            params = [
+                _get_broadcast_parameters(arg.shape, current_shape) for arg in cargs
+            ]
             reduced_params = [all(p) for p in zip(*params)]
-            reduced_shape = _get_reduced_shape(arg2.shape,
-                                               _rev_idx(reduced_params, arg2.ndim))
+            reduced_shape = _get_reduced_shape(
+                arg2.shape, _rev_idx(reduced_params, arg2.ndim)
+            )
 
-            reduced_coords = [_get_reduced_coords(arg.coords, _rev_idx(reduced_params, arg.ndim))
-                              for arg in cargs]
+            reduced_coords = [
+                _get_reduced_coords(arg.coords, _rev_idx(reduced_params, arg.ndim))
+                for arg in cargs
+            ]
 
             linear = [linear_loc(rc, reduced_shape) for rc in reduced_coords]
             sorted_idx = [np.argsort(idx) for idx in linear]
             linear = [idx[s] for idx, s in zip(linear, sorted_idx)]
             matched_idx = _match_arrays(*linear)
 
             if return_midx:
-                matched_idx = [sidx[midx] for sidx, midx in zip(sorted_idx, matched_idx)]
+                matched_idx = [
+                    sidx[midx] for sidx, midx in zip(sorted_idx, matched_idx)
+                ]
                 return matched_idx
 
             coords = [arg.coords[:, s] for arg, s in zip(cargs, sorted_idx)]
             mcoords = [c[:, idx] for c, idx in zip(coords, matched_idx)]
             mcoords = _get_matching_coords(mcoords, params)
             mdata = [arg.data[sorted_idx[0]][matched_idx[0]] for arg in matched_arrays]
             mdata.append(arg2.data[sorted_idx[1]][matched_idx[1]])
             # The coords aren't truly sorted, but we don't need them, so it's
             # best to avoid the extra cost.
             matched_arrays = [
                 COO(mcoords, md, shape=current_shape, sorted=True, has_duplicates=False)
-                for md in mdata]
+                for md in mdata
+            ]
 
             if cache is not None:
                 cache[key] = matched_arrays
 
         if broadcast_shape is not None and matched_arrays[0].shape != broadcast_shape:
             params = _get_broadcast_parameters(matched_arrays[0].shape, broadcast_shape)
             coords, idx = _get_expanded_coords_data(
-                matched_arrays[0].coords, np.arange(matched_arrays[0].nnz), params, broadcast_shape
+                matched_arrays[0].coords,
+                np.arange(matched_arrays[0].nnz),
+                params,
+                broadcast_shape,
             )
 
             matched_arrays = [
-                COO(coords, arr.data[idx], shape=broadcast_shape, sorted=True, has_duplicates=False)
+                COO(
+                    coords,
+                    arr.data[idx],
+                    shape=broadcast_shape,
+                    sorted=True,
+                    has_duplicates=False,
+                )
                 for arr in matched_arrays
             ]
 
         return matched_arrays
 
 
 def _rev_idx(arg, idx):
     if idx == 0:
-        return arg[len(arg):]
+        return arg[len(arg) :]
 
     return arg[-idx:]
```

### Comparing `sparse-0.8.0/sparse/_dok.py` & `sparse-0.9.1/sparse/_dok.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     >>> s6 = DOK((5, 5, 5), values)
     >>> s6
     <DOK: shape=(5, 5, 5), dtype=int64, nnz=1, fill_value=0.0>
     """
 
     def __init__(self, shape, data=None, dtype=None, fill_value=None):
         from ._coo import COO
+
         self.data = dict()
 
         if isinstance(shape, COO):
             ar = DOK.from_coo(shape)
             self._make_shallow_copy_of(ar)
             return
 
@@ -108,22 +109,24 @@
             data = dict()
 
         super().__init__(shape, fill_value=fill_value)
 
         if isinstance(data, dict):
             if not dtype:
                 if not len(data):
-                    self.dtype = np.dtype('float64')
+                    self.dtype = np.dtype("float64")
                 else:
-                    self.dtype = np.result_type(*map(lambda x: np.asarray(x).dtype, data.values()))
+                    self.dtype = np.result_type(
+                        *map(lambda x: np.asarray(x).dtype, data.values())
+                    )
 
             for c, d in data.items():
                 self[c] = d
         else:
-            raise ValueError('data must be a dict.')
+            raise ValueError("data must be a dict.")
 
     def _make_shallow_copy_of(self, other):
         self.dtype = other.dtype
         self.data = other.data
         super().__init__(other.shape, fill_value=other.fill_value)
 
     @classmethod
@@ -172,14 +175,15 @@
         >>> s
         <DOK: shape=(5, 5), dtype=float64, nnz=4, fill_value=0.0>
         >>> s2 = s.to_coo()
         >>> s2
         <COO: shape=(5, 5), dtype=float64, nnz=4, fill_value=0.0>
         """
         from ._coo import COO
+
         return COO(self)
 
     @classmethod
     def from_numpy(cls, x):
         """
         Get a :obj:`DOK` array from a Numpy array.
 
@@ -238,21 +242,23 @@
         """
         return len(self.data)
 
     def __getitem__(self, key):
         key = normalize_index(key, self.shape)
 
         if not all(isinstance(i, Integral) for i in key):
-            raise NotImplementedError('All indices must be integers'
-                                      ' when getting an item.')
+            raise NotImplementedError(
+                "All indices must be integers" " when getting an item."
+            )
 
         if len(key) != self.ndim:
-            raise NotImplementedError('Can only get single elements. '
-                                      'Expected key of length %d, got %s'
-                                      % (self.ndim, str(key)))
+            raise NotImplementedError(
+                "Can only get single elements. "
+                "Expected key of length %d, got %s" % (self.ndim, str(key))
+            )
 
         key = tuple(int(k) for k in key)
 
         if key in self.data:
             return self.data[key]
         else:
             return self.fill_value
@@ -264,18 +270,20 @@
         value = value.astype(self.dtype)
 
         key_list = [int(k) if isinstance(k, Integral) else k for k in key]
 
         self._setitem(key_list, value)
 
     def _setitem(self, key_list, value):
-        value_missing_dims = len([ind for ind in key_list if isinstance(ind, slice)]) - value.ndim
+        value_missing_dims = (
+            len([ind for ind in key_list if isinstance(ind, slice)]) - value.ndim
+        )
 
         if value_missing_dims < 0:
-            raise ValueError('setting an array element with a sequence.')
+            raise ValueError("setting an array element with a sequence.")
 
         for i, ind in enumerate(key_list):
             if isinstance(ind, slice):
                 step = ind.step if ind.step is not None else 1
                 if step > 0:
                     start = ind.start if ind.start is not None else 0
                     start = max(start, 0)
@@ -290,31 +298,35 @@
                     stop = max(stop, -1)
                     if start < stop:
                         start = stop
 
                 key_list_temp = key_list[:]
                 for v_idx, ki in enumerate(range(start, stop, step)):
                     key_list_temp[i] = ki
-                    vi = value if value_missing_dims > 0 else \
-                        (value[0] if value.shape[0] == 1 else value[v_idx])
+                    vi = (
+                        value
+                        if value_missing_dims > 0
+                        else (value[0] if value.shape[0] == 1 else value[v_idx])
+                    )
                     self._setitem(key_list_temp, vi)
 
                 return
             elif not isinstance(ind, Integral):
-                raise IndexError('All indices must be slices or integers'
-                                 ' when setting an item.')
+                raise IndexError(
+                    "All indices must be slices or integers" " when setting an item."
+                )
 
         key = tuple(key_list)
         if not equivalent(value, self.fill_value):
             self.data[key] = value[()]
         elif key in self.data:
             del self.data[key]
 
     def __str__(self):
-        return '<DOK: shape={!s}, dtype={!s}, nnz={:d}, fill_value={!s}>'.format(
+        return "<DOK: shape={!s}, dtype={!s}, nnz={:d}, fill_value={!s}>".format(
             self.shape, self.dtype, self.nnz, self.fill_value
         )
 
     __repr__ = __str__
 
     def todense(self):
         """
@@ -363,15 +375,18 @@
             The converted array.
 
         Raises
         ------
         NotImplementedError
             If the format isn't supported.
         """
-        if format == 'dok' or format is DOK:
+        if format == "dok" or format is DOK:
             return self
 
         from ._coo import COO
-        if format == 'coo' or format is COO:
-            return COO.from_iter(self.data, shape=self.shape, fill_value=self.fill_value)
 
-        raise NotImplementedError('The given format is not supported.')
+        if format == "coo" or format is COO:
+            return COO.from_iter(
+                self.data, shape=self.shape, fill_value=self.fill_value
+            )
+
+        raise NotImplementedError("The given format is not supported.")
```

### Comparing `sparse-0.8.0/sparse/_io.py` & `sparse-0.9.1/sparse/_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,18 @@
     scipy.sparse.load_npz
     numpy.savez
     numpy.load
 
     """
 
     nodes = {
-        'data': matrix.data,
-        'coords': matrix.coords,
-        'shape': matrix.shape,
-        'fill_value': matrix.fill_value,
+        "data": matrix.data,
+        "coords": matrix.coords,
+        "shape": matrix.shape,
+        "fill_value": matrix.fill_value,
     }
 
     if compressed:
         np.savez_compressed(filename, **nodes)
     else:
         np.savez(filename, **nodes)
 
@@ -88,15 +88,23 @@
     numpy.savez
     numpy.load
 
     """
 
     with np.load(filename) as fp:
         try:
-            coords = fp['coords']
-            data = fp['data']
-            shape = tuple(fp['shape'])
-            fill_value = fp['fill_value'][()]
-            return COO(coords=coords, data=data, shape=shape, sorted=True, has_duplicates=False,
-                       fill_value=fill_value)
+            coords = fp["coords"]
+            data = fp["data"]
+            shape = tuple(fp["shape"])
+            fill_value = fp["fill_value"][()]
+            return COO(
+                coords=coords,
+                data=data,
+                shape=shape,
+                sorted=True,
+                has_duplicates=False,
+                fill_value=fill_value,
+            )
         except KeyError:
-            raise RuntimeError('The file {!s} does not contain a valid sparse matrix'.format(filename))
+            raise RuntimeError(
+                "The file {!s} does not contain a valid sparse matrix".format(filename)
+            )
```

### Comparing `sparse-0.8.0/sparse/_slicing.py` & `sparse-0.9.1/sparse/_slicing.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     (slice(0, 10, 1), None)
     """
     if not isinstance(idx, tuple):
         idx = (idx,)
     idx = replace_ellipsis(len(shape), idx)
     n_sliced_dims = 0
     for i in idx:
-        if hasattr(i, 'ndim') and i.ndim >= 1:
+        if hasattr(i, "ndim") and i.ndim >= 1:
             n_sliced_dims += i.ndim
         elif i is None:
             continue
         else:
             n_sliced_dims += 1
     idx = idx + (slice(None),) * (len(shape) - n_sliced_dims)
     if len([i for i in idx if i is not None]) > len(shape):
@@ -75,15 +75,17 @@
     if not isellipsis:
         return index
     elif len(isellipsis) > 1:
         raise IndexError("an index can only have a single ellipsis ('...')")
     else:
         loc = isellipsis[0]
     extra_dimensions = n - (len(index) - sum(i is None for i in index) - 1)
-    return index[:loc] + (slice(None, None, None),) * extra_dimensions + index[loc + 1:]
+    return (
+        index[:loc] + (slice(None, None, None),) * extra_dimensions + index[loc + 1 :]
+    )
 
 
 def check_index(ind, dimension):
     """ Check validity of index for a given dimension
     Examples
     --------
     >>> check_index(3, 5)
@@ -106,28 +108,36 @@
     ...
     IndexError: Index out of bounds for dimension 5
     >>> check_index(slice(0, 3), 5)
     """
     # unknown dimension, assumed to be in bounds
     if isinstance(ind, Iterable):
         x = np.asanyarray(ind)
-        if np.issubdtype(x.dtype, np.integer) and \
-                ((x >= dimension) | (x < -dimension)).any():
+        if (
+            np.issubdtype(x.dtype, np.integer)
+            and ((x >= dimension) | (x < -dimension)).any()
+        ):
             raise IndexError("Index out of bounds for dimension {:d}".format(dimension))
         elif x.dtype == bool and len(x) != dimension:
-            raise IndexError("boolean index did not match indexed array; dimension is {:d} "
-                             "but corresponding boolean dimension is {:d}".format(dimension, len(x)))
+            raise IndexError(
+                "boolean index did not match indexed array; dimension is {:d} "
+                "but corresponding boolean dimension is {:d}".format(dimension, len(x))
+            )
     elif isinstance(ind, slice):
         return
     elif not isinstance(ind, Integral):
-        raise IndexError("only integers, slices (`:`), ellipsis (`...`), numpy.newaxis (`None`) and "
-                         "integer or boolean arrays are valid indices")
+        raise IndexError(
+            "only integers, slices (`:`), ellipsis (`...`), numpy.newaxis (`None`) and "
+            "integer or boolean arrays are valid indices"
+        )
 
     elif ind >= dimension:
-        raise IndexError("Index is not smaller than dimension {:d} >= {:d}".format(ind, dimension))
+        raise IndexError(
+            "Index is not smaller than dimension {:d} >= {:d}".format(ind, dimension)
+        )
 
     elif ind < -dimension:
         msg = "Negative index is not greater than negative dimension {:d} <= -{:d}"
         raise IndexError(msg.format(ind, dimension))
 
 
 def sanitize_index(ind):
@@ -147,31 +157,37 @@
         ...
     IndexError: only integers, slices (`:`), ellipsis (`...`),
     numpy.newaxis (`None`) and integer or boolean arrays are valid indices
     """
     if ind is None:
         return None
     elif isinstance(ind, slice):
-        return slice(_sanitize_index_element(ind.start),
-                     _sanitize_index_element(ind.stop),
-                     _sanitize_index_element(ind.step))
+        return slice(
+            _sanitize_index_element(ind.start),
+            _sanitize_index_element(ind.stop),
+            _sanitize_index_element(ind.step),
+        )
     elif isinstance(ind, Number):
         return _sanitize_index_element(ind)
-    index_array = np.asanyarray(ind)
-    if index_array.dtype == np.bool_:
-        nonzero = np.nonzero(index_array)
+    if not hasattr(ind, "dtype") and len(ind) == 0:
+        ind = np.array([], dtype=np.intp)
+    ind = np.asarray(ind)
+    if ind.dtype == np.bool_:
+        nonzero = np.nonzero(ind)
         if len(nonzero) == 1:
             # If a 1-element tuple, unwrap the element
             nonzero = nonzero[0]
         return np.asanyarray(nonzero)
-    elif np.issubdtype(index_array.dtype, np.integer):
-        return index_array
+    elif np.issubdtype(ind.dtype, np.integer):
+        return ind
     else:
-        raise IndexError("only integers, slices (`:`), ellipsis (`...`), numpy.newaxis (`None`) and "
-                         "integer or boolean arrays are valid indices")
+        raise IndexError(
+            "only integers, slices (`:`), ellipsis (`...`), numpy.newaxis (`None`) and "
+            "integer or boolean arrays are valid indices"
+        )
 
 
 def _sanitize_index_element(ind):
     """Sanitize a one-element index."""
     if ind is None:
         return None
```

### Comparing `sparse-0.8.0/sparse/_sparse_array.py` & `sparse-0.9.1/sparse/_sparse_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from numbers import Integral
 from functools import reduce
 from typing import Callable
 import operator
 
 import numpy as np
 
-from ._utils import _zero_of_dtype
+from ._utils import _zero_of_dtype, html_table
 
 
 class SparseArray:
     """
     An abstract base class for all the sparse array classes.
 
     Attributes
@@ -25,21 +25,23 @@
     __metaclass__ = ABCMeta
 
     def __init__(self, shape, fill_value=None):
         if not isinstance(shape, Iterable):
             shape = (shape,)
 
         if not all(isinstance(l, Integral) and int(l) >= 0 for l in shape):
-            raise ValueError('shape must be an non-negative integer or a tuple '
-                             'of non-negative integers.')
+            raise ValueError(
+                "shape must be an non-negative integer or a tuple "
+                "of non-negative integers."
+            )
 
         self.shape = tuple(int(l) for l in shape)
 
         if fill_value is not None:
-            if not hasattr(fill_value, 'dtype') or fill_value.dtype != self.dtype:
+            if not hasattr(fill_value, "dtype") or fill_value.dtype != self.dtype:
                 self.fill_value = self.dtype.type(fill_value)
             else:
                 self.fill_value = fill_value
         else:
             self.fill_value = _zero_of_dtype(self.dtype)
 
     dtype = None
@@ -154,14 +156,21 @@
         >>> x[0, :] = 1
         >>> s = COO.from_numpy(x)
         >>> s.density
         0.125
         """
         return self.nnz / self.size
 
+    def _repr_html_(self):
+        """
+        Diagnostic report about this array.
+        Renders in Jupyter.
+        """
+        return html_table(self)
+
     @abstractmethod
     def asformat(self, format):
         """
         Convert this sparse array to a given format.
 
         Parameters
         ----------
@@ -204,34 +213,49 @@
         >>> x2 = s.todense()
         >>> np.array_equal(x, x2)
         True
         """
 
     def __array__(self, **kwargs):
         from ._settings import AUTO_DENSIFY
+
         if not AUTO_DENSIFY:
-            raise RuntimeError('Cannot convert a sparse array to dense automatically. '
-                               'To manually densify, use the todense method.')
+            raise RuntimeError(
+                "Cannot convert a sparse array to dense automatically. "
+                "To manually densify, use the todense method."
+            )
 
         return np.asarray(self.todense(), **kwargs)
 
     def __array_function__(self, func, types, args, kwargs):
         import sparse as module
+
+        sparse_func = None
         try:
-            submodules = getattr(func, '__module__', 'numpy').split('.')[1:]
+            submodules = getattr(func, "__module__", "numpy").split(".")[1:]
             for submodule in submodules:
                 module = getattr(module, submodule)
             sparse_func = getattr(module, func.__name__)
         except AttributeError:
             pass
         else:
             return sparse_func(*args, **kwargs)
 
         try:
             sparse_func = getattr(type(self), func.__name__)
         except AttributeError:
-            return NotImplemented
+            pass
 
-        if not isinstance(sparse_func, Callable):
-            return getattr(self, func.__name__)
+        if (
+            not isinstance(sparse_func, Callable)
+            and len(args) == 1
+            and len(kwargs) == 0
+        ):
+            try:
+                return getattr(self, func.__name__)
+            except AttributeError:
+                pass
+
+        if sparse_func is None:
+            return NotImplemented
 
         return sparse_func(*args, **kwargs)
```

### Comparing `sparse-0.8.0/sparse/_utils.py` & `sparse-0.9.1/sparse/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 import functools
 from collections.abc import Iterable
 from numbers import Integral
+from functools import reduce
 
+import operator
 import numpy as np
 
 
 def assert_eq(x, y, check_nnz=True, compare_dtype=True, **kwargs):
     from ._coo import COO
+
     assert x.shape == y.shape
 
     if compare_dtype:
         assert x.dtype == y.dtype
 
-    check_equal = np.array_equal \
-        if np.issubdtype(x.dtype, np.integer) and np.issubdtype(y.dtype, np.integer) \
+    check_equal = (
+        np.array_equal
+        if np.issubdtype(x.dtype, np.integer) and np.issubdtype(y.dtype, np.integer)
         else functools.partial(np.allclose, equal_nan=True)
+    )
 
     if isinstance(x, COO):
         assert is_canonical(x)
     if isinstance(y, COO):
         assert is_canonical(y)
 
     if isinstance(x, COO) and isinstance(y, COO) and check_nnz:
         assert np.array_equal(x.coords, y.coords)
         assert check_equal(x.data, y.data, **kwargs)
         assert x.fill_value == y.fill_value
         return
 
-    if hasattr(x, 'todense'):
+    if hasattr(x, "todense"):
         xx = x.todense()
         if check_nnz:
             assert_nnz(x, xx)
     else:
         xx = x
-    if hasattr(y, 'todense'):
+    if hasattr(y, "todense"):
         yy = y.todense()
         if check_nnz:
             assert_nnz(y, yy)
     else:
         yy = y
     assert check_equal(xx, yy, **kwargs)
 
 
 def assert_nnz(s, x):
-    fill_value = s.fill_value if hasattr(
-        s, 'fill_value') else _zero_of_dtype(s.dtype)
+    fill_value = s.fill_value if hasattr(s, "fill_value") else _zero_of_dtype(s.dtype)
     assert np.sum(~equivalent(x, fill_value)) == s.nnz
 
 
 def is_canonical(x):
-    return not x.shape or ((np.diff(x.linear_loc()) > 0).all() and not equivalent(x.data, x.fill_value).any())
+    return not x.shape or (
+        (np.diff(x.linear_loc()) > 0).all()
+        and not equivalent(x.data, x.fill_value).any()
+    )
 
 
 def _zero_of_dtype(dtype):
     """
     Creates a ()-shaped 0-dimensional zero array of a given dtype.
 
     Parameters
@@ -66,21 +73,21 @@
     np.ndarray
         The zero array.
     """
     return np.zeros((), dtype=dtype)[()]
 
 
 def random(
-        shape,
-        density=0.01,
-        random_state=None,
-        data_rvs=None,
-        format='coo',
-        compressed_axes=None,
-        fill_value=None
+    shape,
+    density=0.01,
+    random_state=None,
+    data_rvs=None,
+    format="coo",
+    compressed_axes=None,
+    fill_value=None,
 ):
     """ Generate a random sparse multidimensional array
 
     Parameters
     ----------
     shape: Tuple[int]
         Shape of the array
@@ -133,17 +140,18 @@
     # See https://github.com/scipy/scipy/blob/master/LICENSE.txt
     from ._coo import COO
 
     elements = np.prod(shape, dtype=np.intp)
 
     nnz = int(elements * density)
 
-    if format != 'gxcs' and compressed_axes is not None:
+    if format != "gcxs" and compressed_axes is not None:
         raise ValueError(
-            'compressed_axes is not supported for {} format'.format(format))
+            "compressed_axes is not supported for {} format".format(format)
+        )
 
     if random_state is None:
         random_state = np.random
     elif isinstance(random_state, Integral):
         random_state = np.random.RandomState(random_state)
     if data_rvs is None:
         data_rvs = random_state.rand
@@ -159,22 +167,22 @@
             while j in selected:
                 j = random_state.randint(elements)
             selected.add(j)
             ind[i] = j
 
     data = data_rvs(nnz)
 
-    ar = COO(ind[None, :], data, shape=elements,
-             fill_value=fill_value).reshape(shape)
+    ar = COO(ind[None, :], data, shape=elements, fill_value=fill_value).reshape(shape)
 
     return ar.asformat(format, compressed_axes=compressed_axes)
 
 
 def isscalar(x):
     from ._sparse_array import SparseArray
+
     return not isinstance(x, SparseArray) and np.isscalar(x)
 
 
 def random_value_array(value, fraction):
     def replace_values(n):
         i = int(n * fraction)
 
@@ -208,16 +216,15 @@
 
     if isinstance(axis, Integral):
         axis = int(axis)
         if axis < 0:
             axis += ndim
 
         if axis >= ndim or axis < 0:
-            raise ValueError(
-                'Invalid axis index %d for ndim=%d' % (axis, ndim))
+            raise ValueError("Invalid axis index %d for ndim=%d" % (axis, ndim))
 
         return axis
 
     if isinstance(axis, Iterable):
         if not all(isinstance(a, Integral) for a in axis):
             raise ValueError("axis %s not understood" % axis)
 
@@ -253,24 +260,111 @@
     True
     >>> equivalent(np.PZERO, np.NZERO)
     True
     """
     x = np.asarray(x)
     y = np.asarray(y)
     # Can't contain NaNs
-    if any(np.issubdtype(x.dtype, t) for t in
-           [np.integer, np.bool_, np.character]):
+    if any(np.issubdtype(x.dtype, t) for t in [np.integer, np.bool_, np.character]):
         return x == y
 
     # Can contain NaNs
     # FIXME: Complex floats and np.void with multiple values can't be compared properly.
     # lgtm [py/comparison-of-identical-expressions]
     return (x == y) | ((x != x) & (y != y))
 
 
+# copied from zarr
+# See https://github.com/zarr-developers/zarr-python/blob/master/zarr/util.py
+def human_readable_size(size):
+    if size < 2 ** 10:
+        return "%s" % size
+    elif size < 2 ** 20:
+        return "%.1fK" % (size / float(2 ** 10))
+    elif size < 2 ** 30:
+        return "%.1fM" % (size / float(2 ** 20))
+    elif size < 2 ** 40:
+        return "%.1fG" % (size / float(2 ** 30))
+    elif size < 2 ** 50:
+        return "%.1fT" % (size / float(2 ** 40))
+    else:
+        return "%.1fP" % (size / float(2 ** 50))
+
+
+def html_table(arr):
+    table = "<table>"
+    table += "<tbody>"
+    headings = ["Format", "Data Type", "Shape", "nnz", "Density", "Read-only"]
+    info = [
+        type(arr).__name__.lower(),
+        str(arr.dtype),
+        str(arr.shape),
+        str(arr.nnz),
+        str(arr.nnz / arr.size),
+    ]
+
+    # read-only
+    info.append(str(not hasattr(arr, "__setitem__")))
+
+    if hasattr(arr, "nbytes"):
+        headings.append("Size")
+        info.append(human_readable_size(arr.nbytes))
+        headings.append("Storage ratio")
+        info.append(
+            "%.1f"
+            % (arr.nbytes / (reduce(operator.mul, arr.shape, 1) * arr.dtype.itemsize))
+        )
+
+    # compressed_axes
+    if type(arr).__name__ == "GCXS":
+        headings.append("Compressed Axes")
+        info.append(str(arr.compressed_axes))
+
+    for h, i in zip(headings, info):
+        table += (
+            "<tr>"
+            '<th style="text-align: left">%s</th>'
+            '<td style="text-align: left">%s</td>'
+            "</tr>" % (h, i)
+        )
+    table += "</tbody>"
+    table += "</table>"
+    return table
+
+
+def check_compressed_axes(ndim, compressed_axes):
+    """
+    Checks if the given compressed_axes are compatible with the shape of the array.
+
+    Parameters
+    ----------
+    shape : int
+    compressed_axes : Iterable
+
+    Raises
+    ------
+    ValueError
+        If the compressed_axes are incompatible with the number of dimensions     
+    """
+    if compressed_axes is None:
+        pass
+    if isinstance(ndim, Iterable):
+        ndim = len(ndim)
+    if not isinstance(compressed_axes, Iterable):
+        raise ValueError("compressed_axes must be an iterable")
+    if len(compressed_axes) == ndim:
+        raise ValueError("cannot compress all axes")
+    if not np.array_equal(list(set(compressed_axes)), compressed_axes):
+        raise ValueError("axes must be sorted without repeats")
+    if not all(isinstance(a, Integral) for a in compressed_axes):
+        raise ValueError("axes must be represented with integers")
+    if min(compressed_axes) < 0 or max(compressed_axes) >= ndim:
+        raise ValueError("axis out of range")
+
+
 def check_zero_fill_value(*args):
     """
     Checks if all the arguments have zero fill-values.
 
     Parameters
     ----------
     args : Iterable[SparseArray]
@@ -292,18 +386,21 @@
     ValueError: This operation requires zero fill values, but argument 0 had a fill value of 0.5.
     >>> check_zero_fill_value(s1, s2)
     Traceback (most recent call last):
         ...
     ValueError: This operation requires zero fill values, but argument 1 had a fill value of 0.5.
     """
     for i, arg in enumerate(args):
-        if (hasattr(arg, 'fill_value') and
-                not equivalent(arg.fill_value, _zero_of_dtype(arg.dtype))):
-            raise ValueError('This operation requires zero fill values, '
-                             'but argument {:d} had a fill value of {!s}.'.format(i, arg.fill_value))
+        if hasattr(arg, "fill_value") and not equivalent(
+            arg.fill_value, _zero_of_dtype(arg.dtype)
+        ):
+            raise ValueError(
+                "This operation requires zero fill values, "
+                "but argument {:d} had a fill value of {!s}.".format(i, arg.fill_value)
+            )
 
 
 def check_consistent_fill_value(arrays):
     """
     Checks if all the arguments have consistent fill-values.
 
     Parameters
@@ -327,19 +424,21 @@
     ValueError: This operation requires consistent fill-values, but argument 1 had a fill value of 0.5,\
         which is different from a fill_value of 0.1 in the first argument.
     """
     arrays = list(arrays)
     from ._sparse_array import SparseArray
 
     if not all(isinstance(s, SparseArray) for s in arrays):
-        raise ValueError('All arrays must be instances of SparseArray.')
+        raise ValueError("All arrays must be instances of SparseArray.")
     if len(arrays) == 0:
-        raise ValueError('At least one array required.')
+        raise ValueError("At least one array required.")
 
     fv = arrays[0].fill_value
 
     for i, arg in enumerate(arrays):
         if not equivalent(fv, arg.fill_value):
-            raise ValueError('This operation requires consistent fill-values, '
-                             'but argument {:d} had a fill value of {!s}, which '
-                             'is different from a fill_value of {!s} in the first '
-                             'argument.'.format(i, arg.fill_value, fv))
+            raise ValueError(
+                "This operation requires consistent fill-values, "
+                "but argument {:d} had a fill value of {!s}, which "
+                "is different from a fill_value of {!s} in the first "
+                "argument.".format(i, arg.fill_value, fv)
+            )
```

### Comparing `sparse-0.8.0/sparse/tests/test_array_function.py` & `sparse-0.9.1/sparse/tests/test_array_function.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,46 +2,40 @@
 from sparse._settings import NEP18_ENABLED
 from sparse._utils import assert_eq
 import numpy as np
 import pytest
 
 
 if not NEP18_ENABLED:
-    pytest.skip(
-        "NEP18 is not enabled", allow_module_level=True
-    )
+    pytest.skip("NEP18 is not enabled", allow_module_level=True)
 
 
-@pytest.mark.parametrize('func', [
-    np.mean,
-    np.std,
-    np.var,
-    np.sum,
-    lambda x: np.sum(x, axis=0),
-    lambda x: np.transpose(x),
-])
+@pytest.mark.parametrize(
+    "func",
+    [
+        np.mean,
+        np.std,
+        np.var,
+        np.sum,
+        lambda x: np.sum(x, axis=0),
+        lambda x: np.transpose(x),
+    ],
+)
 def test_unary(func):
-    y = sparse.random((50, 50), density=.25)
+    y = sparse.random((50, 50), density=0.25)
     x = y.todense()
     xx = func(x)
     yy = func(y)
     assert_eq(xx, yy)
 
 
-@pytest.mark.parametrize('arg_order', [
-    (0, 1), (1, 0), (1, 1)
-])
-@pytest.mark.parametrize('func', [
-    np.dot,
-    np.result_type,
-    np.tensordot,
-    np.matmul,
-])
+@pytest.mark.parametrize("arg_order", [(0, 1), (1, 0), (1, 1)])
+@pytest.mark.parametrize("func", [np.dot, np.result_type, np.tensordot, np.matmul])
 def test_binary(func, arg_order):
-    y = sparse.random((50, 50), density=.25)
+    y = sparse.random((50, 50), density=0.25)
     x = y.todense()
     xx = func(x, x)
     args = [(x, y)[i] for i in arg_order]
     yy = func(*args)
 
     if isinstance(xx, np.ndarray):
         assert_eq(xx, yy)
@@ -49,33 +43,35 @@
         # result_type returns a dtype
         assert xx == yy
 
 
 def test_stack():
     """stack(), by design, does not allow for mixed type inputs
     """
-    y = sparse.random((50, 50), density=.25)
+    y = sparse.random((50, 50), density=0.25)
     x = y.todense()
     xx = np.stack([x, x])
     yy = np.stack([y, y])
     assert_eq(xx, yy)
 
 
-@pytest.mark.parametrize('arg_order', [
-    (0, 0, 1),
-    (0, 1, 0),
-    (0, 1, 1),
-    (1, 0, 0),
-    (1, 0, 1),
-    (1, 1, 0),
-    (1, 1, 1),
-])
-@pytest.mark.parametrize('func', [
-    lambda a, b, c: np.where(a.astype(bool), b, c),
-])
+@pytest.mark.parametrize(
+    "arg_order",
+    [(0, 0, 1), (0, 1, 0), (0, 1, 1), (1, 0, 0), (1, 0, 1), (1, 1, 0), (1, 1, 1)],
+)
+@pytest.mark.parametrize("func", [lambda a, b, c: np.where(a.astype(bool), b, c)])
 def test_ternary(func, arg_order):
-    y = sparse.random((50, 50), density=.25)
+    y = sparse.random((50, 50), density=0.25)
     x = y.todense()
     xx = func(x, x, x)
     args = [(x, y)[i] for i in arg_order]
     yy = func(*args)
     assert_eq(xx, yy)
+
+
+@pytest.mark.parametrize("func", [np.shape, np.size, np.ndim])
+def test_property(func):
+    y = sparse.random((50, 50), density=0.25)
+    x = y.todense()
+    xx = func(x)
+    yy = func(y)
+    assert xx == yy
```

### Comparing `sparse-0.8.0/sparse/tests/test_coo.py` & `sparse-0.9.1/sparse/tests/test_coo.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,261 +9,269 @@
 
 import sparse
 from sparse import COO
 from sparse._settings import NEP18_ENABLED
 from sparse._utils import assert_eq, random_value_array
 
 
-@pytest.fixture(scope='module', params=['f8', 'f4', 'i8', 'i4'])
+@pytest.fixture(scope="module", params=["f8", "f4", "i8", "i4"])
 def random_sparse(request):
     dtype = request.param
     if np.issubdtype(dtype, np.integer):
+
         def data_rvs(n):
             return np.random.randint(-1000, 1000, n)
+
     else:
         data_rvs = None
-    return sparse.random((20, 30, 40), density=.25, data_rvs=data_rvs).astype(dtype)
+    return sparse.random((20, 30, 40), density=0.25, data_rvs=data_rvs).astype(dtype)
 
 
-@pytest.fixture(scope='module', params=['f8', 'f4', 'i8', 'i4'])
+@pytest.fixture(scope="module", params=["f8", "f4", "i8", "i4"])
 def random_sparse_small(request):
     dtype = request.param
     if np.issubdtype(dtype, np.integer):
+
         def data_rvs(n):
             return np.random.randint(-10, 10, n)
+
     else:
         data_rvs = None
-    return sparse.random((20, 30, 40), density=.25, data_rvs=data_rvs).astype(dtype)
+    return sparse.random((20, 30, 40), density=0.25, data_rvs=data_rvs).astype(dtype)
 
 
-@pytest.mark.parametrize('reduction, kwargs', [
-    ('sum', {}),
-    ('sum', {'dtype': np.float32}),
-    ('prod', {}),
-])
-@pytest.mark.parametrize('axis', [None, 0, 1, 2, (0, 2), -3, (1, -1)])
-@pytest.mark.parametrize('keepdims', [True, False])
+@pytest.mark.parametrize(
+    "reduction, kwargs", [("sum", {}), ("sum", {"dtype": np.float32}), ("prod", {})]
+)
+@pytest.mark.parametrize("axis", [None, 0, 1, 2, (0, 2), -3, (1, -1)])
+@pytest.mark.parametrize("keepdims", [True, False])
 def test_reductions_fv(reduction, random_sparse_small, axis, keepdims, kwargs):
-    x = random_sparse_small + np.random.randint(-1, 1, dtype='i4')
+    x = random_sparse_small + np.random.randint(-1, 1, dtype="i4")
     y = x.todense()
     xx = getattr(x, reduction)(axis=axis, keepdims=keepdims, **kwargs)
     yy = getattr(y, reduction)(axis=axis, keepdims=keepdims, **kwargs)
     assert_eq(xx, yy)
 
 
-@pytest.mark.parametrize('reduction, kwargs', [
-    ('sum', {}),
-    ('sum', {'dtype': np.float32}),
-    ('mean', {}),
-    ('mean', {'dtype': np.float32}),
-    ('prod', {}),
-    ('max', {}),
-    ('min', {}),
-    ('std', {}),
-    ('var', {}),
-])
-@pytest.mark.parametrize('axis', [None, 0, 1, 2, (0, 2), -3, (1, -1)])
-@pytest.mark.parametrize('keepdims', [True, False])
+@pytest.mark.parametrize(
+    "reduction, kwargs",
+    [
+        ("sum", {}),
+        ("sum", {"dtype": np.float32}),
+        ("mean", {}),
+        ("mean", {"dtype": np.float32}),
+        ("prod", {}),
+        ("max", {}),
+        ("min", {}),
+        ("std", {}),
+        ("var", {}),
+    ],
+)
+@pytest.mark.parametrize("axis", [None, 0, 1, 2, (0, 2), -3, (1, -1)])
+@pytest.mark.parametrize("keepdims", [True, False])
 def test_reductions(reduction, random_sparse, axis, keepdims, kwargs):
     x = random_sparse
     y = x.todense()
     xx = getattr(x, reduction)(axis=axis, keepdims=keepdims, **kwargs)
     yy = getattr(y, reduction)(axis=axis, keepdims=keepdims, **kwargs)
     assert_eq(xx, yy)
 
 
-@pytest.mark.xfail(reason=('Setting output dtype=float16 produces results '
-                           'inconsistent with numpy'))
-@pytest.mark.filterwarnings('ignore:overflow')
-@pytest.mark.parametrize('reduction, kwargs', [
-    ('sum', {'dtype': np.float16}),
-    ('mean', {'dtype': np.float16}),
-])
-@pytest.mark.parametrize('axis', [None, 0, 1, 2, (0, 2)])
+@pytest.mark.xfail(
+    reason=("Setting output dtype=float16 produces results " "inconsistent with numpy")
+)
+@pytest.mark.filterwarnings("ignore:overflow")
+@pytest.mark.parametrize(
+    "reduction, kwargs",
+    [("sum", {"dtype": np.float16}), ("mean", {"dtype": np.float16})],
+)
+@pytest.mark.parametrize("axis", [None, 0, 1, 2, (0, 2)])
 def test_reductions_float16(random_sparse, reduction, kwargs, axis):
     x = random_sparse
     y = x.todense()
     xx = getattr(x, reduction)(axis=axis, **kwargs)
     yy = getattr(y, reduction)(axis=axis, **kwargs)
     assert_eq(xx, yy, atol=1e-2)
 
 
-@pytest.mark.parametrize('reduction,kwargs', [
-    ('any', {}),
-    ('all', {}),
-])
-@pytest.mark.parametrize('axis', [None, 0, 1, 2, (0, 2), -3, (1, -1)])
-@pytest.mark.parametrize('keepdims', [True, False])
+@pytest.mark.parametrize("reduction,kwargs", [("any", {}), ("all", {})])
+@pytest.mark.parametrize("axis", [None, 0, 1, 2, (0, 2), -3, (1, -1)])
+@pytest.mark.parametrize("keepdims", [True, False])
 def test_reductions_bool(random_sparse, reduction, kwargs, axis, keepdims):
     y = np.zeros((2, 3, 4), dtype=bool)
     y[0] = True
     y[1, 1, 1] = True
     x = sparse.COO.from_numpy(y)
     xx = getattr(x, reduction)(axis=axis, keepdims=keepdims, **kwargs)
     yy = getattr(y, reduction)(axis=axis, keepdims=keepdims, **kwargs)
     assert_eq(xx, yy)
 
 
-@pytest.mark.parametrize('reduction,kwargs', [
-    (np.max, {}),
-    (np.sum, {}),
-    (np.sum, {'dtype': np.float32}),
-    (np.mean, {}),
-    (np.mean, {'dtype': np.float32}),
-    (np.prod, {}),
-    (np.min, {}),
-])
-@pytest.mark.parametrize('axis', [None, 0, 1, 2, (0, 2), -1, (0, -1)])
-@pytest.mark.parametrize('keepdims', [True, False])
+@pytest.mark.parametrize(
+    "reduction,kwargs",
+    [
+        (np.max, {}),
+        (np.sum, {}),
+        (np.sum, {"dtype": np.float32}),
+        (np.mean, {}),
+        (np.mean, {"dtype": np.float32}),
+        (np.prod, {}),
+        (np.min, {}),
+    ],
+)
+@pytest.mark.parametrize("axis", [None, 0, 1, 2, (0, 2), -1, (0, -1)])
+@pytest.mark.parametrize("keepdims", [True, False])
 def test_ufunc_reductions(random_sparse, reduction, kwargs, axis, keepdims):
     x = random_sparse
     y = x.todense()
     xx = reduction(x, axis=axis, keepdims=keepdims, **kwargs)
     yy = reduction(y, axis=axis, keepdims=keepdims, **kwargs)
     assert_eq(xx, yy)
     # If not a scalar/1 element array, must be a sparse array
     if xx.size > 1:
         assert isinstance(xx, COO)
 
 
-@pytest.mark.parametrize('reduction,kwargs', [
-    (np.max, {}),
-    (np.sum, {'axis': 0}),
-    (np.prod, {'keepdims': True}),
-    (np.add.reduce, {}),
-    (np.add.reduce, {'keepdims': True}),
-    (np.minimum.reduce, {'axis': 0}),
-])
+@pytest.mark.parametrize(
+    "reduction,kwargs",
+    [
+        (np.max, {}),
+        (np.sum, {"axis": 0}),
+        (np.prod, {"keepdims": True}),
+        (np.add.reduce, {}),
+        (np.add.reduce, {"keepdims": True}),
+        (np.minimum.reduce, {"axis": 0}),
+    ],
+)
 def test_ufunc_reductions_kwargs(reduction, kwargs):
-    x = sparse.random((2, 3, 4), density=.5)
+    x = sparse.random((2, 3, 4), density=0.5)
     y = x.todense()
     xx = reduction(x, **kwargs)
     yy = reduction(y, **kwargs)
     assert_eq(xx, yy)
     # If not a scalar/1 element array, must be a sparse array
     if xx.size > 1:
         assert isinstance(xx, COO)
 
 
-@pytest.mark.parametrize('reduction', [
-    'nansum',
-    'nanmean',
-    'nanprod',
-    'nanmax',
-    'nanmin',
-])
-@pytest.mark.parametrize('axis', [None, 0, 1])
-@pytest.mark.parametrize('keepdims', [False])
-@pytest.mark.parametrize('fraction', [0.25, 0.5, 0.75, 1.0])
-@pytest.mark.filterwarnings('ignore:All-NaN')
-@pytest.mark.filterwarnings('ignore:Mean of empty slice')
+@pytest.mark.parametrize(
+    "reduction", ["nansum", "nanmean", "nanprod", "nanmax", "nanmin"]
+)
+@pytest.mark.parametrize("axis", [None, 0, 1])
+@pytest.mark.parametrize("keepdims", [False])
+@pytest.mark.parametrize("fraction", [0.25, 0.5, 0.75, 1.0])
+@pytest.mark.filterwarnings("ignore:All-NaN")
+@pytest.mark.filterwarnings("ignore:Mean of empty slice")
 def test_nan_reductions(reduction, axis, keepdims, fraction):
-    s = sparse.random((2, 3, 4), data_rvs=random_value_array(np.nan, fraction),
-                      density=.25)
+    s = sparse.random(
+        (2, 3, 4), data_rvs=random_value_array(np.nan, fraction), density=0.25
+    )
     x = s.todense()
     expected = getattr(np, reduction)(x, axis=axis, keepdims=keepdims)
     actual = getattr(sparse, reduction)(s, axis=axis, keepdims=keepdims)
     assert_eq(expected, actual)
 
 
-@pytest.mark.parametrize('reduction', [
-    'nanmax',
-    'nanmin',
-    'nanmean',
-])
-@pytest.mark.parametrize('axis', [None, 0, 1])
+@pytest.mark.parametrize("reduction", ["nanmax", "nanmin", "nanmean"])
+@pytest.mark.parametrize("axis", [None, 0, 1])
 def test_all_nan_reduction_warning(reduction, axis):
     x = random_value_array(np.nan, 1.0)(2 * 3 * 4).reshape(2, 3, 4)
     s = COO.from_numpy(x)
 
     with pytest.warns(RuntimeWarning):
         getattr(sparse, reduction)(s, axis=axis)
 
 
-@pytest.mark.parametrize('axis', [
-    None,
-    (1, 2, 0),
-    (2, 1, 0),
-    (0, 1, 2),
-    (0, 1, -1),
-    (0, -2, -1),
-    (-3, -2, -1),
-])
+@pytest.mark.parametrize(
+    "axis",
+    [None, (1, 2, 0), (2, 1, 0), (0, 1, 2), (0, 1, -1), (0, -2, -1), (-3, -2, -1)],
+)
 def test_transpose(axis):
-    x = sparse.random((2, 3, 4), density=.25)
+    x = sparse.random((2, 3, 4), density=0.25)
     y = x.todense()
     xx = x.transpose(axis)
     yy = y.transpose(axis)
     assert_eq(xx, yy)
 
 
-@pytest.mark.parametrize('axis', [
-    (0, 1),  # too few
-    (0, 1, 2, 3),  # too many
-    (3, 1, 0),  # axis 3 illegal
-    (0, -1, -4),  # axis -4 illegal
-    (0, 0, 1),  # duplicate axis 0
-    (0, -1, 2),  # duplicate axis -1 == 2
-    0.3,  # Invalid type in axis
-    ((0, 1, 2),),  # Iterable inside iterable
-])
+@pytest.mark.parametrize(
+    "axis",
+    [
+        (0, 1),  # too few
+        (0, 1, 2, 3),  # too many
+        (3, 1, 0),  # axis 3 illegal
+        (0, -1, -4),  # axis -4 illegal
+        (0, 0, 1),  # duplicate axis 0
+        (0, -1, 2),  # duplicate axis -1 == 2
+        0.3,  # Invalid type in axis
+        ((0, 1, 2),),  # Iterable inside iterable
+    ],
+)
 def test_transpose_error(axis):
-    x = sparse.random((2, 3, 4), density=.25)
+    x = sparse.random((2, 3, 4), density=0.25)
 
     with pytest.raises(ValueError):
         x.transpose(axis)
 
 
-@pytest.mark.parametrize('a,b', [
-    [(3, 4), (5, 5)],
-    [(12,), (3, 4)],
-    [(12,), (3, 6)],
-    [(5, 5, 5), (6, 6, 6)],
-    [(3, 4), (9, 4)],
-    [(5,), (4,)],
-    [(2, 3, 4, 5), (2, 3, 4, 5, 6)],
-    [(100,), (5, 5)],
-    [(2, 3, 4, 5), (20, 6)],
-    [(), ()],
-])
+@pytest.mark.parametrize(
+    "a,b",
+    [
+        [(3, 4), (5, 5)],
+        [(12,), (3, 4)],
+        [(12,), (3, 6)],
+        [(5, 5, 5), (6, 6, 6)],
+        [(3, 4), (9, 4)],
+        [(5,), (4,)],
+        [(2, 3, 4, 5), (2, 3, 4, 5, 6)],
+        [(100,), (5, 5)],
+        [(2, 3, 4, 5), (20, 6)],
+        [(), ()],
+    ],
+)
 def test_resize(a, b):
     s = sparse.random(a, density=0.5)
     orig_size = s.size
     x = s.todense()
     x = np.resize(x, b)
     s.resize(b)
     temp = x.reshape(x.size)
     temp[orig_size:] = s.fill_value
     assert isinstance(s, sparse.SparseArray)
     assert_eq(x, s)
 
 
-@pytest.mark.parametrize('a,b', [
-    [(3, 4), (3, 4)],
-    [(12,), (3, 4)],
-    [(12,), (3, -1)],
-    [(3, 4), (12,)],
-    [(3, 4), (-1, 4)],
-    [(3, 4), (3, -1)],
-    [(2, 3, 4, 5), (8, 15)],
-    [(2, 3, 4, 5), (24, 5)],
-    [(2, 3, 4, 5), (20, 6)],
-    [(), ()],
-])
+@pytest.mark.parametrize(
+    "a,b",
+    [
+        [(3, 4), (3, 4)],
+        [(12,), (3, 4)],
+        [(12,), (3, -1)],
+        [(3, 4), (12,)],
+        [(3, 4), (-1, 4)],
+        [(3, 4), (3, -1)],
+        [(2, 3, 4, 5), (8, 15)],
+        [(2, 3, 4, 5), (24, 5)],
+        [(2, 3, 4, 5), (20, 6)],
+        [(), ()],
+    ],
+)
 def test_reshape(a, b):
     s = sparse.random(a, density=0.5)
     x = s.todense()
 
     assert_eq(x.reshape(b), s.reshape(b))
 
 
 def test_large_reshape():
     n = 100
     m = 10
-    row = np.arange(n, dtype=np.uint16)  # np.random.randint(0, n, size=n, dtype=np.uint16)
+    row = np.arange(
+        n, dtype=np.uint16
+    )  # np.random.randint(0, n, size=n, dtype=np.uint16)
     col = row % m  # np.random.randint(0, m, size=n, dtype=np.uint16)
     data = np.ones(n, dtype=np.uint8)
 
     x = COO((data, (row, col)), sorted=True, has_duplicates=False)
 
     assert_eq(x, x.reshape(x.shape))
 
@@ -288,132 +296,144 @@
     s = sparse.random((3, 5), density=0.5)
     a = s.to_scipy_sparse()
     b = scipy.sparse.coo_matrix(s.todense())
 
     assert_eq(a, b)
 
 
-@pytest.mark.parametrize('a_shape,b_shape,axes', [
-    [(3, 4), (4, 3), (1, 0)],
-    [(3, 4), (4, 3), (0, 1)],
-    [(3, 4, 5), (4, 3), (1, 0)],
-    [(3, 4), (5, 4, 3), (1, 1)],
-    [(3, 4), (5, 4, 3), ((0, 1), (2, 1))],
-    [(3, 4), (5, 4, 3), ((1, 0), (1, 2))],
-    [(3, 4, 5), (4,), (1, 0)],
-    [(4,), (3, 4, 5), (0, 1)],
-    [(4,), (4,), (0, 0)],
-    [(4,), (4,), 0],
-])
+@pytest.mark.parametrize(
+    "a_shape,b_shape,axes",
+    [
+        [(3, 4), (4, 3), (1, 0)],
+        [(3, 4), (4, 3), (0, 1)],
+        [(3, 4, 5), (4, 3), (1, 0)],
+        [(3, 4), (5, 4, 3), (1, 1)],
+        [(3, 4), (5, 4, 3), ((0, 1), (2, 1))],
+        [(3, 4), (5, 4, 3), ((1, 0), (1, 2))],
+        [(3, 4, 5), (4,), (1, 0)],
+        [(4,), (3, 4, 5), (0, 1)],
+        [(4,), (4,), (0, 0)],
+        [(4,), (4,), 0],
+    ],
+)
 def test_tensordot(a_shape, b_shape, axes):
     sa = sparse.random(a_shape, density=0.5)
     sb = sparse.random(b_shape, density=0.5)
 
     a = sa.todense()
     b = sb.todense()
 
-    assert_eq(np.tensordot(a, b, axes),
-              sparse.tensordot(sa, sb, axes))
+    assert_eq(np.tensordot(a, b, axes), sparse.tensordot(sa, sb, axes))
 
-    assert_eq(np.tensordot(a, b, axes),
-              sparse.tensordot(sa, b, axes))
+    assert_eq(np.tensordot(a, b, axes), sparse.tensordot(sa, b, axes))
 
     # assert isinstance(sparse.tensordot(sa, b, axes), COO)
 
-    assert_eq(np.tensordot(a, b, axes),
-              sparse.tensordot(a, sb, axes))
+    assert_eq(np.tensordot(a, b, axes), sparse.tensordot(a, sb, axes))
 
     # assert isinstance(sparse.tensordot(a, sb, axes), COO)
 
 
 def test_tensordot_empty():
     x1 = np.empty((0, 0, 0))
     x2 = np.empty((0, 0, 0))
     s1 = sparse.COO.from_numpy(x1)
     s2 = sparse.COO.from_numpy(x2)
 
     assert_eq(np.tensordot(x1, x2), sparse.tensordot(s1, s2))
 
 
-@pytest.mark.parametrize('a_shape, b_shape', [
-    ((3, 1, 6, 5), (2, 1, 4, 5, 6)),
-    ((2, 1, 4, 5, 6), (3, 1, 6, 5)),
-    ((1, 1, 5), (3, 5, 6)),
-    ((3, 4, 5), (1, 5, 6)),
-    ((3, 4, 5), (3, 5, 6)),
-    ((3, 4, 5), (5, 6)),
-    ((4, 5), (5, 6)),
-    ((5,), (5, 6)),
-    ((4, 5), (5,)),
-    ((5,), (5,)),
-    ((3, 4), (1, 2, 4, 3)),
-])
+@pytest.mark.parametrize(
+    "a_shape, b_shape",
+    [
+        ((3, 1, 6, 5), (2, 1, 4, 5, 6)),
+        ((2, 1, 4, 5, 6), (3, 1, 6, 5)),
+        ((1, 1, 5), (3, 5, 6)),
+        ((3, 4, 5), (1, 5, 6)),
+        ((3, 4, 5), (3, 5, 6)),
+        ((3, 4, 5), (5, 6)),
+        ((4, 5), (5, 6)),
+        ((5,), (5, 6)),
+        ((4, 5), (5,)),
+        ((5,), (5,)),
+        ((3, 4), (1, 2, 4, 3)),
+    ],
+)
 def test_matmul(a_shape, b_shape):
     sa = sparse.random(a_shape, density=0.5)
     sb = sparse.random(b_shape, density=0.5)
 
     a = sa.todense()
     b = sb.todense()
 
     assert_eq(np.matmul(a, b), sparse.matmul(sa, sb))
     assert_eq(sparse.matmul(sa, b), sparse.matmul(a, sb))
     assert_eq(np.matmul(a, b), sparse.matmul(sa, sb))
 
     if a.ndim == 2 or b.ndim == 2:
         assert_eq(
             np.matmul(a, b),
-            sparse.matmul(scipy.sparse.coo_matrix(a) if a.ndim == 2 else sa,
-                          scipy.sparse.coo_matrix(b) if b.ndim == 2 else sb))
+            sparse.matmul(
+                scipy.sparse.coo_matrix(a) if a.ndim == 2 else sa,
+                scipy.sparse.coo_matrix(b) if b.ndim == 2 else sb,
+            ),
+        )
 
-    if hasattr(operator, 'matmul'):
+    if hasattr(operator, "matmul"):
         assert_eq(operator.matmul(a, b), operator.matmul(sa, sb))
 
 
 def test_matmul_errors():
     with pytest.raises(ValueError):
         sa = sparse.random((3, 4, 5, 6), 0.5)
         sb = sparse.random((3, 6, 5, 6), 0.5)
         sparse.matmul(sa, sb)
 
 
-@pytest.mark.parametrize('a_shape, b_shape', [
-    ((1, 4, 5), (3, 5, 6)),
-    ((3, 4, 5), (1, 5, 6)),
-    ((3, 4, 5), (3, 5, 6)),
-    ((3, 4, 5), (5, 6)),
-    ((4, 5), (5, 6)),
-    ((5,), (5, 6)),
-    ((4, 5), (5,)),
-    ((5,), (5,)),
-])
+@pytest.mark.parametrize(
+    "a_shape, b_shape",
+    [
+        ((1, 4, 5), (3, 5, 6)),
+        ((3, 4, 5), (1, 5, 6)),
+        ((3, 4, 5), (3, 5, 6)),
+        ((3, 4, 5), (5, 6)),
+        ((4, 5), (5, 6)),
+        ((5,), (5, 6)),
+        ((4, 5), (5,)),
+        ((5,), (5,)),
+    ],
+)
 def test_dot(a_shape, b_shape):
     sa = sparse.random(a_shape, density=0.5)
     sb = sparse.random(b_shape, density=0.5)
 
     a = sa.todense()
     b = sb.todense()
 
     assert_eq(a.dot(b), sa.dot(sb))
     assert_eq(np.dot(a, b), sparse.dot(sa, sb))
     assert_eq(sparse.dot(sa, b), sparse.dot(a, sb))
     assert_eq(np.dot(a, b), sparse.dot(sa, sb))
 
-    if hasattr(operator, 'matmul'):
+    if hasattr(operator, "matmul"):
         # Basic equivalences
         assert_eq(operator.matmul(a, b), operator.matmul(sa, sb))
         # Test that SOO's and np.array's combine correctly
         # Not possible due to https://github.com/numpy/numpy/issues/9028
         # assert_eq(eval("a @ sb"), eval("sa @ b"))
 
 
-@pytest.mark.parametrize('a_dense, b_dense, o_type', [
-    (False, False, sparse.SparseArray),
-    (False, True, np.ndarray),
-    (True, False, np.ndarray),
-])
+@pytest.mark.parametrize(
+    "a_dense, b_dense, o_type",
+    [
+        (False, False, sparse.SparseArray),
+        (False, True, np.ndarray),
+        (True, False, np.ndarray),
+    ],
+)
 def test_dot_type(a_dense, b_dense, o_type):
     a = sparse.random((3, 4), density=0.8)
     b = sparse.random((4, 5), density=0.8)
 
     if a_dense:
         a = a.todense()
 
@@ -430,22 +450,22 @@
 
     a = sa.todense()
     b = sb.todense()
 
     la = a.tolist()
     lb = b.tolist()
 
-    if hasattr(operator, 'matmul'):
+    if hasattr(operator, "matmul"):
         # Operations with naive collection (list)
         assert_eq(operator.matmul(la, b), operator.matmul(la, sb))
         assert_eq(operator.matmul(a, lb), operator.matmul(sa, lb))
 
 
-@pytest.mark.parametrize('a_ndim', [1, 2, 3])
-@pytest.mark.parametrize('b_ndim', [1, 2, 3])
+@pytest.mark.parametrize("a_ndim", [1, 2, 3])
+@pytest.mark.parametrize("b_ndim", [1, 2, 3])
 def test_kron(a_ndim, b_ndim):
     a_shape = (2, 3, 4)[:a_ndim]
     b_shape = (5, 6, 7)[:b_ndim]
 
     sa = sparse.random(a_shape, density=0.5)
     a = sa.todense()
     sb = sparse.random(b_shape, density=0.5)
@@ -456,19 +476,17 @@
     assert_eq(sparse.kron(sa, b), sol)
     assert_eq(sparse.kron(a, sb), sol)
 
     with pytest.raises(ValueError):
         assert_eq(sparse.kron(a, b), sol)
 
 
-@pytest.mark.parametrize('a_spmatrix, b_spmatrix', [
-    (True, True),
-    (True, False),
-    (False, True)
-])
+@pytest.mark.parametrize(
+    "a_spmatrix, b_spmatrix", [(True, True), (True, False), (False, True)]
+)
 def test_kron_spmatrix(a_spmatrix, b_spmatrix):
     sa = sparse.random((3, 4), density=0.5)
     a = sa.todense()
     sb = sparse.random((5, 6), density=0.5)
     b = sb.todense()
 
     if a_spmatrix:
@@ -482,50 +500,82 @@
     assert_eq(sparse.kron(sa, b), sol)
     assert_eq(sparse.kron(a, sb), sol)
 
     with pytest.raises(ValueError):
         assert_eq(sparse.kron(a, b), sol)
 
 
-@pytest.mark.parametrize('ndim', [1, 2, 3])
+@pytest.mark.parametrize("ndim", [1, 2, 3])
 def test_kron_scalar(ndim):
     if ndim:
         a_shape = (3, 4, 5)[:ndim]
         sa = sparse.random(a_shape, density=0.5)
         a = sa.todense()
     else:
         sa = a = np.array(6)
     scalar = np.array(5)
 
     sol = np.kron(a, scalar)
     assert_eq(sparse.kron(sa, scalar), sol)
     assert_eq(sparse.kron(scalar, sa), sol)
 
 
-@pytest.mark.parametrize('func', [np.expm1, np.log1p, np.sin, np.tan,
-                                  np.sinh, np.tanh, np.floor, np.ceil,
-                                  np.sqrt, np.conj, np.round, np.rint,
-                                  lambda x: x.astype('int32'), np.conjugate,
-                                  np.conj, lambda x: x.round(decimals=2), abs])
+@pytest.mark.parametrize(
+    "func",
+    [
+        np.expm1,
+        np.log1p,
+        np.sin,
+        np.tan,
+        np.sinh,
+        np.tanh,
+        np.floor,
+        np.ceil,
+        np.sqrt,
+        np.conj,
+        np.round,
+        np.rint,
+        lambda x: x.astype("int32"),
+        np.conjugate,
+        np.conj,
+        lambda x: x.round(decimals=2),
+        abs,
+    ],
+)
 def test_elemwise(func):
     s = sparse.random((2, 3, 4), density=0.5)
     x = s.todense()
 
     fs = func(s)
     assert isinstance(fs, COO)
     assert fs.nnz <= s.nnz
 
     assert_eq(func(x), fs)
 
 
-@pytest.mark.parametrize('func', [np.expm1, np.log1p, np.sin, np.tan,
-                                  np.sinh, np.tanh, np.floor, np.ceil,
-                                  np.sqrt, np.conj,
-                                  np.round, np.rint, np.conjugate,
-                                  np.conj, lambda x, out: x.round(decimals=2, out=out)])
+@pytest.mark.parametrize(
+    "func",
+    [
+        np.expm1,
+        np.log1p,
+        np.sin,
+        np.tan,
+        np.sinh,
+        np.tanh,
+        np.floor,
+        np.ceil,
+        np.sqrt,
+        np.conj,
+        np.round,
+        np.rint,
+        np.conjugate,
+        np.conj,
+        lambda x, out: x.round(decimals=2, out=out),
+    ],
+)
 def test_elemwise_inplace(func):
     s = sparse.random((2, 3, 4), density=0.5)
     x = s.todense()
 
     func(s, out=s)
     func(x, out=x)
     assert isinstance(s, COO)
@@ -556,15 +606,15 @@
     x2 = np.random.rand(5, 1, 1, 1)
 
     with pytest.raises(ValueError):
         s1 * x2
 
 
 def test_elemwise_unsupported():
-    class A():
+    class A:
         pass
 
     s1 = sparse.random((2, 3, 4), density=0.5)
     x2 = A()
 
     with pytest.raises(TypeError):
         s1 + x2
@@ -582,53 +632,54 @@
 
     def func(x1, x2, x3):
         return x1 * x2 * x3
 
     assert_eq(sparse.elemwise(func, s1, s2, x3), func(x1, x2, x3))
 
 
-@pytest.mark.parametrize('func', [
-    operator.mul, operator.add, operator.sub, operator.gt,
-    operator.lt, operator.ne
-])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize(
+    "func",
+    [operator.mul, operator.add, operator.sub, operator.gt, operator.lt, operator.ne],
+)
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_elemwise_binary(func, shape):
     xs = sparse.random(shape, density=0.5)
     ys = sparse.random(shape, density=0.5)
 
     x = xs.todense()
     y = ys.todense()
 
     assert_eq(func(xs, ys), func(x, y))
 
 
-@pytest.mark.parametrize('func', [
-    operator.imul, operator.iadd, operator.isub
-])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize("func", [operator.imul, operator.iadd, operator.isub])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_elemwise_binary_inplace(func, shape):
     xs = sparse.random(shape, density=0.5)
     ys = sparse.random(shape, density=0.5)
 
     x = xs.todense()
     y = ys.todense()
 
     xs = func(xs, ys)
     x = func(x, y)
 
     assert_eq(xs, x)
 
 
-@pytest.mark.parametrize('func', [
-    lambda x, y, z: x + y + z,
-    lambda x, y, z: x * y * z,
-    lambda x, y, z: x + y * z,
-    lambda x, y, z: (x + y) * z
-])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize(
+    "func",
+    [
+        lambda x, y, z: x + y + z,
+        lambda x, y, z: x * y * z,
+        lambda x, y, z: x + y * z,
+        lambda x, y, z: (x + y) * z,
+    ],
+)
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_elemwise_trinary(func, shape):
     xs = sparse.random(shape, density=0.5)
     ys = sparse.random(shape, density=0.5)
     zs = sparse.random(shape, density=0.5)
 
     x = xs.todense()
     y = ys.todense()
@@ -636,25 +687,30 @@
 
     fs = sparse.elemwise(func, xs, ys, zs)
     assert isinstance(fs, COO)
 
     assert_eq(fs, func(x, y, z))
 
 
-@pytest.mark.parametrize('func', [operator.add, operator.mul])
-@pytest.mark.parametrize('shape1,shape2', [((2, 3, 4), (3, 4)),
-                                           ((3, 4), (2, 3, 4)),
-                                           ((3, 1, 4), (3, 2, 4)),
-                                           ((1, 3, 4), (3, 4)),
-                                           ((3, 4, 1), (3, 4, 2)),
-                                           ((1, 5), (5, 1)),
-                                           ((3, 1), (3, 4)),
-                                           ((3, 1), (1, 4)),
-                                           ((1, 4), (3, 4)),
-                                           ((2, 2, 2), (1, 1, 1))])
+@pytest.mark.parametrize("func", [operator.add, operator.mul])
+@pytest.mark.parametrize(
+    "shape1,shape2",
+    [
+        ((2, 3, 4), (3, 4)),
+        ((3, 4), (2, 3, 4)),
+        ((3, 1, 4), (3, 2, 4)),
+        ((1, 3, 4), (3, 4)),
+        ((3, 4, 1), (3, 4, 2)),
+        ((1, 5), (5, 1)),
+        ((3, 1), (3, 4)),
+        ((3, 1), (1, 4)),
+        ((1, 4), (3, 4)),
+        ((2, 2, 2), (1, 1, 1)),
+    ],
+)
 def test_binary_broadcasting(func, shape1, shape2):
     density1 = 1 if np.prod(shape1) == 1 else 0.5
     density2 = 1 if np.prod(shape2) == 1 else 0.5
 
     xs = sparse.random(shape1, density=density1)
     x = xs.todense()
 
@@ -666,171 +722,133 @@
 
     assert isinstance(actual, COO)
     assert_eq(expected, actual)
 
     assert np.count_nonzero(expected) == actual.nnz
 
 
-@pytest.mark.parametrize('shape1,shape2', [
-    ((3, 4), (2, 3, 4)),
-    ((3, 1, 4), (3, 2, 4)),
-    ((3, 4, 1), (3, 4, 2))
-])
+@pytest.mark.parametrize(
+    "shape1,shape2",
+    [((3, 4), (2, 3, 4)), ((3, 1, 4), (3, 2, 4)), ((3, 4, 1), (3, 4, 2))],
+)
 def test_broadcast_to(shape1, shape2):
     a = sparse.random(shape1, density=0.5)
     x = a.todense()
 
     assert_eq(np.broadcast_to(x, shape2), a.broadcast_to(shape2))
 
 
-@pytest.mark.parametrize('shapes', [
-    [
-        (2,),
-        (3, 2),
-        (4, 3, 2),
-    ],
-    [
-        (3,),
-        (2, 3),
-        (2, 2, 3),
-    ],
-    [
-        (2,),
-        (2, 2),
-        (2, 2, 2),
-    ],
+@pytest.mark.parametrize(
+    "shapes",
     [
-        (4,),
-        (4, 4),
-        (4, 4, 4),
+        [(2,), (3, 2), (4, 3, 2)],
+        [(3,), (2, 3), (2, 2, 3)],
+        [(2,), (2, 2), (2, 2, 2)],
+        [(4,), (4, 4), (4, 4, 4)],
+        [(4,), (4, 4), (4, 4, 4)],
+        [(4,), (4, 4), (4, 4, 4)],
+        [(1, 1, 2), (1, 3, 1), (4, 1, 1)],
+        [(2,), (2, 1), (2, 1, 1)],
     ],
+)
+@pytest.mark.parametrize(
+    "func",
     [
-        (4,),
-        (4, 4),
-        (4, 4, 4),
+        lambda x, y, z: (x + y) * z,
+        lambda x, y, z: x * (y + z),
+        lambda x, y, z: x * y * z,
+        lambda x, y, z: x + y + z,
+        lambda x, y, z: x + y - z,
+        lambda x, y, z: x - y + z,
     ],
-    [
-        (4,),
-        (4, 4),
-        (4, 4, 4),
-    ],
-    [
-        (1, 1, 2),
-        (1, 3, 1),
-        (4, 1, 1)
-    ],
-    [
-        (2,),
-        (2, 1),
-        (2, 1, 1)
-    ],
-])
-@pytest.mark.parametrize('func', [
-    lambda x, y, z: (x + y) * z,
-    lambda x, y, z: x * (y + z),
-    lambda x, y, z: x * y * z,
-    lambda x, y, z: x + y + z,
-    lambda x, y, z: x + y - z,
-    lambda x, y, z: x - y + z,
-])
+)
 def test_trinary_broadcasting(shapes, func):
     args = [sparse.random(s, density=0.5) for s in shapes]
     dense_args = [arg.todense() for arg in args]
 
     fs = sparse.elemwise(func, *args)
     assert isinstance(fs, COO)
 
     assert_eq(fs, func(*dense_args))
 
 
-@pytest.mark.parametrize('shapes, func', [
-    ([
-        (2,),
-        (3, 2),
-        (4, 3, 2),
-    ], lambda x, y, z: (x + y) * z),
-    ([
-        (3,),
-        (2, 3),
-        (2, 2, 3),
-    ], lambda x, y, z: x * (y + z)),
-    ([
-        (2,),
-        (2, 2),
-        (2, 2, 2),
-    ], lambda x, y, z: x * y * z),
-    ([
-        (4,),
-        (4, 4),
-        (4, 4, 4),
-    ], lambda x, y, z: x + y + z),
-])
-@pytest.mark.parametrize('value', [
-    np.nan,
-    np.inf,
-    -np.inf
-])
-@pytest.mark.parametrize('fraction', [0.25, 0.5, 0.75, 1.0])
-@pytest.mark.filterwarnings('ignore:invalid value')
+@pytest.mark.parametrize(
+    "shapes, func",
+    [
+        ([(2,), (3, 2), (4, 3, 2)], lambda x, y, z: (x + y) * z),
+        ([(3,), (2, 3), (2, 2, 3)], lambda x, y, z: x * (y + z)),
+        ([(2,), (2, 2), (2, 2, 2)], lambda x, y, z: x * y * z),
+        ([(4,), (4, 4), (4, 4, 4)], lambda x, y, z: x + y + z),
+    ],
+)
+@pytest.mark.parametrize("value", [np.nan, np.inf, -np.inf])
+@pytest.mark.parametrize("fraction", [0.25, 0.5, 0.75, 1.0])
+@pytest.mark.filterwarnings("ignore:invalid value")
 def test_trinary_broadcasting_pathological(shapes, func, value, fraction):
-    args = [sparse.random(s, density=0.5, data_rvs=random_value_array(value, fraction))
-            for s in shapes]
+    args = [
+        sparse.random(s, density=0.5, data_rvs=random_value_array(value, fraction))
+        for s in shapes
+    ]
     dense_args = [arg.todense() for arg in args]
 
     fs = sparse.elemwise(func, *args)
     assert isinstance(fs, COO)
 
     assert_eq(fs, func(*dense_args))
 
 
 def test_sparse_broadcasting(monkeypatch):
     orig_unmatch_coo = sparse._coo.umath._Elemwise._get_func_coords_data
 
-    state = {'num_matches': 0}
+    state = {"num_matches": 0}
 
     xs = sparse.random((3, 4), density=0.5)
     ys = sparse.random((3, 4), density=0.5)
 
     def mock_unmatch_coo(*args, **kwargs):
         result = orig_unmatch_coo(*args, **kwargs)
         if result is not None:
-            state['num_matches'] += 1
+            state["num_matches"] += 1
         return result
 
-    monkeypatch.setattr(sparse._coo.umath._Elemwise, '_get_func_coords_data', mock_unmatch_coo)
+    monkeypatch.setattr(
+        sparse._coo.umath._Elemwise, "_get_func_coords_data", mock_unmatch_coo
+    )
 
     xs * ys
 
     # Less than in case there's absolutely no overlap in some cases.
-    assert state['num_matches'] <= 1
+    assert state["num_matches"] <= 1
 
 
 def test_dense_broadcasting(monkeypatch):
     orig_unmatch_coo = sparse._coo.umath._Elemwise._get_func_coords_data
 
-    state = {'num_matches': 0}
+    state = {"num_matches": 0}
 
     xs = sparse.random((3, 4), density=0.5)
     ys = sparse.random((3, 4), density=0.5)
 
     def mock_unmatch_coo(*args, **kwargs):
         result = orig_unmatch_coo(*args, **kwargs)
         if result is not None:
-            state['num_matches'] += 1
+            state["num_matches"] += 1
         return result
 
-    monkeypatch.setattr(sparse._coo.umath._Elemwise, '_get_func_coords_data', mock_unmatch_coo)
+    monkeypatch.setattr(
+        sparse._coo.umath._Elemwise, "_get_func_coords_data", mock_unmatch_coo
+    )
 
     xs + ys
 
     # Less than in case there's absolutely no overlap in some cases.
-    assert state['num_matches'] <= 3
+    assert state["num_matches"] <= 3
 
 
-@pytest.mark.parametrize('format', ['coo', 'dok'])
+@pytest.mark.parametrize("format", ["coo", "dok"])
 def test_sparsearray_elemwise(format):
     xs = sparse.random((3, 4), density=0.5, format=format)
     ys = sparse.random((3, 4), density=0.5, format=format)
 
     x = xs.todense()
     y = ys.todense()
 
@@ -851,50 +869,61 @@
 def test_elemwise_noargs():
     def func():
         return np.float_(5.0)
 
     assert_eq(sparse.elemwise(func), func())
 
 
-@pytest.mark.parametrize('func', [
-    operator.pow, operator.truediv, operator.floordiv,
-    operator.ge, operator.le, operator.eq, operator.mod
-])
-@pytest.mark.filterwarnings('ignore:divide by zero')
-@pytest.mark.filterwarnings('ignore:invalid value')
+@pytest.mark.parametrize(
+    "func",
+    [
+        operator.pow,
+        operator.truediv,
+        operator.floordiv,
+        operator.ge,
+        operator.le,
+        operator.eq,
+        operator.mod,
+    ],
+)
+@pytest.mark.filterwarnings("ignore:divide by zero")
+@pytest.mark.filterwarnings("ignore:invalid value")
 def test_nonzero_outout_fv_ufunc(func):
     xs = sparse.random((2, 3, 4), density=0.5)
     ys = sparse.random((2, 3, 4), density=0.5)
 
     x = xs.todense()
     y = ys.todense()
 
     f = func(x, y)
     fs = func(xs, ys)
     assert isinstance(fs, COO)
 
     assert_eq(f, fs)
 
 
-@pytest.mark.parametrize('func, scalar', [
-    (operator.mul, 5),
-    (operator.add, 0),
-    (operator.sub, 0),
-    (operator.pow, 5),
-    (operator.truediv, 3),
-    (operator.floordiv, 4),
-    (operator.gt, 5),
-    (operator.lt, -5),
-    (operator.ne, 0),
-    (operator.ge, 5),
-    (operator.le, -3),
-    (operator.eq, 1),
-    (operator.mod, 5)
-])
-@pytest.mark.parametrize('convert_to_np_number', [True, False])
+@pytest.mark.parametrize(
+    "func, scalar",
+    [
+        (operator.mul, 5),
+        (operator.add, 0),
+        (operator.sub, 0),
+        (operator.pow, 5),
+        (operator.truediv, 3),
+        (operator.floordiv, 4),
+        (operator.gt, 5),
+        (operator.lt, -5),
+        (operator.ne, 0),
+        (operator.ge, 5),
+        (operator.le, -3),
+        (operator.eq, 1),
+        (operator.mod, 5),
+    ],
+)
+@pytest.mark.parametrize("convert_to_np_number", [True, False])
 def test_elemwise_scalar(func, scalar, convert_to_np_number):
     xs = sparse.random((2, 3, 4), density=0.5)
     if convert_to_np_number:
         scalar = np.float32(scalar)
     y = scalar
 
     x = xs.todense()
@@ -902,26 +931,29 @@
 
     assert isinstance(fs, COO)
     assert xs.nnz >= fs.nnz
 
     assert_eq(fs, func(x, y))
 
 
-@pytest.mark.parametrize('func, scalar', [
-    (operator.mul, 5),
-    (operator.add, 0),
-    (operator.sub, 0),
-    (operator.gt, -5),
-    (operator.lt, 5),
-    (operator.ne, 0),
-    (operator.ge, -5),
-    (operator.le, 3),
-    (operator.eq, 1),
-])
-@pytest.mark.parametrize('convert_to_np_number', [True, False])
+@pytest.mark.parametrize(
+    "func, scalar",
+    [
+        (operator.mul, 5),
+        (operator.add, 0),
+        (operator.sub, 0),
+        (operator.gt, -5),
+        (operator.lt, 5),
+        (operator.ne, 0),
+        (operator.ge, -5),
+        (operator.le, 3),
+        (operator.eq, 1),
+    ],
+)
+@pytest.mark.parametrize("convert_to_np_number", [True, False])
 def test_leftside_elemwise_scalar(func, scalar, convert_to_np_number):
     xs = sparse.random((2, 3, 4), density=0.5)
     if convert_to_np_number:
         scalar = np.float32(scalar)
     y = scalar
 
     x = xs.todense()
@@ -929,29 +961,32 @@
 
     assert isinstance(fs, COO)
     assert xs.nnz >= fs.nnz
 
     assert_eq(fs, func(y, x))
 
 
-@pytest.mark.parametrize('func, scalar', [
-    (operator.add, 5),
-    (operator.sub, -5),
-    (operator.pow, -3),
-    (operator.truediv, 0),
-    (operator.floordiv, 0),
-    (operator.gt, -5),
-    (operator.lt, 5),
-    (operator.ne, 1),
-    (operator.ge, -3),
-    (operator.le, 3),
-    (operator.eq, 0)
-])
-@pytest.mark.filterwarnings('ignore:divide by zero')
-@pytest.mark.filterwarnings('ignore:invalid value')
+@pytest.mark.parametrize(
+    "func, scalar",
+    [
+        (operator.add, 5),
+        (operator.sub, -5),
+        (operator.pow, -3),
+        (operator.truediv, 0),
+        (operator.floordiv, 0),
+        (operator.gt, -5),
+        (operator.lt, 5),
+        (operator.ne, 1),
+        (operator.ge, -3),
+        (operator.le, 3),
+        (operator.eq, 0),
+    ],
+)
+@pytest.mark.filterwarnings("ignore:divide by zero")
+@pytest.mark.filterwarnings("ignore:invalid value")
 def test_scalar_output_nonzero_fv(func, scalar):
     xs = sparse.random((2, 3, 4), density=0.5)
     y = scalar
 
     x = xs.todense()
 
     f = func(x, y)
@@ -959,44 +994,30 @@
 
     assert isinstance(fs, COO)
     assert fs.nnz <= xs.nnz
 
     assert_eq(f, fs)
 
 
-@pytest.mark.parametrize('func', [
-    operator.and_, operator.or_, operator.xor
-])
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-    (2, 3, 4, 5)
-])
+@pytest.mark.parametrize("func", [operator.and_, operator.or_, operator.xor])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitwise_binary(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
     ys = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
 
     x = xs.todense()
     y = ys.todense()
 
     assert_eq(func(xs, ys), func(x, y))
 
 
-@pytest.mark.parametrize('func', [
-    operator.iand, operator.ior, operator.ixor
-])
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-    (2, 3, 4, 5)
-])
+@pytest.mark.parametrize("func", [operator.iand, operator.ior, operator.ixor])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitwise_binary_inplace(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
     ys = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
 
     x = xs.todense()
@@ -1004,23 +1025,16 @@
 
     xs = func(xs, ys)
     x = func(x, y)
 
     assert_eq(xs, x)
 
 
-@pytest.mark.parametrize('func', [
-    operator.lshift, operator.rshift
-])
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-    (2, 3, 4, 5)
-])
+@pytest.mark.parametrize("func", [operator.lshift, operator.rshift])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitshift_binary(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
 
     # Can't merge into test_bitwise_binary because left/right shifting
     # with something >= 64 isn't defined.
@@ -1028,23 +1042,16 @@
 
     x = xs.todense()
     y = ys.todense()
 
     assert_eq(func(xs, ys), func(x, y))
 
 
-@pytest.mark.parametrize('func', [
-    operator.ilshift, operator.irshift
-])
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-    (2, 3, 4, 5)
-])
+@pytest.mark.parametrize("func", [operator.ilshift, operator.irshift])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitshift_binary_inplace(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
 
     # Can't merge into test_bitwise_binary because left/right shifting
     # with something >= 64 isn't defined.
@@ -1055,60 +1062,46 @@
 
     xs = func(xs, ys)
     x = func(x, y)
 
     assert_eq(xs, x)
 
 
-@pytest.mark.parametrize('func', [
-    operator.and_
-])
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-    (2, 3, 4, 5)
-])
+@pytest.mark.parametrize("func", [operator.and_])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitwise_scalar(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
     y = np.random.randint(100)
 
     x = xs.todense()
 
     assert_eq(func(xs, y), func(x, y))
     assert_eq(func(y, xs), func(y, x))
 
 
-@pytest.mark.parametrize('func', [
-    operator.lshift, operator.rshift
-])
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-    (2, 3, 4, 5)
-])
+@pytest.mark.parametrize("func", [operator.lshift, operator.rshift])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitshift_scalar(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
 
     # Can't merge into test_bitwise_binary because left/right shifting
     # with something >= 64 isn't defined.
     y = np.random.randint(64)
 
     x = xs.todense()
 
     assert_eq(func(xs, y), func(x, y))
 
 
-@pytest.mark.parametrize('func', [operator.invert])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize("func", [operator.invert])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_unary_bitwise_nonzero_output_fv(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
     x = xs.todense()
 
     f = func(x)
@@ -1116,16 +1109,16 @@
 
     assert isinstance(fs, COO)
     assert fs.nnz <= xs.nnz
 
     assert_eq(f, fs)
 
 
-@pytest.mark.parametrize('func', [operator.or_, operator.xor])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize("func", [operator.or_, operator.xor])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_binary_bitwise_nonzero_output_fv(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     xs = (sparse.random(shape, density=0.5) * 100).astype(np.int_)
     y = np.random.randint(1, 100)
 
     x = xs.todense()
@@ -1135,31 +1128,31 @@
 
     assert isinstance(fs, COO)
     assert fs.nnz <= xs.nnz
 
     assert_eq(f, fs)
 
 
-@pytest.mark.parametrize('func', [
-    operator.mul, operator.add, operator.sub, operator.gt,
-    operator.lt, operator.ne
-])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize(
+    "func",
+    [operator.mul, operator.add, operator.sub, operator.gt, operator.lt, operator.ne],
+)
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_elemwise_nonzero_input_fv(func, shape):
     xs = sparse.random(shape, density=0.5, fill_value=np.random.rand())
     ys = sparse.random(shape, density=0.5, fill_value=np.random.rand())
 
     x = xs.todense()
     y = ys.todense()
 
     assert_eq(func(xs, ys), func(x, y))
 
 
-@pytest.mark.parametrize('func', [operator.lshift, operator.rshift])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize("func", [operator.lshift, operator.rshift])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_binary_bitshift_densification_fails(func, shape):
     # Small arrays need high density to have nnz entries
     # Casting floats to int will result in all zeros, hence the * 100
     x = np.random.randint(1, 100)
     ys = (sparse.random(shape, density=0.5) * 64).astype(np.int_)
 
     y = ys.todense()
@@ -1169,16 +1162,16 @@
 
     assert isinstance(fs, COO)
     assert fs.nnz <= ys.nnz
 
     assert_eq(f, fs)
 
 
-@pytest.mark.parametrize('func', [operator.and_, operator.or_, operator.xor])
-@pytest.mark.parametrize('shape', [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
+@pytest.mark.parametrize("func", [operator.and_, operator.or_, operator.xor])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4), (2, 3, 4, 5)])
 def test_bitwise_binary_bool(func, shape):
     # Small arrays need high density to have nnz entries
     xs = sparse.random(shape, density=0.5).astype(bool)
     ys = sparse.random(shape, density=0.5).astype(bool)
 
     x = xs.todense()
     y = ys.todense()
@@ -1204,127 +1197,137 @@
     assert_eq(x > m, s > m)
 
     m = s.data[2]
     assert_eq(x > m, s > m)
     assert_eq(x >= m, s >= m)
 
 
-@pytest.mark.parametrize('index', [
-    # Integer
-    0,
-    1,
-    -1,
-    (1, 1, 1),
-    # Pure slices
-    (slice(0, 2),),
-    (slice(None, 2), slice(None, 2)),
-    (slice(1, None), slice(1, None)),
-    (slice(None, None),),
-    (slice(None, None, -1),),
-    (slice(None, 2, -1), slice(None, 2, -1)),
-    (slice(1, None, 2), slice(1, None, 2)),
-    (slice(None, None, 2),),
-    (slice(None, 2, -1), slice(None, 2, -2)),
-    (slice(1, None, 2), slice(1, None, 1)),
-    (slice(None, None, -2),),
-    # Combinations
-    (0, slice(0, 2),),
-    (slice(0, 1), 0),
-    (None, slice(1, 3), 0),
-    (slice(0, 3), None, 0),
-    (slice(1, 2), slice(2, 4)),
-    (slice(1, 2), slice(None, None)),
-    (slice(1, 2), slice(None, None), 2),
-    (slice(1, 2, 2), slice(None, None), 2),
-    (slice(1, 2, None), slice(None, None, 2), 2),
-    (slice(1, 2, -2), slice(None, None), -2),
-    (slice(1, 2, None), slice(None, None, -2), 2),
-    (slice(1, 2, -1), slice(None, None), -1),
-    (slice(1, 2, None), slice(None, None, -1), 2),
-    (slice(2, 0, -1), slice(None, None), -1),
-    (slice(-2, None, None),),
-    (slice(-1, None, None), slice(-2, None, None)),
-    # With ellipsis
-    (Ellipsis, slice(1, 3)),
-    (1, Ellipsis, slice(1, 3)),
-    (slice(0, 1), Ellipsis),
-    (Ellipsis, None),
-    (None, Ellipsis),
-    (1, Ellipsis),
-    (1, Ellipsis, None),
-    (1, 1, 1, Ellipsis),
-    (Ellipsis, 1, None),
-    # Pathological - Slices larger than array
-    (slice(None, 1000)),
-    (slice(None), slice(None, 1000)),
-    (slice(None), slice(1000, -1000, -1)),
-    (slice(None), slice(1000, -1000, -50)),
-    # Pathological - Wrong ordering of start/stop
-    (slice(5, 0),),
-    (slice(0, 5, -1),),
-    (slice(0, 0, None),),
-])
+@pytest.mark.parametrize(
+    "index",
+    [
+        # Integer
+        0,
+        1,
+        -1,
+        (1, 1, 1),
+        # Pure slices
+        (slice(0, 2),),
+        (slice(None, 2), slice(None, 2)),
+        (slice(1, None), slice(1, None)),
+        (slice(None, None),),
+        (slice(None, None, -1),),
+        (slice(None, 2, -1), slice(None, 2, -1)),
+        (slice(1, None, 2), slice(1, None, 2)),
+        (slice(None, None, 2),),
+        (slice(None, 2, -1), slice(None, 2, -2)),
+        (slice(1, None, 2), slice(1, None, 1)),
+        (slice(None, None, -2),),
+        # Combinations
+        (0, slice(0, 2)),
+        (slice(0, 1), 0),
+        (None, slice(1, 3), 0),
+        (slice(0, 3), None, 0),
+        (slice(1, 2), slice(2, 4)),
+        (slice(1, 2), slice(None, None)),
+        (slice(1, 2), slice(None, None), 2),
+        (slice(1, 2, 2), slice(None, None), 2),
+        (slice(1, 2, None), slice(None, None, 2), 2),
+        (slice(1, 2, -2), slice(None, None), -2),
+        (slice(1, 2, None), slice(None, None, -2), 2),
+        (slice(1, 2, -1), slice(None, None), -1),
+        (slice(1, 2, None), slice(None, None, -1), 2),
+        (slice(2, 0, -1), slice(None, None), -1),
+        (slice(-2, None, None),),
+        (slice(-1, None, None), slice(-2, None, None)),
+        # With ellipsis
+        (Ellipsis, slice(1, 3)),
+        (1, Ellipsis, slice(1, 3)),
+        (slice(0, 1), Ellipsis),
+        (Ellipsis, None),
+        (None, Ellipsis),
+        (1, Ellipsis),
+        (1, Ellipsis, None),
+        (1, 1, 1, Ellipsis),
+        (Ellipsis, 1, None),
+        # Pathological - Slices larger than array
+        (slice(None, 1000)),
+        (slice(None), slice(None, 1000)),
+        (slice(None), slice(1000, -1000, -1)),
+        (slice(None), slice(1000, -1000, -50)),
+        # Pathological - Wrong ordering of start/stop
+        (slice(5, 0),),
+        (slice(0, 5, -1),),
+        (slice(0, 0, None),),
+    ],
+)
 def test_slicing(index):
     s = sparse.random((2, 3, 4), density=0.5)
     x = s.todense()
 
     assert_eq(x[index], s[index])
 
 
-@pytest.mark.parametrize('index', [
-    ([1, 0], 0),
-    (1, [0, 2]),
-    (0, [1, 0], 0),
-    (1, [2, 0], 0),
-    ([True, False], slice(1, None), slice(-2, None)),
-    (slice(1, None), slice(-2, None), [True, False, True, False]),
-    ([1, 0],),
-    (Ellipsis, [2, 1, 3],),
-    (slice(None), [2, 1, 2],),
-    (1, [2, 0, 1],),
-])
+@pytest.mark.parametrize(
+    "index",
+    [
+        ([1, 0], 0),
+        (1, [0, 2]),
+        (0, [1, 0], 0),
+        (1, [2, 0], 0),
+        (1, [], 0),
+        ([True, False], slice(1, None), slice(-2, None)),
+        (slice(1, None), slice(-2, None), [True, False, True, False]),
+        ([1, 0],),
+        (Ellipsis, [2, 1, 3]),
+        (slice(None), [2, 1, 2]),
+        (1, [2, 0, 1]),
+    ],
+)
 def test_advanced_indexing(index):
     s = sparse.random((2, 3, 4), density=0.5)
     x = s.todense()
 
     assert_eq(x[index], s[index])
 
 
 def test_custom_dtype_slicing():
-    dt = np.dtype([('part1', np.float_),
-                   ('part2', np.int_, (2,)),
-                   ('part3', np.int_, (2, 2))])
+    dt = np.dtype(
+        [("part1", np.float_), ("part2", np.int_, (2,)), ("part3", np.int_, (2, 2))]
+    )
 
     x = np.zeros((2, 3, 4), dtype=dt)
     x[1, 1, 1] = (0.64, [4, 2], [[1, 2], [3, 0]])
 
     s = COO.from_numpy(x)
 
     assert x[1, 1, 1] == s[1, 1, 1]
     assert x[0, 1, 2] == s[0, 1, 2]
 
-    assert_eq(x['part1'], s['part1'])
-    assert_eq(x['part2'], s['part2'])
-    assert_eq(x['part3'], s['part3'])
-
-
-@pytest.mark.parametrize('index', [
-    (Ellipsis, Ellipsis),
-    (1, 1, 1, 1),
-    (slice(None),) * 4,
-    5,
-    -5,
-    'foo',
-    [True, False, False],
-    0.5,
-    [0.5],
-    {'potato': 'kartoffel'},
-    ([0, 1],) * 2,
-    ([[0, 1]],),
-])
+    assert_eq(x["part1"], s["part1"])
+    assert_eq(x["part2"], s["part2"])
+    assert_eq(x["part3"], s["part3"])
+
+
+@pytest.mark.parametrize(
+    "index",
+    [
+        (Ellipsis, Ellipsis),
+        (1, 1, 1, 1),
+        (slice(None),) * 4,
+        5,
+        -5,
+        "foo",
+        [True, False, False],
+        0.5,
+        [0.5],
+        {"potato": "kartoffel"},
+        ([0, 1],) * 2,
+        ([[0, 1]],),
+    ],
+)
 def test_slicing_errors(index):
     s = sparse.random((2, 3, 4), density=0.5)
 
     with pytest.raises(IndexError):
         s[index]
 
 
@@ -1332,116 +1335,113 @@
     xx = sparse.random((2, 3, 4), density=0.5)
     x = xx.todense()
     yy = sparse.random((5, 3, 4), density=0.5)
     y = yy.todense()
     zz = sparse.random((4, 3, 4), density=0.5)
     z = zz.todense()
 
-    assert_eq(np.concatenate([x, y, z], axis=0),
-              sparse.concatenate([xx, yy, zz], axis=0))
+    assert_eq(
+        np.concatenate([x, y, z], axis=0), sparse.concatenate([xx, yy, zz], axis=0)
+    )
 
     xx = sparse.random((5, 3, 1), density=0.5)
     x = xx.todense()
     yy = sparse.random((5, 3, 3), density=0.5)
     y = yy.todense()
     zz = sparse.random((5, 3, 2), density=0.5)
     z = zz.todense()
 
-    assert_eq(np.concatenate([x, y, z], axis=2),
-              sparse.concatenate([xx, yy, zz], axis=2))
+    assert_eq(
+        np.concatenate([x, y, z], axis=2), sparse.concatenate([xx, yy, zz], axis=2)
+    )
 
-    assert_eq(np.concatenate([x, y, z], axis=-1),
-              sparse.concatenate([xx, yy, zz], axis=-1))
+    assert_eq(
+        np.concatenate([x, y, z], axis=-1), sparse.concatenate([xx, yy, zz], axis=-1)
+    )
 
 
-@pytest.mark.parametrize('axis', [0, 1])
-@pytest.mark.parametrize('func', [sparse.stack, sparse.concatenate])
+@pytest.mark.parametrize("axis", [0, 1])
+@pytest.mark.parametrize("func", [sparse.stack, sparse.concatenate])
 def test_concatenate_mixed(func, axis):
     s = sparse.random((10, 10), density=0.5)
     d = s.todense()
 
     with pytest.raises(ValueError):
         func([d, s, s], axis=axis)
 
 
 def test_concatenate_noarrays():
     with pytest.raises(ValueError):
         sparse.concatenate([])
 
 
-@pytest.mark.parametrize('shape', [(5,), (2, 3, 4), (5, 2)])
-@pytest.mark.parametrize('axis', [0, 1, -1])
+@pytest.mark.parametrize("shape", [(5,), (2, 3, 4), (5, 2)])
+@pytest.mark.parametrize("axis", [0, 1, -1])
 def test_stack(shape, axis):
     xx = sparse.random(shape, density=0.5)
     x = xx.todense()
     yy = sparse.random(shape, density=0.5)
     y = yy.todense()
     zz = sparse.random(shape, density=0.5)
     z = zz.todense()
 
-    assert_eq(np.stack([x, y, z], axis=axis),
-              sparse.stack([xx, yy, zz], axis=axis))
+    assert_eq(np.stack([x, y, z], axis=axis), sparse.stack([xx, yy, zz], axis=axis))
 
 
 def test_large_concat_stack():
     data = np.array([1], dtype=np.uint8)
     coords = np.array([[255]], dtype=np.uint8)
 
     xs = COO(coords, data, shape=(256,), has_duplicates=False, sorted=True)
     x = xs.todense()
 
-    assert_eq(np.stack([x, x]),
-              sparse.stack([xs, xs]))
+    assert_eq(np.stack([x, x]), sparse.stack([xs, xs]))
 
-    assert_eq(np.concatenate((x, x)),
-              sparse.concatenate((xs, xs)))
+    assert_eq(np.concatenate((x, x)), sparse.concatenate((xs, xs)))
 
 
 def test_addition():
     a = sparse.random((2, 3, 4), density=0.5)
     x = a.todense()
 
     b = sparse.random((2, 3, 4), density=0.5)
     y = b.todense()
 
     assert_eq(x + y, a + b)
     assert_eq(x - y, a - b)
 
 
-@pytest.mark.parametrize('scalar', [2, 2.5, np.float32(2.0), np.int8(3)])
+@pytest.mark.parametrize("scalar", [2, 2.5, np.float32(2.0), np.int8(3)])
 def test_scalar_multiplication(scalar):
     a = sparse.random((2, 3, 4), density=0.5)
     x = a.todense()
 
     assert_eq(x * scalar, a * scalar)
     assert (a * scalar).nnz == a.nnz
     assert_eq(scalar * x, scalar * a)
     assert (scalar * a).nnz == a.nnz
     assert_eq(x / scalar, a / scalar)
     assert (a / scalar).nnz == a.nnz
     assert_eq(x // scalar, a // scalar)
     # division may reduce nnz.
 
 
-@pytest.mark.filterwarnings('ignore:divide by zero')
+@pytest.mark.filterwarnings("ignore:divide by zero")
 def test_scalar_exponentiation():
     a = sparse.random((2, 3, 4), density=0.5)
     x = a.todense()
 
     assert_eq(x ** 2, a ** 2)
     assert_eq(x ** 0.5, a ** 0.5)
 
     assert_eq(x ** -1, a ** -1)
 
 
 def test_create_with_lists_of_tuples():
-    L = [((0, 0, 0), 1),
-         ((1, 2, 1), 1),
-         ((1, 1, 1), 2),
-         ((1, 3, 2), 3)]
+    L = [((0, 0, 0), 1), ((1, 2, 1), 1), ((1, 1, 1), 2), ((1, 3, 2), 3)]
 
     s = COO(L)
 
     x = np.zeros((2, 4, 3), dtype=np.asarray([1, 2, 3]).dtype)
     for ind, value in L:
         x[ind] = value
 
@@ -1475,50 +1475,61 @@
 
     assert_eq(x, xx, check_nnz=False)
     assert_eq(x.T.dot(x), xx.T.dot(xx), check_nnz=False)
     assert isinstance(x + xx, COO)
     assert isinstance(xx + x, COO)
 
 
-@pytest.mark.parametrize('scipy_format', ['coo', 'csr', 'dok', 'csc'])
+@pytest.mark.parametrize("scipy_format", ["coo", "csr", "dok", "csc"])
 def test_scipy_sparse_interaction(scipy_format):
     x = sparse.random((10, 20), density=0.2).todense()
-    sp = getattr(scipy.sparse, scipy_format + '_matrix')(x)
+    sp = getattr(scipy.sparse, scipy_format + "_matrix")(x)
     coo = COO(x)
     assert isinstance(sp + coo, COO)
     assert isinstance(coo + sp, COO)
     assert_eq(sp, coo)
 
 
-@pytest.mark.parametrize('func', [
-    operator.mul, operator.add, operator.sub, operator.gt,
-    operator.lt, operator.ne
-])
+@pytest.mark.parametrize(
+    "func",
+    [operator.mul, operator.add, operator.sub, operator.gt, operator.lt, operator.ne],
+)
 def test_op_scipy_sparse(func):
     xs = sparse.random((3, 4), density=0.5)
     y = sparse.random((3, 4), density=0.5).todense()
 
     ys = scipy.sparse.csr_matrix(y)
     x = xs.todense()
 
     assert_eq(func(x, y), func(xs, ys))
 
 
-@pytest.mark.parametrize('func', [
-    operator.add,
-    operator.sub,
-    pytest.param(operator.mul,
-                 marks=pytest.mark.xfail(reason="Scipy sparse auto-densifies in this case.")),
-    pytest.param(operator.gt,
-                 marks=pytest.mark.xfail(reason="Scipy sparse doesn't support this yet.")),
-    pytest.param(operator.lt,
-                 marks=pytest.mark.xfail(reason="Scipy sparse doesn't support this yet.")),
-    pytest.param(operator.ne,
-                 marks=pytest.mark.xfail(reason="Scipy sparse doesn't support this yet.")),
-])
+@pytest.mark.parametrize(
+    "func",
+    [
+        operator.add,
+        operator.sub,
+        pytest.param(
+            operator.mul,
+            marks=pytest.mark.xfail(reason="Scipy sparse auto-densifies in this case."),
+        ),
+        pytest.param(
+            operator.gt,
+            marks=pytest.mark.xfail(reason="Scipy sparse doesn't support this yet."),
+        ),
+        pytest.param(
+            operator.lt,
+            marks=pytest.mark.xfail(reason="Scipy sparse doesn't support this yet."),
+        ),
+        pytest.param(
+            operator.ne,
+            marks=pytest.mark.xfail(reason="Scipy sparse doesn't support this yet."),
+        ),
+    ],
+)
 def test_op_scipy_sparse_left(func):
     ys = sparse.random((3, 4), density=0.5)
     x = sparse.random((3, 4), density=0.5).todense()
 
     xs = scipy.sparse.csr_matrix(x)
     y = ys.todense()
 
@@ -1566,25 +1577,31 @@
     x = COO({(1, 1): 1})
     y = sum([x] * 100)
     assert y.nnz < np.prod(y.shape)
 
 
 def test_caching():
     x = COO({(9, 9, 9): 1})
-    assert x[:].reshape((100, 10)).transpose().tocsr() is not x[:].reshape((100, 10)).transpose().tocsr()
+    assert (
+        x[:].reshape((100, 10)).transpose().tocsr()
+        is not x[:].reshape((100, 10)).transpose().tocsr()
+    )
 
     x = COO({(9, 9, 9): 1}, cache=True)
-    assert x[:].reshape((100, 10)).transpose().tocsr() is x[:].reshape((100, 10)).transpose().tocsr()
+    assert (
+        x[:].reshape((100, 10)).transpose().tocsr()
+        is x[:].reshape((100, 10)).transpose().tocsr()
+    )
 
     x = COO({(1, 1, 1, 1, 1, 1, 1, 2): 1}, cache=True)
 
     for i in range(x.ndim):
         x.reshape(x.size)
 
-    assert len(x._cache['reshape']) < 5
+    assert len(x._cache["reshape"]) < 5
 
 
 def test_scalar_slicing():
     x = np.array([0, 1])
     s = COO(x)
     assert np.isscalar(s[0])
     assert_eq(x[0], s[0])
@@ -1597,45 +1614,35 @@
     assert_eq(x[1], s[1])
 
     assert isinstance(s[1, ...], COO)
     assert s[1, ...].shape == ()
     assert_eq(x[1, ...], s[1, ...])
 
 
-@pytest.mark.parametrize('shape, k', [
-    ((3, 4), 0),
-    ((3, 4, 5), 1),
-    ((4, 2), -1),
-    ((2, 4), -2),
-    ((4, 4), 1000),
-])
+@pytest.mark.parametrize(
+    "shape, k",
+    [((3, 4), 0), ((3, 4, 5), 1), ((4, 2), -1), ((2, 4), -2), ((4, 4), 1000)],
+)
 def test_triul(shape, k):
     s = sparse.random(shape, density=0.5)
     x = s.todense()
 
     assert_eq(np.triu(x, k), sparse.triu(s, k))
     assert_eq(np.tril(x, k), sparse.tril(s, k))
 
 
 def test_empty_reduction():
     x = np.zeros((2, 3, 4), dtype=np.float_)
     xs = COO.from_numpy(x)
 
-    assert_eq(x.sum(axis=(0, 2)),
-              xs.sum(axis=(0, 2)))
+    assert_eq(x.sum(axis=(0, 2)), xs.sum(axis=(0, 2)))
 
 
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-])
-@pytest.mark.parametrize('density', [
-    0.1, 0.3, 0.5, 0.7
-])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4)])
+@pytest.mark.parametrize("density", [0.1, 0.3, 0.5, 0.7])
 def test_random_shape(shape, density):
     s = sparse.random(shape, density)
 
     assert isinstance(s, COO)
 
     assert s.shape == shape
     expected_nnz = density * np.prod(shape)
@@ -1653,35 +1660,31 @@
     state = np.random.randint(100)
     s1 = sparse.random((2, 3, 4), 0.3, random_state=state)
     s2 = sparse.random((2, 3, 4), 0.3, random_state=state)
 
     assert_eq(s1, s2)
 
 
-@pytest.mark.parametrize('rvs, dtype', [
-    (None, np.float64),
-    (scipy.stats.poisson(25, loc=10).rvs, np.int),
-    (lambda x: np.random.choice([True, False], size=x), np.bool),
-])
-@pytest.mark.parametrize('shape', [
-    (2, 4, 5),
-    (20, 40, 50),
-])
-@pytest.mark.parametrize('density', [
-    0.0, 0.01, 0.1, 0.2,
-])
+@pytest.mark.parametrize(
+    "rvs, dtype",
+    [
+        (None, np.float64),
+        (scipy.stats.poisson(25, loc=10).rvs, np.int),
+        (lambda x: np.random.choice([True, False], size=x), np.bool),
+    ],
+)
+@pytest.mark.parametrize("shape", [(2, 4, 5), (20, 40, 50)])
+@pytest.mark.parametrize("density", [0.0, 0.01, 0.1, 0.2])
 def test_random_rvs(rvs, dtype, shape, density):
     x = sparse.random(shape, density, data_rvs=rvs)
     assert x.shape == shape
     assert x.dtype == dtype
 
 
-@pytest.mark.parametrize('format', [
-    'coo', 'dok'
-])
+@pytest.mark.parametrize("format", ["coo", "dok"])
 def test_random_fv(format):
     fv = np.random.rand()
     s = sparse.random((2, 3, 4), density=0.5, format=format, fill_value=fv)
 
     assert s.fill_value == fv
 
 
@@ -1712,66 +1715,29 @@
 def test_np_array():
     s = sparse.random((20, 30, 40))
 
     with pytest.raises(RuntimeError):
         np.array(s)
 
 
-@pytest.mark.parametrize('shapes', [
-    [
-        (2,),
-        (3, 2),
-        (4, 3, 2),
-    ],
+@pytest.mark.parametrize(
+    "shapes",
     [
-        (3,),
-        (2, 3),
-        (2, 2, 3),
+        [(2,), (3, 2), (4, 3, 2)],
+        [(3,), (2, 3), (2, 2, 3)],
+        [(2,), (2, 2), (2, 2, 2)],
+        [(4,), (4, 4), (4, 4, 4)],
+        [(4,), (4, 4), (4, 4, 4)],
+        [(4,), (4, 4), (4, 4, 4)],
+        [(1, 1, 2), (1, 3, 1), (4, 1, 1)],
+        [(2,), (2, 1), (2, 1, 1)],
+        [(3,), (), (2, 3)],
+        [(4, 4), (), ()],
     ],
-    [
-        (2,),
-        (2, 2),
-        (2, 2, 2),
-    ],
-    [
-        (4,),
-        (4, 4),
-        (4, 4, 4),
-    ],
-    [
-        (4,),
-        (4, 4),
-        (4, 4, 4),
-    ],
-    [
-        (4,),
-        (4, 4),
-        (4, 4, 4),
-    ],
-    [
-        (1, 1, 2),
-        (1, 3, 1),
-        (4, 1, 1)
-    ],
-    [
-        (2,),
-        (2, 1),
-        (2, 1, 1)
-    ],
-    [
-        (3,),
-        (),
-        (2, 3)
-    ],
-    [
-        (4, 4),
-        (),
-        ()
-    ]
-])
+)
 def test_three_arg_where(shapes):
     cs = sparse.random(shapes[0], density=0.5).astype(np.bool)
     xs = sparse.random(shapes[1], density=0.5)
     ys = sparse.random(shapes[2], density=0.5)
 
     c = cs.todense()
     x = xs.todense()
@@ -1808,17 +1774,15 @@
     cs = sparse.random((2, 3, 4), density=0.5).astype(np.bool)
     xs = sparse.random((2, 3, 4), density=0.5)
 
     with pytest.raises(ValueError):
         sparse.where(cs, xs)
 
 
-@pytest.mark.parametrize('func', [
-    operator.imul, operator.iadd, operator.isub
-])
+@pytest.mark.parametrize("func", [operator.imul, operator.iadd, operator.isub])
 def test_inplace_invalid_shape(func):
     xs = sparse.random((3, 4), density=0.5)
     ys = sparse.random((2, 3, 4), density=0.5)
 
     with pytest.raises(ValueError):
         func(xs, ys)
 
@@ -1840,43 +1804,37 @@
 def test_argwhere():
     s = sparse.random((2, 3, 4), density=0.5)
     x = s.todense()
 
     assert_eq(np.argwhere(s), np.argwhere(x), compare_dtype=False)
 
 
-@pytest.mark.parametrize('format', [
-    'coo',
-    'dok',
-])
+@pytest.mark.parametrize("format", ["coo", "dok"])
 def test_asformat(format):
-    s = sparse.random((2, 3, 4), density=0.5, format='coo')
+    s = sparse.random((2, 3, 4), density=0.5, format="coo")
     s2 = s.asformat(format)
 
     assert_eq(s, s2)
 
 
-@pytest.mark.parametrize('format', [
-    sparse.COO,
-    sparse.DOK,
-    scipy.sparse.csr_matrix,
-    np.asarray
-])
+@pytest.mark.parametrize(
+    "format", [sparse.COO, sparse.DOK, scipy.sparse.csr_matrix, np.asarray]
+)
 def test_as_coo(format):
-    x = format(sparse.random((3, 4), density=0.5, format='coo').todense())
+    x = format(sparse.random((3, 4), density=0.5, format="coo").todense())
 
     s1 = sparse.as_coo(x)
     s2 = COO(x)
 
     assert_eq(x, s1)
     assert_eq(x, s2)
 
 
 def test_invalid_attrs_error():
-    s = sparse.random((3, 4), density=0.5, format='coo')
+    s = sparse.random((3, 4), density=0.5, format="coo")
 
     with pytest.raises(ValueError):
         sparse.as_coo(s, shape=(2, 3))
 
     with pytest.raises(ValueError):
         COO(s, shape=(2, 3))
 
@@ -1907,80 +1865,74 @@
     assert_eq(s1.prod(axis=0), x1.prod(axis=0))
     assert_eq(s2.prod(axis=0), x2.prod(axis=0))
 
 
 class TestRoll:
 
     # test on 1d array #
-    @pytest.mark.parametrize('shift', [0, 2, -2, 20, -20])
+    @pytest.mark.parametrize("shift", [0, 2, -2, 20, -20])
     def test_1d(self, shift):
         xs = sparse.random((100,), density=0.5)
         x = xs.todense()
         assert_eq(np.roll(x, shift), sparse.roll(xs, shift))
         assert_eq(np.roll(x, shift), sparse.roll(x, shift))
 
     # test on 2d array #
-    @pytest.mark.parametrize(
-        'shift', [0, 2, -2, 20, -20])
-    @pytest.mark.parametrize(
-        'ax', [None, 0, 1, (0, 1)])
+    @pytest.mark.parametrize("shift", [0, 2, -2, 20, -20])
+    @pytest.mark.parametrize("ax", [None, 0, 1, (0, 1)])
     def test_2d(self, shift, ax):
         xs = sparse.random((10, 10), density=0.5)
         x = xs.todense()
         assert_eq(np.roll(x, shift, axis=ax), sparse.roll(xs, shift, axis=ax))
         assert_eq(np.roll(x, shift, axis=ax), sparse.roll(x, shift, axis=ax))
 
     # test on rolling multiple axes at once #
-    @pytest.mark.parametrize(
-        'shift', [(0, 0), (1, -1), (-1, 1), (10, -10)])
-    @pytest.mark.parametrize(
-        'ax', [(0, 1), (0, 2), (1, 2), (-1, 1)])
+    @pytest.mark.parametrize("shift", [(0, 0), (1, -1), (-1, 1), (10, -10)])
+    @pytest.mark.parametrize("ax", [(0, 1), (0, 2), (1, 2), (-1, 1)])
     def test_multiaxis(self, shift, ax):
         xs = sparse.random((9, 9, 9), density=0.5)
         x = xs.todense()
         assert_eq(np.roll(x, shift, axis=ax), sparse.roll(xs, shift, axis=ax))
         assert_eq(np.roll(x, shift, axis=ax), sparse.roll(x, shift, axis=ax))
 
     # test original is unchanged #
-    @pytest.mark.parametrize(
-        'shift', [0, 2, -2, 20, -20])
-    @pytest.mark.parametrize(
-        'ax', [None, 0, 1, (0, 1)])
+    @pytest.mark.parametrize("shift", [0, 2, -2, 20, -20])
+    @pytest.mark.parametrize("ax", [None, 0, 1, (0, 1)])
     def test_original_is_copied(self, shift, ax):
         xs = sparse.random((10, 10), density=0.5)
         xc = COO(np.copy(xs.coords), np.copy(xs.data), shape=xs.shape)
         sparse.roll(xs, shift, axis=ax)
         assert_eq(xs, xc)
 
     # test on empty array #
     def test_empty(self):
         x = np.array([])
         assert_eq(np.roll(x, 1), sparse.roll(sparse.as_coo(x), 1))
 
     # test error handling #
     @pytest.mark.parametrize(
-        'args', [
+        "args",
+        [
             # iterable shift, but axis not iterable
             ((1, 1), 0),
             # ndim(axis) != 1
             (1, [[0, 1]]),
             # ndim(shift) != 1
             ([[0, 1]], [0, 1]),
-            ([[0, 1], [0, 1]], [0, 1])
-        ]
+            ([[0, 1], [0, 1]], [0, 1]),
+        ],
     )
     def test_valerr(self, args):
         x = sparse.random((2, 2, 2), density=1)
         with pytest.raises(ValueError):
             sparse.roll(x, *args)
 
 
 def test_clip():
-    x = np.array([[0, 0, 1, 0, 2],
-                  [5, 0, 0, 3, 0]])
+    x = np.array([[0, 0, 1, 0, 2], [5, 0, 0, 3, 0]])
 
     s = sparse.COO.from_numpy(x)
 
     assert_eq(s.clip(min=1), x.clip(min=1))
     assert_eq(s.clip(max=3), x.clip(max=3))
     assert_eq(s.clip(min=1, max=3), x.clip(min=1, max=3))
     assert_eq(s.clip(min=1, max=3.0), x.clip(min=1, max=3.0))
@@ -2021,15 +1973,15 @@
     assert x._cache is not None
     # Pickle sends data but not cache
     x2 = pickle.loads(pickle.dumps(x))
     assert_eq(x, x2)
     assert x2._cache is None
 
 
-@pytest.mark.parametrize('deep', [True, False])
+@pytest.mark.parametrize("deep", [True, False])
 def test_copy(deep):
     x = sparse.COO.from_numpy([1, 0, 0, 0, 0]).reshape((5, 1))
     # Enable caching and add some data to it
     x.enable_caching()
     x.T
     assert x._cache is not None
 
@@ -2038,74 +1990,74 @@
     assert (x2.data is x.data) is not deep
     assert (x2.coords is x.coords) is not deep
     assert x2._cache is None
 
 
 @pytest.mark.parametrize("ndim", [2, 3, 4, 5])
 def test_initialization(ndim):
-    shape = [10, ] * ndim
+    shape = [10] * ndim
     shape[1] *= 2
     shape = tuple(shape)
 
     coords = np.random.randint(10, size=ndim * 20).reshape(ndim, 20)
     data = np.random.rand(20)
     COO(coords, data=data, shape=shape)
 
     with pytest.raises(ValueError, match="data length"):
         COO(coords, data=data[:5], shape=shape)
     with pytest.raises(ValueError, match="shape of `coords`"):
         coords = np.random.randint(10, size=20).reshape(1, 20)
         COO(coords, data=data, shape=shape)
 
 
-@pytest.mark.parametrize('N, M', [(4, None), (4, 10), (10, 4), (0, 10)])
+@pytest.mark.parametrize("N, M", [(4, None), (4, 10), (10, 4), (0, 10)])
 def test_eye(N, M):
     m = M or N
     for k in [0, N - 2, N + 2, m - 2, m + 2]:
         assert_eq(sparse.eye(N, M=M, k=k), np.eye(N, M=M, k=k))
-        assert_eq(sparse.eye(N, M=M, k=k, dtype='i4'), np.eye(N, M=M, k=k, dtype='i4'))
+        assert_eq(sparse.eye(N, M=M, k=k, dtype="i4"), np.eye(N, M=M, k=k, dtype="i4"))
 
 
-@pytest.mark.parametrize('funcname', ['ones', 'zeros'])
+@pytest.mark.parametrize("funcname", ["ones", "zeros"])
 def test_ones_zeros(funcname):
     sp_func = getattr(sparse, funcname)
     np_func = getattr(np, funcname)
 
     assert_eq(sp_func(5), np_func(5))
     assert_eq(sp_func((5, 4)), np_func((5, 4)))
-    assert_eq(sp_func((5, 4), dtype='i4'), np_func((5, 4), dtype='i4'))
+    assert_eq(sp_func((5, 4), dtype="i4"), np_func((5, 4), dtype="i4"))
     assert_eq(sp_func((5, 4), dtype=None), np_func((5, 4), dtype=None))
 
 
-@pytest.mark.parametrize('funcname', ['ones_like', 'zeros_like'])
+@pytest.mark.parametrize("funcname", ["ones_like", "zeros_like"])
 def test_ones_zeros_like(funcname):
     sp_func = getattr(sparse, funcname)
     np_func = getattr(np, funcname)
 
-    x = np.ones((5, 5), dtype='i8')
+    x = np.ones((5, 5), dtype="i8")
 
     assert_eq(sp_func(x), np_func(x))
-    assert_eq(sp_func(x, dtype='f8'), np_func(x, dtype='f8'))
+    assert_eq(sp_func(x, dtype="f8"), np_func(x, dtype="f8"))
     assert_eq(sp_func(x, dtype=None), np_func(x, dtype=None))
 
 
 def test_full():
     assert_eq(sparse.full(5, 9), np.full(5, 9))
-    assert_eq(sparse.full(5, 9, dtype='f8'), np.full(5, 9, dtype='f8'))
+    assert_eq(sparse.full(5, 9, dtype="f8"), np.full(5, 9, dtype="f8"))
     assert_eq(sparse.full((5, 4), 9.5), np.full((5, 4), 9.5))
-    assert_eq(sparse.full((5, 4), 9.5, dtype='i4'), np.full((5, 4), 9.5, dtype='i4'))
+    assert_eq(sparse.full((5, 4), 9.5, dtype="i4"), np.full((5, 4), 9.5, dtype="i4"))
 
 
 def test_full_like():
-    x = np.zeros((5, 5), dtype='i8')
+    x = np.zeros((5, 5), dtype="i8")
     assert_eq(sparse.full_like(x, 9.5), np.full_like(x, 9.5))
-    assert_eq(sparse.full_like(x, 9.5, dtype='f8'), np.full_like(x, 9.5, dtype='f8'))
+    assert_eq(sparse.full_like(x, 9.5, dtype="f8"), np.full_like(x, 9.5, dtype="f8"))
 
 
-@pytest.mark.parametrize('complex', [True, False])
+@pytest.mark.parametrize("complex", [True, False])
 def test_complex_methods(complex):
     if complex:
         x = np.array([1 + 2j, 2 - 1j, 0, 1, 0])
     else:
         x = np.array([1, 2, 0, 0, 0])
     s = sparse.COO.from_numpy(x)
     assert_eq(s.imag, x.imag)
@@ -2117,79 +2069,140 @@
     x = np.random.rand(10, 1).view(type=np.matrix)
     s = sparse.COO.from_numpy(x)
 
     assert_eq(x, s)
 
 
 def test_out_dtype():
-    a = sparse.eye(5, dtype='float32')
-    b = sparse.eye(5, dtype='float64')
+    a = sparse.eye(5, dtype="float32")
+    b = sparse.eye(5, dtype="float64")
 
-    assert np.positive(a, out=b).dtype == \
-        np.positive(a.todense(), out=b.todense()).dtype
-    assert np.positive(a, out=b, dtype='float64').dtype == \
-        np.positive(a.todense(), out=b.todense(), dtype='float64').dtype
+    assert (
+        np.positive(a, out=b).dtype == np.positive(a.todense(), out=b.todense()).dtype
+    )
+    assert (
+        np.positive(a, out=b, dtype="float64").dtype
+        == np.positive(a.todense(), out=b.todense(), dtype="float64").dtype
+    )
 
 
 def test_failed_densification():
     import os
     from importlib import reload
 
-    os.environ['SPARSE_AUTO_DENSIFY'] = '1'
+    os.environ["SPARSE_AUTO_DENSIFY"] = "1"
     reload(sparse._settings)
 
     s = sparse.random((3, 4, 5), density=0.5)
     x = np.array(s)
 
     assert isinstance(x, np.ndarray)
     assert_eq(s, x)
 
-    del os.environ['SPARSE_AUTO_DENSIFY']
+    del os.environ["SPARSE_AUTO_DENSIFY"]
     reload(sparse._settings)
 
 
 def test_warn_on_too_dense():
     import os
     from importlib import reload
 
-    os.environ['SPARSE_WARN_ON_TOO_DENSE'] = '1'
+    os.environ["SPARSE_WARN_ON_TOO_DENSE"] = "1"
     reload(sparse._settings)
 
     with pytest.warns(RuntimeWarning):
         sparse.random((3, 4, 5), density=1.0)
 
-    del os.environ['SPARSE_WARN_ON_TOO_DENSE']
+    del os.environ["SPARSE_WARN_ON_TOO_DENSE"]
     reload(sparse._settings)
 
 
 def test_prune_coo():
     coords = np.array([[0, 1, 2, 3]])
     data = np.array([1, 0, 1, 2])
     s1 = COO(coords, data)
     s2 = COO(coords, data, prune=True)
     assert s2.nnz == 3
 
     # Densify s1 because it isn't canonical
     assert_eq(s1.todense(), s2, check_nnz=False)
 
 
+def test_diagonal():
+
+    a = sparse.random((4, 4), density=0.5)
+
+    assert_eq(sparse.diagonal(a, offset=0), np.diagonal(a.todense(), offset=0))
+    assert_eq(sparse.diagonal(a, offset=1), np.diagonal(a.todense(), offset=1))
+    assert_eq(sparse.diagonal(a, offset=2), np.diagonal(a.todense(), offset=2))
+
+    a = sparse.random((4, 5, 4, 6), density=0.5)
+
+    assert_eq(
+        sparse.diagonal(a, offset=0, axis1=0, axis2=2),
+        np.diagonal(a.todense(), offset=0, axis1=0, axis2=2),
+    )
+
+    assert_eq(
+        sparse.diagonal(a, offset=1, axis1=0, axis2=2),
+        np.diagonal(a.todense(), offset=1, axis1=0, axis2=2),
+    )
+
+    assert_eq(
+        sparse.diagonal(a, offset=2, axis1=0, axis2=2),
+        np.diagonal(a.todense(), offset=2, axis1=0, axis2=2),
+    )
+
+
+def test_diagonalize():
+
+    assert_eq(sparse.diagonalize(np.ones(3)), sparse.eye(3))
+
+    assert_eq(
+        sparse.diagonalize(scipy.sparse.coo_matrix(np.eye(3))),
+        sparse.diagonalize(sparse.eye(3)),
+    )
+
+    # inverse of diagonal
+    b = sparse.random((4, 3, 2), density=0.5)
+    b_diag = sparse.diagonalize(b, axis=1)
+
+    assert_eq(b, sparse.diagonal(b_diag, axis1=1, axis2=3).transpose([0, 2, 1]))
+
+
 RESULT_TYPE_DTYPES = [
-    'i1', 'i2', 'i4', 'i8', 'u1', 'u2', 'u4', 'u8',
-    'f4', 'f8', 'c8', 'c16', object,
+    "i1",
+    "i2",
+    "i4",
+    "i8",
+    "u1",
+    "u2",
+    "u4",
+    "u8",
+    "f4",
+    "f8",
+    "c8",
+    "c16",
+    object,
 ]
-@pytest.mark.parametrize('t1', RESULT_TYPE_DTYPES)
-@pytest.mark.parametrize('t2', RESULT_TYPE_DTYPES)
-@pytest.mark.parametrize('func', [
-    sparse.result_type,
-    pytest.param(
-        np.result_type,
-        marks=pytest.mark.skipif(not NEP18_ENABLED, reason="NEP18 is not enabled")
-    ),
-])
-@pytest.mark.parametrize('data', [1, [1]])  # Not the same outputs!
+
+
+@pytest.mark.parametrize("t1", RESULT_TYPE_DTYPES)
+@pytest.mark.parametrize("t2", RESULT_TYPE_DTYPES)
+@pytest.mark.parametrize(
+    "func",
+    [
+        sparse.result_type,
+        pytest.param(
+            np.result_type,
+            marks=pytest.mark.skipif(not NEP18_ENABLED, reason="NEP18 is not enabled"),
+        ),
+    ],
+)
+@pytest.mark.parametrize("data", [1, [1]])  # Not the same outputs!
 def test_result_type(t1, t2, func, data):
     a = np.array(data, dtype=t1)
     b = np.array(data, dtype=t2)
     expect = np.result_type(a, b)
     assert func(a, sparse.COO(b)) == expect
     assert func(sparse.COO(a), b) == expect
     assert func(sparse.COO(a), sparse.COO(b)) == expect
```

### Comparing `sparse-0.8.0/sparse/tests/test_dok.py` & `sparse-0.9.1/sparse/tests/test_dok.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,121 +3,106 @@
 import numpy as np
 
 import sparse
 from sparse import DOK
 from sparse._utils import assert_eq
 
 
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-])
-@pytest.mark.parametrize('density', [
-    0.1, 0.3, 0.5, 0.7
-])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4)])
+@pytest.mark.parametrize("density", [0.1, 0.3, 0.5, 0.7])
 def test_random_shape_nnz(shape, density):
-    s = sparse.random(shape, density, format='dok')
+    s = sparse.random(shape, density, format="dok")
 
     assert isinstance(s, DOK)
 
     assert s.shape == shape
     expected_nnz = density * np.prod(shape)
     assert np.floor(expected_nnz) <= s.nnz <= np.ceil(expected_nnz)
 
 
 def test_convert_to_coo():
-    s1 = sparse.random((2, 3, 4), 0.5, format='dok')
+    s1 = sparse.random((2, 3, 4), 0.5, format="dok")
     s2 = sparse.COO(s1)
 
     assert_eq(s1, s2)
 
 
 def test_convert_from_coo():
-    s1 = sparse.random((2, 3, 4), 0.5, format='coo')
+    s1 = sparse.random((2, 3, 4), 0.5, format="coo")
     s2 = DOK(s1)
 
     assert_eq(s1, s2)
 
 
 def test_convert_from_numpy():
     x = np.random.rand(2, 3, 4)
     s = DOK(x)
 
     assert_eq(x, s)
 
 
 def test_convert_to_numpy():
-    s = sparse.random((2, 3, 4), 0.5, format='dok')
+    s = sparse.random((2, 3, 4), 0.5, format="dok")
     x = s.todense()
 
     assert_eq(x, s)
 
 
-@pytest.mark.parametrize('shape, data', [
-    (2, {
-        0: 1
-    }),
-    ((2, 3), {
-        (0, 1): 3,
-        (1, 2): 4,
-    }),
-    ((2, 3, 4), {
-        (0, 1): 3,
-        (1, 2, 3): 4,
-        (1, 1): [6, 5, 4, 1]
-    }),
-])
+@pytest.mark.parametrize(
+    "shape, data",
+    [
+        (2, {0: 1}),
+        ((2, 3), {(0, 1): 3, (1, 2): 4}),
+        ((2, 3, 4), {(0, 1): 3, (1, 2, 3): 4, (1, 1): [6, 5, 4, 1]}),
+    ],
+)
 def test_construct(shape, data):
     s = DOK(shape, data)
     x = np.zeros(shape, dtype=s.dtype)
 
     for c, d in data.items():
         x[c] = d
 
     assert_eq(x, s)
 
 
-@pytest.mark.parametrize('shape', [
-    (2,),
-    (2, 3),
-    (2, 3, 4),
-])
-@pytest.mark.parametrize('density', [
-    0.1, 0.3, 0.5, 0.7
-])
+@pytest.mark.parametrize("shape", [(2,), (2, 3), (2, 3, 4)])
+@pytest.mark.parametrize("density", [0.1, 0.3, 0.5, 0.7])
 def test_getitem(shape, density):
-    s = sparse.random(shape, density, format='dok')
+    s = sparse.random(shape, density, format="dok")
     x = s.todense()
 
     for _ in range(s.nnz):
         idx = np.random.randint(np.prod(shape))
         idx = np.unravel_index(idx, shape)
 
         assert np.isclose(s[idx], x[idx])
 
 
-@pytest.mark.parametrize('shape, index, value', [
-    ((2,), slice(None), np.random.rand()),
-    ((2,), slice(1, 2), np.random.rand()),
-    ((2,), slice(0, 2), np.random.rand(2)),
-    ((2,), 1, np.random.rand()),
-    ((2, 3), (0, slice(None)), np.random.rand()),
-    ((2, 3), (0, slice(1, 3)), np.random.rand()),
-    ((2, 3), (1, slice(None)), np.random.rand(3)),
-    ((2, 3), (0, slice(1, 3)), np.random.rand(2)),
-    ((2, 3), (0, slice(2, 0, -1)), np.random.rand(2)),
-    ((2, 3), (slice(None), 1), np.random.rand()),
-    ((2, 3), (slice(None), 1), np.random.rand(2)),
-    ((2, 3), (slice(1, 2), 1), np.random.rand()),
-    ((2, 3), (slice(1, 2), 1), np.random.rand(1)),
-    ((2, 3), (0, 2), np.random.rand()),
-])
+@pytest.mark.parametrize(
+    "shape, index, value",
+    [
+        ((2,), slice(None), np.random.rand()),
+        ((2,), slice(1, 2), np.random.rand()),
+        ((2,), slice(0, 2), np.random.rand(2)),
+        ((2,), 1, np.random.rand()),
+        ((2, 3), (0, slice(None)), np.random.rand()),
+        ((2, 3), (0, slice(1, 3)), np.random.rand()),
+        ((2, 3), (1, slice(None)), np.random.rand(3)),
+        ((2, 3), (0, slice(1, 3)), np.random.rand(2)),
+        ((2, 3), (0, slice(2, 0, -1)), np.random.rand(2)),
+        ((2, 3), (slice(None), 1), np.random.rand()),
+        ((2, 3), (slice(None), 1), np.random.rand(2)),
+        ((2, 3), (slice(1, 2), 1), np.random.rand()),
+        ((2, 3), (slice(1, 2), 1), np.random.rand(1)),
+        ((2, 3), (0, 2), np.random.rand()),
+    ],
+)
 def test_setitem(shape, index, value):
-    s = sparse.random(shape, 0.5, format='dok')
+    s = sparse.random(shape, 0.5, format="dok")
     x = s.todense()
 
     s[index] = value
     x[index] = value
 
     assert_eq(x, s)
 
@@ -125,29 +110,23 @@
 def test_default_dtype():
     s = DOK((5,))
 
     assert s.dtype == np.float64
 
 
 def test_int_dtype():
-    data = {
-        1: np.uint8(1),
-        2: np.uint16(2),
-    }
+    data = {1: np.uint8(1), 2: np.uint16(2)}
 
     s = DOK((5,), data)
 
     assert s.dtype == np.uint16
 
 
 def test_float_dtype():
-    data = {
-        1: np.uint8(1),
-        2: np.float32(2),
-    }
+    data = {1: np.uint8(1), 2: np.float32(2)}
 
     s = DOK((5,), data)
 
     assert s.dtype == np.float32
 
 
 def test_set_zero():
@@ -155,24 +134,21 @@
     s[0] = 1
     s[0] = 0
 
     assert s[0] == 0
     assert s.nnz == 0
 
 
-@pytest.mark.parametrize('format', [
-    'coo',
-    'dok',
-])
+@pytest.mark.parametrize("format", ["coo", "dok"])
 def test_asformat(format):
-    s = sparse.random((2, 3, 4), density=0.5, format='dok')
+    s = sparse.random((2, 3, 4), density=0.5, format="dok")
     s2 = s.asformat(format)
 
     assert_eq(s, s2)
 
 
 def test_coo_fv_interface():
-    s1 = sparse.full((5, 5), fill_value=1+np.random.rand())
+    s1 = sparse.full((5, 5), fill_value=1 + np.random.rand())
     s2 = sparse.DOK(s1)
     assert_eq(s1, s2)
     s3 = sparse.COO(s2)
     assert_eq(s1, s3)
```

### Comparing `sparse-0.8.0/sparse/tests/test_io.py` & `sparse-0.9.1/sparse/tests/test_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 import sparse
 
 from sparse import save_npz, load_npz
 from sparse._utils import assert_eq
 
 
-@pytest.mark.parametrize('compression', [True, False])
+@pytest.mark.parametrize("compression", [True, False])
 def test_save_load_npz_file(compression):
-    x = sparse.random((2, 3, 4, 5), density=.25)
+    x = sparse.random((2, 3, 4, 5), density=0.25)
     y = x.todense()
 
     dir_name = tempfile.mkdtemp()
-    filename = os.path.join(dir_name, 'mat.npz')
+    filename = os.path.join(dir_name, "mat.npz")
 
     save_npz(filename, x, compressed=compression)
     z = load_npz(filename)
     assert_eq(x, z)
     assert_eq(y, z.todense())
 
     shutil.rmtree(dir_name)
 
 
 def test_load_wrong_format_exception():
     x = np.array([1, 2, 3])
 
     dir_name = tempfile.mkdtemp()
-    filename = os.path.join(dir_name, 'mat.npz')
+    filename = os.path.join(dir_name, "mat.npz")
 
     np.savez(filename, x)
     with pytest.raises(RuntimeError):
         load_npz(filename)
 
     shutil.rmtree(dir_name)
```

### Comparing `sparse-0.8.0/sparse.egg-info/PKG-INFO` & `sparse-0.9.1/sparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse
-Version: 0.8.0
+Version: 0.9.1
 Summary: Sparse n-dimensional arrays
 Home-page: https://github.com/pydata/sparse/
 Maintainer: Hameer Abbasi
 Maintainer-email: hameerabbasi@yahoo.com
 License: BSD 3-Clause License (Revised)
 Project-URL: Documentation, https://sparse.pydata.org/
 Project-URL: Source, https://github.com/pydata/sparse/
@@ -42,11 +42,11 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.5, <4
+Provides-Extra: docs
 Provides-Extra: tests
-Provides-Extra: all
 Provides-Extra: tox
-Provides-Extra: docs
+Provides-Extra: all
```

### Comparing `sparse-0.8.0/sparse.egg-info/SOURCES.txt` & `sparse-0.9.1/sparse.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 docs/generated/sparse.SparseArray.nnz.rst
 docs/generated/sparse.SparseArray.rst
 docs/generated/sparse.SparseArray.size.rst
 docs/generated/sparse.SparseArray.todense.rst
 docs/generated/sparse.argwhere.rst
 docs/generated/sparse.as_coo.rst
 docs/generated/sparse.concatenate.rst
+docs/generated/sparse.diagonal.rst
+docs/generated/sparse.diagonalize.rst
 docs/generated/sparse.dot.rst
 docs/generated/sparse.elemwise.rst
 docs/generated/sparse.eye.rst
 docs/generated/sparse.full.rst
 docs/generated/sparse.full_like.rst
 docs/generated/sparse.isneginf.rst
 docs/generated/sparse.isposinf.rst
@@ -111,35 +113,41 @@
 docs/generated/sparse.zeros.rst
 docs/generated/sparse.zeros_like.rst
 requirements/all.txt
 requirements/docs.txt
 requirements/tests.txt
 requirements/tox.txt
 sparse/__init__.py
+sparse/_common.py
 sparse/_dok.py
 sparse/_io.py
+sparse/_numba_extension.py
 sparse/_settings.py
 sparse/_slicing.py
 sparse/_sparse_array.py
 sparse/_utils.py
 sparse/_version.py
 sparse.egg-info/PKG-INFO
 sparse.egg-info/SOURCES.txt
 sparse.egg-info/dependency_links.txt
+sparse.egg-info/entry_points.txt
 sparse.egg-info/not-zip-safe
 sparse.egg-info/requires.txt
 sparse.egg-info/top_level.txt
 sparse/_compressed/__init__.py
+sparse/_compressed/common.py
 sparse/_compressed/compressed.py
 sparse/_compressed/convert.py
 sparse/_compressed/indexing.py
 sparse/_coo/__init__.py
 sparse/_coo/common.py
 sparse/_coo/core.py
 sparse/_coo/indexing.py
+sparse/_coo/numba_extension.py
 sparse/_coo/umath.py
 sparse/tests/conftest.py
 sparse/tests/test_array_function.py
 sparse/tests/test_compressed.py
 sparse/tests/test_coo.py
+sparse/tests/test_coo_numba.py
 sparse/tests/test_dok.py
 sparse/tests/test_io.py
```

### Comparing `sparse-0.8.0/versioneer.py` & `sparse-0.9.1/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -273,14 +272,15 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,33 +304,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(me), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -344,14 +348,15 @@
         parser.readfp(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
+
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -368,36 +373,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            p = subprocess.Popen(
+                [c] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -414,15 +423,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY[
+    "git"
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -989,71 +1000,86 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = run_command(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            "%s*" % tag_prefix,
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1068,54 +1094,55 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1163,24 +1190,30 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1201,29 +1234,30 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1247,16 +1281,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1362,19 +1395,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1386,17 +1421,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1411,16 +1450,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1466,17 +1506,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1517,14 +1561,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1549,22 +1594,23 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1577,25 +1623,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1606,21 +1656,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1639,16 +1693,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1695,36 +1751,41 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        EnvironmentError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1758,16 +1819,18 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
+        print(
+            " appending versionfile_source ('%s') to MANIFEST.in"
+            % cfg.versionfile_source
+        )
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

