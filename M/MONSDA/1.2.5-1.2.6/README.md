# Comparing `tmp/monsda-1.2.5.tar.gz` & `tmp/monsda-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsda-1.2.5.tar", last modified: Tue Apr 16 12:15:45 2024, max compression
+gzip compressed data, was "monsda-1.2.6.tar", last modified: Wed May 22 12:27:33 2024, max compression
```

## Comparing `monsda-1.2.5.tar` & `monsda-1.2.6.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.108296 monsda-1.2.5/
--rw-r--r--   0 fall      (1000) fall      (1000)    35149 2024-03-04 09:35:20.000000 monsda-1.2.5/LICENSE
--rw-r--r--   0 fall      (1000) fall      (1000)       49 2024-03-04 09:35:20.000000 monsda-1.2.5/MANIFEST.in
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.091296 monsda-1.2.5/MONSDA/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    70162 2024-03-25 16:31:46.000000 monsda-1.2.5/MONSDA/Configurator.py
--rw-r--r--   0 fall      (1000) fall      (1000)     5763 2024-03-04 09:35:20.000000 monsda-1.2.5/MONSDA/Deprecated.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2581 2024-03-04 09:35:20.000000 monsda-1.2.5/MONSDA/Logger.py
--rw-r--r--   0 fall      (1000) fall      (1000)    37733 2024-03-25 16:31:46.000000 monsda-1.2.5/MONSDA/Params.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    34812 2024-03-28 08:34:24.000000 monsda-1.2.5/MONSDA/RunMONSDA.py
--rw-r--r--   0 fall      (1000) fall      (1000)    18515 2024-03-25 16:31:46.000000 monsda-1.2.5/MONSDA/Utils.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)   171767 2024-03-25 16:31:46.000000 monsda-1.2.5/MONSDA/Workflows.py
--rw-r--r--   0 fall      (1000) fall      (1000)       73 2024-03-04 09:35:20.000000 monsda-1.2.5/MONSDA/__init__.py
--rw-r--r--   0 fall      (1000) fall      (1000)       32 2024-03-04 09:35:20.000000 monsda-1.2.5/MONSDA/__main__.py
--rw-r--r--   0 fall      (1000) fall      (1000)      497 2024-04-16 12:15:45.108296 monsda-1.2.5/MONSDA/_version.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.092296 monsda-1.2.5/MONSDA/lib/
--rw-r--r--   0 fall      (1000) fall      (1000)     2357 2024-03-04 09:35:20.000000 monsda-1.2.5/MONSDA/lib/Collection.groovy
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.108296 monsda-1.2.5/MONSDA.egg-info/
--rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-04-16 12:15:45.000000 monsda-1.2.5/MONSDA.egg-info/PKG-INFO
--rw-r--r--   0 fall      (1000) fall      (1000)     6004 2024-04-16 12:15:45.000000 monsda-1.2.5/MONSDA.egg-info/SOURCES.txt
--rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-04-16 12:15:45.000000 monsda-1.2.5/MONSDA.egg-info/dependency_links.txt
--rw-r--r--   0 fall      (1000) fall      (1000)       93 2024-04-16 12:15:45.000000 monsda-1.2.5/MONSDA.egg-info/entry_points.txt
--rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-19 14:46:42.000000 monsda-1.2.5/MONSDA.egg-info/not-zip-safe
--rw-r--r--   0 fall      (1000) fall      (1000)       89 2024-04-16 12:15:45.000000 monsda-1.2.5/MONSDA.egg-info/requires.txt
--rw-r--r--   0 fall      (1000) fall      (1000)        7 2024-04-16 12:15:45.000000 monsda-1.2.5/MONSDA.egg-info/top_level.txt
--rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-04-16 12:15:45.108296 monsda-1.2.5/PKG-INFO
--rw-r--r--   0 fall      (1000) fall      (1000)     6058 2024-03-04 09:43:25.000000 monsda-1.2.5/README.md
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.092296 monsda-1.2.5/configs/
--rw-r--r--   0 fall      (1000) fall      (1000)    24464 2024-04-16 12:14:02.000000 monsda-1.2.5/configs/template.json
--rw-r--r--   0 fall      (1000) fall      (1000)    14131 2024-03-04 09:43:25.000000 monsda-1.2.5/configs/template_base_commented.json
--rw-r--r--   0 fall      (1000) fall      (1000)     9007 2024-04-16 12:14:02.000000 monsda-1.2.5/configs/template_clean.json
--rw-r--r--   0 fall      (1000) fall      (1000)    19963 2024-04-16 12:14:02.000000 monsda-1.2.5/configs/tutorial_exhaustive.json
--rw-r--r--   0 fall      (1000) fall      (1000)    13787 2024-04-16 12:14:02.000000 monsda-1.2.5/configs/tutorial_postprocess.json
--rw-r--r--   0 fall      (1000) fall      (1000)     1171 2024-04-16 12:14:02.000000 monsda-1.2.5/configs/tutorial_quick.json
--rw-r--r--   0 fall      (1000) fall      (1000)     8919 2024-04-16 12:14:02.000000 monsda-1.2.5/configs/tutorial_toolmix.json
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.096296 monsda-1.2.5/envs/
--rw-r--r--   0 fall      (1000) fall      (1000)     5071 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/LoveSonesonPatro.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      259 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/base.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/bbduk.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/bbmap.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      210 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/bedtools.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      132 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/bwa.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      136 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/bwa2.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/bwameth.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      122 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/ciri2.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      356 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/countreads.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      359 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/countreads_de.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      118 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/cutadapt.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     4345 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/deseq2_DE.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     3328 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/dexseq_DEU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     3200 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/dexseq_DTU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      347 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/diego_DAS.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      120 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/dorado.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     2948 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/drimseq_DTU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/edger_DAS.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     2758 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/edger_DE.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/edger_DEU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.5/envs/fastqc.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      290 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/guppy.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      190 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/hisat2.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      149 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/index.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     3195 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/isoformswitchanalyzer.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      153 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/macs.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      139 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/minimap.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      632 2024-04-16 12:14:02.000000 monsda-1.2.5/envs/monsda.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     6213 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/peaks.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     1525 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/perl.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      129 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/picard.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      142 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/piranha.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.5/envs/qc.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      103 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/salmon.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      131 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/samtools.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      213 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/scyphy.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      151 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/segemehl.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      145 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/segemehl3.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      158 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/sra.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      121 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/star.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      562 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/summary.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      123 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/trimgalore.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      235 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/trimm.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      161 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/trimmomatic.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/trnascan.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      228 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/ucsc.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      150 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/umitools.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      106 2024-03-04 09:35:20.000000 monsda-1.2.5/envs/zip.yaml
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.096296 monsda-1.2.5/profile_nextflow/
--rw-r--r--   0 fall      (1000) fall      (1000)      217 2024-03-27 11:17:58.000000 monsda-1.2.5/profile_nextflow/nextflow.config
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.096296 monsda-1.2.5/profile_snakemake/
--rw-r--r--   0 fall      (1000) fall      (1000)      344 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/cluster_config.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      277 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/config.yaml
--rwxr-xr-x   0 fall      (1000) fall      (1000)       51 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/slurm-jobscript.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)     1826 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/slurm-status.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    10397 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/slurm-submit-advanced.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     1880 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/slurm-submit.py
--rw-r--r--   0 fall      (1000) fall      (1000)    10495 2024-03-04 09:35:20.000000 monsda-1.2.5/profile_snakemake/slurm_utils.py
--rw-r--r--   0 fall      (1000) fall      (1000)     1303 2024-03-28 12:07:30.000000 monsda-1.2.5/pyproject.toml
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.089296 monsda-1.2.5/scripts/
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.097296 monsda-1.2.5/scripts/Analysis/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2882 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/AddStructure.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3647 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/Cluster2tRNA.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    12627 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/CollectBamStat.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    25757 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/CountEnds.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)      490 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/CountFastqEnds.pl
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.098296 monsda-1.2.5/scripts/Analysis/DAS/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    27615 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DAS/DIEGO.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    12133 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DAS/EDGER.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2108 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)    13715 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DAS/FeatureCounts2DIEGO.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     4720 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DAS/diego_contrast_files.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.098296 monsda-1.2.5/scripts/Analysis/DE/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    15681 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DE/DESEQ2.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)    16168 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DE/EDGER.R
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.098296 monsda-1.2.5/scripts/Analysis/DEU/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     9059 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DEU/DEXSEQ.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     9938 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DEU/EDGER.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     9611 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DEU/prepare_deu_annotation.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.098296 monsda-1.2.5/scripts/Analysis/DTU/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     7268 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DTU/DEXSEQ.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)    14986 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/DTU/DRIMSEQ.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3421 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/FindPeaks.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2737 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/GOA.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)    14628 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/GenerateTrackDb.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)      426 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/GettRNAExpression.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)     5106 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/NormalizePeaks.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     5174 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/PlBed2Bedgraph.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2228 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/PreprocessPeaks.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     8094 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/RemoveSoftClip.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    11489 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/RmdCreator.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.098296 monsda-1.2.5/scripts/Analysis/SUMMARY/
--rwxr-xr-x   0 fall      (1000) fall      (1000)      408 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/SUMMARY/header_summary.Rmd
--rwxr-xr-x   0 fall      (1000) fall      (1000)    13324 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/build_DEU_table.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    10925 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/build_DTU_table.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    14005 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/build_count_table.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    11421 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Analysis/build_salmon_table.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.098296 monsda-1.2.5/scripts/Preprocessing/
--rwxr-xr-x   0 fall      (1000) fall      (1000)      237 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Preprocessing/indexfa.sh
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.099296 monsda-1.2.5/scripts/Shells/
--rw-r--r--   0 fall      (1000) fall      (1000)     1754 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/MergeExpression_Cufflinks.sh
--rw-r--r--   0 fall      (1000) fall      (1000)     1620 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/MergeExpression_RNAcounter.sh
--rw-r--r--   0 fall      (1000) fall      (1000)     1517 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/MergeGeneExpression_Cufflinks.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      670 2024-03-25 16:31:46.000000 monsda-1.2.5/scripts/Shells/NonUniqueBam_woPicard.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      565 2024-03-15 07:51:51.000000 monsda-1.2.5/scripts/Shells/NonUniqueBam_woPicard.sh~
--rwxr-xr-x   0 fall      (1000) fall      (1000)      460 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/Sam2Bam.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      440 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/Sam2Bed.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      966 2024-04-16 12:14:02.000000 monsda-1.2.5/scripts/Shells/UniqueBam_woPicard.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      551 2024-03-15 07:50:55.000000 monsda-1.2.5/scripts/Shells/UniqueBam_woPicard.sh~
--rwxr-xr-x   0 fall      (1000) fall      (1000)     1628 2024-04-16 12:14:02.000000 monsda-1.2.5/scripts/Shells/UniqueSam_woPicard.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      536 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/printEnds.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      342 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Shells/printFQEnds.sh
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.100296 monsda-1.2.5/scripts/Universal/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     8806 2024-03-28 12:04:17.000000 monsda-1.2.5/scripts/Universal/AnnotateBed.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     5046 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Universal/Bed2Bedgraph.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     8118 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Universal/ExtendBed.pl
--rw-r--r--   0 fall      (1000) fall      (1000)     2303 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Universal/countCCA.pl
--rw-r--r--   0 fall      (1000) fall      (1000)      710 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/Universal/sam2fastq.pl
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.100296 monsda-1.2.5/scripts/lib/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    67149 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/lib/Collection.pm
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3227 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/lib/Logger.py
--rw-r--r--   0 fall      (1000) fall      (1000)        0 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/lib/__init.py__
--rw-r--r--   0 fall      (1000) fall      (1000)     1099 2024-03-04 09:35:20.000000 monsda-1.2.5/scripts/lib/_lib.R
--rw-r--r--   0 fall      (1000) fall      (1000)      648 2024-04-16 12:15:45.108296 monsda-1.2.5/setup.cfg
--rw-r--r--   0 fall      (1000) fall      (1000)     3297 2024-03-26 16:29:05.000000 monsda-1.2.5/setup.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.100296 monsda-1.2.5/tests/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3454 2024-03-25 16:31:46.000000 monsda-1.2.5/tests/test_functions.py
--rw-r--r--   0 fall      (1000) fall      (1000)    78254 2024-03-04 09:35:20.000000 monsda-1.2.5/versioneer.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-04-16 12:15:45.107296 monsda-1.2.5/workflows/
--rw-r--r--   0 fall      (1000) fall      (1000)     7289 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/annotatebed.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2023 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bbduk.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2713 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bbduk.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3857 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bwa.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    14226 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bwa.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3846 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bwa2.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3499 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bwa2.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4232 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bwameth.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3360 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/bwameth.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2050 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/ciri2.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1816 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/ciri2.smk
--rw-r--r--   0 fall      (1000) fall      (1000)      507 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/collect.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     9861 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/countreads.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    15432 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/countreads.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2243 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/cutadapt.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2934 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/cutadapt.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7456 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/deseq2_DE.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7927 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/deseq2_DE.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     9193 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/dexseq_DEU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8476 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/dexseq_DEU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     8100 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/dexseq_DTU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    10062 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/dexseq_DTU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     9334 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/diego_DAS.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8157 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/diego_DAS.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1394 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/dorado.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1262 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/dorado.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     8123 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/drimseq_DTU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    13421 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/drimseq_DTU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7763 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/edger_DAS.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7887 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/edger_DAS.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7631 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/edger_DE.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7806 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/edger_DE.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7681 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/edger_DEU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7668 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/edger_DEU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3191 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     5830 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2040 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_dedup.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4596 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_dedup.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2851 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_dedup_trim.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     5978 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_dedup_trim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)      860 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_raw.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2901 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_raw.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2069 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_trim.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4661 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/fastqc_trim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/footer.nf
--rw-r--r--   0 fall      (1000) fall      (1000)       90 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/footer.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1788 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/guppy.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1661 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/guppy.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1609 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/header.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    12190 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/header.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4459 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/hisat2.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4844 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/hisat2.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7366 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/macs.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    14219 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/macs.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2372 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/manipulate_genome.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2359 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/manipulate_genome.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4247 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/mapping.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2698 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/mapping.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3854 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/minimap.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2968 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/minimap.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1022 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/multiqc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    10636 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/multiqc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     5667 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/notify.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    11912 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/peaks.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    21124 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/peaks.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1797 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/picard_dedup.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1250 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/picard_dedup.smk
--rw-r--r--   0 fall      (1000) fall      (1000)    12177 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/piranha.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    20575 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/piranha.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1150 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/premultiqc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1557 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/premultiqc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     5313 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/salmon.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3679 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/salmon.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4997 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/salmon_trim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)    22666 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/scyphy.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    32938 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/scyphy.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3881 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3098 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4378 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl3.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4699 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl3.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4613 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl3_bisulfite.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3695 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl3_bisulfite.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4681 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl_bisulfite.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3848 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/segemehl_bisulfite.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1719 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/simulatetrim.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1425 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/simulatetrim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2017 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/sra.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3905 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/sra.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     6531 2024-03-25 16:31:46.000000 monsda-1.2.5/workflows/star.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8723 2024-03-25 16:31:46.000000 monsda-1.2.5/workflows/star.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1190 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/summary.nf
--rw-r--r--   0 fall      (1000) fall      (1000)      857 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/summary.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2028 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/trimgalore.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3378 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/trimgalore.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7481 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/ucsc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8139 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/ucsc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4093 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/umitools.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7717 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/umitools.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1656 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/umitools_dedup.nf
--rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-04 09:35:20.000000 monsda-1.2.5/workflows/unlock.smk
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.704138 monsda-1.2.6/
+-rw-r--r--   0 fall      (1000) fall      (1000)    35149 2024-03-04 09:35:20.000000 monsda-1.2.6/LICENSE
+-rw-r--r--   0 fall      (1000) fall      (1000)       49 2024-03-04 09:35:20.000000 monsda-1.2.6/MANIFEST.in
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.684138 monsda-1.2.6/MONSDA/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    70162 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Configurator.py
+-rw-r--r--   0 fall      (1000) fall      (1000)     5763 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/Deprecated.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2581 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/Logger.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    37733 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Params.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    34812 2024-03-28 08:34:24.000000 monsda-1.2.6/MONSDA/RunMONSDA.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    18515 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Utils.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)   171767 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Workflows.py
+-rw-r--r--   0 fall      (1000) fall      (1000)       73 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/__init__.py
+-rw-r--r--   0 fall      (1000) fall      (1000)       32 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/__main__.py
+-rw-r--r--   0 fall      (1000) fall      (1000)      497 2024-05-22 12:27:33.704138 monsda-1.2.6/MONSDA/_version.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.685138 monsda-1.2.6/MONSDA/lib/
+-rw-r--r--   0 fall      (1000) fall      (1000)     2357 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/lib/Collection.groovy
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.703138 monsda-1.2.6/MONSDA.egg-info/
+-rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/PKG-INFO
+-rw-r--r--   0 fall      (1000) fall      (1000)     6004 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/SOURCES.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/dependency_links.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)       93 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/entry_points.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-19 14:46:42.000000 monsda-1.2.6/MONSDA.egg-info/not-zip-safe
+-rw-r--r--   0 fall      (1000) fall      (1000)       89 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/requires.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)        7 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/top_level.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-05-22 12:27:33.704138 monsda-1.2.6/PKG-INFO
+-rw-r--r--   0 fall      (1000) fall      (1000)     6058 2024-03-04 09:43:25.000000 monsda-1.2.6/README.md
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.686138 monsda-1.2.6/configs/
+-rw-r--r--   0 fall      (1000) fall      (1000)    24464 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/template.json
+-rw-r--r--   0 fall      (1000) fall      (1000)    14131 2024-03-04 09:43:25.000000 monsda-1.2.6/configs/template_base_commented.json
+-rw-r--r--   0 fall      (1000) fall      (1000)     9007 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/template_clean.json
+-rw-r--r--   0 fall      (1000) fall      (1000)    19963 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_exhaustive.json
+-rw-r--r--   0 fall      (1000) fall      (1000)    13787 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_postprocess.json
+-rw-r--r--   0 fall      (1000) fall      (1000)     1171 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_quick.json
+-rw-r--r--   0 fall      (1000) fall      (1000)     8919 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_toolmix.json
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.689138 monsda-1.2.6/envs/
+-rw-r--r--   0 fall      (1000) fall      (1000)     5071 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/LoveSonesonPatro.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      259 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/base.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bbduk.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bbmap.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      210 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bedtools.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      132 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bwa.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      136 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bwa2.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bwameth.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      122 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/ciri2.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      356 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/countreads.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      359 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/countreads_de.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      118 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/cutadapt.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     4345 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/deseq2_DE.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     3328 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/dexseq_DEU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     3200 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/dexseq_DTU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      347 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/diego_DAS.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      120 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/dorado.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     2948 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/drimseq_DTU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/edger_DAS.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     2758 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/edger_DE.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/edger_DEU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.6/envs/fastqc.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      290 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/guppy.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      190 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/hisat2.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      149 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/index.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     3195 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/isoformswitchanalyzer.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      153 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/macs.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      139 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/minimap.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      632 2024-05-22 12:25:05.000000 monsda-1.2.6/envs/monsda.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     6213 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/peaks.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     1525 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/perl.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      129 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/picard.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      142 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/piranha.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.6/envs/qc.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      103 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/salmon.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      131 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/samtools.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      213 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/scyphy.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      151 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/segemehl.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      145 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/segemehl3.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      158 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/sra.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      121 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/star.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      562 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/summary.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      123 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trimgalore.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      235 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trimm.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      161 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trimmomatic.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trnascan.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      228 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/ucsc.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      150 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/umitools.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      106 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/zip.yaml
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.689138 monsda-1.2.6/profile_nextflow/
+-rw-r--r--   0 fall      (1000) fall      (1000)      217 2024-03-27 11:17:58.000000 monsda-1.2.6/profile_nextflow/nextflow.config
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.690138 monsda-1.2.6/profile_snakemake/
+-rw-r--r--   0 fall      (1000) fall      (1000)      344 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/cluster_config.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      277 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/config.yaml
+-rwxr-xr-x   0 fall      (1000) fall      (1000)       51 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-jobscript.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     1826 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-status.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    10397 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-submit-advanced.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     1880 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-submit.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    10495 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm_utils.py
+-rw-r--r--   0 fall      (1000) fall      (1000)     1303 2024-03-28 12:07:30.000000 monsda-1.2.6/pyproject.toml
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.683138 monsda-1.2.6/scripts/
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2882 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/AddStructure.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3647 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/Cluster2tRNA.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    12627 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/CollectBamStat.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    25757 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/CountEnds.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      490 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/CountFastqEnds.pl
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/DAS/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    27615 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/DIEGO.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    12133 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/EDGER.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2108 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    13715 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     4720 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/diego_contrast_files.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/DE/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    15681 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DE/DESEQ2.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    16168 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DE/EDGER.R
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/DEU/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     9059 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DEU/DEXSEQ.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     9938 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DEU/EDGER.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     9611 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DEU/prepare_deu_annotation.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.693138 monsda-1.2.6/scripts/Analysis/DTU/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     7268 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DTU/DEXSEQ.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    14986 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DTU/DRIMSEQ.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3421 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/FindPeaks.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2737 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/GOA.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    14628 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/GenerateTrackDb.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      426 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/GettRNAExpression.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     5106 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/NormalizePeaks.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     5174 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/PlBed2Bedgraph.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2228 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/PreprocessPeaks.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     8094 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/RemoveSoftClip.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    11489 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/RmdCreator.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.693138 monsda-1.2.6/scripts/Analysis/SUMMARY/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      408 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/SUMMARY/header_summary.Rmd
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    13324 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_DEU_table.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    10925 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_DTU_table.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    14005 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_count_table.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    11421 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_salmon_table.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.693138 monsda-1.2.6/scripts/Preprocessing/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      237 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Preprocessing/indexfa.sh
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/scripts/Shells/
+-rw-r--r--   0 fall      (1000) fall      (1000)     1754 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/MergeExpression_Cufflinks.sh
+-rw-r--r--   0 fall      (1000) fall      (1000)     1620 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/MergeExpression_RNAcounter.sh
+-rw-r--r--   0 fall      (1000) fall      (1000)     1517 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/MergeGeneExpression_Cufflinks.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      670 2024-03-25 16:31:46.000000 monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      565 2024-03-15 07:51:51.000000 monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh~
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      460 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/Sam2Bam.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      440 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/Sam2Bed.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      966 2024-04-16 12:14:02.000000 monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      551 2024-03-15 07:50:55.000000 monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh~
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     1628 2024-04-16 12:14:02.000000 monsda-1.2.6/scripts/Shells/UniqueSam_woPicard.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      536 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/printEnds.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      342 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/printFQEnds.sh
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/scripts/Universal/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     8806 2024-03-28 12:04:17.000000 monsda-1.2.6/scripts/Universal/AnnotateBed.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     5046 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/Bed2Bedgraph.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     8118 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/ExtendBed.pl
+-rw-r--r--   0 fall      (1000) fall      (1000)     2303 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/countCCA.pl
+-rw-r--r--   0 fall      (1000) fall      (1000)      710 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/sam2fastq.pl
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/scripts/lib/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    67149 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/Collection.pm
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3227 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/Logger.py
+-rw-r--r--   0 fall      (1000) fall      (1000)        0 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/__init.py__
+-rw-r--r--   0 fall      (1000) fall      (1000)     1099 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/_lib.R
+-rw-r--r--   0 fall      (1000) fall      (1000)      648 2024-05-22 12:27:33.704138 monsda-1.2.6/setup.cfg
+-rw-r--r--   0 fall      (1000) fall      (1000)     3297 2024-03-26 16:29:05.000000 monsda-1.2.6/setup.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/tests/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3454 2024-03-25 16:31:46.000000 monsda-1.2.6/tests/test_functions.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    78254 2024-03-04 09:35:20.000000 monsda-1.2.6/versioneer.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.703138 monsda-1.2.6/workflows/
+-rw-r--r--   0 fall      (1000) fall      (1000)     7289 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/annotatebed.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2023 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bbduk.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2713 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bbduk.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3857 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    14226 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3846 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa2.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3499 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa2.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4232 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwameth.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3360 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwameth.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2050 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ciri2.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1816 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ciri2.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)      507 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/collect.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     9861 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/countreads.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    15432 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/countreads.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2243 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/cutadapt.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2934 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/cutadapt.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7456 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/deseq2_DE.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7927 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/deseq2_DE.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     9193 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DEU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8476 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DEU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     8100 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DTU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    10062 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DTU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     9334 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/diego_DAS.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8157 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/diego_DAS.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1394 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dorado.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1262 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dorado.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     8123 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/drimseq_DTU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    13421 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/drimseq_DTU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7763 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DAS.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7887 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DAS.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7631 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DE.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7806 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DE.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7681 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DEU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7668 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DEU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3191 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     5830 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2040 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4596 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2851 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup_trim.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     5978 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup_trim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)      860 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_raw.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2901 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_raw.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2069 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_trim.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4661 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_trim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/footer.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)       90 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/footer.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1788 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/guppy.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1661 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/guppy.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1609 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/header.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    12190 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/header.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4459 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/hisat2.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4844 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/hisat2.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7366 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/macs.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    14219 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/macs.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2372 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/manipulate_genome.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2359 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/manipulate_genome.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4247 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/mapping.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2698 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/mapping.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3854 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/minimap.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2968 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/minimap.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1022 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/multiqc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    10636 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/multiqc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     5667 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/notify.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    11912 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/peaks.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    21124 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/peaks.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1797 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/picard_dedup.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1250 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/picard_dedup.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)    12177 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/piranha.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    20575 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/piranha.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1150 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/premultiqc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1557 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/premultiqc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     5313 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/salmon.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3679 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/salmon.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4997 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/salmon_trim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)    22666 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/scyphy.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    32938 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/scyphy.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3881 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3098 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4378 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4699 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4613 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3_bisulfite.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3695 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3_bisulfite.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4681 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl_bisulfite.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3848 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl_bisulfite.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1719 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/simulatetrim.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1425 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/simulatetrim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2017 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/sra.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3905 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/sra.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     6531 2024-03-25 16:31:46.000000 monsda-1.2.6/workflows/star.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8723 2024-03-25 16:31:46.000000 monsda-1.2.6/workflows/star.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1190 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/summary.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)      857 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/summary.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2028 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/trimgalore.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3378 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/trimgalore.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7481 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ucsc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8139 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ucsc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4093 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/umitools.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7717 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/umitools.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1656 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/umitools_dedup.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/unlock.smk
```

### Comparing `monsda-1.2.5/LICENSE` & `monsda-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/Configurator.py` & `monsda-1.2.6/MONSDA/Configurator.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/Deprecated.py` & `monsda-1.2.6/MONSDA/Deprecated.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/Logger.py` & `monsda-1.2.6/MONSDA/Logger.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/Params.py` & `monsda-1.2.6/MONSDA/Params.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/RunMONSDA.py` & `monsda-1.2.6/MONSDA/RunMONSDA.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/Utils.py` & `monsda-1.2.6/MONSDA/Utils.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/Workflows.py` & `monsda-1.2.6/MONSDA/Workflows.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA/lib/Collection.groovy` & `monsda-1.2.6/MONSDA/lib/Collection.groovy`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/MONSDA.egg-info/PKG-INFO` & `monsda-1.2.6/MONSDA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MONSDA
-Version: 1.2.5
+Version: 1.2.6
 Summary: MONSDA, Modular Organizer of Nextflow and Snakemake driven hts Data Analysis
 Home-page: https://github.com/jfallmann/MONSDA
 Author: Joerg Fallmann
 Author-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 Maintainer-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `monsda-1.2.5/MONSDA.egg-info/SOURCES.txt` & `monsda-1.2.6/MONSDA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/PKG-INFO` & `monsda-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MONSDA
-Version: 1.2.5
+Version: 1.2.6
 Summary: MONSDA, Modular Organizer of Nextflow and Snakemake driven hts Data Analysis
 Home-page: https://github.com/jfallmann/MONSDA
 Author: Joerg Fallmann
 Author-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 Maintainer-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `monsda-1.2.5/README.md` & `monsda-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/configs/template.json` & `monsda-1.2.6/configs/template.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
     "WORKFLOWS": "", #which workflows do you want to run "MAPPING, QC, DEDUP, TRIMMING, COUNTING, TRACKS, PEAKS, DE, DEU, DAS, DTU, CIRCS"
     "BINS": "", #where to find customscripts used in the workflow !!!ADVANCED USAGE ONLY!!!
     "MAXTHREADS": "20", #maximum number of cores to use, make sure this fits your needs
-    "VERSION": "1.2.5", #needs to be identical to the installed version for reproducibility reasons
+    "VERSION": "1.2.6", #needs to be identical to the installed version for reproducibility reasons
     "SETTINGS": {
         "id": {
             "condition": {
                 "setting": {
                     "SAMPLES": ["Sample_1","Sample_2"] # List of samples you whish to analyze; skip file ending, this names will be used for input/output files of various formats; if paired sequencing make sure the names have _R1/_R2 as identifiers of first/second in pair at the very end of the filename and only list one file without the _R1/_R2 extension, this will be appended automatically
                     "SEQUENCING": "single",  #or paired and stranded (rf,fr) info comma separated
                     "REFERENCE": "GENOMES/Dm6/dm6.fa.gz",  #default Referene Genome fa.gz file
```

### Comparing `monsda-1.2.5/configs/template_base_commented.json` & `monsda-1.2.6/configs/template_base_commented.json`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/configs/template_clean.json` & `monsda-1.2.6/configs/template_clean.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   "WORKFLOWS": "",
   "BINS": "",
   "MAXTHREADS": "20",
-  "VERSION": "1.2.5",
+  "VERSION": "1.2.6",
   "SETTINGS": {
     "id": {
       "condition": {
         "SAMPLES": [
           "rep_1",
           "rep_2"
         ],
```

### Comparing `monsda-1.2.5/configs/tutorial_exhaustive.json` & `monsda-1.2.6/configs/tutorial_exhaustive.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "WORKFLOWS": "FETCH, QC, TRIMMING, MAPPING, DEDUP, TRACKS, PEAKS, DE, DEU, DAS, DTU, COUNTING",
-    "VERSION": "1.2.5",
+    "VERSION": "1.2.6",
     "BINS": "",
     "MAXTHREADS": "16",
     "SETTINGS": {
         "Ecoli": {
             "WT": {
                 "dummylevel": {
                     "SAMPLES": [
```

### Comparing `monsda-1.2.5/configs/tutorial_postprocess.json` & `monsda-1.2.6/configs/tutorial_postprocess.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "WORKFLOWS": "FETCH, QC, TRIMMING, MAPPING, DEDUP, TRACKS, PEAKS, DE, DEU, COUNTING",
-    "VERSION": "1.2.5",
+    "VERSION": "1.2.6",
     "BINS": "",
     "MAXTHREADS": "16",
     "SETTINGS": {
         "Ecoli": {
             "WT": {
                 "dummylevel": {
                     "SAMPLES": [
```

### Comparing `monsda-1.2.5/configs/tutorial_quick.json` & `monsda-1.2.6/configs/tutorial_quick.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'VERSION'": "'1.2.6'"}*

```diff
@@ -37,10 +37,10 @@
             "REFERENCE": "GENOMES/Ecoli/ecoli.fa.gz",
             "SAMPLES": [
                 "SRR16324019"
             ],
             "SEQUENCING": "paired"
         }
     },
-    "VERSION": "1.2.5",
+    "VERSION": "1.2.6",
     "WORKFLOWS": "FETCH,MAPPING"
 }
```

### Comparing `monsda-1.2.5/configs/tutorial_toolmix.json` & `monsda-1.2.6/configs/tutorial_toolmix.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "WORKFLOWS": "FETCH, QC, TRIMMING, MAPPING, DEDUP",
-    "VERSION": "1.2.5",
+    "VERSION": "1.2.6",
     "BINS": "",
     "MAXTHREADS": "16",
     "SETTINGS": {
         "Ecoli": {
             "WT": {   
                 "dummylevel": {       
                     "SAMPLES": [
```

### Comparing `monsda-1.2.5/envs/LoveSonesonPatro.yaml` & `monsda-1.2.6/envs/LoveSonesonPatro.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/deseq2_DE.yaml` & `monsda-1.2.6/envs/deseq2_DE.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/dexseq_DEU.yaml` & `monsda-1.2.6/envs/dexseq_DEU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/dexseq_DTU.yaml` & `monsda-1.2.6/envs/dexseq_DTU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/drimseq_DTU.yaml` & `monsda-1.2.6/envs/drimseq_DTU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/edger_DAS.yaml` & `monsda-1.2.6/envs/edger_DAS.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/edger_DE.yaml` & `monsda-1.2.6/envs/edger_DE.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/edger_DEU.yaml` & `monsda-1.2.6/envs/edger_DEU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/isoformswitchanalyzer.yaml` & `monsda-1.2.6/envs/isoformswitchanalyzer.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/monsda.yaml` & `monsda-1.2.6/envs/monsda.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
   - conda-forge
   - bioconda
   - defaults
 dependencies:
   - biopython=1.83
   - grep >=3.4
   - isort=5.13.2
-  - monsda=1.2.5
+  - monsda=1.2.6
   - natsort=8.4.0
   - nextflow=23.10.1
   - numpy=1.26.4
   - pandas=2.2.1
   - perl=5.34.0
   - pip>=24.0
   - python=3.12.2
   - pyyaml=6.0.1
   - scipy=1.12.0
-  - snakemake=8.10.0
-  - snakemake-executor-plugin-slurm=0.4.2
+  - snakemake=8.11.3
+  - snakemake-executor-plugin-slurm=0.5.0
   - snakemake-executor-plugin-cluster-generic=1.0.9
-  - snakemake-interface-common=1.17.1
-  - snakemake-interface-executor-plugins=9.0.2
+  - snakemake-interface-common=1.17.2
+  - snakemake-interface-executor-plugins=9.1.1
   - snakemake-interface-report-plugins=1.0.0
-  - snakemake-interface-storage-plugins=3.1.1
-  - snakemake-storage-plugin-s3=0.2.10
+  - snakemake-interface-storage-plugins=3.2.2
+  - snakemake-storage-plugin-s3=0.2.11
```

### Comparing `monsda-1.2.5/envs/peaks.yaml` & `monsda-1.2.6/envs/peaks.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/perl.yaml` & `monsda-1.2.6/envs/perl.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/envs/summary.yaml` & `monsda-1.2.6/envs/summary.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/profile_snakemake/slurm-status.py` & `monsda-1.2.6/profile_snakemake/slurm-status.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/profile_snakemake/slurm-submit-advanced.py` & `monsda-1.2.6/profile_snakemake/slurm-submit-advanced.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/profile_snakemake/slurm-submit.py` & `monsda-1.2.6/profile_snakemake/slurm-submit.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/profile_snakemake/slurm_utils.py` & `monsda-1.2.6/profile_snakemake/slurm_utils.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/pyproject.toml` & `monsda-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/AddStructure.py` & `monsda-1.2.6/scripts/Analysis/AddStructure.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/Cluster2tRNA.py` & `monsda-1.2.6/scripts/Analysis/Cluster2tRNA.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/CollectBamStat.py` & `monsda-1.2.6/scripts/Analysis/CollectBamStat.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/CountEnds.py` & `monsda-1.2.6/scripts/Analysis/CountEnds.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DAS/DIEGO.py` & `monsda-1.2.6/scripts/Analysis/DAS/DIEGO.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DAS/EDGER.R` & `monsda-1.2.6/scripts/Analysis/DAS/EDGER.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl` & `monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DAS/FeatureCounts2DIEGO.py` & `monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DAS/diego_contrast_files.py` & `monsda-1.2.6/scripts/Analysis/DAS/diego_contrast_files.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DE/DESEQ2.R` & `monsda-1.2.6/scripts/Analysis/DE/DESEQ2.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DE/EDGER.R` & `monsda-1.2.6/scripts/Analysis/DE/EDGER.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DEU/DEXSEQ.R` & `monsda-1.2.6/scripts/Analysis/DEU/DEXSEQ.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DEU/EDGER.R` & `monsda-1.2.6/scripts/Analysis/DEU/EDGER.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DEU/prepare_deu_annotation.py` & `monsda-1.2.6/scripts/Analysis/DEU/prepare_deu_annotation.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DTU/DEXSEQ.R` & `monsda-1.2.6/scripts/Analysis/DTU/DEXSEQ.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/DTU/DRIMSEQ.R` & `monsda-1.2.6/scripts/Analysis/DTU/DRIMSEQ.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/FindPeaks.pl` & `monsda-1.2.6/scripts/Analysis/FindPeaks.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/GOA.R` & `monsda-1.2.6/scripts/Analysis/GOA.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/GenerateTrackDb.py` & `monsda-1.2.6/scripts/Analysis/GenerateTrackDb.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/NormalizePeaks.pl` & `monsda-1.2.6/scripts/Analysis/NormalizePeaks.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/PlBed2Bedgraph.pl` & `monsda-1.2.6/scripts/Analysis/PlBed2Bedgraph.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/PreprocessPeaks.pl` & `monsda-1.2.6/scripts/Analysis/PreprocessPeaks.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/RemoveSoftClip.py` & `monsda-1.2.6/scripts/Analysis/RemoveSoftClip.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/RmdCreator.py` & `monsda-1.2.6/scripts/Analysis/RmdCreator.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/build_DEU_table.py` & `monsda-1.2.6/scripts/Analysis/build_DEU_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/build_DTU_table.py` & `monsda-1.2.6/scripts/Analysis/build_DTU_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/build_count_table.py` & `monsda-1.2.6/scripts/Analysis/build_count_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Analysis/build_salmon_table.py` & `monsda-1.2.6/scripts/Analysis/build_salmon_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/MergeExpression_Cufflinks.sh` & `monsda-1.2.6/scripts/Shells/MergeExpression_Cufflinks.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/MergeExpression_RNAcounter.sh` & `monsda-1.2.6/scripts/Shells/MergeExpression_RNAcounter.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/MergeGeneExpression_Cufflinks.sh` & `monsda-1.2.6/scripts/Shells/MergeGeneExpression_Cufflinks.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/NonUniqueBam_woPicard.sh` & `monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/NonUniqueBam_woPicard.sh~` & `monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh~`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/UniqueBam_woPicard.sh` & `monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/UniqueBam_woPicard.sh~` & `monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh~`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/UniqueSam_woPicard.sh` & `monsda-1.2.6/scripts/Shells/UniqueSam_woPicard.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Shells/printEnds.sh` & `monsda-1.2.6/scripts/Shells/printEnds.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Universal/AnnotateBed.pl` & `monsda-1.2.6/scripts/Universal/AnnotateBed.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Universal/Bed2Bedgraph.pl` & `monsda-1.2.6/scripts/Universal/Bed2Bedgraph.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Universal/ExtendBed.pl` & `monsda-1.2.6/scripts/Universal/ExtendBed.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Universal/countCCA.pl` & `monsda-1.2.6/scripts/Universal/countCCA.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/Universal/sam2fastq.pl` & `monsda-1.2.6/scripts/Universal/sam2fastq.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/lib/Collection.pm` & `monsda-1.2.6/scripts/lib/Collection.pm`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/lib/Logger.py` & `monsda-1.2.6/scripts/lib/Logger.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/scripts/lib/_lib.R` & `monsda-1.2.6/scripts/lib/_lib.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/setup.cfg` & `monsda-1.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/setup.py` & `monsda-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/tests/test_functions.py` & `monsda-1.2.6/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/versioneer.py` & `monsda-1.2.6/versioneer.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/annotatebed.smk` & `monsda-1.2.6/workflows/annotatebed.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bbduk.nf` & `monsda-1.2.6/workflows/bbduk.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bbduk.smk` & `monsda-1.2.6/workflows/bbduk.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bwa.nf` & `monsda-1.2.6/workflows/bwa.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bwa.smk` & `monsda-1.2.6/workflows/bwa.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bwa2.nf` & `monsda-1.2.6/workflows/bwa2.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bwa2.smk` & `monsda-1.2.6/workflows/bwa2.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bwameth.nf` & `monsda-1.2.6/workflows/bwameth.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/bwameth.smk` & `monsda-1.2.6/workflows/bwameth.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/ciri2.nf` & `monsda-1.2.6/workflows/ciri2.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/ciri2.smk` & `monsda-1.2.6/workflows/ciri2.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/countreads.nf` & `monsda-1.2.6/workflows/countreads.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/countreads.smk` & `monsda-1.2.6/workflows/countreads.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/cutadapt.nf` & `monsda-1.2.6/workflows/cutadapt.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/cutadapt.smk` & `monsda-1.2.6/workflows/cutadapt.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/deseq2_DE.nf` & `monsda-1.2.6/workflows/deseq2_DE.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/deseq2_DE.smk` & `monsda-1.2.6/workflows/deseq2_DE.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/dexseq_DEU.nf` & `monsda-1.2.6/workflows/dexseq_DEU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/dexseq_DEU.smk` & `monsda-1.2.6/workflows/dexseq_DEU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/dexseq_DTU.nf` & `monsda-1.2.6/workflows/dexseq_DTU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/dexseq_DTU.smk` & `monsda-1.2.6/workflows/dexseq_DTU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/diego_DAS.nf` & `monsda-1.2.6/workflows/diego_DAS.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/diego_DAS.smk` & `monsda-1.2.6/workflows/diego_DAS.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/dorado.nf` & `monsda-1.2.6/workflows/dorado.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/dorado.smk` & `monsda-1.2.6/workflows/dorado.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/drimseq_DTU.nf` & `monsda-1.2.6/workflows/drimseq_DTU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/drimseq_DTU.smk` & `monsda-1.2.6/workflows/drimseq_DTU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/edger_DAS.nf` & `monsda-1.2.6/workflows/edger_DAS.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/edger_DAS.smk` & `monsda-1.2.6/workflows/edger_DAS.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/edger_DE.nf` & `monsda-1.2.6/workflows/edger_DE.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/edger_DE.smk` & `monsda-1.2.6/workflows/edger_DE.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/edger_DEU.nf` & `monsda-1.2.6/workflows/edger_DEU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/edger_DEU.smk` & `monsda-1.2.6/workflows/edger_DEU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc.nf` & `monsda-1.2.6/workflows/fastqc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc.smk` & `monsda-1.2.6/workflows/fastqc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_dedup.nf` & `monsda-1.2.6/workflows/fastqc_dedup.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_dedup.smk` & `monsda-1.2.6/workflows/fastqc_dedup.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_dedup_trim.nf` & `monsda-1.2.6/workflows/fastqc_dedup_trim.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_dedup_trim.smk` & `monsda-1.2.6/workflows/fastqc_dedup_trim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_raw.nf` & `monsda-1.2.6/workflows/fastqc_raw.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_raw.smk` & `monsda-1.2.6/workflows/fastqc_raw.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_trim.nf` & `monsda-1.2.6/workflows/fastqc_trim.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/fastqc_trim.smk` & `monsda-1.2.6/workflows/fastqc_trim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/guppy.nf` & `monsda-1.2.6/workflows/guppy.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/guppy.smk` & `monsda-1.2.6/workflows/guppy.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/header.nf` & `monsda-1.2.6/workflows/header.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/header.smk` & `monsda-1.2.6/workflows/header.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/hisat2.nf` & `monsda-1.2.6/workflows/hisat2.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/hisat2.smk` & `monsda-1.2.6/workflows/hisat2.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/macs.nf` & `monsda-1.2.6/workflows/macs.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/macs.smk` & `monsda-1.2.6/workflows/macs.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/manipulate_genome.nf` & `monsda-1.2.6/workflows/manipulate_genome.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/manipulate_genome.smk` & `monsda-1.2.6/workflows/manipulate_genome.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/mapping.nf` & `monsda-1.2.6/workflows/mapping.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/mapping.smk` & `monsda-1.2.6/workflows/mapping.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/minimap.nf` & `monsda-1.2.6/workflows/minimap.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/minimap.smk` & `monsda-1.2.6/workflows/minimap.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/multiqc.nf` & `monsda-1.2.6/workflows/multiqc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/multiqc.smk` & `monsda-1.2.6/workflows/multiqc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/notify.nf` & `monsda-1.2.6/workflows/notify.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/peaks.nf` & `monsda-1.2.6/workflows/peaks.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/peaks.smk` & `monsda-1.2.6/workflows/peaks.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/picard_dedup.nf` & `monsda-1.2.6/workflows/picard_dedup.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/picard_dedup.smk` & `monsda-1.2.6/workflows/picard_dedup.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/piranha.nf` & `monsda-1.2.6/workflows/piranha.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/piranha.smk` & `monsda-1.2.6/workflows/piranha.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/premultiqc.nf` & `monsda-1.2.6/workflows/premultiqc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/premultiqc.smk` & `monsda-1.2.6/workflows/premultiqc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/salmon.nf` & `monsda-1.2.6/workflows/salmon.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/salmon.smk` & `monsda-1.2.6/workflows/salmon.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/salmon_trim.smk` & `monsda-1.2.6/workflows/salmon_trim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/scyphy.nf` & `monsda-1.2.6/workflows/scyphy.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/scyphy.smk` & `monsda-1.2.6/workflows/scyphy.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl.nf` & `monsda-1.2.6/workflows/segemehl.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl.smk` & `monsda-1.2.6/workflows/segemehl.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl3.nf` & `monsda-1.2.6/workflows/segemehl3.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl3.smk` & `monsda-1.2.6/workflows/segemehl3.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl3_bisulfite.nf` & `monsda-1.2.6/workflows/segemehl3_bisulfite.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl3_bisulfite.smk` & `monsda-1.2.6/workflows/segemehl3_bisulfite.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl_bisulfite.nf` & `monsda-1.2.6/workflows/segemehl_bisulfite.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/segemehl_bisulfite.smk` & `monsda-1.2.6/workflows/segemehl_bisulfite.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/simulatetrim.nf` & `monsda-1.2.6/workflows/simulatetrim.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/simulatetrim.smk` & `monsda-1.2.6/workflows/simulatetrim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/sra.nf` & `monsda-1.2.6/workflows/sra.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/sra.smk` & `monsda-1.2.6/workflows/sra.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/star.nf` & `monsda-1.2.6/workflows/star.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/star.smk` & `monsda-1.2.6/workflows/star.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/summary.nf` & `monsda-1.2.6/workflows/summary.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/summary.smk` & `monsda-1.2.6/workflows/summary.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/trimgalore.nf` & `monsda-1.2.6/workflows/trimgalore.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/trimgalore.smk` & `monsda-1.2.6/workflows/trimgalore.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/ucsc.nf` & `monsda-1.2.6/workflows/ucsc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/ucsc.smk` & `monsda-1.2.6/workflows/ucsc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/umitools.nf` & `monsda-1.2.6/workflows/umitools.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/umitools.smk` & `monsda-1.2.6/workflows/umitools.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.5/workflows/umitools_dedup.nf` & `monsda-1.2.6/workflows/umitools_dedup.nf`

 * *Files identical despite different names*

