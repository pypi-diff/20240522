# Comparing `tmp/pocket_coffea-1.0rc2.tar.gz` & `tmp/pocket_coffea-1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocket_coffea-1.0rc2.tar", last modified: Mon Oct  9 21:00:13 2023, max compression
+gzip compressed data, was "pocket_coffea-1.0rc3.tar", last modified: Tue Oct 10 07:02:02 2023, max compression
```

## Comparing `pocket_coffea-1.0rc2.tar` & `pocket_coffea-1.0rc3.tar`

### file list

```diff
@@ -1,508 +1,508 @@
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.629052 pocket_coffea-1.0rc2/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      119 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.flake8
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      125 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.git_archival.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       32 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.gitattributes
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.361074 pocket_coffea-1.0rc2/.github/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2405 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.github/CONTRIBUTING.md
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      163 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.github/dependabot.yml
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.364074 pocket_coffea-1.0rc2/.github/matchers/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      668 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.github/matchers/pylint.json
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.366074 pocket_coffea-1.0rc2/.github/workflows/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2320 2023-08-21 09:28:59.000000 pocket_coffea-1.0rc2/.github/workflows/ci.yml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2193 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.gitignore
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2276 2023-08-11 20:33:24.000000 pocket_coffea-1.0rc2/.gitlab-ci.yml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2811 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2866 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.pyproject_621.toml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      396 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/.readthedocs.yml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      656 2023-08-11 20:33:24.000000 pocket_coffea-1.0rc2/Dockerfile
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1528 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/LICENSE
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-06-15 11:17:16.000000 pocket_coffea-1.0rc2/MANIFEST.in
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4083 2023-10-09 21:00:13.629052 pocket_coffea-1.0rc2/PKG-INFO
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2572 2023-06-20 15:50:43.000000 pocket_coffea-1.0rc2/README.md
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8781 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/README_old.md
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1880 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/noxfile.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.377074 pocket_coffea-1.0rc2/pocket_coffea/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      250 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc2/pocket_coffea/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      465 2023-10-09 20:55:20.000000 pocket_coffea-1.0rc2/pocket_coffea/_version.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      118 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/_version.pyi
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.434073 pocket_coffea-1.0rc2/pocket_coffea/lib/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    18552 2023-06-19 09:09:17.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/categorization.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7410 2023-08-11 21:53:54.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/columns_manager.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2525 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/cut_definition.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10391 2023-05-05 11:27:53.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/cut_functions.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8598 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/deltaR_matching.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    33055 2023-08-21 09:58:18.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/hist_manager.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9338 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/jets.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5232 2023-05-25 16:41:04.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/leptons.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       43 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/objects.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9121 2023-07-04 13:28:25.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/parton_provenance.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26056 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/reconstruction.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15676 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/scale_factors.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2258 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/triggers.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16046 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/lib/weights_manager.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.476072 pocket_coffea-1.0rc2/pocket_coffea/parameters/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       24 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/__init__.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.489072 pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9336 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9387 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2637 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4048 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4101 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1520 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/btagging.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      181 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/cuts.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      848 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/dask_env.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.497072 pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    11686 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15830 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15616 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5569 2023-06-20 09:43:20.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/defaults.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1323 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/event_flags.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13181 2023-06-21 15:11:53.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/histograms.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.069062 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40541 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40538 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41031 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39763 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38575 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38572 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39465 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    37960 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1810 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1794 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7391 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7386 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7371 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7425 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2413 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2440 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1826 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1789 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7389 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7039 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7364 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PF.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PF.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4222 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4217 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4268 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1817 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1811 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    95855 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    90742 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   100572 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    65138 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    91966 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    63555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2432 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2409 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7095 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7336 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7325 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173413 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173478 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2587 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jec_config.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1429 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jet_scale_factors.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13003 2023-05-23 08:53:32.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/jets_calibration.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3201 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/lepton_scale_factors.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45900 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/lumi.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      977 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/lumi.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      672 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/pileup.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1824 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/plotting_style.yaml
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.305075 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.077062 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    54894 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_phi_leading_2017_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48984 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_pt_leading_2017_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34659 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_phi_pt_leading_2017_Ele32_EleHT_pass.json
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.108061 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19688 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19728 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19807 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19726 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14692 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14724 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14794 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14721 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8517 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8547 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8588 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8552 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.468055 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10370 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v05.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v07.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v08.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v09.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v10.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v11.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v12.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v13.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v14.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v15.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19663 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19663 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    32392 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v05.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v07.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v08.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    64399 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v09.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16291 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16291 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26777 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    58725 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10682 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8705 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8705 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9225 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9225 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15002 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41466 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6238 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v05.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v07.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v08.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v09.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v10.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v11.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v12.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v13.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v14.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v15.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v16.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v17.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v18.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v19.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v20.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v21.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v22.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v23.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v24.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v25.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v26.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v27.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v28.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v29.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v30.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v31.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v32.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v33.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v34.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v35.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    23172 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    23172 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31656 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31653 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31653 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68662 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68659 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68659 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48639 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48639 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45165 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31635 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31630 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31630 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68624 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68626 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68626 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44287 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44284 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    43386 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6124 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6122 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6064 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2925 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2926 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2926 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7185 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v03.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v04.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v05.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v07.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v08.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v09.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v10.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v11.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2857 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2858 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2858 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v02.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2872 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2873 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v01.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2873 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v02.json
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.478055 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    58051 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    52902 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41467 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.489055 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    54868 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_phi_leading_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48959 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_pt_leading_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34639 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_phi_pt_leading_2018_Ele32_EleHT_pass_v06.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      619 2023-08-21 09:58:11.000000 pocket_coffea-1.0rc2/pocket_coffea/parameters/variations.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/py.typed
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.530054 pocket_coffea-1.0rc2/pocket_coffea/utils/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2812 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/build_jets_calibrator.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26297 2023-08-11 20:40:20.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/configurator.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13581 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/dataset.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      193 2023-06-20 09:07:30.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/load_output.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4644 2022-11-20 17:13:41.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/logging.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      910 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/network.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    55055 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/plot_efficiency.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7472 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/plot_sf.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39639 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/plot_utils.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6614 2023-07-05 16:40:29.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/rucio.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10977 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/run.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2517 2023-07-05 13:00:35.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/skim.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2646 2023-07-05 13:03:18.000000 pocket_coffea-1.0rc2/pocket_coffea/utils/utils.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.546054 pocket_coffea-1.0rc2/pocket_coffea/workflows/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/workflows/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34647 2023-08-30 09:36:12.000000 pocket_coffea-1.0rc2/pocket_coffea/workflows/base.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1665 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc2/pocket_coffea/workflows/genweights.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1589 2023-02-28 09:29:31.000000 pocket_coffea-1.0rc2/pocket_coffea/workflows/semileptonic_triggerSF.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1581 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pocket_coffea/workflows/sf_lepton_variations.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4686 2023-05-05 11:27:53.000000 pocket_coffea-1.0rc2/pocket_coffea/workflows/tthbb_base_processor.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:12.392073 pocket_coffea-1.0rc2/pocket_coffea.egg-info/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4083 2023-10-09 21:00:11.000000 pocket_coffea-1.0rc2/pocket_coffea.egg-info/PKG-INFO
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44386 2023-10-09 21:00:12.000000 pocket_coffea-1.0rc2/pocket_coffea.egg-info/SOURCES.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        1 2023-10-09 21:00:11.000000 pocket_coffea-1.0rc2/pocket_coffea.egg-info/dependency_links.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      448 2023-10-09 21:00:11.000000 pocket_coffea-1.0rc2/pocket_coffea.egg-info/requires.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       14 2023-10-09 21:00:11.000000 pocket_coffea-1.0rc2/pocket_coffea.egg-info/top_level.txt
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.566053 pocket_coffea-1.0rc2/profiling/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1882 2022-06-15 09:24:30.000000 pocket_coffea-1.0rc2/profiling/mem.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703383 2022-06-29 14:04:29.000000 pocket_coffea-1.0rc2/profiling/parton_matching_semilep_newgenmatch_v4.prof
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703285 2022-06-29 14:04:29.000000 pocket_coffea-1.0rc2/profiling/parton_matching_semilep_v3.prof
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1131 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/pyproject.toml
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.591053 pocket_coffea-1.0rc2/scripts/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8969 2023-05-30 08:29:35.000000 pocket_coffea-1.0rc2/scripts/build_jec.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6976 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/scripts/compute_btagSF_calibration.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.603052 pocket_coffea-1.0rc2/scripts/dataset/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1100 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/scripts/dataset/append_genweights.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1508 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc2/scripts/dataset/append_parents.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2142 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/scripts/dataset/build_datasets.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2185 2023-02-28 08:58:11.000000 pocket_coffea-1.0rc2/scripts/dataset/download.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3275 2023-02-28 08:58:11.000000 pocket_coffea-1.0rc2/scripts/hadd_skimmed_files.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.609053 pocket_coffea-1.0rc2/scripts/lumi/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1302 2023-02-28 09:34:38.000000 pocket_coffea-1.0rc2/scripts/lumi/filter_lumi_json.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1741 2023-02-28 09:34:38.000000 pocket_coffea-1.0rc2/scripts/lumi/run_brilcalc.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      580 2023-05-18 10:10:56.000000 pocket_coffea-1.0rc2/scripts/merge_outputs.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.618052 pocket_coffea-1.0rc2/scripts/plot/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4201 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/scripts/plot/make_plots.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8656 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/scripts/plot/trigger_efficiency.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2060 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/scripts/plot/trigger_scalefactor.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19389 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc2/scripts/runner.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2194 2023-10-09 21:00:13.634052 pocket_coffea-1.0rc2/setup.cfg
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/setup.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-09 21:00:13.626052 pocket_coffea-1.0rc2/tests/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      776 2023-02-07 15:21:45.000000 pocket_coffea-1.0rc2/tests/test_categorization.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1696 2022-11-20 17:13:42.000000 pocket_coffea-1.0rc2/tests/test_hlt_cut.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      109 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc2/tests/test_package.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.400091 pocket_coffea-1.0rc3/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      119 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.flake8
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      125 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.git_archival.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       32 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.gitattributes
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.147113 pocket_coffea-1.0rc3/.github/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2405 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.github/CONTRIBUTING.md
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      163 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.github/dependabot.yml
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.150113 pocket_coffea-1.0rc3/.github/matchers/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      668 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.github/matchers/pylint.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.153113 pocket_coffea-1.0rc3/.github/workflows/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2320 2023-08-21 09:28:59.000000 pocket_coffea-1.0rc3/.github/workflows/ci.yml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2193 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.gitignore
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2276 2023-08-11 20:33:24.000000 pocket_coffea-1.0rc3/.gitlab-ci.yml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2811 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2866 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.pyproject_621.toml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      396 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.readthedocs.yml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      656 2023-08-11 20:33:24.000000 pocket_coffea-1.0rc3/Dockerfile
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1528 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/LICENSE
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-06-15 11:17:16.000000 pocket_coffea-1.0rc3/MANIFEST.in
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4083 2023-10-10 07:02:02.401091 pocket_coffea-1.0rc3/PKG-INFO
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2572 2023-06-20 15:50:43.000000 pocket_coffea-1.0rc3/README.md
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8781 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/README_old.md
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1880 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/noxfile.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.163113 pocket_coffea-1.0rc3/pocket_coffea/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      250 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/pocket_coffea/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      465 2023-10-09 20:55:20.000000 pocket_coffea-1.0rc3/pocket_coffea/_version.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      118 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/_version.pyi
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.214112 pocket_coffea-1.0rc3/pocket_coffea/lib/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    18552 2023-06-19 09:09:17.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/categorization.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7410 2023-08-11 21:53:54.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/columns_manager.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2525 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/cut_definition.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10391 2023-05-05 11:27:53.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/cut_functions.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8598 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/deltaR_matching.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    33055 2023-08-21 09:58:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/hist_manager.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9338 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/jets.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5232 2023-05-25 16:41:04.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/leptons.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       43 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/objects.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9121 2023-07-04 13:28:25.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/parton_provenance.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26056 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/reconstruction.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15676 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/scale_factors.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2258 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/triggers.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16046 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/weights_manager.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.255111 pocket_coffea-1.0rc3/pocket_coffea/parameters/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       24 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/__init__.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.267111 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9336 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9387 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2637 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4048 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4101 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1520 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btagging.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      181 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/cuts.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      848 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/dask_env.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.275111 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    11686 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15830 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15616 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5569 2023-06-20 09:43:20.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/defaults.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1323 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/event_flags.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13181 2023-06-21 15:11:53.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/histograms.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.822101 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40541 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40538 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41031 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39763 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38575 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38572 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39465 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    37960 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1810 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1794 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7391 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7386 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7371 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7425 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2413 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2440 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1826 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1789 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7389 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7039 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7364 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PF.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PF.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4222 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4217 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4268 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1817 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1811 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    95855 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    90742 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   100572 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    65138 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    91966 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    63555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2432 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2409 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7095 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7336 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7325 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173413 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173478 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2587 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec_config.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1429 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jet_scale_factors.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13003 2023-05-23 08:53:32.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jets_calibration.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3201 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/lepton_scale_factors.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45900 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      977 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      672 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/pileup.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1824 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/plotting_style.yaml
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.091114 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.830101 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    54894 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_phi_leading_2017_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48984 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_pt_leading_2017_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34659 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_phi_pt_leading_2017_Ele32_EleHT_pass.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.861101 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19688 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19728 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19807 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19726 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14692 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14724 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14794 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14721 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8517 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8547 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8588 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8552 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.239094 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10370 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v10.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v11.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v12.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v13.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v14.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v15.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19663 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19663 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    32392 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    64399 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16291 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16291 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26777 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    58725 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10682 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8705 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8705 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9225 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9225 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15002 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41466 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6238 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v10.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v11.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v12.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v13.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v14.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v15.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v16.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v17.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v18.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v19.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v20.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v21.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v22.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v23.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v24.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v25.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v26.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v27.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v28.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v29.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v30.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v31.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v32.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v33.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v34.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v35.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    23172 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    23172 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31656 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31653 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31653 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68662 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68659 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68659 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48639 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48639 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45165 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31635 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31630 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31630 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68624 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68626 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68626 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44287 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44284 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    43386 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6124 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6122 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6064 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2925 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2926 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2926 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7185 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v10.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v11.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2857 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2858 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2858 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2872 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2873 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2873 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v02.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.250094 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    58051 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    52902 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41467 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.261094 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    54868 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_phi_leading_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48959 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_pt_leading_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34639 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_phi_pt_leading_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      619 2023-08-21 09:58:11.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/variations.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/py.typed
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.300093 pocket_coffea-1.0rc3/pocket_coffea/utils/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2812 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/build_jets_calibrator.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26297 2023-08-11 20:40:20.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/configurator.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13581 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/dataset.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      193 2023-06-20 09:07:30.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/load_output.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4644 2022-11-20 17:13:41.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/logging.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      910 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/network.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    55055 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/plot_efficiency.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7472 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/plot_sf.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39639 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/plot_utils.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6614 2023-07-05 16:40:29.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/rucio.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10867 2023-10-10 07:00:58.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/run.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2517 2023-07-05 13:00:35.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/skim.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2646 2023-07-05 13:03:18.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/utils.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.316093 pocket_coffea-1.0rc3/pocket_coffea/workflows/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34647 2023-08-30 09:36:12.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/base.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1665 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/genweights.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1589 2023-02-28 09:29:31.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/semileptonic_triggerSF.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1581 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/sf_lepton_variations.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4686 2023-05-05 11:27:53.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/tthbb_base_processor.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.176113 pocket_coffea-1.0rc3/pocket_coffea.egg-info/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4083 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/PKG-INFO
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44386 2023-10-10 07:02:00.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/SOURCES.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        1 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/dependency_links.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      448 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/requires.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       14 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/top_level.txt
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.337092 pocket_coffea-1.0rc3/profiling/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1882 2022-06-15 09:24:30.000000 pocket_coffea-1.0rc3/profiling/mem.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703383 2022-06-29 14:04:29.000000 pocket_coffea-1.0rc3/profiling/parton_matching_semilep_newgenmatch_v4.prof
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703285 2022-06-29 14:04:29.000000 pocket_coffea-1.0rc3/profiling/parton_matching_semilep_v3.prof
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1131 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pyproject.toml
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.363092 pocket_coffea-1.0rc3/scripts/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8969 2023-05-30 08:29:35.000000 pocket_coffea-1.0rc3/scripts/build_jec.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6976 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/scripts/compute_btagSF_calibration.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.375092 pocket_coffea-1.0rc3/scripts/dataset/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1100 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/scripts/dataset/append_genweights.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1508 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/scripts/dataset/append_parents.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2142 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/dataset/build_datasets.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2185 2023-02-28 08:58:11.000000 pocket_coffea-1.0rc3/scripts/dataset/download.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3275 2023-02-28 08:58:11.000000 pocket_coffea-1.0rc3/scripts/hadd_skimmed_files.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.381092 pocket_coffea-1.0rc3/scripts/lumi/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1302 2023-02-28 09:34:38.000000 pocket_coffea-1.0rc3/scripts/lumi/filter_lumi_json.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1741 2023-02-28 09:34:38.000000 pocket_coffea-1.0rc3/scripts/lumi/run_brilcalc.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      580 2023-05-18 10:10:56.000000 pocket_coffea-1.0rc3/scripts/merge_outputs.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.389092 pocket_coffea-1.0rc3/scripts/plot/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4201 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/plot/make_plots.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8656 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/plot/trigger_efficiency.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2060 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/scripts/plot/trigger_scalefactor.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19389 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/runner.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2194 2023-10-10 07:02:02.404091 pocket_coffea-1.0rc3/setup.cfg
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/setup.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.398091 pocket_coffea-1.0rc3/tests/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      776 2023-02-07 15:21:45.000000 pocket_coffea-1.0rc3/tests/test_categorization.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1696 2022-11-20 17:13:42.000000 pocket_coffea-1.0rc3/tests/test_hlt_cut.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      109 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/tests/test_package.py
```

### Comparing `pocket_coffea-1.0rc2/.github/CONTRIBUTING.md` & `pocket_coffea-1.0rc3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/.github/matchers/pylint.json` & `pocket_coffea-1.0rc3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/.github/workflows/ci.yml` & `pocket_coffea-1.0rc3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/.gitignore` & `pocket_coffea-1.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/.gitlab-ci.yml` & `pocket_coffea-1.0rc3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/.pre-commit-config.yaml` & `pocket_coffea-1.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/.pyproject_621.toml` & `pocket_coffea-1.0rc3/.pyproject_621.toml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/Dockerfile` & `pocket_coffea-1.0rc3/Dockerfile`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/LICENSE` & `pocket_coffea-1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/PKG-INFO` & `pocket_coffea-1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocket_coffea
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: Configurable analysis framework based on Coffea for CMS NanoAOD events analysis
 Home-page: https://github.com/PocketCoffea/PocketCoffea
 Author: Davide Valsecchi,Matteo Marchegiani
 Author-email: davide.valsecchi@cern.ch,matteo.marchegiani@cern.ch
 License: BSD-3-Clause
 Project-URL: Documentation, https://PocketCoffea.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/PocketCoffea/PocketCoffea/issues
```

### Comparing `pocket_coffea-1.0rc2/README.md` & `pocket_coffea-1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/README_old.md` & `pocket_coffea-1.0rc3/README_old.md`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/noxfile.py` & `pocket_coffea-1.0rc3/noxfile.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/categorization.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/categorization.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/columns_manager.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/columns_manager.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/cut_definition.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/cut_definition.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/cut_functions.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/cut_functions.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/deltaR_matching.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/deltaR_matching.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/hist_manager.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/hist_manager.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/jets.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/jets.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/leptons.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/leptons.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/parton_provenance.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/parton_provenance.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/reconstruction.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/reconstruction.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/scale_factors.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/scale_factors.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/triggers.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/triggers.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/lib/weights_manager.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/weights_manager.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/btagging.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btagging.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/dask_env.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/dask_env.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/defaults.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/defaults.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/event_flags.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/event_flags.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/histograms.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/histograms.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jec_config.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec_config.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jet_scale_factors.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jet_scale_factors.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/jets_calibration.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jets_calibration.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/lepton_scale_factors.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/lepton_scale_factors.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/lumi.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/lumi.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/pileup.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/pileup.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/plotting_style.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/plotting_style.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_phi_leading_2017_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_phi_leading_2017_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_pt_leading_2017_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_pt_leading_2017_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_phi_pt_leading_2017_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_phi_pt_leading_2017_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v05.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v05.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v07.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v07.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v08.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v08.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v09.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v09.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v10.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v10.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v11.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v11.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v12.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v12.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v13.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v13.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v14.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v14.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v15.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v15.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v05.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v05.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v07.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v07.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v08.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v08.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v09.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v09.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v05.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v05.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v07.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v07.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v08.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v08.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v09.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v09.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v10.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v10.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v11.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v11.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v12.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v12.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v13.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v13.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v14.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v14.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v15.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v15.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v16.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v16.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v17.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v17.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v18.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v18.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v19.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v19.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v20.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v20.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v21.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v21.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v22.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v22.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v23.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v23.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v24.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v24.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v25.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v25.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v26.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v26.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v27.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v27.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v28.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v28.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v29.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v29.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v30.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v30.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v31.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v31.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v32.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v32.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v33.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v33.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v34.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v34.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v35.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v35.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v03.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v03.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v04.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v04.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v05.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v05.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v07.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v07.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v08.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v08.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v09.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v09.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v10.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v10.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v11.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v11.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v01.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v01.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v02.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v02.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_phi_leading_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_phi_leading_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_pt_leading_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_pt_leading_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_phi_pt_leading_2018_Ele32_EleHT_pass_v06.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_phi_pt_leading_2018_Ele32_EleHT_pass_v06.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/parameters/variations.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/variations.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/build_jets_calibrator.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/build_jets_calibrator.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/configurator.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/configurator.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/dataset.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/logging.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/network.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/network.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/plot_efficiency.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/plot_efficiency.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/plot_sf.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/plot_sf.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/plot_utils.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/rucio.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/rucio.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/run.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,14 @@
         full=False,
     ):
         super().run(
             filesets,
             processor_instance,
             full,
         )
-        self.run_fileset(filesets, processor_instance)
 
         if full:
             # Running separately on each dataset
             logging.info(f"Working on samples: {list(filesets.keys())}")
 
             output = self.run_fileset(filesets, processor_instance)
             print(f"Saving output to {self.output_file.format('all')}")
@@ -255,15 +254,14 @@
         full=False,
     ):
         super().run(
             filesets,
             processor_instance,
             full=full,
         )
-        self.run_fileset(filesets, processor_instance)
 
         if full:
             # Running separately on each dataset
             logging.info(f"Working on samples: {list(filesets.keys())}")
             
             output = self.run_fileset(filesets, processor_instance)
             print(f"Saving output to {self.output_file.format('all')}")
```

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/skim.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/skim.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/utils/utils.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/workflows/base.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/base.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/workflows/genweights.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/genweights.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/workflows/semileptonic_triggerSF.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/semileptonic_triggerSF.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/workflows/sf_lepton_variations.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/sf_lepton_variations.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea/workflows/tthbb_base_processor.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/tthbb_base_processor.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pocket_coffea.egg-info/PKG-INFO` & `pocket_coffea-1.0rc3/pocket_coffea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocket-coffea
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: Configurable analysis framework based on Coffea for CMS NanoAOD events analysis
 Home-page: https://github.com/PocketCoffea/PocketCoffea
 Author: Davide Valsecchi,Matteo Marchegiani
 Author-email: davide.valsecchi@cern.ch,matteo.marchegiani@cern.ch
 License: BSD-3-Clause
 Project-URL: Documentation, https://PocketCoffea.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/PocketCoffea/PocketCoffea/issues
```

### Comparing `pocket_coffea-1.0rc2/pocket_coffea.egg-info/SOURCES.txt` & `pocket_coffea-1.0rc3/pocket_coffea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/profiling/mem.py` & `pocket_coffea-1.0rc3/profiling/mem.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/profiling/parton_matching_semilep_newgenmatch_v4.prof` & `pocket_coffea-1.0rc3/profiling/parton_matching_semilep_newgenmatch_v4.prof`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/profiling/parton_matching_semilep_v3.prof` & `pocket_coffea-1.0rc3/profiling/parton_matching_semilep_v3.prof`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/pyproject.toml` & `pocket_coffea-1.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/build_jec.py` & `pocket_coffea-1.0rc3/scripts/build_jec.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/compute_btagSF_calibration.py` & `pocket_coffea-1.0rc3/scripts/compute_btagSF_calibration.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/dataset/append_genweights.py` & `pocket_coffea-1.0rc3/scripts/dataset/append_genweights.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/dataset/append_parents.py` & `pocket_coffea-1.0rc3/scripts/dataset/append_parents.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/dataset/build_datasets.py` & `pocket_coffea-1.0rc3/scripts/dataset/build_datasets.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/dataset/download.py` & `pocket_coffea-1.0rc3/scripts/dataset/download.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/hadd_skimmed_files.py` & `pocket_coffea-1.0rc3/scripts/hadd_skimmed_files.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/lumi/filter_lumi_json.py` & `pocket_coffea-1.0rc3/scripts/lumi/filter_lumi_json.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/lumi/run_brilcalc.py` & `pocket_coffea-1.0rc3/scripts/lumi/run_brilcalc.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/merge_outputs.py` & `pocket_coffea-1.0rc3/scripts/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/plot/make_plots.py` & `pocket_coffea-1.0rc3/scripts/plot/make_plots.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/plot/trigger_efficiency.py` & `pocket_coffea-1.0rc3/scripts/plot/trigger_efficiency.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/plot/trigger_scalefactor.py` & `pocket_coffea-1.0rc3/scripts/plot/trigger_scalefactor.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/scripts/runner.py` & `pocket_coffea-1.0rc3/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/setup.cfg` & `pocket_coffea-1.0rc3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pocket_coffea
-version = 1.0rc2
+version = 1.0rc3
 description = Configurable analysis framework based on Coffea for CMS NanoAOD events analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PocketCoffea/PocketCoffea
 author = Davide Valsecchi,Matteo Marchegiani
 author_email = davide.valsecchi@cern.ch,matteo.marchegiani@cern.ch
 license = BSD-3-Clause
```

### Comparing `pocket_coffea-1.0rc2/tests/test_categorization.py` & `pocket_coffea-1.0rc3/tests/test_categorization.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-1.0rc2/tests/test_hlt_cut.py` & `pocket_coffea-1.0rc3/tests/test_hlt_cut.py`

 * *Files identical despite different names*

