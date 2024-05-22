# Comparing `tmp/adofaipy-3.0.3.tar.gz` & `tmp/adofaipy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adofaipy-3.0.3.tar", last modified: Mon Mar 18 11:37:25 2024, max compression
+gzip compressed data, was "adofaipy-3.1.0.tar", last modified: Wed May 22 16:59:56 2024, max compression
```

## Comparing `adofaipy-3.0.3.tar` & `adofaipy-3.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 11:37:25.504130 adofaipy-3.0.3/
--rw-rw-rw-   0        0        0     2051 2024-03-18 11:31:51.000000 adofaipy-3.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1061 2023-09-03 12:23:29.000000 adofaipy-3.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       36 2023-09-03 12:23:30.000000 adofaipy-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8584 2024-03-18 11:37:25.503124 adofaipy-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5923 2024-01-24 13:59:02.000000 adofaipy-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 11:37:25.467834 adofaipy-3.0.3/adofaipy/
--rw-rw-rw-   0        0        0    12337 2024-03-18 11:27:44.000000 adofaipy-3.0.3/adofaipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 11:37:25.499321 adofaipy-3.0.3/adofaipy.egg-info/
--rw-rw-rw-   0        0        0     8584 2024-03-18 11:37:25.000000 adofaipy-3.0.3/adofaipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-03-18 11:37:25.000000 adofaipy-3.0.3/adofaipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 11:37:25.000000 adofaipy-3.0.3/adofaipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 11:37:25.000000 adofaipy-3.0.3/adofaipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 11:37:25.505222 adofaipy-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0      767 2024-03-18 11:29:19.000000 adofaipy-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:59:56.717445 adofaipy-3.1.0/
+-rw-rw-rw-   0        0        0     2584 2024-05-22 16:57:31.000000 adofaipy-3.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1061 2023-09-03 12:23:29.000000 adofaipy-3.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       36 2023-09-03 12:23:30.000000 adofaipy-3.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9845 2024-05-22 16:59:56.715443 adofaipy-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6679 2024-05-22 16:57:17.000000 adofaipy-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 16:59:56.702335 adofaipy-3.1.0/adofaipy/
+-rw-rw-rw-   0        0        0    14849 2024-05-22 10:45:20.000000 adofaipy-3.1.0/adofaipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:59:56.711843 adofaipy-3.1.0/adofaipy.egg-info/
+-rw-rw-rw-   0        0        0     9845 2024-05-22 16:59:56.000000 adofaipy-3.1.0/adofaipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-22 16:59:56.000000 adofaipy-3.1.0/adofaipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:59:56.000000 adofaipy-3.1.0/adofaipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 16:59:56.000000 adofaipy-3.1.0/adofaipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:59:56.717445 adofaipy-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      767 2024-05-22 16:24:53.000000 adofaipy-3.1.0/setup.py
```

### Comparing `adofaipy-3.0.3/CHANGELOG.md` & `adofaipy-3.1.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 
 <h1>Changelog</h1>
 
-## 3.0.3 (2023/03/18)
+## 3.1.0 (2024/05/20)
+------------------
+- Major update and bugfixes
+- Added `getAngles()` and `setAngles()`
+- Added `getAnglesRelative()` and `setAnglesRelative()`, with options to take twirls/midspins into account
+- `tiles` list is now type-check friendly
+- Updated `Settings` class
+- Added support for levels that use `pathData`
+- Fixed `writeToFile()` no longer working (again)
+- Fixed typos in `_getFileString()` and `_getFileDict()`
+- Cleaned up some errors in README.md
+- Version number is no longer out of sync
+
+## 3.0.3 (2024/03/18)
 ------------------
 - Minor bugfixes
 - Fixed `writeToFile()` no longer working
 - Replaced `json.dumps()` with faster `json.dump()` in `writeToFile()`
 - Known issue: version number is out of sync
 
 ## 3.0.1 (2023/12/02)
```

### Comparing `adofaipy-3.0.3/LICENSE.txt` & `adofaipy-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-3.0.3/PKG-INFO` & `adofaipy-3.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: adofaipy
-Version: 3.0.3
+Version: 3.1.0
 Summary: A library that makes automating events in ADOFAI levels more convenient.
-Home-page: UNKNOWN
+Home-page: 
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
 Keywords: adofai
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -23,53 +22,62 @@
 <i><code style="color : white">LevelDict</code></i>
 <dl>
     Initalize with <code>LevelDict(filename, encoding)</code> (encoding is optional, default is utf-8-sig)<br>
     <br><dt><code>LevelDict.filename : str</code>
     <dd>The filename of the file from which the <code>LevelDict</code> was obtained.
     <dt><code>LevelDict.encoding : str</code>
     <dd>The encoding of the file from which the <code>LevelDict</code> was obtained.
-    <dd>A list of all decorations (including objects and text) in the level.
     <dt><code>LevelDict.nonFloorDecos : list[Decoration]</code>
     <dd>A list of all decorations in the level that are not tied to any particular tile.
     <dt><code>LevelDict.settings : Settings</code>
     <dd>The level settings, as a Settings object.
     <dt><code>LevelDict.tiles : list[Tile]</code>
     <dd>A list of all tiles in the level. (See <code>Tile</code> class)</dd>
-    <br><dt><code>LevelDict.appendTile(self, angle : float) -> None:</code>
+    <hr><dt><code>LevelDict.appendTile(angle : float) -> None:</code>
     <dd>Adds a single tile to the end of the level.
-    <dt><code>LevelDict.appendTiles(self, angles : list[float]) -> None:</code>
+    <dt><code>LevelDict.appendTiles(angles : list[float]) -> None:</code>
     <dd>Adds a list of tiles to the end of the level.
-    <dt><code>LevelDict.insertTile(self, angle : float, index : int) -> None:</code>
+    <dt><code>LevelDict.insertTile(angle : float, index : int) -> None:</code>
     <dd>Adds a single tile to the level before the specified index.
-    <dt><code>LevelDict.insertTiles(self, angles : list[float], index : int) -> None:</code>
+    <dt><code>LevelDict.insertTiles(angles : list[float], index : int) -> None:</code>
     <dd>Adds a list of tiles to the level before the specified index.
-    <dt><code>LevelDict.addAction(self, event : Action) -> int:</code>
+    <dt><code>LevelDict.getAngles() -> list[float]:</code>
+    <dd>Returns a list of angles for each tile.
+    <dt><code>LevelDict.setAngles(angles: list[float]) -> None:</code>
+    <dd>Writes a list of angles to angleData. The list is truncated if it's too big, and the track is truncated if the list is too small.
+    <dt><code>LevelDict.getAnglesRelative(ignoretwirls: bool=False) -> list[float]</code>
+    <dd>Gets a list of relative angles (degrees between each pair of tiles.) Twirls are taken into account by default. To disable this, set ignoretwirls to True. Midspins are always taken into account.
+    <dt><code>LevelDict.setAnglesRelative(angles: list[float]) -> None</code>
+    <dd>Sets a list of relative angles (degrees between each pair of tiles.)
+    <dt><code>LevelDict.addAction(event : Action) -> int:</code>
     <dd>Adds the given action to the level. Returns the index of the event within the tile.
-    <dt><code>LevelDict.addDecoration(self, event : Decoration) -> int:</code>
+    <dt><code>LevelDict.addAction(event : Action) -> int:</code>
+    <dd>Adds the given action to the level. Returns the index of the event within the tile.
+    <dt><code>LevelDict.addDecoration(event : Decoration) -> int:</code>
     <dd>Adds the given decoration to the level. Returns the index of the event within the tile / within the list of non-floor decorations.
-    <dt><code>LevelDict.getActions(self, condition : Callable) -> list[Action]:</code>
+    <dt><code>LevelDict.getActions(condition : Callable) -> list[Action]:</code>
     <dd>Returns a list of actions in the level that meet the given condition. Returns a list of all actions if condition is not specified.
-    <dt><code>LevelDict.getDecorations(self, condition : Callable) -> list[Decoration]:</code>
+    <dt><code>LevelDict.getDecorations(condition : Callable) -> list[Decoration]:</code>
     <dd>Returns a list of decorations in the level that meet the given condition. Returns a list of all decorations if condition is not specified.
-    <dt><code>LevelDict.removeActions(self, condition : Callable) -> list[Action]:</code>
+    <dt><code>LevelDict.removeActions(condition : Callable) -> list[Action]:</code>
     <dd>Removes all actions in the level that meet the given condition. Returns a list of removed actions.
-    <dt><code>LevelDict.removeDecorations(self, condition : Callable) -> list[Decoration]:</code>
+    <dt><code>LevelDict.removeDecorations(condition : Callable) -> list[Decoration]:</code>
     <dd>Removes all decorations in the level that meet the given condition. Returns a list of removed decorations.
-    <dt><code>LevelDict.popAction(self, tile, index) -> Action:</code>
+    <dt><code>LevelDict.popAction(tile, index) -> Action:</code>
     <dd>Removes the action at the specified tile at the specified index. Returns the event.
-    <dt><code>LevelDict.popDecoration(self, tile, index) -> Decoration:</code>
+    <dt><code>LevelDict.popDecoration(tile, index) -> Decoration:</code>
     <dd>Removes the decoration at the specified tile at the specified index. Returns the event.
-    <dt><code>LevelDict.replaceFieldAction(self, condition : Callable, field : str, new) -> None:</code>
+    <dt><code>LevelDict.replaceFieldAction(condition : Callable, field : str, new) -> None:</code>
     <dd>Changes the value of "field" to "new" in all actions that meet the given condition.
-    <dt><code>LevelDict.replaceFieldDecoration(self, condition : Callable, field : str, new) -> None:</code>
+    <dt><code>LevelDict.replaceFieldDecoration(condition : Callable, field : str, new) -> None:</code>
     <dd>Changes the value of "field" to "new" in all decorations that meet the given condition.
-    <dt><code>LevelDict.writeDictToFile(self, leveldict : dict, filename : str):</code>
+    <dt><code>LevelDict.writeDictToFile(leveldict : dict, filename : str):</code>
     <dd>Writes the given dictionary to the specified file. Overwrites the original file if filename is not specified.
     <br><i>Use this if you are working with <code>LevelDict.leveldict</code>.</i>
-    <dt><code>LevelDict.writeToFile(self, filename : str=None) -> None:</code>
+    <dt><code>LevelDict.writeToFile(filename : str=None) -> None:</code>
     <dd>Writes the level to the specified file. Overwrites the original file if filename is not specified.
 </dl>
 <hr>
 <i><code style="color : white">Settings</code></i><br>
 Part of a LevelDict object. The properties of this class are equivalent to the parameters in the <code>settings</code> field of a .adofai file.
 <hr>
 <i><code style="color : white">Tile</code></i><br>
@@ -92,15 +100,28 @@
 A decoration, object decoration, or text decoration (anything found in the decorations menu on the left sidebar). A <code> Decoration</code> object behaves like a <code>dict</code>. The keys depend on the event type. Check any entry in the <code>decorations</code> field of a .adofai file for more information on the fields used by that event type.
 <br><br>
 Decoration objects are found in a list of decorations in a <code>Tile</code> object. If the decoration is not tied to any tile, it is found in the list of non-floor decos.
 <hr><br>
 
 <h1>Changelog</h1>
 
-## 3.0.3 (2023/03/18)
+## 3.1.0 (2024/05/20)
+------------------
+- Major update and bugfixes
+- Added `getAngles()` and `setAngles()`
+- Added `getAnglesRelative()` and `setAnglesRelative()`, with options to take twirls/midspins into account
+- `tiles` list is now type-check friendly
+- Updated `Settings` class
+- Added support for levels that use `pathData`
+- Fixed `writeToFile()` no longer working (again)
+- Fixed typos in `_getFileString()` and `_getFileDict()`
+- Cleaned up some errors in README.md
+- Version number is no longer out of sync
+
+## 3.0.3 (2024/03/18)
 ------------------
 - Minor bugfixes
 - Fixed `writeToFile()` no longer working
 - Replaced `json.dumps()` with faster `json.dump()` in `writeToFile()`
 - Known issue: version number is out of sync
 
 ## 3.0.1 (2023/12/02)
@@ -162,8 +183,7 @@
 ## 0.0.2 (2023/06/13)
 ------------------
 - Minor bugfix: `'re'` is no longer a dependency
 
 ## 0.0.1 (2023/05/28)
 ------------------
 - First Release
-
```

### Comparing `adofaipy-3.0.3/README.md` & `adofaipy-3.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,53 +5,62 @@
 <i><code style="color : white">LevelDict</code></i>
 <dl>
     Initalize with <code>LevelDict(filename, encoding)</code> (encoding is optional, default is utf-8-sig)<br>
     <br><dt><code>LevelDict.filename : str</code>
     <dd>The filename of the file from which the <code>LevelDict</code> was obtained.
     <dt><code>LevelDict.encoding : str</code>
     <dd>The encoding of the file from which the <code>LevelDict</code> was obtained.
-    <dd>A list of all decorations (including objects and text) in the level.
     <dt><code>LevelDict.nonFloorDecos : list[Decoration]</code>
     <dd>A list of all decorations in the level that are not tied to any particular tile.
     <dt><code>LevelDict.settings : Settings</code>
     <dd>The level settings, as a Settings object.
     <dt><code>LevelDict.tiles : list[Tile]</code>
     <dd>A list of all tiles in the level. (See <code>Tile</code> class)</dd>
-    <br><dt><code>LevelDict.appendTile(self, angle : float) -> None:</code>
+    <hr><dt><code>LevelDict.appendTile(angle : float) -> None:</code>
     <dd>Adds a single tile to the end of the level.
-    <dt><code>LevelDict.appendTiles(self, angles : list[float]) -> None:</code>
+    <dt><code>LevelDict.appendTiles(angles : list[float]) -> None:</code>
     <dd>Adds a list of tiles to the end of the level.
-    <dt><code>LevelDict.insertTile(self, angle : float, index : int) -> None:</code>
+    <dt><code>LevelDict.insertTile(angle : float, index : int) -> None:</code>
     <dd>Adds a single tile to the level before the specified index.
-    <dt><code>LevelDict.insertTiles(self, angles : list[float], index : int) -> None:</code>
+    <dt><code>LevelDict.insertTiles(angles : list[float], index : int) -> None:</code>
     <dd>Adds a list of tiles to the level before the specified index.
-    <dt><code>LevelDict.addAction(self, event : Action) -> int:</code>
+    <dt><code>LevelDict.getAngles() -> list[float]:</code>
+    <dd>Returns a list of angles for each tile.
+    <dt><code>LevelDict.setAngles(angles: list[float]) -> None:</code>
+    <dd>Writes a list of angles to angleData. The list is truncated if it's too big, and the track is truncated if the list is too small.
+    <dt><code>LevelDict.getAnglesRelative(ignoretwirls: bool=False) -> list[float]</code>
+    <dd>Gets a list of relative angles (degrees between each pair of tiles.) Twirls are taken into account by default. To disable this, set ignoretwirls to True. Midspins are always taken into account.
+    <dt><code>LevelDict.setAnglesRelative(angles: list[float]) -> None</code>
+    <dd>Sets a list of relative angles (degrees between each pair of tiles.)
+    <dt><code>LevelDict.addAction(event : Action) -> int:</code>
     <dd>Adds the given action to the level. Returns the index of the event within the tile.
-    <dt><code>LevelDict.addDecoration(self, event : Decoration) -> int:</code>
+    <dt><code>LevelDict.addAction(event : Action) -> int:</code>
+    <dd>Adds the given action to the level. Returns the index of the event within the tile.
+    <dt><code>LevelDict.addDecoration(event : Decoration) -> int:</code>
     <dd>Adds the given decoration to the level. Returns the index of the event within the tile / within the list of non-floor decorations.
-    <dt><code>LevelDict.getActions(self, condition : Callable) -> list[Action]:</code>
+    <dt><code>LevelDict.getActions(condition : Callable) -> list[Action]:</code>
     <dd>Returns a list of actions in the level that meet the given condition. Returns a list of all actions if condition is not specified.
-    <dt><code>LevelDict.getDecorations(self, condition : Callable) -> list[Decoration]:</code>
+    <dt><code>LevelDict.getDecorations(condition : Callable) -> list[Decoration]:</code>
     <dd>Returns a list of decorations in the level that meet the given condition. Returns a list of all decorations if condition is not specified.
-    <dt><code>LevelDict.removeActions(self, condition : Callable) -> list[Action]:</code>
+    <dt><code>LevelDict.removeActions(condition : Callable) -> list[Action]:</code>
     <dd>Removes all actions in the level that meet the given condition. Returns a list of removed actions.
-    <dt><code>LevelDict.removeDecorations(self, condition : Callable) -> list[Decoration]:</code>
+    <dt><code>LevelDict.removeDecorations(condition : Callable) -> list[Decoration]:</code>
     <dd>Removes all decorations in the level that meet the given condition. Returns a list of removed decorations.
-    <dt><code>LevelDict.popAction(self, tile, index) -> Action:</code>
+    <dt><code>LevelDict.popAction(tile, index) -> Action:</code>
     <dd>Removes the action at the specified tile at the specified index. Returns the event.
-    <dt><code>LevelDict.popDecoration(self, tile, index) -> Decoration:</code>
+    <dt><code>LevelDict.popDecoration(tile, index) -> Decoration:</code>
     <dd>Removes the decoration at the specified tile at the specified index. Returns the event.
-    <dt><code>LevelDict.replaceFieldAction(self, condition : Callable, field : str, new) -> None:</code>
+    <dt><code>LevelDict.replaceFieldAction(condition : Callable, field : str, new) -> None:</code>
     <dd>Changes the value of "field" to "new" in all actions that meet the given condition.
-    <dt><code>LevelDict.replaceFieldDecoration(self, condition : Callable, field : str, new) -> None:</code>
+    <dt><code>LevelDict.replaceFieldDecoration(condition : Callable, field : str, new) -> None:</code>
     <dd>Changes the value of "field" to "new" in all decorations that meet the given condition.
-    <dt><code>LevelDict.writeDictToFile(self, leveldict : dict, filename : str):</code>
+    <dt><code>LevelDict.writeDictToFile(leveldict : dict, filename : str):</code>
     <dd>Writes the given dictionary to the specified file. Overwrites the original file if filename is not specified.
     <br><i>Use this if you are working with <code>LevelDict.leveldict</code>.</i>
-    <dt><code>LevelDict.writeToFile(self, filename : str=None) -> None:</code>
+    <dt><code>LevelDict.writeToFile(filename : str=None) -> None:</code>
     <dd>Writes the level to the specified file. Overwrites the original file if filename is not specified.
 </dl>
 <hr>
 <i><code style="color : white">Settings</code></i><br>
 Part of a LevelDict object. The properties of this class are equivalent to the parameters in the <code>settings</code> field of a .adofai file.
 <hr>
 <i><code style="color : white">Tile</code></i><br>
```

### Comparing `adofaipy-3.0.3/adofaipy/__init__.py` & `adofaipy-3.1.0/adofaipy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 		super(Action, self).__init__(*arg, **kw)
 
 class Decoration(UserDict):
 	def __init__(self,*arg,**kw):
 		super(Decoration, self).__init__(*arg, **kw)
 
 class Tile():
-	def __init__(self, angle : int, actions : list[Action]=[], decorations : list[Decoration]=[]):
+	def __init__(self, angle : float, actions : list[Action]=[], decorations : list[Decoration]=[]):
 		self.angle = angle
 		self.actions = actions.copy()
 		self.decorations = decorations.copy()
 
 class Settings():
 	def __init__(self, values : dict) -> None:
 		self.version = values["version"]
@@ -97,45 +97,55 @@
 		
 class LevelDict:
 
 	def __init__(self, filename : str, encoding="utf-8-sig") -> None:
 		
 		self.filename = filename
 		self.encoding = encoding
-		leveldict = self.__getFileDict()
-		angleData = leveldict["angleData"]
-		angleData.append(angleData[len(angleData)-1])
+		leveldict = self._getFileDict()
+
+		if "angleData" in leveldict:
+			__angleData = leveldict["angleData"]
+		else:
+			__pathchars = { "R": 0, "p": 15, "J": 30, "E": 45, "T": 60, "o": 75, "U": 90, "q": 105, "G": 120, "Q": 135, "H": 150, "W": 165, "L": 180, "x": 195, "N": 210, "Z": 225, "F": 240, "V": 255, "D": 270, "Y": 285, "B": 300, "C": 315, "M": 330, "A": 345, "!": 999}
+
+			__angleData = []
+			for i in "".split(leveldict["pathData"]):
+				__angleData.append(__pathchars[i])
+		
+		__angleData.append(__angleData[-1] if __angleData[-1] != 999 else (__angleData[-2]+180)%360)
 		actions = leveldict["actions"]
 		decorations = leveldict["decorations"]
 		self.nonFloorDecos = [Decoration(j) for j in decorations if "floor" not in j.keys()]
 		self.settings = Settings(leveldict["settings"])
-		self.tiles = list()
+		self.tiles = [Tile(0)]
+		self.tiles.pop()
 
-		for angle in angleData:
+		for angle in __angleData:
 			self.tiles.append(Tile(angle))
 
 		for action in actions:
 			self.tiles[action["floor"]].actions.append(Action(action))
 
 		for deco in decorations:
 			if "floor" in deco.keys():
 				self.tiles[deco["floor"]].decorations.append(Decoration(deco))
 
-	def __getFileString(self) -> str:
+	def _getFileString(self) -> str:
 		"""Returns the specified file in string format.
-		It is reccomended to use getFileDict() unless absolutely necessary.
+		It is recommended to use getFileDict() unless absolutely necessary.
 		"""
 		with open(self.filename, "r", encoding=self.encoding) as f:
 			s = f.read()
 			return s
 
-	def __getFileDict(self) -> dict:
+	def _getFileDict(self) -> dict:
 		"""Returns the specified file in the form of nested dictionaries and lists.
 		"""
-		a = self.__getFileString()
+		a = self._getFileString()
 		sp=re.split(r"(?<!\\)(?:\\\\)*(\")",a)
 
 		for i in range(len(sp)):
 			if i % 4 == 0:
 				sp[i] = re.sub(r"(\n|\t)", "", sp[i])
 				sp[i] = re.sub(r"\,(( *)(\]|\}))", "\\3", sp[i])
 				sp[i] = re.sub(r"(\]|\})(\[|\{)", "\\1,\\2", sp[i])
@@ -195,15 +205,83 @@
 		"""
 		self.__addTiles(angles, index)
 		for i in range(index+len(angles), len(self.tiles)):
 			for action in self.tiles[i].actions:
 				action["floor"] += len(angles)
 			for deco in self.tiles[i].decorations:
 				deco["floor"] += len(angles)
+
+	def getAngles(self) -> list[float]:
+		"""Returns a list of angles for each tile.
+		"""
+		angles = []
+		for tile in self.tiles:
+			angles.append(tile.angle)
+		return angles
 	
+	def setAngles(self, angles: list[float]) -> None:
+		"""Writes a list of angles to angleData.
+		The list is truncated if it's too big, and the track is truncated if the list is too small.
+		"""
+		self.tiles = self.tiles[:len(angles)]
+		for tile,angle in zip(self.tiles,angles):
+			tile.angle = angle
+
+	def getAnglesRelative(self, ignoretwirls: bool=False) -> list[float]:
+		"""Gets a list of relative angles (degrees between each pair of tiles.)
+		Twirls are taken into account by default. To disable this, set ignoretwirls to True.
+		Midspins are always taken into account.
+		"""
+		absangles = self.getAngles()
+		midspins = []
+		anglesrev = list(reversed(absangles)).copy()
+		for idx,angle in enumerate(anglesrev):
+			if angle == 999:
+				for idx_ in range(idx):
+					anglesrev[idx_] = (anglesrev[idx_] + 180) % 360
+				print(anglesrev.pop(idx))
+		absangles = list(reversed(anglesrev))
+
+		angles = []
+		for angle,angle_ in zip(absangles,absangles[1:]):
+			angles.append(angle - angle_ + 180)
+
+		angles.insert(0,180)
+
+		twirls = [event['floor'] for event in self.getActions(lambda x: x['eventType'] == 'Twirl')]
+		twirltiles = []
+
+		if len(twirls)%2 == 1:
+			twirls.append(len(self.tiles)+10)
+
+		for i in range(0,len(twirls),2):
+			twirltiles += list(range(twirls[i],twirls[i+1]))
+
+		offset = 0
+		if not ignoretwirls:
+			for idx,angle in enumerate(angles):
+				if idx in midspins:
+					offset += 1
+				if idx+offset in twirltiles:
+					angles[idx] = (((360-angle)-1)%360)+1 if angle != 999 else 999
+
+		angles = [(angle-1)%360 + 1 for angle in angles]
+
+		return angles
+	
+	def setAnglesRelative(self, angles: list[float]) -> None:
+		"""Sets a list of relative angles (degrees between pairs of tiles).
+		"""
+		nangles = [0]
+		for angle in angles:
+			nangles.append((nangles[-1] - angle + 180)%360)
+
+		nangles.pop(0)
+		self.setAngles(nangles)
+
 	def addAction(self, event : Action) -> int:
 		"""Adds the given action to the level.
 		Returns the index of the event within the tile.
 		"""
 
 		self.tiles[event["floor"]].actions.append(event)
 		return len(self.tiles[event["floor"]].actions) - 1
@@ -300,35 +378,33 @@
 		for deco in eventlist:
 			if field in deco:
 				deco[field] = new
 
 		for deco in eventlist:
 			self.addDecoration(deco)
 
-	def writeDictToFile(self, leveldict : dict, filename : str=None):
+	def _writeDictToFile(self, leveldict : dict, filename : str=None):
 		"""Writes the given dictionary to the specified file.
 		Overwrites the original file if filename is not specified.
 		"""
 		name = self.filename if filename is None else filename
-		filestring = json.dumps(leveldict, indent=4)
 		with open(name, "w", encoding=self.encoding) as f:
-			f.write(filestring)
+			json.dump(leveldict, f, indent=4)
 
 	def writeToFile(self, filename : str=None) -> None:
 		"""Writes the level to the specified file.
 		Overwrites the original file if filename is not specified.
 		"""
 		
 		final = {"angleData": [], "settings": {}, "actions": [], "decorations": []}
 		final["settings"] = vars(self.settings)
 		for tile in self.tiles:
 			final["angleData"].append(tile.angle)
 			final["actions"].extend([dict(action) for action in tile.actions])
 			final["decorations"].extend([dict(decoration) for decoration in tile.decorations])
 		
-		final["decorations"] += [decoration for decoration in self.nonFloorDecos]
+		final["decorations"] += [dict(decoration) for decoration in self.nonFloorDecos]
 		final["angleData"].pop()
 
 		name = self.filename if filename is None else filename
-		filestring = json.dumps(final, indent=4)
 		with open(name, "w", encoding=self.encoding) as f:
-			f.write(filestring)
+			json.dump(final, f, indent=4)
```

### Comparing `adofaipy-3.0.3/adofaipy.egg-info/PKG-INFO` & `adofaipy-3.1.0/adofaipy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: adofaipy
-Version: 3.0.3
+Version: 3.1.0
 Summary: A library that makes automating events in ADOFAI levels more convenient.
-Home-page: UNKNOWN
+Home-page: 
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
 Keywords: adofai
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -23,53 +22,62 @@
 <i><code style="color : white">LevelDict</code></i>
 <dl>
     Initalize with <code>LevelDict(filename, encoding)</code> (encoding is optional, default is utf-8-sig)<br>
     <br><dt><code>LevelDict.filename : str</code>
     <dd>The filename of the file from which the <code>LevelDict</code> was obtained.
     <dt><code>LevelDict.encoding : str</code>
     <dd>The encoding of the file from which the <code>LevelDict</code> was obtained.
-    <dd>A list of all decorations (including objects and text) in the level.
     <dt><code>LevelDict.nonFloorDecos : list[Decoration]</code>
     <dd>A list of all decorations in the level that are not tied to any particular tile.
     <dt><code>LevelDict.settings : Settings</code>
     <dd>The level settings, as a Settings object.
     <dt><code>LevelDict.tiles : list[Tile]</code>
     <dd>A list of all tiles in the level. (See <code>Tile</code> class)</dd>
-    <br><dt><code>LevelDict.appendTile(self, angle : float) -> None:</code>
+    <hr><dt><code>LevelDict.appendTile(angle : float) -> None:</code>
     <dd>Adds a single tile to the end of the level.
-    <dt><code>LevelDict.appendTiles(self, angles : list[float]) -> None:</code>
+    <dt><code>LevelDict.appendTiles(angles : list[float]) -> None:</code>
     <dd>Adds a list of tiles to the end of the level.
-    <dt><code>LevelDict.insertTile(self, angle : float, index : int) -> None:</code>
+    <dt><code>LevelDict.insertTile(angle : float, index : int) -> None:</code>
     <dd>Adds a single tile to the level before the specified index.
-    <dt><code>LevelDict.insertTiles(self, angles : list[float], index : int) -> None:</code>
+    <dt><code>LevelDict.insertTiles(angles : list[float], index : int) -> None:</code>
     <dd>Adds a list of tiles to the level before the specified index.
-    <dt><code>LevelDict.addAction(self, event : Action) -> int:</code>
+    <dt><code>LevelDict.getAngles() -> list[float]:</code>
+    <dd>Returns a list of angles for each tile.
+    <dt><code>LevelDict.setAngles(angles: list[float]) -> None:</code>
+    <dd>Writes a list of angles to angleData. The list is truncated if it's too big, and the track is truncated if the list is too small.
+    <dt><code>LevelDict.getAnglesRelative(ignoretwirls: bool=False) -> list[float]</code>
+    <dd>Gets a list of relative angles (degrees between each pair of tiles.) Twirls are taken into account by default. To disable this, set ignoretwirls to True. Midspins are always taken into account.
+    <dt><code>LevelDict.setAnglesRelative(angles: list[float]) -> None</code>
+    <dd>Sets a list of relative angles (degrees between each pair of tiles.)
+    <dt><code>LevelDict.addAction(event : Action) -> int:</code>
     <dd>Adds the given action to the level. Returns the index of the event within the tile.
-    <dt><code>LevelDict.addDecoration(self, event : Decoration) -> int:</code>
+    <dt><code>LevelDict.addAction(event : Action) -> int:</code>
+    <dd>Adds the given action to the level. Returns the index of the event within the tile.
+    <dt><code>LevelDict.addDecoration(event : Decoration) -> int:</code>
     <dd>Adds the given decoration to the level. Returns the index of the event within the tile / within the list of non-floor decorations.
-    <dt><code>LevelDict.getActions(self, condition : Callable) -> list[Action]:</code>
+    <dt><code>LevelDict.getActions(condition : Callable) -> list[Action]:</code>
     <dd>Returns a list of actions in the level that meet the given condition. Returns a list of all actions if condition is not specified.
-    <dt><code>LevelDict.getDecorations(self, condition : Callable) -> list[Decoration]:</code>
+    <dt><code>LevelDict.getDecorations(condition : Callable) -> list[Decoration]:</code>
     <dd>Returns a list of decorations in the level that meet the given condition. Returns a list of all decorations if condition is not specified.
-    <dt><code>LevelDict.removeActions(self, condition : Callable) -> list[Action]:</code>
+    <dt><code>LevelDict.removeActions(condition : Callable) -> list[Action]:</code>
     <dd>Removes all actions in the level that meet the given condition. Returns a list of removed actions.
-    <dt><code>LevelDict.removeDecorations(self, condition : Callable) -> list[Decoration]:</code>
+    <dt><code>LevelDict.removeDecorations(condition : Callable) -> list[Decoration]:</code>
     <dd>Removes all decorations in the level that meet the given condition. Returns a list of removed decorations.
-    <dt><code>LevelDict.popAction(self, tile, index) -> Action:</code>
+    <dt><code>LevelDict.popAction(tile, index) -> Action:</code>
     <dd>Removes the action at the specified tile at the specified index. Returns the event.
-    <dt><code>LevelDict.popDecoration(self, tile, index) -> Decoration:</code>
+    <dt><code>LevelDict.popDecoration(tile, index) -> Decoration:</code>
     <dd>Removes the decoration at the specified tile at the specified index. Returns the event.
-    <dt><code>LevelDict.replaceFieldAction(self, condition : Callable, field : str, new) -> None:</code>
+    <dt><code>LevelDict.replaceFieldAction(condition : Callable, field : str, new) -> None:</code>
     <dd>Changes the value of "field" to "new" in all actions that meet the given condition.
-    <dt><code>LevelDict.replaceFieldDecoration(self, condition : Callable, field : str, new) -> None:</code>
+    <dt><code>LevelDict.replaceFieldDecoration(condition : Callable, field : str, new) -> None:</code>
     <dd>Changes the value of "field" to "new" in all decorations that meet the given condition.
-    <dt><code>LevelDict.writeDictToFile(self, leveldict : dict, filename : str):</code>
+    <dt><code>LevelDict.writeDictToFile(leveldict : dict, filename : str):</code>
     <dd>Writes the given dictionary to the specified file. Overwrites the original file if filename is not specified.
     <br><i>Use this if you are working with <code>LevelDict.leveldict</code>.</i>
-    <dt><code>LevelDict.writeToFile(self, filename : str=None) -> None:</code>
+    <dt><code>LevelDict.writeToFile(filename : str=None) -> None:</code>
     <dd>Writes the level to the specified file. Overwrites the original file if filename is not specified.
 </dl>
 <hr>
 <i><code style="color : white">Settings</code></i><br>
 Part of a LevelDict object. The properties of this class are equivalent to the parameters in the <code>settings</code> field of a .adofai file.
 <hr>
 <i><code style="color : white">Tile</code></i><br>
@@ -92,15 +100,28 @@
 A decoration, object decoration, or text decoration (anything found in the decorations menu on the left sidebar). A <code> Decoration</code> object behaves like a <code>dict</code>. The keys depend on the event type. Check any entry in the <code>decorations</code> field of a .adofai file for more information on the fields used by that event type.
 <br><br>
 Decoration objects are found in a list of decorations in a <code>Tile</code> object. If the decoration is not tied to any tile, it is found in the list of non-floor decos.
 <hr><br>
 
 <h1>Changelog</h1>
 
-## 3.0.3 (2023/03/18)
+## 3.1.0 (2024/05/20)
+------------------
+- Major update and bugfixes
+- Added `getAngles()` and `setAngles()`
+- Added `getAnglesRelative()` and `setAnglesRelative()`, with options to take twirls/midspins into account
+- `tiles` list is now type-check friendly
+- Updated `Settings` class
+- Added support for levels that use `pathData`
+- Fixed `writeToFile()` no longer working (again)
+- Fixed typos in `_getFileString()` and `_getFileDict()`
+- Cleaned up some errors in README.md
+- Version number is no longer out of sync
+
+## 3.0.3 (2024/03/18)
 ------------------
 - Minor bugfixes
 - Fixed `writeToFile()` no longer working
 - Replaced `json.dumps()` with faster `json.dump()` in `writeToFile()`
 - Known issue: version number is out of sync
 
 ## 3.0.1 (2023/12/02)
@@ -162,8 +183,7 @@
 ## 0.0.2 (2023/06/13)
 ------------------
 - Minor bugfix: `'re'` is no longer a dependency
 
 ## 0.0.1 (2023/05/28)
 ------------------
 - First Release
-
```

### Comparing `adofaipy-3.0.3/setup.py` & `adofaipy-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.11'
 ]
  
 setup(
   name='adofaipy',
-  version='3.0.3',
+  version='3.1.0',
   description='A library that makes automating events in ADOFAI levels more convenient.',
   long_description=open('README.md').read() + open('CHANGELOG.md').read(),
   long_description_content_type="text/markdown",
   url='',
   author='M1n3c4rt',
   author_email='vedicbits@gmail.com',
   license='MIT',
```

