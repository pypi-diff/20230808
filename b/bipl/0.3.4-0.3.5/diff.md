# Comparing `tmp/bipl-0.3.4.tar.gz` & `tmp/bipl-0.3.5.tar.gz`

## Comparing `bipl-0.3.4.tar` & `bipl-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/_env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_gdal.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_util.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.4/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.4/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.4/hatch_build.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bipl-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 bipl-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_gdal.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/io/_util.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    15598 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 bipl-0.3.5/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.5/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.5/hatch_build.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bipl-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 bipl-0.3.5/PKG-INFO
```

### Comparing `bipl-0.3.4/src/bipl/io/__init__.py` & `bipl-0.3.5/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_dzi.py` & `bipl-0.3.5/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_gdal.py` & `bipl-0.3.5/src/bipl/io/_gdal.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_libs.py` & `bipl-0.3.5/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_openslide.py` & `bipl-0.3.5/src/bipl/io/_openslide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_slide.py` & `bipl-0.3.5/src/bipl/io/_slide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_slide_bases.py` & `bipl-0.3.5/src/bipl/io/_slide_bases.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_tiff.py` & `bipl-0.3.5/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/io/_util.py` & `bipl-0.3.5/src/bipl/io/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/src/bipl/ops/_mosaic.py` & `bipl-0.3.5/src/bipl/ops/_mosaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
 
 def get_fusion(tiles: Iterable[Tile],
                shape: tuple[int, ...] | None = None) -> np.ndarray | None:
     r: np.ndarray | None = None
 
     if shape is None:  # Collect all the tiles to compute destination size
         tiles = [*tiles]
+        if not tiles:
+            return None
         # N arrays of (yx + hw)
         yx_hw = np.array([[[t.vec, t.data.shape[:2]] for t in tiles]]).sum(1)
         # bottom left most edge
         shape = *yx_hw.max(0).tolist(),
     else:
         assert len(shape) == 2
 
@@ -204,30 +206,42 @@
                 Mosaic(self.m.step // stride, self.m.overlap // stride), shape,
                 self.cells, stride, self))
 
     def crop(self) -> _BaseView:
         return _IterView(self.m, self.shape, self.cells, _crop(
             self, self.shape))
 
-    def zip_with(
-            self, view: np.ndarray,
-            v_scale: int) -> Iterator[tuple[Vec, Vec, np.ndarray, np.ndarray]]:
+    def zip_with(self, view: np.ndarray, v_scale: int) -> _ZipView:
         """Extracts tiles from `view` simultaneously with tiles from self"""
         assert v_scale >= 1
-        for tile in self:
-            tw, th = tile.data.shape[:2]
-            v = view[tile.vec[0] // v_scale:,
-                     tile.vec[1] // v_scale:][:tw // v_scale, :th // v_scale]
-            yield tile.idx, tile.vec, tile.data, v
+        return _ZipView(self, view, v_scale)
 
     def with_cm(self: _Self, cm: AbstractContextManager) -> _Self:
         return cast(_Self, _CmView(self.m, self.shape, self.cells, self, cm))
 
 
 @dataclass
+class _ZipView:
+    source: _BaseView
+    view: NumpyLike
+    v_scale: int
+
+    def __len__(self) -> int:
+        return len(self.source)
+
+    def __iter__(self) -> Iterator[tuple[Vec, Vec, np.ndarray, np.ndarray]]:
+        assert self.v_scale >= 1
+        scale = self.v_scale
+        for tile in self.source:
+            loc = *(slice(o // scale, (o + s) // scale)
+                    for o, s in zip(tile.vec, tile.data.shape[:2])),
+            yield tile.idx, tile.vec, tile.data, self.view[loc]
+
+
+@dataclass
 class _View(_BaseView):
     def map_batched(self,
                     fn: Callable[[list[np.ndarray]], Iterable[np.ndarray]],
                     /,
                     batch_size: int = 1,
                     max_workers: int = 0) -> _View:
         """
```

### Comparing `bipl-0.3.4/src/bipl/ops/_util.py` & `bipl-0.3.5/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/LICENSE` & `bipl-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/README.md` & `bipl-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/hatch_build.py` & `bipl-0.3.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.4/pyproject.toml` & `bipl-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.3.4"
+version = "0.3.5"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `bipl-0.3.4/PKG-INFO` & `bipl-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.3.4
+Version: 0.3.5
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

