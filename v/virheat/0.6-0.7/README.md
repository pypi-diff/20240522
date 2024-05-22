# Comparing `tmp/virheat-0.6.tar.gz` & `tmp/virheat-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virheat-0.6.tar", last modified: Fri Nov 17 10:47:13 2023, max compression
+gzip compressed data, was "virheat-0.7.tar", last modified: Wed May 22 07:44:33 2024, max compression
```

## Comparing `virheat-0.6.tar` & `virheat-0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 10:47:13.093362 virheat-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2023-11-17 10:47:13.093362 virheat-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2023-11-17 10:46:57.000000 virheat-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 10:47:13.093362 virheat-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-11-17 10:46:57.000000 virheat-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 10:47:13.093362 virheat-0.6/virheat/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-11-17 10:46:57.000000 virheat-0.6/virheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-17 10:46:57.000000 virheat-0.6/virheat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2023-11-17 10:46:57.000000 virheat-0.6/virheat/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 10:47:13.093362 virheat-0.6/virheat/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 10:46:57.000000 virheat-0.6/virheat/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2023-11-17 10:46:57.000000 virheat-0.6/virheat/scripts/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2023-11-17 10:46:57.000000 virheat-0.6/virheat/scripts/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 10:47:13.093362 virheat-0.6/virheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2023-11-17 10:47:13.000000 virheat-0.6/virheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-17 10:47:13.000000 virheat-0.6/virheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 10:47:13.000000 virheat-0.6/virheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-17 10:47:13.000000 virheat-0.6/virheat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 10:47:12.000000 virheat-0.6/virheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-17 10:47:13.000000 virheat-0.6/virheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-17 10:47:13.000000 virheat-0.6/virheat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:44:33.292784 virheat-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-22 07:44:33.292784 virheat-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-22 07:44:24.000000 virheat-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:44:33.292784 virheat-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-22 07:44:24.000000 virheat-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:44:33.288783 virheat-0.7/virheat/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 07:44:24.000000 virheat-0.7/virheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 07:44:24.000000 virheat-0.7/virheat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-22 07:44:24.000000 virheat-0.7/virheat/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:44:33.292784 virheat-0.7/virheat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:44:24.000000 virheat-0.7/virheat/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-22 07:44:24.000000 virheat-0.7/virheat/scripts/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-22 07:44:24.000000 virheat-0.7/virheat/scripts/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:44:33.292784 virheat-0.7/virheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 07:44:33.000000 virheat-0.7/virheat.egg-info/top_level.txt
```

### Comparing `virheat-0.6/PKG-INFO` & `virheat-0.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,103 @@
-Metadata-Version: 2.1
-Name: virheat
-Version: 0.6
-Summary: virHEAT creates a heatmap from vcf files and maps positions on to a reference genome.
-Home-page: https://github.com/jonas-fuchs/virHEAT
-Author: Dr. Jonas Fuchs
-Author-email: jonas.fuchs@uniklinik-freiburg.de
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: matplotlib<=3.8.0,>=3.5.1
-Requires-Dist: numpy>=1.23.3
-Requires-Dist: pandas>=1.4.4
-
-[![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
-[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
-[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
-[![pypi version](https://static.pepy.tech/badge/virheat)](https://pypi.org/project/virheat/)
-[![CONDA](https://img.shields.io/conda/v/bioconda/virheat?label=conda%20version)](https://anaconda.org/bioconda/virheat)
-[![CONDA](https://img.shields.io/conda/dn/bioconda/virheat?label=conda%20downloads)](https://anaconda.org/bioconda/virheat)
-
-![Logo](./virheat.png)
-
-
-
-**virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
-
-
-
-Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
-
-## SARS-CoV-2 example:
-
-![Example](./example_data/example.png)
-
-## Installation
-
-### via pip (recommened):
-```shell
-pip install virheat
-```
-### via conda:
-```shell
-conda install -c bioconda virheat
-```
-### from this repo:
-```shell
-git clone https://github.com/jonas-fuchs/virHEAT
-cd virHEAT
-pip install -r requirements.txt
-# or
-pip install .
-```
-That was already it. To check if it worked:
-
-```shell
-virheat -v
-```
-You should see the current virHEAT version.
-
-## Usage
-
-```shell
-usage: 	virheat <folder containing vcfs> <output dir> -l or -g [additional arguments]
-
-```
-
-**Arguments:**
-
-```
-positional arguments:
-  input                 folder containing input files and output folder
-
-options:
-  -h, --help            show this help message and exit
-  --name virHEAT_plot.pdf
-                        plot name and file type (pdf, png, svg, jpg). Default: virHEAT_plot.pdf
-  -l None, --genome-length None
-                        length of the genome (needed if gff3 is not provided)
-  -g None, --gff3-path None
-                        path to gff3 (needed if length is not provided)
-  -a [gene ...], --gff3-annotations [gene ...]
-                        annotations to display from gff3 file (standard: gene). Multiple possible.
-  -t 0, --threshold 0   display frequencies above this threshold (0-1)
-  --delete, --no-delete
-                        delete mutations that are present in all samples and their maximum frequency divergence is smaller than 0.5 (default: True)
-  -n None, --delete-n None
-                        do not show mutations that occur n times or less (default: Do not delete)
-  -z start stop, --zoom start stop
-                        restrict the plot to a specific genomic region.                      
-  --sort, --no-sort     sort sample names alphanumerically (default: False)
-  --min-cov 20          display mutations covered at least x time (only if per base cov tsv files are provided)
-  -v, --version         show program's version number and exit
-```
-
-You need to either provide the length of your reference genome or if you want to get the sequence annotation you will need to provide the gff3 file.
-
-Additionally, you can also analyse if mutations are sufficiently covered and display non-covered cells in grey. For that first create a per base coverage tsv files for each bam file with [Qualimap](http://qualimap.conesalab.org/) and provide it in the same folder as the vcf files. Give them the same name as your vcf files.
-
-<a href="https://www.buymeacoffee.com/jofox" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
-
----
-
-**Important disclaimer:**
-*The code is under the GPLv3 licence. The code is WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.*
+[![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
+[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
+[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
+[![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+[![pypi version](https://static.pepy.tech/badge/virheat)](https://pypi.org/project/virheat/)
+[![CONDA](https://img.shields.io/conda/v/bioconda/virheat?label=conda%20version)](https://anaconda.org/bioconda/virheat)
+[![CONDA](https://img.shields.io/conda/dn/bioconda/virheat?label=conda%20downloads)](https://anaconda.org/bioconda/virheat)
+
+![Logo](./virheat.png)
+
+
+
+**virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
+
+
+
+Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
+
+## SARS-CoV-2 example:
+
+![Example](./example_data/example.png)
+
+## SARS-CoV-2 example with additional score tracks `--scores`
+
+![Example_Scores](./example_mave_data/example_scores.png)
+
+## Installation
+
+### via pip (recommened):
+```shell
+pip install virheat
+```
+### via conda:
+```shell
+conda install -c bioconda virheat
+```
+### from this repo:
+```shell
+git clone https://github.com/jonas-fuchs/virHEAT
+cd virHEAT
+pip install -r requirements.txt
+# or
+pip install .
+```
+That was already it. To check if it worked:
+
+```shell
+virheat -v
+```
+You should see the current virHEAT version.
+
+## Usage
+
+```shell
+usage: 	virheat <folder containing vcfs> <output dir> -l or -g [additional arguments]
+
+```
+
+**Arguments:**
+
+```
+positional arguments:
+  input                 folder containing input files and output folder
+
+options:
+  -h, --help            show this help message and exit
+  --name virHEAT_plot.pdf
+                        plot name and file type (pdf, png, svg, jpg). Default: virHEAT_plot.pdf
+  -l None, --genome-length None
+                        length of the genome (needed if gff3 is not provided)
+  -g None, --gff3-path None
+                        path to gff3 (needed if length is not provided)
+  -a [gene ...], --gff3-annotations [gene ...]
+                        annotations to display from gff3 file (standard: gene). Multiple possible.
+  -t 0, --threshold 0   display frequencies above this threshold (0-1)
+  --delete, --no-delete
+                        delete mutations that are present in all samples and their maximum frequency divergence is smaller than 0.5 (default: True)
+  -n None, --delete-n None
+                        do not show mutations that occur n times or less (default: Do not delete)
+  -z start stop, --zoom start stop
+                        restrict the plot to a specific genomic region.                      
+  --sort, --no-sort     sort sample names alphanumerically (default: False)
+  --min-cov 20          display mutations covered at least x time (only if per base cov tsv files are provided)
+  -s scores_file pos_col score_col score_name, --scores scores_file pos_col score_col score_name
+                        specify scores to be added to the plot by providing a CSV file containing scores, along with its column for amino-acid positions, its column for scores, and descriptive score names (e.g., expression, binding, antibody escape, etc.).
+                        This option can be used multiple times to include multiple sets of scores.
+  -v, --version         show program's version number and exit
+```
+
+You need to either provide the length of your reference genome or if you want to get the sequence annotation you will need to provide the gff3 file.
+
+Additionally, you can also analyse if mutations are sufficiently covered and display non-covered cells in grey. For that first create a per base coverage tsv files for each bam file with [Qualimap](http://qualimap.conesalab.org/) and provide it in the same folder as the vcf files. Give them the same name as your vcf files.
+
+Moreover, there is an option to include visualizations of additional scores (e.g., MAVE scores for binding affinity, expression level, antibody escape, etc.) mapped to mutations on the heatmap. To utilize this feature, use the -s or --scores 
+argument, and provide the following arguments: 1) path to the CSV file containing scores; 2) the name of the column in this file containing mutation positions in classic notation (e.g., T430Y); 3) the name of the column in this file containing the 
+scores themselves; 4) a descriptive score name that will be used as labels in the plot. Multiple score sets can be included simultaneously by repeating the -s or --scores option with different arguments. For example input and possible output data,
+please refer to the files located in the  [example_data/example_mave_data](example_mave_data) folder.
+
+---
+
+**Important disclaimer:**
+*The code is under the GPLv3 licence. The code is WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.*
```

### Comparing `virheat-0.6/setup.py` & `virheat-0.7/setup.py`

 * *Files identical despite different names*

### Comparing `virheat-0.6/virheat/command.py` & `virheat-0.7/virheat/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -105,14 +105,21 @@
         "--min-cov",
         type=int,
         metavar="20",
         default=20,
         help="display mutations covered at least x time (only if per base cov tsv files are provided)"
     )
     parser.add_argument(
+        "-s", "--scores",
+        metavar=('scores_file', 'pos_col', 'score_col', 'score_name'),
+        nargs=4,
+        action='append',
+        help="specify scores to be added to the plot by providing a CSV file containing scores, along with its column for amino-acid positions, its column for scores, and descriptive score names (e.g., expression, binding, antibody escape, etc.). This option can be used multiple times to include multiple sets of scores."
+    )
+    parser.add_argument(
         "-v",
         "--version",
         action='version',
         version=f"virheat {__version__}"
     )
     if len(sysargs) < 1:
         parser.print_help()
@@ -131,58 +138,74 @@
 
     # get vcf files and sort
     vcf_files = data_prep.get_files(args.input[0], "vcf")
     if args.sort:
         vcf_files = sorted(vcf_files, key=lambda x: data_prep.get_digit_and_alpha(os.path.basename(x)))
 
     # extract vcf info
-    reference_name, frequency_lists, unique_mutations, file_names = data_prep.extract_vcf_data(vcf_files, threshold=args.threshold)
+    n_scores = 0
+    if not vcf_files:
+        sys.exit("\033[31m\033[1mERROR:\033[0m No VCF files provided")
+    else:
+        if args.scores:
+            reference_name, frequency_lists, unique_mutations, file_names = data_prep.extract_vcf_data(vcf_files, threshold=args.threshold, scores=True)
+            n_scores = len(args.scores)
+        else:
+            reference_name, frequency_lists, unique_mutations, file_names = data_prep.extract_vcf_data(vcf_files, threshold=args.threshold)
+
     if args.zoom:
         unique_mutations = data_prep.zoom_to_genomic_regions(unique_mutations, args.zoom)
     frequency_array = data_prep.create_freq_array(unique_mutations, frequency_lists)
 
     # user specified delete options (removes mutations based on various rationales)
     if args.delete:
         frequency_array = data_prep.delete_common_mutations(frequency_array, unique_mutations)
     if args.delete_n is not None:
         frequency_array = data_prep.delete_n_mutations(frequency_array, unique_mutations, args.delete_n)
 
-    # annotate low coverage if per base coveage from qualimap was provided
+    # annotate low coverage if per base coverage from qualimap was provided
     data_prep.annotate_non_covered_regions(args.input[0], args.min_cov, frequency_array, file_names, unique_mutations)
 
     # define relative locations of all items in the plot
     n_samples, n_mutations = len(frequency_array), len(frequency_array[0])
     if n_mutations == 0:
         sys.exit("\033[31m\033[1mERROR:\033[0m Frequency array seems to be empty. There is nothing to plot.")
     if n_samples < 4:
         genome_y_location = 2
     else:
         genome_y_location = math.log2(n_samples)
 
-    # gff3 data extraction
+    # gff3 data extraction and define y coordinates
     if args.gff3_path is not None and args.genome_length is not None:
         sys.exit("\033[31m\033[1mERROR:\033[0m Do not provide the -g and -l argument simultaneously!")
     elif args.gff3_path is not None:
         gff3_info, gff3_ref_name = data_prep.parse_gff3(args.gff3_path)
         # issue a warning if #CHROM and gff3 do not match
         if gff3_ref_name not in reference_name and reference_name not in gff3_ref_name:
             print("\033[31m\033[1mWARNING:\033[0m gff3 reference does not match the vcf reference!")
         genome_end = data_prep.get_genome_end(gff3_info)
         genes_with_mutations, n_tracks = data_prep.create_track_dict(unique_mutations, gff3_info, args.gff3_annotations)
-        # define space for the genome vis tracks
-        min_y_location = genome_y_location + genome_y_location/2 * (n_tracks+1)
     elif args.genome_length is not None:
         genome_end = args.genome_length
-        min_y_location = genome_y_location
+        n_tracks = 0
     else:
         sys.exit("\033[31m\033[1mERROR:\033[0m Provide either a gff3 file (-g) or the length (-l) of the genome which you used for mapping")
 
+    # define min y coordinate
+    if n_tracks != 0 or n_scores != 0:
+        min_y_location = genome_y_location + genome_y_location / 2 * (n_tracks + n_scores + 2)
+    else:
+        min_y_location = genome_y_location
+
     # define size of the plot
     y_size = n_mutations*0.4
-    x_size = y_size*(n_samples+min_y_location)/n_mutations
+    if args.scores:
+        x_size = y_size * (n_samples + min_y_location + n_scores) / n_mutations
+    else:
+        x_size = y_size*(n_samples + min_y_location)/n_mutations
     x_size = x_size-x_size*0.15  # compensate of heatmap annotation
 
     # ini the fig
     fig, ax = plt.subplots(figsize=[y_size, x_size])
 
     # define boundaries for the plot
     if args.zoom:
@@ -191,31 +214,41 @@
         if args.zoom[0] < 0:
             start = 0
         if args.zoom[1] > genome_end:
             stop = genome_end
     else:
         start, stop = 0, genome_end
 
-    # plot all elements
+    # plot all common elements
     cmap = cm.gist_heat_r
     cmap.set_bad('silver', 1.)
     cmap_cells = cm.ScalarMappable(norm=colors.Normalize(0, 1), cmap=cmap)
     plotting.create_heatmap(ax, frequency_array, cmap_cells)
     mutation_set = plotting.create_genome_vis(ax, genome_y_location, n_mutations, unique_mutations, start, stop)
+    plotting.create_axis(ax, n_mutations, min_y_location, n_samples, file_names, start, stop, genome_y_location,
+                         unique_mutations, reference_name)
+    plotting.create_mutation_legend(mutation_set, min_y_location, n_samples, n_scores)
+    plotting.create_colorbar(args.threshold, cmap_cells, min_y_location, n_samples, ax)
+    # plot gene track
     if args.gff3_path is not None:
         if genes_with_mutations:
             # distinct colors for the genes
             cmap_genes = plt.get_cmap('tab20', len(genes_with_mutations))
             colors_genes = [cmap_genes(i) for i in range(len(genes_with_mutations))]
             # plot gene track
-            plotting.create_gene_vis(ax, genes_with_mutations, n_mutations, y_size, n_tracks, start, stop, min_y_location, genome_y_location, colors_genes)
-    plotting.create_axis(ax, n_mutations, min_y_location, n_samples, file_names, start, stop, genome_y_location, unique_mutations, reference_name)
-    plotting.create_colorbar(args.threshold, cmap_cells, min_y_location, n_samples, ax)
-    plotting.create_mutation_legend(mutation_set, min_y_location, n_samples)
-
+            plotting.create_gene_vis(ax, genes_with_mutations, n_mutations, y_size, n_tracks, start, stop, min_y_location, genome_y_location, colors_genes, n_scores)
+    # plot scores as track below the gene/genome track
+    if args.scores:
+        score_count = 1
+        for score_params in args.scores:
+            scores_file, pos_col, score_col, score_name = score_params
+            unique_scores = data_prep.extract_scores(unique_mutations, scores_file, pos_col, score_col)
+            track_created = plotting.create_scores_vis(ax, genome_y_location, n_mutations, n_tracks, unique_scores, start, stop, score_count, score_name)
+            if track_created:  # only creates a track if it finds mutations to annotate
+                score_count += 1
     # create output folder
     if not os.path.exists(args.input[1]):
         os.makedirs(args.input[1])
 
     # save fig
     fig.savefig(os.path.join(args.input[1], args.name), bbox_inches="tight")
```

### Comparing `virheat-0.6/virheat/scripts/data_prep.py` & `virheat-0.7/virheat/scripts/data_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,19 @@
     """
     parse vcf files to dictionary
     """
     vcf_dict = {}
 
     # get header and values
     with open(vcf_file, "r") as f:
-        header = [l.split("\t") for l in f if l.startswith('#CHROM')][0]
+        header_lines = [l.split("\t") for l in f if l.startswith('#CHROM')]
+        if not header_lines:
+            print(f"\033[31m\033[1mWARNING:\033[0m {vcf_file} does not contain a '#CHROM' header!")
+            return {}
+        header = header_lines[0]
     # get each line as frequency_lists
     with open(vcf_file, "r") as f:
         lines = [l.split("\t") for l in f if not l.startswith('#')]
     # check if vcf is empty
     if not lines:
         print(f"\033[31m\033[1mWARNING:\033[0m {vcf_file} is empty!")
     # get standard headers as keys
@@ -96,15 +100,15 @@
         # append none for ech none visited key
         for key in [k for k in vcf_dict.keys() if k not in visited_keys]:
             vcf_dict[key].append(None)
 
     return vcf_dict
 
 
-def extract_vcf_data(vcf_files, threshold=0):
+def extract_vcf_data(vcf_files, threshold=0, scores=False):
     """
     extract relevant vcf data
     """
 
     file_names = []
     frequency_lists = []
 
@@ -112,26 +116,59 @@
         file_names.append(os.path.splitext(os.path.basename(file))[0])
         vcf_dict = read_vcf(file)
         frequency_list = []
         # write all mutation info in a '_' sep string
         for idx in range(0, len(vcf_dict["#CHROM"])):
             if not vcf_dict["AF"][idx] >= threshold:
                 continue
-            frequency_list.append(
-                (f"{vcf_dict['POS'][idx]}_{vcf_dict['REF'][idx]}_{vcf_dict['ALT'][idx]}_{vcf_dict['MUT_TYPE_'][idx]}", vcf_dict['AF'][idx])
-            )
+            if scores:
+                if vcf_dict['EFF'][idx] is not None:
+                    aa_change = vcf_dict['EFF'][idx].split('|')[3]  # extract amino acid changes if provided
+                else:
+                    aa_change = '-'
+                frequency_list.append(
+                    (f"{vcf_dict['POS'][idx]}_{vcf_dict['REF'][idx]}_{vcf_dict['ALT'][idx]}_{vcf_dict['MUT_TYPE_'][idx]}_{aa_change}", vcf_dict['AF'][idx])
+                )
+            else:
+                frequency_list.append(
+                    (f"{vcf_dict['POS'][idx]}_{vcf_dict['REF'][idx]}_{vcf_dict['ALT'][idx]}_{vcf_dict['MUT_TYPE_'][idx]}", vcf_dict['AF'][idx])
+                )
+
         frequency_lists.append(frequency_list)
     # sort by mutation index
     unique_mutations = sorted(
         {x[0] for li in frequency_lists for x in li}, key=lambda x: int(x.split("_")[0])
     )
 
     return vcf_dict["#CHROM"][0], frequency_lists, unique_mutations, file_names
 
 
+def extract_scores(unique_mutations, scores_file, aa_pos_col, score_col):
+    """
+    Extract scores from scores_file which corresponding value from aa_pos_col is equal to unique_aa_mutations
+    """
+    scores_df = pd.read_csv(scores_file)
+
+    # create a dictionary to store the scores for each mutation
+    mutation_scores = {}
+    for idx, row in scores_df.iterrows():
+        mutation_scores[row[aa_pos_col]] = row[score_col]
+
+    unique_scores = []
+    for mutation in unique_mutations:
+        aa_mut = mutation.split('_')[4]
+        if aa_mut in mutation_scores:
+            score = mutation_scores[aa_mut]
+            unique_scores.append(f"{mutation}_{score}")
+        else:
+            unique_scores.append(f"{mutation}_nan")
+
+    return unique_scores
+
+
 def create_freq_array(unique_mutations, frequency_lists):
     """
     create an np array of the mutation frequencies
     """
 
     frequency_array = []
 
@@ -191,14 +228,15 @@
             mut_to_del.append(idx)
 
     for idx in sorted(mut_to_del, reverse=True):
         del unique_mutations[idx]
 
     return np.delete(frequency_array, mut_to_del, axis=1)
 
+
 def delete_n_mutations(frequency_array, unique_mutations, min_mut):
     """
     delete mutations that are not present in more than n samples
     """
     mut_to_del = []
 
     for idx in range(0, len(frequency_array[0])):
@@ -224,14 +262,15 @@
 
     for mutation in unique_mutations:
         if start_stop[0] <= int(mutation.split("_")[0]) <= start_stop[1]:
             zoomed_unique.append(mutation)
 
     return zoomed_unique
 
+
 def parse_gff3(file):
     """
     parse gff3 to dictionary
     """
 
     gff3_dict = {}
```

