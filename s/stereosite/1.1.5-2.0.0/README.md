# Comparing `tmp/stereosite-1.1.5.tar.gz` & `tmp/stereosite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stereosite-1.1.5.tar", last modified: Tue Mar 12 07:46:06 2024, max compression
+gzip compressed data, was "stereosite-2.0.0.tar", last modified: Wed May 22 08:29:01 2024, max compression
```

## Comparing `stereosite-1.1.5.tar` & `stereosite-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.150841 stereosite-1.1.5/
--rw-rw-rw-   0        0        0    35823 2024-01-09 07:00:02.000000 stereosite-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     1911 2024-03-12 07:46:06.149835 stereosite-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2024-01-09 07:00:02.000000 stereosite-1.1.5/PYPI.rst
--rw-rw-rw-   0        0        0     5093 2024-01-09 07:00:02.000000 stereosite-1.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-12 07:46:06.150841 stereosite-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      833 2024-03-12 07:45:59.000000 stereosite-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.109252 stereosite-1.1.5/stereosite/
--rw-rw-rw-   0        0        0        0 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.117255 stereosite-1.1.5/stereosite/cn/
--rw-rw-rw-   0        0        0       45 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/cn/__init__.py
--rw-rw-rw-   0        0        0     8402 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/cn/cellneighbor.py
--rw-rw-rw-   0        0        0    17464 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/cn/deconvolution.py
--rw-rw-rw-   0        0        0     2800 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/degene.py
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.139838 stereosite-1.1.5/stereosite/plot/
--rw-rw-rw-   0        0        0       44 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/__init__.py
--rw-rw-rw-   0        0        0     2475 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/cellneighbor.py
--rw-rw-rw-   0        0        0     8344 2024-03-07 03:16:09.000000 stereosite-1.1.5/stereosite/plot/intensity.py
--rw-rw-rw-   0        0        0     3822 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/mask.py
--rw-rw-rw-   0        0        0     7195 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/net.py
--rw-rw-rw-   0        0        0    19611 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/sankey.py
--rw-rw-rw-   0        0        0    18465 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/scii.py
--rw-rw-rw-   0        0        0    12339 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/scii_circos.py
--rw-rw-rw-   0        0        0     4964 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/plot/scii_net.py
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.145837 stereosite-1.1.5/stereosite/ppi/
--rw-rw-rw-   0        0        0       50 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/ppi/__init__.py
--rw-rw-rw-   0        0        0     4819 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/ppi/ppi_analysis.py
--rw-rw-rw-   0        0        0     4354 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/ppi/query.py
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.148802 stereosite-1.1.5/stereosite/read/
--rw-rw-rw-   0        0        0       46 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/read/__init__.py
--rw-rw-rw-   0        0        0     6784 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/read/gem.py
--rw-rw-rw-   0        0        0    24385 2024-03-11 02:21:05.000000 stereosite-1.1.5/stereosite/scii.py
--rw-rw-rw-   0        0        0     1214 2024-01-09 07:00:02.000000 stereosite-1.1.5/stereosite/tf_infer.py
-drwxrwxrwx   0        0        0        0 2024-03-12 07:46:06.148802 stereosite-1.1.5/stereosite.egg-info/
--rw-rw-rw-   0        0        0     1911 2024-03-12 07:46:05.000000 stereosite-1.1.5/stereosite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      756 2024-03-12 07:46:05.000000 stereosite-1.1.5/stereosite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 07:46:05.000000 stereosite-1.1.5/stereosite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-03-12 07:46:05.000000 stereosite-1.1.5/stereosite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-12 07:46:05.000000 stereosite-1.1.5/stereosite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.657348 stereosite-2.0.0/
+-rw-rw-rw-   0        0        0    35823 2024-01-09 07:00:02.000000 stereosite-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2111 2024-05-22 08:29:01.656348 stereosite-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1404 2024-01-09 07:00:02.000000 stereosite-2.0.0/PYPI.rst
+-rw-rw-rw-   0        0        0     5093 2024-01-09 07:00:02.000000 stereosite-2.0.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:29:01.657348 stereosite-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2024-05-22 08:26:55.000000 stereosite-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.599610 stereosite-2.0.0/stereosite/
+-rw-rw-rw-   0        0        0        0 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.607612 stereosite-2.0.0/stereosite/cn/
+-rw-rw-rw-   0        0        0       45 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/cn/__init__.py
+-rw-rw-rw-   0        0        0     8402 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/cn/cellneighbor.py
+-rw-rw-rw-   0        0        0    17464 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/cn/deconvolution.py
+-rw-rw-rw-   0        0        0     2800 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/degene.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.647348 stereosite-2.0.0/stereosite/plot/
+-rw-rw-rw-   0        0        0       44 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/plot/__init__.py
+-rw-rw-rw-   0        0        0     2475 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/plot/cellneighbor.py
+-rw-rw-rw-   0        0        0     8344 2024-03-07 03:16:09.000000 stereosite-2.0.0/stereosite/plot/intensity.py
+-rw-rw-rw-   0        0        0     3822 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/plot/mask.py
+-rw-rw-rw-   0        0        0     7195 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/plot/net.py
+-rw-rw-rw-   0        0        0    19611 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/plot/sankey.py
+-rw-rw-rw-   0        0        0    18465 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/plot/scii.py
+-rw-rw-rw-   0        0        0    12782 2024-05-17 09:01:58.000000 stereosite-2.0.0/stereosite/plot/scii_circos.py
+-rw-rw-rw-   0        0        0     5376 2024-05-17 09:02:48.000000 stereosite-2.0.0/stereosite/plot/scii_net.py
+-rw-rw-rw-   0        0        0     2905 2024-05-22 07:23:15.000000 stereosite-2.0.0/stereosite/plot/scii_tensor.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.652348 stereosite-2.0.0/stereosite/ppi/
+-rw-rw-rw-   0        0        0       50 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/ppi/__init__.py
+-rw-rw-rw-   0        0        0     4819 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/ppi/ppi_analysis.py
+-rw-rw-rw-   0        0        0     4354 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/ppi/query.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.654348 stereosite-2.0.0/stereosite/read/
+-rw-rw-rw-   0        0        0       46 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/read/__init__.py
+-rw-rw-rw-   0        0        0     6784 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/read/gem.py
+-rw-rw-rw-   0        0        0    24385 2024-03-11 02:21:05.000000 stereosite-2.0.0/stereosite/scii.py
+-rw-rw-rw-   0        0        0    28675 2024-05-22 08:25:26.000000 stereosite-2.0.0/stereosite/scii_tensor.py
+-rw-rw-rw-   0        0        0     1214 2024-01-09 07:00:02.000000 stereosite-2.0.0/stereosite/tf_infer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:29:01.655350 stereosite-2.0.0/stereosite.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-22 08:29:01.000000 stereosite-2.0.0/stereosite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2024-05-22 08:29:01.000000 stereosite-2.0.0/stereosite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:29:01.000000 stereosite-2.0.0/stereosite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2024-05-22 08:29:01.000000 stereosite-2.0.0/stereosite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 08:29:01.000000 stereosite-2.0.0/stereosite.egg-info/top_level.txt
```

### Comparing `stereosite-1.1.5/LICENSE` & `stereosite-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/PKG-INFO` & `stereosite-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: stereosite
-Version: 1.1.5
+Version: 2.0.0
 Summary: Analysis spatial transcriptomics data
 Home-page: https://github.com/STOmics/StereoSiTE
 Author: LiuXing
 Author-email: liuxing2@genomics.cn
 License: GPL-3 License
 Keywords: spatial cell interaction intensity
 Platform: any
 License-File: LICENSE
 Requires-Dist: anndata>=0.8.0
 Requires-Dist: scanpy>=1.9.1
 Requires-Dist: squidpy>=1.1.2
 Requires-Dist: decoupler>=1.4.0
 Requires-Dist: pydeseq2>=0.3.6
 Requires-Dist: networkx>=3.1
+Requires-Dist: tensorly>=0.8.1
+Requires-Dist: scikit-learn>=1.2.1
+Requires-Dist: torch>=1.11.0
+Requires-Dist: igraph>=0.10.4
+Requires-Dist: pycirclize>=1.1.0
+Requires-Dist: cell2location==0.1.3
 
 StereoSiTE - Spatial Transcriptome Analysis in Python
 ======================================================
 
 **StereoSiTE** is a package for the analysis and visualization of spatial transcriptome data.
 It builds on top of `anndata`_, `scanpy`_ and `squidpy`_, from which it inherits modularity and scalability.
 It provides analysis tools to dissect cellular neighborhood based on cell composition and quantitatively define cell-cell communication in spatial.
```

### Comparing `stereosite-1.1.5/PYPI.rst` & `stereosite-2.0.0/PYPI.rst`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/README.rst` & `stereosite-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/cn/cellneighbor.py` & `stereosite-2.0.0/stereosite/cn/cellneighbor.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/cn/deconvolution.py` & `stereosite-2.0.0/stereosite/cn/deconvolution.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/degene.py` & `stereosite-2.0.0/stereosite/degene.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/cellneighbor.py` & `stereosite-2.0.0/stereosite/plot/cellneighbor.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/intensity.py` & `stereosite-2.0.0/stereosite/plot/intensity.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/mask.py` & `stereosite-2.0.0/stereosite/plot/mask.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/net.py` & `stereosite-2.0.0/stereosite/plot/net.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/sankey.py` & `stereosite-2.0.0/stereosite/plot/sankey.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/scii.py` & `stereosite-2.0.0/stereosite/plot/scii.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/plot/scii_circos.py` & `stereosite-2.0.0/stereosite/plot/scii_circos.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,22 +63,24 @@
     for c1 in cells:
         for c2 in cells:
             cell_pairs[f"{c1}{separator}{c2}"] = (c1, c2)
     return cell_pairs
 
 def interaction_matrix_process(interaction_matrix:pd.DataFrame,
                                cells:list,
-                               separator:str="_"
+                               separator:str="-",
+                               cell_lr_separator:str="|",
                                ) -> tuple:
     '''
     Input
         interaction_matrix: DataFrame. Matrix contains interesting interaction in the TME region of interest, index represents cell-cell pairs
                             while column represents ligand-receptor pairs
         cells: List of cell type names, which will be used to separate cells of the cell pair.
-        separator: Separator used to combine sender and receiver cells into a cell pair.
+        separator: Separator used to combine ligand with receptor genes into LR pairs.
+        cell_lr_separator: Separatpr used to combine cells with LR genes.
     Return
         (sectors:dict, links:list, genes:set)
         sectors: The dictionary containing all vertices and their weight. {sender-ligand: value, receiver-receptor: value, ...}
         links: List containing all links between sectors. [[sender-ligand, receiver-receptor, value], ...]
         genes: Set contains names of all genes.
     '''
     #Normalize the value into 0~100
@@ -95,95 +97,97 @@
     links = []
     for index, row in norm_mt.iterrows():
         sender, receiver = cell_pairs[index]
         for LR, value in row.items():
             if value == 0:
                 continue
             ligand, receptor = LR.split(separator, 1)
-            v1 = f"{sender}-{ligand}"
-            v2 = f"{receiver}-{receptor}"
+            v1 = f"{sender}{cell_lr_separator}{ligand}"
+            v2 = f"{receiver}{cell_lr_separator}{receptor}"
             if sender not in sectors1.keys():
                 sectors1[sender] = defaultdict(int)
             if receiver not in sectors2.keys():
                 sectors2[receiver] = defaultdict(int)
             sectors1[sender][ligand] += value
             sectors2[receiver][receptor] += value
             genes.add(ligand)
             genes.add(receptor)
             links.append([v1, v2, value])
 
     sectors = defaultdict(int)
     for cell in cells:
         if cell in sectors1.keys():
             for ligand, value in sectors1[cell].items():
-                sectors[f"{cell}-{ligand}"] += value
+                sectors[f"{cell}{cell_lr_separator}{ligand}"] += value
         if cell in sectors2.keys():
             for receptor, value in sectors2[cell].items():
-                sectors[f"{cell}-{receptor}"] += value
+                sectors[f"{cell}{cell_lr_separator}{receptor}"] += value
     return sectors, links, genes
 
 def cells_lr_circos(interaction_matrix:pd.DataFrame,
               cells:list,
+              cell_lr_separator:str="|",
               save:str=None,
               ):
     '''
     Input:
         interaction_matrix: The dataframe that contains the spatial cell interaction intensity(SCII) values of each interaction.
                             The index represents cell_cell pairs and the column represents ligand_receptor pairs.
         cells: The list contains the names of all cell types. This will be used to separate the sender and receiver cells that were 
                 combined to create index names for the interaction_matrix.
+        cell_lr_separator: Separator used to combine cells with LR genes.
         save: File name of the figure that will be saved.
     Return:    
         None
     '''
 
-    sectors, links, genes = interaction_matrix_process(interaction_matrix, cells)
+    sectors, links, genes = interaction_matrix_process(interaction_matrix, cells, cell_lr_separator=cell_lr_separator)
 
     cell_groups = defaultdict(list)
     for key in sectors.keys():
-        cell, gene = key.split("-", 1)
+        cell, gene = key.split(cell_lr_separator, 1)
         cell_groups[cell].append(key)
     group_sizes = [len(value) for key, value in cell_groups.items()]
 
     #Generate the color palette for cells, genes and links
     cmap1 = plt.get_cmap('tab20b')
     cmap2 = plt.get_cmap('tab20c')
     
     cell_color_palette = plt.get_cmap("Set3", len(cells)).colors
     cell_colors = dict(zip(cells, cell_color_palette))
 
     new_cmap = ListedColormap(cmap1.colors + cmap2.colors, N=len(genes))
     gene_color_palette = new_cmap.colors
     gene_colors = dict(zip(sorted(list(genes)), gene_color_palette))
 
-    lr_links = sorted(list(set([(x[0].split("-", 1)[1], x[1].split("-", 1)[1]) for x in links])))
+    lr_links = sorted(list(set([(x[0].split(cell_lr_separator, 1)[1], x[1].split(cell_lr_separator, 1)[1]) for x in links])))
     new_cmap = ListedColormap(cmap1.colors + cmap2.colors, N=len(lr_links))
     link_color_palette = new_cmap.colors
     link_colors = dict(zip(lr_links, link_color_palette))
 
     spaces = calc_group_spaces(group_sizes, space_bw_group=10, space_in_group=1)
     circos = Circos(sectors, space=spaces)
 
     # Plot sector track
     #ColorCycler.set_cmap("Set3")
     for sector in circos.sectors:
         track = sector.add_track(r_lim=(90, 95))
-        track.axis(fc=gene_colors[sector.name.split("-", 1)[1]])
+        track.axis(fc=gene_colors[sector.name.split(cell_lr_separator, 1)[1]])
         #track.text(sector.name.split("-", 1)[1], fontsize=5, r=92, orientation="vertical")
 
     #ColorCycler.set_cmap("tab10")
     for cell, group in cell_groups.items():
         group_deg_lim = circos.get_group_sectors_deg_lim(group)
         circos.rect(r_lim=(100, 103), deg_lim=group_deg_lim, fc=cell_colors[cell], ec="black", lw=0.5)
         group_center_deg = sum(group_deg_lim)/2
         circos.text(cell, r=106, deg=group_center_deg, adjust_rotation=True, fontsize=8)
 
     #Plot links
     for sender, receiver, value in links:
-        ligand, receptor = sender.split("-", 1)[1], receiver.split("-", 1)[1]
+        ligand, receptor = sender.split(cell_lr_separator, 1)[1], receiver.split(cell_lr_separator, 1)[1]
         circos.link((sender, sectors[sender]-value, sectors[sender]), (receiver, sectors[receiver]-value, sectors[receiver]), color=link_colors[(ligand, receptor)], direction=1)
         sectors[sender] -= value
         sectors[receiver] -= value
         
     fig = circos.plotfig()
     #Plot legend
     rect_handles = []
```

### Comparing `stereosite-1.1.5/stereosite/plot/scii_net.py` & `stereosite-2.0.0/stereosite/plot/scii_net.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,76 +4,80 @@
 import matplotlib.pyplot as plt
 import igraph as ig
 from igraph import Graph
 from .scii_circos import interaction_matrix_process
 
 def lr_link_graph_generate(interaction_matrix:pd.DataFrame,
                   cells:list,
-                  separator:str="_",
+                  separator:str="-",
+                  cell_lr_separator="|",
                   reducer:int=3,
                   ) -> Graph:
     '''
     Input:
         interaction_matrix: DataFrame. Matrix contains interesting interaction in the TME region of interest, index represents cell-cell pairs
                             while column represents ligand-receptor pairs
         cells: List of cell type names, which will be used to separate cells of the cell pair.
-        separator: Separator used to combine sender and receiver cells into a cell pair.
+        separator: Separator used to combine ligand with receptor genes into LR pairs.
+        cell_lr_separator: Separator used to combine cells with LR genes.
         reducer: The size of a vertex = weight of the vertex/reducer
     Return:
         g: Graph containing all vertices(ligand or receptor) and their links information.
         
     '''
     #generate color palette for cells and links
     cell_palette = 'Set3'
     cell_colors = dict(zip(cells, [tuple(x[0:3]) for x in plt.get_cmap(cell_palette, len(cells)).colors]))
 
     #transfer matrix into igraph
-    sectors, links, genes = interaction_matrix_process(interaction_matrix, cells, separator=separator)
+    sectors, links, genes = interaction_matrix_process(interaction_matrix, cells, separator=separator, cell_lr_separator=cell_lr_separator)
     vertices = list(sectors.keys())
-    vertices_color = [cell_colors[x.split("-")[0]] for x in vertices]
+    vertices_color = [cell_colors[x.split(cell_lr_separator)[0]] for x in vertices]
     vertices_dict = dict(zip(vertices, range(len(vertices))))
     edges_index = [(vertices_dict[x[0]], vertices_dict[x[1]]) for x in links]
-    lr_links = set([(x[0].split("-")[1], x[1].split("-")[1]) for x in links])
+    lr_links = set([(x[0].split(cell_lr_separator)[1], x[1].split(cell_lr_separator)[1]) for x in links])
     lr_palette = "tab20"
     link_color_palette = [tuple(x[0:3]) for x in plt.get_cmap(lr_palette, len(lr_links)).colors]
     link_colors = dict(zip(lr_links, link_color_palette))
-    edges_color = [link_colors[(x[0].split("-")[1], x[1].split("-")[1])] for x in links]
+    edges_color = [link_colors[(x[0].split(cell_lr_separator)[1], x[1].split(cell_lr_separator)[1])] for x in links]
 
     g = Graph(n=len(vertices), edges=edges_index, directed=True)
     g.vs['name'] = vertices
-    g.vs['label'] = [x.split("-", 1)[1] for x in vertices]
+    g.vs['label'] = [x.split(cell_lr_separator, 1)[1] for x in vertices]
     g.vs['color'] = vertices_color
     g.vs['weight'] = [x/reducer if x>reducer*5 else 5 for x in sectors.values()]
     g.es['weight'] = [x[2] for x in links]
     g.es['color'] = edges_color
     return g
 
 def grap_plot(interaction_matrix:pd.DataFrame,
               cells:list,
-              separator:str='_',
+              separator:str='-',
+              cell_lr_separator:str="|",
               layout_type:str='kk',
               save:str=None,
               **kwargs,
               ):
     '''
     Input:
         interaction_matrix: DataFrame. Matrix contains interesting interaction in the TME region of interest, index represents cell-cell pairs
                             while column represents ligand-receptor pairs
         cells: List of cell type names, which will be used to separate cells of the cell pair.
-        separator: Separator used to combine sender and receiver cells into a cell pair.
+        separator: Separator used to combine ligand with receptor genes into LR pairs.
+        cell_lr_separator: Separator used to combine cells with LR genes.
         layout_type: Layout style used to draw the graph. Same to the layout of igraph
         save: File name of the figure that will be saved.
         **kwargs: Dictionary containing parameters of igraph plot setting.
     Return:
         None
     '''
     
-    g = lr_link_graph_generate(interaction_matrix, cells, separator=separator)
-    cell_colors = dict(zip([x.split("-")[0] for x in g.vs['name']], g.vs['color']))
-    link_colors = dict(zip([f"{x.source_vertex['label']}-{x.target_vertex['label']}" for x in g.es], g.es['color']))
+    g = lr_link_graph_generate(interaction_matrix, cells, separator=separator, cell_lr_separator=cell_lr_separator)
+    cell_colors = dict(zip([x.split(cell_lr_separator)[0] for x in g.vs['name']], g.vs['color']))
+    link_colors = dict(zip([f"{x.source_vertex['label']}{separator}{x.target_vertex['label']}" for x in g.es], g.es['color']))
 
     fig, ax = plt.subplots()
     layout = g.layout(layout_type)
     layout.rotate(0)
     #draw graph
     ig.plot(g,
             layout = layout,
```

### Comparing `stereosite-1.1.5/stereosite/ppi/ppi_analysis.py` & `stereosite-2.0.0/stereosite/ppi/ppi_analysis.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/ppi/query.py` & `stereosite-2.0.0/stereosite/ppi/query.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/read/gem.py` & `stereosite-2.0.0/stereosite/read/gem.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/scii.py` & `stereosite-2.0.0/stereosite/scii.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite/tf_infer.py` & `stereosite-2.0.0/stereosite/tf_infer.py`

 * *Files identical despite different names*

### Comparing `stereosite-1.1.5/stereosite.egg-info/PKG-INFO` & `stereosite-2.0.0/stereosite.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: stereosite
-Version: 1.1.5
+Version: 2.0.0
 Summary: Analysis spatial transcriptomics data
 Home-page: https://github.com/STOmics/StereoSiTE
 Author: LiuXing
 Author-email: liuxing2@genomics.cn
 License: GPL-3 License
 Keywords: spatial cell interaction intensity
 Platform: any
 License-File: LICENSE
 Requires-Dist: anndata>=0.8.0
 Requires-Dist: scanpy>=1.9.1
 Requires-Dist: squidpy>=1.1.2
 Requires-Dist: decoupler>=1.4.0
 Requires-Dist: pydeseq2>=0.3.6
 Requires-Dist: networkx>=3.1
+Requires-Dist: tensorly>=0.8.1
+Requires-Dist: scikit-learn>=1.2.1
+Requires-Dist: torch>=1.11.0
+Requires-Dist: igraph>=0.10.4
+Requires-Dist: pycirclize>=1.1.0
+Requires-Dist: cell2location==0.1.3
 
 StereoSiTE - Spatial Transcriptome Analysis in Python
 ======================================================
 
 **StereoSiTE** is a package for the analysis and visualization of spatial transcriptome data.
 It builds on top of `anndata`_, `scanpy`_ and `squidpy`_, from which it inherits modularity and scalability.
 It provides analysis tools to dissect cellular neighborhood based on cell composition and quantitatively define cell-cell communication in spatial.
```

### Comparing `stereosite-1.1.5/stereosite.egg-info/SOURCES.txt` & `stereosite-2.0.0/stereosite.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 PYPI.rst
 README.rst
 setup.py
 stereosite/__init__.py
 stereosite/degene.py
 stereosite/scii.py
+stereosite/scii_tensor.py
 stereosite/tf_infer.py
 stereosite.egg-info/PKG-INFO
 stereosite.egg-info/SOURCES.txt
 stereosite.egg-info/dependency_links.txt
 stereosite.egg-info/requires.txt
 stereosite.egg-info/top_level.txt
 stereosite/cn/__init__.py
@@ -19,12 +20,13 @@
 stereosite/plot/intensity.py
 stereosite/plot/mask.py
 stereosite/plot/net.py
 stereosite/plot/sankey.py
 stereosite/plot/scii.py
 stereosite/plot/scii_circos.py
 stereosite/plot/scii_net.py
+stereosite/plot/scii_tensor.py
 stereosite/ppi/__init__.py
 stereosite/ppi/ppi_analysis.py
 stereosite/ppi/query.py
 stereosite/read/__init__.py
 stereosite/read/gem.py
```

