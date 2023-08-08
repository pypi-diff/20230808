# Comparing `tmp/kctools-0.23.8.tar.gz` & `tmp/kctools-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kctools-0.23.8.tar", last modified: Mon Aug  7 20:13:14 2023, max compression
+gzip compressed data, was "kctools-23.8.0.tar", last modified: Tue Aug  8 14:25:29 2023, max compression
```

## Comparing `kctools-0.23.8.tar` & `kctools-23.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1061 2022-01-22 01:49:58.000000 kctools-0.23.8/LICENSE
--rw-rw-r--   0 kcs       (1000) kcs       (1000)      514 2023-08-07 20:13:14.312344 kctools-0.23.8/PKG-INFO
--rw-r--r--   0 kcs       (1000) kcs       (1000)       63 2022-01-22 01:52:01.000000 kctools-0.23.8/README.md
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools/
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1416 2023-08-04 18:10:16.000000 kctools-0.23.8/kctools/__init__.py
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools/classes/
--rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-0.23.8/kctools/classes/__init__.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1027 2022-12-17 18:05:40.000000 kctools-0.23.8/kctools/classes/cuke.py
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools/classes/data/
--rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-0.23.8/kctools/classes/data/__init__.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     3033 2023-03-04 23:53:30.000000 kctools-0.23.8/kctools/classes/data/config.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1537 2022-12-17 18:07:26.000000 kctools-0.23.8/kctools/classes/dicts.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     1334 2022-09-30 00:15:37.000000 kctools-0.23.8/kctools/classes/lock.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     3936 2022-01-29 17:28:35.000000 kctools-0.23.8/kctools/classes/map.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     2897 2023-08-04 21:28:02.000000 kctools-0.23.8/kctools/classes/reg.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)    15102 2023-08-04 18:45:06.000000 kctools-0.23.8/kctools/classes/sub.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)     3992 2023-08-05 19:32:57.000000 kctools-0.23.8/kctools/classes/vec.py
--rw-r--r--   0 kcs       (1000) kcs       (1000)    12361 2023-08-06 14:56:18.000000 kctools-0.23.8/kctools/kctools.py
-drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-07 20:13:14.312344 kctools-0.23.8/kctools.egg-info/
--rw-r--r--   0 kcs       (1000) kcs       (1000)      514 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/PKG-INFO
--rw-r--r--   0 kcs       (1000) kcs       (1000)      446 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/SOURCES.txt
--rw-r--r--   0 kcs       (1000) kcs       (1000)        1 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/dependency_links.txt
--rw-r--r--   0 kcs       (1000) kcs       (1000)        8 2023-08-07 20:13:14.000000 kctools-0.23.8/kctools.egg-info/top_level.txt
--rw-rw-r--   0 kcs       (1000) kcs       (1000)       38 2023-08-07 20:13:14.312344 kctools-0.23.8/setup.cfg
--rw-r--r--   0 kcs       (1000) kcs       (1000)      797 2023-08-04 19:12:30.000000 kctools-0.23.8/setup.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-08 14:25:29.251766 kctools-23.8.0/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1061 2022-01-22 01:49:58.000000 kctools-23.8.0/LICENSE
+-rw-rw-r--   0 kcs       (1000) kcs       (1000)      514 2023-08-08 14:25:29.251766 kctools-23.8.0/PKG-INFO
+-rw-r--r--   0 kcs       (1000) kcs       (1000)       63 2022-01-22 01:52:01.000000 kctools-23.8.0/README.md
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-08 14:25:29.251766 kctools-23.8.0/kctools/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1416 2023-08-04 18:10:16.000000 kctools-23.8.0/kctools/__init__.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-08 14:25:29.251766 kctools-23.8.0/kctools/classes/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-23.8.0/kctools/classes/__init__.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1027 2022-12-17 18:05:40.000000 kctools-23.8.0/kctools/classes/cuke.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-08 14:25:29.251766 kctools-23.8.0/kctools/classes/data/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        0 2022-02-22 14:00:15.000000 kctools-23.8.0/kctools/classes/data/__init__.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     3033 2023-03-04 23:53:30.000000 kctools-23.8.0/kctools/classes/data/config.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1537 2022-12-17 18:07:26.000000 kctools-23.8.0/kctools/classes/dicts.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     1334 2022-09-30 00:15:37.000000 kctools-23.8.0/kctools/classes/lock.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     3936 2022-01-29 17:28:35.000000 kctools-23.8.0/kctools/classes/map.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     2897 2023-08-04 21:28:02.000000 kctools-23.8.0/kctools/classes/reg.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)    15086 2023-08-08 10:47:58.000000 kctools-23.8.0/kctools/classes/sub.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)     3992 2023-08-05 19:32:57.000000 kctools-23.8.0/kctools/classes/vec.py
+-rw-r--r--   0 kcs       (1000) kcs       (1000)    12361 2023-08-06 14:56:18.000000 kctools-23.8.0/kctools/kctools.py
+drwxrwxr-x   0 kcs       (1000) kcs       (1000)        0 2023-08-08 14:25:29.251766 kctools-23.8.0/kctools.egg-info/
+-rw-r--r--   0 kcs       (1000) kcs       (1000)      514 2023-08-08 14:25:29.000000 kctools-23.8.0/kctools.egg-info/PKG-INFO
+-rw-r--r--   0 kcs       (1000) kcs       (1000)      446 2023-08-08 14:25:29.000000 kctools-23.8.0/kctools.egg-info/SOURCES.txt
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        1 2023-08-08 14:25:29.000000 kctools-23.8.0/kctools.egg-info/dependency_links.txt
+-rw-r--r--   0 kcs       (1000) kcs       (1000)        8 2023-08-08 14:25:29.000000 kctools-23.8.0/kctools.egg-info/top_level.txt
+-rw-rw-r--   0 kcs       (1000) kcs       (1000)       38 2023-08-08 14:25:29.255766 kctools-23.8.0/setup.cfg
+-rw-r--r--   0 kcs       (1000) kcs       (1000)      797 2023-08-08 12:43:24.000000 kctools-23.8.0/setup.py
```

### Comparing `kctools-0.23.8/LICENSE` & `kctools-23.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/PKG-INFO` & `kctools-23.8.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kctools
-Version: 0.23.8
+Version: 23.8.0
 Summary: miscellaneous elves
 Home-page: https://github.com/kcstokely/kctools
 Author: kevin c. stokely
 Author-email: kcstokely@gmail.com
 License: MIT
 Description: # kctools
```

### Comparing `kctools-0.23.8/kctools/__init__.py` & `kctools-23.8.0/kctools/__init__.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/cuke.py` & `kctools-23.8.0/kctools/classes/cuke.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/data/config.py` & `kctools-23.8.0/kctools/classes/data/config.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/dicts.py` & `kctools-23.8.0/kctools/classes/dicts.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/lock.py` & `kctools-23.8.0/kctools/classes/lock.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/map.py` & `kctools-23.8.0/kctools/classes/map.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/reg.py` & `kctools-23.8.0/kctools/classes/reg.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/classes/sub.py` & `kctools-23.8.0/kctools/classes/sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ################################################
 
+from functools import wraps
 from collections import Counter
 
 from ..kctools import endify as _e
 from ..kctools import is_np, is_pd
-from ..kctools import np_check, pd_check
+from ..kctools import pd_check
+
+from .data.config import conf as cf
 
 if is_np:
     import numpy as np
     
 if is_np and is_pd:
     import pandas as pd
 
-from .data.config import conf as cf
-
 ################################################
 
-@np_check
 class N():
     
     '''
         This class represents one or more
           objects in the power-set 2**L.
 
         It has methods that are useful
@@ -40,26 +40,29 @@
 
         All methods:
           - rely only on self._hot
           - written to act on 1-D array
           - wrappers extend to act on 2-D
     '''
 
-    ############ CONFIG   
+    ### CONFIG   
     
     _L = 12 # overwrite to warp spacetime
     _conf = cf # overwrite to name things
     _cmap = {v: k for k, v in cf.items()}
     
     ############ BIRTH
     
     def __init__(self, inp = []):
 
+        if not is_np:
+            raise Exception('Please install numpy, and maybe pandas.')
+        
         if isinstance(inp, N):
-            self._hot = N._hot
+            self._hot = inp._hot
         else:
             
             if isinstance(inp, str):
                 ndxs = N._conf[inp]
             elif isinstance(inp, int):
                 ndxs = np.where([ int(x) for x in list(f'{int(bin(inp)[2:]):0{N._L}d}') ])[0]
             elif len(inp) == N._L:
@@ -72,15 +75,15 @@
     
     ############ WHAT
     
     def __len__(self):
         return self._hot.shape[0] if self._hot.ndim > 1 else 1
 
     def __iter__(self):
-        return (x for x in self._hot) if self._hot.ndim > 1 else self._hot
+        return (N(x) for x in self._hot) if self._hot.ndim > 1 else (N(x) for x in [self._hot])
     
     def __repr__(self):
         return str(N(self)._hot.astype(int))
 
     ############ ORGANIZE
     
     def crush(self):
@@ -151,15 +154,15 @@
         return tuple(np.diff(list(self.notes())+[N._L+self.notes()[0]])) if self.notes() else ()
     
     @tuple_mapper
     def lookup(self):
         name = N._cmap.get(self.notes(), '')
         if not name:
             modes = N(self).modes()
-            for mode in modes._hot:
+            for mode in modes:
                 mode = N(mode)
                 name = N._cmap.get(mode.notes())
                 if name:
                     if not self._hot[0]:
                         name = f'disp. mode of {name}'
                     else:
                         for mdx in range(self.num()):
@@ -424,27 +427,25 @@
         '''
             Creates a panda of all 2**L sequences, or
               optionally filtered down to a musically
               relevant subset.
         '''
         
         if isinstance(filt, str):
-            assert filt in ['hot', 'canon', 'ext_canon']
-
-        hots  = self._hot if self._hot.ndim > 1 else [self._hot]    
+            assert filt in ['hot', 'canon', 'ext_canon']   
             
         cols  = ['hot', 'num', 'energy', 'symmetry']
         cols += ['ext_canonical', 'runs', 'gaps']
         cols += ['canonical', 'handedness', 'string', 'lookup']
 
         rows = []
-        for hot in hots:
+        for hot in self:
             row = []
             for col in cols:
-                value = getattr(N(hot), col)()
+                value = getattr(hot, col)()
                 value = value.hot() if isinstance(value, N) else value
                 row.append(value)
             rows.append(row)
         df = pd.DataFrame(rows, columns=cols)
 
         if filt:
 
@@ -486,10 +487,8 @@
                 ascending = [True, True, False, False, False, False]
             )
 
         return df
 
 ################################################
 
-if __name__ == '__main__':    
-    n  = N()
-    df = n.uv().df()
+
```

### Comparing `kctools-0.23.8/kctools/classes/vec.py` & `kctools-23.8.0/kctools/classes/vec.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools/kctools.py` & `kctools-23.8.0/kctools/kctools.py`

 * *Files identical despite different names*

### Comparing `kctools-0.23.8/kctools.egg-info/PKG-INFO` & `kctools-23.8.0/kctools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kctools
-Version: 0.23.8
+Version: 23.8.0
 Summary: miscellaneous elves
 Home-page: https://github.com/kcstokely/kctools
 Author: kevin c. stokely
 Author-email: kcstokely@gmail.com
 License: MIT
 Description: # kctools
```

### Comparing `kctools-0.23.8/setup.py` & `kctools-23.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as fp:
     long_description = fp.read()
     long_description_content_type = 'text/markdown'
 
 setuptools.setup(
     name             = 'kctools',
-    version          = '0.23.8',
+    version          = '23.8.0',
     author           = 'kevin c. stokely',
     author_email     = 'kcstokely@gmail.com',
     description      = 'miscellaneous elves',
     url              = 'https://github.com/kcstokely/kctools',
     packages         = setuptools.find_packages(),
     license          = 'MIT',
     classifiers = [
```

