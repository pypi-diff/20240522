# Comparing `tmp/thapbi_pict-1.0.8.tar.gz` & `tmp/thapbi_pict-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thapbi_pict-1.0.8.tar", last modified: Tue Feb  6 15:50:38 2024, max compression
+gzip compressed data, was "thapbi_pict-1.0.9.tar", last modified: Mon Feb 12 16:09:01 2024, max compression
```

## Comparing `thapbi_pict-1.0.8.tar` & `thapbi_pict-1.0.9.tar`

### file list

```diff
@@ -1,551 +1,551 @@
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:38.760329 thapbi_pict-1.0.8/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      749 2023-09-01 15:48:38.000000 thapbi_pict-1.0.8/.flake8
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      883 2022-02-15 12:09:29.000000 thapbi_pict-1.0.8/.zenodo.json
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    14353 2024-02-06 15:46:30.000000 thapbi_pict-1.0.8/CHANGELOG.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5203 2024-01-23 11:10:40.000000 thapbi_pict-1.0.8/CONTRIBUTING.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2469 2023-08-18 10:45:24.000000 thapbi_pict-1.0.8/INSTALL.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1094 2023-08-18 10:45:24.000000 thapbi_pict-1.0.8/LICENSE.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4559 2024-01-23 11:10:40.000000 thapbi_pict-1.0.8/MANIFEST.in
--rw-r--r--   0 pcock    (896600025) pcock    (896600025)     8355 2024-02-06 15:50:38.000000 thapbi_pict-1.0.8/PKG-INFO
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6931 2023-08-18 10:58:31.000000 thapbi_pict-1.0.8/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:12.000000 thapbi_pict-1.0.8/database/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   490569 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/database/ITS1_DB.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1087445 2024-02-06 11:10:58.000000 thapbi_pict-1.0.8/database/ITS1_DB.sql
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3890 2022-06-13 12:04:40.000000 thapbi_pict-1.0.8/database/Nothophytophthora_ITS1_curated.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    25814 2024-01-23 16:29:14.000000 thapbi_pict-1.0.8/database/Oomycota_ITS1_obs.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1845234 2024-01-24 13:47:45.000000 thapbi_pict-1.0.8/database/Oomycota_ITS1_w32.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70688 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/database/Phytophthora_ITS1_curated.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3348 2024-01-23 11:11:04.000000 thapbi_pict-1.0.8/database/README.rst
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5823 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/database/build_ITS1_DB.sh
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1216 2024-01-23 11:10:41.000000 thapbi_pict-1.0.8/database/controls.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:15.000000 thapbi_pict-1.0.8/database/single_isolates/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/2019-BL-1B_S117_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      832 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/2019-Pp2_S176_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      265 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      283 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/88069-P-infestans-56-A04_S4_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      294 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/P-foliorum-DNA-from-FR-81-D08_S44_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/P-foliorum_S165_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/Pd2c_S105_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/RG161_S139_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      291 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-390-1-or-2-P-lateralis-G07_S79_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      466 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      542 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1218_S174_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1750 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1220_S151_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1222_S187_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1226_S186_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP1227_S103_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      246 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP179-P-citrophthora-58-C05_S29_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1304 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP179_S177_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      583 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      289 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      274 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      278 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      531 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP390_S129_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      579 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1156 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      867 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP538-P-pseudotsugae-54-B04_S16_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      792 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      577 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP660_S153_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2645 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP722-P-kernoviae-84-dil-1-100-C09_S33_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP722_S141_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      582 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2045 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/SRCP1221_S175_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-1-A01_S1_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-1-E02_S50_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-2-B01_S13_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-2-F02_S62_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-2-F09_S69_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-3-C01_S25_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      565 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-3-G02_S74_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T-30-4-3-G09_S81_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      848 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/WL54_S128_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.8/database/single_isolates/WL77_S152_L001.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:16.000000 thapbi_pict-1.0.8/examples/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      539 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:16.000000 thapbi_pict-1.0.8/examples/endangered_species/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    52287 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/PRJEB18620.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      503 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:17.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_1.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_10.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_11.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_12.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_13.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_14.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_15.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_2.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_3.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_4.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_5.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_6.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_7.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      154 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_8.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      139 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/EM_9.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      200 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S1.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      257 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S10.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      207 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S2.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      203 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S4.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S5.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S6.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      256 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S7.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/expected/S9.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9016 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/metadata.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:17.000000 thapbi_pict-1.0.8/examples/endangered_species/raw_download/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    29160 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/raw_download/MD5SUM.txt
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:18.000000 thapbi_pict-1.0.8/examples/endangered_species/references/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      571 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/references/16S.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3551 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/references/ITS2.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3956 2023-08-18 10:45:25.000000 thapbi_pict-1.0.8/examples/endangered_species/references/Mini-16S.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2392 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/references/Mini-COI.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3356 2022-02-15 12:09:32.000000 thapbi_pict-1.0.8/examples/endangered_species/references/Mini-cyt-b.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5225 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/endangered_species/references/Mini-rbcL.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/endangered_species/references/cyt-b.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      157 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/endangered_species/references/rbcL.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/endangered_species/references/trnL-P6-loop.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2994 2023-08-18 10:45:25.000000 thapbi_pict-1.0.8/examples/endangered_species/references/trnL-UAA.fasta
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3880 2023-08-18 10:45:25.000000 thapbi_pict-1.0.8/examples/endangered_species/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2669 2023-08-18 10:45:25.000000 thapbi_pict-1.0.8/examples/endangered_species/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:18.000000 thapbi_pict-1.0.8/examples/fecal_sequel/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    17024 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/PRJNA574765.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      722 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2783 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/curated_bats.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1561 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/metadata.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      135 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/mock_community.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3600 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/observed_3_bats.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:18.000000 thapbi_pict-1.0.8/examples/fecal_sequel/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6840 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2229 2023-08-18 10:45:25.000000 thapbi_pict-1.0.8/examples/fecal_sequel/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1502 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fecal_sequel/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:19.000000 thapbi_pict-1.0.8/examples/fungal_mock/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7670 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/ITS1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11427 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/ITS2.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21115 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/PRJNA377530.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      368 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2873 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/metadata_AL1.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2433 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/metadata_AL2.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      439 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/mock_community.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/negative_control.known.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:11.000000 thapbi_pict-1.0.8/examples/fungal_mock/raw_data/
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:19.000000 thapbi_pict-1.0.8/examples/fungal_mock/raw_data/AL2/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3360 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/raw_data/AL2/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4022 2024-01-23 11:10:41.000000 thapbi_pict-1.0.8/examples/fungal_mock/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1602 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/fungal_mock/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:20.000000 thapbi_pict-1.0.8/examples/great_lakes/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70417 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/MOL16S.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5836 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/PRJNA379165.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      424 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    53173 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/SPH16S.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:20.000000 thapbi_pict-1.0.8/examples/great_lakes/expected/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/expected/mock_community.MOL16S.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      152 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/expected/mock_community.SPH16S.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/expected/negative_control.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1298 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/metadata.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:20.000000 thapbi_pict-1.0.8/examples/great_lakes/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2016 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3310 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/examples/great_lakes/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1974 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/great_lakes/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:21.000000 thapbi_pict-1.0.8/examples/recycled_water/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   201938 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/PRJNA417859.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   260627 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    48276 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2220 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/make_meta.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    19485 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/metadata.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:21.000000 thapbi_pict-1.0.8/examples/recycled_water/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    43008 2022-02-15 12:09:33.000000 thapbi_pict-1.0.8/examples/recycled_water/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1894 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/examples/recycled_water/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/recycled_water/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:22.000000 thapbi_pict-1.0.8/examples/soil_nematodes/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4498 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/soil_nematodes/PRJEB27581.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      500 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/soil_nematodes/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      594 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/soil_nematodes/metadata.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      499 2022-07-05 14:15:37.000000 thapbi_pict-1.0.8/examples/soil_nematodes/mock_community.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-07-05 14:15:37.000000 thapbi_pict-1.0.8/examples/soil_nematodes/negative_control.known.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:22.000000 thapbi_pict-1.0.8/examples/soil_nematodes/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1792 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/soil_nematodes/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2883 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/examples/soil_nematodes/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2392 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/examples/soil_nematodes/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:22.000000 thapbi_pict-1.0.8/examples/woody_hosts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/woody_hosts/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:22.000000 thapbi_pict-1.0.8/examples/woody_hosts/expected/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/woody_hosts/expected/DNA10MIX_bycopynumber.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/woody_hosts/expected/DNA10MIX_diluted25x.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/woody_hosts/expected/DNA10MIX_undiluted.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      474 2024-01-29 13:57:31.000000 thapbi_pict-1.0.8/examples/woody_hosts/expected/DNA15MIX.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3131 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/examples/woody_hosts/metadata.tsv
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2007 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/examples/woody_hosts/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      381 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/examples/woody_hosts/setup.sh
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2023-08-18 10:45:26.000000 thapbi_pict-1.0.8/requirements-ext.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      366 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/requirements.txt
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:23.000000 thapbi_pict-1.0.8/scripts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      204 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/scripts/README.rst
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2443 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/scripts/blast_to_fasta.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3307 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/scripts/gg_to_sintax.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1048 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/scripts/make_nr.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      604 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/scripts/make_nr_ctrl_a.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1185 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/scripts/md5.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5549 2022-07-15 14:45:53.000000 thapbi_pict-1.0.8/scripts/missed_refs.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    11313 2023-08-18 10:58:31.000000 thapbi_pict-1.0.8/scripts/plot_reduction.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    16418 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/scripts/pooling.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    11751 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/scripts/rst_doc_test.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3629 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/scripts/sample_filter.py
--rwxr-xr-x   0 pcock    (896600025) pcock    (896600025)     2611 2023-11-09 13:39:50.000000 thapbi_pict-1.0.8/scripts/sp_label_ncbi_fasta.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1107 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/scripts/swarm2usearch.py
--rwxr-xr-x   0 pcock    (896600025) pcock    (896600025)     1047 2023-08-08 14:42:45.000000 thapbi_pict-1.0.8/scripts/swarm_to_usearch.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5748 2024-01-23 11:11:04.000000 thapbi_pict-1.0.8/scripts/unknowns.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       38 2024-02-06 15:50:38.000000 thapbi_pict-1.0.8/setup.cfg
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4098 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/setup.py
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:25.000000 thapbi_pict-1.0.8/tests/
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:27.000000 thapbi_pict-1.0.8/tests/assess/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      325 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/ex1.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      400 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/ex1.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex1.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      258 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex1a.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex1a.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      380 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/ex2.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      369 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex2.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      151 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex2.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      321 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/ex3.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      234 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex3.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       71 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex3.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      383 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/ex4.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex4.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/ex4.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      319 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/fp.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/fp.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       74 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/fp.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      173 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/meta.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      638 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/samples.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      378 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/samples.confusion.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/samples.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2278 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/seven.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      195 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/assess/unclassified.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      214 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/unclassified.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       79 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/assess/unclassified.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6757 2023-06-02 14:45:19.000000 thapbi_pict-1.0.8/tests/ceil-no-limit.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:28.000000 thapbi_pict-1.0.8/tests/classifier/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      826 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2307 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2319 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2331 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2343 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1902 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2263 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2295 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1118 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4305 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4329 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4353 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4377 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3691 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4237 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4281 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      703 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      830 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/corner_cases_query.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      232 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      382 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classifier/genus_boundary_query.onebp.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:29.000000 thapbi_pict-1.0.8/tests/classify/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1548 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1614 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      124 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.meta.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1533 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1732 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.reads.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.samples.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.substr.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1244 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      210 2022-03-09 12:53:03.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-etc.meta.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5335 2022-03-09 12:53:03.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-etc.reads.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      962 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/classify/P-infestans-etc.samples.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4187 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/hmm_trim.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4199 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/hmm_trim.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3822 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/classify/hmm_trim.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3992 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/hmm_trim.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4172 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/hmm_trim.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3925 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/classify/hmm_trim.tally.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:29.000000 thapbi_pict-1.0.8/tests/conflicts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2084 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/tests/conflicts/default.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      248 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/conflicts/dup_seqs.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:29.000000 thapbi_pict-1.0.8/tests/curated-import/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1135 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/curated-import/dup_seqs.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:29.000000 thapbi_pict-1.0.8/tests/edit-graph/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      619 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/edit-graph/DNAMIX_S95_L001.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3811 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/edit-graph/DNAMIX_S95_L001.xgmml
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/marker_clash/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2725 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2747 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2702 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.NotITS1.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2616 2022-02-15 12:09:34.000000 thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/marker_clash/Phytophthora_cinnamomi.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      600 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/marker_clash/conflicts.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6865 2023-06-02 14:45:17.000000 thapbi_pict-1.0.8/tests/master.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      662 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/multi_marker/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:11.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/16S/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/16S/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/ITS2/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/ITS2/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-16S/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      446 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-16S/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-COI/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      223 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-COI/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-cyt-b/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      569 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-rbcL/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      395 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-rbcL/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/rbcL/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/rbcL/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/trnL-P6-loop/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      302 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/trnL-P6-loop/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:30.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/trnL-UAA/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/multi_marker/intermediate/trnL-UAA/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:31.000000 thapbi_pict-1.0.8/tests/multi_marker/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    35070 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    47717 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:31.000000 thapbi_pict-1.0.8/tests/multi_marker/summary/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1264 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/multi_marker/summary/pooled.reads.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      237 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/multi_marker/summary/pooled.samples.onebp.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:31.000000 thapbi_pict-1.0.8/tests/ncbi-import/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    62168 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/ncbi-import/20th_Century_ITS1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    76127 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1058 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/ncbi-import/hybrid.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5646 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/ncbi-import/multiple_hmm.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:31.000000 thapbi_pict-1.0.8/tests/nematodes/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1207 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/nematodes/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4660 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/nematodes/sample_R1.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6783 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/nematodes/sample_R2.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      483 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/nematodes/sample_flip_a10.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/nematodes/sample_noflip_a10.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:31.000000 thapbi_pict-1.0.8/tests/pipeline/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2567 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/tests/pipeline/thapbi-pict.reads.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      926 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/tests/pipeline/thapbi-pict.samples.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2113 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/pipeline/thapbi-pict.tally.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:31.000000 thapbi_pict-1.0.8/tests/pooling/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1722 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/pooling/example.pooled.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4999 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/pooling/example.samples.onebp.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:32.000000 thapbi_pict-1.0.8/tests/prepare-reads/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/prepare-reads/6e847180a4da6eed316e1fb98b21218f.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2613 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1911 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/prepare-reads/DNAMIX_S95_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2021-04-07 19:03:04.000000 thapbi_pict-1.0.8/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      429 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/prepare-reads/SRR6303948_sample_default.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3434 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/prepare-reads/SRR6303948_sample_primers.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:33.000000 thapbi_pict-1.0.8/tests/read-correction/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2409 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/AA.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/AA.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      113 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/AA.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/AA.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/ACGT.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1043 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/ACGT.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      698 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/ACGT.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1158 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/ACGT.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      775 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/Brassica.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/Brassica.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-08-18 10:45:27.000000 thapbi_pict-1.0.8/tests/read-correction/Brassica.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4588 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_cinnamomi.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2664 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8036 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Rhabditis.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Rhabditis.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/Rhabditis.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2476 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/chimeras.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-02-08 13:36:24.000000 thapbi_pict-1.0.8/tests/read-correction/chimeras.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2253 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/chimeras.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-09-01 15:48:39.000000 thapbi_pict-1.0.8/tests/read-correction/chimeras.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2698 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/read-correction/chimeras.vsearch.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:33.000000 thapbi_pict-1.0.8/tests/reads/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq.md5
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   580693 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz.md5
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   679862 2020-09-11 17:49:04.000000 thapbi_pict-1.0.8/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/SRR6303948_sample_1.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/SRR6303948_sample_1.fastq.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/SRR6303948_sample_2.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/SRR6303948_sample_2.fastq.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      812 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/ena_submit.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      878 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/ena_submit_custom.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      147 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/reads/metadata.tsv
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1908 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/run_tests.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:33.000000 thapbi_pict-1.0.8/tests/sample-tally/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1971 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/sample-tally/DNAMIX_S95_L001.tally.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:35.000000 thapbi_pict-1.0.8/tests/summary/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      550 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/summary/assess-meta.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.8/tests/summary/assess.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      434 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary/classify-meta-req.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      457 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary/classify-meta-req.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary/classify-meta-req.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary/classify-meta-req.swarm.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary/classify-meta-req.swarmid.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      838 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary/classify-meta.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      465 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary/classify-meta.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary/classify-meta.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary/classify-meta.swarm.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary/classify-meta.swarmid.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      738 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary/classify.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      365 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary/classify.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      749 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary/classify.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      188 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary/classify.swarm.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary/classify.swarmid.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:36.000000 thapbi_pict-1.0.8/tests/summary_meta/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1456 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/A1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/A1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      823 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/A2.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      630 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/A2.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      674 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/B1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      666 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/B1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      677 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/B1r.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      667 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/B1r.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/C1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/C1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/X1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/X1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      385 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/summary_meta/Y1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      386 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/Y1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      138 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/metadata.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2953 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/summary-q.reads.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2022-04-14 14:33:41.000000 thapbi_pict-1.0.8/tests/summary_meta/summary-q.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1021 2022-05-18 10:46:39.000000 thapbi_pict-1.0.8/tests/summary_meta/summary-qu.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1306 2022-05-18 10:46:39.000000 thapbi_pict-1.0.8/tests/summary_meta/summary-u.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3324 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/summary_meta/summary.reads.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1228 2022-04-14 14:33:42.000000 thapbi_pict-1.0.8/tests/summary_meta/summary.samples.1s3g.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:36.000000 thapbi_pict-1.0.8/tests/synthetic_controls/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11507 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11656 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2785 2024-02-06 11:02:38.000000 thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10447 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9803 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/synthetic_controls/single-plate.ITS1.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10950 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-A.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11366 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-B.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12065 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-C.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12310 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-D.fasta
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3475 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_assess.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1240 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_build_db.sh
--rw-r--r--   0 pcock    (896600025) pcock    (896600025)   862238 2023-06-02 14:41:16.000000 thapbi_pict-1.0.8/tests/test_case2.fasta
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4980 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_classify.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1106 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/test_conflicts.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6951 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/tests/test_curated-import.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3681 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_denoise.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1654 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/tests/test_dump.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2252 2024-01-23 11:11:04.000000 thapbi_pict-1.0.8/tests/test_edit-graph.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/test_ena-submit.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      991 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_fasta-nr.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3155 2023-09-01 15:48:39.000000 thapbi_pict-1.0.8/tests/test_load-tax.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3458 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/tests/test_marker_clash.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4096 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_multi_marker.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     9683 2022-07-08 11:55:38.000000 thapbi_pict-1.0.8/tests/test_ncbi-import.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4302 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_pipeline.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      872 2022-04-15 14:20:11.000000 thapbi_pict-1.0.8/tests/test_pooling.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4966 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_prepare-reads.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2263 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_sample-tally.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4890 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_summary.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6127 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_synthetic_controls.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5659 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/test_woody_hosts.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:37.000000 thapbi_pict-1.0.8/tests/woody_hosts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1802 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/tests/woody_hosts/DNA_MIXES.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      681 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/woody_hosts/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    26225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.8/tests/woody_hosts/all.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    59765 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/tests/woody_hosts/all.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    60777 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/tests/woody_hosts/all.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    58076 2023-08-18 10:45:28.000000 thapbi_pict-1.0.8/tests/woody_hosts/all.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    36279 2023-08-18 10:45:29.000000 thapbi_pict-1.0.8/tests/woody_hosts/denoise.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10457 2022-02-15 12:09:37.000000 thapbi_pict-1.0.8/tests/woody_hosts/intermediate.tar.bz2
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:38.000000 thapbi_pict-1.0.8/thapbi_pict/
--rw-r--r--   0 pcock    (896600025) pcock    (896600025)  1531904 2024-02-06 11:10:48.000000 thapbi_pict-1.0.8/thapbi_pict/ITS1_DB.sqlite
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1031 2024-01-30 18:23:44.000000 thapbi_pict-1.0.8/thapbi_pict/__init__.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70578 2024-01-23 11:11:04.000000 thapbi_pict-1.0.8/thapbi_pict/__main__.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    24514 2024-01-24 14:34:45.000000 thapbi_pict-1.0.8/thapbi_pict/assess.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    30757 2024-02-06 11:19:58.000000 thapbi_pict-1.0.8/thapbi_pict/classify.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4186 2023-08-18 10:45:29.000000 thapbi_pict-1.0.8/thapbi_pict/conflicts.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    29013 2024-01-24 14:34:55.000000 thapbi_pict-1.0.8/thapbi_pict/db_import.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5014 2024-01-24 14:31:28.000000 thapbi_pict-1.0.8/thapbi_pict/db_orm.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21168 2024-01-24 14:30:36.000000 thapbi_pict-1.0.8/thapbi_pict/denoise.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7705 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/thapbi_pict/dump.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    23786 2024-01-24 14:31:58.000000 thapbi_pict-1.0.8/thapbi_pict/edit_graph.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5997 2023-08-18 10:45:29.000000 thapbi_pict-1.0.8/thapbi_pict/ena_submit.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3031 2024-01-24 14:34:14.000000 thapbi_pict-1.0.8/thapbi_pict/fasta_nr.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    32336 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/thapbi_pict/prepare.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    22436 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/thapbi_pict/sample_tally.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    34858 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/thapbi_pict/summary.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    15079 2024-01-24 14:33:12.000000 thapbi_pict-1.0.8/thapbi_pict/taxdump.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    37451 2024-01-24 14:33:48.000000 thapbi_pict-1.0.8/thapbi_pict/utils.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6061 2024-01-23 11:10:42.000000 thapbi_pict-1.0.8/thapbi_pict/versions.py
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-06 15:50:38.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/
--rw-r--r--   0 pcock    (896600025) pcock    (896600025)     8355 2024-02-06 15:50:07.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/PKG-INFO
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21055 2024-02-06 15:50:11.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/SOURCES.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        1 2024-02-06 15:50:07.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/dependency_links.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       58 2024-02-06 15:50:07.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/entry_points.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      121 2024-02-06 15:50:07.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/requires.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       12 2024-02-06 15:50:07.000000 thapbi_pict-1.0.8/thapbi_pict.egg-info/top_level.txt
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:09:01.041082 thapbi_pict-1.0.9/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      749 2023-09-01 15:48:38.000000 thapbi_pict-1.0.9/.flake8
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      883 2022-02-15 12:09:29.000000 thapbi_pict-1.0.9/.zenodo.json
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    14426 2024-02-12 15:56:38.000000 thapbi_pict-1.0.9/CHANGELOG.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5203 2024-01-23 11:10:40.000000 thapbi_pict-1.0.9/CONTRIBUTING.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2469 2023-08-18 10:45:24.000000 thapbi_pict-1.0.9/INSTALL.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1094 2023-08-18 10:45:24.000000 thapbi_pict-1.0.9/LICENSE.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4559 2024-01-23 11:10:40.000000 thapbi_pict-1.0.9/MANIFEST.in
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)     8355 2024-02-12 16:09:01.000000 thapbi_pict-1.0.9/PKG-INFO
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6931 2023-08-18 10:58:31.000000 thapbi_pict-1.0.9/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:49.000000 thapbi_pict-1.0.9/database/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   490569 2024-02-12 16:05:30.000000 thapbi_pict-1.0.9/database/ITS1_DB.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1087445 2024-02-12 16:05:30.000000 thapbi_pict-1.0.9/database/ITS1_DB.sql
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3890 2022-06-13 12:04:40.000000 thapbi_pict-1.0.9/database/Nothophytophthora_ITS1_curated.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    25814 2024-01-23 16:29:14.000000 thapbi_pict-1.0.9/database/Oomycota_ITS1_obs.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1845234 2024-01-24 13:47:45.000000 thapbi_pict-1.0.9/database/Oomycota_ITS1_w32.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70688 2024-02-06 11:19:58.000000 thapbi_pict-1.0.9/database/Phytophthora_ITS1_curated.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3348 2024-01-23 11:11:04.000000 thapbi_pict-1.0.9/database/README.rst
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5823 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/database/build_ITS1_DB.sh
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1216 2024-01-23 11:10:41.000000 thapbi_pict-1.0.9/database/controls.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/database/single_isolates/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/2019-BL-1B_S117_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      832 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/2019-Pp2_S176_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      265 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      283 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/88069-P-infestans-56-A04_S4_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      294 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/P-foliorum-DNA-from-FR-81-D08_S44_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/P-foliorum_S165_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/Pd2c_S105_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/RG161_S139_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      291 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-390-1-or-2-P-lateralis-G07_S79_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      466 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      542 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1218_S174_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1750 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1220_S151_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1222_S187_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1226_S186_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP1227_S103_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      246 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP179-P-citrophthora-58-C05_S29_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1304 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP179_S177_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      583 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      289 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      274 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      278 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      531 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP390_S129_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      579 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1156 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      867 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP538-P-pseudotsugae-54-B04_S16_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      792 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      577 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP660_S153_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2645 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP722-P-kernoviae-84-dil-1-100-C09_S33_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP722_S141_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      582 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2045 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/SRCP1221_S175_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-1-A01_S1_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-1-E02_S50_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-2-B01_S13_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-2-F02_S62_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-2-F09_S69_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-3-C01_S25_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      565 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-3-G02_S74_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T-30-4-3-G09_S81_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      848 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/WL54_S128_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.9/database/single_isolates/WL77_S152_L001.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/examples/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      539 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/examples/endangered_species/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    52287 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/PRJEB18620.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      503 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_1.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_10.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_11.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_12.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_13.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_14.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_15.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_2.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_3.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_4.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_5.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_6.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_7.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      154 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_8.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      139 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/EM_9.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      200 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S1.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      257 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S10.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      207 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S2.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      203 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S4.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S5.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S6.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      256 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S7.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/expected/S9.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9016 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/metadata.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/examples/endangered_species/raw_download/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    29160 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/raw_download/MD5SUM.txt
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/examples/endangered_species/references/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      571 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/references/16S.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3551 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/references/ITS2.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3956 2023-08-18 10:45:25.000000 thapbi_pict-1.0.9/examples/endangered_species/references/Mini-16S.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2392 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/references/Mini-COI.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3356 2022-02-15 12:09:32.000000 thapbi_pict-1.0.9/examples/endangered_species/references/Mini-cyt-b.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5225 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/endangered_species/references/Mini-rbcL.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/endangered_species/references/cyt-b.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      157 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/endangered_species/references/rbcL.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/endangered_species/references/trnL-P6-loop.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2994 2023-08-18 10:45:25.000000 thapbi_pict-1.0.9/examples/endangered_species/references/trnL-UAA.fasta
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3880 2023-08-18 10:45:25.000000 thapbi_pict-1.0.9/examples/endangered_species/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2669 2023-08-18 10:45:25.000000 thapbi_pict-1.0.9/examples/endangered_species/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:51.000000 thapbi_pict-1.0.9/examples/fecal_sequel/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    17024 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/PRJNA574765.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      722 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2783 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/curated_bats.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1561 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/metadata.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      135 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/mock_community.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3600 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/observed_3_bats.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:52.000000 thapbi_pict-1.0.9/examples/fecal_sequel/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6840 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2229 2023-08-18 10:45:25.000000 thapbi_pict-1.0.9/examples/fecal_sequel/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1502 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fecal_sequel/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:52.000000 thapbi_pict-1.0.9/examples/fungal_mock/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7670 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/ITS1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11427 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/ITS2.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21115 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/PRJNA377530.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      368 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2873 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/metadata_AL1.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2433 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/metadata_AL2.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      439 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/mock_community.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/negative_control.known.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:48.000000 thapbi_pict-1.0.9/examples/fungal_mock/raw_data/
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:52.000000 thapbi_pict-1.0.9/examples/fungal_mock/raw_data/AL2/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3360 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/raw_data/AL2/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4022 2024-01-23 11:10:41.000000 thapbi_pict-1.0.9/examples/fungal_mock/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1602 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/fungal_mock/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:52.000000 thapbi_pict-1.0.9/examples/great_lakes/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70417 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/MOL16S.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5836 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/PRJNA379165.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      424 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    53173 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/SPH16S.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:52.000000 thapbi_pict-1.0.9/examples/great_lakes/expected/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/expected/mock_community.MOL16S.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      152 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/expected/mock_community.SPH16S.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/expected/negative_control.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1298 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/metadata.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:52.000000 thapbi_pict-1.0.9/examples/great_lakes/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2016 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3310 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/examples/great_lakes/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1974 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/great_lakes/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:53.000000 thapbi_pict-1.0.9/examples/recycled_water/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   201938 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/PRJNA417859.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   260627 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    48276 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2220 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/make_meta.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    19485 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/metadata.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:53.000000 thapbi_pict-1.0.9/examples/recycled_water/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    43008 2022-02-15 12:09:33.000000 thapbi_pict-1.0.9/examples/recycled_water/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1894 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/examples/recycled_water/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/recycled_water/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:53.000000 thapbi_pict-1.0.9/examples/soil_nematodes/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4498 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/soil_nematodes/PRJEB27581.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      500 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/soil_nematodes/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      594 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/soil_nematodes/metadata.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      499 2022-07-05 14:15:37.000000 thapbi_pict-1.0.9/examples/soil_nematodes/mock_community.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-07-05 14:15:37.000000 thapbi_pict-1.0.9/examples/soil_nematodes/negative_control.known.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:53.000000 thapbi_pict-1.0.9/examples/soil_nematodes/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1792 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/soil_nematodes/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2883 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/examples/soil_nematodes/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2392 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/examples/soil_nematodes/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:53.000000 thapbi_pict-1.0.9/examples/woody_hosts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/woody_hosts/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:53.000000 thapbi_pict-1.0.9/examples/woody_hosts/expected/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/woody_hosts/expected/DNA10MIX_bycopynumber.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/woody_hosts/expected/DNA10MIX_diluted25x.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/woody_hosts/expected/DNA10MIX_undiluted.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      474 2024-01-29 13:57:31.000000 thapbi_pict-1.0.9/examples/woody_hosts/expected/DNA15MIX.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3131 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/examples/woody_hosts/metadata.tsv
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2007 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/examples/woody_hosts/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      381 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/examples/woody_hosts/setup.sh
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2023-08-18 10:45:26.000000 thapbi_pict-1.0.9/requirements-ext.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      366 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/requirements.txt
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:54.000000 thapbi_pict-1.0.9/scripts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      204 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/scripts/README.rst
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2443 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/scripts/blast_to_fasta.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3307 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/scripts/gg_to_sintax.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1048 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/scripts/make_nr.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      604 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/scripts/make_nr_ctrl_a.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1185 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/scripts/md5.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5549 2022-07-15 14:45:53.000000 thapbi_pict-1.0.9/scripts/missed_refs.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    11313 2023-08-18 10:58:31.000000 thapbi_pict-1.0.9/scripts/plot_reduction.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    16418 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/scripts/pooling.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    11751 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/scripts/rst_doc_test.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3629 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/scripts/sample_filter.py
+-rwxr-xr-x   0 pcock    (896600025) pcock    (896600025)     2611 2023-11-09 13:39:50.000000 thapbi_pict-1.0.9/scripts/sp_label_ncbi_fasta.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1107 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/scripts/swarm2usearch.py
+-rwxr-xr-x   0 pcock    (896600025) pcock    (896600025)     1047 2023-08-08 14:42:45.000000 thapbi_pict-1.0.9/scripts/swarm_to_usearch.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5748 2024-01-23 11:11:04.000000 thapbi_pict-1.0.9/scripts/unknowns.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       38 2024-02-12 16:09:01.000000 thapbi_pict-1.0.9/setup.cfg
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4098 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/setup.py
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:54.000000 thapbi_pict-1.0.9/tests/
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:55.000000 thapbi_pict-1.0.9/tests/assess/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      325 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/ex1.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      400 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/ex1.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex1.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      258 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex1a.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex1a.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      380 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/ex2.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      369 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex2.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      151 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex2.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      321 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/ex3.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      234 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex3.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       71 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex3.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      383 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/ex4.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex4.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/ex4.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      319 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/fp.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/fp.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       74 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/fp.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      173 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/meta.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      638 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/samples.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      378 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/samples.confusion.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/samples.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2278 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/seven.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      195 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/assess/unclassified.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      214 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/unclassified.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       79 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/assess/unclassified.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6757 2023-06-02 14:45:19.000000 thapbi_pict-1.0.9/tests/ceil-no-limit.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/classifier/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      826 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2307 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2319 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2331 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2343 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1902 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2263 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2295 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1118 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4305 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4329 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4353 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4377 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3691 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4237 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4281 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      703 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      830 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/corner_cases_query.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      232 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      382 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classifier/genus_boundary_query.onebp.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/classify/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1548 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1614 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      124 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.meta.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1533 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1732 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.reads.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.samples.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.substr.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1244 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      210 2022-03-09 12:53:03.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-etc.meta.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5335 2022-03-09 12:53:03.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-etc.reads.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      962 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/classify/P-infestans-etc.samples.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4187 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/hmm_trim.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4199 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/hmm_trim.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3822 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/classify/hmm_trim.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3992 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/hmm_trim.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4172 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/hmm_trim.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3925 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/classify/hmm_trim.tally.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/conflicts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2084 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/tests/conflicts/default.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      248 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/conflicts/dup_seqs.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/curated-import/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1135 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/curated-import/dup_seqs.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/edit-graph/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      619 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/edit-graph/DNAMIX_S95_L001.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3811 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/edit-graph/DNAMIX_S95_L001.xgmml
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/marker_clash/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2725 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2747 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2702 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.NotITS1.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2616 2022-02-15 12:09:34.000000 thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/marker_clash/Phytophthora_cinnamomi.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      600 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/marker_clash/conflicts.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6865 2023-06-02 14:45:17.000000 thapbi_pict-1.0.9/tests/master.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/multi_marker/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      662 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/multi_marker/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:48.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:56.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/16S/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/16S/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/ITS2/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/ITS2/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-16S/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      446 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-16S/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-COI/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      223 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-COI/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-cyt-b/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      569 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-rbcL/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      395 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-rbcL/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/rbcL/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/rbcL/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/trnL-P6-loop/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      302 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/trnL-P6-loop/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/trnL-UAA/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/multi_marker/intermediate/trnL-UAA/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    35070 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    47717 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/multi_marker/summary/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1264 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/multi_marker/summary/pooled.reads.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      237 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/multi_marker/summary/pooled.samples.onebp.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/ncbi-import/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    62168 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/ncbi-import/20th_Century_ITS1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    76127 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1058 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/ncbi-import/hybrid.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5646 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/ncbi-import/multiple_hmm.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/nematodes/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1207 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/nematodes/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4660 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/nematodes/sample_R1.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6783 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/nematodes/sample_R2.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      483 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/nematodes/sample_flip_a10.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/nematodes/sample_noflip_a10.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/pipeline/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2567 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/tests/pipeline/thapbi-pict.reads.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      926 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/tests/pipeline/thapbi-pict.samples.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2113 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/pipeline/thapbi-pict.tally.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/pooling/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1722 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/pooling/example.pooled.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4999 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/pooling/example.samples.onebp.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:57.000000 thapbi_pict-1.0.9/tests/prepare-reads/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/prepare-reads/6e847180a4da6eed316e1fb98b21218f.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2613 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1911 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/prepare-reads/DNAMIX_S95_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2021-04-07 19:03:04.000000 thapbi_pict-1.0.9/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      429 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/prepare-reads/SRR6303948_sample_default.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3434 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/prepare-reads/SRR6303948_sample_primers.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:58.000000 thapbi_pict-1.0.9/tests/read-correction/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2409 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/AA.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/AA.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      113 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/AA.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/AA.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/ACGT.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1043 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/ACGT.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      698 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/ACGT.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1158 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/ACGT.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      775 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/Brassica.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/Brassica.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-08-18 10:45:27.000000 thapbi_pict-1.0.9/tests/read-correction/Brassica.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4588 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_cinnamomi.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2664 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8036 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Rhabditis.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Rhabditis.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/Rhabditis.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2476 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/chimeras.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-02-08 13:36:24.000000 thapbi_pict-1.0.9/tests/read-correction/chimeras.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2253 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/chimeras.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-09-01 15:48:39.000000 thapbi_pict-1.0.9/tests/read-correction/chimeras.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2698 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/read-correction/chimeras.vsearch.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:58.000000 thapbi_pict-1.0.9/tests/reads/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq.md5
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   580693 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz.md5
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   679862 2020-09-11 17:49:04.000000 thapbi_pict-1.0.9/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/SRR6303948_sample_1.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/SRR6303948_sample_1.fastq.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/SRR6303948_sample_2.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/SRR6303948_sample_2.fastq.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      812 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/ena_submit.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      878 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/ena_submit_custom.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      147 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/reads/metadata.tsv
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1908 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/run_tests.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:58.000000 thapbi_pict-1.0.9/tests/sample-tally/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1971 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/sample-tally/DNAMIX_S95_L001.tally.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:59.000000 thapbi_pict-1.0.9/tests/summary/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      550 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/summary/assess-meta.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.9/tests/summary/assess.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      434 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary/classify-meta-req.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      457 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary/classify-meta-req.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary/classify-meta-req.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary/classify-meta-req.swarm.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary/classify-meta-req.swarmid.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      838 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary/classify-meta.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      465 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary/classify-meta.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary/classify-meta.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary/classify-meta.swarm.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary/classify-meta.swarmid.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      738 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary/classify.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      365 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary/classify.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      749 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary/classify.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      188 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary/classify.swarm.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary/classify.swarmid.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:08:59.000000 thapbi_pict-1.0.9/tests/summary_meta/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1456 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/A1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/A1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      823 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/A2.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      630 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/A2.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      674 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/B1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      666 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/B1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      677 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/B1r.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      667 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/B1r.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/C1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/C1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/X1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/X1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      385 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/summary_meta/Y1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      386 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/Y1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      138 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/metadata.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2953 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/summary-q.reads.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2022-04-14 14:33:41.000000 thapbi_pict-1.0.9/tests/summary_meta/summary-q.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1021 2022-05-18 10:46:39.000000 thapbi_pict-1.0.9/tests/summary_meta/summary-qu.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1306 2022-05-18 10:46:39.000000 thapbi_pict-1.0.9/tests/summary_meta/summary-u.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3324 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/summary_meta/summary.reads.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1228 2022-04-14 14:33:42.000000 thapbi_pict-1.0.9/tests/summary_meta/summary.samples.1s3g.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:09:00.000000 thapbi_pict-1.0.9/tests/synthetic_controls/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11507 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11656 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2785 2024-02-06 11:02:38.000000 thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10447 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9803 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/synthetic_controls/single-plate.ITS1.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10950 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-A.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11366 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-B.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12065 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-C.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12310 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-D.fasta
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3475 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_assess.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1240 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_build_db.sh
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)   862238 2023-06-02 14:41:16.000000 thapbi_pict-1.0.9/tests/test_case2.fasta
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4980 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_classify.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1106 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/test_conflicts.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6951 2024-02-06 11:19:58.000000 thapbi_pict-1.0.9/tests/test_curated-import.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3681 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_denoise.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1654 2024-02-06 11:19:58.000000 thapbi_pict-1.0.9/tests/test_dump.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2252 2024-01-23 11:11:04.000000 thapbi_pict-1.0.9/tests/test_edit-graph.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/test_ena-submit.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      991 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_fasta-nr.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3155 2023-09-01 15:48:39.000000 thapbi_pict-1.0.9/tests/test_load-tax.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3458 2024-01-23 11:10:42.000000 thapbi_pict-1.0.9/tests/test_marker_clash.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4096 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_multi_marker.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     9683 2022-07-08 11:55:38.000000 thapbi_pict-1.0.9/tests/test_ncbi-import.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4302 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_pipeline.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      872 2022-04-15 14:20:11.000000 thapbi_pict-1.0.9/tests/test_pooling.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4966 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_prepare-reads.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2263 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_sample-tally.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4890 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_summary.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6127 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_synthetic_controls.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5659 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/test_woody_hosts.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:09:00.000000 thapbi_pict-1.0.9/tests/woody_hosts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1802 2024-02-06 11:19:58.000000 thapbi_pict-1.0.9/tests/woody_hosts/DNA_MIXES.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      681 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/woody_hosts/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    26225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.9/tests/woody_hosts/all.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    59765 2024-02-06 11:19:58.000000 thapbi_pict-1.0.9/tests/woody_hosts/all.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    60777 2024-02-06 11:19:58.000000 thapbi_pict-1.0.9/tests/woody_hosts/all.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    58076 2023-08-18 10:45:28.000000 thapbi_pict-1.0.9/tests/woody_hosts/all.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    36279 2023-08-18 10:45:29.000000 thapbi_pict-1.0.9/tests/woody_hosts/denoise.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10457 2022-02-15 12:09:37.000000 thapbi_pict-1.0.9/tests/woody_hosts/intermediate.tar.bz2
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:09:00.000000 thapbi_pict-1.0.9/thapbi_pict/
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)  1531904 2024-02-12 16:04:35.000000 thapbi_pict-1.0.9/thapbi_pict/ITS1_DB.sqlite
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1031 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/__init__.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70728 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/__main__.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    25205 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/assess.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    32323 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/classify.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4290 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/conflicts.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    29392 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/db_import.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5014 2024-01-24 14:31:28.000000 thapbi_pict-1.0.9/thapbi_pict/db_orm.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21960 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/denoise.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7894 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/dump.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    23905 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/edit_graph.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6397 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/ena_submit.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3160 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/fasta_nr.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    33919 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/prepare.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    23268 2024-02-12 15:36:35.000000 thapbi_pict-1.0.9/thapbi_pict/sample_tally.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    35455 2024-02-12 15:36:36.000000 thapbi_pict-1.0.9/thapbi_pict/summary.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    15852 2024-02-12 15:36:36.000000 thapbi_pict-1.0.9/thapbi_pict/taxdump.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    38278 2024-02-12 15:36:36.000000 thapbi_pict-1.0.9/thapbi_pict/utils.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6251 2024-02-12 15:36:36.000000 thapbi_pict-1.0.9/thapbi_pict/versions.py
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2024-02-12 16:09:01.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)     8355 2024-02-12 16:08:47.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/PKG-INFO
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21055 2024-02-12 16:08:48.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/SOURCES.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        1 2024-02-12 16:08:47.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/dependency_links.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       58 2024-02-12 16:08:47.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/entry_points.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      121 2024-02-12 16:08:47.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/requires.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       12 2024-02-12 16:08:47.000000 thapbi_pict-1.0.9/thapbi_pict.egg-info/top_level.txt
```

### Comparing `thapbi_pict-1.0.8/.flake8` & `thapbi_pict-1.0.9/.flake8`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/.zenodo.json` & `thapbi_pict-1.0.9/.zenodo.json`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/CHANGELOG.rst` & `thapbi_pict-1.0.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Release History
 ===============
 
 ======= ========== ============================================================================
 Version Date       Notes
 ======= ========== ============================================================================
+v1.0.9  2024-02-12 Using Python type annotations (internal code change).
 v1.0.8  2024-02-06 Additional curated *Phytophthora* in default DB. Adds ``1s6g`` classifier.
 v1.0.7  2024-01-29 Treat *Phytophthora cambivora* as a synonym of *Phytophthora x cambivora*.
 v1.0.6  2024-01-24 Added some *Peronosclerospora* to curated DB. Updated NCBI import.
 v1.0.5  2023-11-22 Updated NCBI import, and scripted most of what was a semi-manual process.
 v1.0.4  2023-11-20 Dropped unused ``-m`` / ``--method`` argument to ``edit-graph`` command.
 v1.0.3  2023-09-04 Updated NCBI import and curated *P. condilina* entries in default DB.
 v1.0.2  2023-08-18 Use sum of cutadapt and singleton values etc for pooled marker reports.
```

### Comparing `thapbi_pict-1.0.8/CONTRIBUTING.rst` & `thapbi_pict-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/INSTALL.rst` & `thapbi_pict-1.0.9/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/LICENSE.rst` & `thapbi_pict-1.0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/MANIFEST.in` & `thapbi_pict-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/PKG-INFO` & `thapbi_pict-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thapbi_pict
-Version: 1.0.8
+Version: 1.0.9
 Summary: THAPBI Phytophthora ITS1 Classifier Tool (PICT).
 Home-page: https://github.com/peterjc/thapbi-pict
 Download-URL: https://github.com/peterjc/thapbi-pict
 Author: Peter Cock
 Author-email: peter.cock@hutton.ac.uk
 Project-URL: Documentation, https://thapbi-pict.readthedocs.io/
 Project-URL: Source, https://github.com/peterjc/thapbi-pict/
```

### Comparing `thapbi_pict-1.0.8/README.rst` & `thapbi_pict-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/ITS1_DB.fasta` & `thapbi_pict-1.0.9/database/ITS1_DB.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/ITS1_DB.sql` & `thapbi_pict-1.0.9/database/ITS1_DB.sql`

 * *Files 0% similar despite different names*

```diff
@@ -5,101 +5,101 @@
 	name VARCHAR(100), 
 	uri VARCHAR(200), 
 	md5 VARCHAR(32), 
 	notes VARCHAR(1000), 
 	PRIMARY KEY (id), 
 	UNIQUE (md5)
 );
-INSERT INTO data_source VALUES(1,'Import of trimmed-controls.fasta','trimmed-controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(83,'Import of Oomycota_ITS1_obs.fasta','Oomycota_ITS1_obs.fasta','5552759144e4a83de2fac5e8a41ffd5e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(84,'Import of Oomycota_ITS1_w32.fasta','Oomycota_ITS1_w32.fasta','7c6c66a0d2e2086fdb4797efff555ff5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','4dbbd9f7e08eaf5ed5d31f110abe28ca','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(87,'Import of Peronosporales_ITS1_curated.fasta','Peronosporales_ITS1_curated.fasta','af5790abc65086a2a1b74704dacc0672','ITS1 imported with thapbi_pict v1.0.8');
+INSERT INTO data_source VALUES(1,'Import of trimmed-controls.fasta','trimmed-controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(83,'Import of Oomycota_ITS1_obs.fasta','Oomycota_ITS1_obs.fasta','5552759144e4a83de2fac5e8a41ffd5e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(84,'Import of Oomycota_ITS1_w32.fasta','Oomycota_ITS1_w32.fasta','7c6c66a0d2e2086fdb4797efff555ff5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','4dbbd9f7e08eaf5ed5d31f110abe28ca','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(87,'Import of Peronosporales_ITS1_curated.fasta','Peronosporales_ITS1_curated.fasta','af5790abc65086a2a1b74704dacc0672','ITS1 imported with thapbi_pict v1.0.9');
 CREATE TABLE taxonomy (
 	id INTEGER NOT NULL, 
 	ncbi_taxid INTEGER, 
 	genus VARCHAR(100) NOT NULL, 
 	species VARCHAR(100) NOT NULL, 
 	PRIMARY KEY (id)
 );
```

### Comparing `thapbi_pict-1.0.8/database/Nothophytophthora_ITS1_curated.fasta` & `thapbi_pict-1.0.9/database/Nothophytophthora_ITS1_curated.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/Oomycota_ITS1_obs.fasta` & `thapbi_pict-1.0.9/database/Oomycota_ITS1_obs.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/Oomycota_ITS1_w32.fasta` & `thapbi_pict-1.0.9/database/Oomycota_ITS1_w32.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/Phytophthora_ITS1_curated.fasta` & `thapbi_pict-1.0.9/database/Phytophthora_ITS1_curated.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/README.rst` & `thapbi_pict-1.0.9/database/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/build_ITS1_DB.sh` & `thapbi_pict-1.0.9/database/build_ITS1_DB.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/controls.fasta` & `thapbi_pict-1.0.9/database/controls.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/2019-Pp2_S176_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/2019-Pp2_S176_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/RG161_S139_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/RG161_S139_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP1218_S174_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP1218_S174_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP1220_S151_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP1220_S151_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP1222_S187_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP1222_S187_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP179_S177_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP179_S177_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP390_S129_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP390_S129_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/SRCP1221_S175_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/SRCP1221_S175_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-1-A01_S1_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-1-A01_S1_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-2-B01_S13_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-2-B01_S13_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-2-F02_S62_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-2-F02_S62_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-2-F09_S69_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-2-F09_S69_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-3-C01_S25_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-3-C01_S25_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-3-G02_S74_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-3-G02_S74_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T-30-4-3-G09_S81_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T-30-4-3-G09_S81_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/database/single_isolates/WL54_S128_L001.fasta` & `thapbi_pict-1.0.9/database/single_isolates/WL54_S128_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/README.rst` & `thapbi_pict-1.0.9/examples/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/PRJEB18620.tsv` & `thapbi_pict-1.0.9/examples/endangered_species/PRJEB18620.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/metadata.tsv` & `thapbi_pict-1.0.9/examples/endangered_species/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/raw_download/MD5SUM.txt` & `thapbi_pict-1.0.9/examples/endangered_species/raw_download/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/16S.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/ITS2.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/ITS2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/Mini-16S.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/Mini-16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/Mini-COI.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/Mini-COI.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/Mini-cyt-b.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/Mini-cyt-b.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/Mini-rbcL.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/Mini-rbcL.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/trnL-P6-loop.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/trnL-P6-loop.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/references/trnL-UAA.fasta` & `thapbi_pict-1.0.9/examples/endangered_species/references/trnL-UAA.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/run.sh` & `thapbi_pict-1.0.9/examples/endangered_species/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/endangered_species/setup.sh` & `thapbi_pict-1.0.9/examples/endangered_species/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/PRJNA574765.tsv` & `thapbi_pict-1.0.9/examples/fecal_sequel/PRJNA574765.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/README.rst` & `thapbi_pict-1.0.9/examples/fecal_sequel/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/curated_bats.fasta` & `thapbi_pict-1.0.9/examples/fecal_sequel/curated_bats.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/metadata.tsv` & `thapbi_pict-1.0.9/examples/fecal_sequel/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/observed_3_bats.fasta` & `thapbi_pict-1.0.9/examples/fecal_sequel/observed_3_bats.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.9/examples/fecal_sequel/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/run.sh` & `thapbi_pict-1.0.9/examples/fecal_sequel/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fecal_sequel/setup.sh` & `thapbi_pict-1.0.9/examples/fecal_sequel/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/ITS1.fasta` & `thapbi_pict-1.0.9/examples/fungal_mock/ITS1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/ITS2.fasta` & `thapbi_pict-1.0.9/examples/fungal_mock/ITS2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/PRJNA377530.tsv` & `thapbi_pict-1.0.9/examples/fungal_mock/PRJNA377530.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/metadata_AL1.tsv` & `thapbi_pict-1.0.9/examples/fungal_mock/metadata_AL1.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/metadata_AL2.tsv` & `thapbi_pict-1.0.9/examples/fungal_mock/metadata_AL2.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/raw_data/AL2/MD5SUM.txt` & `thapbi_pict-1.0.9/examples/fungal_mock/raw_data/AL2/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/run.sh` & `thapbi_pict-1.0.9/examples/fungal_mock/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/fungal_mock/setup.sh` & `thapbi_pict-1.0.9/examples/fungal_mock/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/MOL16S.fasta` & `thapbi_pict-1.0.9/examples/great_lakes/MOL16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/PRJNA379165.tsv` & `thapbi_pict-1.0.9/examples/great_lakes/PRJNA379165.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/SPH16S.fasta` & `thapbi_pict-1.0.9/examples/great_lakes/SPH16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/metadata.tsv` & `thapbi_pict-1.0.9/examples/great_lakes/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.9/examples/great_lakes/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/run.sh` & `thapbi_pict-1.0.9/examples/great_lakes/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/great_lakes/setup.sh` & `thapbi_pict-1.0.9/examples/great_lakes/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/PRJNA417859.tsv` & `thapbi_pict-1.0.9/examples/recycled_water/PRJNA417859.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta` & `thapbi_pict-1.0.9/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv` & `thapbi_pict-1.0.9/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/make_meta.py` & `thapbi_pict-1.0.9/examples/recycled_water/make_meta.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/metadata.tsv` & `thapbi_pict-1.0.9/examples/recycled_water/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.9/examples/recycled_water/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/run.sh` & `thapbi_pict-1.0.9/examples/recycled_water/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/recycled_water/setup.sh` & `thapbi_pict-1.0.9/examples/recycled_water/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/soil_nematodes/PRJEB27581.tsv` & `thapbi_pict-1.0.9/examples/soil_nematodes/PRJEB27581.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/soil_nematodes/metadata.tsv` & `thapbi_pict-1.0.9/examples/soil_nematodes/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/soil_nematodes/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.9/examples/soil_nematodes/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/soil_nematodes/run.sh` & `thapbi_pict-1.0.9/examples/soil_nematodes/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/soil_nematodes/setup.sh` & `thapbi_pict-1.0.9/examples/soil_nematodes/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/woody_hosts/metadata.tsv` & `thapbi_pict-1.0.9/examples/woody_hosts/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/examples/woody_hosts/run.sh` & `thapbi_pict-1.0.9/examples/woody_hosts/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/blast_to_fasta.py` & `thapbi_pict-1.0.9/scripts/blast_to_fasta.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/gg_to_sintax.py` & `thapbi_pict-1.0.9/scripts/gg_to_sintax.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/make_nr.py` & `thapbi_pict-1.0.9/scripts/make_nr.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/make_nr_ctrl_a.py` & `thapbi_pict-1.0.9/scripts/make_nr_ctrl_a.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/md5.py` & `thapbi_pict-1.0.9/scripts/md5.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/missed_refs.py` & `thapbi_pict-1.0.9/scripts/missed_refs.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/plot_reduction.py` & `thapbi_pict-1.0.9/scripts/plot_reduction.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/pooling.py` & `thapbi_pict-1.0.9/scripts/pooling.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/rst_doc_test.py` & `thapbi_pict-1.0.9/scripts/rst_doc_test.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/sample_filter.py` & `thapbi_pict-1.0.9/scripts/sample_filter.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/sp_label_ncbi_fasta.py` & `thapbi_pict-1.0.9/scripts/sp_label_ncbi_fasta.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/swarm2usearch.py` & `thapbi_pict-1.0.9/scripts/swarm2usearch.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/swarm_to_usearch.py` & `thapbi_pict-1.0.9/scripts/swarm_to_usearch.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/scripts/unknowns.py` & `thapbi_pict-1.0.9/scripts/unknowns.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/setup.py` & `thapbi_pict-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/assess/samples.assess.tsv` & `thapbi_pict-1.0.9/tests/assess/samples.assess.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/assess/seven.fasta` & `thapbi_pict-1.0.9/tests/assess/seven.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/ceil-no-limit.fasta` & `thapbi_pict-1.0.9/tests/ceil-no-limit.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang.fasta` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s2g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s3g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s4g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.1s5g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.fasta` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.identity.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_bilorbang_query.onebp.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_bilorbang_query.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica.fasta` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s2g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s3g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s4g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.1s5g.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.fasta` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.identity.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/P_vulcanica_query.onebp.tsv` & `thapbi_pict-1.0.9/tests/classifier/P_vulcanica_query.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s2g.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s3g.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s4g.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.1s5g.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.blast.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.fasta` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.identity.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/corner_cases_query.onebp.tsv` & `thapbi_pict-1.0.9/tests/classifier/corner_cases_query.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classifier/genus_boundary.fasta` & `thapbi_pict-1.0.9/tests/classifier/genus_boundary.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.1s3g.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.blast.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.fasta` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.identity.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.onebp.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.reads.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.reads.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.substr.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.substr.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-T30-4.tally.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-T30-4.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-etc.reads.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-etc.reads.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/P-infestans-etc.samples.tsv` & `thapbi_pict-1.0.9/tests/classify/P-infestans-etc.samples.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/hmm_trim.1s3g.tsv` & `thapbi_pict-1.0.9/tests/classify/hmm_trim.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/hmm_trim.blast.tsv` & `thapbi_pict-1.0.9/tests/classify/hmm_trim.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/hmm_trim.fasta` & `thapbi_pict-1.0.9/tests/classify/hmm_trim.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/hmm_trim.identity.tsv` & `thapbi_pict-1.0.9/tests/classify/hmm_trim.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/hmm_trim.onebp.tsv` & `thapbi_pict-1.0.9/tests/classify/hmm_trim.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/classify/hmm_trim.tally.tsv` & `thapbi_pict-1.0.9/tests/classify/hmm_trim.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/conflicts/default.tsv` & `thapbi_pict-1.0.9/tests/conflicts/default.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/curated-import/dup_seqs.fasta` & `thapbi_pict-1.0.9/tests/curated-import/dup_seqs.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/edit-graph/DNAMIX_S95_L001.tsv` & `thapbi_pict-1.0.9/tests/edit-graph/DNAMIX_S95_L001.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/edit-graph/DNAMIX_S95_L001.xgmml` & `thapbi_pict-1.0.9/tests/edit-graph/DNAMIX_S95_L001.xgmml`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.NotITS1.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.NotITS1.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/GBLOCK-example.fasta` & `thapbi_pict-1.0.9/tests/marker_clash/GBLOCK-example.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/marker_clash/conflicts.tsv` & `thapbi_pict-1.0.9/tests/marker_clash/conflicts.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/master.fasta` & `thapbi_pict-1.0.9/tests/master.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/multi_marker/README.rst` & `thapbi_pict-1.0.9/tests/multi_marker/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta` & `thapbi_pict-1.0.9/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz` & `thapbi_pict-1.0.9/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz` & `thapbi_pict-1.0.9/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/multi_marker/summary/pooled.reads.onebp.tsv` & `thapbi_pict-1.0.9/tests/multi_marker/summary/pooled.reads.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/ncbi-import/20th_Century_ITS1.fasta` & `thapbi_pict-1.0.9/tests/ncbi-import/20th_Century_ITS1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta` & `thapbi_pict-1.0.9/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/ncbi-import/hybrid.fasta` & `thapbi_pict-1.0.9/tests/ncbi-import/hybrid.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/ncbi-import/multiple_hmm.fasta` & `thapbi_pict-1.0.9/tests/ncbi-import/multiple_hmm.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/nematodes/README.rst` & `thapbi_pict-1.0.9/tests/nematodes/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/nematodes/sample_R1.fastq.gz` & `thapbi_pict-1.0.9/tests/nematodes/sample_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/nematodes/sample_R2.fastq.gz` & `thapbi_pict-1.0.9/tests/nematodes/sample_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/pipeline/thapbi-pict.reads.onebp.tsv` & `thapbi_pict-1.0.9/tests/pipeline/thapbi-pict.reads.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/pipeline/thapbi-pict.samples.onebp.tsv` & `thapbi_pict-1.0.9/tests/pipeline/thapbi-pict.samples.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/pipeline/thapbi-pict.tally.tsv` & `thapbi_pict-1.0.9/tests/pipeline/thapbi-pict.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/pooling/example.pooled.tsv` & `thapbi_pict-1.0.9/tests/pooling/example.pooled.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/pooling/example.samples.onebp.tsv` & `thapbi_pict-1.0.9/tests/pooling/example.samples.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta` & `thapbi_pict-1.0.9/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/prepare-reads/DNAMIX_S95_L001.fasta` & `thapbi_pict-1.0.9/tests/prepare-reads/DNAMIX_S95_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv` & `thapbi_pict-1.0.9/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/prepare-reads/SRR6303948_sample_primers.fasta` & `thapbi_pict-1.0.9/tests/prepare-reads/SRR6303948_sample_primers.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/AA.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/AA.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/AA.unoise.fasta` & `thapbi_pict-1.0.9/tests/read-correction/AA.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/AA.vsearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/AA.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/ACGT.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/ACGT.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/ACGT.unoise.fasta` & `thapbi_pict-1.0.9/tests/read-correction/ACGT.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/ACGT.usearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/ACGT.usearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/ACGT.vsearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/ACGT.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Brassica.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Brassica.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_cinnamomi.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_cinnamomi.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Rhabditis.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Rhabditis.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Rhabditis.unoise.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Rhabditis.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/Rhabditis.vsearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/Rhabditis.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/chimeras.before.fasta` & `thapbi_pict-1.0.9/tests/read-correction/chimeras.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/chimeras.fasta` & `thapbi_pict-1.0.9/tests/read-correction/chimeras.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/chimeras.unoise.fasta` & `thapbi_pict-1.0.9/tests/read-correction/chimeras.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/chimeras.usearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/chimeras.usearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/read-correction/chimeras.vsearch.fasta` & `thapbi_pict-1.0.9/tests/read-correction/chimeras.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq` & `thapbi_pict-1.0.9/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq` & `thapbi_pict-1.0.9/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz` & `thapbi_pict-1.0.9/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz` & `thapbi_pict-1.0.9/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/SRR6303948_sample_1.fastq` & `thapbi_pict-1.0.9/tests/reads/SRR6303948_sample_1.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/SRR6303948_sample_2.fastq` & `thapbi_pict-1.0.9/tests/reads/SRR6303948_sample_2.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/ena_submit.tsv` & `thapbi_pict-1.0.9/tests/reads/ena_submit.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/reads/ena_submit_custom.tsv` & `thapbi_pict-1.0.9/tests/reads/ena_submit_custom.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/run_tests.sh` & `thapbi_pict-1.0.9/tests/run_tests.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/sample-tally/DNAMIX_S95_L001.tally.tsv` & `thapbi_pict-1.0.9/tests/sample-tally/DNAMIX_S95_L001.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary/assess-meta.identity.tsv` & `thapbi_pict-1.0.9/tests/summary/assess-meta.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary/classify-meta.blast.tsv` & `thapbi_pict-1.0.9/tests/summary/classify-meta.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary/classify-meta.onebp.tsv` & `thapbi_pict-1.0.9/tests/summary/classify-meta.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary/classify.blast.tsv` & `thapbi_pict-1.0.9/tests/summary/classify.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary/classify.onebp.tsv` & `thapbi_pict-1.0.9/tests/summary/classify.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/A1.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/A1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/A1.fasta` & `thapbi_pict-1.0.9/tests/summary_meta/A1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/A2.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/A2.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/A2.fasta` & `thapbi_pict-1.0.9/tests/summary_meta/A2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/B1.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/B1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/B1.fasta` & `thapbi_pict-1.0.9/tests/summary_meta/B1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/B1r.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/B1r.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/B1r.fasta` & `thapbi_pict-1.0.9/tests/summary_meta/B1r.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/C1.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/C1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/C1.fasta` & `thapbi_pict-1.0.9/tests/summary_meta/C1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/X1.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/X1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/X1.fasta` & `thapbi_pict-1.0.9/tests/summary_meta/X1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/summary-q.reads.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/summary-q.reads.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/summary-q.samples.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/summary-q.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/summary-qu.samples.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/summary-qu.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/summary-u.samples.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/summary-u.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/summary.reads.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/summary.reads.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/summary_meta/summary.samples.1s3g.tsv` & `thapbi_pict-1.0.9/tests/summary_meta/summary.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.1s3g.tsv` & `thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv` & `thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv` & `thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/report.ITS1.tally.tsv` & `thapbi_pict-1.0.9/tests/synthetic_controls/report.ITS1.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/single-plate.ITS1.tally.tsv` & `thapbi_pict-1.0.9/tests/synthetic_controls/single-plate.ITS1.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-A.fasta` & `thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-A.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-B.fasta` & `thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-B.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-C.fasta` & `thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-C.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/synthetic_controls/spike-in-D.fasta` & `thapbi_pict-1.0.9/tests/synthetic_controls/spike-in-D.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_assess.sh` & `thapbi_pict-1.0.9/tests/test_assess.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_build_db.sh` & `thapbi_pict-1.0.9/tests/test_build_db.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_case2.fasta` & `thapbi_pict-1.0.9/tests/test_case2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_classify.sh` & `thapbi_pict-1.0.9/tests/test_classify.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_conflicts.sh` & `thapbi_pict-1.0.9/tests/test_conflicts.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_curated-import.sh` & `thapbi_pict-1.0.9/tests/test_curated-import.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_denoise.sh` & `thapbi_pict-1.0.9/tests/test_denoise.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_dump.sh` & `thapbi_pict-1.0.9/tests/test_dump.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_edit-graph.sh` & `thapbi_pict-1.0.9/tests/test_edit-graph.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_ena-submit.sh` & `thapbi_pict-1.0.9/tests/test_ena-submit.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_fasta-nr.sh` & `thapbi_pict-1.0.9/tests/test_fasta-nr.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_load-tax.sh` & `thapbi_pict-1.0.9/tests/test_load-tax.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_marker_clash.sh` & `thapbi_pict-1.0.9/tests/test_marker_clash.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_multi_marker.sh` & `thapbi_pict-1.0.9/tests/test_multi_marker.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_ncbi-import.sh` & `thapbi_pict-1.0.9/tests/test_ncbi-import.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_pipeline.sh` & `thapbi_pict-1.0.9/tests/test_pipeline.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_pooling.sh` & `thapbi_pict-1.0.9/tests/test_pooling.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_prepare-reads.sh` & `thapbi_pict-1.0.9/tests/test_prepare-reads.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_sample-tally.sh` & `thapbi_pict-1.0.9/tests/test_sample-tally.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_summary.sh` & `thapbi_pict-1.0.9/tests/test_summary.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_synthetic_controls.sh` & `thapbi_pict-1.0.9/tests/test_synthetic_controls.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/test_woody_hosts.sh` & `thapbi_pict-1.0.9/tests/test_woody_hosts.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/DNA_MIXES.assess.tsv` & `thapbi_pict-1.0.9/tests/woody_hosts/DNA_MIXES.assess.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/README.rst` & `thapbi_pict-1.0.9/tests/woody_hosts/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/all.fasta` & `thapbi_pict-1.0.9/tests/woody_hosts/all.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/all.identity.tsv` & `thapbi_pict-1.0.9/tests/woody_hosts/all.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/all.onebp.tsv` & `thapbi_pict-1.0.9/tests/woody_hosts/all.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/all.tally.tsv` & `thapbi_pict-1.0.9/tests/woody_hosts/all.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/denoise.tally.tsv` & `thapbi_pict-1.0.9/tests/woody_hosts/denoise.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/tests/woody_hosts/intermediate.tar.bz2` & `thapbi_pict-1.0.9/tests/woody_hosts/intermediate.tar.bz2`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/thapbi_pict/ITS1_DB.sqlite` & `thapbi_pict-1.0.9/thapbi_pict/ITS1_DB.sqlite`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -5,101 +5,101 @@
 	name VARCHAR(100), 
 	uri VARCHAR(200), 
 	md5 VARCHAR(32), 
 	notes VARCHAR(1000), 
 	PRIMARY KEY (id), 
 	UNIQUE (md5)
 );
-INSERT INTO data_source VALUES(1,'Import of trimmed-controls.fasta','trimmed-controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(83,'Import of Oomycota_ITS1_obs.fasta','Oomycota_ITS1_obs.fasta','5552759144e4a83de2fac5e8a41ffd5e','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(84,'Import of Oomycota_ITS1_w32.fasta','Oomycota_ITS1_w32.fasta','7c6c66a0d2e2086fdb4797efff555ff5','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','4dbbd9f7e08eaf5ed5d31f110abe28ca','ITS1 imported with thapbi_pict v1.0.8');
-INSERT INTO data_source VALUES(87,'Import of Peronosporales_ITS1_curated.fasta','Peronosporales_ITS1_curated.fasta','af5790abc65086a2a1b74704dacc0672','ITS1 imported with thapbi_pict v1.0.8');
+INSERT INTO data_source VALUES(1,'Import of trimmed-controls.fasta','trimmed-controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(83,'Import of Oomycota_ITS1_obs.fasta','Oomycota_ITS1_obs.fasta','5552759144e4a83de2fac5e8a41ffd5e','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(84,'Import of Oomycota_ITS1_w32.fasta','Oomycota_ITS1_w32.fasta','7c6c66a0d2e2086fdb4797efff555ff5','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','4dbbd9f7e08eaf5ed5d31f110abe28ca','ITS1 imported with thapbi_pict v1.0.9');
+INSERT INTO data_source VALUES(87,'Import of Peronosporales_ITS1_curated.fasta','Peronosporales_ITS1_curated.fasta','af5790abc65086a2a1b74704dacc0672','ITS1 imported with thapbi_pict v1.0.9');
 CREATE TABLE taxonomy (
 	id INTEGER NOT NULL, 
 	ncbi_taxid INTEGER, 
 	genus VARCHAR(100) NOT NULL, 
 	species VARCHAR(100) NOT NULL, 
 	PRIMARY KEY (id)
 );
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/__init__.py` & `thapbi_pict-1.0.9/thapbi_pict/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 The `tool documentation <https://thapbi-pict.readthedocs.io/>`_ is
 hosted by `Read The Docs <https://readthedocs.org/>`_, generated
 automatically from the ``docs/`` folder of the `software repository
 <https://github.com/peterjc/thapbi-pict/>`_ and the *"docstrings"*
 within the source code which document the Python API.
 """
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/__main__.py` & `thapbi_pict-1.0.9/thapbi_pict/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Copyright 2018-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Defines the ``thapbi_pict`` command line tool.
 
 This works via ``setup.py`` where under ``entry_points`` we define a
 ``console_scripts`` entry for ``thapbi_pict`` (executable name) pointing to
 the ``main()`` function define in this Python file.
 """
 import argparse
 import os
 import sys
+from typing import Optional
 
 from . import __version__
 from .classify import method_classify_file as method_classifier
 from .db_import import DEF_MAX_LENGTH
 from .db_import import DEF_MIN_LENGTH
 from .db_import import fasta_parsing_function as fasta_conventions
 from .db_orm import connect_to_db
@@ -52,21 +53,23 @@
         return min(available, cpu)  # cap requested number
     else:
         sys.exit(
             f"ERROR: CPU argument {cpu} should be positive, or zero for all available."
         )
 
 
-def check_input_file(filename):
+def check_input_file(filename: str) -> None:
     """Command line validation of an input filename."""
     if not os.path.isfile(filename):
         sys.exit(f"ERROR: Could not find input file: {filename}")
 
 
-def check_output_stem(out_stem, dir_only_ok=False, dir_must_exist=True):
+def check_output_stem(
+    out_stem: str, dir_only_ok: bool = False, dir_must_exist: bool = True
+) -> Optional[str]:
     """Command line validation of output stem value.
 
     Returns the output directory, or aborts.
     """
     if not out_stem:
         sys.exit("ERROR: Output stem is blank")
     elif out_stem.endswith(os.path.sep) or os.path.isdir(out_stem):
@@ -81,28 +84,30 @@
     elif os.path.isfile(out_dir):
         sys.exit(f"ERROR: Output stem directory name is a file: {out_dir!r}")
     elif dir_must_exist:
         sys.exit(f"ERROR: Output stem directory does not exist: {out_dir!r}")
     return None
 
 
-def check_output_directory(out_dir, must_exist=True):
+def check_output_directory(out_dir: str, must_exist: bool = True) -> Optional[bool]:
     """Command line validation of output directory value."""
     if not out_dir:
         sys.exit("ERROR: Output directory name blank")
     elif out_dir == "-" or os.path.isdir(out_dir):
         return True
     elif os.path.isfile(out_dir):
         sys.exit(f"ERROR: Output directory name is a file: {out_dir!r}")
     elif must_exist:
         sys.exit(f"ERROR: Output directory does not exist: {out_dir!r}")
     return None
 
 
-def expand_database_argument(text, exist=False, hyphen_default=False):
+def expand_database_argument(
+    text: str, exist: bool = False, hyphen_default: bool = False
+) -> str:
     """Expand an SQLite3 filename to an SQLalchemy URL."""
     # TODO: Expand this to allow other DB prefixes later
     # Note we are not currently checking file exists,
     # as we might be about to create it.
     if text == "-":
         if hyphen_default:
             # Expand to the default bundled DB
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/assess.py` & `thapbi_pict-1.0.9/thapbi_pict/assess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Assess classification of marker reads at species level.
 
 This implements the ``thapbi_pict assess ...`` command.
@@ -23,15 +23,17 @@
 from .utils import md5seq
 from .utils import parse_sample_tsv
 from .utils import parse_species_tsv
 from .utils import species_level
 from .utils import split_read_name_abundance
 
 
-def load_tsv(mapping, classifier_file, min_abundance):
+def load_tsv(
+    mapping: dict[tuple[str, str], str], classifier_file: str, min_abundance: int
+) -> dict[tuple[str, str], str]:
     """Update dict mapping of (marker, MD5) to semi-colon separated species string."""
     for marker, name, _taxid, sp in parse_species_tsv(
         classifier_file, min_abundance, req_species_level=True, allow_wildcard=False
     ):
         if "_" not in name:
             sys.exit(f"ERROR: Bad entry {name} in {classifier_file}")
         if not marker:
@@ -45,15 +47,17 @@
                     f"{mapping[marker, md5]} vs {sp}"
                 )
         else:
             mapping[marker, md5] = sp
     return mapping
 
 
-def sp_for_sample(fasta_files, min_abundance, pooled_sp):
+def sp_for_sample(
+    fasta_files: list[str], min_abundance: int, pooled_sp: dict[tuple[str, str], str]
+) -> str:
     """Return semi-colon separated species string from FASTA files via dict."""
     answer = set()
     for fasta_file in fasta_files:
         try:
             marker = load_fasta_header(fasta_file)["marker"]
         except KeyError:
             sys.exit(f"ERROR: Missing marker in header of {fasta_file}")
@@ -68,35 +72,37 @@
                 sp = pooled_sp[marker, md5]
                 if sp:
                     answer.update(sp.split(";"))
     assert "" not in answer
     return ";".join(sorted(answer))
 
 
-def sp_in_tsv(classifier_files, min_abundance):
+def sp_in_tsv(classifier_files: list[str], min_abundance: int) -> str:
     """Return semi-colon separated list of species in column 2.
 
     Will ignore genus level predictions.
     """
     species = set()
     for classifier_file in classifier_files:
         for _marker, _name, _taxid, sp in parse_species_tsv(
             classifier_file, min_abundance, req_species_level=True, allow_wildcard=True
         ):
             species.update(sp.split(";"))
     return ";".join(sorted(_ for _ in species if species_level(_)))
 
 
-def tally_files(expected_file, predicted_file, min_abundance=0):
+def tally_files(
+    expected_file: str, predicted_file: str, min_abundance: int = 0
+) -> dict[tuple[str, str], set[str]]:
     """Make dictionary tally confusion matrix of species assignments.
 
     Rather than the values simply being an integer count, they are
     the set of MD5 identifiers (take the length for the count).
     """
-    counter = {}
+    counter: dict[tuple[str, str], set[str]] = {}
     # Sorting because currently not all the classifiers produce out in
     # the same order. The identify classifier respects the input FASTA
     # order (which is by decreasing abundance), while the swarm classifier
     # uses the cluster order. Currently the outputs are all small, so fine.
     try:
         for expt, pred in zip(
             sorted(parse_species_tsv(expected_file, req_species_level=True)),
@@ -148,15 +154,17 @@
             try:
                 counter[expt_sp_genus, pred[3]].add(md5)
             except KeyError:
                 counter[expt_sp_genus, pred[3]] = {md5}
     return counter
 
 
-def class_list_from_tally_and_db_list(tally, db_sp_list):
+def class_list_from_tally_and_db_list(
+    tally: dict[tuple[str, str], int], db_sp_list: list[str]
+) -> list[str]:
     """Sorted list of all class names used in a confusion table dict."""
     classes = set()
     impossible = set()
     for expt, pred in tally:
         if expt:
             for sp in expt.split(";"):
                 assert species_level(
@@ -179,28 +187,37 @@
             f" possible prediction: {';'.join(sorted(impossible))}\n"
         )
 
     classes.update(db_sp_list)
     return sorted(classes)
 
 
-def save_mapping(tally, filename, debug=False):
+def save_mapping(
+    tally: dict[tuple[str, str], int], filename: str, debug: bool = False
+) -> None:
     """Output tally table of expected species to predicted sp."""
     with open(filename, "w") as handle:
         handle.write("#sample-count\tExpected\tPredicted\n")
         for expt, pred in sorted(tally):
             handle.write(f"{tally[expt, pred]}\t{expt}\t{pred}\n")
     if debug:
         sys.stderr.write(
             f"DEBUG: Wrote {len(tally)} entry mapping table"
             f" (total {sum(tally.values())}) to {filename}\n"
         )
 
 
-def save_confusion_matrix(tally, db_sp_list, sp_list, filename, exp_total, debug=False):
+def save_confusion_matrix(
+    tally: dict[tuple[str, str], int],
+    db_sp_list: list[str],
+    sp_list: list[str],
+    filename: str,
+    exp_total: int,
+    debug: bool = False,
+) -> None:
     """Output a multi-class confusion matrix as a tab-separated table."""
     total = 0
 
     assert "" not in db_sp_list
     assert "" not in sp_list
     for sp in db_sp_list:
         assert sp in sp_list, sp
@@ -223,15 +240,15 @@
         list({"(None)" for (expt, pred) in tally if expt == ""})
         + sorted({expt for (expt, pred) in tally if expt in sp_list})
         + sorted({expt for (expt, pred) in tally if expt and expt not in sp_list})
     )
 
     assert len(sp_list) * sum(tally.values()) == exp_total
 
-    values = Counter()
+    values: dict[tuple[str, str], int] = Counter()
     for (expt, pred), count in tally.items():
         if expt:
             assert expt in rows
             e_list = expt.split(";")
         else:
             expt = "(None)"
             e_list = []
@@ -273,30 +290,34 @@
             f" (total {total}) to {filename}\n"
         )
     assert total >= sum(tally.values())
     if total != exp_total:
         sys.exit(f"ERROR: Expected {exp_total} but confusion matrix total {total}")
 
 
-def extract_binary_tally(class_name, tally):
+def extract_binary_tally(
+    class_name: str, tally: dict[tuple[str, str], int]
+) -> tuple[int, int, int, int]:
     """Extract single-class TP, FP, FN, TN from multi-class confusion tally.
 
     Reduces the mutli-class expectation/prediction to binary - did they
     include the class of interest, or not?
 
     Returns a 4-tuple of values, True Positives (TP), False Positives (FP),
     False Negatives (FN), True Negatives (TN), which sum to the tally total.
     """
-    bt = Counter()
+    bt: dict[tuple[bool, bool], int] = Counter()
     for (expt, pred), count in tally.items():
         bt[class_name in expt.split(";"), class_name in pred.split(";")] += count
     return bt[True, True], bt[False, True], bt[True, False], bt[False, False]
 
 
-def extract_global_tally(tally, sp_list):
+def extract_global_tally(
+    tally: dict[tuple[str, str], int], sp_list: list[str]
+) -> tuple[int, int, int, int]:
     """Process multi-label confusion matrix (tally dict) to TP, FP, FN, TN.
 
     If the input data has no negative controls, all there will be no
     true negatives (TN).
 
     Returns a 4-tuple of values, True Positives (TP), False Positives (FP),
     False Negatives (FN), True Negatives (TN).
@@ -327,15 +348,15 @@
             all_sp.update(expt.split(";"))
         if pred:
             all_sp.update(pred.split(";"))
     assert "" not in all_sp
     for sp in all_sp:
         assert sp in sp_list, sp
 
-    x = Counter()
+    x: dict[tuple[bool, bool], int] = Counter()
     for (expt, pred), count in tally.items():
         if expt == "" and pred == "":
             # TN special case
             x[False, False] += count * len(sp_list)
         else:
             for class_name in sp_list:
                 x[class_name in expt.split(";"), class_name in pred.split(";")] += count
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/classify.py` & `thapbi_pict-1.0.9/thapbi_pict/classify.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 This implements the ``thapbi_pict classify ...`` command.
 """
 import os
 import shutil
 import sys
 import tempfile
+from typing import Callable
+from typing import Iterable
+from typing import Iterator
+from typing import Sequence
+from typing import Union
 
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from numpy import int8
 from rapidfuzz.distance import Levenshtein
 from rapidfuzz.process import cdist
 
 from .db_orm import MarkerDef
@@ -38,23 +43,25 @@
 MIN_BLAST_COVERAGE = 0.85  # percentage of query length
 
 db_seqs = None  # global dict (seq to genus) for onebp and 1s?g distance classifiers
 max_dist_genus = None  # global variable for 1s?g distance classifiers
 genus_taxid = {}  # global variable to cache taxids for genus names
 
 
-def unique_or_separated(values, sep=";"):
+def unique_or_separated(values: Sequence[Union[str, int]], sep: str = ";") -> str:
     """Return sole element, or a string joining all elements using the separator."""
     if len(set(values)) == 1:
-        return values[0]
+        return str(values[0])
     else:
         return sep.join(str(_) for _ in values)
 
 
-def consoliate_and_sort_taxonomy(genus_species_taxid):
+def consoliate_and_sort_taxonomy(
+    genus_species_taxid: Iterable[tuple[str, str, int]],
+) -> list[tuple[str, str, int]]:
     """Remove any redundant entries, returns new sorted list.
 
     Drops zero taxid entries if has matching non-zero entry.
 
     Drops genus only entries if have species level entries.
     Note ignoring the TaxID here - would need to know the parent/child
     relationship to confirm the genus we're removing does have species
@@ -98,15 +105,17 @@
         ("Genie", "", 0),
         ("Genie", "", 100),
         ("Genie", "alpha", 101),
     ]
 ) == [("Genie", "alpha", 101)]
 
 
-def taxid_and_sp_lists(taxon_entries):
+def taxid_and_sp_lists(
+    taxon_entries: Iterable,
+) -> tuple[Union[int, str], str, str]:
     """Return semi-colon separated summary of the taxonomy objects from DB.
 
     Will discard genus level predictions (e.g. 'Phytophthora') if there is a
     species level prediciton within that genus (e.g. 'Phytophthora infestans').
 
     If there is a single result, returns a tuple of taxid (integer), genus-species,
     and debugging comment (strings).
@@ -123,15 +132,17 @@
     return (
         unique_or_separated([t[2] for t in tax]),
         unique_or_separated([genus_species_name(t[0], t[1]) for t in tax]),
         "",  # Not very useful to report # of entries
     )
 
 
-def perfect_match_in_db(session, marker_name, seq, debug=False):
+def perfect_match_in_db(
+    session, marker_name: str, seq: str, debug: bool = False
+) -> tuple[Union[int, str], str, str]:
     """Lookup sequence in DB, returns taxid, genus_species, note as tuple.
 
     If the 100% matches in the DB give multiple species, then taxid and
     genus_species will be semi-colon separated strings.
     """
     assert seq == seq.upper(), seq
     # Now, does this equal any of the marker sequences in our DB?
@@ -142,21 +153,24 @@
         .filter(MarkerDef.name == marker_name)
         .join(MarkerSeq)
         .filter(MarkerSeq.sequence == seq)
         .distinct()
     )
 
 
-def perfect_substr_in_db(session, marker_name, seq, debug=False):
+def perfect_substr_in_db(
+    session, marker_name: str, seq: str, debug: bool = False
+) -> tuple[Union[int, str], str, str]:
     """Lookup sequence in DB, returns taxid, genus_species, note as tuple.
 
     If the matches containing the sequence as a substring give multiple species,
     then taxid and genus_species will be semi-colon separated strings.
     """
     global db_seqs
+    assert db_seqs is not None
     assert seq == seq.upper(), seq
     matches = set()
     for db_seq in db_seqs:
         if seq in db_seq:
             matches.add(db_seq)
     if not matches:
         return 0, "", ""
@@ -168,43 +182,43 @@
         .join(MarkerSeq)
         .filter(MarkerSeq.sequence.in_(matches))
         .distinct()
     )
 
 
 def apply_method_to_seqs(
-    method_fn,
-    input_seqs,
+    method_fn: Callable,
+    input_seqs: dict[str, str],
     session,
-    marker_name,
-    min_abundance=0,
-    debug=False,
-):
+    marker_name: str,
+    min_abundance: int = 0,
+    debug: bool = False,
+) -> Iterator[tuple[str, str, str, str]]:
     """Call given method on each sequence in the dict.
 
     Assumes any abundance filter has already been applied. Input is a dict of
     identifiers mapped to upper case sequences.
     """
     for idn, seq in input_seqs.items():
         taxid, genus_species, note = method_fn(
             session, marker_name, seq.upper(), debug=debug
         )
         yield idn, str(taxid), genus_species, note
 
 
 def method_identity(
-    input_seqs,
+    input_seqs: dict[str, str],
     session,
-    marker_name,
-    tmp_dir,
-    shared_tmp_dir,
-    min_abundance=0,
-    debug=False,
-    cpu=0,
-):
+    marker_name: str,
+    tmp_dir: str,
+    shared_tmp_dir: str,
+    min_abundance: int = 0,
+    debug: bool = False,
+    cpu: int = 0,
+) -> Iterator[tuple[str, str, str, str]]:
     """Classify using perfect identity.
 
     This is a deliberately simple approach, in part for testing
     purposes. It looks for a perfect identical entry in the database.
     """
     return apply_method_to_seqs(
         perfect_match_in_db,
@@ -213,23 +227,23 @@
         marker_name,
         min_abundance=min_abundance,
         debug=debug,
     )
 
 
 def method_substr(
-    input_seqs,
+    input_seqs: dict[str, str],
     session,
-    marker_name,
-    tmp_dir,
-    shared_tmp_dir,
-    min_abundance=0,
-    debug=False,
-    cpu=0,
-):
+    marker_name: str,
+    tmp_dir: str,
+    shared_tmp_dir: str,
+    min_abundance: int = 0,
+    debug: bool = False,
+    cpu: int = 0,
+) -> Iterator[tuple[str, str, str, str]]:
     """Classify using perfect identity including as a sub-string.
 
     Like the 'identity' method, but allows for a database where the marker
     has not been trimmed, or has been imperfectly trimmed (e.g. primer
     mismatch).
     """
     return apply_method_to_seqs(
@@ -238,15 +252,17 @@
         session,
         marker_name,
         min_abundance=min_abundance,
         debug=debug,
     )
 
 
-def setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_seqs(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+) -> None:
     """Prepare a set of all the DB marker sequences as upper case strings.
 
     Also setup set of sequences in the DB, and dict of genus to NCBI taxid.
     """
     global db_seqs
     global genus_taxid
 
@@ -264,47 +280,57 @@
         _.genus: _.ncbi_taxid
         for _ in session.query(Taxonomy)
         .filter(Taxonomy.species == "")
         .filter(Taxonomy.ncbi_taxid != 0)
     }
 
 
-def setup_onebp(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_onebp(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+) -> None:
     """Prepare a set of all the DB marker sequences; set dist to 1."""
     global max_dist_genus
     check_rapidfuzz()
     setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0)
     max_dist_genus = 1
 
 
-def setup_dist2(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_dist2(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+) -> None:
     """Prepare a set of all DB marker sequences; set dist to 2."""
     global max_dist_genus
     check_rapidfuzz()
     setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0)
     max_dist_genus = 2
 
 
-def setup_dist3(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_dist3(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+) -> None:
     """Prepare a set of all DB marker sequences; set dist to 3."""
     global max_dist_genus
     check_rapidfuzz()
     setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0)
     max_dist_genus = 3
 
 
-def setup_dist4(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_dist4(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+) -> None:
     """Prepare a set of all DB marker sequences; set dist to 4."""
     global max_dist_genus
     check_rapidfuzz()
     setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0)
     max_dist_genus = 4
 
 
-def setup_dist5(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_dist5(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+) -> None:
     """Prepare a set of all DB marker sequences; set dist to 5."""
     global max_dist_genus
     check_rapidfuzz()
     setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0)
     max_dist_genus = 5
 
 
@@ -313,43 +339,44 @@
     global max_dist_genus
     check_rapidfuzz()
     setup_seqs(session, marker_name, shared_tmp_dir, debug=False, cpu=0)
     max_dist_genus = 6
 
 
 def method_dist(
-    input_seqs,
+    input_seqs: dict[str, str],
     session,
-    marker_name,
-    tmp_dir,
-    shared_tmp_dir,
-    min_abundance=0,
-    debug=False,
-    cpu=0,
-):
+    marker_name: str,
+    tmp_dir: str,
+    shared_tmp_dir: str,
+    min_abundance: int = 0,
+    debug: bool = False,
+    cpu: int = 0,
+) -> Iterator[tuple[str, str, str, str]]:
     """Classify using edit distance."""
     global db_seqs
+    assert db_seqs is not None
     global genus_taxid
     global max_dist_genus
-    assert max_dist_genus >= 1, max_dist_genus
+    assert max_dist_genus and max_dist_genus >= 1, max_dist_genus
 
     if not input_seqs:
         # Shortcut
         return {}
 
     # Compute all the query vs DB distances in one call
     all_dists = cdist(
         input_seqs.values(),
         db_seqs,
         scorer=Levenshtein.distance,
         dtype=int8,
         score_cutoff=max_dist_genus,
     )
 
-    results = {}
+    results: dict[str, tuple[Union[int, str], str, str]] = {}
     for (idn, seq), dists in zip(input_seqs.items(), all_dists):
         min_dist = min(dists)
         results[idn] = 0, "", f"No matches up to distance {max_dist_genus}"
         if min_dist == 0:
             assert (
                 seq in db_seqs
             ), f"Expected {idn} to be in DB as min dist zero:\n{seq}"
@@ -407,15 +434,17 @@
         assert results[idn]
 
     for idn in input_seqs:
         taxid, genus_species, note = results[idn]
         yield idn, str(taxid), genus_species, note
 
 
-def setup_blast(session, marker_name, shared_tmp_dir, debug=False, cpu=0):
+def setup_blast(
+    session, marker_name: str, shared_tmp_dir: str, debug: bool = False, cpu: int = 0
+):
     """Prepare a BLAST DB from the marker sequence DB entries."""
     view = (
         session.query(MarkerSeq)
         .join(SeqSource)
         .join(MarkerDef, SeqSource.marker_definition)
         .filter(MarkerDef.name == marker_name)
     )
@@ -432,23 +461,23 @@
         f"Wrote {count} unique sequences from DB to FASTA file for BLAST database.\n"
     )
     cmd = ["makeblastdb", "-dbtype", "nucl", "-in", db_fasta, "-out", blast_db]
     run(cmd, debug)
 
 
 def method_blast(
-    input_seqs,
+    input_seqs: dict[str, str],
     session,
-    marker_name,
-    tmp_dir,
-    shared_tmp_dir,
-    min_abundance=0,
-    debug=False,
-    cpu=0,
-):
+    marker_name: str,
+    tmp_dir: str,
+    shared_tmp_dir: str,
+    min_abundance: int = 0,
+    debug: bool = False,
+    cpu: int = 0,
+) -> Iterator[tuple[str, str, str, str]]:
     """Classify using BLAST.
 
     Another simplistic classifier, run the reads through blastn
     against a BLAST database of our marker sequence database entries.
     """
     assert os.path.isdir(tmp_dir)
     assert os.path.isdir(shared_tmp_dir)
@@ -500,16 +529,16 @@
         for title, seq in SimpleFastaParser(handle):
             idn = title.split(None, 1)[0]
             query_length[idn] = len(seq)
 
     # Load the top-equal BLAST results into a dict, values are lists hit MD5,
     # and the associated score in a second dict
     blast_hits = {}
-    blast_score = {}
-    score = None
+    blast_score: dict[str, str] = {}
+    score: Union[str, float] = ""
     with open(blast_out) as handle:
         for line in handle:
             # if debug:
             #     sys.stderr.write(line)
             parts = line.rstrip("\n").split("\t")
             idn = parts[0]
             if float(parts[3]) / query_length[idn] < MIN_BLAST_COVERAGE:
@@ -543,26 +572,26 @@
         else:
             taxid = 0
             genus_species = ""
             note = "No DB match"
         yield idn, str(taxid), genus_species, note
 
 
-def method_cleanup():
+def method_cleanup() -> None:
     """Free any memory and/or delete any files on disk.
 
     Currently no need to generalise this for the different classifiers, but
     could if for example we also needed to delete any files on disk.
     """
     global db_seqs, max_dist_genus
     db_seqs = None  # global variable for onbep and 1s?g classifiers
     max_dist_genus = None  # global variable for 1s?g distance classifier
 
 
-method_tool_check = {
+method_tool_check: dict[str, list[str]] = {
     "blast": ["makeblastdb", "blastn"],
     "identity": [],
     "onebp": [],
     "1s2g": [],
     "1s3g": [],
     "1s4g": [],
     "1s5g": [],
@@ -592,26 +621,26 @@
     "1s5g": setup_dist5,
     "1s6g": setup_dist6,
     "substr": setup_seqs,
 }
 
 
 def main(
-    inputs,
+    inputs: list[str],
     session,
-    marker_name,
-    method,
-    out_dir,
-    ignore_prefixes,
-    tmp_dir,
-    min_abundance=0,
+    marker_name: str,
+    method: str,
+    out_dir: str,
+    ignore_prefixes: tuple[str],
+    tmp_dir: str,
+    min_abundance: int = 0,
     biom=False,
-    debug=False,
-    cpu=0,
-):
+    debug: bool = False,
+    cpu: int = 0,
+) -> list[Union[str, None]]:
     """Implement the ``thapbi_pict classify`` command.
 
     For use in the pipeline command, returns a filename list of the TSV
     classifier output.
 
     The input files should have been prepared with the same or a lower minimum
     abundance - this acts as an additional filter useful if exploring the best
@@ -719,17 +748,18 @@
         shared_tmp = tmp_obj.name
 
     if debug:
         sys.stderr.write(f"DEBUG: Shared temp folder {shared_tmp}\n")
 
     classifier_output = []  # return value
 
-    seq_count = 0
-    match_count = 0
-    skipped_samples = set()
+    abundance: int = 0
+    seq_count: int = 0
+    match_count: int = 0
+    skipped_samples: set[str] = set()
     for filename in input_files:
         sys.stdout.flush()
         sys.stderr.flush()
 
         folder, stem = os.path.split(filename)
         if stem.endswith(".tally.tsv"):
             stem = stem[:-10]
@@ -759,18 +789,18 @@
             # There are some files still to process, do setup now (once only)
             setup_fn(session, marker_name, shared_tmp, debug, cpu)
             setup_fn = None
 
         if filename.endswith(".fasta"):
             sample = file_to_sample_name(filename)
             # Populate as if this was a single sample tally TSV input:
-            input_seqs = {}
+            input_seqs: dict[str, str] = {}
             seq_meta = {}
-            md5_count = {}
-            tally_counts = {}
+            md5_count: dict[str, int] = {}
+            tally_counts: dict[tuple[str, str, str], int] = {}
             # TODO - avoid repeated definition here, in summary code, and sample-tally:
             stats_fields = (
                 "Raw FASTQ",
                 "Flash",
                 "Cutadapt",
                 "Threshold pool",
                 "Threshold",
@@ -909,14 +939,15 @@
         )
 
     if tmp_dir:
         sys.stderr.write(
             f"WARNING: Please remove temporary files written to {tmp_dir}\n"
         )
     else:
+        assert tmp_obj is not None
         tmp_obj.cleanup()
 
     sys.stderr.write(
         f"{method} classifier assigned species/genus to {match_count}"
         f" of {seq_count} unique sequences from {len(input_files)} files\n"
     )
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/conflicts.py` & `thapbi_pict-1.0.9/thapbi_pict/conflicts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2021 by Peter Cock, The James Hutton Institute.
+# Copyright 2019-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Explore conflicts at species and genus level."""
 import sys
 
@@ -13,15 +13,15 @@
 from .db_orm import MarkerDef
 from .db_orm import MarkerSeq
 from .db_orm import SeqSource
 from .db_orm import Taxonomy
 from .utils import genus_species_name
 
 
-def main(db_url, output_filename, debug=False):
+def main(db_url: str, output_filename: str, debug: bool = False) -> int:
     """Implement the ``thapbi_pict conflicts`` subcommand.
 
     Looks for taxonomy conflicts at marker, genus or species level, with the
     number of marker or genus level conflicts used as the return code. i.e.
     Unix failure (non-zero) when there are marker or genus level conflicts.
 
     A marker level conflict is when a unique sequence appears in the DB under
@@ -51,18 +51,18 @@
         .join(marker_seq, SeqSource.marker_seq)
         .join(marker_def, SeqSource.marker_definition)
         .join(cur_tax, SeqSource.taxonomy)
         .options(contains_eager(SeqSource.marker_seq, alias=marker_seq))
         .options(contains_eager(SeqSource.marker_definition, alias=marker_def))
         .options(contains_eager(SeqSource.taxonomy, alias=cur_tax))
     )
-    md5_to_seq = {}
-    md5_to_marker = {}
-    md5_to_genus = {}
-    md5_to_species = {}
+    md5_to_seq: dict[str, str] = {}
+    md5_to_marker: dict[str, set[str]] = {}
+    md5_to_genus: dict[str, set[str]] = {}
+    md5_to_species: dict[str, set[str]] = {}
     for seq_source in view:
         md5 = seq_source.marker_seq.md5
         seq = seq_source.marker_seq.sequence
         genus = seq_source.taxonomy.genus
         md5_to_seq[md5] = seq
         try:
             md5_to_marker[md5].add(seq_source.marker_definition.name)
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/db_import.py` & `thapbi_pict-1.0.9/thapbi_pict/db_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright 2018-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Shared code for THAPBI PICT to import FASTA into our database.
 
 This code is used for importing NCBI formatted FASTA files, our curated ITS1
 sequence FASTA file databases, and other other FASTA naming conventions.
 """
 import os
 import re
 import sys
+from typing import Optional
 
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 
 from . import __version__
 from .db_orm import connect_to_db
 from .db_orm import DataSource
 from .db_orm import MarkerDef
@@ -32,15 +33,17 @@
 
 DEF_MIN_LENGTH = 100
 DEF_MAX_LENGTH = 1000
 
 taxid_regex = re.compile(r"(ncbi|[ _:;({\[\-\t])taxid=\d+")
 
 
-def parse_ncbi_fasta_entry(text, known_species=None):
+def parse_ncbi_fasta_entry(
+    text: str, known_species: Optional[list[str]] = None
+) -> tuple[int, str]:
     """Split an entry of Accession Genus Species-name Description.
 
     Returns a two-tuple: taxid (always zero), presumed genus-species (may be
     the empty string).
 
     >>> parse_ncbi_fasta_entry('LC159493.1 Phytophthora drechsleri genes ...')
     (0, 'Phytophthora drechsleri')
@@ -111,15 +114,17 @@
 ) == (0, "Phytophthora humicola x inundata")
 
 assert parse_ncbi_fasta_entry(
     "MG707849.1 Phytophthora humicola x inundata isolate SCVWD597 internal transcribed spacer 1, ..."  # noqa: E501
 ) == (0, "Phytophthora humicola x inundata")
 
 
-def parse_ncbi_taxid_entry(text, know_species=None):
+def parse_ncbi_taxid_entry(
+    text: str, know_species: Optional[list[str]] = None
+) -> tuple[int, str]:
     """Find any NCBI taxid as a pattern in the text.
 
     Returns a two-tuple of taxid (zero if not found), and an
     empty string (use the taxonomy table in the DB to get the
     genus-species).
 
     Uses a regular expression based on taxid=<digits>, and
@@ -145,15 +150,17 @@
 ) == (456, "")
 assert parse_ncbi_taxid_entry(
     "HQ013219 Phytophthora arenaria [key=value;taxid=456;key=value]"
 ) == (456, "")
 assert parse_ncbi_taxid_entry("HQ013219:Phytophthora_arenaria:taxid=456") == (456, "")
 
 
-def parse_curated_fasta_entry(text, known_species=None):
+def parse_curated_fasta_entry(
+    text: str, known_species: Optional[list[str]] = None
+) -> tuple[int, str]:
     """Split an entry of "Accession genus species etc" into fields.
 
     Does not use the optional known_species argument.
 
     Returns a two-tuple of taxid (0 unless taxid=... entry found), genus-species.
 
     >>> parse_curated_fasta_entry('HQ013219 Phytophthora arenaria')
@@ -206,15 +213,17 @@
     "P13660 Phytophthora aff infestans [taxid=907744] ignored text"
 ) == (
     907744,
     "Phytophthora aff infestans",
 )
 
 
-def parse_sintax_fasta_entry(text, known_species=None):
+def parse_sintax_fasta_entry(
+    text: str, known_species: Optional[list[str]] = None
+) -> tuple[int, str]:
     """Extract the species from SINTAX taxonomy annotation.
 
     See https://drive5.com/usearch/manual/tax_annot.html which defines
     this taxonomy annotation convention as used in USEARCH and VSEARCH.
     The tax=names field is separated from other fields in the FASTA
     description line by semi-colons, for example:
 
@@ -255,15 +264,17 @@
 ) == (0, "Streptococcus")
 
 assert parse_sintax_fasta_entry(
     ">X80725_S000004313;tax=d:Bacteria,p:Proteobacteria,c:Gammaproteobacteria,o:Enterobacteriales,f:Enterobacteriaceae,g:Escherichia/Shigella,s:Escherichia_coli"  # noqa: E501
 ) == (0, "Escherichia coli")
 
 
-def parse_obitools_fasta_entry(text, known_species=None):
+def parse_obitools_fasta_entry(
+    text: str, known_species: Optional[list[str]] = None
+) -> tuple[int, str]:
     """Parse species from the OBITools extended FASTA header.
 
     See https://pythonhosted.org/OBITools/attributes.html which explains that
     OBITools splits the FASTA line into identifier, zero or more key=value;
     entries, and a free text description.
 
     We are specifically interested in the species_name, genus_name (used if
@@ -303,29 +314,29 @@
     "ncbi": parse_ncbi_fasta_entry,
     "sintax": parse_sintax_fasta_entry,
     "taxid": parse_ncbi_taxid_entry,
     "obitools": parse_obitools_fasta_entry,
 }
 
 
-def load_taxonomy(session):
+def load_taxonomy(session) -> set[str]:
     """Pre-load all the species and synonym names as a set."""
     names = set()
     view = session.query(Taxonomy).distinct(Taxonomy.genus, Taxonomy.species)
     for taxonomy in view:
         names.add(genus_species_name(taxonomy.genus, taxonomy.species))
     for synonym in session.query(Synonym):
         if synonym.name in names:
             sys.stderr.write(f"WARNING: Synonym {synonym.name} duplicated?\n")
         else:
             names.add(synonym.name)
     return names
 
 
-def lookup_species(session, name):
+def lookup_species(session, name: str):
     """Find this species entry in the taxonomy/synonym table (if present)."""
     assert isinstance(name, str), name
     genus, species = genus_species_split(name)
     # Try main table
     taxonomy = (
         session.query(Taxonomy).filter_by(genus=genus, species=species).one_or_none()
     )
@@ -333,15 +344,15 @@
         return taxonomy
     # Try synonyms
     return (
         session.query(Taxonomy).join(Synonym).filter(Synonym.name == name).one_or_none()
     )
 
 
-def lookup_genus(session, name):
+def lookup_genus(session, name: str):
     """Find genus entry via taxonomy/synonym table (if present)."""
     # Apply synonym (which might change the genus)
     taxonomy = (
         session.query(Taxonomy).join(Synonym).filter(Synonym.name == name).one_or_none()
     )
     if taxonomy:
         genus = taxonomy.genus
@@ -482,18 +493,18 @@
     bad_sp_entries = 0
     downgraded_entries = 0  # unknown species --> genus only
     good_entries = 0
     idn_set = set()
 
     valid_letters = set("GATCRYWSMKHBVDN")
 
-    existing_taxonomy = {}
-    existing_sequences = {}
-    additional_taxonomy = {}
-    additional_sequences = {}
+    existing_taxonomy: dict[str, str] = {}
+    existing_sequences: dict[str, str] = {}
+    additional_taxonomy: dict[str, str] = {}
+    additional_sequences: dict[str, str] = {}
     record_entries = []
     with open(fasta_file) as handle:
         for title, seq in SimpleFastaParser(handle):
             if "-" in seq:
                 sys.exit(f"ERROR: Gap in sequence for {title}")
             # NOTE: at this point don't have full sequence prior to primer removal
             seq = seq.upper()
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/db_orm.py` & `thapbi_pict-1.0.9/thapbi_pict/db_orm.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.8/thapbi_pict/denoise.py` & `thapbi_pict-1.0.9/thapbi_pict/denoise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 by Peter Cock, The James Hutton Institute.
+# Copyright 2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Apply UNOISE read-correction to denoise FASTA file(s).
 
 This implements the ``thapbi_pict denoise ...`` command, which is a simplified
@@ -14,29 +14,35 @@
 import sys
 import tempfile
 from collections import Counter
 from collections import defaultdict
 from math import floor
 from math import log2
 from time import time
+from typing import Optional
+from typing import Union
 
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from rapidfuzz.distance import Levenshtein
 from rapidfuzz.process import extract
 from rapidfuzz.process import extract_iter
 
 from .utils import abundance_from_read_name
 from .utils import md5seq
 from .utils import run
 from .versions import check_tools
 
 
 def unoise(
-    counts, unoise_alpha=2.0, unoise_gamma=4, abundance_based=False, debug=False
-):
+    counts: dict[str, int],
+    unoise_alpha: Optional[float] = 2.0,
+    unoise_gamma: Optional[int] = 4,
+    abundance_based: bool = False,
+    debug: bool = False,
+) -> tuple[dict[str, str], dict[str, str]]:
     """Apply UNOISE2 algorithm.
 
     Argument counts is an (unsorted) dict of sequences (for the same amplicon
     marker) as keys, with their total abundance counts as values.
 
     If not specified (i.e. set to zero or None), unoise_alpha defaults to 2.0
     and unoise_gamma to 4.
@@ -51,15 +57,15 @@
         unoise_alpha = 2.0
     if not unoise_gamma:
         unoise_gamma = 4
 
     top_a = max(counts.values())  # will become first centroid
     last_a = None
     cutoff = 0
-    centroids = defaultdict(set)
+    centroids: dict[str, set[str]] = defaultdict(set)
     high_abundance_centroids = None
     if abundance_based:
         sys.stderr.write("Starting UNOISE abundance-based greedy clustering (AGC)\n")
     else:
         sys.stderr.write("Starting UNOISE distance-based greedy clustering (DGC)\n")
     # Start by sorting sequences by abundance, largest first
     for a, query in sorted(
@@ -145,31 +151,31 @@
                         f"<-- Q:{md5seq(query)}_{a} dist {dist}\n"
                     )
             else:
                 # New centroid
                 centroids[query].add(query)
                 # print(query, "new")
 
-    corrections = {}
+    corrections: dict[str, str] = {}
     for seq, choices in centroids.items():
         for _ in choices:
             corrections[_] = seq
         assert corrections[seq] == seq, "Centroid missing"
     return corrections, {}
 
 
 def usearch(
-    counts,
-    unoise_alpha=None,
-    unoise_gamma=None,
-    abundance_based=False,
-    tmp_dir=None,
-    debug=False,
-    cpu=0,
-):
+    counts: dict[str, int],
+    unoise_alpha: Optional[float] = None,
+    unoise_gamma: Optional[int] = None,
+    abundance_based: bool = False,
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[dict[str, str], dict[str, str]]:
     """Invoke USEARCH to run its implementation of the UNOISE3 algorithm.
 
     Assumes v10 or v11 (or later if the command line API is the same).
     Parses the four columns tabbed output.
 
     Returns a dict mapping input sequences to centroid sequences, and a dict
     of MD5 checksums of any sequences flagged as chimeras.
@@ -274,22 +280,22 @@
             else:
                 sys.exit(f"ERROR: Unexpected usearch tabbedout line: {line!r}")
     del md5_to_seq
     return corrections, chimeras
 
 
 def vsearch(
-    counts,
-    unoise_alpha=None,
-    unoise_gamma=None,
-    abundance_based=False,
-    tmp_dir=None,
-    debug=False,
-    cpu=0,
-):
+    counts: dict[str, int],
+    unoise_alpha: Optional[float] = None,
+    unoise_gamma: Optional[int] = None,
+    abundance_based: bool = True,
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[dict[str, str], dict[str, str]]:
     """Invoke VSEARCH to run its reimplementation of the UNOISE3 algorithm.
 
     Argument counts is an (unsorted) dict of sequences (for the same amplicon
     marker) as keys, with their total abundance counts as values.
 
     Returns a dict mapping input sequences to centroid sequences, and a dict
     of MD5 checksums of any sequences flagged as chimeras.
@@ -378,15 +384,15 @@
                 sys.exit(
                     f"ERROR: vsearch --uc output line started {parts[0]}, not S, H or C"
                 )
     del md5_to_seq
 
     with open(denoised_fasta, "w") as handle:
         # TODO: Wasteful as will re-compute the post-correction counts
-        post_counts = defaultdict(int)
+        post_counts: dict[str, int] = defaultdict(int)
         for seq, a in counts.items():
             if seq not in corrections:
                 # Ignored as per UNOISE algorithm
                 if unoise_gamma:
                     assert (
                         a < unoise_gamma
                     ), f"{md5seq(seq)} total {a} vs {unoise_gamma}"
@@ -421,23 +427,23 @@
             assert len(md5) == 32, line
             chimeras[md5] = parts[2].split(";", 1)[0] + "/" + parts[3].split(";", 1)[0]
 
     return corrections, chimeras
 
 
 def read_correction(
-    algorithm,
-    counts,
-    unoise_alpha=2.0,
-    unoise_gamma=4,
-    abundance_based=False,
-    tmp_dir=None,
-    debug=False,
-    cpu=0,
-):
+    algorithm: str,
+    counts: dict[str, int],
+    unoise_alpha: Optional[float] = 2.0,
+    unoise_gamma: Optional[int] = 4,
+    abundance_based: bool = False,
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[dict[str, str], dict[str, str]]:
     """Apply builtin UNOISE algorithm or invoke an external tool like VSEARCH.
 
     Argument algorithm is a string, "unoise-l" for our reimplementation of the
     UNOISE2 algorithm, or "usearch" or "vsearch" to invoke those tools at the
     command line.
 
     Argument counts is an (unsorted) dict of sequences (for the same amplicon
@@ -471,26 +477,26 @@
     sys.stderr.write(
         f"Spent {time_corrections:0.1f}s running {algorithm} for read-corrections\n"
     )
     return answer
 
 
 def main(
-    inputs,
-    output,
-    denoise_algorithm,
-    total_min_abundance=0,
-    min_length=0,
-    max_length=sys.maxsize,
-    unoise_alpha=None,  # e.g. 2.0,
-    unoise_gamma=None,  # e.g. 4,
-    gzipped=False,  # output
-    tmp_dir=None,
-    debug=False,
-    cpu=0,
+    inputs: Union[str, list[str]],
+    output: str,
+    denoise_algorithm: str,
+    total_min_abundance: int = 0,
+    min_length: int = 0,
+    max_length: int = sys.maxsize,
+    unoise_alpha: Optional[float] = None,  # e.g. 2.0,
+    unoise_gamma: Optional[int] = None,  # e.g. 4,
+    gzipped: bool = False,  # output
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
+    cpu: int = 0,
 ):
     """Implement the ``thapbi_pict denoise`` command.
 
     This is a simplified version of the ``thapbi_pict sample-tally`` command
     which pools one or more FASTA input files before running the UNOISE read
     correction algorithm to denoise the dataset.
 
@@ -508,15 +514,15 @@
 
     assert "-" not in inputs
     assert denoise_algorithm != "-"
 
     if os.path.isdir(output):
         sys.exit("ERROR: Output directory given, want a FASTA filename.")
 
-    totals = Counter()
+    totals: dict[str, int] = Counter()
     for filename in inputs:
         if debug:
             sys.stderr.write(f"DEBUG: Parsing {filename}\n")
         with open(filename) as handle:
             for _, seq in SimpleFastaParser(handle):
                 seq = seq.upper()
                 if min_length <= len(seq) <= max_length:
@@ -540,15 +546,15 @@
         totals,
         unoise_alpha=unoise_alpha,
         unoise_gamma=unoise_gamma,
         tmp_dir=tmp_dir,
         debug=debug,
         cpu=cpu,
     )
-    new_totals = defaultdict(int)
+    new_totals: dict[str, int] = defaultdict(int)
     for seq, a in totals.items():
         if seq not in corrections:
             # Ignored as per UNOISE algorithm
             if unoise_gamma:
                 assert (
                     totals[seq] < unoise_gamma
                 ), f"{md5seq(seq)} total {totals[seq]} vs {unoise_gamma}"
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/dump.py` & `thapbi_pict-1.0.9/thapbi_pict/dump.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-# Copyright 2018-2022 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Dumping out marker database to text files.
 
 This implements the ``thapbi_pict dump ...`` command.
 """
 import sys
+from typing import Optional
 
 from sqlalchemy.orm import aliased
 from sqlalchemy.orm import contains_eager
 
 from .classify import taxid_and_sp_lists
 from .db_orm import connect_to_db
 from .db_orm import MarkerDef
 from .db_orm import MarkerSeq
 from .db_orm import SeqSource
 from .db_orm import Taxonomy
 from .utils import genus_species_name
 
 
-def none_str(value, none_value=""):
+def none_str(value, none_value: str = "") -> str:
     """Turn value into a string, special case None to empty string."""
     if value is None:
         return none_value
     else:
         return str(value)
 
 
 def main(
-    db_url,
-    output_filename,
-    output_format,
-    marker=None,
-    minimal=False,
-    genus="",
-    species="",
-    sep=None,
-    debug=True,
+    db_url: str,
+    output_filename: str,
+    output_format: str,
+    marker: Optional[str] = None,
+    minimal: bool = False,
+    genus: str = "",
+    species: str = "",
+    sep: Optional[str] = None,
+    debug: bool = True,
 ):
     """Run the database dump with arguments from the command line."""
     if not sep:
         # TODO - Use this argument for tab/comma/etc in txt output?
         sep = ";"
 
     # Connect to the DB,
     Session = connect_to_db(db_url, echo=debug)
     session = Session()
 
-    entry_count = 0
+    entry_count: int = 0
 
     if output_filename == "-":
         out_handle = sys.stdout
     else:
         out_handle = open(output_filename, "w")
 
     # Doing a join to pull in the marker and taxonomy tables too:
@@ -114,18 +115,18 @@
         pass
     elif minimal:
         out_handle.write("#MD5\tSpecies\tSequence\n")
     else:
         out_handle.write("#Marker\tIdentifier\tGenus\tSpecies\tTaxID\tMD5\tSequence\n")
 
     if minimal:
-        md5_seq = {}
-        md5_sp = {}
+        md5_seq: dict[str, str] = {}
+        md5_sp: dict[str, set[str]] = {}
         for seq_source in view:
-            md5 = seq_source.marker_seq.md5
+            md5: str = seq_source.marker_seq.md5
             # genus_species = genus_species_name(
             #                            seq_source.taxonomy.genus,
             #                            seq_source.taxonomy.species,
             #                            )
             if md5 in md5_seq:
                 assert md5_seq[md5] == seq_source.marker_seq.sequence
                 md5_sp[md5].add(seq_source.taxonomy)
@@ -145,15 +146,15 @@
                 # Likely writing to stdout | head, or similar
                 # If so, stdout has been closed
                 sys.stderr.write("Aborting with broken pipe\n")
                 sys.stderr.close()
                 sys.exit(1)
         entry_count = len(md5_seq)
     elif output_format == "fasta":
-        seq_entry = {}
+        seq_entry: dict[str, set[str]] = {}
         for seq_source in view:
             seq = seq_source.marker_seq.sequence
             genus_species = genus_species_name(
                 seq_source.taxonomy.genus, seq_source.taxonomy.species
             )
             entry = f"{seq_source.source_accession} {genus_species}"
             if seq_source.taxonomy.ncbi_taxid:
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/edit_graph.py` & `thapbi_pict-1.0.9/thapbi_pict/edit_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2019-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Generate edit-distance network graph from FASTA files.
 
 This implements the ``thapbi_pict edit-graph ...`` command.
@@ -58,15 +58,15 @@
     #
     # Special cases:
     # ==============
     "synthetic": "#FFA500",  # Orange
 }
 
 
-def write_pdf(G, handle):
+def write_pdf(G, handle) -> None:
     """Render NetworkX graph to PDF using GraphViz fdp."""
     # TODO: Try "sfdp" but need GraphViz built with triangulation library
     default = G.graph["node_default"]["color"]
     node_colors = [G.nodes[_].get("color", default) for _ in G]
 
     default = 1.0
     node_sizes = [G.nodes[_].get("size", default) for _ in G]
@@ -94,15 +94,15 @@
         alpha=0.5,
     )
     nx.draw_networkx_labels(G, placement, node_labels, font_size=4)
     plt.axis("off")
     plt.savefig(handle, format="pdf")
 
 
-def write_xgmml(G, handle, name="THAPBI PICT edit-graph"):
+def write_xgmml(G, handle, name: str = "THAPBI PICT edit-graph") -> None:
     """Save graph in XGMML format suitable for Cytoscape import."""
     # Not currently supported in NetworkX, and third party
     # package networkxgmml is not up to date (Python 3,
     # setting graphical properties on edges). So, DIY time!
     handle.write(b'<?xml version="1.0" encoding="UTF-8" standalone="yes"?>\n')
     handle.write(
         b'<graph directed="0"  xmlns:dc="http://purl.org/dc/elements/1.1/" '
@@ -221,22 +221,22 @@
     """
     assert isinstance(input_file, str) or input_file is None
 
     if 3 < max_edit_dist:
         sys.exit("ERROR: Maximum supported edit distance is 3bp.")
 
     samples = set()
-    md5_abundance = Counter()
-    md5_sample_count = Counter()
+    md5_abundance: dict[str, int] = Counter()
+    md5_sample_count: dict[tuple[str, str], int] = Counter()
     abundance_by_samples = {}
-    max_sample_abundance = {}
-    md5_to_seq = {}
+    max_sample_abundance: dict[str, int] = {}
+    md5_to_seq: dict[str, str] = {}
     md5_species = {}
-    md5_in_db = set()
-    md5_in_fasta = set()
+    md5_in_db: set[str] = set()
+    md5_in_fasta: set[str] = set()
 
     if not (input_file or db_url):
         sys.exit("Require -d / --database and/or -i / --input argument.")
 
     if not input_file and not show_db_marker:
         sys.exit(
             "If not using -i / --input argument, require -k / --marker to use DB only."
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/ena_submit.py` & `thapbi_pict-1.0.9/thapbi_pict/ena_submit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright 2019-2021 by Peter Cock, The James Hutton Institute.
+# Copyright 2019-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Code for sample submission to ENA/SRA.
 
 This implements the ``thapbi_pict ena-submit ...`` command.
 """
 import os
 import shutil
 import sys
 import tempfile
+from typing import Optional
 
 from .prepare import find_fastq_pairs
 from .utils import load_metadata
 
 
 TABLE_HEADER = (
     "sample_alias\tinstrument_model\tlibrary_name\tlibrary_source\t"
@@ -23,15 +24,15 @@
     "forward_file_name\tforward_file_md5\t"
     "reverse_file_name\treverse_file_md5\n"
 )
 TABLE_TEMPLATE = "%s\t%s\t%s\tMETAGENOMIC\tPCR\tAMPLICON\t%s\t%s\t%i\t%s\t%s\t%s\t%s\n"
 assert TABLE_HEADER.count("\t") == TABLE_TEMPLATE.count("\t")
 
 
-def load_md5(file_list):
+def load_md5(file_list: list[str]) -> dict[str, str]:
     """Return a dict mapping given filenames to MD5 digests."""
     assert file_list, "Nothing to do here."
     answer = {}
     base_names = {os.path.split(_)[1] for _ in file_list}
     if len(base_names) < len(file_list):
         # This isn't a problem locally, but will be on upload to ENA
         sys.exit("ERROR: Duplicate FASTQ names once folder dropped")
@@ -55,22 +56,22 @@
         if f not in answer:
             sys.exit(f"ERROR: Need MD5 for {f} and not in {f}.md5 or MD5SUM.txt")
     return answer
 
 
 def write_table(
     handle,
-    pairs,
-    meta,
-    library_name,
-    instrument_model,
-    design_description,
-    library_construction_protocol,
-    insert_size,
-):
+    pairs: list[tuple[str, str, str]],
+    meta: Optional[dict[str, str]],
+    library_name: str,
+    instrument_model: str,
+    design_description: str,
+    library_construction_protocol: str,
+    insert_size: int,
+) -> None:
     """Write read file table for ENA upload."""
     file_list = [_[1] for _ in pairs] + [_[2] for _ in pairs]
     md5_dict = load_md5(file_list)
     lines = []
     for stem, raw_R1, raw_R2 in pairs:
         sample = os.path.split(stem)[1]
         folder = os.path.split(os.path.split(raw_R1)[0])[1]
@@ -91,29 +92,29 @@
         )
     handle.write(TABLE_HEADER)
     for line in sorted(lines):
         handle.write(line)
 
 
 def main(
-    fastq,
-    output,
-    metadata_file=None,
-    metadata_encoding=None,
-    metadata_cols=None,
-    metadata_fieldnames=None,
-    metadata_index=None,
-    ignore_prefixes=None,
-    library_name="-",
-    instrument_model="Illumina MiSeq",
-    design_description="",
-    library_construction_protocol="",
-    insert_size=250,
-    tmp_dir=None,
-    debug=False,
+    fastq: list[str],
+    output: str,
+    metadata_file: Optional[str] = None,
+    metadata_encoding: Optional[str] = None,
+    metadata_cols: Optional[str] = None,
+    metadata_fieldnames: Optional[str] = None,
+    metadata_index: Optional[str] = None,
+    ignore_prefixes: Optional[str] = None,
+    library_name: str = "-",
+    instrument_model: str = "Illumina MiSeq",
+    design_description: str = "",
+    library_construction_protocol: str = "",
+    insert_size: int = 250,
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
 ):
     """Implement the ``thapbi_pict ena-submit`` command."""
     fastq_file_pairs = find_fastq_pairs(fastq, debug=debug)
 
     if not fastq_file_pairs:
         sys.exit("ERROR: No FASTQ pairs found")
     if debug:
@@ -183,9 +184,11 @@
         instrument_model,
         design_description,
         library_construction_protocol,
         insert_size,
     )
 
     if output != "-":
+        assert table_handle is not None
         table_handle.close()
+        assert tmp_output is not None
         shutil.move(tmp_output, output)
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/fasta_nr.py` & `thapbi_pict-1.0.9/thapbi_pict/fasta_nr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-# Copyright 2018-2022 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Prepare a non-redundant FASTA file using MD5 naming.
 
 This implements the ``thapbi_pict fasta-nr ...`` command, using some of the
 same code internally as the ``thapbi_pict prepare-reads`` command.
 """
 import os
 import sys
 from collections import Counter
+from typing import Union
 
 from Bio.Seq import reverse_complement
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 
 from .prepare import save_nr_fasta
 from .utils import abundance_from_read_name
 
 
 def main(
-    inputs,
-    revcomp,
-    output,
-    min_abundance=0,
-    min_length=0,
-    max_length=sys.maxsize,
-    debug=False,
-):
+    inputs: Union[str, list[str]],
+    revcomp: Union[str, list[str]],
+    output: str,
+    min_abundance: int = 0,
+    min_length: int = 0,
+    max_length: int = sys.maxsize,
+    debug: bool = False,
+) -> None:
     """Implement the ``thapbi_pict fasta-nr`` command."""
     if not inputs:
         inputs = []
     if not revcomp:
         revcomp = []
     if isinstance(inputs, str):
         inputs = [inputs]
@@ -50,15 +51,15 @@
                     f" writing to {output}\n"
                 )
         else:
             sys.exit(
                 "ERROR: Output directory can only be used with a single input file"
             )
 
-    counts = Counter()
+    counts: dict[str, int] = Counter()
     for filename in inputs:
         # Assuming FASTA for now
         if debug:
             sys.stderr.write(f"DEBUG: Parsing {filename}\n")
         with open(filename) as handle:
             for _, seq in SimpleFastaParser(handle):
                 if min_length <= len(seq) <= max_length:
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/prepare.py` & `thapbi_pict-1.0.9/thapbi_pict/prepare.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 import os
 import shutil
 import sys
 import tempfile
 from collections import Counter
 from math import ceil
 from time import time
+from typing import Any
+from typing import Optional
+from typing import Union
 
 from Bio.Seq import reverse_complement
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from Bio.SeqIO.QualityIO import FastqGeneralIterator
 from sqlalchemy import func
 from sqlalchemy.orm import aliased
 from sqlalchemy.orm import contains_eager
@@ -34,19 +37,19 @@
 from .utils import md5seq
 from .utils import primer_clean
 from .utils import run
 from .versions import check_tools
 
 
 def find_fastq_pairs(
-    filenames_or_folders,
-    ext=(".fastq", ".fastq.gz", ".fq", ".fq.gz"),
-    ignore_prefixes=None,
-    debug=False,
-):
+    filenames_or_folders: list[str],
+    ext: tuple[str, ...] = (".fastq", ".fastq.gz", ".fq", ".fq.gz"),
+    ignore_prefixes: Optional[tuple[str]] = None,
+    debug: bool = False,
+) -> list[tuple[str, str, str]]:
     """Interpret a list of filenames and/or foldernames.
 
     Returns a list of tuples (stem, left filename, right filename)
     where stem is intended for use in logging and output naming,
     and may include a directory name.
 
     The filenames will be normalised relative to the current directory
@@ -145,15 +148,15 @@
                 f"ERROR: Did not recognise pair naming for {left!r} and {right!r}\n"
             )
         pairs.append((stem, left, right))
 
     return pairs
 
 
-def parse_cutadapt_stdout(stdout):
+def parse_cutadapt_stdout(stdout: str) -> tuple[int, int]:
     r"""Extract FASTA count before and after cutadapt.
 
     >>> parse_cutadapt_stdout("...\nTotal reads processed: 5,869\n...\nReads written (passing filters): 5,861 (99.9%)\n...")
     (5869, 5861)
     """  # noqa: E501
     before = None
     after = None
@@ -189,21 +192,21 @@
 Reads that were too long:                    0 (0.0%)
 Reads written (passing filters):         1,471 (1.4%)
 """,
 ) == (106089, 1471)
 
 
 def run_cutadapt(
-    long_in,
-    out_template,
-    marker_definitions,
-    flip=False,
-    debug=False,
-    cpu=0,
-):
+    long_in: str,
+    out_template: str,
+    marker_definitions: dict[str, Any],
+    flip: bool = False,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[int, int]:
     """Run cutadapt on a single file (i.e. after merging paired FASTQ).
 
     The input and/or output files may be compressed as long as they
     have an appropriate suffix (e.g. gzipped with ``.gz`` suffix).
 
     Returns FASTA count before and after cutadapt.
     """
@@ -238,15 +241,15 @@
         "-o",
         out_template,
         long_in,
     ]
     return parse_cutadapt_stdout(run(cmd, debug=debug).stdout)
 
 
-def parse_flash_stdout(stdout):
+def parse_flash_stdout(stdout: str) -> tuple[int, int]:
     r"""Extract FASTQ pair count before/after running flash.
 
     >>> parse_flash_stdout("...\n[FLASH] Read combination statistics:[FLASH]     Total pairs:      6105\n[FLASH]     Combined pairs:   5869\n...")
     (6105, 5869)
     """  # noqa: E501
     before = None
     after = None
@@ -270,15 +273,22 @@
 [FLASH]     Total pairs:      6105
 [FLASH]     Combined pairs:   5869
 ...
 """
 ) == (6105, 5869)
 
 
-def run_flash(trimmed_R1, trimmed_R2, output_dir, output_prefix, debug=False, cpu=0):
+def run_flash(
+    trimmed_R1: str,
+    trimmed_R2: str,
+    output_dir: str,
+    output_prefix: str,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[int, int]:
     """Run FLASH on a pair of trimmed FASTQ files to merge overlapping pairs.
 
     Returns two integers, FASTQ pair count for input and output files.
     """
     # Note our reads tend to overlap a lot, thus increase max overlap with -M
     # Also, some of our samples are mostly 'outies' rather than 'innies', so -O
     cmd = ["flash", "-O", "-M", "300"]
@@ -286,20 +296,20 @@
         # Default is all CPUs
         cmd += ["-t", str(cpu)]
     cmd += ["-d", output_dir, "-o", output_prefix, trimmed_R1, trimmed_R2]
     return parse_flash_stdout(run(cmd, debug=debug).stdout)
 
 
 def save_nr_fasta(
-    counts,
-    output_fasta,
-    min_abundance=0,
-    gzipped=False,
-    header_dict=None,
-):
+    counts: dict[str, int],
+    output_fasta: str,
+    min_abundance: int = 0,
+    gzipped: bool = False,
+    header_dict: Optional[dict[str, Union[str, int, None]]] = None,
+) -> tuple[int, int]:
     r"""Save a dictionary of sequences and counts as a FASTA file.
 
     Writes a FASTA file with header lines starting # (which not all tools will
     accept as valid FASTA format).
 
     The output FASTA records are named ``>MD5_abundance\n``, which is the
     default style used in SWARM. This could in future be generalised,
@@ -344,25 +354,25 @@
     if output_fasta != "-":
         out_handle.close()
     assert accepted_total >= 0
     return accepted_total, len(values)
 
 
 def make_nr_fasta(
-    input_fasta_or_fastq,
-    output_fasta,
-    min_abundance=0,
-    min_len=0,
-    max_len=sys.maxsize,
-    weighted_input=False,
-    fastq=False,
-    gzipped=False,
-    header_dict=None,
-    debug=False,
-):
+    input_fasta_or_fastq: str,
+    output_fasta: str,
+    min_abundance: int = 0,
+    min_len: int = 0,
+    max_len: int = sys.maxsize,
+    weighted_input: bool = False,
+    fastq: bool = False,
+    gzipped: bool = False,
+    header_dict: Optional[dict[str, Union[str, int, None]]] = None,
+    debug: bool = False,
+) -> tuple[int, int, int, int]:
     r"""Trim and make non-redundant FASTA/Q file from FASTA input.
 
     Makes a non-redundant FASTA file with the sequences named
     ``>MD5_abundance\n``.
 
     For FASTQ files all input reads are treated as abundance one
     (using weighted_input=True gives an error).
@@ -375,15 +385,15 @@
     ``>MD5_abundance\n``.
 
     Returns the total number of accepted reads before de-duplication
     (integer), number of those unique (integer), and the total number
     of those which passed the minimum abundance threshold (integer),
     and number of those which are unique (integer).
     """
-    counts = Counter()
+    counts: dict[str, int] = Counter()
     with open(input_fasta_or_fastq) as handle:
         if fastq:
             assert not weighted_input, "Not implemented for FASTQ"
             for _, seq, _ in FastqGeneralIterator(handle):
                 if min_len <= len(seq) <= max_len:
                     counts[seq.upper()] += 1
         elif weighted_input:
@@ -412,21 +422,21 @@
         len(counts),
         accepted_total,
         accepted_count,
     )
 
 
 def merge_paired_reads(
-    raw_R1,
-    raw_R2,
-    merged_fasta_gz,
-    tmp,
-    debug=False,
-    cpu=0,
-):
+    raw_R1: str,
+    raw_R2: str,
+    merged_fasta_gz: str,
+    tmp: str,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[int, int]:
     """Create NR FASTA file by overlap merging the paired FASTQ files."""
     if os.path.isfile(merged_fasta_gz):
         if debug:
             sys.stderr.write(f"DEBUG: Reusing {merged_fasta_gz}\n")
         # Just unzip and read header:
         header = load_fasta_header(merged_fasta_gz, gzipped=True)
         try:
@@ -458,30 +468,29 @@
             # "cutadapt": count_cutadapt,
             # "abundance": accepted_total,
             # "threshold": min_abundance,
         },
     )
     shutil.move(tmp_fasta_gz, merged_fasta_gz)
     del tmp_fasta_gz
-    merged_fastq = None
     return count_raw, count_flash
 
 
 def prepare_sample(
-    fasta_name,
-    trimmed_fasta,
-    headers,
-    min_len,
-    max_len,
-    min_abundance,
-    min_abundance_fraction,
-    tmp,
-    debug=False,
-    cpu=0,
-):
+    fasta_name: str,
+    trimmed_fasta: str,
+    headers: dict[str, Union[int, str, None]],
+    min_len: int,
+    max_len: int,
+    min_abundance: int,
+    min_abundance_fraction: float,
+    tmp: str,
+    debug: bool = False,
+    cpu: int = 0,
+) -> tuple[Optional[int], Optional[int], Optional[int], int]:
     """Create marker-specific FASTA file for sample from paired FASTQ.
 
     Applies abundance threshold, and min/max length.
 
     Returns pre-threshold total read count, accepted unique sequence count,
     accepted total read count, and the absolute abundance threshold used
     (higher of the given absolute threshold or the given fractional threshold).
@@ -542,14 +551,15 @@
     )
     if count_cutadapt < count:
         # Can be less if cutadapt had to use more relaxed global min/max length
         sys.exit(
             f"ERROR: Cutadapt says wrote {count_cutadapt}, but we saw {count} reads."
         )
     if debug:
+        assert isinstance(headers["raw_fastq"], int)
         count_raw = headers["raw_fastq"]
         count_flash = headers["flash"]
         if count_raw:
             sys.stderr.write(
                 "DEBUG:"
                 f" FASTQ pairs {count_raw}; flash -> {count_flash};"
                 f" cutadapt -> {count_cutadapt} [{uniq_count} unique];"
@@ -587,24 +597,24 @@
         accepted_total,
         min_abundance,
     )
 
 
 def marker_cut(
     marker_definitions,
-    file_pairs,
-    out_dir,
-    merged_cache,
-    tmp,
-    flip,
-    min_abundance,
-    min_abundance_fraction,
-    debug=False,
-    cpu=0,
-):
+    file_pairs: list[tuple[str, str, str]],
+    out_dir: str,
+    merged_cache: str,
+    tmp: str,
+    flip: bool,
+    min_abundance: int,
+    min_abundance_fraction: float,
+    debug: bool = False,
+    cpu: int = 0,
+) -> list[str]:
     """Apply primer-trimming for given markers."""
     sys.stderr.write(
         f"Looking for {len(marker_definitions)} markers in {len(file_pairs)} samples\n"
     )
 
     time_flash = time_cutadapt = time_abundance = 0.0
 
@@ -643,15 +653,16 @@
         ):
             # Run flash to merge reads; or parse pre-existing files
             start = time()
             count_raw, count_flash = merge_paired_reads(
                 raw_R1, raw_R2, merged_fasta_gz, tmp, debug=debug, cpu=cpu
             )
             time_flash += time() - start
-
+            assert count_raw is not None
+            assert count_flash is not None
             if count_flash:
                 # Run cutadapt to cut primers (giving one output per marker)
                 start = time()
                 unique_merged_, unique_cutadapt_ = run_cutadapt(
                     merged_fasta_gz,
                     # Here {name} is the cutadapt filename template:
                     os.path.join(tmp, stem + ".{name}.fasta"),
@@ -704,26 +715,30 @@
                 min_abundance_fraction,
                 tmp,
                 debug=debug,
                 cpu=cpu,
             )
             fasta_files_prepared.append(fasta_name)
             if uniq_count:
+                assert marker_total is not None
+                assert accepted_total is not None
                 assert accepted_total <= marker_total, (accepted_total, marker_total)
             if uniq_count is None:
                 skipped_samples.add(stem)
                 if debug:
                     sys.stderr.write(f"Skipping {fasta_name} as already done\n")
             elif min_a > 1:
+                assert marker_total is not None
                 sys.stderr.write(
                     f"Sample {stem} has {uniq_count} unique {marker} sequences,"
                     f" or {accepted_total}/{marker_total}"
                     f" reads over abundance threshold {min_a}\n"
                 )
             else:
+                assert marker_total is not None
                 assert accepted_total == marker_total
                 sys.stderr.write(
                     f"Sample {stem} has {uniq_count} unique {marker} sequences,"
                     f" or {accepted_total} reads (abundance threshold {min_a})\n"
                 )
         time_abundance += time() - start
         if debug:
@@ -747,15 +762,17 @@
 
     sys.stdout.flush()
     sys.stderr.flush()
 
     return fasta_files_prepared
 
 
-def load_marker_defs(session, spike_genus=""):
+def load_marker_defs(
+    session, spike_genus: str = ""
+) -> dict[str, dict[str, Union[int, str, list[tuple[str, str, set[str]]]]]]:
     """Load marker definitions and any spike-in sequences from the DB."""
     tmp_genus_set = set()
     # Split on commas, strip white spaces,
     for x in {_.strip() for _ in spike_genus.strip().split(",") if _.strip()}:
         view = session.query(Taxonomy).filter(func.lower(Taxonomy.genus) == x.lower())
         if not view.count():
             sys.stderr.write(
@@ -764,28 +781,30 @@
         else:
             for taxonomy in view:
                 tmp_genus_set.add(taxonomy.genus)  # record case as used in DB
     del spike_genus
     spike_genera = sorted(tmp_genus_set)
     del tmp_genus_set
 
-    marker_definitions = {}
+    marker_definitions: dict[
+        str, dict[str, Union[int, str, list[tuple[str, str, set[str]]]]]
+    ] = {}
     for reference_marker in session.query(MarkerDef).order_by(MarkerDef.name):
         if not reference_marker.left_primer or not reference_marker.right_primer:
             # TODO - ERROR if more than one marker? Always an error?
             sys.exit(f"ERROR: Missing primer(s) for {reference_marker.name}")
         if reference_marker.min_length > reference_marker.max_length:
             sys.exit(
                 f"ERROR: Marker {reference_marker.name}"
                 f" min length {reference_marker.min_length}"
                 f" but max length {reference_marker.max_length}"
             )
 
         # Spike-in negative controls are marker specific
-        spikes = []
+        spikes: list[tuple[str, str, set[str]]] = []
         if spike_genera:
             # Doing a join to pull in the marker and taxonomy tables too:
             cur_tax = aliased(Taxonomy)
             marker_seq = aliased(MarkerSeq)
             for seq_source in (
                 session.query(SeqSource)
                 .join(marker_seq, SeqSource.marker_seq)
@@ -812,26 +831,26 @@
             "max_length": reference_marker.max_length,
             "spike_kmers": spikes,
         }
     return marker_definitions
 
 
 def main(
-    fastq,
-    out_dir,
+    fastq: list[str],
+    out_dir: str,
     session,
-    flip=False,
-    min_abundance=2,
-    min_abundance_fraction=0,
-    ignore_prefixes=None,
-    merged_cache=None,
-    tmp_dir=None,
-    debug=False,
-    cpu=0,
-):
+    flip: bool = False,
+    min_abundance: int = 2,
+    min_abundance_fraction: float = 0.0,
+    ignore_prefixes: Optional[tuple[str]] = None,
+    merged_cache: Optional[str] = None,
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
+    cpu: int = 0,
+) -> list[str]:
     """Implement the ``thapbi_pict prepare-reads`` command.
 
     For use in the pipeline command, returns a filename listing of the FASTA
     files created.
     """
     assert isinstance(fastq, (list, set))
 
@@ -906,14 +925,15 @@
     )
 
     if tmp_dir:
         sys.stderr.write(
             f"WARNING: Please remove temporary files written to {tmp_dir}\n"
         )
     else:
+        assert tmp_obj is not None
         tmp_obj.cleanup()
 
     if debug:
         sys.stderr.write(f"Prepared {len(fasta_files_prepared)} FASTA files\n")
     sys.stdout.flush()
     sys.stderr.flush()
     return fasta_files_prepared
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/sample_tally.py` & `thapbi_pict-1.0.9/thapbi_pict/sample_tally.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2022-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Prepare a non-redundant TSV file using MD5 naming.
 
 This implements the ``thapbi_pict sample-tally ...`` command.
@@ -10,48 +10,50 @@
 import gzip
 import os
 import sys
 from collections import Counter
 from collections import defaultdict
 from math import ceil
 from time import time
+from typing import Optional
+from typing import Union
 
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 
 from .denoise import read_correction
 from .prepare import load_marker_defs
 from .utils import abundance_from_read_name
 from .utils import file_to_sample_name
 from .utils import is_spike_in
 from .utils import load_fasta_header
 from .utils import md5seq
 
 
 def main(
-    inputs,
-    synthetic_controls,
-    negative_controls,
-    output,
+    inputs: Union[str, list[str]],
+    synthetic_controls: list[str],
+    negative_controls: list[str],
+    output: str,
     session,
-    marker=None,
+    marker: Optional[str] = None,
     spike_genus=None,
     fasta=None,
-    min_abundance=100,
-    min_abundance_fraction=0.001,
-    total_min_abundance=0,
-    min_length=0,
-    max_length=sys.maxsize,
-    denoise_algorithm="-",
-    unoise_alpha=2.0,
-    unoise_gamma=4,
-    gzipped=False,  # output
-    tmp_dir=None,
-    debug=False,
-    cpu=0,
-):
+    min_abundance: int = 100,
+    min_abundance_fraction: float = 0.001,
+    total_min_abundance: int = 0,
+    min_length: int = 0,
+    max_length: int = sys.maxsize,
+    denoise_algorithm: str = "-",
+    unoise_alpha: float = 2.0,
+    unoise_gamma: int = 4,
+    gzipped: bool = False,  # output
+    tmp_dir: Optional[str] = None,
+    debug: bool = False,
+    cpu: int = 0,
+) -> None:
     """Implement the ``thapbi_pict sample-tally`` command.
 
     Arguments min_length and max_length are applied while loading the input
     per-sample FASTA files.
 
     Argument algorithm is a string, "-" for no read correction (denoising),
     "unoise-l" for our reimplementation of the UNOISE2 algorithm, or "usearch"
@@ -86,40 +88,43 @@
     if debug and not controls:
         sys.stderr.write("DEBUG: No control samples\n")
 
     if os.path.isdir(output):
         sys.exit("ERROR: Output directory given, want a filename.")
 
     marker_definitions = load_marker_defs(session, spike_genus)
+    spikes: list[tuple[str, str, set[str]]] = []
     if marker:
         if not marker_definitions:
             sys.exit("ERROR: Marker given with -k / --marker not in DB.")
-        spikes = marker_definitions[marker]["spike_kmers"]
+        marker_def = marker_definitions[marker]
     elif len(marker_definitions) > 1:
         sys.exit("ERROR: DB has multiple markers, please set -k / --marker.")
     else:
         # Implicit -k / --marker choice as only one in the DB
         marker, marker_def = marker_definitions.popitem()
-        spikes = marker_def["spike_kmers"]
-        del marker_def
+    assert isinstance(marker_def["spike_kmers"], list)
+    spikes = marker_def["spike_kmers"]
+    del marker_def
     del marker_definitions
     assert marker
 
-    totals = Counter()
-    counts = Counter()
-    sample_cutadapt = {}  # before any thresholds
-    samples = set()
-    sample_pool = {}
-    sample_headers = {}
+    totals: dict[str, int] = Counter()
+    counts: dict[tuple[str, str], int] = Counter()
+    sample_cutadapt: dict[str, int] = {}  # before any thresholds
+    samples: Union[set[str], list[str]] = set()
+    sample_pool: dict[str, str] = {}
+    sample_headers: dict[str, dict] = {}
     for filename in inputs:
         # Assuming FASTA for now
         if debug:
             sys.stderr.write(f"DEBUG: Parsing {filename}\n")
         sample = file_to_sample_name(filename)
         assert sample not in samples, f"ERROR: Duplicate stem from {filename}"
+        assert isinstance(samples, set)  # will later turn it into a list
         samples.add(sample)
         sample_headers[sample] = load_fasta_header(filename)
         if not sample_headers[sample]:
             if min_abundance_fraction or synthetic_controls:
                 sys.exit(
                     f"ERROR: Missing FASTA header in {filename}, "
                     "required for fractional abundance threshold\n"
@@ -148,31 +153,31 @@
         sys.stderr.write(
             f"Loaded {len(totals)} unique sequences from {sum(totals.values())}"
             f" in total within length range, max abundance {max(totals.values())}\n"
         )
     else:
         sys.stderr.write("WARNING: Loaded zero sequences within length range\n")
 
-    chimeras = {}
+    chimeras: dict[str, str] = {}
     if denoise_algorithm != "-":
         if debug:
             sys.stderr.write(
                 f"DEBUG: Starting read-correction with {denoise_algorithm}...\n"
             )
         corrections, chimeras = read_correction(
             denoise_algorithm,
             totals,
             unoise_alpha=unoise_alpha,
             unoise_gamma=unoise_gamma,
             tmp_dir=tmp_dir,
             debug=debug,
             cpu=cpu,
         )
-        new_counts = defaultdict(int)
-        new_totals = defaultdict(int)
+        new_counts: dict[tuple[str, str], int] = defaultdict(int)
+        new_totals: dict[str, int] = defaultdict(int)
         for (seq, sample), a in counts.items():
             if seq not in corrections:
                 # Should have been ignored as per UNOISE algorithm
                 if unoise_gamma:
                     assert (
                         totals[seq] < unoise_gamma
                     ), f"{md5seq(seq)} total {totals[seq]} vs {unoise_gamma}"
@@ -218,16 +223,16 @@
                 f"from {before} to {len(new_totals)}.\n"
             )
         del before
         counts = new_counts
         totals = new_totals
         del new_totals, new_counts
 
-    pool_absolute_threshold = {}
-    pool_fraction_threshold = {}
+    pool_absolute_threshold: dict[str, int] = {}
+    pool_fraction_threshold: dict[str, float] = {}
     max_spike_abundance = {sample: 0 for sample in samples}  # exporting in metadata
     max_non_spike_abundance = {sample: 0 for sample in samples}  # exporting in metadata
     if spikes:
         if debug:
             sys.stderr.write(
                 "DEBUG: About to identify spike-in synthetic sequences...\n"
             )
@@ -262,15 +267,15 @@
                 f"DEBUG: Spent {time_spike_tagging:0.1f}s tagging spike-in sequences.\n"
             )
     else:
         for (_, sample), a in counts.items():
             max_non_spike_abundance[sample] = max(max_non_spike_abundance[sample], a)
 
     start = time()
-    sample_threshold = {}
+    sample_threshold: dict[str, int] = {}
     if controls:
         if debug:
             sys.stderr.write("DEBUG: Applying dynamic abundance thresholds...\n")
         for sample in controls:
             pool = sample_pool[sample]
             a = max_non_spike_abundance[sample]
             # Ignore rest of pool. Respect FASTA header which could be more.
@@ -338,20 +343,20 @@
 
     for pool, value in pool_absolute_threshold.items():
         if value > min_abundance:
             sys.stderr.write(
                 f"Negative controls for marker {marker} increased "
                 f"pool {pool} absolute abundance threshold to {value}.\n"
             )
-    for pool, value in pool_fraction_threshold.items():
-        if value > min_abundance_fraction:
+    for pool, fraction in pool_fraction_threshold.items():
+        if fraction > min_abundance_fraction:
             sys.stderr.write(
                 f"Negative controls for marker {marker} increased "
                 f"pool {pool} fractional abundance threshold to "
-                f"{value*100:0.4f}%\n."
+                f"{fraction*100:0.4f}%\n."
             )
 
     # Apply any dynamic abundance threshold increases from controls:
     for sample in samples:
         if sample in controls:
             # Done above
             assert sample in sample_threshold, sample
@@ -430,15 +435,15 @@
     # (to match historic behaviour of pipeline via prepare-reads)
     for sample in samples:
         if max_spike_abundance[sample] < sample_threshold[sample]:
             max_spike_abundance[sample] = 0
         if max_non_spike_abundance[sample] < sample_threshold[sample]:
             max_non_spike_abundance[sample] = 0
 
-    samples = sorted(samples)
+    samples = sorted(samples)  # converting from set to list
     values = sorted(
         ((count, seq) for seq, count in totals.items()),
         # (sort by marker), then put the highest abundance entries first:
         key=lambda x: (-x[0], x[1]),
     )
     del totals
 
@@ -467,14 +472,15 @@
             raise ValueError(msg)
         out_handle = sys.stdout
     elif gzipped:
         out_handle = gzip.open(output, "wt")
     else:
         out_handle = open(output, "w")
     missing = [None] * len(samples)
+    stat_values: Union[list[int], list[str]] = []
     for stat in stats_fields:
         if stat == "Max non-spike":
             if not spike_genus:
                 continue
             stat_values = [max_non_spike_abundance[sample] for sample in samples]
         elif stat == "Max spike-in":
             if not spike_genus:
@@ -507,16 +513,16 @@
                 continue
             if None in stat_values:
                 sys.stderr.write(
                     f"WARNING: Missing some {stat} values in FASTA headers\n"
                 )
         if stat == "Threshold pool":
             # Try to remove any common folder prefix like raw_data/
-            # or C:/Users/... or /tmp/...
-            common = os.path.commonpath(set(stat_values))
+            # or C:/Users/... or /tmp/... - note making str type explicit:
+            common = os.path.commonpath([str(_) for _ in stat_values])
             if len(set(stat_values)) > 1 and common:
                 if debug:
                     sys.stderr.write(
                         f"DEBUG: Dropping threshold pool common prefix {common}\n"
                     )
                 stat_values = [_[len(common) + 1 :] for _ in stat_values]
             elif len(set(stat_values)) == 1:
@@ -569,13 +575,15 @@
             # TODO - Include the marker? Older fasta-nr command did not.
             if md5 in chimeras:
                 # Write any dict value as it is...
                 fasta_handle.write(f">{md5}_{count} chimera {chimeras[md5]}\n{seq}\n")
             else:
                 fasta_handle.write(f">{md5}_{count}\n{seq}\n")
     if output != "-":
+        assert out_handle is not None
         out_handle.close()
     if fasta and fasta != "-":
+        assert fasta_handle is not None
         fasta_handle.close()
     if debug:
         time_output = time() - start
         sys.stderr.write(f"DEBUG: Spent {time_output:0.1f}s writing output files\n")
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/summary.py` & `thapbi_pict-1.0.9/thapbi_pict/summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 by Peter Cock, The James Hutton Institute.
+# Copyright 2019-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Summarise classification results at sample and read level.
 
 This implements the ``thapbi_pict summary ...`` command.
@@ -12,39 +12,41 @@
 and statistics for the internally tracked information about
 each sample like the number of raw reads in the original FASTQ
 files (via header lines in the intermediate FASTA files).
 """
 import os
 import sys
 from collections import Counter
+from typing import Optional
+from typing import Union
 
 import xlsxwriter
 
 from .utils import color_bands
 from .utils import export_sample_biom
 from .utils import find_requested_files
 from .utils import load_metadata
 from .utils import md5seq
 from .utils import parse_sample_tsv
 
 MISSING_META = ""
 MISSING_DATA = "-"
 
 
-def _sp_display(species):
+def _sp_display(species: str) -> str:
     """Format species classification for reports, see also _sp_sort_key."""
     if " " in species:
         return species
     elif species:
         return species + " (unknown species)"
     else:
         return "Unknown"
 
 
-def _sp_sort_key(species):
+def _sp_sort_key(species: str) -> str:
     """Sort unknowns after knowns, see also _sp_display.
 
     Want this order:
 
       * Genus1 species1
       * Genus1 species2
       * Genus1 (unknown species) -- aka "Genus1"
@@ -372,15 +374,15 @@
     stats_fields,
     output,
     method,
     min_abundance=1,
     excel=None,
     biom=None,  # filename
     debug=False,
-):
+) -> None:
     """Create reads (rows) vs species (cols) report.
 
     The expectation is that the inputs represent all the samples
     from one (96 well) plate, or some other meaningful batch.
     """
     if biom and marker_md5_to_seq and stem_to_meta:
         if export_sample_biom(
@@ -689,29 +691,29 @@
 
     handle.close()
     workbook.close()
 
 
 def main(
     inputs,
-    report_stem,
-    method,
-    min_abundance=1,
-    metadata_file=None,
-    metadata_encoding=None,
-    metadata_cols=None,
-    metadata_groups=None,
-    metadata_fieldnames=None,
-    metadata_index=None,
-    require_metadata=False,
-    show_unsequenced=True,
-    ignore_prefixes=None,
-    biom=False,  # boolean
-    debug=False,
-):
+    report_stem: str,
+    method: str,
+    min_abundance: int = 1,
+    metadata_file: Optional[str] = None,
+    metadata_encoding: Optional[str] = None,
+    metadata_cols: Optional[str] = None,
+    metadata_groups: Optional[str] = None,
+    metadata_fieldnames: Optional[str] = None,
+    metadata_index: Optional[str] = None,
+    require_metadata: bool = False,
+    show_unsequenced: bool = True,
+    ignore_prefixes: Optional[tuple[str]] = None,
+    biom: bool = False,
+    debug: bool = False,
+) -> int:
     """Implement the ``thapbi_pict summary`` command.
 
     The expectation is that the inputs represent all the samples from
     a meaningful group, likely from multiple sequencing runs (plates).
     """
     # TODO - refactor the old separate reporting code
     assert isinstance(inputs, list)
@@ -732,15 +734,15 @@
         metadata_fieldnames,
         metadata_index,
         ignore_prefixes=ignore_prefixes,
         debug=debug,
     )
 
     meta_default = tuple([MISSING_META] * len(meta_names))
-    markers = set()
+    markers: set[str] = set()
 
     classifications_tsv = [
         _
         for _ in find_requested_files(inputs, f".{method}.tsv", ignore_prefixes, debug)
         # These are what we'll call the output files:
         if not _.endswith((f".reads.{method}.tsv", f".samples.{method}.tsv"))
     ]
@@ -749,37 +751,42 @@
 
     if debug:
         sys.stderr.write(
             f"DEBUG: Have metadata for {len(stem_to_meta)} samples, found "
             f"{len(classifications_tsv)} classifier files\n"
         )
 
-    marker_md5_abundance = Counter()
-    abundance_by_samples = {}
-    marker_md5_species = {}  # sp values are sets (e.g. ambiguous matches)
-    marker_md5_to_seq = {}
-    sample_species_counts = {}  # 2nd key is sp list with semi-colons
+    marker_md5_abundance: dict[tuple[str, str], int] = Counter()
+    abundance_by_samples: dict[tuple[str, str, str], int] = {}
+    marker_md5_species: dict[
+        tuple[str, str], set[str]
+    ] = {}  # sp values are sets (e.g. ambiguous matches)
+    marker_md5_to_seq: dict[tuple[str, str], str] = {}
+    sample_species_counts: dict[
+        str, dict[str, int]
+    ] = {}  # 2nd key is sp list with semi-colons
 
     # Not loading the post-abundance-threshold count,
     # Count should match the Seq-count column, but will not if running
     # report with higher abundance threshold - simpler to exclude.
     # For the threshold we have to update this if the report is stricter...
-    stats_fields = (
+    stats_fields: tuple[str, ...] = (
         "Raw FASTQ",
         "Flash",
         "Cutadapt",
         "Threshold pool",
         "Threshold",
         "Control",
         "Max non-spike",
         "Max spike-in",
         "Singletons",
     )
     blank_stat = -1
-    sample_stats = {}  # nested dict, keys are sample, then field name
+    # nested dict, keys are sample, then field name:
+    sample_stats: dict[str, dict[str, Union[str, int]]] = {}
 
     if not markers:
         # Corner case of zero sequences in all markers?
         assert not marker_md5_species
 
     if debug:
         sys.stderr.write(
@@ -905,23 +912,24 @@
                 if field in sample_stats[sample]:
                     del sample_stats[sample][field]
         stats_fields = tuple(field for field in stats_fields if field not in bad_fields)
     del bad_fields
 
     if "Threshold pool" in stats_fields:
         # Try to remove any common folder prefix like raw_data/
-        i = stats_fields.index("Threshold pool")
+        i: int = stats_fields.index("Threshold pool")
         paths = {_["Threshold pool"] for _ in sample_stats.values()}
-        common = os.path.commonpath(paths)
+        common = os.path.commonpath([str(_) for _ in paths])  # make type explicit!
         if len(paths) > 1 and common:
             if debug:
                 sys.stderr.write(
                     f"DEBUG: Dropping threshold pool common prefix {common}\n"
                 )
             for values in sample_stats.values():
+                assert isinstance(values, list)
                 values[i] = values[i][len(common) + 1 :]
 
     if require_metadata:
         assert set(sample_stats) == set(sample_species_counts) == set(stem_to_meta)
     else:
         assert set(sample_stats) == set(
             sample_species_counts
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/taxdump.py` & `thapbi_pict-1.0.9/thapbi_pict/taxdump.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,102 @@
-# Copyright 2018-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Code for THAPBI PICT to deal with NCBI taxonomy dumps.
 
 The code is needed initially for loading an NCBI taxdump folder (files
 ``names.dmp``, ``nodes.dmp``, ``merged.dmp`` etc) into a marker database.
 """
 import os
 import sys
 from collections import defaultdict
+from typing import Iterator
+from typing import Optional
+from typing import Sequence
 
 from .db_orm import connect_to_db
 from .db_orm import Synonym
 from .db_orm import Taxonomy
 from .utils import reject_species_name
 
 
-def load_nodes(nodes_dmp, wanted_ranks=None):
+def load_nodes(
+    nodes_dmp: str, wanted_ranks: Optional[Sequence[str]] = None
+) -> tuple[dict[int, int], dict[str, set[int]]]:
     """Load the NCBI taxdump nodes.dmp file.
 
     Returns two dicts, the parent/child relationships, and the ranks (values
     are lists of taxids).
 
     Default is all ranks, can provide a possibly empty list/set of ranks of
     interest.
     """
-    tree = {}
-    ranks = {}  # keys are rank names, values are lists of ids
+    tree: dict[int, int] = {}
+    ranks: dict[str, set[int]] = {}  # keys are rank names, values are sets of ids
     with open(nodes_dmp) as handle:
         for line in handle:
             parts = line.split("\t|\t", 3)
             taxid = int(parts[0].strip())
             parent = int(parts[1].strip())
             rank = parts[2].strip()
             tree[taxid] = parent
             if wanted_ranks is None or rank in wanted_ranks:
                 try:
-                    ranks[rank].append(taxid)
+                    ranks[rank].add(taxid)
                 except KeyError:
-                    ranks[rank] = [taxid]
+                    ranks[rank] = {
+                        taxid,
+                    }
     return tree, ranks
 
 
-def load_merged(merged_dmp, wanted=None):
+def load_merged(merged_dmp: str, wanted: Optional[set[int]] = None) -> dict[int, int]:
     """Load mapping of merged taxids of interest from NCBI taxdump merged.dmp file."""
     merged = {}
     with open(merged_dmp) as handle:
         for line in handle:
             parts = line.split("|", 3)
             alias = int(parts[0].strip())
             taxid = int(parts[1].strip())
             assert alias != taxid, line
             if wanted and taxid not in wanted:
                 continue
             merged[alias] = taxid
     return merged
 
 
-def load_names(names_dmp, wanted=None):
+def load_names(
+    names_dmp: str, wanted: Optional[set[int]] = None
+) -> tuple[dict[int, str], dict[int, set[str]]]:
     """Load scientific names of species from NCBI taxdump names.dmp file."""
     names = {}
-    synonym = defaultdict(list)
+    synonym = defaultdict(set)
     with open(names_dmp) as handle:
         for line in handle:
             parts = line.split("\t|\t", 3)
             taxid = int(parts[0].strip())
             if wanted and taxid not in wanted:
                 continue
             name = parts[1].strip()
             if line.endswith("\t|\tscientific name\t|\n"):
                 names[taxid] = name
             elif line.endswith(
                 ("\t|\tsynonym\t|\n", "\t|\tincludes\t|\n", "\t|\tequivalent name\t|\n")
             ):
                 # e.g. Phytophthora aquimorbida 'includes' Phytophthora sp. CCH-2009b
                 # which we want to treat like a synonym
-                synonym[taxid].append(name)
+                synonym[taxid].add(name)
     return names, synonym
 
 
-def filter_tree(tree, ranks, ancestors):
+def filter_tree(
+    tree: dict[int, int], ranks: dict[str, set[int]], ancestors: set[int]
+) -> tuple[dict[int, int], dict[str, set[int]]]:
     """Return a filtered version of the tree & ranks dict.
 
     NOTE: Does NOT preserve the original dict order.
     """
     count = len(tree)
     wanted = {a: a for a in ancestors}  # new tree
     reject = set()
@@ -119,62 +130,70 @@
                 # sys.stderr.write(f"Rejecting {taxid} via {batch}\n")
                 reject.add(taxid)
                 reject.update(batch)
                 break
     assert count == len(wanted) + len(reject)
 
     return wanted, {
-        rank: sorted(set(values).intersection(wanted)) for rank, values in ranks.items()
+        rank: set(values).intersection(wanted) for rank, values in ranks.items()
     }
 
 
-def get_ancestor(taxid, tree, stop_nodes):
+def get_ancestor(taxid: int, tree: dict[int, int], stop_nodes: set[int]) -> int:
     """Walk up tree until reach a stop node, or root."""
     t = taxid
     while True:
         if t in stop_nodes:
             return t
         elif not t or t == tree[t]:
             return t  # root
         else:
             t = tree[t]
 
 
-def species_or_species_groups(tree, ranks, names):
-    """Find taxids for species or species groups under the genus_list.
+def species_or_species_groups(
+    tree: dict[int, int], ranks: dict[str, set[int]], names: dict[int, str]
+) -> Iterator[tuple[int, int]]:
+    """Find taxids for species or species groups.
 
     Our "genus" list matches the NCBI rank "genus", and includes child nodes
     as aliases (unless they fall on our "species" list or reject list of
     "environmental samples" or "unclassified <genus>").
 
     However, our "species" list are either NCBI rank "species" or "species
     group" (in the later case child species are taken as aliases).
 
     Does not distinguish between "top level" species, or those under "no rank"
     nodes like "environmental samples" or "unclassified Phytophthora" (taxid
     211524),
 
     Yields (species taxid, genus taxid) tuples.
     """
-    genus_list = set(ranks["genus"])
+    genus_set = set(ranks["genus"])
     spgroup = set(ranks["species group"])
     species_or_spgroup = spgroup.union(ranks["species"])
     for taxid in tree:
         if taxid in species_or_spgroup and tree[taxid] not in spgroup:
             # Want this as a "species"
-            assert taxid not in genus_list
+            assert taxid not in genus_set, f"species {taxid} has genus rank!?"
             if reject_species_name(names[taxid]):
                 # Strange, but happens for "uncultured Hyaloperonospora"
                 # taxid 660915 which currently has rank "species"
                 continue
-            genus_taxid = get_ancestor(taxid, tree, genus_list)
+            genus_taxid = get_ancestor(taxid, tree, genus_set)
             yield taxid, genus_taxid
 
 
-def not_top_species(tree, ranks, names, synonyms, top_species):
+def not_top_species(
+    tree: dict[int, int],
+    ranks: dict[str, set[int]],
+    names: dict[int, str],
+    synonyms: dict[int, set[str]],
+    top_species,
+) -> Iterator[tuple[int, str]]:
     """Find all 'minor' species, takes set of species taxid to ignore.
 
     Will map assorted sub-species (i.e. any nodes under top_species) to the
     parent species, e.g. varietas 'Phytophthora nicotianae var. parasitica'
     NCBI:txid4791 will be mapped to species 'Phytophthora nicotianae'
     NCBI:txid4790 instead.
 
@@ -190,81 +209,81 @@
       genus 'Hyaloperonospora' NCBI:txid184462 - but we skip uncultured.
 
     However, if you wanted to import this part of the tree:
 
     * clade entry 'Skeletonema marinoi-dohrnii complex' NCBI:txid1171708 would
       be mapped to genus 'Skeletonema' NCBI:txid2842
 
-    Yields (genus taxid, node name, node taxid) tuples.
+    Yields (genus taxid, node name) tuples.
     """
     stop_nodes = set(top_species).union(ranks["genus"])
     for taxid in tree:
         if taxid in stop_nodes:
             continue
         parent = get_ancestor(taxid, tree, stop_nodes)
         if taxid != parent and not reject_species_name(names[taxid]):
             yield parent, names[taxid]
             if taxid in synonyms:
                 for name in synonyms[taxid]:
                     yield parent, name
             yield parent, f"NCBI:taxid{taxid}"
 
 
-def main(tax, db_url, ancestors, debug=True):
+def main(tax: str, db_url: str, ancestors: str, debug: bool = True) -> int:
     """Load an NCBI taxdump into a database."""
     if not os.path.isdir(tax):
         sys.exit(f"ERROR: Could not find taxdump directory: {tax!r}\n")
     for filename in ("names.dmp", "nodes.dmp"):
         if not os.path.isfile(os.path.join(tax, filename)):
             sys.exit(f"ERROR: Missing {filename} in the taxdump directory: {tax!r}\n")
 
     try:
-        ancestors = [int(_) for _ in ancestors.split(",")]
+        ancestors_set = {int(_) for _ in ancestors.split(",")}
     except ValueError:
         sys.exit(f"ERROR: Invalid ancestors argument: {ancestors!r}\n")
 
     tree, ranks = load_nodes(
         os.path.join(tax, "nodes.dmp"),
         ("genus", "species group", "species"),
     )
     if debug:
         sys.stderr.write(f"Loaded {len(tree)} nodes from nodes.dmp\n")
-    tree, ranks = filter_tree(tree, ranks, ancestors)
+    tree, ranks = filter_tree(tree, ranks, ancestors_set)
     if debug:
         sys.stderr.write(f"Reduced to {len(tree)} nodes under ancestors\n")
-    genus_list = sorted(ranks["genus"])
-    if not genus_list:
+    genus_set = set(ranks["genus"])
+    if not genus_set:
         sys.exit("ERROR: Could not identify any genus names under the given nodes\n")
-    tree, ranks = filter_tree(tree, ranks, genus_list)
+    tree, ranks = filter_tree(tree, ranks, genus_set)
     if debug:
         sys.stderr.write(
-            f"Reduced to {len(tree)} nodes under {len(genus_list)} genera\n"
+            f"Reduced to {len(tree)} nodes under {len(genus_set)} genera\n"
         )
-    assert genus_list == sorted(ranks["genus"])
+    assert sorted(genus_set) == sorted(ranks["genus"])  # remove?
 
-    names, synonyms = load_names(os.path.join(tax, "names.dmp"), tree)
+    names, synonyms = load_names(os.path.join(tax, "names.dmp"), set(tree))
     if debug:
         sys.stderr.write(f"Loaded {len(names)} scientific names from names.dmp\n")
 
     if debug:
         sys.stderr.write(
-            f"Identified {len(genus_list)} genera under specified ancestor node:"
-            f" {', '.join(sorted(names[_] for _ in genus_list))}\n"
+            f"Identified {len(genus_set)} genera under specified ancestor node:"
+            f" {', '.join(sorted(names[_] for _ in genus_set))}\n"
         )
 
     genus_species = sorted(species_or_species_groups(tree, ranks, names))
     if debug:
         sys.stderr.write(f"Filtered down to {len(genus_species)} species names\n")
 
-    merged = load_merged(os.path.join(tax, "merged.dmp"), tree)
+    merged = load_merged(os.path.join(tax, "merged.dmp"), set(tree))
     if debug:
         sys.stderr.write(f"Loaded {len(merged)} relevant aliases from merged.dmp\n")
     # Treat the merged nodes like aliases
     for alias, taxid in merged.items():
-        synonyms[taxid].append(f"NCBI:taxid{alias}")
+        synonyms[taxid].add(f"NCBI:taxid{alias}")
     del merged
 
     synonym_entries = defaultdict(set)
     for taxid, name in not_top_species(
         tree, ranks, names, synonyms, {_[0] for _ in genus_species}
     ):
         synonym_entries[taxid].add(name)
@@ -276,15 +295,15 @@
 
     # Connect to the DB,
     Session = connect_to_db(db_url, echo=False)  # echo=debug
     session = Session()
 
     g_old = 0
     g_new = 0
-    for taxid in genus_list:
+    for taxid in sorted(genus_set):
         genus = names[taxid]
         # Is genus already there? e.g. prior import
         taxonomy = (
             session.query(Taxonomy)
             .filter_by(genus=genus, species="", ncbi_taxid=taxid)
             .one_or_none()
         )
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/utils.py` & `thapbi_pict-1.0.9/thapbi_pict/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# Copyright 2018-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Helper functions for THAPB-PICT code."""
 import gzip
 import hashlib
 import os
 import subprocess
 import sys
 import time
 from collections import Counter
 from keyword import iskeyword
+from typing import Iterator
+from typing import Optional
+from typing import Union
 
 from Bio.Data.IUPACData import ambiguous_dna_values
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 
 
 KMER_LENGTH = 31
 
 
-def valid_marker_name(text):
+def valid_marker_name(text: str) -> bool:
     """Check the proposed string valid for use as a marker name.
 
     Want to be able to use the string for file or directory names, and also
     column names etc in reports. At very least should reject whitespace, line
     breaks, and slashes.
 
     Also rejecting all digits, as might want to accept integers as argument
@@ -40,101 +43,102 @@
         text.replace("-", "").isalnum()
         and not iskeyword(text)
         and not text.isdigit()
         and text != "pooled"
     )
 
 
-def primer_clean(primer):
+def primer_clean(primer: str) -> str:
     """Handle non-IUPAC entries in primers, maps I for inosine to N.
 
     >>> primer_clean("I")
     'N'
 
     Inosine is found naturally at the wobble position of tRNA, and can match
     any base. Structurally similar to guanine (G), it preferentially binds
     cytosine (C). It sometimes used in primer design (Ben-Dov et al, 2006),
     where degeneracy N would give similar results.
     """
     return primer.upper().replace("I", "N")
 
 
-def reject_species_name(species):
+def reject_species_name(species: str) -> bool:
     """Reject species names like 'environmental samples' or 'uncultured ...'."""
     return (
         not species
         or species.split(None, 1)[0] in ("unclassified", "uncultured", "unidentified")
         or species == "environmental samples"
     )
 
 
-def genus_species_name(genus, species):
+def genus_species_name(genus: str, species: str) -> str:
     """Return name, genus with species if present.
 
     Copes with species being None (or empty string).
     """
     # This is a simple function, centralising it for consistency
     assert genus and genus == genus.strip(), repr(genus)
     if species:
         assert species == species.strip(), repr(species)
         return f"{genus} {species}"
     else:
         return genus
 
 
-def genus_species_split(name):
+def genus_species_split(name: str) -> tuple[str, str]:
     """Return (genus, species) splitting on first space.
 
     If there are no spaces, returns (name, '') instead.
     """
     if " " in name:
-        return name.split(" ", 1)
+        g, s = name.split(" ", 1)
+        return (g, s)
     else:
         return name, ""
 
 
-def species_level(prediction):
+def species_level(prediction: str) -> bool:
     """Is this prediction at species level.
 
     Returns True for a binomial name (at least one space), False for genus
     only or no prediction.
     """
     assert ";" not in prediction, prediction
-    return prediction and " " in prediction
+    return bool(prediction) and " " in prediction
 
 
-def onebp_substitutions(seq):
+def onebp_substitutions(seq: str):
     """Generate all 1bp substitutions of the sequence.
 
     Assumes unambiguous IUPAC codes A, C, G, T only.
     """
     seq = seq.upper()
     variants = set()
     for i in range(len(seq)):
         for s in "ACGT":
             # One base substitutions
             variants.add(seq[:i] + s + seq[i + 1 :])
     variants.remove(seq)
     return variants
 
 
-def onebp_deletions(seq):
+def onebp_deletions(seq: str) -> set[str]:
     """Generate all variants of sequence with 1bp deletion.
 
     Assumes unambiguous IUPAC codes A, C, G, T only.
     """
     seq = seq.upper()
     variants = set()
     for i in range(len(seq)):
         # One base deletion
         variants.add(seq[:i] + seq[i + 1 :])
     return variants
 
 
-def onebp_inserts(seq):
+def onebp_inserts(seq: str) -> set[str]:
     """Generate all variants of sequence with 1bp insert.
 
     Assumes unambiguous IUPAC codes A, C, G, T only.
     """
     seq = seq.upper()
     variants = set()
     for i in range(len(seq)):
@@ -143,15 +147,15 @@
             variants.add(seq[:i] + s + seq[i:])
     for s in "ACGT":
         # One base "insertion" at the end
         variants.add(seq + s)
     return variants
 
 
-def expand_IUPAC_ambiguity_codes(seq):
+def expand_IUPAC_ambiguity_codes(seq: str):
     """Convert to upper case and iterate over possible unabmigous interpretations.
 
     This is a crude recursive implementation, intended for use on sequences with
     just a few ambiguity codes in them - it may not scale very well!
     """
     seq = seq.upper()
     ambig_letters = set(seq).difference(["A", "C", "G", "T"])
@@ -189,25 +193,25 @@
     "GTGGGGACGAAAGTCCCTGC",
     "GTGGGGACGAAAGTCCTTGC",
     "GTGGGGACGAAAGTCTCTGC",
     "GTGGGGACGAAAGTCTTTGC",
 ]
 
 
-def md5seq(seq):
+def md5seq(seq: str) -> str:
     """Return MD5 32-letter hex digest of the (upper case) sequence.
 
     >>> md5seq("ACGT")
     'f1f8f4bf413b16ad135722aa4591043e'
 
     """
     return hashlib.md5(seq.upper().encode("ascii")).hexdigest()
 
 
-def md5_hexdigest(filename, chunk_size=1024):
+def md5_hexdigest(filename: str, chunk_size: int = 1024) -> str:
     """Return the MD5 hex-digest of the given file."""
     hash_md5 = hashlib.md5()
     with open(filename, "rb") as f:
         while True:
             chunk = f.read(chunk_size)
             if not chunk:
                 # EOF
@@ -224,18 +228,18 @@
     if isinstance(cmd, list):
         # Quote any entries with spaces or semi-colons
         return " ".join('"%s"' % _ if (" " in _ or ";" in _) else _ for _ in cmd)
     else:
         return cmd
 
 
-def run(cmd, debug=False, attempts=1):
+def run(cmd, debug: bool = False, attempts: int = 1) -> subprocess.CompletedProcess:
     """Run a command via subprocess, abort if fails.
 
-    Returns a subprocess.CompletedProcess object.
+    Returns a subprocess.CompletedProcess object, or None if all attempts fail.
     """
     for i in range(attempts):
         if debug:
             if attempts > 1:
                 sys.stderr.write(
                     f"Attempt {i + 1} of {attempts} calling command:"
                     f" {cmd_as_string(cmd)}\n"
@@ -275,18 +279,18 @@
                     sys.stdout.write(e.stdout)
                     sys.stdout.flush()
                     sys.stderr.write(e.stderr)
                 sys.exit(
                     f"ERROR: Attempt {i + 1} of {attempts} failed"
                     f" with return code {e.returncode}, cmd:\n{cmd_as_string(cmd)}\n"
                 )
-    return None
+    raise RuntimeError(f"Attempts exceeded for {cmd}")
 
 
-def abundance_from_read_name(text, debug=False):
+def abundance_from_read_name(text: str, debug: bool = False) -> int:
     """Extract abundance from SWARM style read name.
 
     >>> abundance_from_read_name("9e8f051c64c2b9cc3b6fcb27559418ca_988")
     988
 
     If fails, will return one.
     """
@@ -294,15 +298,15 @@
         return int(text.rsplit("_", 1)[1])
     except (ValueError, IndexError):
         if debug:
             sys.stderr.write(f"WARNING: No abundance suffix in {text!r}\n")
         return 1
 
 
-def split_read_name_abundance(text, debug=False):
+def split_read_name_abundance(text: str, debug: bool = False) -> tuple[str, int]:
     """Split SWARM style read name into prefix and abundance.
 
     >>> abundance_from_read_name("9e8f051c64c2b9cc3b6fcb27559418ca_988")
     '9e8f051c64c2b9cc3b6fcb27559418ca', 988
 
     If fails to detect the abundance, will return the original text
     as the prefix with an abundance of 1.
@@ -312,19 +316,21 @@
         return prefix, int(abundance)
     except (ValueError, IndexError):
         if debug:
             sys.stderr.write(f"WARNING: No abundance suffix in {text!r}\n")
         return text, 1
 
 
-def abundance_values_in_fasta(fasta_file, gzipped=False):
+def abundance_values_in_fasta(
+    fasta_file: str, gzipped: bool = False
+) -> tuple[int, int, dict[str, int]]:
     """Return unique count, total abundance, and maximum abundances by spike-in."""
     unique = 0
     total = 0
-    max_a = Counter()
+    max_a: dict[str, int] = Counter()
     if gzipped:
         handle = gzip.open(fasta_file, "rt")
     else:
         handle = open(fasta_file)
     with handle:
         for title, _ in SimpleFastaParser(handle):
             unique += 1
@@ -334,42 +340,47 @@
                 hmm = title.split(None, 1)[1].strip()
             except IndexError:
                 hmm = ""  # prepared with no HMM
             max_a[hmm] = max(a, max_a[hmm])
     return unique, total, max_a
 
 
-def abundance_filter_fasta(input_fasta, output_fasta, min_abundance):
+def abundance_filter_fasta(
+    input_fasta: str, output_fasta: str, min_abundance: int
+) -> None:
     """Apply a minimum abundance filter to a FASTA file."""
     with open(input_fasta) as in_handle:
         with open(output_fasta, "w") as out_handle:
             for title, seq in SimpleFastaParser(in_handle):
                 a = abundance_from_read_name(title.split(None, 1)[0])
                 if a < min_abundance:
                     continue
                 out_handle.write(f">{title}\n{seq}\n")
 
 
-def file_to_sample_name(filename):
+def file_to_sample_name(filename: str) -> str:
     """Given filename (with or without a directory name), return sample name only.
 
     i.e. XXX.fasta, XXX.fastq.gz, XXX.method.tsv --> XXX
     """
     if filename.endswith(".fasta"):
         return os.path.basename(filename).rsplit(".", 1)[0]
     elif filename.endswith((".fasta.gz", ".tsv", ".fastq.gz")):
         return os.path.basename(filename).rsplit(".", 2)[0]
     else:
         msg = f"Invalid file_to_sample_name arg: {filename}"
         raise ValueError(msg)
 
 
 def find_requested_files(
-    filenames_or_folders, ext=".fasta", ignore_prefixes=None, debug=False
-):
+    filenames_or_folders: list[str],
+    ext: Union[str, tuple[str, ...]] = ".fasta",
+    ignore_prefixes: Optional[tuple[str]] = None,
+    debug: bool = False,
+) -> list[str]:
     """Interpret a list of filenames and/or foldernames.
 
     The extensions argument can be a tuple.
     """
     assert ignore_prefixes  # DEBUG - TODO - remove this
     answer = []
     for x in filenames_or_folders:
@@ -678,22 +689,22 @@
         for sample, value in zip(samples, parts[1:seq_col]):
             sample_headers[sample][name] = value
     return seqs, seq_meta, sample_headers, counts
 
 
 def parse_species_tsv(
     tabular_file, min_abundance=0, req_species_level=False, allow_wildcard=False
-):
+) -> Iterator[tuple[Optional[str], str, str, str]]:
     """Parse file of species assignments/predictions by sequence.
 
     Yields tuples of marker name (from the file header line), sequence name,
     taxid, and genus_species.
     """
-    marker = None
-    tally_mode = False
+    marker: Optional[str] = None
+    tally_mode: Optional[tuple] = None
     with open(tabular_file) as handle:
         for line in handle:
             if line.startswith("#"):
                 parts = line[1:].strip("\n").split("\t")
                 if parts[0].endswith("/sequence-name") and parts[1] == "taxid":
                     marker = parts[0][:-14]
                 if (
@@ -945,15 +956,15 @@
             f"ERROR: Duplicated metadata for {len(bad)} samples,"
             f" {sorted(bad)[0]} (etc)"
         )
 
     return stem_to_meta, meta_to_stem, names, group_col
 
 
-def color_bands(meta_groups, sample_color_bands, debug=False):
+def color_bands(meta_groups, sample_color_bands, debug: bool = False) -> list:
     """Return a list for formats, one for each sample."""
     default = [None] * len(meta_groups)
 
     min_groups = 3
     max_groups = 0.8 * len(meta_groups)
     if min_groups > max_groups:
         if debug:
@@ -1018,15 +1029,15 @@
                 return default
             bands.append(max(bands) + 1)
             debug_msg.append(value)
     assert len(set(bands)) == max(bands) + 1, bands
     return [sample_color_bands[_ % len(sample_color_bands)] for _ in bands]
 
 
-def load_fasta_header(fasta_file, gzipped=False):
+def load_fasta_header(fasta_file, gzipped=False) -> dict:
     """Parse our FASTA hash-comment line header as a dict."""
     answer = {}
     if gzipped:
         handle = gzip.open(fasta_file, "rt")
     else:
         handle = open(fasta_file)
     for line in handle:
@@ -1042,20 +1053,20 @@
         elif not line.strip():
             pass
         else:
             sys.exit(f"ERROR: Unexpected line in headered FASTA file {fasta_file}")
     return answer
 
 
-def kmers(sequence, k=KMER_LENGTH):
+def kmers(sequence: str, k: int = KMER_LENGTH) -> set[str]:
     """Make set of all kmers in the given sequence."""
     return {sequence[i : i + k] for i in range(len(sequence) - k + 1)}
 
 
-def is_spike_in(sequence, spikes):
+def is_spike_in(sequence: str, spikes: list[tuple[str, str, set[str]]]) -> str:
     """Return spike-in name if sequence matches, else empty string."""
     for spike_name, spike_seq, spike_kmers in spikes:
         if sequence == spike_seq:
             return spike_name
         # This will not work when len(spike) <~ kmer length
         # (fail gracefully with an impossible to meet value of 10)
         threshold = max((len(spike_seq) - KMER_LENGTH) / 3, 10)
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict/versions.py` & `thapbi_pict-1.0.9/thapbi_pict/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2023 by Peter Cock, The James Hutton Institute.
+# Copyright 2019-2024 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """Helper code to get command line tool versions.
 
 Defines various functions to check a tool is on the ``$PATH`` and if so,
@@ -16,38 +16,39 @@
 
 If we cannot parse the output, again the commands return None - which is
 likely an indication of a major version change, meaning the tool ought to be
 re-evaluated for use with THAPBI-PICT.
 """
 import sys
 from subprocess import getoutput
+from typing import Optional
 
 
-def check_rapidfuzz():
+def check_rapidfuzz() -> str:
     """Check can import rapidfuzz and confirm recent enough."""
     try:
         import rapidfuzz
     except ImportError:
         sys.exit("ERROR: Missing Python library rapidfuzz")
     try:
-        version = rapidfuzz.__version__
+        version: str = rapidfuzz.__version__
     except AttributeError:
         sys.exit("ERROR: Could not check rapidfuzz.__version__")
     try:
         major_minor = tuple(int(_) for _ in version.split(".")[:2])
     except ValueError:
         sys.exit(
             f"ERROR: Could not parse rapidfuzz.__version__ {rapidfuzz.__version__}"
         )
     if major_minor < (2, 4):
         sys.exit(f"ERROR: Need at least rapidfuzz v2.4, have {rapidfuzz.__version__}")
     return version
 
 
-def check_tools(names, debug):
+def check_tools(names: list[str], debug: bool) -> list[str]:
     """Verify the named tools are present, log versions if debug=True.
 
     Argument names should be an interable of tool binary names.
 
     If all the tools are present, returns a list of version strings.
 
     If any tools are missing (or have a version we could not parse),
@@ -79,15 +80,15 @@
         sys.exit("ERROR: Missing external tool: " + missing[0])
     elif missing:
         sys.exit("ERROR: Missing external tool(s): " + ",".join(missing))
     else:
         return versions
 
 
-def version_blast(cmd="blastn"):
+def version_blast(cmd: str = "blastn") -> Optional[str]:
     """Return the version of the NCBI BLAST+ suite's blastn (as a short string).
 
     In the absence of a built in version switch like ``-v``, this works by
     parsing the short help output with ``-h`` (which does vary between the
     tools in the suite)::
 
         $ makeblastdb -h | grep BLAST
@@ -110,15 +111,15 @@
         if line.strip().endswith("+"):
             words = line.strip().split()
             if "BLAST" in words or "version" in words:
                 return words[-1]
     return None
 
 
-def version_cutadapt(cmd="cutadapt"):
+def version_cutadapt(cmd: str = "cutadapt") -> Optional[str]:
     """Return the version of cutadapt (as a short string).
 
     Uses the output with ``--version``::
 
         $ cutadapt --version
         1.18
 
@@ -131,15 +132,15 @@
     """
     text = getoutput(cmd + " --version").strip().split("\n", 1)[0]
     if "." in text:
         return text
     return None
 
 
-def version_flash(cmd="flash"):
+def version_flash(cmd: str = "flash") -> Optional[str]:
     """Return the version of flash (as a short string).
 
     Parses the output with ``-v``::
 
         $ flash -v | head -n 1
         FLASH v1.2.11
 
@@ -153,15 +154,15 @@
     text = getoutput(cmd + " -v")
     ver = text.split("\n", 1)[0]
     if ver.upper().startswith("FLASH V"):
         return ver[7:]
     return None
 
 
-def version_usearch(cmd="usearch"):
+def version_usearch(cmd: str = "usearch") -> Optional[str]:
     """Return the version of usearch (as a short string).
 
     Uses the output with ``--version``::
 
         $ usearch --version
         usearch v11.0.667_i86linux32
 
@@ -175,15 +176,15 @@
     text = getoutput(cmd + " --version").strip().split("\n", 1)[0]
     ver = text.split("_", 1)[0]
     if ver.lower().startswith("usearch v"):
         return ver[8:]
     return None
 
 
-def version_vsearch(cmd="vsearch"):
+def version_vsearch(cmd: str = "vsearch") -> Optional[str]:
     """Return the version of vsearch (as a short string).
 
     Uses the output with ``--version``::
 
         $ vsearch --version
         ...
         vsearch v2.22.1_macos_x86_64, 8.0GB RAM, 8 cores
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict.egg-info/PKG-INFO` & `thapbi_pict-1.0.9/thapbi_pict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thapbi_pict
-Version: 1.0.8
+Version: 1.0.9
 Summary: THAPBI Phytophthora ITS1 Classifier Tool (PICT).
 Home-page: https://github.com/peterjc/thapbi-pict
 Download-URL: https://github.com/peterjc/thapbi-pict
 Author: Peter Cock
 Author-email: peter.cock@hutton.ac.uk
 Project-URL: Documentation, https://thapbi-pict.readthedocs.io/
 Project-URL: Source, https://github.com/peterjc/thapbi-pict/
```

### Comparing `thapbi_pict-1.0.8/thapbi_pict.egg-info/SOURCES.txt` & `thapbi_pict-1.0.9/thapbi_pict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

