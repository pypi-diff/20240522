# Comparing `tmp/procedure_data_tool-0.0.6.tar.gz` & `tmp/procedure_data_tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procedure_data_tool-0.0.6.tar", last modified: Wed May 15 22:14:27 2024, max compression
+gzip compressed data, was "procedure_data_tool-0.0.7.tar", last modified: Tue May 21 23:20:04 2024, max compression
```

## Comparing `procedure_data_tool-0.0.6.tar` & `procedure_data_tool-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.392218 procedure_data_tool-0.0.6/
--rw-rw-rw-   0        0        0        0 2024-05-09 22:58:17.000000 procedure_data_tool-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       54 2024-05-15 14:25:33.000000 procedure_data_tool-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2024-05-15 22:14:27.392218 procedure_data_tool-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:28.000000 procedure_data_tool-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.360553 procedure_data_tool-0.0.6/procedure_data_tool/
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.6/procedure_data_tool/__init__.py
--rw-rw-rw-   0        0        0     5996 2024-05-15 21:17:11.000000 procedure_data_tool-0.0.6/procedure_data_tool/main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.391088 procedure_data_tool-0.0.6/procedure_data_tool/utils/
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/__init__.py
--rw-rw-rw-   0        0        0     4641 2024-05-15 21:42:42.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/docwriter.py
--rw-rw-rw-   0        0        0     2693 2024-05-15 18:45:51.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/excelData.py
--rw-rw-rw-   0        0        0     1054 2024-05-15 21:25:54.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/graph.py
--rw-rw-rw-   0        0        0     2764 2024-05-15 21:29:01.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/node.py
--rw-rw-rw-   0        0        0      531 2024-05-15 14:27:17.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/pit.py
--rw-rw-rw-   0        0        0      504 2024-05-15 21:28:27.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/pump.py
--rw-rw-rw-   0        0        0      479 2024-05-15 22:00:26.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/split.py
--rw-rw-rw-   0        0        0      601 2024-05-15 21:28:41.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/tankreturn.py
--rw-rw-rw-   0        0        0      497 2024-05-15 15:35:12.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/valve.py
--rw-rw-rw-   0        0        0      606 2024-05-15 21:31:22.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/valve2.py
--rw-rw-rw-   0        0        0     1171 2024-05-15 22:09:15.000000 procedure_data_tool-0.0.6/procedure_data_tool/utils/valve3.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:14:27.372393 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-15 22:14:27.000000 procedure_data_tool-0.0.6/procedure_data_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-15 22:14:27.393309 procedure_data_tool-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-05-15 20:49:25.000000 procedure_data_tool-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:20:04.954338 procedure_data_tool-0.0.7/
+-rw-rw-rw-   0        0        0        0 2024-05-09 22:58:17.000000 procedure_data_tool-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       54 2024-05-15 14:25:33.000000 procedure_data_tool-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2024-05-21 23:20:04.954338 procedure_data_tool-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:28.000000 procedure_data_tool-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 23:20:04.924311 procedure_data_tool-0.0.7/procedure_data_tool/
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.7/procedure_data_tool/__init__.py
+-rw-rw-rw-   0        0        0     5549 2024-05-21 23:18:41.000000 procedure_data_tool-0.0.7/procedure_data_tool/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:20:04.953338 procedure_data_tool-0.0.7/procedure_data_tool/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-21 18:16:34.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/docwriter.py
+-rw-rw-rw-   0        0        0     2693 2024-05-15 18:45:51.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/excelData.py
+-rw-rw-rw-   0        0        0      915 2024-05-21 21:48:09.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/graph.py
+-rw-rw-rw-   0        0        0     2893 2024-05-21 23:10:52.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/node.py
+-rw-rw-rw-   0        0        0      595 2024-05-21 17:51:35.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/pit.py
+-rw-rw-rw-   0        0        0      504 2024-05-21 23:10:52.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/pump.py
+-rw-rw-rw-   0        0        0      479 2024-05-15 22:00:26.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/split.py
+-rw-rw-rw-   0        0        0      601 2024-05-15 21:28:41.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/tankreturn.py
+-rw-rw-rw-   0        0        0      497 2024-05-15 15:35:12.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/valve.py
+-rw-rw-rw-   0        0        0      654 2024-05-21 23:10:52.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/valve2.py
+-rw-rw-rw-   0        0        0     1934 2024-05-21 23:10:52.000000 procedure_data_tool-0.0.7/procedure_data_tool/utils/valve3.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:20:04.936249 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-21 23:20:04.000000 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2024-05-21 23:20:04.000000 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:20:04.000000 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-21 23:20:04.000000 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-05-21 23:20:04.000000 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 23:20:04.000000 procedure_data_tool-0.0.7/procedure_data_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-21 23:20:04.955338 procedure_data_tool-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-05-21 23:19:47.000000 procedure_data_tool-0.0.7/setup.py
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/main.py` & `procedure_data_tool-0.0.7/procedure_data_tool/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,51 +3,56 @@
 import procedure_data_tool.utils.graph as gr
 import tkinter as tk
 from tkinter import messagebox
 from tkinter import filedialog
 
 import os
 
+def find_dvi(route):
+    for element in route:
+        element.setPosition(route)
+        element.findDVI(route)
+    return route
+
 def find_routes(source, destination, alternatives = 1):
     src = source.get()
     dst = destination.get()
     alts = 1
     try:
         alts = int(alternatives)
     except ValueError:
         messagebox.showwarning("Warning", "Valid number of alternatives not specified, showing shortest route available.")
     writer = DocWriter(src + " to " + dst + " draft procedure data:")
-    #route is found here:
     routes = components[src].routesTo(components[dst], alts)
     #change this to use a selected route from a list of route options instead!
-    gr.makeGraph(components, routes[0])
     for route in routes:
-        for i in range(1,len(route)-2):
-            route[i].setPosition(route)
-        writer.buildDocument(route,pits)
+        full_route = find_dvi(route)
+        writer.buildDocument(full_route,pits)
+    gr.makeGraph(components, routes[0])
     filename = src +"_to_"+ dst + ".docx"
     writer.save(filename)
     os.system(f'start {filename}')
     
 
 def src_filter(*args):
     query = src_entry.get().lower() 
     src_dropdown['menu'].delete(0, tk.END)
-    for node in nodes:
-        # if query in node.lower() and (components[node].in_tank or select_from_all):
-        if query in node.lower():
-            src_dropdown['menu'].add_command(label=node, command=tk._setit(source, node))
+    for node in displayed_nodes:
+        if node:
+            if (query in node.lower() and (components[node].in_tank or show_all.get())):
+                src_dropdown['menu'].add_command(label=node, command=tk._setit(source, node))
+
 
 def dst_filter(*args):
     query = dst_entry.get().lower() 
     dst_dropdown['menu'].delete(0, tk.END)
-    for node in nodes:
-        # if query in node.lower() and (components[node].in_tank or select_from_all):
-        if query in node.lower():
-            dst_dropdown['menu'].add_command(label=node, command=tk._setit(destination, node))
+    for node in displayed_nodes:
+        if node:
+            if (query in node.lower() and (components[node].in_tank or show_all.get())):
+                dst_dropdown['menu'].add_command(label=node, command=tk._setit(destination, node))
 
 def browse_file(*args):
     filename = filedialog.askopenfilename(defaultextension="xlsx", title = "Select Procedure Data Excel file")
     return filename
 
 def load_new_file(*args):
     new_file_path = None
@@ -77,79 +82,67 @@
     global header_message 
     header_message = tk.StringVar()
     header_message.set("Using data from: "+ file_path)
     label3 = tk.Label(window, textvariable = header_message, wraplength=400, anchor="w")
     label3.grid(row = 0, columnspan=3, rowspan=1, padx=10, pady=20,sticky = "w")
 
     file_button = tk.Button(window, text= "Use a different file", command=lambda: load_new_file())
-    file_button.grid(row = 0, column = 4, padx= 10)
+    file_button.grid(row = 0, column = 3, padx= 10)
+
+    global displayed_nodes 
+    displayed_nodes = components.keys()
 
     def toggle_boolean(*args):
-        if select_from_all:
-            nodes = components.keys()
-            for node in nodes:
-                # dst_dropdown['menu'].delete(0, tk.END)
-                src_dropdown['menu'].add_command(label=node, command=tk._setit(source, node))
-                dst_dropdown['menu'].add_command(label=node, command=tk._setit(destination, node))
-        else:
-            src_filter()
-            dst_filter()
-
-    items_to_tank = set()
-    for item in components.keys():
-        if components[item].in_tank:
-            items_to_tank.add(item)
-    
-    global nodes 
-    nodes = items_to_tank
+        src_filter()
+        dst_filter()
 
     label0 = tk.Label(window, text="Select transfer origin:")
     label0.grid(row=2, column= 0, pady = 2, padx=10,sticky = "w")
 
     global source
     source = tk.StringVar(window)
     global src_dropdown
-    src_dropdown = tk.OptionMenu(window, source, *nodes)
+    src_dropdown = tk.OptionMenu(window, source, *displayed_nodes)
     src_dropdown.grid(row=2, column= 2, pady=2)
     global src_entry
     src_entry = tk.Entry(window)
     src_entry.grid(row=2, column= 1, pady=5, padx=4, sticky="w")
 
     label1 = tk.Label(window, text="Select transfer destination:")
     label1.grid(row=3, column= 0, pady = 2, padx=10, sticky = "w")
 
     global destination
     destination = tk.StringVar(window)
     global dst_dropdown
-    dst_dropdown = tk.OptionMenu(window, destination, *nodes)
+    dst_dropdown = tk.OptionMenu(window, destination, *displayed_nodes)
     dst_dropdown.grid(row=3, column= 2, pady=2)
     global dst_entry
     dst_entry = tk.Entry(window)
     dst_entry.grid(row=3, column= 1, pady=5, padx=4, sticky="w")
 
-    global select_from_all
-    select_from_all = tk.BooleanVar()
-    select_from_all.set(False)
+    global show_all
+    show_all = tk.BooleanVar()
+    show_all.set(False)
 
-    checkbox = tk.Checkbutton(window, text="Show valves", variable=select_from_all, command = toggle_boolean)
-    checkbox.grid(row=2, column=4)
+    checkbox = tk.Checkbutton(window, text="Include valves", variable=show_all, command = toggle_boolean)
+    checkbox.grid(row=2, column=3)
 
     label2 = tk.Label(window, text="Number of route alternatives:")
     label2.grid(row=5, column= 0, pady = 5, padx=10, sticky = "w")
 
     global alternatives 
     alternatives = tk.Entry(window, width= 7, relief="groove")
     alternatives.insert(0, "1") 
     alternatives.grid(row=5, column= 1, columnspan=1, padx=4, pady=2, sticky="w")
    
-    find_routes_button = tk.Button(window, text="Find routes", command=lambda: find_routes(source, destination, alternatives.get()))
-    find_routes_button.grid(row=5, column= 4, padx = 10, pady=15)
+    find_routes_button = tk.Button(window, text="Find routes!", command=lambda: find_routes(source, destination, alternatives.get()))
+    find_routes_button.grid(row=5, column= 3, padx = 10, pady=15)
 
     src_entry.bind("<KeyRelease>", src_filter)
     dst_entry.bind("<KeyRelease>", dst_filter)
+    src_filter()
+    dst_filter()
 
     window.mainloop()
 
 if __name__== '__main__':   
     main()
-
-# TO DO: FIGURE OUT DVI, FIGURE OUT SPLITS NECESSARY??
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/docwriter.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/docwriter.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,79 +29,82 @@
         prompt.font.size = Pt(11)
         return paragraph
 
     def save(self, filename= "PrintedRoute.docx"):
         self.doc.save(filename)
 
     def buildDocument(self, route, pits):
-        route_list = self.makeSection("Valves in Route (reference only): ", "DVI Credited YES/NO/Position dependent")
         used_pits = OrderedDict()
         used_jumpers = OrderedDict()
         for node in route:
             if node.pit in pits:
-                used_pits[node.pit] = None
+                used_pits[node.pit] = pits[node.pit]
             if node.onJumper:
                 jumper = (node.pit, node.jumper)
                 used_jumpers[jumper] = None
+            used_pits[node.pit].add_node(node)
+        route_list = self.makeSection("Valves in Route (reference only): ", "DVI Credited YES/NO/POSition dependent")
+        for node in route:
             if node.show:
                 route_list.add_run("\n")
                 route_list.add_run(node.EIN())
-                route_list.add_run("\t")
-                route_list.add_run(node.dvi_credited)
-        
         heaterEINs = self.makeSection("Section 5.5.3 heaters: " ,"Replace existing data with the following:")
-        for pit in used_pits:
-            for heater in pits[pit].heaters:
+        for pit in used_pits.values():
+            for heater in pit.heaters:
                 heaterEINs.add_run("\n")      
                 heaterEINs.add_run(heater)
                 heaterEINs.add_run("\t \t")
-                heaterEINs.add_run(pits[pit].nacePMID)
-        
-        pits579 = self.makeSection("Steps 5.17.9: ","Replace existing data with the following:")
-        for pit in used_pits:
-            pits579.add_run("\n")
-            pits579.add_run(pits[pit].label)
+                heaterEINs.add_run(pit.nacePMID)
+        pits5179 = self.makeSection("Steps 5.17.9: ","Replace existing data with the following:")
+        for pit in used_pits.values():
+            pits5179.add_run("\n")
+            pits5179.add_run(pit.label)
         checklist1 = self.makeSection("Checklist 1: ","Replace list with:")
         for jumper in used_jumpers:
             checklist1.add_run("\n")
             checklist1.add_run(jumper[0])
-            checklist1.add_run("\t \t")
+            checklist1.add_run("\t \t \t")
             checklist1.add_run("Jumper: ").font.bold = True
             checklist1.add_run(jumper[1])
-        checklist3 = self.makeSection("Checklist 3:","")
-        checklist4 = self.makeSection("Checklist 4:","")
-        checklist5 = self.makeSection("Checklist 5:","")
-        checklist6 = self.makeSection("Checklist 6:","")
+        checklist3 = self.makeSection("*IN DEVELOPMENT* Checklist 3: Transfer Valving","")
+        for pit in used_pits.values():
+            checklist3.add_run("\n")
+            checklist3.add_run(pit.nace[0:6]).bold = True
+            checklist3.add_run(" Tank Farm").bold = True
+            for node in pit.nodes:
+                if (type(node) == Valve3 or type(node) == Valve2 ):
+                    checklist3.add_run("\n")
+                    checklist3.add_run(node.EIN())
+                    checklist3.add_run("\t \t")
+                    checklist3.add_run(node.position)
+            checklist3.add_run("\n")
+            checklist3.add_run("Confirm open route: ").bold = True
+            checklist3.add_run(pit.nace).bold = True
+            checklist3.add_run("\n")
+        checklist4 = self.makeSection("Checklist 4: Checklist 4 - Flush Transfer Route to Transfer Pump Valving","")
+        checklist5 = self.makeSection("Checklist 5: Checklist 4 - Flush Transfer Route to Receiving Tank Valving","")
+        checklist6 = self.makeSection("Checklist 6: Return to Transfer Valving","")
         checklist7LD = self.makeSection("Checklist 7 - Tank pit/Structure Leak Detection")
         checklist7TF = self.makeSection("Checklist 7 - TFSPS Temperature Equipment Checks")
-        for pit in used_pits:
-            for tfsps , pmid in zip(pits[pit].tfsps,pits[pit].tfsps_pmid):
+        for pit in used_pits.values():
+            for tfsps , pmid in zip(pit.tfsps,pit.tfsps_pmid):
                 checklist7TF.add_run("\n")
                 checklist7TF.add_run(tfsps)
                 checklist7TF.add_run("\t \t")
                 checklist7TF.add_run(pmid)
-
         checklist7D = self.makeSection("Checklist 7 - Drain Seal Assemblies:")
-        for pit in used_pits:
+        for pit in used_pits.values():
             checklist7D.add_run("\n")
-            checklist7D.add_run(pits[pit].label)
+            checklist7D.add_run(pit.label)
             checklist7D.add_run(" ")
-            checklist7D.add_run(pits[pit].drain)
+            checklist7D.add_run(pit.drain)
             checklist7D.add_run("\t \t")
-            checklist7D.add_run(pits[pit].drainSealPos)
-
+            checklist7D.add_run(pit.drainSealPos)
         checklist7N = self.makeSection("Checklist 7 - NACE Inspection:")
-        for pit in used_pits:
+        for pit in used_pits.values():
             checklist7N.add_run("\n")
-            checklist7N.add_run(pits[pit].nace)
+            checklist7N.add_run(pit.nace)
             checklist7N.add_run("\t \t")
-            checklist7N.add_run(pits[pit].nacePMID)
+            checklist7N.add_run(pit.nacePMID)
 
-        dviBlockTest = self.makeSection("Test: ", "(Valve Positions Test)")
-        for i in range(1,len(route)-2):
-            if (type(route[i]) == Valve3 or type(route[i]) == Valve2 ):
-                dviBlockTest.add_run("\n")
-                dviBlockTest.add_run(route[i].EIN())
-                dviBlockTest.add_run("\t \t")
-                dviBlockTest.add_run(route[i].position)
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/excelData.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/excelData.py`

 * *Files identical despite different names*

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/graph.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,13 @@
     # for key, value in components.items():
     #     if key:
     #         G.add_node(key)
     #         for connection in value.connections:
     #             G.add_edge(key, connection.ein)
 
     for node in G:
-        color_map.append(inventory[node].color)
+        color_map.append(inventory[node].getColor())
 
     pos = nx.planar_layout(G)  # Position nodes using the Fruchterman-Reingold force-directed algorithm
-    # nx.draw(G, pos, with_labels=True, node_size=80, node_color="skyblue", font_size=9, font_color='black', edge_color='gray', linewidths=10)
     nx.draw(G, pos, with_labels=True, node_size=80, node_color=color_map, font_size=9, font_color='black', edge_color='gray', linewidths=10)
-    plt.title = "Route PReview"
+    plt.title = "Route Preview"
     plt.show()
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/node.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,28 @@
     directions = 0
     pit = None
     jumper = None
     jumperLabel = None
     position = None
     onJumper = True
     dvi_credited = None
+    dvi_used = None
     in_tank = False
     color = 'lightgray'
     def __init__(self, ein, pit, jumper):
         self.ein = ein
         self.pit = pit
         self.jumper = jumper
         self.directions
         self.connections
-        # self.dvi_credited 
         # self.dvi_used
         self.show = True
         self.in_tank = False
         self.dvi_credited = None
+        self.dvi_used = None
         self.jumperLabel
         self.position
         self.onJumper
         self.color
 
     def EIN(self):
         return self.ein
@@ -35,17 +36,23 @@
     
     def setPit(self, str):
         self.pit = str
 
     def setJumper(self, jumper):
         self.jumper = jumper
 
+    def findDVI(self, route):
+        return 
+    
     def setPosition(self, route = None):
         return
     
+    def getColor(self):
+        return self.color
+
     def connectBack(self, node):
         if node in self.connections: return
         elif len(self.connections) < self.directions: self.connect(node)
         else: 
             print(self.EIN(), "has maximum number of connections, cant connect back")
             print(type(self))
             for con in self.connections:
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/pit.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/pit.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,8 +9,10 @@
         self.tfsps = []
         self.tfsps_pmid = []
         self.nodes = []
         self.label = label
         self.drain = drain
         self.drainSealPos = drainSealPos 
         self.encasementDrainValve = []
-        self.edvPos = []
+        self.edvPos = []
+    def add_node(self, node):
+        self.nodes.append(node)
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/tankreturn.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/tankreturn.py`

 * *Files identical despite different names*

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/valve2.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/valve2.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
         self.ein = ein
         self.directions = 2 
         self.connections = []
         self.show = True
         self.in_tank = False
         self.position = "CLOSED"
         self.dvi_credited = dvi
-        if (dvi == "YES"):
-            self.color = "skyblue"
 
     def setPosition(self, route = None):
-            self.position = "OPEN "
-
-        
+            self.position = "OPEN"
+    
+    def findDVI(self, route):
+        self.dvi_used = "YES"
+        self.color = "#A0A0A0"
+        return 
+
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool/utils/valve3.py` & `procedure_data_tool-0.0.7/procedure_data_tool/utils/valve3.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,28 +7,46 @@
         self.directions = 3
         self.ein = ein
         self.connections = []
         self.show = True
         self.in_tank = False
         self.position
         self.dvi_credited = dvi
-        if (dvi == "YES"):
-            self.color = "skyblue"
-        elif (dvi == "POS"):
-            self.color = "red"
-    
+
     def setPosition(self, route = None):
         for connection in self.connections:
             if connection in route:
                 pass
             else:
                 if connection.EIN():
                     self.position = "BLOCK " +  connection.EIN()
                 else:
                     for next_connection in connection.connections:
                         if next_connection == self or next_connection in self.connections:
                             pass
                         else:
                             self.position = "BLOCK " + next_connection.EIN()
 
-
-
+    def findDVI(self, route):
+        self.dvi_used = self.dvi_credited #CORRECT. ALWAYS
+        for connection in self.connections:
+            if connection in route:
+                pass
+            else:
+                if connection.EIN():
+                    route.append(connection)
+                else:
+                    for next_connection in connection.connections:
+                        if next_connection == self or next_connection in self.connections:
+                            pass
+                        else:
+                            route.append(next_connection)
+        return 
+    
+    def getColor(self):
+        if (self.dvi_used == "YES"):
+            self.color = "skyblue"
+        elif (self.dvi_used == "POS"):
+            self.color = "red"
+        if (self.dvi_used == "NO"):
+            self.color = "#A0A0A0"
+        return self.color
```

### Comparing `procedure_data_tool-0.0.6/procedure_data_tool.egg-info/SOURCES.txt` & `procedure_data_tool-0.0.7/procedure_data_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procedure_data_tool-0.0.6/setup.py` & `procedure_data_tool-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="procedure_data_tool",
-    version="0.0.6",
+    version="0.0.7",
     description="Reference tool for DST Waste Transfer Procedures Based on automatically generated route",
     packages=find_packages(include=['procedure_data_tool', 'procedure_data_tool.*']),
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author="Josue Estrada",
     author_email="jramiroem@gmail.com",
     license="MIT",
     install_requires=[
         'openpyxl',
         'python-docx',
         'networkx',
         'matplotlib',
     ],
     include_package_data=True,
-
 )
```

