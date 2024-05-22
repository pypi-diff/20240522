# Comparing `tmp/undumper-0.0.1.tar.gz` & `tmp/undumper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undumper-0.0.1.tar", max compression
+gzip compressed data, was "undumper-0.0.2.tar", max compression
```

## Comparing `undumper-0.0.1.tar` & `undumper-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1929 2024-05-08 16:34:04.053338 undumper-0.0.1/README.md
--rw-r--r--   0        0        0      445 2024-05-22 15:14:42.560927 undumper-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1076 2024-05-08 16:34:04.053338 undumper-0.0.1/undumper/LICENSE
--rw-r--r--   0        0        0     7018 2024-05-22 15:02:14.166638 undumper-0.0.1/undumper/main.py
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 undumper-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-22 17:59:00.480273 undumper-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2928 2024-05-22 17:59:00.480273 undumper-0.0.2/README.md
+-rw-r--r--   0        0        0      445 2024-05-22 17:59:00.480273 undumper-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6830 2024-05-22 17:59:00.480273 undumper-0.0.2/undumper/undumper.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 undumper-0.0.2/PKG-INFO
```

### Comparing `undumper-0.0.1/README.md` & `undumper-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -40,7 +40,38 @@
 
 ### Milestones
 1. Implement `read_whole_dump`.
 2. Implement `read_dump` using what was learned.
 3. Potentially rewrite `read_whole_dump`, if performance improvements are expected.
 4. Potentially rewrite the whole package with Rust bindings.
 
+
+### Current Usage
+```python
+import undumper 
+
+data = undumper.read_dump(file) #where file can be a classic, grid or yaml lammps dump file 
+
+for snapshot in data:
+    timesteps.append(snapshot["TIMESTEP"])
+    positions.append([])
+
+    for atom in snapshot["ATOMS"]:
+        if atom["element"] == "Li":
+            positions[-1].append([atom["xu"], atom["yu"], atom["zu"]])
+
+whole_data = undumper.read_whole_dump(file) #where file can be a classic, grid or yaml lammps dump file
+```
+
+The output data structure in each of these cases looks as follows, the only difference is that read_dump generates a dictionary representing one frame and read_whole dump generates a list of dictionaries with each being an individual frame
+
+```python
+unDumped = [{'TIMESTEP':0, 'NUMBER OF ATOMS':1600, 'BOX BOUNDS':{x: [0,0], y: [0,0]. z: [0,0]}, 'ATOMS':{id: 1, 'Element': "Li", "xu": 1, "yu": 2, "zu": 3}]
+```
+
+### FUll COMMAND LIST
+
+**read_dump**
+**read_whole_dump**
+**read_classic**
+**read_yaml**
+**read_grid**
```

### Comparing `undumper-0.0.1/undumper/LICENSE` & `undumper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `undumper-0.0.1/undumper/main.py` & `undumper-0.0.2/undumper/undumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     """Generator object that yields one frame of the file at a time for yaml style lammp dump files"""
     unDumped = {}
     with open(file, "r") as yams:
         for line in yaml.safe_load_all(yams):
             unDumped["TIMESTEP"] = line["timestep"]
             unDumped["NUMBER OF ATOMS"] = line["natoms"]
             unDumped["BOX BOUNDS"] = {}
-            unDumped["BOX BOUNDS"]["x"] = line["box"][0]  # this may not always follow this structure, test this further format here may be slightly diff from classic, check if thats okay
+            unDumped["BOX BOUNDS"]["x"] = line["box"][0]  
             unDumped["BOX BOUNDS"]["y"] = line["box"][1]
             unDumped["BOX BOUNDS"]["z"] = line["box"][2]
             unDumped["ATOMS"] = []
             paraList = line["keywords"]
             for val in range(len(line["data"])):
                 atomDict = {}
                 paraNum = 0
@@ -124,19 +124,19 @@
                 checkLoop = loopCount
             if mode == Modes.DIM and (loopCount - checkLoop) == 1:
                 unDumped["DIMENSION"] = int(line)
             if "GRID SIZE" in line:
                 mode = Modes.GRID_S
                 checkLoop = loopCount
             if mode == Modes.GRID_S and (loopCount - checkLoop) == 1:
-                unDumped["GRID SIZE"] = line.split() #Ask Xander if this format okay
+                unDumped["GRID SIZE"] = line.split() 
             if "GRID CELLS" in line:
                 mode = Modes.GRID_C
                 checkLoop = loopCount
-                gridName = line.split()[3] #is it always the 3rd index? 
+                gridName = line.split()[3] u
                 unDumped[gridName] = {}
                 gridID = 1
             if mode == Modes.GRID_C and (loopCount - checkLoop) >= 1:
                 unDumped[gridName][gridID] = line
                 gridID += 1
             if frameCount > 1 and unDumped and (loopCount - frameLength) % (gridID + 10) == 0:
                 yield unDumped
```

