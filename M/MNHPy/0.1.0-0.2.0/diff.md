# Comparing `tmp/MNHPy-0.1.0.tar.gz` & `tmp/MNHPy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MNHPy-0.1.0.tar", last modified: Wed Jun  1 21:19:00 2022, max compression
+gzip compressed data, was "MNHPy-0.2.0.tar", last modified: Wed Jun  8 12:14:37 2022, max compression
```

## Comparing `MNHPy-0.1.0.tar` & `MNHPy-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-01 21:19:00.624034 MNHPy-0.1.0/
--rw-r--r--   0 rodierq  (24296) phynh     (3201)      451 2022-06-01 21:19:00.624034 MNHPy-0.1.0/PKG-INFO
--rw-r--r--   0 rodierq  (24296) phynh     (3201)      262 2022-06-01 21:17:45.000000 MNHPy-0.1.0/README.md
--rw-r--r--   0 rodierq  (24296) phynh     (3201)       38 2022-06-01 21:19:00.624034 MNHPy-0.1.0/setup.cfg
--rw-r--r--   0 rodierq  (24296) phynh     (3201)      780 2022-06-01 21:18:07.000000 MNHPy-0.1.0/setup.py
-drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-01 21:19:00.620034 MNHPy-0.1.0/src/
-drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-01 21:19:00.620034 MNHPy-0.1.0/src/MNHPy/
--rw-r--r--   0 rodierq  (24296) phynh     (3201)    52870 2022-06-01 10:47:08.000000 MNHPy-0.1.0/src/MNHPy/Panel_Plot.py
--rw-r--r--   0 rodierq  (24296) phynh     (3201)      433 2022-06-01 12:03:16.000000 MNHPy-0.1.0/src/MNHPy/__init__.py
--rw-r--r--   0 rodierq  (24296) phynh     (3201)     7167 2022-06-01 21:06:37.000000 MNHPy-0.1.0/src/MNHPy/misc_functions.py
--rw-r--r--   0 rodierq  (24296) phynh     (3201)    19338 2022-06-01 09:55:11.000000 MNHPy-0.1.0/src/MNHPy/read_MNHfile.py
-drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-01 21:19:00.624034 MNHPy-0.1.0/src/MNHPy.egg-info/
--rw-r--r--   0 rodierq  (24296) phynh     (3201)      451 2022-06-01 21:19:00.000000 MNHPy-0.1.0/src/MNHPy.egg-info/PKG-INFO
--rw-r--r--   0 rodierq  (24296) phynh     (3201)      282 2022-06-01 21:19:00.000000 MNHPy-0.1.0/src/MNHPy.egg-info/SOURCES.txt
--rw-r--r--   0 rodierq  (24296) phynh     (3201)        1 2022-06-01 21:19:00.000000 MNHPy-0.1.0/src/MNHPy.egg-info/dependency_links.txt
--rw-r--r--   0 rodierq  (24296) phynh     (3201)       74 2022-06-01 21:19:00.000000 MNHPy-0.1.0/src/MNHPy.egg-info/requires.txt
--rw-r--r--   0 rodierq  (24296) phynh     (3201)        6 2022-06-01 21:19:00.000000 MNHPy-0.1.0/src/MNHPy.egg-info/top_level.txt
+drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-08 12:14:37.505459 MNHPy-0.2.0/
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)      487 2022-06-08 12:14:37.501459 MNHPy-0.2.0/PKG-INFO
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)      262 2022-06-01 21:17:45.000000 MNHPy-0.2.0/README.md
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)       38 2022-06-08 12:14:37.505459 MNHPy-0.2.0/setup.cfg
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)      849 2022-06-08 12:14:32.000000 MNHPy-0.2.0/setup.py
+drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-08 12:14:37.501459 MNHPy-0.2.0/src/
+drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-08 12:14:37.501459 MNHPy-0.2.0/src/MNHPy/
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)    53004 2022-06-07 14:57:11.000000 MNHPy-0.2.0/src/MNHPy/Panel_Plot.py
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)      433 2022-06-01 12:03:16.000000 MNHPy-0.2.0/src/MNHPy/__init__.py
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)     7167 2022-06-01 21:06:37.000000 MNHPy-0.2.0/src/MNHPy/misc_functions.py
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)    19338 2022-06-01 09:55:11.000000 MNHPy-0.2.0/src/MNHPy/read_MNHfile.py
+drwxr-xr-x   0 rodierq  (24296) phynh     (3201)        0 2022-06-08 12:14:37.501459 MNHPy-0.2.0/src/MNHPy.egg-info/
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)      487 2022-06-08 12:14:37.000000 MNHPy-0.2.0/src/MNHPy.egg-info/PKG-INFO
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)      282 2022-06-08 12:14:37.000000 MNHPy-0.2.0/src/MNHPy.egg-info/SOURCES.txt
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)        1 2022-06-08 12:14:37.000000 MNHPy-0.2.0/src/MNHPy.egg-info/dependency_links.txt
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)       74 2022-06-08 12:14:37.000000 MNHPy-0.2.0/src/MNHPy.egg-info/requires.txt
+-rw-r--r--   0 rodierq  (24296) phynh     (3201)        6 2022-06-08 12:14:37.000000 MNHPy-0.2.0/src/MNHPy.egg-info/top_level.txt
```

### Comparing `MNHPy-0.1.0/setup.py` & `MNHPy-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from setuptools import setup
 
 MAINTAINER_EMAIL = 'mesonhsupport@obs-mip.fr'
 AUTHORS = 'Quentin Rodier & Meso-NH Team'
 
 setup(
    name='MNHPy',
-   version='0.1.0',
+   version='0.2.0',
    description=('Python visulization tools for MesoNH atmospheric research model'),
+   long_description=('Compatible with Meso-NH model version 5.5.1'),
    author=AUTHORS,
    author_email=MAINTAINER_EMAIL,
    url='https://github.com/QuentinRodier/MNHPy',
    classifiers=[
        "Programming Language :: Python :: 3",
        "License :: CeCILL-C Free Software License Agreement (CECILL-C)"],
    packages=['MNHPy'],	#name of package (dir with the modules)
```

### Comparing `MNHPy-0.1.0/src/MNHPy/Panel_Plot.py` & `MNHPy-0.2.0/src/MNHPy/Panel_Plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,28 +79,29 @@
           Handle drawing of the background plot (coastlines, departements, grid lines and labels)
         """
         self.drawCoastLines = drawCoastLines
         self.projo = projo
 
         #  Grid lines and labels
         gl = ax.gridlines(crs=self.projo, draw_labels=True, linewidth=1, color='gray')
-        print(cartopy.__version__[:4])
         if float(cartopy.__version__[:4]) >= 0.18:
+            from cartopy.mpl.ticker import (LatitudeLocator, LongitudeLocator,LongitudeFormatter, LatitudeFormatter) 
             gl.top_labels = False
             gl.right_labels = False
-            gl.xlines = False
+            gl.xlines = True
+            gl.ylines = True
             gl.xlocator = LongitudeLocator()
             gl.ylocator = LatitudeLocator()
             gl.xformatter = LongitudeFormatter()
             gl.yformatter = LatitudeFormatter()
         else:
             gl.xlabels_top = False
             gl.ylabels_right = False
-        gl.xlabel_style = {'size': self.xyTicksLabelSize, 'color': 'gray'}
-        gl.ylabel_style = {'size': self.xyTicksLabelSize, 'color': 'gray'}
+        gl.xlabel_style = {'size': self.xyTicksLabelSize, 'color': 'black'}
+        gl.ylabel_style = {'size': self.xyTicksLabelSize, 'color': 'black'}
 
         #  Coastlines
         if self.drawCoastLines and 'GeoAxes' in str(type(ax)):
             ax.coastlines(resolution='10m', color='black', linewidth=1)
 
             #  Countries border
             ax.add_feature(cfeature.BORDERS)
@@ -643,28 +644,28 @@
                 Lcolormap[i] = self.addWhitecm(Lcolormap[i], len(levels_contour), LwhiteTop[i])
 
             #  Plot
             if Lproj:
                 if Lpltype[i] == 'c':  # Contour
                     if LcolorLine:
                         cf = self.ax[iax].contour(lon[i], lat[i], vartoPlot * Lfacconv[i], levels=levels_contour, transform=Lproj[i],
-                                                  norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], colors=LcolorLine[i])
+                                                  norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], colors=LcolorLine[i],linewidths=Llinewidth[i])
                     else:
                         cf = self.ax[iax].contour(lon[i], lat[i], vartoPlot * Lfacconv[i], levels=levels_contour, transform=Lproj[i],
-                                                  norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], cmap=Lcolormap[i])
+                                                  norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], cmap=Lcolormap[i],linewidths=Llinewidth[i])
                 else:
                     cf = self.ax[iax].contourf(lon[i], lat[i], vartoPlot * Lfacconv[i], levels=levels_contour, transform=Lproj[i],
                                                norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], cmap=Lcolormap[i])
             else:  # Cartesian coordinates
                 if Lpltype[i] == 'c':  # Contour
                     cf = self.ax[iax].contour(lon[i], lat[i], vartoPlot * Lfacconv[i], levels=levels_contour,
                                               norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], colors=LcolorLine[i],linewidths=Llinewidth[i])
                 else:
                     cf = self.ax[iax].contourf(lon[i], lat[i], vartoPlot * Lfacconv[i], levels=levels_contour,
-                                               norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], cmap=Lcolormap[i],linewidths=Llinewidth[i])
+                                               norm=norm, vmin=Lminval[i], vmax=Lmaxval[i], cmap=Lcolormap[i])
             #  Title
             self.set_Title(self.ax, iax, Ltitle[i], Lid_overlap, Lxlab[i], Lylab[i])
 
             #  Coastlines / Grid lines and labels
             if Lproj:
                 self.draw_Backmap(coastLines, self.ax[iax], Lproj[i])
```

### Comparing `MNHPy-0.1.0/src/MNHPy/misc_functions.py` & `MNHPy-0.2.0/src/MNHPy/misc_functions.py`

 * *Files identical despite different names*

### Comparing `MNHPy-0.1.0/src/MNHPy/read_MNHfile.py` & `MNHPy-0.2.0/src/MNHPy/read_MNHfile.py`

 * *Files identical despite different names*

