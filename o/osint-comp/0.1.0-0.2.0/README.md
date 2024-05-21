# Comparing `tmp/osint-comp-0.1.0.tar.gz` & `tmp/osint_comp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-comp-0.1.0.tar", last modified: Fri Mar  8 14:59:46 2024, max compression
+gzip compressed data, was "osint_comp-0.2.0.tar", last modified: Tue May 21 22:16:24 2024, max compression
```

## Comparing `osint-comp-0.1.0.tar` & `osint_comp-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:46.023997 osint-comp-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-08 14:59:46.023997 osint-comp-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-08 14:59:40.000000 osint-comp-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-08 14:59:40.000000 osint-comp-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 14:59:46.023997 osint-comp-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:46.023997 osint-comp-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:46.023997 osint-comp-0.1.0/src/osint_comp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-08 14:59:46.000000 osint-comp-0.1.0/src/osint_comp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-08 14:59:46.000000 osint-comp-0.1.0/src/osint_comp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:59:46.000000 osint-comp-0.1.0/src/osint_comp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-08 14:59:46.000000 osint-comp-0.1.0/src/osint_comp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 14:59:46.000000 osint-comp-0.1.0/src/osint_comp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-08 14:59:46.000000 osint-comp-0.1.0/src/osint_comp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:59:46.023997 osint-comp-0.1.0/src/osinter/
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-03-08 14:59:40.000000 osint-comp-0.1.0/src/osinter/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 22:16:24.023048 osint_comp-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 22:16:18.000000 osint_comp-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 22:16:18.000000 osint_comp-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:16:24.023048 osint_comp-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/src/osint_comp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/src/osinter/
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-21 22:16:18.000000 osint_comp-0.2.0/src/osinter/__main__.py
```

### Comparing `osint-comp-0.1.0/src/osinter/__main__.py` & `osint_comp-0.2.0/src/osinter/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import rich_click as click
 import os
 from rich import print as rprint
 from rich.console import Console
 from rich.table import Table
 
-formatkeys = ["n","nf","nma","nm","nl","a","al","ac","as","an","az","aa"]
+formatkeys = ["n","nf","nma","nm","nl","a","al","ac","as","an","az","aa","fb","in","tx","rd","li","tt"]
 
 # osinter reader legend; line in corresponding file; top-level format
 # n is full name; line 1; nf (if no nm, nma, if no nma, leave blank) nl
 # nf is first name; line 2
 # nma is middle name abbrevated; line 3
 # nm is middle name; line 4
 # nl is last name; line 5
@@ -39,18 +39,22 @@
     else:
         if os.path.exists(f"osint/{file}"):
             raise click.ClickException(f"A file with the name {file} already exists.")        
     os.mkdir(f"osint/{file}")
     os.system(f"touch osint/{file}/init.oie")
     os.system(f"touch osint/{file}/name.oie")
     os.system(f"touch osint/{file}/address.oie")
+    os.system(f"touch osint/{file}/online/usernames.oie")
+    os.system(f"touch osint/{file}/online/emails.oie")
     fn = open(f"osint/{file}/name.oie", "a")
     fa = open(f"osint/{file}/address.oie", "a")
+    fos = open(f"osint/{file}/online/socials.oie", "a")
     fn.write("\n\n\n\n\n")
     fa.write("\n\n\n\n\n\n\n")
+    fos.write("\n\n\n\n\n\n")
     fn.close()
     fa.close()
     rprint("Files created!")
     exit()
     
     
 
@@ -181,48 +185,52 @@
     rprint("[bold]Welcome to OSINTer[/]\n\n")
     if file == "":
         file = click.prompt("what file would you like to add to?")
         if not os.path.exists("osint/" + file):
             raise click.ClickException("This file does not exist")
     elif not os.path.exists("osint/" + file):
         raise click.ClickException("This file does not exist")
-    fsplit = []
+    fileSplit = []
     divider = "/"
-    fq = ""
-    fullm = False
+    fileQuery = ""
+    fullMiddle = False
     if autoformat == False:
         click.echo("What data would you like to add? (data format) (use osint format to see format names) (make sure to use dividers like '.' or '/')")
         format = click.prompt("Format")
         divider = click.prompt("Divider")
-        fsplit = format.split(divider)
+        fileSplit = format.split(divider)
     else: 
         click.echo("What data type are you adding?")
-        fq = click.prompt("(a/n)")
-        if fq == "a":
-            fsplit = ["al", "ac", "as", "an", "az", "aa"]
-        elif fq == "n":
-            mq = click.prompt("Do you have a full middle name? (y/n)")
-            fullm = True if mq == "y" else False
-            fullm = False if mq == "n" else True
-            if mq not in ["y", "n"]:
+        fileQuery = click.prompt("(a/n/s)")
+        if fileQuery == "a":
+            fileSplit = ["al", "ac", "as", "an", "az", "aa"]
+        elif fileQuery == "n":
+            middleQuery = click.prompt("Do you have a full middle name? (y/n)")
+            fullMiddle = True if middleQuery == "y" else False
+            fullMiddle = False if middleQuery == "n" else True
+            if middleQuery not in ["y", "n"]:
                 raise click.ClickException("Not a valid option")
-            fsplit = ["n", "nf", "nma", "nm", "nl"]
-    for i in fsplit:
+            fileSplit = ["n", "nf", "nma", "nm", "nl"]
+        elif fileQuery == "s":
+            fileSplit = ["fb", "in", "tx", "rd", "li", "tt"]
+    for i in fileSplit:
         if i not in formatkeys:
             raise Exception(f"\n\nFormat key '{i}' not found")
     data = click.prompt("Data")
     dsplit = data.split(divider)
     d = dsplit
     for i in range(len(dsplit)):
-        ft = fsplit[i]
+        ft = fileSplit[i]
         dt = dsplit[i]
         fa = open(f"osint/{file}/address.oie", "r").readlines()
         fn = open(f"osint/{file}/name.oie", "r").readlines()
+        fos = open(f"osint/{file}/online/socials.oie", "r").readlines()
         fn.append("\n")
         fa.append("\n")
+        fos.append("\n")
         if autoformat == False:
             if ft == "n":
                 fn[0] = dt
                 open(f"osint/{file}/name.oie", "w").writelines(fn)
             elif ft == "nf":
                 fn[1] = dt
                 open(f"osint/{file}/name.oie", "w").writelines(fn)
@@ -253,31 +261,34 @@
             elif ft == "az":
                 fa[5] = dt
                 open(f"osint/{file}/address.oie", "w").writelines(fa)
             elif ft == "aa":
                 fa[6] = dt
                 open(f"osint/{file}/address.oie", "w").writelines(fa)
         elif autoformat == True:
-            if fq == "a":
+            if fileQuery == "a":
                 if len(d) == 5:
                     d.append("N/A")
                 fa = [f"{d[0]}, {d[1]}, {d[2]}, {d[3]}\n",f"{d[0]}\n",f"{d[1]}\n",f"{d[2]}\n",f"{d[3]}\n",f"{d[4]}\n",f"{d[5]}\n"]
                 open(f"osint/{file}/address.oie", "w").writelines(fa)
-            elif fq == "n":
+            elif fileQuery == "n":
                 if len(d) == 2:
                     fn = [f"{d[0]} {d[1]}\n",f"{d[0]}\n","\n","\n",f"{d[1]}\n"]
                     open(f"osint/{file}/name.oie", "w").writelines(fn)
                 elif len(d) == 3:
-                    if fullm == True:
+                    if fullMiddle == True:
                         abm = [*d[1]][0] + "."
                         fn = [f"{d[0]} {d[1]} {d[2]}\n",f"{d[0]}\n",f"{abm}\n",f"{d[1]}\n",f"{d[2]}\n"]
                         open(f"osint/{file}/name.oie", "w").writelines(fn)
-                    if fullm == False:
+                    if fullMiddle == False:
                         fn = [f"{d[0]} {d[1]} {d[2]}\n",f"{d[0]}\n",f"{d[1]}\n","\n",f"{d[2]}\n"]
                         open(f"osint/{file}/name.oie", "w").writelines(fn)
+            elif fileQuery == "s":
+                fos = [f"{d[0]}\n",f"{d[1]}\n",f"{d[2]}\n",f"{d[3]}\n",f"{d[4]}\n",f"{d[5]}\n"]
+                open(f"osint/{file}/online/socials.oie", "w").writelines(fos)
         
 @cli.command()
 def remove():
     """Removes a specific osint file"""
     os.system("clear")
     rprint("[bold]Welcome to OSINTer[/]\n\n")
     click.echo("Which file would you like to remove?")
@@ -321,13 +332,22 @@
     rprint("  [b]a[/] - Full Address")
     rprint("  [b]al[/] - Address Line")
     rprint("  [b]ac[/] - City")
     rprint("  [b]as[/] - State (or Province)")
     rprint("  [b]an[/] - Nation (country)")
     rprint("  [b]az[/] - Zip Code")
     rprint("  [b]aa[/] - Apartment Number")
+    rprint("\n\n[b]Socials[/]")
+    rprint("  [b]s[/] - All Socials")
+    rprint("  [b]fb[/] - Facebook")
+    rprint("  [b]in[/] - Instagram")
+    rprint("  [b]tx[/] - Twitter/X")
+    rprint("  [b]rd[/] - Reddit")
+    rprint("  [b]li[/] - LinkedIn")
+    rprint("  [b]tt[/] - Tiktok")
     rprint("\n\n\n[bold]Autoformats[/]")
     rprint("  [b]a[/] - al/ac/as/an/az(/aa)")
     rprint("  [b]n[/] - nf(/nm)/nl")
+    rprint("  [b]s[/] - fb/in/tx/rd/li/tt")
                       
 if __name__ == "__main__":
     cli()
```

