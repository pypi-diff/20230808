# Comparing `tmp/pybarnes-0.1.1.tar.gz` & `tmp/pybarnes-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarnes-0.1.1.tar", last modified: Mon Apr 10 09:21:11 2023, max compression
+gzip compressed data, was "pybarnes-0.2.0a0.tar", last modified: Tue Aug  8 15:33:50 2023, max compression
```

## Comparing `pybarnes-0.1.1.tar` & `pybarnes-0.2.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-04-10 09:21:11.575901 pybarnes-0.1.1/
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       71 2023-04-10 09:21:11.575901 pybarnes-0.1.1/PKG-INFO
-drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-04-10 09:21:11.572568 pybarnes-0.1.1/pybarnes/
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       63 2023-04-10 09:20:54.000000 pybarnes-0.1.1/pybarnes/__init__.py
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)     8477 2023-04-10 08:50:32.000000 pybarnes-0.1.1/pybarnes/barnes_filter.py
-drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-04-10 09:21:11.575901 pybarnes-0.1.1/pybarnes.egg-info/
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       71 2023-04-10 09:21:11.000000 pybarnes-0.1.1/pybarnes.egg-info/PKG-INFO
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)      214 2023-04-10 09:21:11.000000 pybarnes-0.1.1/pybarnes.egg-info/SOURCES.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)        1 2023-04-10 09:21:11.000000 pybarnes-0.1.1/pybarnes.egg-info/dependency_links.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)        6 2023-04-10 09:21:11.000000 pybarnes-0.1.1/pybarnes.egg-info/requires.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)        9 2023-04-10 09:21:11.000000 pybarnes-0.1.1/pybarnes.egg-info/top_level.txt
--rw-r--r--   0 ouyang    (1000) ouyang    (1000)       38 2023-04-10 09:21:11.575901 pybarnes-0.1.1/setup.cfg
--rwxr-xr-x   0 ouyang    (1000) ouyang    (1000)      186 2023-04-10 08:51:08.000000 pybarnes-0.1.1/setup.py
+drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       73 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/PKG-INFO
+drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-08 15:33:50.350612 pybarnes-0.2.0a0/pybarnes/
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       91 2023-08-08 15:31:54.000000 pybarnes-0.2.0a0/pybarnes/__init__.py
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)    12031 2023-08-08 15:27:36.000000 pybarnes-0.2.0a0/pybarnes/barnes_filter.py
+drwxr-xr-x   0 ouyang    (1000) ouyang    (1000)        0 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/pybarnes.egg-info/
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       73 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/PKG-INFO
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)      214 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/SOURCES.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)        1 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/dependency_links.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)        6 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/requires.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)        9 2023-08-08 15:33:50.000000 pybarnes-0.2.0a0/pybarnes.egg-info/top_level.txt
+-rw-r--r--   0 ouyang    (1000) ouyang    (1000)       38 2023-08-08 15:33:50.353946 pybarnes-0.2.0a0/setup.cfg
+-rwxr-xr-x   0 ouyang    (1000) ouyang    (1000)      192 2023-08-08 15:30:04.000000 pybarnes-0.2.0a0/setup.py
```

### Comparing `pybarnes-0.1.1/pybarnes/barnes_filter.py` & `pybarnes-0.2.0a0/pybarnes/barnes_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         D[..., i, -radius_grid[0]:, :, :] = data[..., None, idx, -grids[0]:]
     D[..., :radius_grid[1], :radius_grid[0], :, :] = data[..., None, None, :grids[1], :grids[0]]
     D[..., :radius_grid[1], -radius_grid[0]:, :, :] = data[..., None, None, :grids[1], -grids[0]:]
     D[..., -radius_grid[1]:, :radius_grid[0], :, :] = data[..., None, None, -grids[1]:, :grids[0]]
     D[..., -radius_grid[1]:, -radius_grid[0]:, :, :] = data[..., None, None, -grids[1]:, -grids[0]:]
     return D
 
+def get_lon_distance(x, y):
+    dlon1 = np.abs(x[:, None] - y)
+    dlon2 = np.abs(x[:, None] - y - 360)
+    return np.min(np.stack((dlon1, dlon2), axis=0), axis=0)
 
 class BarnesFilter:
 
     """
     The Barnes method performs grid point interpolation by selecting appropriate
     filtering parameters *c* and *g* to filter out shortwave noise in the original field,
     making the analysis results stable and smooth. In addition, it can form a bandpass filter
@@ -51,15 +55,15 @@
     achieving the purpose of scale separation.
 
     Reference:
     DOI : https://doi.org/10.1175/1520-0493(1980)108<1108:AOTFSM>2.0.CO;2
     """
 
 
-    def __init__(self, data_arr, lon=None, lat=None, radius_degree=10):
+    def __init__(self, data_arr, lon=None, lat=None, radius_degree=8):
         """
         Initializing the data and caculate the distance.
 
 
         Parameters
         ----------
         data_arr : numpy.array or xarray.Dataset or xarray.DataArray
@@ -207,7 +211,87 @@
             Mesoscale wave field filtered out from raw data
         """
         lowpass1 = self.__lowpass(g1, c1)
         lowpass2 = self.__lowpass(g2, c2)
         return self.__convert_data(lowpass1 - lowpass2)
 
 
+class BarnesFilter4Scatter:
+
+    def __init__(self, lon, lat, data_arr, radius_degree=10, neighbor_dots=None):
+        assert data_arr.ndim == lon.ndim == lat.ndim == 1
+        idx = np.isnan(data_arr)
+        if idx.sum() > 0:
+            data = data_arr[~idx]
+            lon = lon[~idx]
+            lat = lat[~idx]
+        self.ndots = len(data_arr)
+        self.lon = lon
+        self.data = data_arr
+        self.lat = lat
+
+        lat0, lon0 = np.mean(self.lat), np.mean(self.lon)
+        self.factor = 6370 * np.cos(np.deg2rad(lat0)) * np.pi/180
+        deg2center = np.sqrt((self.lon - lon0) ** 2 + (self.lat - lat0) ** 2)
+        if neighbor_dots is None:
+            self.dots = max((deg2center <= radius_degree).sum(), 1)
+        else:
+            self.dots = neighbor_dots
+        self.thereshold = 10000
+        self.__distance_data_field()
+
+    def __distance_data_field(self):
+        if self.ndots < self.thereshold:
+            dlon, dlat = get_lon_distance(self.lon, self.lon), self.lat[:, None] - self.lat
+            ddeg2 = dlon ** 2 + dlat ** 2
+            k2 = ddeg2 * self.factor ** 2
+            self.idx = np.argsort(k2, axis=-1)[:, :self.dots]
+            self.kilometer_distance2 = k2[np.arange(self.ndots)[:, None], self.idx]
+        else:
+            pts = np.stack((self.lon, self.lat), 0)
+            kilometer_distance2, idx = [], []
+            for x, y in np.array_split(pts, self.thereshold, axis=1):
+                dlon = get_lon_distance(x, self.lon)
+                dlat = y[:, None] - self.lat
+                ddeg2 = dlon ** 2 + dlat ** 2
+                k2 = ddeg2 * self.factor ** 2
+                ind = np.argsort(k2, axis=-1)[:, :self.dots]
+                kilometer_distance2.append(k2[np.arange(len(x))[:, None], ind])
+                idx.append(ind)
+            self.idx = np.concatenate(idx, 0)
+            self.kilometer_distance2 = np.concatenate(kilometer_distance2, 0)
+    
+    def __make_datafield(self, data):
+        return data[self.idx]
+
+    def lowpass(self, g=0.3, c=150000):
+        weights1 = np.exp(-self.kilometer_distance2/(4*c))
+        sum_weights1 = np.sum(weights1, -1, keepdims=True)
+        normed_weights1 = weights1/sum_weights1
+        del weights1, sum_weights1
+        weights2 = np.exp(-self.kilometer_distance2/(4*g*c))
+        sum_weights2 = np.sum(weights2, -1, keepdims=True)
+        normed_weights2 = weights2/sum_weights2
+        del weights2, sum_weights2
+        data = self.__make_datafield(self.data)
+        revision1 = np.sum(data * normed_weights1, -1)
+        diff = self.__make_datafield(self.data - revision1)
+        weighted_diff = np.sum(diff * normed_weights2, -1)
+        revision2 = revision1 + weighted_diff
+        return xr.DataArray(revision2, dict(lon=(("dots",), self.lon), lat=(("dots", ), self.lat)), dims=("dots", ), name="data")
+
+if __name__ == "__main__":
+    ngrid = 200
+    d = np.random.uniform(-10, 10, (ngrid, ))
+    x, y = np.random.uniform(0, 90, (2, ngrid, ))
+    f = BarnesFilter4Scatter(x, y, d)
+    a = f.lowpass()
+    import matplotlib.pyplot as plt
+    plt.figure(1, (14, 4.8))
+    plt.subplot(131)
+    plt.colorbar(plt.tricontourf(x, y, d, cmap=plt.cm.RdYlBu_r))
+    plt.subplot(132)
+    plt.colorbar(plt.tricontourf(x, y, a.data, cmap=plt.cm.RdYlBu_r))
+    plt.subplot(133)
+    plt.colorbar(plt.tricontourf(x, y, d - a.data, cmap=plt.cm.RdYlBu_r))
+    plt.show()
+
```

