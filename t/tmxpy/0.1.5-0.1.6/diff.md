# Comparing `tmp/tmxpy-0.1.5.tar.gz` & `tmp/tmxpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmxpy-0.1.5.tar", last modified: Thu Jul 27 23:40:40 2023, max compression
+gzip compressed data, was "tmxpy-0.1.6.tar", last modified: Tue Aug  8 13:49:31 2023, max compression
```

## Comparing `tmxpy-0.1.5.tar` & `tmxpy-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.805318 tmxpy-0.1.5/
--rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1890 2023-07-27 23:40:40.804317 tmxpy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2023-07-27 23:39:59.000000 tmxpy-0.1.5/README.md
--rw-rw-rw-   0        0        0      719 2023-07-27 21:23:19.000000 tmxpy-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 23:40:40.805318 tmxpy-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.781296 tmxpy-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.792307 tmxpy-0.1.5/src/tmxpy/
--rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.5/src/tmxpy/__init__.py
--rw-rw-rw-   0        0        0    10158 2023-07-27 23:32:33.000000 tmxpy-0.1.5/src/tmxpy/tmxpy.py
-drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.802316 tmxpy-0.1.5/src/tmxpy.egg-info/
--rw-rw-rw-   0        0        0     1890 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 13:49:31.619666 tmxpy-0.1.6/
+-rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1890 2023-08-08 13:49:31.617664 tmxpy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2023-07-27 23:39:59.000000 tmxpy-0.1.6/README.md
+-rw-rw-rw-   0        0        0      719 2023-08-08 13:49:14.000000 tmxpy-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 13:49:31.619666 tmxpy-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 13:49:31.594644 tmxpy-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 13:49:31.604653 tmxpy-0.1.6/src/tmxpy/
+-rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.6/src/tmxpy/__init__.py
+-rw-rw-rw-   0        0        0    10865 2023-08-08 12:20:57.000000 tmxpy-0.1.6/src/tmxpy/tmxpy.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:49:31.615662 tmxpy-0.1.6/src/tmxpy.egg-info/
+-rw-rw-rw-   0        0        0     1890 2023-08-08 13:49:31.000000 tmxpy-0.1.6/src/tmxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-08-08 13:49:31.000000 tmxpy-0.1.6/src/tmxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:49:31.000000 tmxpy-0.1.6/src/tmxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-08-08 13:49:31.000000 tmxpy-0.1.6/src/tmxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 13:49:31.000000 tmxpy-0.1.6/src/tmxpy.egg-info/top_level.txt
```

### Comparing `tmxpy-0.1.5/LICENSE` & `tmxpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.5/PKG-INFO` & `tmxpy-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `tmxpy-0.1.5/README.md` & `tmxpy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.5/pyproject.toml` & `tmxpy-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tmxpy"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="AnotherPillow", email="redacted@email.xyz" }
 ]
 description = "A Python library for reading and writing TMX files."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tmxpy-0.1.5/src/tmxpy/tmxpy.py` & `tmxpy-0.1.6/src/tmxpy/tmxpy.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,26 +48,31 @@
         if path != '':
             self.path = path
             self.inputFile = bs4.BeautifulSoup(open(path), "xml")
         elif xml != '':
             self.inputFile = bs4.BeautifulSoup(xml, "xml")
         else:
             raise Exception("TMXpy: No path or xml given")
+        
+        map = self.inputFile.find("map")
+        if map is None:
+            raise Exception("TMXpy: No map element found")
+        
+        map = cast(dict, map)
+
+        self.tmxDimensions = (int(map['width']), int(map['height']))
 
         self.spriteSheetFolderPaths = sheets
 
     
     def generateGIDDict(self) -> None:
         """Generates a dictionary of GIDs to tile information"""
         tilesets = self.inputFile.find_all("tileset")
-        layer1 = cast(dict, self.inputFile.find('layer'))
 
-        
 
-        self.tmxDimensions = (int(layer1['width']), int(layer1['height']))
         for tileset in tilesets:
             self.tileDimensions = (int(tileset["tilewidth"]), int(tileset["tileheight"]))
             src = tileset.find("image")["source"]
 
             for i in range(int(tileset["firstgid"]), int(tileset["tilecount"]) + int(tileset["firstgid"])):
                 #<tileset firstgid="33" name="untitled tile sheet" tilewidth="16" tileheight="16" tilecount="1975" columns="25">
                 self.tiles[str(i)] = {
@@ -94,15 +99,22 @@
         if not path.endswith(ext):
             path += ext
         return path
         
 
     def renderTile(self, gid: str) -> Image.Image:
         """Renders a tile from the TMX file"""
-        tile = self.tiles[gid]
+        try:
+            tile = self.tiles[gid]
+        except KeyError:
+            # print(gid, self.tiles)
+            if str(gid) == "0":
+                return Image.new("RGBA", self.tileDimensions)
+            
+            raise Exception(f"TMXpy: Tile {gid} not found in tileset")
         
         #path = os.path.join(self.spriteSheetFolderPaths[0], tile["src"]) + ".png"
         path = self.findPathOfTileSheet(tile["src"], ".png")
         tilesheet = Image.open(path)
         
         tile = tilesheet.crop((tile["x"] * tile["width"], tile["y"] * tile["height"], tile["x"] * tile["width"] + tile["width"], tile["y"] * tile["height"] + tile["height"]))
         return tile
@@ -122,35 +134,46 @@
 
         for i, tile in enumerate(tiles):
             tile = tile.strip()
             if tile == "0":
                 continue
             if '\n' in tile:
                 tile = tile.split('\n')[0].strip()
-            img.paste(self.renderTile(tile), (int(i % int(layer['width'])) * int(self.tileDimensions[0]), int(i / int(layer['width'])) * int(self.tileDimensions[1])))
+            
+            render = self.renderTile(tile)
+            alpha = render.getchannel('A')
+            
+            img.paste(
+                self.renderTile(tile), 
+                (
+                    int(i % int(layer['width'])) * int(self.tileDimensions[0]),
+                    int(i / int(layer['width'])) * int(self.tileDimensions[1])
+                ),
+                alpha
+            )
 
         return img
     
     def renderAllLayers(self, blocked: list[str] = []) -> Image.Image:
         """Renders all layers in the TMX file, except for the ones in the blocked list"""
         width = int(self.tmxDimensions[0]) * int(self.tileDimensions[0])
         height = int(self.tmxDimensions[1]) * int(self.tileDimensions[1])
-        img = Image.new("RGBA", (width, height))
+        img = Image.new("RGBA", (width, height), (0, 0, 0, 0))
 
 
 
         
         for i, layer in enumerate(self.inputFile.find_all("layer")):
             if layer['name'] in blocked or str(i) in blocked or i in blocked:
                 # print(f'Skipping layer {layer["name"]} - {i}')
                 continue
             # print(f'Rendering layer {layer["name"]} - {i}')
             layer = self.renderLayer(i)
             #stick it on top of the last layer, and not overwriting the transparent pixels
-            img.paste(layer, (0, 0), layer)
+            img.paste(layer, (0, 0), layer.getchannel('A'))
             # print(f'Layer {i} rendered, layer width: {layer.width}, layer height: {layer.height} - img width: {width}, img height: {height}')
         return img
     
     def parseWarps(self) -> list[dict]:
         #extract property[name="Warp"]
         prop = cast(dict, self.inputFile.find("property", {"name": "Warp"}))
         if prop is None or prop == {}:
@@ -187,15 +210,15 @@
         elif layerName != "":
             layer = self.inputFile.find("layer", {"name": layerName})
         else:
             raise Exception("TMXpy: No layerID or layerName given")
         if layer is None:
             raise Exception("TMXpy: Layer not found")
         
-        rows = layer.text.split("\n")
+        rows = [x for x in layer.text.split("\n") if str(x) not in ["", " ", [], [""], [" "]]]
         columns = rows[y].split(",")
         
         columns[x] = tile
         rows[y] = ",".join(columns)
         output = "\n".join(rows)
         
         layer.contents[0].replace_with(output) # type: ignore <-- like wtf pylint why what is this
```

### Comparing `tmxpy-0.1.5/src/tmxpy.egg-info/PKG-INFO` & `tmxpy-0.1.6/src/tmxpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

