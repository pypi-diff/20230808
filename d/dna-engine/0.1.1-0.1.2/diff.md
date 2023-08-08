# Comparing `tmp/dna_engine-0.1.1.tar.gz` & `tmp/dna_engine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_engine-0.1.1.tar", last modified: Tue Aug  8 18:46:27 2023, max compression
+gzip compressed data, was "dna_engine-0.1.2.tar", last modified: Tue Aug  8 18:50:20 2023, max compression
```

## Comparing `dna_engine-0.1.1.tar` & `dna_engine-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 18:46:27.126516 dna_engine-0.1.1/
--rw-rw-rw-   0        0        0      609 2023-08-08 18:46:27.126516 dna_engine-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 18:46:27.062903 dna_engine-0.1.1/dna_engine/
--rw-rw-rw-   0        0        0      445 2023-08-08 18:30:31.000000 dna_engine-0.1.1/dna_engine/__init__.py
--rw-rw-rw-   0        0        0    17596 2023-08-08 18:41:32.000000 dna_engine-0.1.1/dna_engine/actor.py
--rw-rw-rw-   0        0        0     4866 2023-07-24 10:44:53.000000 dna_engine-0.1.1/dna_engine/audio_manager.py
--rw-rw-rw-   0        0        0     3216 2023-07-20 19:38:19.000000 dna_engine-0.1.1/dna_engine/background.py
--rw-rw-rw-   0        0        0    10622 2023-08-08 18:41:12.000000 dna_engine-0.1.1/dna_engine/game.py
--rw-rw-rw-   0        0        0     6990 2023-07-24 11:12:58.000000 dna_engine-0.1.1/dna_engine/input_manager.py
--rw-rw-rw-   0        0        0    11268 2023-07-31 17:33:20.000000 dna_engine-0.1.1/dna_engine/text.py
-drwxrwxrwx   0        0        0        0 2023-08-08 18:46:27.126516 dna_engine-0.1.1/dna_engine/tilemaps/
--rw-rw-rw-   0        0        0      123 2023-08-08 18:29:52.000000 dna_engine-0.1.1/dna_engine/tilemaps/__init__.py
--rw-rw-rw-   0        0        0     2635 2023-07-30 19:09:28.000000 dna_engine-0.1.1/dna_engine/tilemaps/tile.py
--rw-rw-rw-   0        0        0     3370 2023-07-11 16:44:30.000000 dna_engine-0.1.1/dna_engine/tilemaps/tile_map.py
--rw-rw-rw-   0        0        0    10495 2023-08-08 18:43:03.000000 dna_engine-0.1.1/dna_engine/world.py
-drwxrwxrwx   0        0        0        0 2023-08-08 18:46:27.121003 dna_engine-0.1.1/dna_engine.egg-info/
--rw-rw-rw-   0        0        0      609 2023-08-08 18:46:26.000000 dna_engine-0.1.1/dna_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-08-08 18:46:26.000000 dna_engine-0.1.1/dna_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 18:46:26.000000 dna_engine-0.1.1/dna_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-08-08 18:46:26.000000 dna_engine-0.1.1/dna_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-08 18:46:26.000000 dna_engine-0.1.1/dna_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 18:46:27.126516 dna_engine-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1168 2023-08-08 18:46:14.000000 dna_engine-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:50:20.280566 dna_engine-0.1.2/
+-rw-rw-rw-   0        0        0      609 2023-08-08 18:50:20.271604 dna_engine-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 18:50:20.178286 dna_engine-0.1.2/dna_engine/
+-rw-rw-rw-   0        0        0      445 2023-08-08 18:30:31.000000 dna_engine-0.1.2/dna_engine/__init__.py
+-rw-rw-rw-   0        0        0    17596 2023-08-08 18:41:32.000000 dna_engine-0.1.2/dna_engine/actor.py
+-rw-rw-rw-   0        0        0     4866 2023-07-24 10:44:53.000000 dna_engine-0.1.2/dna_engine/audio_manager.py
+-rw-rw-rw-   0        0        0     3216 2023-07-20 19:38:19.000000 dna_engine-0.1.2/dna_engine/background.py
+-rw-rw-rw-   0        0        0    10622 2023-08-08 18:41:12.000000 dna_engine-0.1.2/dna_engine/game.py
+-rw-rw-rw-   0        0        0     6990 2023-07-24 11:12:58.000000 dna_engine-0.1.2/dna_engine/input_manager.py
+-rw-rw-rw-   0        0        0    11268 2023-07-31 17:33:20.000000 dna_engine-0.1.2/dna_engine/text.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:50:20.271604 dna_engine-0.1.2/dna_engine/tilemaps/
+-rw-rw-rw-   0        0        0      123 2023-08-08 18:29:52.000000 dna_engine-0.1.2/dna_engine/tilemaps/__init__.py
+-rw-rw-rw-   0        0        0     2635 2023-07-30 19:09:28.000000 dna_engine-0.1.2/dna_engine/tilemaps/tile.py
+-rw-rw-rw-   0        0        0     3359 2023-08-08 18:49:41.000000 dna_engine-0.1.2/dna_engine/tilemaps/tile_map.py
+-rw-rw-rw-   0        0        0    10495 2023-08-08 18:43:03.000000 dna_engine-0.1.2/dna_engine/world.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:50:20.230834 dna_engine-0.1.2/dna_engine.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-08-08 18:50:19.000000 dna_engine-0.1.2/dna_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-08-08 18:50:19.000000 dna_engine-0.1.2/dna_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:50:19.000000 dna_engine-0.1.2/dna_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-08 18:50:19.000000 dna_engine-0.1.2/dna_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 18:50:19.000000 dna_engine-0.1.2/dna_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 18:50:20.280566 dna_engine-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-08-08 18:50:12.000000 dna_engine-0.1.2/setup.py
```

### Comparing `dna_engine-0.1.1/PKG-INFO` & `dna_engine-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna_engine
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-0.1.1/dna_engine/actor.py` & `dna_engine-0.1.2/dna_engine/actor.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/audio_manager.py` & `dna_engine-0.1.2/dna_engine/audio_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/background.py` & `dna_engine-0.1.2/dna_engine/background.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/game.py` & `dna_engine-0.1.2/dna_engine/game.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/input_manager.py` & `dna_engine-0.1.2/dna_engine/input_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/text.py` & `dna_engine-0.1.2/dna_engine/text.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/tilemaps/tile.py` & `dna_engine-0.1.2/dna_engine/tilemaps/tile.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine/tilemaps/tile_map.py` & `dna_engine-0.1.2/dna_engine/tilemaps/tile_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pygame.rect import Rect
 from pygame.surface import Surface
 
-from dna_engine.dna_engine.tilemaps.tile import Tile
+from dna_engine.tilemaps.tile import Tile
 
 class TileMap:
     def __init__(self, world, grid_width : int, grid_height : int, pixels_apart: int) -> None:
         self.__world = world
         self.__pixel_difference = max(0, pixels_apart)
         self.__tiles = [[None for i in range(max(0, grid_height))] for j in range(max(0, grid_width))]
         self.__tile_width = (self.__world.get_width() / grid_width) - pixels_apart
```

### Comparing `dna_engine-0.1.1/dna_engine/world.py` & `dna_engine-0.1.2/dna_engine/world.py`

 * *Files identical despite different names*

### Comparing `dna_engine-0.1.1/dna_engine.egg-info/PKG-INFO` & `dna_engine-0.1.2/dna_engine.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna-engine
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-0.1.1/setup.py` & `dna_engine-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1' 
+VERSION = '0.1.2' 
 DESCRIPTION = 'PyGame Abstraction Library'
 LONG_DESCRIPTION = 'A library of code which presents users with a simple, extensible program structure to make simple, 2D games with. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="dna_engine",
```

