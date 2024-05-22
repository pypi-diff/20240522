# Comparing `tmp/oras-0.1.29.tar.gz` & `tmp/oras-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.29.tar", last modified: Fri Apr  5 17:27:10 2024, max compression
+gzip compressed data, was "oras-0.1.30.tar", last modified: Wed May 22 12:55:37 2024, max compression
```

## Comparing `oras-0.1.29.tar` & `oras-0.1.30.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-05 17:27:00.000000 oras-0.1.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 17:27:00.000000 oras-0.1.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-05 17:27:10.293628 oras-0.1.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-05 17:27:00.000000 oras-0.1.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 17:27:00.000000 oras-0.1.29/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-05 17:27:00.000000 oras-0.1.29/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-05 17:27:00.000000 oras-0.1.29/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-05 17:27:00.000000 oras-0.1.29/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-05 17:27:00.000000 oras-0.1.29/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-05 17:27:00.000000 oras-0.1.29/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-05 17:27:00.000000 oras-0.1.29/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/main/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:00.000000 oras-0.1.29/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 17:27:00.000000 oras-0.1.29/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-05 17:27:00.000000 oras-0.1.29/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    39049 2024-04-05 17:27:00.000000 oras-0.1.29/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-05 17:27:00.000000 oras-0.1.29/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/artifact.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-05 17:27:00.000000 oras-0.1.29/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-05 17:27:00.000000 oras-0.1.29/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-05 17:27:00.000000 oras-0.1.29/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 17:27:00.000000 oras-0.1.29/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:27:02.000000 oras-0.1.29/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 17:27:00.000000 oras-0.1.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 17:27:10.297628 oras-0.1.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-05 17:27:00.000000 oras-0.1.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.349274 oras-0.1.30/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-22 12:55:26.000000 oras-0.1.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-22 12:55:26.000000 oras-0.1.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-22 12:55:37.349274 oras-0.1.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-22 12:55:26.000000 oras-0.1.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.345274 oras-0.1.30/oras/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 12:55:26.000000 oras-0.1.30/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-22 12:55:26.000000 oras-0.1.30/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-05-22 12:55:26.000000 oras-0.1.30/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-22 12:55:26.000000 oras-0.1.30/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-22 12:55:26.000000 oras-0.1.30/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-22 12:55:26.000000 oras-0.1.30/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-22 12:55:26.000000 oras-0.1.30/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.349274 oras-0.1.30/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:26.000000 oras-0.1.30/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 12:55:26.000000 oras-0.1.30/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-22 12:55:26.000000 oras-0.1.30/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38970 2024-05-22 12:55:26.000000 oras-0.1.30/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-22 12:55:26.000000 oras-0.1.30/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.349274 oras-0.1.30/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/artifact.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/test_oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.349274 oras-0.1.30/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 12:55:26.000000 oras-0.1.30/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.349274 oras-0.1.30/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 12:55:26.000000 oras-0.1.30/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-05-22 12:55:26.000000 oras-0.1.30/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-22 12:55:26.000000 oras-0.1.30/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 12:55:26.000000 oras-0.1.30/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:55:37.349274 oras-0.1.30/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-22 12:55:37.000000 oras-0.1.30/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-22 12:55:37.000000 oras-0.1.30/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:55:37.000000 oras-0.1.30/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:55:29.000000 oras-0.1.30/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 12:55:37.000000 oras-0.1.30/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 12:55:37.000000 oras-0.1.30/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 12:55:26.000000 oras-0.1.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 12:55:37.349274 oras-0.1.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-22 12:55:26.000000 oras-0.1.30/setup.py
```

### Comparing `oras-0.1.29/LICENSE` & `oras-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/PKG-INFO` & `oras-0.1.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.29
+Version: 0.1.30
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-20-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -72,14 +72,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://saketjajoo.github.io"><img src="https://avatars.githubusercontent.com/u/23132557?v=4?s=100" width="100px;" alt="Saket Jajoo"/><br /><sub><b>Saket Jajoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=saketjajoo" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/miker985"><img src="https://avatars.githubusercontent.com/u/26555712?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=miker985" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/linshokaku"><img src="https://avatars.githubusercontent.com/u/18627646?v=4?s=100" width="100px;" alt="deoxy"/><br /><sub><b>deoxy</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=linshokaku" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kavish-p"><img src="https://avatars.githubusercontent.com/u/29086148?v=4?s=100" width="100px;" alt="Kavish Punchoo"/><br /><sub><b>Kavish Punchoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=kavish-p" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/my5cents"><img src="https://avatars.githubusercontent.com/u/4820203?v=4?s=100" width="100px;" alt="my5cents"/><br /><sub><b>my5cents</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=my5cents" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tumido"><img src="https://avatars.githubusercontent.com/u/7453394?v=4?s=100" width="100px;" alt="Tom Coufal"/><br /><sub><b>Tom Coufal</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=tumido" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.29 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.30 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python [![All Contributors](https://img.shields.io/badge/
-all_contributors-19-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
+all_contributors-20-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
 (https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
@@ -28,13 +28,13 @@
                 _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»       _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
                   _ð___»    _ð___»                    _ð___»      _ð___»      _ð___»
 _[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s   _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
  _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr   _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
      _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»        _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
                           _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm   _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
                           _ð___»                    _ð___»      _ð___»
- _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]
-  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss
-     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»
-                                     _PP_uu_nn_cc_hh_oo_oo
-                                      _ð___»
+ _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]   _[_T_o_m
+  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss  _C_o_u_f_a_l_]
+     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»      _TT_oo_mm
+                                     _PP_uu_nn_cc_hh_oo_oo               _CC_oo_uu_ff_aa_ll
+                                      _ð___»                  _ð___»
 ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.29/README.md` & `oras-0.1.30/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-20-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -47,14 +47,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://saketjajoo.github.io"><img src="https://avatars.githubusercontent.com/u/23132557?v=4?s=100" width="100px;" alt="Saket Jajoo"/><br /><sub><b>Saket Jajoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=saketjajoo" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/miker985"><img src="https://avatars.githubusercontent.com/u/26555712?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=miker985" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/linshokaku"><img src="https://avatars.githubusercontent.com/u/18627646?v=4?s=100" width="100px;" alt="deoxy"/><br /><sub><b>deoxy</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=linshokaku" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kavish-p"><img src="https://avatars.githubusercontent.com/u/29086148?v=4?s=100" width="100px;" alt="Kavish Punchoo"/><br /><sub><b>Kavish Punchoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=kavish-p" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/my5cents"><img src="https://avatars.githubusercontent.com/u/4820203?v=4?s=100" width="100px;" alt="my5cents"/><br /><sub><b>my5cents</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=my5cents" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tumido"><img src="https://avatars.githubusercontent.com/u/7453394?v=4?s=100" width="100px;" alt="Tom Coufal"/><br /><sub><b>Tom Coufal</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=tumido" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # ORAS Python [![All Contributors](https://img.shields.io/badge/
-all_contributors-19-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
+all_contributors-20-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
 (https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
@@ -17,13 +17,13 @@
                 _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»       _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
                   _ð___»    _ð___»                    _ð___»      _ð___»      _ð___»
 _[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s   _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
  _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr   _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
      _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»        _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
                           _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm   _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
                           _ð___»                    _ð___»      _ð___»
- _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]
-  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss
-     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»
-                                     _PP_uu_nn_cc_hh_oo_oo
-                                      _ð___»
+ _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]   _[_T_o_m
+  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss  _C_o_u_f_a_l_]
+     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»      _TT_oo_mm
+                                     _PP_uu_nn_cc_hh_oo_oo               _CC_oo_uu_ff_aa_ll
+                                      _ð___»                  _ð___»
 ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.29/oras/auth.py` & `oras-0.1.30/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/client.py` & `oras-0.1.30/oras/client.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/container.py` & `oras-0.1.30/oras/container.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/decorator.py` & `oras-0.1.30/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/defaults.py` & `oras-0.1.30/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/logger.py` & `oras-0.1.30/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/main/login.py` & `oras-0.1.30/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/oci.py` & `oras-0.1.30/oras/oci.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
 import copy
+import hashlib
+import json
 import os
+from dataclasses import dataclass
 from typing import Dict, Optional, Tuple
 
 import jsonschema
 
 import oras.defaults
 import oras.schemas
 import oras.utils
@@ -147,7 +150,31 @@
 
 
 def NewManifest() -> dict:
     """
     Get an empty manifest config.
     """
     return copy.deepcopy(EmptyManifest)
+
+
+@dataclass
+class Subject:
+    mediaType: str
+    digest: str
+    size: int
+
+    @classmethod
+    def from_manifest(cls, manifest: dict) -> "Subject":
+        """
+        Create a new Subject from a Manifest
+
+        :param manifest: manifest to convert to subject
+        """
+        manifest_string = json.dumps(manifest).encode("utf-8")
+        digest = "sha256:" + hashlib.sha256(manifest_string).hexdigest()
+        size = len(manifest_string)
+
+        return cls(
+            manifest["mediaType"] or oras.defaults.default_manifest_media_type,
+            digest,
+            size,
+        )
```

### Comparing `oras-0.1.29/oras/provider.py` & `oras-0.1.30/oras/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
 import copy
 import os
 import urllib
 from contextlib import contextmanager, nullcontext
-from dataclasses import asdict, dataclass
+from dataclasses import asdict
 from http.cookiejar import DefaultCookiePolicy
 from tempfile import TemporaryDirectory
 from typing import Callable, Generator, List, Optional, Tuple, Union
 
 import jsonschema
 import requests
 
@@ -31,21 +31,14 @@
 def temporary_empty_config() -> Generator[str, None, None]:
     with TemporaryDirectory() as tmpdir:
         config_file = oras.utils.get_tmpfile(tmpdir=tmpdir, suffix=".json")
         oras.utils.write_file(config_file, "{}")
         yield config_file
 
 
-@dataclass
-class Subject:
-    mediaType: str
-    digest: str
-    size: int
-
-
 class Registry:
     """
     Direct interactions with an OCI registry.
 
     This could also be called a "provider" when we add in the "copy" logic
     and the registry isn't necessarily the "remote" endpoint.
     """
@@ -693,15 +686,15 @@
         :param manifest_annotations: manifest annotations
         :type manifest_annotations: dict
         :param target: target location to push to
         :type target: str
         :param refresh_headers: if true or None, headers are refreshed
         :type refresh_headers: bool
         :param subject: optional subject reference
-        :type subject: Subject
+        :type subject: oras.oci.Subject
         """
         container = self.get_container(kwargs["target"])
         self.load_configs(container, configs=kwargs.get("config_path"))
 
         # Hold state of request for http/https
         validate_path = not kwargs.get("disable_path_validation", False)
```

### Comparing `oras-0.1.29/oras/schemas.py` & `oras-0.1.30/oras/schemas.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/tests/conftest.py` & `oras-0.1.30/oras/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/tests/test_oras.py` & `oras-0.1.30/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/tests/test_provider.py` & `oras-0.1.30/oras/tests/test_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 from pathlib import Path
 
 import pytest
 
 import oras.client
 import oras.defaults
+import oras.oci
 import oras.provider
 import oras.utils
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 @pytest.mark.with_auth(False)
```

### Comparing `oras-0.1.29/oras/tests/test_utils.py` & `oras-0.1.30/oras/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/utils/fileio.py` & `oras-0.1.30/oras/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/utils/request.py` & `oras-0.1.30/oras/utils/request.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.29/oras/version.py` & `oras-0.1.30/oras/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.29"
+__version__ = "0.1.30"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.29/oras.egg-info/PKG-INFO` & `oras-0.1.30/oras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.29
+Version: 0.1.30
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-20-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -72,14 +72,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://saketjajoo.github.io"><img src="https://avatars.githubusercontent.com/u/23132557?v=4?s=100" width="100px;" alt="Saket Jajoo"/><br /><sub><b>Saket Jajoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=saketjajoo" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/miker985"><img src="https://avatars.githubusercontent.com/u/26555712?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=miker985" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/linshokaku"><img src="https://avatars.githubusercontent.com/u/18627646?v=4?s=100" width="100px;" alt="deoxy"/><br /><sub><b>deoxy</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=linshokaku" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kavish-p"><img src="https://avatars.githubusercontent.com/u/29086148?v=4?s=100" width="100px;" alt="Kavish Punchoo"/><br /><sub><b>Kavish Punchoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=kavish-p" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/my5cents"><img src="https://avatars.githubusercontent.com/u/4820203?v=4?s=100" width="100px;" alt="my5cents"/><br /><sub><b>my5cents</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=my5cents" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tumido"><img src="https://avatars.githubusercontent.com/u/7453394?v=4?s=100" width="100px;" alt="Tom Coufal"/><br /><sub><b>Tom Coufal</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=tumido" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.29 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.30 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python [![All Contributors](https://img.shields.io/badge/
-all_contributors-19-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
+all_contributors-20-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
 (https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
@@ -28,13 +28,13 @@
                 _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»       _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
                   _ð___»    _ð___»                    _ð___»      _ð___»      _ð___»
 _[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s   _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
  _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr   _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
      _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»        _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
                           _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm   _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
                           _ð___»                    _ð___»      _ð___»
- _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]
-  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss
-     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»
-                                     _PP_uu_nn_cc_hh_oo_oo
-                                      _ð___»
+ _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]   _[_T_o_m
+  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss  _C_o_u_f_a_l_]
+     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»      _TT_oo_mm
+                                     _PP_uu_nn_cc_hh_oo_oo               _CC_oo_uu_ff_aa_ll
+                                      _ð___»                  _ð___»
 ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.29/oras.egg-info/SOURCES.txt` & `oras-0.1.30/oras.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 oras/main/__init__.py
 oras/main/login.py
 oras/tests/__init__.py
 oras/tests/annotations.json
 oras/tests/artifact.txt
 oras/tests/conftest.py
 oras/tests/run_registry.sh
+oras/tests/test_oci.py
 oras/tests/test_oras.py
 oras/tests/test_provider.py
 oras/tests/test_utils.py
 oras/tests/upload_data/artifact.txt
 oras/utils/__init__.py
 oras/utils/fileio.py
 oras/utils/request.py
```

### Comparing `oras-0.1.29/setup.py` & `oras-0.1.30/setup.py`

 * *Files identical despite different names*

