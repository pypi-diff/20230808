# Comparing `tmp/hpmoc-1.0a5.tar.gz` & `tmp/hpmoc-1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpmoc-1.0a5.tar", last modified: Thu Jul 13 23:20:06 2023, max compression
+gzip compressed data, was "hpmoc-1.0a6.tar", last modified: Tue Aug  1 09:56:54 2023, max compression
```

## Comparing `hpmoc-1.0a5.tar` & `hpmoc-1.0a6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a5/LICENSE
--rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a5/Makefile
--rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a5/README.md
--rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/.gitignore
--rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/make.bat
--rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/source/conf.py
--rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/source/index.rst
--rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/source/jup/plotting-examples.ipynb
--rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a5/hpmoc-dev-win.yml
--rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a5/hpmoc-dev.yml
--rw-r--r--   0        0        0     1032 2023-07-13 23:19:20.730072 hpmoc-1.0a5/hpmoc/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a5/hpmoc/abstract.py
--rw-r--r--   0        0        0     6201 2023-07-07 05:29:37.570077 hpmoc-1.0a5/hpmoc/arraysetops.py
--rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a5/hpmoc/healpy.py
--rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a5/hpmoc/healpy_utils.py
--rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a5/hpmoc/io/__init__.py
--rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a5/hpmoc/io/abstract.py
--rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a5/hpmoc/io/astroquery.py
--rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a5/hpmoc/io/fits.py
--rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a5/hpmoc/io/gracedb.py
--rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a5/hpmoc/io/ligo.py
--rw-r--r--   0        0        0    54608 2023-07-13 23:18:30.270072 hpmoc-1.0a5/hpmoc/partial.py
--rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a5/hpmoc/plot.py
--rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a5/hpmoc/plotters.py
--rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a5/hpmoc/points.py
--rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a5/hpmoc/psf.py
--rw-r--r--   0        0        0    93078 2023-07-07 05:26:12.900078 hpmoc-1.0a5/hpmoc/utils.py
--rw-r--r--   0        0        0     1768 2023-07-13 22:48:45.670065 hpmoc-1.0a5/pyproject.toml
--rw-r--r--   0        0        0     5458 1970-01-01 00:00:00.000000 hpmoc-1.0a5/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a6/LICENSE
+-rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a6/Makefile
+-rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a6/README.md
+-rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a6/docs/.gitignore
+-rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a6/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a6/docs/make.bat
+-rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a6/docs/source/conf.py
+-rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a6/docs/source/index.rst
+-rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a6/docs/source/jup/plotting-examples.ipynb
+-rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a6/hpmoc-dev-win.yml
+-rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a6/hpmoc-dev.yml
+-rw-r--r--   0        0        0     1032 2023-08-01 09:55:47.280395 hpmoc-1.0a6/hpmoc/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a6/hpmoc/abstract.py
+-rw-r--r--   0        0        0     6201 2023-07-07 05:29:37.570077 hpmoc-1.0a6/hpmoc/arraysetops.py
+-rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a6/hpmoc/healpy.py
+-rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a6/hpmoc/healpy_utils.py
+-rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a6/hpmoc/io/__init__.py
+-rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a6/hpmoc/io/abstract.py
+-rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a6/hpmoc/io/astroquery.py
+-rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a6/hpmoc/io/fits.py
+-rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a6/hpmoc/io/gracedb.py
+-rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a6/hpmoc/io/ligo.py
+-rw-r--r--   0        0        0    54608 2023-07-13 23:18:30.270072 hpmoc-1.0a6/hpmoc/partial.py
+-rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a6/hpmoc/plot.py
+-rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a6/hpmoc/plotters.py
+-rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a6/hpmoc/points.py
+-rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a6/hpmoc/psf.py
+-rw-r--r--   0        0        0    93071 2023-08-01 09:55:22.130395 hpmoc-1.0a6/hpmoc/utils.py
+-rw-r--r--   0        0        0     1768 2023-07-13 22:48:45.670065 hpmoc-1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     5458 1970-01-01 00:00:00.000000 hpmoc-1.0a6/PKG-INFO
```

### Comparing `hpmoc-1.0a5/LICENSE` & `hpmoc-1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/Makefile` & `hpmoc-1.0a6/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/README.md` & `hpmoc-1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/docs/Makefile` & `hpmoc-1.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/docs/make.bat` & `hpmoc-1.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/docs/source/conf.py` & `hpmoc-1.0a6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/docs/source/index.rst` & `hpmoc-1.0a6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/docs/source/jup/plotting-examples.ipynb` & `hpmoc-1.0a6/docs/source/jup/plotting-examples.ipynb`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc-dev-win.yml` & `hpmoc-1.0a6/hpmoc-dev-win.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc-dev.yml` & `hpmoc-1.0a6/hpmoc-dev.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/__init__.py` & `hpmoc-1.0a6/hpmoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 """
 HPMOC is an ultra high-performance, cross-platform toolset for working with
 multi-order coordinate (MOC) HEALPix images (i.e. images with multiple pixel
 resolutions).
 """
 
-__version__ = '1.0a5'
+__version__ = '1.0a6'
 
 from .partial import PartialUniqSkymap as PartialUniqSkymap
```

### Comparing `hpmoc-1.0a5/hpmoc/abstract.py` & `hpmoc-1.0a6/hpmoc/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/arraysetops.py` & `hpmoc-1.0a6/hpmoc/arraysetops.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/healpy.py` & `hpmoc-1.0a6/hpmoc/healpy.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/healpy_utils.py` & `hpmoc-1.0a6/hpmoc/healpy_utils.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/io/__init__.py` & `hpmoc-1.0a6/hpmoc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/io/abstract.py` & `hpmoc-1.0a6/hpmoc/io/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/io/astroquery.py` & `hpmoc-1.0a6/hpmoc/io/astroquery.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/io/fits.py` & `hpmoc-1.0a6/hpmoc/io/fits.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/io/gracedb.py` & `hpmoc-1.0a6/hpmoc/io/gracedb.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/io/ligo.py` & `hpmoc-1.0a6/hpmoc/io/ligo.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/partial.py` & `hpmoc-1.0a6/hpmoc/partial.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/plot.py` & `hpmoc-1.0a6/hpmoc/plot.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/plotters.py` & `hpmoc-1.0a6/hpmoc/plotters.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/points.py` & `hpmoc-1.0a6/hpmoc/points.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/psf.py` & `hpmoc-1.0a6/hpmoc/psf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/hpmoc/utils.py` & `hpmoc-1.0a6/hpmoc/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,17 +167,17 @@
         the declination (in degrees) of each pixel. You can get each of these
         individually with ``ra, dec = nest2ang(...)``.
     """
     from astropy.units import degree  # pylint: disable=no-name-in-module
 
     nside = np.full(n.shape, nside) if isinstance(nside, Integral) else nside
     ra_dec = np.ndarray((2, len(n)))                    # pre-allocate results
-    for nside in np.unique(nside):                            # iterate NSIDE values
-        i = np.nonzero(nside == nside)[0]
-        ra_dec[:, i] = np.array(hp.pix2ang(nside, n[i], nest=True, lonlat=True))
+    for ns in np.unique(nside):                            # iterate NSIDE values
+        i = np.nonzero(nside == ns)[0]
+        ra_dec[:, i] = np.array(hp.pix2ang(ns, n[i], nest=True, lonlat=True))
     return ra_dec*degree
 
 
 def resol2nside(res, coarse=False, degrees=True):
     """Get the HEALPix NSIDE value corresponding to a given resolution.
 
     Parameters
@@ -304,16 +304,16 @@
 
     See Also
     --------
     nest2dangle
     """
     [uˢ], _, o⃗, _, [v⃗], [u̇ˢ] = nside_slices(u, return_inverse=True,
                                             dtype=float)
-    nside = 1 << o⃗                                     # NSIDE for each view
-    for nside, v⃗ⁱ in zip(nside, v⃗):                       # views into uˢ
+    nsides = 1 << o⃗                                     # NSIDE for each view
+    for nside, v⃗ⁱ in zip(nsides, v⃗):                       # views into uˢ
         v⃗ⁱ -= 4*nside**2                               # convert to nest in-place
         u = nest2dangle(v⃗ⁱ, nside, ra, dec, degrees=degrees, in_place=True).unit
     return uˢ[u̇ˢ]*u                                 # unsort results in uˢ*
 
 
 def dangle_rad(ra, dec, mapra, mapdec):  # pylint: disable=invalid-name
     """Get an array of angular distances in radians between the point specified
```

### Comparing `hpmoc-1.0a5/pyproject.toml` & `hpmoc-1.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a5/PKG-INFO` & `hpmoc-1.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpmoc
-Version: 1.0a5
+Version: 1.0a6
 Summary: HPMOC is an ultra high-performance, cross-platform toolset for working with
 Author-email: Stefan Trklja Countryman <stefan.countryman@gmail.com>
 Maintainer-email: Albert Zhang <alchzh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: IPython
```

