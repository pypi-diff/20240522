# Comparing `tmp/ADViewpy-0.2a0.tar.gz` & `tmp/ADViewpy-0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADViewpy-0.2a0.tar", last modified: Fri May 17 07:38:10 2024, max compression
+gzip compressed data, was "ADViewpy-0.3a0.tar", last modified: Wed May 22 13:48:54 2024, max compression
```

## Comparing `ADViewpy-0.2a0.tar` & `ADViewpy-0.3a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:38:10.086003 ADViewpy-0.2a0/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:38:10.066999 ADViewpy-0.2a0/ADViewpy/
--rw-rw-rw-   0        0        0    44333 2024-05-06 09:06:33.000000 ADViewpy-0.2a0/ADViewpy/ADViewpy.py
--rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.2a0/ADViewpy/__init__.py
--rw-rw-rw-   0        0        0    18629 2024-05-06 05:26:44.000000 ADViewpy-0.2a0/ADViewpy/myCanvas.py
--rw-rw-rw-   0        0        0     3014 2024-05-06 02:28:03.000000 ADViewpy-0.2a0/ADViewpy/myUtils.py
--rw-rw-rw-   0        0        0    46111 2024-05-06 05:27:03.000000 ADViewpy-0.2a0/ADViewpy/pairwiseCanvas.py
--rw-rw-rw-   0        0        0    22890 2024-05-06 05:27:03.000000 ADViewpy-0.2a0/ADViewpy/rtCanvas.py
--rw-rw-rw-   0        0        0    64944 2024-05-06 05:27:03.000000 ADViewpy-0.2a0/ADViewpy/tcCanvas.py
--rw-rw-rw-   0        0        0    21925 2024-05-06 05:26:57.000000 ADViewpy-0.2a0/ADViewpy/treeDistributionView.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:38:10.083998 ADViewpy-0.2a0/ADViewpy.egg-info/
--rw-rw-rw-   0        0        0     6202 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6202 2024-05-17 07:38:10.087002 ADViewpy-0.2a0/PKG-INFO
--rw-rw-rw-   0        0        0     5716 2024-05-17 07:36:32.000000 ADViewpy-0.2a0/README.md
--rw-rw-rw-   0        0        0      539 2024-05-17 07:37:43.000000 ADViewpy-0.2a0/pyproject.toml
--rw-rw-rw-   0        0        0       94 2024-05-17 07:38:10.089000 ADViewpy-0.2a0/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-17 07:37:54.000000 ADViewpy-0.2a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:48:54.064397 ADViewpy-0.3a0/
+drwxrwxrwx   0        0        0        0 2024-05-22 13:48:54.056354 ADViewpy-0.3a0/ADViewpy/
+-rw-rw-rw-   0        0        0    46666 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/ADViewpy.py
+-rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.3a0/ADViewpy/__init__.py
+-rw-rw-rw-   0        0        0    19348 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/myCanvas.py
+-rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.3a0/ADViewpy/myUtils.py
+-rw-rw-rw-   0        0        0    56158 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/pairwiseCanvas.py
+-rw-rw-rw-   0        0        0    23499 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/rtCanvas.py
+-rw-rw-rw-   0        0        0    65738 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/tcCanvas.py
+-rw-rw-rw-   0        0        0    21925 2024-05-22 13:41:29.000000 ADViewpy-0.3a0/ADViewpy/treeDistributionView.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:48:54.064397 ADViewpy-0.3a0/ADViewpy.egg-info/
+-rw-rw-rw-   0        0        0     6202 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 13:48:53.000000 ADViewpy-0.3a0/ADViewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6202 2024-05-22 13:48:54.065402 ADViewpy-0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.3a0/README.md
+-rw-rw-rw-   0        0        0      539 2024-05-22 13:47:29.000000 ADViewpy-0.3a0/pyproject.toml
+-rw-rw-rw-   0        0        0       94 2024-05-22 13:48:54.066403 ADViewpy-0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-22 13:47:29.000000 ADViewpy-0.3a0/setup.py
```

### Comparing `ADViewpy-0.2a0/ADViewpy/ADViewpy.py` & `ADViewpy-0.3a0/ADViewpy/ADViewpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,39 +50,60 @@
 
         self.tree_distribution_view = None
         self.tree_distance_fig = None
 
         self.ad_cluster_canvas_export = None
         self.ad_individual_canvas_export = None
 
+        self.rt_exact_match_range = None
+        self.rt_support_value_range = None
+
+        self.pairwise_tree = None
+
+
         # Paiwise canvas related
         self.pairwise_canvas = None
         self.default_subtree_attribute()
         # Reaf tree file and construct reference tree
         self.read_rt(treefile = treefile, type = type)
 
 
     # ==========================  Public Functions ================================== #
 
     # reference_tree() : Function to show reference tree visualization
     # Parameter: view_support (Whether to write support value of internal node on tree)
     # Draw reference tree on canvas
     # User can select subtree through mouse click
-    def reference_tree(self,view_support=False,show=True):
+    def reference_tree(self,view_support=False,show=True,exact_match_range=None,support_value_range=None):
         # Calculate height of canvas
         height = get_leaf_node_amount(self.rt) * RT_Y_INTERVAL + RT_Y_INTERVAL
+        if exact_match_range and not self.check_attribute_range(exact_match_range):
+            self.parameter_error("exact_match_range")
+            return
+
+        if support_value_range and not self.check_attribute_range(support_value_range):
+            self.parameter_error("support_value_range")
+            return
 
         if not self.rt_canvas and not self.pairwise_canvas:
             self.default_subtree_attribute()
             self.default_rt = None
             self.rt_view_support = view_support
+            self.rt_exact_match_range = exact_match_range
+            self.rt_support_value_range = support_value_range
             self.create_pairwise_rt_canvas(alter_type=BOTH)
 
-        if self.check_parameter_alter(view_support):
-            self.create_pairwise_rt_canvas(alter_type=RT)
+        else:
+            check_parameter = self.check_parameter_alter(view_support, exact_match_range, support_value_range)
+
+            if check_parameter == REDRAW:
+                self.create_pairwise_rt_canvas(alter_type=RT)
+
+            if check_parameter == FILTER_NODE:
+                self.rt_canvas.draw_filter_node(exact_match_range, support_value_range)
 
         if show:
             return self.rt_canvas
 
     # set_outgroup() : Function to set trees' outgroup
     # Parameter : outgroup_taxon (python list)
     def set_outgroup(self,outgroup_taxon):
@@ -199,15 +220,15 @@
         # node = self.rt.find_node_with_taxon_label(node)
         # self.rt_canvas.draw_subtree_block(node)
 
     # AD() : Function to get Aggregated Dendrogram, Individual AD or cluster AD
     def AD(self,view=AD_INDIVIDUAL,scale=1.0,max_ad=None,context_level=2,ad_interval=None,tree_id=None,
            tree_name=None,filter=INCLUDE,sort=RF_DISTANCE,escape_taxa_as_context_block=True,show_block_proportional=True,
            subtree_independent=False,parameter_from_individual_ad=True,differentiate_inexact_match=True,
-           show_tree_name=False,export=False):
+           show_tree_name=False,export=False,compress_escape_taxa=True):
 
         if len(self.subtree_list) == 0:
             print("<Error> : No Subtree Chosen")
             return
 
         if not self.tc:
             self.not_exist_error(tree="Tree Collection",pre_function="add_tree_collection()")
@@ -264,40 +285,43 @@
                     ad_row = math.ceil(max_ad / ad_per_row)
                 else:
                     ad_row = math.ceil(len(self.tc) / ad_per_row)
 
                 canvas_height = (ad_row * DEFAULT_AD_HEIGHT * scale) + (2 * DEFAULT_PADDING_BETWEEN_AD) +  ((ad_row -
                                                                                                              1) * DEFAULT_PADDING_BETWEEN_AD)
                 if export:
-                    self.ad_individual_canvas_export = tcCanvas(layer = ad_row,adPy=self,view=view,
-                                                                  width=CANVAS_MAX_WIDTH,
-                                                                  height=canvas_height, scale=scale,max_ad=max_ad,
-                                                                  ad_per_row=ad_per_row, context_level=context_level,
-                                                                  first_ad=first_ad, last_ad=last_ad,tree_id=tree_id,
-                                                                  tree_name=tree_name, sort_by=sort,
-                                                                  escape_taxa_as_context_block=escape_taxa_as_context_block,
-                                                                  show_block_proportional=show_block_proportional,
-                                                                  subtree_independent=subtree_independent,show_tree_name=show_tree_name)
+                    self.ad_individual_canvas_export = tcCanvas(layer=ad_row, adPy=self, view=view,
+                                                                width=CANVAS_MAX_WIDTH, filter=filter,
+                                                                height=canvas_height, scale=scale, max_ad=max_ad,
+                                                                ad_per_row=ad_per_row, context_level=context_level,
+                                                                first_ad=first_ad, last_ad=last_ad, tree_id=tree_id,
+                                                                tree_name=tree_name, sort_by=sort,
+                                                                escape_taxa_as_context_block=escape_taxa_as_context_block,
+                                                                show_block_proportional=show_block_proportional,
+                                                                subtree_independent=subtree_independent,
+                                                                show_tree_name=show_tree_name,compress_escape_taxa=compress_escape_taxa)
 
                     self.ad_individual_canvas_export.TREE_NAME_LAYER = -3
                     for index, ad_tree in enumerate(self.ad_individual_canvas_export.ad_list):
                         with hold_canvas(self.ad_individual_canvas_export):
                             self.ad_individual_canvas_export.paste_ad_tree_canvas(ad_tree)
                         self.ad_individual_canvas_export[ad_tree.located_layer].flush()
 
                 else:
-                    self.ad_individual_canvas = tcCanvas(layer = ad_row,adPy=self,view=view,
-                                                                  width=CANVAS_MAX_WIDTH,
-                                                                  height=canvas_height, scale=scale,max_ad=max_ad,
-                                                                  ad_per_row=ad_per_row, context_level=context_level,
-                                                                  first_ad=first_ad, last_ad=last_ad,tree_id=tree_id,
-                                                                  tree_name=tree_name, sort_by=sort,
-                                                                  escape_taxa_as_context_block=escape_taxa_as_context_block,
-                                                                  show_block_proportional=show_block_proportional,
-                                                                  subtree_independent=subtree_independent,show_tree_name=show_tree_name)
+                    self.ad_individual_canvas = tcCanvas(layer=ad_row, adPy=self, view=view,
+                                                         width=CANVAS_MAX_WIDTH, filter=filter,
+                                                         height=canvas_height, scale=scale, max_ad=max_ad,
+                                                         ad_per_row=ad_per_row, context_level=context_level,
+                                                         first_ad=first_ad, last_ad=last_ad, tree_id=tree_id,
+                                                         tree_name=tree_name, sort_by=sort,
+                                                         escape_taxa_as_context_block=escape_taxa_as_context_block,
+                                                         show_block_proportional=show_block_proportional,
+                                                         subtree_independent=subtree_independent,
+                                                         show_tree_name=show_tree_name,
+                                                         compress_escape_taxa=compress_escape_taxa)
                     display(self.ad_individual_canvas)
                     for index, ad_tree in enumerate(self.ad_individual_canvas.ad_list):
                         with hold_canvas(self.ad_individual_canvas):
                             self.ad_individual_canvas.paste_ad_tree_canvas(ad_tree)
                         # with hold_canvas(self.ad_individual_canvas):
                         #     self.ad_individual_canvas.draw_ad_tree(ad_tree)
                         self.ad_individual_canvas[ad_tree.located_layer].flush()
@@ -367,14 +391,20 @@
     # Parameter : compare_tree(integer or integer list - tree id ; string or string list - tree name)
     def pairwise_comparison(self,compare_tree=None):
         if not self.rt_canvas and not self.pairwise_canvas:
             self.create_pairwise_rt_canvas()
 
         compare_between_tc = False
         if compare_tree:
+            if compare_tree == self.pairwise_tree:
+                display(self.pairwise_canvas)
+                return
+            else:
+                self.pairwise_tree = compare_tree
+
             if type(compare_tree) is list:
                 tmp_list = []
                 for tree in compare_tree:
                     if isinstance(tree, str):
                         tmp_tree = self.get_tree_by_name(tree)
 
                         if tmp_tree is None:
@@ -417,14 +447,15 @@
         else:
             if not self.ad_individual_canvas.tree_selected:
                 self.no_tree_chosen_error()
                 return
 
             compare_tree = self.ad_individual_canvas.tree_selected.tc_tree
 
+
         display(self.pairwise_canvas)
         self.pairwise_canvas.compare_tc_tree(compare_tree,compare_between_tc=compare_between_tc)
 
     def tree_distribution(self,test=False):
         self.rt_canvas.clear_subtree_compare_canvas()
         self.tc_canvas_tmp = tcCanvas(adPy=self, view=TREE_DISTRIBUTION, subtree_independent=False)
 
@@ -703,24 +734,23 @@
 
         with hold_canvas(rt_canvas_image):
             rt_canvas_image.fill_rect(0, 0, self.rt_canvas.width, self.rt_canvas.height)
 
             for i in range(6):
                 rt_canvas_image.draw_image(self.rt_canvas[i],0,0)
 
-            rt_canvas_image.draw_image(self.rt_canvas[-1], 0, 0)
+            rt_canvas_image.draw_image(self.rt_canvas[-3], 0, 0)
 
 
         rt_canvas_image.flush()
 
         return rt_canvas_image
 
     def save_to_file(self,*args, **kwargs):
         # self.export_canvas.to_file("save_file.png")
-        self.output.append("in save_to_file")
         self.export_canvas.to_file(f"{self.image_name}.{self.image_type}")
 
     def print_tree_distribution(self):
         if not self.ad_individual_canvas and not self.ad_cluster_canvas and not self.tree_distribution_tmp:
             tmp = tcCanvas(adPy=self, view=TREE_DISTRIBUTION)
 
         for subtree in self.subtree_list:
@@ -739,17 +769,21 @@
         rt_label = os.path.basename(treefile)
         self.rt.id = 0
         self.rt.name = rt_label
         self.rt.level = 0
         self.rt.pairwise_canvas = None
         self.rt.missing = set()
 
-        # Get tree's taxa/leaf node
+        self.rt.taxa_list = []
+        self.rt.internal_node = []
+
         self.rt.taxa_list = [leaf.taxon.label for leaf in self.rt.leaf_nodes()]
 
+
+
     def generate_missing_node(self,tree,taxa_name):
         new_taxon = dendropy.Taxon(label=taxa_name)
         new_node = dendropy.Node(taxon=new_taxon, label=taxa_name)
         new_node.is_missing = True
 
         tree.missing_node_list.append(new_node)
 
@@ -892,29 +926,53 @@
         if self.rt_alter:
             self.default_rt = None
             self.rt_alter = False
 
         # Check paramater alter
         if alter_type == BOTH:
             # self.default_rt_value()
-            self.rt_canvas = rtCanvas(self, width=CANVAS_MAX_WIDTH, height=height ,
-                                               view_support=self.rt_view_support, default_rt=self.default_rt)
+            self.rt_canvas = rtCanvas(self, width=CANVAS_MAX_WIDTH, height=height,
+                                      view_support=self.rt_view_support, default_rt=self.default_rt,
+                                      exact_match_range=self.rt_exact_match_range,
+                                      support_value_range=self.rt_support_value_range)
             self.pairwise_canvas = pairwiseCanvas(self, width=CANVAS_MAX_WIDTH, height=height)
         elif alter_type == RT:
             self.rt_canvas = rtCanvas(self, width=CANVAS_MAX_WIDTH, height=height,
-                                               view_support=self.view_support, default_rt=self.default_rt)
+                                      view_support=self.rt_view_support, default_rt=self.default_rt,
+                                      exact_match_range=self.rt_exact_match_range,
+                                      support_value_range=self.rt_support_value_range)
         elif alter_type == PAIRWISE:
             self.pairwise_canvas = pairwiseCanvas(self, width=CANVAS_MAX_WIDTH, height=height)
 
-
-    def check_parameter_alter(self,view_support):
+    def check_parameter_alter(self, view_support, exact_match_range, support_value_range):
         # Check whether parameter has alter and set parameter as self.attribute
         if view_support != self.rt_view_support:
             self.rt_view_support = view_support
-            return True
+            return REDRAW
+
+        if exact_match_range != self.rt_exact_match_range:
+            self.rt_exact_match_range = exact_match_range
+            return FILTER_NODE
+
+        if support_value_range != self.rt_support_value_range:
+            self.rt_support_value_range = support_value_range
+            return FILTER_NODE
+
+    def check_attribute_range(self,interval_list):
+
+        if len(interval_list) != 2:
+            return False
+
+        if not isinstance(interval_list[0], int) or not isinstance(interval_list[1], int):
+            return False
+
+        if interval_list[0] > interval_list[1]:
+            return False
+
+        return True
 
     def select_subtree_from_tree(self,node_selected):
         if not hasattr(node_selected, 'selected') or node_selected.selected == False:
             self.ad_parameter_alter = True
             # Ignore if 5 subtree had selected
             if len(self.subtree_list) >= 5:
                 return None
@@ -945,15 +1003,14 @@
 
                 self.pairwise_canvas.draw_escape_taxa(align=RIGHT)
                 if self.pairwise_canvas.compare_between_tc:
                     self.pairwise_canvas.draw_tc_subtree_block(new_subtree,align=LEFT)
                     self.pairwise_canvas.draw_escape_taxa(align=LEFT)
 
             # return new_subtree
-
         else:
             self.rt_canvas.remove_subtree_block(node_selected.subtree)
             self.pairwise_canvas.remove_subtree_block(node_selected.subtree)
             self.subtree_list.remove(node_selected.subtree)
 
             # Release Color
```

### Comparing `ADViewpy-0.2a0/ADViewpy/myCanvas.py` & `ADViewpy-0.3a0/ADViewpy/myCanvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,18 +287,30 @@
             print(' ' * (level * 4) + node.type, end=" ")
             print(internaL_node)
 
         elif node.type == LEAF:
             block = node.node_or_block
 
             if block.type == SUBTREE_BLOCK:
-                print(' ' * (level * 4) + block.belong_subtree.label + ':' + str(block.subtree_taxa_count))
-            elif block.type == INDIVIDUAL_BLOCK:
+                if type(block.belong_subtree) is list:
+                    str = ""
+                    for subtree in block.belong_subtree:
+                        str += subtree.label + "&"
+                    print(' ' * (level * 4) + str[:-1] + ':' )
+                else:
+                    print(' ' * (level * 4) + block.belong_subtree.label + ':')
+            elif block.type == INDIVIDUAL_BLOCK or block.type == INDIVIDUAL_LEAF_BLOCK:
                 if block.belong_subtree:
-                    print(' ' * (level * 4) + block.belong_subtree.label + ': INDIVIDUAL LEAF')
+                    if type(block.belong_subtree) is list:
+                        for subtree in block.belong_subtree:
+                            str += subtree.label + "&"
+
+                        print(' ' * (level * 4) + str[:-1] + ': INDIVIDUAL LEAF')
+                    else:
+                        print(' ' * (level * 4) + block.belong_subtree.label + ': INDIVIDUAL LEAF')
                 else:
                     print(' ' * (level * 4) + 'INDV BLANK BLOCK')
 
         for child in node.children:
             self.plot_tree(child, level + 1)
 
     def generate_block_list(self):
@@ -493,14 +505,19 @@
                 for index, subtree in enumerate(block.belong_subtree):
                     if subtree_label == subtree.label:
                         block.exact_match[index] = False
             else:
                 if subtree_label == block.belong_subtree.label:
                     block.exact_match = False
 
+class Escape_Taxa:
+    def __init__(self, node):
+        self.node = node
+        self.subtree_list = []
+        self.escape_taxa_block = None
 
 def hex_to_rgb(hex_color):
     hex_color = hex_color.lstrip('#')
     return tuple(int(hex_color[i:i + 2], 16) for i in (0, 2, 4))
 
 def rgb_to_hex(rgb_color):
     return '#{:02x}{:02x}{:02x}'.format(*rgb_color)
```

### Comparing `ADViewpy-0.2a0/ADViewpy/myUtils.py` & `ADViewpy-0.3a0/ADViewpy/myUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,16 @@
 CONTINUE = 'continue'
 TRUE = 'True'
 FULFILL = 'Fulfill'
 
 # Filter
 INCLUDE = 'include'
 EXCLUDE = 'exclude'
+REDRAW = 'Redraw'
+FILTER_NODE = 'Filter node'
 
 # Sort AD
 ID = 'id'
 RF_DISTANCE = 'rf distance'
 SIMILARITY = 'similarity'
 NAME = 'name'
```

### Comparing `ADViewpy-0.2a0/ADViewpy/pairwiseCanvas.py` & `ADViewpy-0.3a0/ADViewpy/pairwiseCanvas.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
         self.adPy = adPy
         self.rt = adPy.rt
         # tc_tree = copy.deepcopy(adPy.rt)
         self.tc_tree = tc_tree
         self.max_level = None
 
-        self.left_escape_taxa_list = {}  # {'node':[subtree.color]}
-        self.right_escape_taxa_list = {}
-        self.left_escape_taxa_subtree = []
+        self.left_escape_taxa_list = []  # {'node':[subtree.color]}
+        self.right_escape_taxa_list = []
+        self.left_escape_taxa_subtree =[]
         self.right_escape_taxa_subtree = []
 
         self.rt_layer_block_list = {}
         self.tc_left_layer_block_list = {}
         self.tc_right_layer_block_list = {}
 
         self.rt_sorted_layer_list = []
@@ -58,20 +58,24 @@
         self.left_tree_width = 0
         self.right_tree_width = self.width
         self.left_tree_height = 0
         self.right_tree_height = 0
 
         self.node_hover = None
 
+        self.initialization = True
+
         self.last_draw_time = time.time()
         self.last_mouse_position = None
 
         self.left_missing_taxa_list = []
         self.right_missing_taxa_list = []
 
+        self.duplicate_subtree_list = []
+
         self.rt_section_list = []
         self.left_tree_section_list = []
         self.right_tree_section_list = []
         self.inner_section = True
         self.last_draw_time = time.time()
         self.last_mouse_position = None
         self.setup_section_list([self.rt_section_list,self.left_tree_section_list,self.right_tree_section_list])
@@ -105,25 +109,25 @@
                         section_list[i].append([])
 
     def default_value(self,align):
         if align == LEFT:
             self.left_tree_width = 0
             self.left_tree_height = 0
             self.x = 30
-            self.left_escape_taxa_list = {}  # {'node':[subtree.color]}
+            self.left_escape_taxa_list = []  # {'node':[subtree.color]}
             self.left_escape_taxa_subtree = []
             self.tc_left_layer_block_list = {}
             self.tc_left_sorted_layer_list = []
             self.tc_left_layer_occupied = [0, 0, 0, 0, 0]
             self.tc_left_subtree_list = []
             self.left_tree_section_list = []
             self.setup_section_list([self.left_tree_section_list])
         elif align == RIGHT:
             self.x = self.width - 200
-            self.right_escape_taxa_list = {}
+            self.right_escape_taxa_list = []
             self.right_escape_taxa_subtree = []
             self.tc_right_layer_block_list = {}
             self.tc_right_sorted_layer_list = []
             self.tc_right_layer_occupied = [0, 0, 0, 0, 0]
             self.tc_right_subtree_list = []
             self.right_tree_width = self.width
             self.right_tree_height = 0
@@ -414,26 +418,24 @@
     def mouse_hover(self, x, y):
         type = None
         align = None
         node_selected = None
         subtree_root = False
 
         current_time = time.time()
-        if current_time - self.last_draw_time > 0.2:
+        if current_time - self.last_draw_time > 0.15:
             self.last_draw_time = current_time
 
             # Filter node
             if x <= self.left_tree_width:
                 align = LEFT
 
                 if self.compare_between_tc:
                     type = TC
                     node_selected = self.filter_node_from_section_list(self.left_tree_section_list, x, y)
-
-
                     if node_selected in self.left_escape_taxa_list:
                         subtree_root = True
                     for subtree in self.adPy.subtree_list:
                         if node_selected == subtree.root.corr[self.tc_tree[0].id]:
                             subtree_root = True
 
                 else:
@@ -646,41 +648,38 @@
         else:
             node = tree.find_node_with_taxon_label(taxa_name)
 
         return node
 
     def remove_escape_taxa(self,subtree_label,escape_taxa_list):
         escape_taxa_delete = []
-        for escape_taxa,subtree_list in escape_taxa_list.items():
-
+        for escape_taxa in escape_taxa_list:
+            subtree_list = escape_taxa.subtree_list
             for subtree in subtree_list:
                 if subtree_label == subtree.label:
                     subtree_list.remove(subtree)
-                    if len(subtree_list) == 0:
-                        escape_taxa_delete.append(escape_taxa)
-        for taxa in escape_taxa_delete:
-            del escape_taxa_list[taxa]
-
+                    escape_taxa_list.remove(escape_taxa)
         return
 
-
     def draw_escape_taxa(self,align):
         if align == LEFT:
             tree = self.left_tree
             layer_index = self.LEFT_ESCAPE_TAXA_LAYER
             escape_taxa_list = self.left_escape_taxa_list
         else:
             tree = self.right_tree
             layer_index = self.RIGHT_ESCAPE_TAXA_LAYER
             escape_taxa_list = self.right_escape_taxa_list
 
         self[layer_index].clear()
-        for escape_taxa,subtree_list in escape_taxa_list.items():
-            node = self.get_node_from_tree(tree,escape_taxa)
-            block = node.escape_taxa_block
+        
+        for escape_taxa in escape_taxa_list:
+            subtree_list = escape_taxa.subtree_list
+            node = escape_taxa.node
+            block = escape_taxa.escape_taxa_block
             if len(subtree_list) == 1:
                 subtree = subtree_list[0]
                 self.draw_rec(block.topL.x, block.topL.y, block.width, block.height,subtree.color,layer_index=layer_index)
             else:
                 segment_width = block.width / len(subtree_list)
                 for index,subtree in enumerate(subtree_list):
                     self.draw_rec(block.topL.x + segment_width * index, block.topL.y, segment_width, block.height,subtree.color,layer_index=layer_index)
@@ -689,20 +688,23 @@
         if align == LEFT:
             taxa_list = self.left_escape_taxa_list
             taxa_subtree_list = self.left_escape_taxa_subtree
         else:
             taxa_list = self.right_escape_taxa_list
             taxa_subtree_list = self.right_escape_taxa_subtree
 
-        node_selected.escape_taxa_block = self.generate_subtree_block(node_selected,align=align)
-        taxa_subtree_list.append(subtree.label)
-        if node_selected.taxon.label not in taxa_list:
-            taxa_list[node_selected.taxon.label] = []
+        for escape_taxa in taxa_list:
+            if escape_taxa.node == node_selected:
+                escape_taxa.subtree_list.append(subtree)
+                return
 
-        taxa_list[node_selected.taxon.label].append(subtree)
+        new_escape_taxa = Escape_Taxa(node_selected)
+        new_escape_taxa.escape_taxa_block = self.generate_subtree_block(node_selected, align=align)
+        new_escape_taxa.subtree_list.append(subtree)
+        taxa_list.append(new_escape_taxa)
 
     def record_missing_taxa(self,node_selected,subtree,align):
         if align == LEFT:
             taxa_list = self.left_missing_taxa_list
         else:
             taxa_list = self.right_missing_taxa_list
 
@@ -728,183 +730,315 @@
             self.draw_subtree_block(taxa,select_tree=TC,new_subtree=taxa.subtree,align=align)
 
     def draw_subtree_block(self,node_selected,select_tree=None,new_subtree=None,subtree_from_rt=None,align=None):
         new_block = self.generate_subtree_block(node_selected, align=align)
         new_subtree.set_pairwise_block(new_block)
 
         if select_tree == RT:
-            first_layer = 0
-            last_layer = 5
-        elif select_tree == TC:
-            if align == RIGHT:
-                first_layer = 7
-                last_layer = 12
-            else:
-                first_layer = 14
-                last_layer = 19
-
-        if select_tree == RT:
-            self.draw_subtree_list = sorted(self.adPy.subtree_list, key=lambda x: x.block_size,reverse=True)
+            draw_layer = self.get_layer_index(subtree=new_subtree,tmp_layer_occupied=self.rt_layer_occupied,
+                                              tmp_layer_block_list=self.rt_layer_block_list,
+                                              align=align,type=select_tree)
         else:
             if align == LEFT:
-                self.draw_subtree_list = sorted(self.tc_left_subtree_list, key=lambda x: x.block_size,reverse=True)
-            else:
-                self.draw_subtree_list = sorted(self.tc_right_subtree_list, key=lambda x: x.block_size, reverse=True)
+                draw_layer = self.get_layer_index(subtree=new_subtree, tmp_layer_occupied=self.tc_left_layer_occupied,
+                                                  tmp_layer_block_list=self.tc_left_layer_block_list,
+                                                  align=align, type=select_tree)
 
-        subtree_cnt = len(self.draw_subtree_list)
-        tmp_sorted_layer_list = []
-        for i in range(first_layer,first_layer + subtree_cnt):
-            if select_tree == RT:
-                subtree = self.draw_subtree_list[i]
+                draw_layer += 14
             else:
-                if align == RIGHT:
-                    subtree = self.draw_subtree_list[i - 7]
-                else:
-                    subtree = self.draw_subtree_list[i - 14]
+                draw_layer = self.get_layer_index(subtree=new_subtree, tmp_layer_occupied=self.tc_right_layer_occupied,
+                                                  tmp_layer_block_list=self.tc_right_layer_block_list,
+                                                  align=align, type=select_tree)
 
-            subtree_block = subtree.pairwise_block
-            tmp_sorted_layer_list.append(subtree.label)
+                draw_layer += 7
 
-            self[i].clear()
-            if subtree.root.is_missing:
-                subtree_block = subtree.root.pairwise_block
+        # draw_layer = self.get_layer_index(subtree=new_subtree,align=align,type=select_tree)
 
+        if new_subtree.root.is_missing:
+            subtree_block = new_subtree.root.pairwise_block
+        else:
+            subtree_block = new_subtree.pairwise_block
 
-            self.draw_rec(subtree_block.topL.x, subtree_block.topL.y, subtree_block.width, subtree_block.height,subtree.color,
-                      layer_index=i)
 
-            if subtree.root.is_missing == False:
-                self.write_block_label(subtree, i,align=align)
+        self.draw_subtree_rec(subtree_block=subtree_block,subtree=new_subtree,layer_index=draw_layer)
 
-            self[i].label = subtree.label
-            self[i].flush()
+        if new_subtree.root.is_missing == False:
+            self.write_block_label(new_subtree, draw_layer,align=align)
 
-        if select_tree == RT:
-            self.rt_sorted_layer_list = tmp_sorted_layer_list
-        elif select_tree == TC:
-            if align == LEFT:
-                self.tc_left_sorted_layer_list = tmp_sorted_layer_list
-            else:
-                self.tc_right_sorted_layer_list = tmp_sorted_layer_list
 
+        self[draw_layer].label = new_subtree.label
+        self[draw_layer].flush()
+
+
+    # def draw_subtree_block(self,node_selected,select_tree=None,new_subtree=None,subtree_from_rt=None,align=None):
+    #     new_block = self.generate_subtree_block(node_selected, align=align)
+    #     new_subtree.set_pairwise_block(new_block)
+    # 
+    #     if select_tree == RT:
+    #         first_layer = 0
+    #         last_layer = 5
+    #     elif select_tree == TC:
+    #         if align == RIGHT:
+    #             first_layer = 7
+    #             last_layer = 12
+    #         else:
+    #             first_layer = 14
+    #             last_layer = 19
+    # 
+    #     if select_tree == RT:
+    #         self.draw_subtree_list = sorted(self.adPy.subtree_list, key=lambda x: x.block_size,reverse=True)
+    #     else:
+    #         if align == LEFT:
+    #             self.draw_subtree_list = sorted(self.tc_left_subtree_list, key=lambda x: x.block_size,reverse=True)
+    #         else:
+    #             self.draw_subtree_list = sorted(self.tc_right_subtree_list, key=lambda x: x.block_size, reverse=True)
+    # 
+    #     subtree_cnt = len(self.draw_subtree_list)
+    #     tmp_sorted_layer_list = []
+    #     for i in range(first_layer,first_layer + subtree_cnt):
+    #         if select_tree == RT:
+    #             subtree = self.draw_subtree_list[i]
+    #         else:
+    #             if align == RIGHT:
+    #                 subtree = self.draw_subtree_list[i - 7]
+    #             else:
+    #                 subtree = self.draw_subtree_list[i - 14]
+    # 
+    #         subtree_block = subtree.pairwise_block
+    #         tmp_sorted_layer_list.append(subtree.label)
+    # 
+    #         self[i].clear()
+    #         if subtree.root.is_missing:
+    #             subtree_block = subtree.root.pairwise_block
+    # 
+    #         self.draw_subtree_rec(subtree_block=subtree_block,subtree=subtree,layer_index=i)
+    #         # self.draw_rec(subtree_block.topL.x, subtree_block.topL.y, subtree_block.width, subtree_block.height,subtree.color,
+    #         #           layer_index=i)
+    # 
+    #         if subtree.root.is_missing == False:
+    #             self.write_block_label(subtree, i,align=align)
+    # 
+    #         self[i].label = subtree.label
+    #         self[i].flush()
+    # 
+    #     if select_tree == RT:
+    #         self.rt_sorted_layer_list = tmp_sorted_layer_list
+    #     elif select_tree == TC:
+    #         if align == LEFT:
+    #             self.tc_left_sorted_layer_list = tmp_sorted_layer_list
+    #         else:
+    #             self.tc_right_sorted_layer_list = tmp_sorted_layer_list
+    def draw_subtree_rec(self,subtree_block,subtree,layer_index):
+        self[layer_index].clear()
+        if hasattr(subtree.root,'duplicate_subtree') and subtree.root.duplicate_subtree:
+            subtree_list = subtree.root.subtree
+            segment_width = subtree_block.width / len(subtree_list)
+            for index, subtree in enumerate(subtree_list):
+                self.draw_rec(subtree_block.topL.x + segment_width * index, subtree_block.topL.y, segment_width, subtree_block.height,
+                              subtree.color, layer_index=layer_index)
+        else:
+            self.draw_rec(subtree_block.topL.x, subtree_block.topL.y, subtree_block.width, subtree_block.height,
+                          subtree.color,
+                          layer_index=layer_index)
     def remove_subtree_block(self,subtree):
         # Clear corresponding rt layer
         try:
-            tc_clear_layer = None
-            clear_layer = self.rt_sorted_layer_list.index(subtree.label)
+            left_clear_layer = None
+            right_clear_layer = None
 
+            # CLear reference tree layer
+            clear_layer = self.rt_sorted_layer_list.index(subtree.label)
             self[clear_layer].clear()
 
+            del self.rt_layer_block_list[subtree.label]
+            self.rt_sorted_layer_list.remove(subtree.label)
+            self.rearrange_canvas_layer(clear_layer_index=clear_layer, type=RT, align=LEFT)
+            self.rt_layer_occupied[len(self.rt_sorted_layer_list)] = 0
+
             if self.tc_tree:
                 if self.compare_between_tc:
                     if subtree.label in self.tc_left_sorted_layer_list:
-                        tc_clear_layer = self.tc_left_sorted_layer_list.index(subtree.label)
-                        self[tc_clear_layer + 14].clear()
+                        left_clear_layer = self.tc_left_sorted_layer_list.index(subtree.label) + 14
+
+                        self[left_clear_layer].clear()
 
                 if subtree.label in self.tc_right_sorted_layer_list:
-                    tc_clear_layer = self.tc_right_sorted_layer_list.index(subtree.label)
-                    self[tc_clear_layer + 7].clear()
+                    right_clear_layer = self.tc_right_sorted_layer_list.index(subtree.label) + 7
+                    self[right_clear_layer].clear()
 
             if self.compare_between_tc:
                 left_subtree = self.get_subtree(self.tc_left_subtree_list, subtree.label)
+                if hasattr(left_subtree.root,'duplicate_subtree') and left_subtree.root.duplicate_subtree:
+                    left_subtree.root.subtree.remove(left_subtree)
+                    if len(left_subtree.root.subtree) == 1:
+                        left_subtree.root.duplicate_subtree = False
+                        left_subtree.root.subtree = left_subtree.root.subtree[0]
+
+                        redraw_layer = self.tc_right_sorted_layer_list.index(left_subtree.root.subtree.label) + 14
+                        self[redraw_layer].clear()
+                        self.draw_subtree_rec(left_subtree.root.subtree.pairwise_block, left_subtree.root.subtree,
+                                              redraw_layer)
+
+                else:
+                    left_subtree.root.selected = False
+                    left_subtree.root.subtree = None
+
+                del self.tc_left_layer_block_list[subtree.label]
+                self.tc_left_sorted_layer_list.remove(subtree.label)
+                self.rearrange_canvas_layer(clear_layer_index=left_clear_layer, type=TC, align=LEFT)
+                self.tc_left_layer_occupied[len(self.rt_sorted_layer_list)] = 0
+
+
                 self.tc_left_subtree_list.remove(left_subtree)
                 self.remove_escape_taxa(subtree.label,self.left_escape_taxa_list)
 
             right_subtree = self.get_subtree(self.tc_right_subtree_list, subtree.label)
             if right_subtree :
+                if hasattr(right_subtree.root,'duplicate_subtree') and right_subtree.root.duplicate_subtree:
+                    right_subtree.root.subtree.remove(right_subtree)
+                    if len(right_subtree.root.subtree) == 1:
+                        right_subtree.root.duplicate_subtree = False
+                        right_subtree.root.subtree = right_subtree.root.subtree[0]
+
+                        redraw_layer = self.tc_right_sorted_layer_list.index(right_subtree.root.subtree.label)
+                        redraw_layer += 7
+                        self[redraw_layer].clear()
+                        self.draw_subtree_rec(right_subtree.root.subtree.pairwise_block,right_subtree.root.subtree,
+                                              redraw_layer)
+                        
+                else:
+                    right_subtree.root.selected = False
+                    right_subtree.root.subtree = None
+
+                del self.tc_right_layer_block_list[subtree.label]
+                self.tc_right_sorted_layer_list.remove(subtree.label)
+                self.rearrange_canvas_layer(clear_layer_index=right_clear_layer, type=TC, align=RIGHT)
+                self.tc_right_layer_occupied[len(self.rt_sorted_layer_list)] = 0
+
                 self.tc_right_subtree_list.remove(right_subtree)
+
             self.remove_escape_taxa(subtree.label,self.right_escape_taxa_list)
 
             if self.compare_between_tc:
                 self.draw_escape_taxa(LEFT)
 
             self.draw_escape_taxa(RIGHT)
 
         except Exception as err:
             self[-1].fill_text("Loading", self.width - 200, 20)
 
-
     def setup_tc_subtree_list(self,tree,align):
         for index,subtree in enumerate(self.adPy.subtree_list):
+            subtree.root.duplicate_subtree = False
+            subtree.corresponding_tc_subtree = None
+
             self.draw_tc_subtree_block(subtree,align)
 
         self.draw_escape_taxa(align)
     def check_block_exact_match(self,tc_subtree,rt_subtree):
         if tc_subtree.leaf_set.issubset(rt_subtree.leaf_set):
             return True
         else:
             return False
 
-
     def draw_tc_subtree_block(self,subtree,align):
         if align == LEFT:
             subtree_list = self.tc_left_subtree_list
             tree = self.tc_tree[0]
         else:
             if self.compare_between_tc:
                 tree = self.tc_tree[1]
             else:
                 tree = self.tc_tree
             subtree_list = self.tc_right_subtree_list
 
         corresponding_subtree = subtree.root.corr[tree.id]
 
         # If taxa in corresponding subtree is all missing taxa in target tree
-
         new_subtree = Subtree(label=subtree.label, belong_tree=tree, root=corresponding_subtree,
                                    color=subtree.color)
         subtree_list.append(new_subtree)
         subtree.corresponding_tc_subtree = new_subtree
 
         if corresponding_subtree == 0:
             for leaf_node in subtree.root.leaf_nodes():
                 tc_corr = leaf_node.corr[tree.id]
 
                 self.record_escape_taxa(tc_corr, new_subtree, align)
             return
 
-
         new_subtree.get_leaf_nodes()
         subtree.get_leaf_nodes()
 
         exact_match = False
         if new_subtree.leaf_set == subtree.leaf_set:
             exact_match = True
 
         new_subtree.root.exact_match_percentage = len(subtree.leaf_set.intersection(new_subtree.leaf_set)) / len(
             subtree.leaf_set)
 
         if not exact_match:
             tmp_result = self.check_block_exact_match(new_subtree,subtree)
             if not tmp_result:
                 # All leaf nodes as escape taxa
-                for leaf_node in subtree.root.leaf_nodes():
-                    tc_corr = leaf_node.corr[tree.id]
-                    tc_corr.exact_match_percentage = new_subtree.root.exact_match_percentage
-                    self.record_escape_taxa(tc_corr,new_subtree,align)
+                escape_taxa_list = self.combine_escape_taxa(leaf_node_list=subtree.root.leaf_nodes(),tc_tree=tree)
+            
+                for taxa in escape_taxa_list:
+                    self.record_escape_taxa(taxa, new_subtree,align)
+                # for leaf_node in subtree.root.leaf_nodes():
+                #
+                #     tc_corr = leaf_node.corr[tree.id]
+                #     tc_corr.exact_match_percentage = new_subtree.root.exact_match_percentage
+                #     self.record_escape_taxa(tc_corr,new_subtree,align)
                 return
             else:
                 # Draw leaf nodes which not in new_subtree
                 escape_taxa = subtree.leaf_set.difference(new_subtree.leaf_set)
-                for leaf_node in subtree.root.leaf_nodes():
-                    if leaf_node.taxon.label not in escape_taxa:
-                        continue
-
-                    tc_corr = leaf_node.corr[tree.id]
-                    tc_corr.exact_match_percentage = new_subtree.root.exact_match_percentage
-                    self.record_escape_taxa(tc_corr, new_subtree,align)
+                target_set = set()
+                for node in subtree.root.leaf_nodes():
+                    if node.taxon.label in escape_taxa:
+                        target_set.add(node)
+
+                escape_taxa_list = self.combine_escape_taxa(leaf_node_list=target_set, tc_tree=tree)
+                self.output.append(escape_taxa_list)
+                    # tc_corr = leaf_node.corr[tree.id]
+                    # tc_corr.exact_match_percentage = new_subtree.root.exact_match_percentage
+                for taxa in escape_taxa_list:
+                    self.record_escape_taxa(taxa, new_subtree,align)
 
         self.check_duplicate_subtree(corresponding_subtree, subtree, new_subtree)
         for leaf_node in corresponding_subtree.leaf_nodes():
             leaf_node.selected = True
 
-
         self.draw_subtree_block(corresponding_subtree, select_tree=TC, new_subtree=new_subtree,
                                 subtree_from_rt=subtree,align=align)
 
+    def combine_escape_taxa(self,tc_tree,leaf_node_list):
+        escape_taxa_list = []
+        taxa_name_list = []
+        for leaf_node in leaf_node_list:
+            inserted = False
+            tc_corr = leaf_node.corr[tc_tree.id]
+            for index,group in enumerate(taxa_name_list):
+                test_taxa_list = group + [tc_corr.taxon.label]
+
+                ancestor = tc_tree.mrca(taxon_labels=test_taxa_list)
+                ancestor_nodes = [node.taxon.label for node in ancestor.leaf_nodes()]
+
+                if set(ancestor_nodes) == set(test_taxa_list):
+                    group.append(tc_corr)
+                    escape_taxa_list[index] = ancestor
+                    inserted = True
+
+            if not inserted:
+                escape_taxa_list.append(tc_corr)
+                taxa_name_list.append([tc_corr.taxon.label])
+
+
+        return escape_taxa_list
     def check_duplicate_subtree(self,corresponding_subtree,subtree,new_subtree):
         if not hasattr(corresponding_subtree, 'subtree') or not corresponding_subtree.subtree:
             corresponding_subtree.subtree = new_subtree
 
         elif hasattr(corresponding_subtree, 'subtree'):
             if type(corresponding_subtree.subtree) is not list and corresponding_subtree.subtree != subtree:
                 corresponding_subtree.duplicate_subtree = True
@@ -914,14 +1048,87 @@
                 corresponding_subtree.subtree = subtree_list
             else:
                 corresponding_subtree.duplicate_subtree = True
                 corresponding_subtree.subtree.append(new_subtree)
 
         corresponding_subtree.selected = True
 
+    def get_layer_index(self,subtree,tmp_layer_block_list,tmp_layer_occupied,align=None,type=None):
+        tmp_layer_block_list[subtree.label] = subtree.block_size  # { 'label' : block-size }
+        tmp_sorted_layer_list = sorted(tmp_layer_block_list, key=lambda x: tmp_layer_block_list[x], reverse=True)
+
+        if type == RT:
+            self.rt_sorted_layer_list = tmp_sorted_layer_list
+        elif type == TC:
+            if align == LEFT:
+                self.tc_left_sorted_layer_list = tmp_sorted_layer_list
+            else:
+                self.tc_right_sorted_layer_list = tmp_sorted_layer_list
+
+        # If no subtree selected
+        if tmp_layer_occupied.count(1) == 0:
+            tmp_layer_occupied[0] = 1
+            return 0
+
+        # If new_subtree is smaller than all existing subtree
+        if all(subtree.block_size <= value for value in tmp_layer_block_list.values()):
+            index = tmp_layer_occupied.index(0)
+            tmp_layer_occupied[index] = 1
+            return index
+
+        # If need to sort multicanvas layer - shift layers in list to the right
+
+        next_index = tmp_layer_occupied.index(0)
+        tmp_layer_occupied[next_index] = 1
+
+        subtree_layer_index = tmp_sorted_layer_list.index(subtree.label)
+        if type == TC:
+            if align == LEFT:
+                next_index += 14
+                subtree_layer_index += 14
+            else:
+                next_index += 7
+                subtree_layer_index += 7
+
+
+        canvas_tmp = Canvas(width=self.width, height=self.height)
+        for i in range(next_index, subtree_layer_index , -1):
+            canvas_tmp.clear()
+            canvas_tmp.draw_image(self[i-1],0,0)
+            self[i].clear()
+            self[i].draw_image(canvas_tmp,0,0)
+
+
+
+
+        index = tmp_sorted_layer_list.index(subtree.label)
+        tmp_layer_occupied[index] = 1
+        return index
+
+    def rearrange_canvas_layer(self, clear_layer_index, type, align):
+        if type == RT:
+            first_layer = 0
+            last_layer = 5
+        elif type == TC:
+            if align == RIGHT:
+                first_layer = 7
+                last_layer = 12
+            else:
+                first_layer = 14
+                last_layer = 19
+
+
+        canvas_tmp = Canvas(width=self.width, height=self.height)
+        for i in range(clear_layer_index, last_layer):
+            canvas_tmp.clear()
+            if i < last_layer - 1:
+                canvas_tmp.draw_image(self[i + 1], 0, 0)
+            self[i].clear()
+            self[i].draw_image(canvas_tmp, 0, 0)
+
     def compare_tc_tree(self,compare_tree=None,compare_between_tc=False):
         self[self.TC_LEFT_LAYER].clear()
         self[self.TC_RIGHT_LAYER].clear()
         self.tc_tree = compare_tree
         self.compare_between_tc = compare_between_tc
         self.last_draw_time = time.time()
         self.reset_subtree_canvas()
@@ -982,14 +1189,15 @@
                     self.draw_missing_taxa_block(align=RIGHT)
 
                     # self.draw_frame(self.right_tree_width, y, width, height, BLACK, layer_index=self.TC_RIGHT_LAYER)
 
             if len(self.adPy.subtree_list) > 0:
                 self.setup_tc_subtree_list(self.tc_tree,RIGHT)
 
+
     def generate_missing_taxa_block_in_tree(self,tree,align):
         if align == RIGHT:
             x = self.width / 2 + PAIRWISE_X_INTERVAL * 2
             end_x = x + MISSING_TAXA_BLOCK_WIDTH
             y = self.right_tree_height + 20
             layer_index = self.TC_RIGHT_LAYER
         else:
```

### Comparing `ADViewpy-0.2a0/ADViewpy/rtCanvas.py` & `ADViewpy-0.3a0/ADViewpy/rtCanvas.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,35 @@
 import time
 
 # Canvas for Reference Tree
 class rtCanvas(MyCanvas):
     # Initial x,y coordinates
     x = 30
     y = 30
-    SUBTREE_COMPARE_LAYER = -3
-    NODE_HOVER_LAYER = -2
-    RT_LAYER = -1
+    SUBTREE_COMPARE_LAYER = -4
+    NODE_HOVER_LAYER = -1
+    RT_LAYER = -3
+    FILTER_NODE_LAYER = -2
 
-    def __init__(self,adPy,width,height,view_support,default_rt=None):
-        super().__init__( 8, width = width, height = height)
+
+    def __init__(self, adPy, width, height, view_support, support_value_range=None,
+                 exact_match_range=None, default_rt=None):
+        super().__init__( 10, width = width, height = height)
         # Layer 7 - reference tree
         # Layer 6 - hover block
         self.adPy = adPy
         self.layer = 8
         self.rt = adPy.rt
         self.view_support = view_support
         self.tree_width = 1
         self.dupletree = None
+        self.support_value_interval = support_value_range
+        self.exact_match_interval = exact_match_range
 
-
+        
         self.layer_block_list = {}
         self.layer_occupied = [0, 0, 0, 0, 0]
         self.subtree_label_used = self.adPy.subtree_label_used
         self.subtree_color_used = self.adPy.subtree_color_used
         self.sorted_layer_list = []
 
         self.node_hover = None
@@ -56,21 +61,19 @@
         self.on_mouse_move(self.mouse_hover)
 
     def setup_section_list(self):
         section_cnt = math.ceil(self.height/ MIN_SECTION_HEIGHT)
 
         for i in range(section_cnt):
             self.section_list.append([])
+
             if self.inner_section:
                 for j in range(3):
                     self.section_list[i].append([])
-            # section_top_border = i * MIN_SECTION_HEIGHT
-            # new_dupletree = DupleTree(self,Point(0,section_top_border),Point(self.width/2,section_top_border +
-            #                                                                  MIN_SECTION_HEIGHT))
-            # self.section_list.append(new_dupletree)
+
 
     # Draw reference tree on rtcanvas
     def draw_rt(self,draw_canvas,node=None,level=0):
 
         if level == 0:
             draw_canvas.fill_style = BLACK
             draw_canvas.font = LEAF_FONT
@@ -123,15 +126,15 @@
             # self.draw_rec(node.pos.x + X_INTERVAL - 2,node.pos.y - NODE_BLOCK_HEIGHT,X_INTERVAL + len(str(node.taxon.label)) * 9,NODE_BLOCK_HEIGHT+2)
 
         else:
             child_nodes = node.child_nodes()
 
             # To determine the midpoint of vertical line connecting multiple children
             first_child = child_nodes[0] if child_nodes else None
-            last_child = child_nodes[self.RT_LAYER] if child_nodes else None
+            last_child = child_nodes[-1] if child_nodes else None
 
             if self.view_support:
                 x = self.x * level
             else:
                 x = RT_X_INTERVAL * level + RT_X_INTERVAL
 
             tmp = first_child.pos.y + last_child.pos.y
@@ -162,14 +165,15 @@
 
             if self.view_support:
                 draw_canvas.fill_style = 'blue'
                 if node.label:
                     draw_canvas.fill_text(node.label, node.pos.x + 3, node.pos.y - 8)
                 draw_canvas.fill_style = BLACK
 
+
             # Testing
             # self.draw_dots(node.pos.x + X_INTERVAL - 4, node.pos.y - X_INTERVAL)
             # self.draw_dots(node.pos.x + X_INTERVAL + 4, node.pos.y )
             # self.draw_rec(node.range_topL.x,node.range_topL.y,8,node.range_botR.y - node.range_topL.y,BEIGE)
 
         # To calculate and record subtree's block size
         if node.parent_node:
@@ -178,30 +182,51 @@
                     node.parent_node.block.topL = node.block.topL
 
                 if node.block.botR.y > node.parent_node.block.botR.y:
                     node.parent_node.block.botR = node.block.botR
             else:
                 node.parent_node.block = Block(node.block.topL,node.block.botR)
 
+        if not node.is_leaf() and self.check_attribute_in_range(node):
+            self.draw_rec(node.pos.x, node.pos.y - RT_X_INTERVAL,RT_X_INTERVAL-2,RT_X_INTERVAL - 2, BEIGE,
+                          layer_index=self.FILTER_NODE_LAYER)
+
 
         node.selected = False
         self.insert_node_section_list(node)
-        # self.dupletree.insert(node=node,point=node.mouse_range.topL)
-        # self.dupletree.insert(node=node, point=node.mouse_range.botR)
-        # self.dupletree.insert(node=node, point=Point(node.mouse_range.botR.x, node.mouse_range.topL.y))
-        # self.dupletree.insert(node=node, point= Point(node.mouse_range.topL.x, node.mouse_range.botR.y))
-        # self.quads.insert(quads.Point(block.topL.x, block.topL.y, data=node))
-        # self.quads.insert(quads.Point(block.topL.x, block.botR.y, data=node))
-        # self.quads.insert(quads.Point(block.botR.x, block.topL.y, data=node))
-        # self.quads.insert(quads.Point(block.botR.x, block.botR.y, data=node))
 
-        # Testing
-        # self.draw_dots(node.pos.x,node.pos.y - X_INTERVAL)
-        # self.draw_dots(node.pos.x + X_INTERVAL, node.pos.y)
-        # self.draw_dots(node.pos.x + X_INTER0L.y,8,node.range_botR.y - node.range_topL.y,BEIGE)
+    def draw_filter_node(self,exact_match_range,support_value_range):
+        self.support_value_interval = support_value_range
+        self.exact_match_interval = exact_match_range
+
+        self[self.FILTER_NODE_LAYER].clear()
+        for node in self.rt.postorder_node_iter():
+            if not node.is_leaf() and self.check_attribute_in_range(node):
+                self.draw_rec(node.pos.x, node.pos.y - RT_X_INTERVAL, RT_X_INTERVAL - 2, RT_X_INTERVAL - 2, BEIGE,
+                              layer_index=self.FILTER_NODE_LAYER)
+
+    def check_attribute_in_range(self,node):
+        exact_match_result = False
+        support_value_result = False
+
+        if self.support_value_interval:
+            if node.support >= self.support_value_interval[0] and node.support <= self.support_value_interval[1]:
+                support_value_result = True
+            else:
+                support_value_result = False
+
+        if self.exact_match_interval:
+            exact_match_percentage = node.exact_match / len(self.adPy.tc) * 100
+
+            if exact_match_percentage >= self.exact_match_interval[0] and exact_match_percentage <= self.exact_match_interval[1]:
+                exact_match_result = True
+            else:
+                exact_match_result = False
+
+        return (exact_match_result and support_value_result)
 
     def insert_node_section_list(self,node):
         top_section_index = math.floor(node.mouse_range.topL.y / MIN_SECTION_HEIGHT)
         bottom_section_index = math.floor(node.mouse_range.botR.y / MIN_SECTION_HEIGHT)
 
         if not self.inner_section:
             if top_section_index == bottom_section_index:
@@ -295,15 +320,15 @@
         # node_selected = self.rt.find_node(lambda node: self.filter_node_selected(node, x,y))
 
         if node_selected:
             self.adPy.select_subtree_from_tree(node_selected)
 
     def mouse_hover(self, x, y):
         current_time = time.time()
-        if current_time - self.last_draw_time > 0.1:
+        if current_time - self.last_draw_time > 0.15:
             self.last_draw_time = current_time
             node_selected = self.filter_node_from_section_list(x, y)
 
             # if (x, y) != self.last_mouse_position:
             #     self.last_mouse_position = (x, y)
 
         else:
@@ -367,17 +392,17 @@
         self[self.NODE_HOVER_LAYER].fill_text("Support : " + support, label_pos , label_y)
         self[self.NODE_HOVER_LAYER].fill_text("Length :  " + str(length), label_pos, label_y + 15)
         self[self.NODE_HOVER_LAYER].fill_text("Exact Match :  " + str(exact_match) + "%", label_pos , label_y + 30)
 
     def draw_hover_block(self):
         if not self.node_hover.is_leaf() and self.view_support:
             self.draw_rec(self.node_hover.pos.x + RT_X_INTERVAL , self.node_hover.pos.y - RT_X_INTERVAL + 2 , RT_X_INTERVAL,
-                          RT_X_INTERVAL - 2, BLACK, layer_index=-2)
+                          RT_X_INTERVAL - 2, BLACK, layer_index=self.NODE_HOVER_LAYER)
         else:
-            self.draw_rec(self.node_hover.pos.x, self.node_hover.pos.y - RT_X_INTERVAL, RT_X_INTERVAL - 2, RT_X_INTERVAL - 2, BLACK, layer_index = -2)
+            self.draw_rec(self.node_hover.pos.x, self.node_hover.pos.y - RT_X_INTERVAL, RT_X_INTERVAL - 2, RT_X_INTERVAL - 2, BLACK, layer_index = self.NODE_HOVER_LAYER)
 
         self[self.NODE_HOVER_LAYER].flush()
 
     def generate_subtree_block(self,node_selected):
         if node_selected.is_leaf():
             rec_x = node_selected.block.topL.x + RT_X_INTERVAL - 5
         else:
```

### Comparing `ADViewpy-0.2a0/ADViewpy/tcCanvas.py` & `ADViewpy-0.3a0/ADViewpy/tcCanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     ad_list = []
     rt_ad = None
 
     # layer -1 for subtree comparison view
     # layer -2 for tree name
     # layer -3 forward for ad
     def __init__(self,adPy,view,ad_per_row=DEFAULT_AD_PER_ROW,width=1100, height=1100,scale=1.0,max_ad=None,
-                 context_level=2,first_ad=None,last_ad=None,tree_id=None,tree_name=None,sort_by=ID,
+                 context_level=2,filter=INCLUDE,first_ad=None,last_ad=None,tree_id=None,tree_name=None,sort_by=ID,
                  escape_taxa_as_context_block=True,show_block_proportional=False,parameter_from_individual_ad=True,
-                 subtree_independent=True,differentiate_inexact_match=True,layer=5,show_tree_name=False):
+                 subtree_independent=True,differentiate_inexact_match=True,layer=5,show_tree_name=False,
+                 compress_escape_taxa=True):
         super().__init__(layer = layer + 4, width = width, height = height)
 
         # Common attribute
         self.AD_LAYER = -3
         self.TREE_NAME_LAYER = -2
         self.COMPARISON_VIEW_LAYER = -1
         self.TREE_SELECTED_BLOCK_LAYER = 0
@@ -32,14 +33,16 @@
         self.scale = scale
         self.max_ad = max_ad
         self.set_tc_canvas_default()
         self.ad_per_row = ad_per_row
         self.context_level = context_level
         self.scale_alter = False
         self.check_result_list = []
+        self.filter_type = filter
+        self.compress_escape_taxa = compress_escape_taxa
 
         self.cluster_agree_rt = None
 
         self.view = view
         self.adPy = adPy
         self.rt = adPy.rt
         self.tc = self.adPy.sort_tc(tc_list=self.adPy.tc, sort_by=sort_by)
@@ -111,35 +114,41 @@
         self.adPy.subtree_list = sorted(self.adPy.subtree_list, key=lambda x: len(x.leaf_set), reverse=True)
 
     def generate_ad_list(self):
         for index, tc_tree in enumerate(self.tc):
             if self.view == AD_INDIVIDUAL:
                 if self.condition_exist and self.check_index_name_fulfill():
                     break
-                result = self.check_condition(index,tc_tree)
+
+                if self.filter_type == INCLUDE:
+                    result = self.check_include_condition(index, tc_tree)
+                else:
+                    result = self.check_exclude_condition(tc_tree)
+
                 if result == CONTINUE:
                     continue
                 elif result == BREAK:
                     break
 
             check_elided = {}
             check_elided['node'] = None
             check_elided['context_level'] = 0
+
             self.construct_ad(tc_tree=tc_tree, level=1, check_elided=check_elided)
 
             self.ad_drawn += 1
 
     def check_index_name_fulfill(self):
         if self.target_tc_tree_index or self.target_tc_tree_name:
             return False
 
         # Condition fulfill, break process
         return True
 
-    def check_condition(self,index,tc_tree):
+    def check_include_condition(self, index, tc_tree):
         if self.first_ad and index < self.first_ad - 1:
             return CONTINUE
         if self.last_ad and index >= self.last_ad:
             return BREAK
         if self.max_ad and self.ad_drawn >= self.max_ad:
             return BREAK
 
@@ -158,14 +167,35 @@
                 self.target_tc_tree_name.remove(tc_tree.name)
                 if len(self.target_tc_tree_name) == 0:
                     self.target_tc_tree_name = None
                 return TRUE
             else:
                 check_tree_index_name = CONTINUE
 
+        return check_tree_index_name
+
+    def check_exclude_condition(self, tc_tree):
+        if self.first_ad and self.last_ad and tc_tree.id >= self.first_ad and tc_tree.id <= self.last_ad:
+            return CONTINUE
+
+        if self.max_ad and self.ad_drawn >= self.max_ad:
+            return BREAK
+
+        check_tree_index_name = TRUE
+        if self.target_tc_tree_index:
+            if tc_tree.id in self.target_tc_tree_index:
+                check_tree_index_name = CONTINUE
+            else:
+                return TRUE
+
+        if self.target_tc_tree_name:
+            if tc_tree.name in self.target_tc_tree_name:
+                check_tree_index_name = CONTINUE
+            else:
+                return TRUE
 
         return check_tree_index_name
 
     def reset_tc_canvas(self):
         # for layer in range(0,self.layer):
         self[self.AD_LAYER].clear()
         self.set_tc_canvas_default()
@@ -184,30 +214,29 @@
             self.height = 10
 
     def construct_individual_ad_canvas(self):
 
         result = self.preprocess_ad_tree(self.ad_list)
 
         if result == SPACE_INSUFFICIENT:
-            self.adjust_display_area()
+            self.adjust_display()
             return
 
         self.check_canvas_height(self.ad_list)
 
         if self.scale_alter:
             self.display_content_exceed_error()
             # self.height += (self.height * self.scale) * 2
 
         self.cluster_from_ad_list()
         self.generate_topology_canvas()
 
         # self.draw_ad_tree_rec(self.ad_list)
 
     def construct_ad(self,tc_tree,construct_rt=False,tc_node=None,current_ad_node=None,level=0,nested_subtree=None,nested_ad=None,check_elided={},nested_subtree_duplicate=False):
-
         if tc_node is None and current_ad_node is None: # When start from root
             tc_node = tc_tree.seed_node
             tc_node.index = 0
 
             ad = AD_Tree(id=tc_tree.id,tc_tree=tc_tree,tc_canvas=self)  # Create a new AD_Tree which belong to
             tc_tree.ad_tree = ad
             # current tc_tree
@@ -231,23 +260,14 @@
                 result = self.check_relation(subtree=subtree,node=tc_node,tree_index = tc_tree.id,nested_subtree_duplicate=nested_subtree_duplicate)
                 if result == SUBTREE_ROOT:
                     self.generate_block_by_result(result=result, subtree=subtree, tc_tree=tc_tree, tc_node=tc_node,
                                                   current_ad_node=current_ad_node , level=level,nested_subtree=nested_subtree, nested_ad=nested_ad,check_elided=check_elided,nested_subtree_duplicate=nested_subtree_duplicate)
 
                     return
 
-            # if result == NON_DESCENDANT:
-            #     self.generate_block_by_result(result=result, subtree=None, tc_tree=tc_tree, tc_node=tc_node,
-            #                                   current_ad_node=current_ad_node, level=level,
-            #                                   nested_subtree=nested_subtree, nested_ad=nested_ad,
-            #                                   check_elided=check_elided,
-            #                                   nested_subtree_duplicate=nested_subtree_duplicate)
-            #     return
-
-
         result_list = {}
 
         for index,child in enumerate(tc_node.child_node_iter()):
             # print("============")
             # print("Child:" ,end="")
             # print(child)
             child.index = index
@@ -258,30 +278,25 @@
 
                 result_tmp = self.check_relation(subtree=subtree,node=child,tree_index = tc_tree.id,nested_subtree_duplicate=nested_subtree_duplicate)
 
                 if result_tmp < result:
                     result = result_tmp
 
                 if result == SUBTREE_ROOT or result == INDEPENDENT_LEAF:
-                    # subtree_prior = 5 - SUBTREE_LABEL_LIST.index(subtree.label)
-                    # print(f"subtree_prior = {subtree_prior}")
-                    # result -= subtree_prior
-                    # print(f"result = {result}")
                     break
 
             result_list[child] = [result,subtree]
             if tc_tree.id > 0:
                 self.check_result_list.append(result_list[child])
 
         # Sort by result
         sorted_list = dict(sorted(result_list.items(), key=lambda item: item[1][0]))
         check_result = { value[0] for value in sorted_list.values() }
 
-
-        if len(check_result) == 1:
+        if len(check_result) == 1 or 0 in check_result or 1 in check_result:
             # Elided stop here
             if check_elided['node'] and check_elided['context_level'] >= self.context_level:
                 ori_child = check_elided['node'].children.pop()
 
                 parent = check_elided['node']
                 current_ad_node.child_index = ori_child.child_index
                 current_ad_node.x_level = ori_child.x_level + 1
@@ -289,65 +304,75 @@
                 check_elided['node'] = None
                 check_elided['context_level'] = 0
 
                 if nested_ad:
                     nested_ad.insert_node(parent, current_ad_node)
                 else:
                     self.ad_constructing.insert_node(parent, current_ad_node)
+            else:
+                check_elided['node'] = None
+                check_elided['context_level'] = 0
 
         for node,result in sorted_list.items():
             self.generate_block_by_result(result=result[0],subtree=result[1],tc_tree=tc_tree,tc_node=node,current_ad_node=current_ad_node,level=level,nested_subtree=nested_subtree,nested_ad=nested_ad,check_elided=check_elided,nested_subtree_duplicate=nested_subtree_duplicate)
 
+            # self.ad_constructing.plot_tree()
+            # print(check_elided)
 
     def generate_block_by_result(self,result,subtree,tc_tree,tc_node=None,current_ad_node=None,level=0,nested_subtree=None,nested_ad=None,check_elided={},nested_subtree_duplicate=False):
         if result == INDEPENDENT_LEAF:
-            # print("INDEPENDENT_LEAF")
+            # print(f"result {result}")
             # if self.escape_taxa_as_context_block and not nested_subtree_duplicate:
             #     return
 
             # print("INDEPENDENT_LEAF")
             # print("Subtree:" + subtree.label)
             # width,height,subtree,ad_tree,type,topL=None, botR=None
             independent_leaf_block = self.individual_block(subtree=subtree, type=INDIVIDUAL_LEAF_BLOCK)
             independent_leaf_block.color = subtree.color
             independent_leaf_block.root = tc_node
-            independent_leaf_block.taxa_list.add(tc_node.taxon.label)
+            if tc_node.taxon:
+                independent_leaf_block.taxa_list.add(tc_node.taxon.label)
             independent_leaf_block.subtree_taxa_count = 1
             new_ad_node = AD_Node(node_or_block=independent_leaf_block, x_level=level, type=LEAF,
                                         child_index=tc_node.index,type_prior=result)
 
 
-            if not self.escape_taxa_as_context_block and check_elided['node'] and check_elided['context_level'] >=self.context_level:
-                ori_child = check_elided['node'].children.pop()
-                current_ad_node.child_index = ori_child.child_index
-                if nested_ad:
-                    nested_ad.insert_node(check_elided['node'], current_ad_node)
-                else:
-                    self.ad_constructing.insert_node(check_elided['node'], current_ad_node)
+            if not self.escape_taxa_as_context_block:
+                if check_elided['node'] and check_elided['context_level'] >= self.context_level:
 
-                current_ad_node.x_level = ori_child.x_level + 1
-                new_ad_node.x_level = current_ad_node.x_level + 1
-                current_ad_node.is_elided = True
-                check_elided['node'] = None
-                check_elided['context_level'] = 0
+                    ori_child = check_elided['node'].children.pop()
+                    parent = check_elided['node']
 
-            elif not self.escape_taxa_as_context_block:
-                check_elided['node'] = None
-                check_elided['context_level'] = 0
+                    current_ad_node.child_index = ori_child.child_index
+                    if nested_ad:
+                        nested_ad.insert_node(parent, current_ad_node)
+                    else:
+                        self.ad_constructing.insert_node(parent, current_ad_node)
+
+                    current_ad_node.x_level = ori_child.x_level + 1
+                    new_ad_node.x_level = current_ad_node.x_level + 1
+                    current_ad_node.is_elided = True
+                    check_elided['node'] = None
+                    check_elided['context_level'] = 0
+
+                else:
+                    check_elided['node'] = None
+                    check_elided['context_level'] = 0
 
             if nested_ad:
                 nested_ad.insert_node(current_ad_node, new_ad_node)
             else:
                 self.ad_constructing.insert_node(current_ad_node, new_ad_node)
 
 
             # current_ad_node.children.append(new_ad_node)
 
         elif result == SUBTREE_ROOT or result == DUPLICATE_SUBTREE_ROOT:
-            # print("SUBTREE_ROOT")
+            # print(f"result {result}")
             # taxa_list = all taxa under corresponding subtree
             # subtree_taxa_count = taxa of reference subtree exist in this corresponding subtree
             # if corresponding subtree exactly same as reference subtree
 
             if result == DUPLICATE_SUBTREE_ROOT:
                 result = self.check_subtree_combine(tc_node, tree_index=tc_tree.id)
                 subtree_block = self.ad_subtree_block(subtree=self.duplicate_subtree,subtree_duplicate=True)
@@ -367,16 +392,14 @@
                         subtree_block.exact_match.append(True)
                     else:
                         subtree_block.exact_match.append(False)
 
                 for count in subtree_block.duplicate_subtree_taxa_count:
                     subtree_block.subtree_taxa_count += count
 
-
-
             else:
                 subtree_block = self.ad_subtree_block(subtree=subtree,subtree_duplicate=False)
                 subtree.check_and_set_topology(tc_node,tc_tree.id)
 
                 subtree_block.color = subtree.color
                 subtree_block.taxa_list = {leaf.taxon.label for leaf in tc_node.leaf_nodes()}
                 subtree_block.subtree_taxa_count = len(subtree_block.taxa_list.intersection(subtree.leaf_set))
@@ -388,17 +411,17 @@
 
             subtree_block.taxa_list = {leaf.taxon.label for leaf in tc_node.leaf_nodes()}
             subtree_block.root = tc_node
 
             new_ad_node = AD_Node(node_or_block=subtree_block, x_level=level, type=LEAF,
                                         child_index=tc_node.index,type_prior=result)
 
+
             if check_elided['node'] and check_elided['context_level'] >= self.context_level:
                 ori_child = check_elided['node'].children.pop()
-
                 parent = check_elided['node']
                 if not subtree_block.exact_match and not self.escape_taxa_as_context_block:
                     current_ad_node.child_index = ori_child.child_index
                     if nested_ad:
                         nested_ad.insert_node(parent, current_ad_node)
                     else:
                         self.ad_constructing.insert_node(parent, current_ad_node)
@@ -419,24 +442,23 @@
                     subtree_block.is_elided = True
                     if nested_ad:
                         nested_ad.insert_node(parent, new_ad_node)
                     else:
                         self.ad_constructing.insert_node(parent, new_ad_node)
 
             else:
+
                 check_elided['node'] = None
                 check_elided['context_level'] = 0
+
                 if nested_ad:
                     nested_ad.insert_node(current_ad_node, new_ad_node)
                 else:
                     self.ad_constructing.insert_node(current_ad_node, new_ad_node)
 
-
-            # current_ad_node.children.append(new_ad_node)
-
             if tc_node.is_leaf():
                 return
 
             # self.ad_constructing.plot_tree()
 
             # Check nested subtree/block
             for check_subtree in self.adPy.subtree_list:
@@ -486,15 +508,15 @@
             # print("IS_DESCENDANT")
             new_ad_node = AD_Node(node_or_block=tc_node, x_level=level, type=INTERNAL,
                                         child_index=tc_node.index,type_prior=result)
 
             if check_elided['node'] != None:
                 check_elided['context_level'] += 1
             else:
-                check_elided['node'] = new_ad_node
+                check_elided['node'] = current_ad_node
 
 
             if nested_ad:
                 nested_ad.insert_node(current_ad_node, new_ad_node)
             else:
                 self.ad_constructing.insert_node(current_ad_node, new_ad_node)
             # current_ad_node.children.append(new_ad_node)
@@ -531,32 +553,37 @@
                 return DUPLICATE_SUBTREE_ROOT
             else:
                 return SUBTREE_ROOT
 
         # If node from tc is target leaf node in this subtree
         if node.is_leaf():
             if node.taxon.label in subtree.leaf_set:
-                return INDEPENDENT_LEAF
+                if not self.escape_taxa_as_context_block:
+                    return INDEPENDENT_LEAF
 
         if self.check_leaf_node_descendant(subtree,node) == IS_DESCENDANT:
             if self.escape_taxa_as_context_block:
                 if nested_subtree_duplicate or self.check_subtree_in_descendant(node,tree_index=tree_index):
                     return IS_DESCENDANT
             else:
+                if self.compress_escape_taxa:
+                    leaf_nodes = {leaf.taxon.label for leaf in node.leaf_nodes()}
+                    if leaf_nodes.issubset(subtree.leaf_set):
+                        return INDEPENDENT_LEAF
+
                 return IS_DESCENDANT
 
         # If current branch has no target taxa
         return NON_DESCENDANT
 
     def check_leaf_node_descendant(self,subtree,node):
         leaf_nodes = {leaf.taxon.label for leaf in node.leaf_nodes()}
 
         if leaf_nodes.intersection(subtree.leaf_set):
             return IS_DESCENDANT
-
         else:
             return False
 
     # Check if node descendant has subtree
     def check_subtree_in_descendant(self,node,tree_index):
         for subtree in self.adPy.subtree_list:
             if self.adPy.is_descendant(parent_node=node,child_node=subtree.root.corr[tree_index]):
@@ -685,15 +712,15 @@
                 # print("nested_block_height = " + str(self.nested_block_height))
                 # print("block_minimum_height = " + str(self.block_minimum_height))
 
                 sufficient_space = self.adjust_ad_block(ad_tree)
                 # print("Sufficient space = " + str(sufficient_space))
         return SPACE_SUFFICIENT
 
-    def adjust_display_area(self):
+    def adjust_display(self):
         self.scale_alter = True
         self.scale += 0.1
         self.reset_tc_canvas()
         if self.view == AD_INDIVIDUAL:
             self.construct_individual_ad_canvas()
         else:
             self.construct_cluster_ad_canvas()
@@ -804,15 +831,15 @@
             width = ad_tree.botR.x - ad_tree.x * self.scale - x
             ad_tree.missing_taxa_block = Block(Point(x,y),Point(x+width,y+self.missing_taxa_height))
 
             self.draw_missing_taxa_block(ad_tree)
 
     def draw_ad_tree(self,ad_tree=None,canvas=None,cluster=False):
         with hold_canvas(self):
-            ad_tree.y *= self.scale
+            ad_tree.y = 8 * self.scale
             for node in ad_tree.traverse_postorder():
                 if canvas and not ad_tree.is_nested:
                     if cluster:
                         ad_topL_x = 5
                         ad_topL_y = CLUSTER_NUMBER_BAR_HEIGHT + DEFAULT_PADDING_BETWEEN_BLOCK * 2 + 5
 
                         ad_tree.topL.x = ad_topL_x
@@ -1059,15 +1086,14 @@
         self.draw_solid_line(Point(x, first_child.branch_head.y), Point(x, last_child.branch_head.y), BLACK,
                              layer_index,canvas=canvas)
 
         if node.type == ROOT:
             # Draw horizontal branch
             self.draw_solid_line(node.branch_head, node.branch_tail, BLACK, layer_index,canvas=canvas)
 
-        # Draw children's branches
         for child in node.children:
             if child.is_elided:
                 self.draw_elided_branch(child.branch_head, child.branch_tail, BLACK, layer_index,canvas=canvas)
             else:
                 self.draw_solid_line(child.branch_head, child.branch_tail, BLACK, layer_index,canvas=canvas)
 
     def write_tree_name(self,ad_tree,extend = False,x=None):
@@ -1315,15 +1341,15 @@
 
         # Convert topology_list to ad_list
         self.topology_list_to_ad_list()
 
         result = self.preprocess_ad_tree(self.cluster_ad_list)
 
         if result == SPACE_INSUFFICIENT:
-            self.adjust_display_area()
+            self.adjust_display()
             return
 
         self.check_canvas_height(self.cluster_ad_list)
 
         if self.scale_alter:
             self.display_content_exceed_error()
```

### Comparing `ADViewpy-0.2a0/ADViewpy/treeDistributionView.py` & `ADViewpy-0.3a0/ADViewpy/treeDistributionView.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,16 +409,16 @@
         nodes = self.segment_button_clicked.metadata.get('nodes_list')
         rt_canvas.draw_subtree_compare_nodes(nodes)
 
         self.rt_subtree_canvas_tmp = Canvas(width = rt_canvas.width,height = rt_canvas.height,sync_image_data=True)
         subtree_layer = rt_canvas.sorted_layer_list.index(self.subtree_chosen.label)
 
         self.rt_subtree_canvas_tmp.draw_image(rt_canvas[subtree_layer], 0, 0)
-        self.rt_subtree_canvas_tmp.draw_image(rt_canvas[-1],0,0)
         self.rt_subtree_canvas_tmp.draw_image(rt_canvas[-3],0,0)
+        self.rt_subtree_canvas_tmp.draw_image(rt_canvas[-4],0,0)
 
         block = self.subtree_chosen.block
         self.rt_subtree_block_canvas = Canvas(width=block.width, height=block.height)
         self.rt_subtree_block_vbox = widgets.VBox(children=[self.rt_subtree_block_canvas])
 
         self.rt_subtree_canvas_tmp.observe(self.crop_canvas, "image_data")
```

### Comparing `ADViewpy-0.2a0/ADViewpy.egg-info/PKG-INFO` & `ADViewpy-0.3a0/ADViewpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.2a0
+Version: 0.3a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.2a0/PKG-INFO` & `ADViewpy-0.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.2a0
+Version: 0.3a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.2a0/README.md` & `ADViewpy-0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.2a0/pyproject.toml` & `ADViewpy-0.3a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2241 4456 6965 7770 7922 0d0a 7665  = "ADViewpy"..ve
-00000020: 7273 696f 6e20 3d20 2730 2e32 2e61 6c70  rsion = '0.2.alp
+00000020: 7273 696f 6e20 3d20 2730 2e33 2e61 6c70  rsion = '0.3.alp
 00000030: 6861 270d 0a64 6573 6372 6970 7469 6f6e  ha'..description
 00000040: 203d 2022 4144 5669 6577 7079 2069 7320   = "ADViewpy is 
 00000050: 5079 7468 6f6e 204c 6962 7261 7279 2074  Python Library t
 00000060: 6f20 7669 7375 616c 6c79 2063 6f6d 7061  o visually compa
 00000070: 7265 2070 6879 6c6f 6765 6e65 7469 6320  re phylogenetic 
 00000080: 7472 6565 7322 0d0a 7265 6164 6d65 203d  trees"..readme =
 00000090: 2022 5245 4144 4d45 2e6d 6422 0d0a 6465   "README.md"..de
```

### Comparing `ADViewpy-0.2a0/setup.py` & `ADViewpy-0.3a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.2.alpha'
+VERSION = '0.3.alpha'
 DESCRIPTION = ('ADViewpy is Python Library to visually compare phylogenetic trees')
 LONG_DESCRIPTION = 'ADViewpy is Python Library to visually compare phylogenetic trees, utilizing Aggregated Dendrogram for phylogenetic tree visualization. '
 
 
 setup(
     name="ADViewpy",
     version=VERSION,
```

