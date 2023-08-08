# Comparing `tmp/accphys-0.1.0.tar.gz` & `tmp/accphys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accphys-0.1.0.tar", max compression
+gzip compressed data, was "accphys-0.1.1.tar", max compression
```

## Comparing `accphys-0.1.0.tar` & `accphys-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,51 @@
--rwxr-xr-x   0        0        0    35149 2022-05-22 16:34:10.594835 accphys-0.1.0/LICENSE
--rwxr-xr-x   0        0        0      180 2022-05-13 18:15:11.050000 accphys-0.1.0/accphys/.ipynb_checkpoints/__init__-checkpoint.py
--rwxr-xr-x   0        0        0     5737 2022-05-28 09:13:01.000000 accphys-0.1.0/accphys/.ipynb_checkpoints/beamline-checkpoint.py
--rwxr-xr-x   0        0        0     8100 2022-05-03 14:53:51.600000 accphys-0.1.0/accphys/.ipynb_checkpoints/convert-checkpoint.py
--rwxr-xr-x   0        0        0    15159 2022-05-13 16:46:08.830000 accphys-0.1.0/accphys/.ipynb_checkpoints/elements-checkpoint.py
--rwxr-xr-x   0        0        0     7084 2022-05-28 09:05:37.000000 accphys-0.1.0/accphys/.ipynb_checkpoints/nf-checkpoint.py
--rwxr-xr-x   0        0        0      936 2022-05-15 17:47:06.930000 accphys-0.1.0/accphys/.ipynb_checkpoints/plotting-checkpoint.py
--rwxr-xr-x   0        0        0     5118 2022-05-28 08:57:14.000000 accphys-0.1.0/accphys/.ipynb_checkpoints/tools-checkpoint.py
--rwxr-xr-x   0        0        0      180 2022-05-22 16:34:10.596788 accphys-0.1.0/accphys/__init__.py
--rwxr-xr-x   0        0        0     5737 2022-05-28 09:13:01.746454 accphys-0.1.0/accphys/beamline.py
--rwxr-xr-x   0        0        0     8100 2022-05-22 16:34:10.600694 accphys-0.1.0/accphys/convert.py
--rwxr-xr-x   0        0        0    15159 2022-05-22 16:34:10.602645 accphys-0.1.0/accphys/elements.py
--rwxr-xr-x   0        0        0     7084 2022-05-28 09:05:37.870638 accphys-0.1.0/accphys/nf.py
--rwxr-xr-x   0        0        0      936 2022-05-22 16:34:10.604600 accphys-0.1.0/accphys/plotting.py
--rwxr-xr-x   0        0        0        0 2022-05-13 15:23:33.360000 accphys-0.1.0/accphys/solver/.ipynb_checkpoints/__init__-checkpoint.py
--rwxr-xr-x   0        0        0      717 2022-05-11 19:16:45.450000 accphys-0.1.0/accphys/solver/.ipynb_checkpoints/heyoka-checkpoint.py
--rwxr-xr-x   0        0        0        0 2022-05-13 15:23:33.360000 accphys-0.1.0/accphys/solver/__init__.py
--rwxr-xr-x   0        0        0      184 2022-05-13 15:21:34.750000 accphys-0.1.0/accphys/solver/__pycache__/__init__.cpython-39.pyc
--rwxr-xr-x   0        0        0     3359 2022-05-13 15:21:34.750000 accphys-0.1.0/accphys/solver/__pycache__/nf.cpython-39.pyc
--rwxr-xr-x   0        0        0      717 2022-05-11 19:16:45.450000 accphys-0.1.0/accphys/solver/heyoka.py
--rwxr-xr-x   0        0        0     3923 2022-05-28 09:01:14.460707 accphys-0.1.0/accphys/tools.py
--rwxr-xr-x   0        0        0      697 2022-05-31 08:40:29.402819 accphys-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      895 2022-05-31 08:40:41.179598 accphys-0.1.0/setup.py
--rw-r--r--   0        0        0      704 2022-05-31 08:40:41.179978 accphys-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-09 20:47:35.018420 accphys-0.1.1/LICENSE
+-rw-r--r--   0        0        0      265 2023-02-22 19:45:31.920833 accphys-0.1.1/accphys/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     7665 2023-03-27 15:32:38.526440 accphys-0.1.1/accphys/.ipynb_checkpoints/adbooster-checkpoint.py
+-rw-r--r--   0        0        0    29670 2023-08-08 10:18:39.946506 accphys-0.1.1/accphys/.ipynb_checkpoints/beamline-checkpoint.py
+-rw-r--r--   0        0        0    10063 2023-02-01 14:51:22.403235 accphys-0.1.1/accphys/.ipynb_checkpoints/convert-checkpoint.py
+-rw-r--r--   0        0        0    30433 2023-02-22 15:48:37.142988 accphys-0.1.1/accphys/.ipynb_checkpoints/elements-checkpoint.py
+-rw-r--r--   0        0        0     4294 2023-02-22 19:54:54.025073 accphys-0.1.1/accphys/.ipynb_checkpoints/knob-checkpoint.py
+-rw-r--r--   0        0        0     7108 2022-11-09 20:47:35.018420 accphys-0.1.1/accphys/.ipynb_checkpoints/nf-checkpoint.py
+-rw-r--r--   0        0        0     4822 2023-02-22 16:01:20.968891 accphys-0.1.1/accphys/.ipynb_checkpoints/tools-checkpoint.py
+-rw-r--r--   0        0        0      201 2023-07-26 08:41:27.223060 accphys-0.1.1/accphys/__init__.py
+-rw-r--r--   0        0        0     7665 2023-03-27 15:32:38.526440 accphys-0.1.1/accphys/adbooster.py
+-rw-r--r--   0        0        0    29670 2023-08-08 10:18:39.946506 accphys-0.1.1/accphys/beamline.py
+-rw-r--r--   0        0        0     4002 2023-02-27 12:38:49.226194 accphys-0.1.1/accphys/da-Copy1.py
+-rw-r--r--   0        0        0      212 2023-07-26 08:44:30.488219 accphys-0.1.1/accphys/elements/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0    13293 2023-07-31 15:24:26.142700 accphys-0.1.1/accphys/elements/.ipynb_checkpoints/cfm-checkpoint.py
+-rw-r--r--   0        0        0    14588 2023-08-02 18:09:50.781344 accphys-0.1.1/accphys/elements/.ipynb_checkpoints/common-checkpoint.py
+-rw-r--r--   0        0        0     2964 2023-08-08 10:31:07.828312 accphys-0.1.1/accphys/elements/.ipynb_checkpoints/poleface-checkpoint.py
+-rw-r--r--   0        0        0      212 2023-07-26 08:44:30.488219 accphys-0.1.1/accphys/elements/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-26 08:44:41.668474 accphys-0.1.1/accphys/elements/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12868 2023-08-08 09:40:09.631682 accphys-0.1.1/accphys/elements/__pycache__/cfm.cpython-310.pyc
+-rw-r--r--   0        0        0    11677 2023-08-08 09:40:09.627684 accphys-0.1.1/accphys/elements/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0        0        0     2086 2023-07-26 08:41:53.399938 accphys-0.1.1/accphys/elements/__pycache__/drift.cpython-310.pyc
+-rw-r--r--   0        0        0     1213 2023-07-26 08:41:53.403938 accphys-0.1.1/accphys/elements/__pycache__/phaserot.cpython-310.pyc
+-rw-r--r--   0        0        0     2281 2023-08-08 10:31:13.896313 accphys-0.1.1/accphys/elements/__pycache__/poleface.cpython-310.pyc
+-rw-r--r--   0        0        0     1851 2023-07-26 08:41:53.403938 accphys-0.1.1/accphys/elements/__pycache__/rfcavity.cpython-310.pyc
+-rw-r--r--   0        0        0    14573 2023-08-08 09:39:49.445309 accphys-0.1.1/accphys/elements/cfm.py
+-rw-r--r--   0        0        0    14975 2023-08-08 09:39:49.445309 accphys-0.1.1/accphys/elements/common.py
+-rw-r--r--   0        0        0     2208 2023-07-26 08:41:27.223060 accphys-0.1.1/accphys/elements/drift.py
+-rw-r--r--   0        0        0      681 2023-07-26 08:41:27.223060 accphys-0.1.1/accphys/elements/phaserot.py
+-rw-r--r--   0        0        0     2964 2023-08-08 10:31:07.828312 accphys-0.1.1/accphys/elements/poleface.py
+-rw-r--r--   0        0        0     1825 2023-07-26 08:41:27.223060 accphys-0.1.1/accphys/elements/rfcavity.py
+-rw-r--r--   0        0        0       88 2023-08-01 10:47:01.992962 accphys-0.1.1/accphys/io/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     5010 2023-08-01 15:48:19.386728 accphys-0.1.1/accphys/io/.ipynb_checkpoints/convert-checkpoint.py
+-rw-r--r--   0        0        0     6203 2023-08-08 14:32:58.965069 accphys-0.1.1/accphys/io/.ipynb_checkpoints/from_madx-checkpoint.py
+-rw-r--r--   0        0        0     3091 2023-07-31 11:04:31.137977 accphys-0.1.1/accphys/io/.ipynb_checkpoints/from_madx_old-checkpoint.py
+-rw-r--r--   0        0        0     6539 2023-08-01 10:43:17.318316 accphys-0.1.1/accphys/io/.ipynb_checkpoints/from_pandas-checkpoint.py
+-rw-r--r--   0        0        0       88 2023-08-08 09:39:49.449307 accphys-0.1.1/accphys/io/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-08 09:40:10.311358 accphys-0.1.1/accphys/io/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5657 2023-08-08 09:40:10.315356 accphys-0.1.1/accphys/io/__pycache__/convert.cpython-310.pyc
+-rw-r--r--   0        0        0     4309 2023-08-08 14:22:05.132944 accphys-0.1.1/accphys/io/__pycache__/from_madx.cpython-310.pyc
+-rw-r--r--   0        0        0     2235 2023-07-31 12:16:18.434342 accphys-0.1.1/accphys/io/__pycache__/from_madx_old.cpython-310.pyc
+-rw-r--r--   0        0        0     4625 2023-08-01 10:43:25.050291 accphys-0.1.1/accphys/io/__pycache__/from_pandas.cpython-310.pyc
+-rw-r--r--   0        0        0     5450 2023-08-08 09:39:49.449307 accphys-0.1.1/accphys/io/convert.py
+-rw-r--r--   0        0        0     6203 2023-08-08 14:32:58.965069 accphys-0.1.1/accphys/io/from_madx.py
+-rw-r--r--   0        0        0     4294 2023-02-22 19:54:54.025073 accphys-0.1.1/accphys/knob.py
+-rw-r--r--   0        0        0     7108 2022-11-09 20:47:35.018420 accphys-0.1.1/accphys/nf.py
+-rw-r--r--   0        0        0      943 2023-07-26 08:41:27.223060 accphys-0.1.1/accphys/plotting.py
+-rw-r--r--   0        0        0     5028 2023-07-26 08:41:27.223060 accphys-0.1.1/accphys/tools.py
+-rw-r--r--   0        0        0      535 2023-08-08 09:39:49.453305 accphys-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      887 2023-08-08 14:33:14.584479 accphys-0.1.1/setup.py
+-rw-r--r--   0        0        0      666 2023-08-08 14:33:14.584674 accphys-0.1.1/PKG-INFO
```

### Comparing `accphys-0.1.0/LICENSE` & `accphys-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `accphys-0.1.0/accphys/.ipynb_checkpoints/convert-checkpoint.py` & `accphys-0.1.1/accphys/.ipynb_checkpoints/convert-checkpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .beamline import beamline
 from .elements import cfm
-from tqdm.auto import tqdm
+
+from tqdm import tqdm
 
 from latticeadaptor.core import LatticeAdaptor
 import numpy as np
 from njet.jet import factorials
 
 def prepare_df(hdf, position_label='s', length_label='L', position=0, tol=1e-6, **kwargs):
     '''
@@ -73,23 +74,29 @@
             new_row[position_label_index] = pos + length
             new_row[length_label_index] = empty_space
             hdf.loc[k + 0.5] = new_row # insert a new row in between k and k + 1
             
     return hdf.sort_index().reset_index(drop=True)
 
 
-def to_beamline(hdf, beta0, component_labels, position_label='s', length_label='L', **kwargs):
+def to_beamline(hdf, component_labels, component_indices, position_label='s', length_label='L', **kwargs):
     '''
     Construct a beamline from a given lattice.
     
     Parameters
     ----------
     hdf: Pandas dataframe
         A Pandas dataframe object containing the position, lengths and field strengths of the individual
         elements in the beamline.
+                
+    component_labels
+        A list of floats, declaring the names of the columns in which to find the combined-function components.
+        
+    component_indices
+        A list of integers, where the k-th entry denotes the index of the respective component.
         
     position_label: str, optional
         Label denoting the position of the individual elements within the dataframe.
         
     length_label: str, optional
         Label denoting the lengths of the individual elements within the dataframe.
         
@@ -97,102 +104,141 @@
         Keyworded arguments passed to the cfm element.
         
     Returns
     -------
     beamline
         A beamline object representing the sequence of elements.
     '''
-    # Preparation; ensure that no empty space exists between elements (they will be filled with drifts if necesary):
+    assert len(component_labels) > 0
+    assert len(component_labels) == len(component_indices)
+    # Preparation; ensure that no empty space exists between elements (they will be filled with drifts if necessary):
     hdf = prepare_df(hdf, position_label=position_label, length_label=length_label, **kwargs)
             
     # group the given elements with respect to the remaining labels & find the uniques among them
     group_labels = [c for c in hdf.columns if c != position_label] # labels by which we distinguish different elements; custom columns may be added to artifically distinguish different element groups
     group_index_label = 'group_index'
     grp = hdf.groupby(group_labels, sort=False)
     hdf[group_index_label] = grp.ngroup()
     unique_elements = hdf.drop_duplicates(group_index_label)
     
     # build the elements:
     elements = []
     group_index = 0
-    for n in tqdm(range(len(unique_elements))):
+    n_components = max(component_indices) + 1 # + 1 because of the 0th-component
+    for n in tqdm(range(len(unique_elements)), disable=kwargs.get('disable_tqdm', False)):
         row = unique_elements.iloc[n]
-        components = [row[c] for c in component_labels]
-        length = row[length_label]
-        assert group_index == row[group_index_label] # verify that the position in the element list corresponds with the group index given by ngroup.
-        elements.append(cfm(beta0=beta0, components=components, length=length, **kwargs))
+        components = [0]*n_components
+        for j in range(len(component_indices)):
+            index = component_indices[j]
+            label = component_labels[j]
+            components[index] = row.get(label, 0)
+        length = row.get(length_label, 0)
+        assert group_index == row[group_index_label] # verify that the position in the element list corresponds to the group index given by ngroup.
+        elements.append(cfm(components=components, length=length, **kwargs))
         group_index += 1
         
     # set the ordering
     ordering = list(hdf[group_index_label])
             
     return beamline(*elements, ordering=ordering)
 
 
-def from_madx(filename, beta0, **kwargs):
+def madx2dataframe(filename, **kwargs):
     '''
     Load MAD-X lattice from file, using LatticeAdaptor module, 
-    and construct a beamline object from the data.
+    and construct a suitable dataframe object. Furthermore, return the
+    required input parameters for to_beamline routine.
     
     Parameters
     ----------
     filename: str
         The name of the MAD-X lattice to be loaded.
         
-    beta0: float
-        The realtivistic beta-factor (related to the energy of the beam). This is required later to
-        build the Hamiltonians.
-        
     **kwargs
         Optional arguments passed to 'to_beamline' routine.
         
     Returns
-    -------
-    beamline
-        A beamline object representing the sequence of elements in the given lattice.
-        
+    -------    
     Pandas dataframe
         A Pandas dataframe object, representing the loaded sequence of the lattice.
+        
+    dict
+        A dictionary containing MAD-X specific input parameters for the general 'to_beamline' routine.
     '''
     la = LatticeAdaptor()
     la.load_from_file(filename, ftype='madx')
     raw_df = la.table
     
     # MAD-X specific labels
     position_label='at'
     length_label='L'
     bend_kx_label = 'K0'
     angle_label = 'ANGLE'
-    component_labels = [bend_kx_label, 'K1', 'K2']
+    max_seek_order = 13 # maximal order of multipoles to be considered
     madx_default_position = 0.5 # MAD-X tends to denote the position of the elements in the center
 
-    if bend_kx_label not in raw_df.columns:
-        # add kx
+    component_indices = [j for j in range(max_seek_order) if f'K{j}' in raw_df.columns]
+    component_labels = [f'K{j}' for j in component_indices]
+    if bend_kx_label not in raw_df.columns and angle_label in raw_df.columns:
+        # add kx (and K0 label) to the dataframe, computed from the bend angles
         angles = raw_df[angle_label].values
         lengths = raw_df[length_label].values 
         valid_indices = np.logical_and((~np.isnan(angles)), lengths > 0)
         kx = np.zeros(len(raw_df))
         kx[valid_indices] = angles[valid_indices]/lengths[valid_indices] # r*phi = L; kx = 1/r
         raw_df[bend_kx_label] = kx
-    
+        component_labels = [bend_kx_label] + component_labels
+        component_indices = [0] + component_indices
+
     # drop elements with zero length and uneccesary columns;
     # N.B. E1 and E2 denote rotation angles of the pole-faces. If they are non-zero,
     # they are usually half the bend angle (in the rectangular case). We will ignore rectangular
     # bends for the time being and use s-bends here.
     columns_oi = [position_label, length_label] + component_labels
     # if they exist, add skew-values to the components; TODO: check & verify this numerically
-    for j in range(1, 3):
-        if f'K{j}S' in raw_df.columns:
-            raw_df[f'K{j}'] = raw_df[f'K{j}'].values + raw_df[f'K{j}S']*1j
+    for cl in component_labels:
+        if cl + 'S' in raw_df.columns:
+            raw_df[cl] = raw_df[cl].values + raw_df[cl + 'S'].values*1j
     raw_df = raw_df.loc[raw_df[length_label] > 0][columns_oi]
     
     # (TO BE CHECKED; TODO)
-    facts = factorials(3)
-    for j in range(1, 3):
-        raw_df[f'K{j}'] = raw_df[f'K{j}'].values/facts[j]
-        
-    # construct the sequence of Lie operators
-    kwargs['position'] = kwargs.get('position', madx_default_position) 
-    seq2 = to_beamline(raw_df, beta0=beta0, 
-                      component_labels=component_labels, position_label=position_label,
-                      length_label=length_label, **kwargs)
-    return seq2, raw_df
+    facts = factorials(len(component_labels))
+    j = 0
+    for cl in component_labels:
+        raw_df[cl] = raw_df[cl].values/facts[j]
+        j += 1
+        
+    if len(component_labels) == 0: # special case: Only pure drifts exist
+        raw_df[bend_kx_label] = [0]*len(raw_df)
+        component_labels = [bend_kx_label]
+        component_indices = [0]
+        
+    to_beamline_inp = {'component_labels': component_labels, 'component_indices': component_indices, 'position_label': position_label,
+                    'length_label': length_label, 'position': kwargs.get('position', madx_default_position)}
+    
+    return raw_df, to_beamline_inp
+
+
+def madx2beamline(filename, beta0, **kwargs):
+    '''
+    Load MAD-X lattice from file and construct a beamline object from the data.
+    
+    Parameters
+    ----------
+    filename: str
+        The name of the MAD-X lattice to be loaded.
+        
+    beta0: float
+        The realtivistic beta-factor (related to the energy of the beam). This is required later to
+        build the Hamiltonians.
+        
+    **kwargs
+        Optional arguments passed to 'load_madx_file' routine.
+        
+    Returns
+    -------
+    beamline
+        A beamline object representing the sequence of elements in the given lattice.
+    '''
+    raw_df, to_beamline_inp = madx2dataframe(filename=filename, **kwargs)
+    to_beamline_inp.update(kwargs)
+    return to_beamline(raw_df, beta0=beta0, **to_beamline_inp)
```

### Comparing `accphys-0.1.0/accphys/.ipynb_checkpoints/elements-checkpoint.py` & `accphys-0.1.1/accphys/elements/.ipynb_checkpoints/cfm-checkpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,219 @@
 import numpy as np
+import warnings
 
-from njet.functions import cos
-from lieops import create_coords, construct
+from .common import hard_edge_element
+from .drift import DriftHamiltonian
 
-# N.B. the length of an element will be used only later, when it comes to calculating the flow.
+def _g(components, tilt=0):
+    '''
+    Compute the g-part of the cfm. Code taken in parts from my MAD-X implementation 
+    (see https://github.com/mtitze/MAD-X/blob/master/src/trrun.f90).
+    '''
+    exp = lambda z: complex(np.exp(z)) # convert numpy.float64 back to float as precaution to prevent unpredictable results if using jets etc.
+
+    # Eq. (2.40) resp. (2.47) in Ref. [2]:
+    # (By + 1j*Bx)_(phi = phi0) = sum_k components[k] r^k,
+    # where phi0 = tilt here.
+
+    # since kx = real(components[0]) and ky = -imag(components[0]), i.e.
+    # components[0] = kx - 1j*ky,
+    # we have:
+    kappa = components[0].conjugate()
+    barkappa = components[0]
+
+    # Now fill up the g_{ij}'s for j = 0, ..., i and i = 0, ..., len(components) - 1.
+    g = {}
+    g[(0, 0)] = 0
+    g[(1, 0)] = -barkappa
+    g[(1, 1)] = -kappa # = g[(1, 0)].conjugate()
+    for k in range(1, len(components) + 1): # k reflects the order up to which we consider the G-function
+        for j in range(k):
+            # Eq. (6), in Ref. [1]
+            g[(k + 1, j + 1)] = ( barkappa*g[(k, j + 1)]*(j + 1)*(j - k + 3/2) + 
+                                 kappa*g[(k, j)]*(k - j)*(1/2 - j) )/(k - j)/(j + 1)
+        # Eq. (8) in Ref. [1]
+        sum0 = 0
+        for j in range(1, k + 1):
+            sum0 = sum0 - (k + 1 - j)*g[(k + 1, j)]*exp(-tilt*2*1j*j)
+
+        g[(k + 1, 0)] = sum0/(k + 1)
+        # Add additional contributions from components, if they exist.
+        if k < len(components) + 1:
+            real = (barkappa*exp(tilt*1j) + kappa*exp(tilt*-1j))/2 # = Re(barkappa*exp(tilt*1j))
+            fk = -2**k*exp(tilt*-1j*k)
+            g[(k + 1, 0)] += fk*real*components[k - 1]/(k + 1)
+            if k < len(components):
+                g[(k + 1, 0)] += fk*components[k]/(k + 1)
+
+        g[(k + 1, k + 1)] = g[(k + 1, 0)].conjugate()
+    return g
+
+def CFMHamiltonian(components, tilt=0, tol_drop=0, **kwargs):
+    '''
+    Compute the Hamiltonian of the cfm (without electric fields).
+    For the underlying coordinate system and further details see Refs. [1, 2] below.
+    In particular, the Hamiltonian is given by Eq. (2.16) in Ref. [2].
+
+    Parameters
+    ----------
+    tol_drop: float, optional
+        Threshold below terms in the Hamiltonian will be dropped.
+    
+    **kwargs
+        Optional keyword arguments passed to 'elements.drift.DriftHamiltonian'.
+
+    Returns
+    -------
+    dict
+        A dictionary having the following keys:
+        
+        kx: float
+            The field strength of the x-component of the dipole.
+            
+        ky: float
+            The field strength of the y-component of the dipole.
+
+        H: poly
+            The Hamiltonian of the cfm up to the requested order.
 
-# Reference(s):
-# [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
-# [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
+        H_drift: poly
+            The drift part of H.
 
-class hard_edge_element:
+        H_field: poly
+            The field part of H.
+            
+        g: dict
+            The g-components in Ref. [1]
+        G: dict
+            The G-components in Ref. [1]
+
+        So that H = H_drift + H_field.
+        
+    References
+    ----------
+    [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
+    [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
+    '''
+    # Compute the Hamiltonian of the drift
+    DH = DriftHamiltonian(tol_drop=tol_drop, **kwargs)
+    x, y, sigma, px, py, psigma = DH['coords']
+    # Compute the CFM vector potential
+    # G = (1 + Kx*x + Ky*y)*A_t near Eq. (2).
+    # Here G := G*e/p0 (The factor e/p0 can be absorbed in the coefficients later; see also the comment on page 4, right column)
+    g = _g(components=components, tilt=tilt)
+    rp = (x + y*1j)/2
+    rm = rp.conjugate()
+    G = sum([rp**(k - j)*rm**j*g[(k, j)] for k, j in g.keys()]) # N.B.: We need to multiply g[(k, j)] from right in case their entries are jetpoly objects etc. They need to be added as the coefficients of the Lie polynomials. 
     
-    def __init__(self, *args, length=1, **kwargs):
-        '''
-        Class to model the Hamiltonian of a 6D hard-edge element.
-        '''
-        self.length = length
-        if 'beta0' in kwargs.keys():
-            self.calcHamiltonian(*args, **kwargs)
-        if hasattr(self, 'full_hamiltonian'):
-            self.setHamiltonian(**kwargs)
+    # Also compute the derivatives of G
+    drp_G = sum([(k - j)*rp**(k - j - 1)*rm**j*g[(k, j)] for k, j in g.keys() if k != j]) # the partial derivative of G with respect to r_+
+    drm_G = sum([j*rp**(k - j)*rm**(j - 1)*g[(k, j)] for k, j in g.keys() if j != 0])
+    dx_G = (drp_G + drm_G)/2
+    dy_G = (-drp_G + drm_G)/2/1j
+    
+    # Assemble output Hamiltonians
+    lamb0 = components[0]
+    kx = (lamb0 + lamb0.conjugate())/2 # lamb0.real; .conjugate() works with floats and other objects better than .real etc.
+    ky = (lamb0.conjugate() - lamb0)/2/1j # -lamb0.imag
+    # N.B.: Hfull = psigma - (1 + kx*x + ky*y)*drift - G
+    drift_s = DH['drift_sqrt'] # the square root expression in the Hamiltonian belonging to the drift
+    H_drift = psigma - drift_s
+    H_field = - drift_s*(x*kx + y*ky) - G
+    H_full = H_drift + H_field
+    
+    # remove any remaining constants; they do not affect the equations of motion. Also drop all terms below the given threshold.
+    H_full = H_full.pop((0, 0, 0, 0, 0, 0), None).above(tol_drop)
+    H_drift = H_drift.pop((0, 0, 0, 0, 0, 0), None).above(tol_drop)
+    H_field = H_field.pop((0, 0, 0, 0, 0, 0), None).above(tol_drop)
+
+    out = DH
+    out['components'] = components
+    out['tilt'] = tilt
+    out['kx'] = kx
+    out['ky'] = ky
+    out['full'] = H_full
+    out['kick'] = H_field
+    out['G'] = G
+    out['drp_G'] = drp_G
+    out['drm_G'] = drm_G
+    out['dx_G'] = dx_G
+    out['dy_G'] = dy_G
+    out['g'] = g
+    out['hamiltonian'] = H_full
+    
+    if kx != 0:
+        out['rhox'] = 1/kx # kx = 1/r
+    else:
+        out['rhox'] = float(np.inf)
+        
+    if ky != 0:
+        out['rhoy'] = 1/ky
+    else:
+        out['rhoy'] = float(np.inf)
+    
+    return out
+    
+def _map(CFMH, x, y, sigma, px, py, psigma, ds):
+    r'''
+    An implementation of map (2.33) in Ref. [2].
+    
+    Parameters
+    ----------
+    CFMH: dict
+        The output of CFMHamiltonian, containing the Hamiltonian of the combined-function-magnet and additional information.
+    
+    ds: float
+        \delta_s according to Eq. (2.33) in Ref. [2].
         
-    def calcHamiltonian(self, beta0, sqrtexp: int=2, **kwargs):
-        '''
-        Compute the Hamiltonian of a drift.
-        For the underlying coordinate system and further details see Refs. [1, 2] below.
-        In particular, the Hamiltonian is given by Eq. (2.16) in Ref. [2].
+    References
+    ----------
+    [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
+    [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
+    '''
+    dx_G_map, dy_G_map = CFMH['dx_G'], CFMH['dy_G']
+    
+    sqrt2 = float(np.sqrt(2))
+    xi1 = (x + px*1j)/sqrt2
+    xi2 = (y + py*1j)/sqrt2
+    xi3 = (sigma + psigma*1j)/sqrt2
+    eta1 = (x - px*1j)/sqrt2
+    eta2 = (y - py*1j)/sqrt2
+    eta3 = (sigma - psigma*1j)/sqrt2
+    
+    dx_G = dx_G_map(xi1, xi2, xi3, eta1, eta2, eta3)
+    dy_G = dy_G_map(xi1, xi2, xi3, eta1, eta2, eta3)
+    
+    ux = px + dx_G*ds
+    uy = py + dy_G*ds
+    
+    # Preparation steps
+    beta0 = CFMH['beta0']
+    dE_E = psigma*beta0**2 # = eta in Ref. [2].
+    one_hateta2 = ((1 + dE_E)**2 - 1 + beta0**2)/beta0**2 # (1 + \hat \eta)**2; Eq. (2.17) in Ref. [2].
+    kx, ky = CFMH['kx'], CFMH['ky']
+    denominator = 1 + (kx**2 + ky**2)*ds**2
+    XI = (ux*kx + uy*ky)/denominator*2*ds
+    ZETA = (ux**2 + uy**2 - one_hateta2)/denominator
+    h = -XI/2 + np.sqrt(XI**2/4 - ZETA)
+    curv = 1 + kx*x + ky*y
+    
+    # Map (2.33) in Ref. [2]:
+    xf = x + ds*curv*(ux/h + ds*kx)
+    yf = y + ds*curv*(uy/h + ds*ky)
+    sigmaf = sigma + ds - ds*curv*(1 + dE_E)/h
+    pxf = ux + ds*kx*h
+    pyf = uy + ds*ky*h
+    psigmaf = psigma
+    
+    return xf, yf, sigmaf, pxf, pyf, psigmaf
+
 
-        Parameters
-        ----------
-        sqrtexp or power: int, optional
-            Power up to which the square root of the drift should be expanded. 
-        '''
-        assert 0 < beta0 and beta0 < 1
-        kwargs['power'] = kwargs.get('power', sqrtexp)
-        # Compute the CFM drift part
-        x, y, sigma, px, py, psigma = create_coords(3, real=True, **kwargs)
-        one_hateta2 = lambda ps: ((1 + ps*beta0**2)**2 - 1 + beta0**2)/beta0**2 # Eqs. (15c) and (17) in Ref. [1]
-        sqrt = lambda p1, p2, ps: (one_hateta2(ps) - p1**2 - p2**2)**(1/2)
-        drift_s = construct(sqrt, px, py, psigma, **kwargs) # expand sqrt around [px, py, psigma] = [0, 0, 0] up to power
-        hamiltonian = psigma - drift_s
-        hamiltonian.pop((0, 0, 0, 0, 0, 0), None)
-        self.full_hamiltonian = hamiltonian
-        self._prop = {}
-        self._prop['beta0'] = beta0
-        self._prop['sqrtexp'] = sqrtexp
-        self._prop['drift'] = hamiltonian
-        self._prop['drift_sqrt'] = drift_s
-        self._prop['full'] = hamiltonian
-        self._prop['coords'] = x, y, sigma, px, py, psigma
-        
-    def setHamiltonian(self, *projection, **kwargs):
-        '''
-        Set Hamiltonian by dropping components associated with terms not in given list.
-        
-        self.hamiltonian will be updated.
-        
-        !! Attention !!
-        After this operation it may become necessary to re-caclulate flows and the one-turn map again.
-        
-        Parameters
-        ----------
-        projection: int
-            The indices of the coordinates of interest. Must reach from 0 to self.full_hamiltonian.dim.
-            If there are no arguments given, then the default Hamiltonian will be restored.
-        '''
-        # consistency checks
-        new_dim = len(projection)
-        ham = self.full_hamiltonian
-        if new_dim == 0: # default: 6D Hamiltonian
-            projection = range(ham.dim)
-            new_dim = ham.dim
-        assert new_dim <= ham.dim and max(projection) < ham.dim, 'Number of spatial dimensions too large.'
-        projection = list(projection) + [p + ham.dim for p in projection] # the eta-components duplicate the indices.
-        complement = [k for k in range(2*ham.dim) if not k in projection]
-        new_values = {}
-        for k, v in ham.items():
-            if any([k[p] != 0 for p in complement]): # only keep those coefficients which do not couple to other directions
-                continue
-            new_values[tuple([k[p] for p in projection])] = v
-        self.hamiltonian = ham.__class__(values=new_values, dim=new_dim, max_power=ham.max_power)
-        
-    def copy(self):
-        result = self.__class__(length=self.length)
-        # copy all the fields
-        for field, value in self.__dict__.items():
-            setattr(result, field, value)
-        return result
-        
-class phaserot(hard_edge_element):
-    def __init__(self, *tunes, length=1, **kwargs):
-        '''
-        A generic uncoupled phase (space) rotation.
-        
-        Parameters
-        ----------
-        tunes: float or array_like
-            Tune(s) defining the phase rotation.
-        '''
-        self.tunes = tunes
-        self.length = length
-        if len(tunes) > 0:
-            self.calcHamiltonian(*tunes, **kwargs)
-        if hasattr(self, 'full_hamiltonian'):
-            self.setHamiltonian(**kwargs)
-        
-    def calcHamiltonian(self, *tunes, **kwargs):
-        dim = len(tunes)
-        xieta = create_coords(dim=dim)
-        self.full_hamiltonian = sum([-tunes[k]*xieta[k]*xieta[k + dim] for k in range(dim)])
-        
-        
 class cfm(hard_edge_element):
-    def __init__(self, components=[0], tilt=0, *args, **kwargs):
+    def __init__(self, components=[0], tilt=0, warn=True, **kwargs):
         '''
         Class to model a combined-function-magnetc (cfm).
 
         Parameters
         ----------
         beta0: float
             Relativistic beta = v/c of the reference trajectory.
@@ -125,233 +222,118 @@
             A list of complex entries, denoting the components of the cfm field.
             The components are hereby given with respect to a transversal axis, tilted against the Serre-Frenet
             coordinate system by an angle of choice (see tilt parameter below and Eq. (2.40) in Ref. [2]).
 
             If K_x = 0 this transverse axis smears out a cone. The ideal trajectory is hereby given by a horizontal
             cut of the cone with a plane.
             
-            Note that additional zeros in the list will cause the routine to compute more orders of the CFM.
+            Attention:
+            1) 
+            Additional zeros in the list will cause the routine to compute more orders of the CFM.
+            This becomes important if the cfm contains a non-zero dipole component and some other multipole components.
             
+            2)
+            In the case of a single entry in the cfm components, an additional zero will be added internally so that
+            the resulting object describes a physical dipole. The reason is that (internally) the order of the G-function
+            in Ref. [2] has to be at least 2 or higher (see the topmost Eq. on p.53 in Ref. [2]). To suppress this behaviour,
+            the switch _addzero can be set to False.
+                        
         tilt: float, optional
             The tilt between the dipole component and the higher-order magnet components of the cfm.
             
-        **kwargs
-            Optional arguments passed to self.calcHamiltonian and self.setHamiltonian.
+        References
+        ----------
+        [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
+        [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
         '''
+        assert len(components) > 0
         self.components = components
         self.tilt = tilt
-        hard_edge_element.__init__(self, *args, **kwargs)
-        
-    def setHamiltonian(self, *args, **kwargs):
+        hard_edge_element.__init__(self, warn=False, **kwargs)
+
+        # also compute the overal bend angles, if a length has been provided:
+        if hasattr(self, 'length'):
+            self.phix = self.length*self.kx # r*phi = L; kx = 1/r
+            self.phiy = self.length*self.ky
+        else:
+            if warn:
+                warnings.warn('Length of dipole not specified. Bend angle can not be determined.')
+
+
+    def setStyle(self, *args, **kwargs):
         '''
-        Set self.hamiltonian to requested dimension.
-        
         Parameters
         ----------
         style: str, optional
-            Name of the key in self._prop denoting the Hamiltonian to be used.
+            Name of the field in 'self', denoting the Hamiltonian to be used.
             Supported options are:
             'full': use the full Hamiltonian (default)
             'kick': Only use the Hamiltonian containing field-components (see Eq. (2.36) in Ref. [2])
             'drift': Only the drift part of the Hamiltonian is used, i.e. all fields switched off.
         '''
         supported_styles = ['full', 'kick', 'drift']
         if not hasattr(self, '_style') or 'style' in kwargs.keys():
             self._style = kwargs.get('style', 'full')
         if not self._style in supported_styles:
             raise RuntimeError(f"Style '{self._style}' not recognized. Supported styles:\n{supported_styles}")
-        self.full_hamiltonian = self._prop[self._style]
-        hard_edge_element.setHamiltonian(self, *args, **kwargs)
-    
-    def _g(self):
-        '''
-        Compute the g-part of the cfm. Code taken in parts from my MAD-X implementation 
-        (see https://github.com/mtitze/MAD-X/blob/master/src/trrun.f90).
-        '''
-        exp = lambda z: complex(np.exp(z)) # convert numpy.float64 back to float as precaution to prevent unpredictable results if using jets etc.
-
-        # Eq. (2.40) resp. (2.47) in Ref. [2]:
-        # (By + 1j*Bx)_(phi = phi0) = sum_k components[k] r^k,
-        # where phi0 = tilt here.
-
-        # since kx = real(components[0]) and ky = -imag(components[0]), i.e.
-        # components[0] = kx - 1j*ky,
-        # we have:
-        kappa = self.components[0].conjugate()
-        barkappa = self.components[0]
-
-        nord = len(self.components) - 1
-        # Now fill up the g_{ij}'s for j = 0, ..., i and i = 0, ..., nord + 1.
-        g = {}
-        g[(0, 0)] = 0
-        g[(1, 0)] = -barkappa
-        g[(1, 1)] = -kappa # = g[(1, 0)].conjugate()
-        for k in range(1, nord + 1):
-            for j in range(k):
-                # Eq. (6), in Ref. [1]
-                g[(k + 1, j + 1)] = ( barkappa*g[(k, j + 1)]*(j + 1)*(j - k + 3/2) + 
-                                     kappa*g[(k, j)]*(k - j)*(1/2 - j) )/(k - j)/(j + 1)
-            # Eq. (8) in Ref. [1]
-            sum0 = 0
-            for j in range(1, k + 1):
-                sum0 = sum0 - (k + 1 - j)*g[(k + 1, j)]*exp(-self.tilt*2*1j*j)
-            g[(k + 1, 0)] = ( sum0 - 2**k*exp(-self.tilt*1j*k)*( self.components[k] 
-                            + 1/2*(barkappa*exp(self.tilt*1j) + kappa*exp(self.tilt*-1j))*self.components[k - 1] ) )/(k + 1)
-            g[(k + 1, k + 1)] = g[(k + 1, 0)].conjugate()
-        return g
+        self.hamiltonian = getattr(self, self._style)
 
     def calcHamiltonian(self, **kwargs):
         '''
-        Compute the Hamiltonian of the cfm (without electric fields).
-        For the underlying coordinate system and further details see Refs. [1, 2] below.
-        In particular, the Hamiltonian is given by Eq. (2.16) in Ref. [2].
-
-        Parameters
-        ----------
-        **kwargs
-            Optional keyword arguments passed to 'construct' routine.
-
-        Returns
-        -------
-        dict
-            A dictionary having the following keys:
-            
-            kx: float
-                The field strength of the x-component of the dipole.
-                
-            ky: float
-                The field strength of the y-component of the dipole.
-
-            H: liepoly
-                The Hamiltonian of the cfm up to the requested order.
-
-            H_drift: liepoly
-                The drift part of H.
-
-            H_field: liepoly
-                The field part of H.
-                
-            g: dict
-                The g-components in Ref. [1]
-            G: dict
-                The G-components in Ref. [1]
-
-            So that H = H_drift + H_field.
+        Calculate the Hamiltonian of the combined-function magnet.
         '''
-        # compute the Hamiltonian of the drift
-        hard_edge_element.calcHamiltonian(self, **kwargs)
-        x, y, sigma, px, py, psigma = self._prop['coords']
-        # Compute the CFM vector potential
-        # G = (1 + Kx*x + Ky*y)*A_t near Eq. (2).
-        # Here G := G*e/p0 (The factor e/p0 can be absorbed in the coefficients later; see also the comment on page 4, right column)
-        g = self._g()
-        rp = (x + y*1j)/2
-        rm = rp.conjugate()
-        G = sum([rp**(k - j)*rm**j*g[(k, j)] for k, j in g.keys()]) # N.B.: We need to multiply g[(k, j)] from right in case their entries are jetpoly objects etc. They need to be added as the coefficients of the Lie polynomials. 
-        
-        # Assemble output Hamiltonians
-        out = {}
-        lamb0 = self.components[0]
-        kx = (lamb0 + lamb0.conjugate())/2 # lamb0.real; .conjugate() works with floats and other objects better than .real etc.
-        ky = (lamb0.conjugate() - lamb0)/2/1j # -lamb0.imag
-        # N.B.: Hfull = psigma - (1 + kx*x + ky*y)*drift - G
-        drift_s = self._prop['drift_sqrt'] # the square root expression in the Hamiltonian belonging to the drift
-        H_drift = psigma - drift_s
-        H_field = - drift_s*(x*kx + y*ky) - G
-        H_full = H_drift + H_field
-        
-        # remove any remaining constants; they do not affect the equations of motion.
-        H_full.pop((0, 0, 0, 0, 0, 0), None)
-        H_drift.pop((0, 0, 0, 0, 0, 0), None)
-        H_field.pop((0, 0, 0, 0, 0, 0), None)
-
-        out = {}
-        out['kx'] = kx
-        out['ky'] = ky
-        out['full'] = H_full
-        out['kick'] = H_field
-        out['G'] = G
-        out['g'] = g
-        self._prop.update(out)
-        self.full_hamiltonian = H_full
+        kwargs = self.__dict__
+        kwargs['components'] = self.components
+        kwargs['tilt'] = self.tilt
+        cfmh = CFMHamiltonian(**kwargs)
+        for k, v in cfmh.items():
+            setattr(self, k, v)
 
 class multipole(cfm):
-    def __init__(self, str=0, n: int=0, *args, **kwargs):
+    def __init__(self, fs=0, n: int=0, *args, **kwargs):
         '''
         Model of a multipole with exactly 2*n pole faces.
         
         Parameters
         ----------
+        fs: float or complex, optional
+            The field strength of the multipole. The real and imaginary part of 'fs' are understood to define the normal and skew components.
+            These components are given with respect to the x-axis (tilt 0) and an axis which is rotated relative to x by an angle of pi/2/n.
+        
         n: int, optional
             Defines the number 2*n of pole faces.
-
-         
-        expansion: int, optional
-            An additional parameter (>= n) by which one can control the number of terms in the expansion of the field.
         '''
         if n == 0: # drift case
             components = [0]
         else: # n > 0
             components = [0]*max([2, n]) # max([2, n]) because if n = 1 (the dipole case) then, since (1 + Kx*x + Ky*y)*(By + 1j*Bx) = - \partial_x G + 1j*\partial_y G (see p. 53 top in Ref. [2]), G must be of order <= 2.
-            # The real and imaginary part of 'str' are understood to define the normal and skew components of the sextupole.
-            # These components are given with respect to the x-axis (tilt 0) and an axis which is rotated relative to x by an angle of pi/2/n.
             #
             # Equivalently, these components are given by the real and imaginary parts of c_n with B_y + i B_x = c_n*(x + iy)**(n - 1), see e.g.
             # Eq. (1.8) in Ref. [2], using y=0 here. The c_n are just the components of the cfm.
             # Therefore:
-            components[n - 1] = str
-        cfm.__init__(self, components=components, *args, **kwargs)
+            components[n - 1] = fs
+        kwargs['components'] = components
+        cfm.__init__(self, *args, **kwargs)
+
         
 class drift(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=0, **kwargs)
         
 class dipole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=1, **kwargs)
         
 class quadrupole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=2, **kwargs)
         
+        
 class sextupole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=3, **kwargs)
+        
     
 class octupole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=4, **kwargs)
-        
-class rfc(hard_edge_element):
-    
-    def __init__(self, voltage, phase, frequency, beta0, *args, **kwargs):
-        '''
-        A generic RF cavity based on the simplest of all models.
-                
-        Reference(s):
-        [1] A. Wolski: Beam Dynamics in High Energy Particle Accelerators.
-        '''
-        assert 0 < beta0 and beta0 < 1
-        self.voltage = voltage
-        self.phase = phase
-        self.frequency = frequency # Actually, translated to: k = 2*np.pi/constants.speed_of_light*1/T
-        self.beta0 = beta0
-        hard_edge_element.__init__(self, *args, beta0=beta0, **kwargs)
-        
-    def calcHamiltonian(self, p=10, **kwargs):
-        '''
-        The Hamiltonian of a simplified RF cavity., see Ref. [1], Eq. (3.138) p. 112.
-        '''
-        hard_edge_element.calcHamiltonian(self, **kwargs)
-        x, y, sigma, px, py, psigma = self._prop['coords']
-        #k = 2*np.pi*self.frequency/constants.speed_of_light # 2.40483/radius # Eq. (3.132) in [1] and earlier: omega = k/c
-        #hamiltonian = construct(cos, sigma/beta0*-k + self.phase, **kwargs)*self.voltage
-        rf_potential = construct(cos, -sigma/self.beta0*self.frequency + self.phase, power=p, **kwargs)*self.voltage/float(np.pi)
-        hamiltonian = self._prop['full'] - rf_potential
-        hamiltonian.pop((0, 0, 0, 0, 0, 0), None) # remove any constant term
-        self.full_hamiltonian = hamiltonian
-        
-        
-        
-    
-
```

### Comparing `accphys-0.1.0/accphys/.ipynb_checkpoints/nf-checkpoint.py` & `accphys-0.1.1/accphys/.ipynb_checkpoints/nf-checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         kind = getattr(self, '_transform_kind', kind_inp)
         if kind != kind_inp:
             self.transform(kind=kind_inp)
         # 2. Determine requested integration length    
         t_nf = kwargs.get('t_nf', self.t_nf)
         if self.t_nf != t_nf:
             # re-calculate inner NF rotation with the new length
-            self._setup_nfRot(t_nf=t_nf)
+            self._setup_nfRot(t_nf=t_nf) # also sets self.t_nf
         
         # Tracking
         points = [self._transform_A2_inv(*self._transform_A2(*xieta))] # Applying A2 and back again ensures that the output will be in a common format (e.g. if one component is given in terms of a numpy array and the other component a float etc.
         xieta = self._transform_A2(*xieta) # apply the linear map first
         xi_nf = self.A(*xieta)
         for k in range(n_reps):
             xi_nf = self.nfRot(*xi_nf)
@@ -132,8 +132,9 @@
         
     def oneTurnMap(self, *xieta, **kwargs):
         kwargs['n_reps'] = 1
         return self.multiturn(*xieta, **kwargs)[-1]
     
     def __call__(self, *xieta, **kwargs):
         return self.oneTurnMap(*xieta, **kwargs)
-    
+
+
```

### Comparing `accphys-0.1.0/accphys/.ipynb_checkpoints/plotting-checkpoint.py` & `accphys-0.1.1/accphys/plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from legacycontour import _cntr as cntr
 import numpy as np
 import matplotlib.pyplot as plt
-from lieops.solver import getRealHamiltonFunction
+from lieops.solver.common import getRealHamiltonFunction
 
 def plot_contours(rham, xrange, yrange, levels=[], q=[], p=[], **kwargs):
     '''
     Show the contours of a real-valued Hamiltonian.
     
     plane:
         define what components to show
```

### Comparing `accphys-0.1.0/accphys/.ipynb_checkpoints/tools-checkpoint.py` & `accphys-0.1.1/accphys/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,29 @@
 # Collection of some common routines, used to plot and perform standard tasks
+import numpy as np
+from scipy import constants
+
+def energy2beta0(gev, particle_type='electron'):
+    # Convert energy in GeV to beta0 (for electrons)
+    energy_joule = gev*1e9*constants.electron_volt
+    if particle_type == 'electron':
+        m = constants.electron_mass
+    elif particle_type == 'proton':
+        m = constants.proton_mass
+    else:
+        raise RuntimeError('Particle type not understood.')
+    c = constants.speed_of_light
+    return np.sqrt(1 - m**2*c**4/energy_joule**2)
 
 def f_identity(*x):
     return x
 
 def f_compose(f, g):
     return lambda *x: f(*g(*x))
 
-def multiturn(bl, xi0, n_reps: int, post=lambda x: x):
-    '''
-    Perform tracking for a given number of repetitions.
-    
-    Parameters
-    ----------
-    bl: beamline, lieoperator or poly
-        The object through which we want to track.
-    
-    n_reps: int
-        The number of repetitions.
-        
-    xi0: The start vector xi0 = [xi0_1, xi0_2, ...]. By default: xi0_k = (q_k + i*p_k)/2, where q_k and
-         p_k are the canonical coordinates in ordinary phase space.
-    
-    post: callable, optional
-        An optional function to be applied after bl. 
-        Example: We want to compute (A o bl o B)**n at xi0, where A = B**(-1) are maps to normal form.
-        Then we need to record for Y0 := B(xi0) the values A(bl(Y0)), A(bl**2(Y0)) etc. Here A = post must
-        be inserted.
-    
-    Returns
-    -------
-    list
-        A list so that the k'th entry corresponds to the k-th component for the requested turns.
-    '''
-    dim = len(xi0)
-    point = xi0
-    points = [[] for c in range(dim)]
-    for k in range(n_reps):
-        point = bl(point)
-        post_point = post(point)
-        for c in range(dim):
-            points[c].append(post_point[c])
-    return points
-
-
 def detuning(nfdict):
     '''
     Get the detuning with amplitude terms for the given normal form dictionary which is returned by the bnf routine.
     
     Parameters
     ----------
     dict
@@ -149,7 +126,24 @@
                     if p[j] == 0: # Ensures that 0**0 = 1 so that e.g. (0, 0) (the constant term) is included
                         continue
                     prod *= action[j]**p[j]
                 sumk += prod*v
             out.append(sumk*s)
         return out
     return pa
+
+def get_optics(bl_optics, tol=1e-11):
+    '''
+    Obtain optics functions from the driving terms of a lattice.
+    '''
+    dterms = bl_optics
+    optics = {}
+    optics['betax'] = []
+    for pos in range(len(dterms)):
+        Sinv_pos = dterms[pos]['bnfout']['nfdict']['Sinv']
+        if tol > 0: # consistency check if Sinv_pos is purely imaginary
+            check = np.linalg.norm(Sinv_pos.imag)
+            assert check < tol, f'Matrix at {pos} not purely real: {check} >= {tol} (tol); point unstable?'
+        s00 = Sinv_pos.real[0, 0]
+        optics['betax'].append(1/s00**2)
+        
+    return optics
```

### Comparing `accphys-0.1.0/accphys/convert.py` & `accphys-0.1.1/accphys/io/.ipynb_checkpoints/from_pandas-checkpoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from .beamline import beamline
-from .elements import cfm
-from tqdm.auto import tqdm
-
-from latticeadaptor.core import LatticeAdaptor
-import numpy as np
-from njet.jet import factorials
+from accphys import beamline
+from accphys.elements import cfm
 
-def prepare_df(hdf, position_label='s', length_label='L', position=0, tol=1e-6, **kwargs):
+from tqdm import tqdm
+
+def _fill_gaps(hdf, position_label='s', length_label='L', position=0, tol=1e-6, **kwargs):
     '''
     Prepare a given data frame so that there will be no zero-spaces in between two elements.
     
     Parameters
     ----------
     hdf: pd.Dataframe
         Pandas dataframe object defining the beam sequence. The dataframe must contain the
@@ -71,25 +68,32 @@
             
             new_row = [0]*len(hdf.columns)
             new_row[position_label_index] = pos + length
             new_row[length_label_index] = empty_space
             hdf.loc[k + 0.5] = new_row # insert a new row in between k and k + 1
             
     return hdf.sort_index().reset_index(drop=True)
+    
 
 
-def to_beamline(hdf, beta0, component_labels, position_label='s', length_label='L', **kwargs):
+def from_pandas(hdf, component_labels, component_indices, position_label='s', length_label='L', **kwargs):
     '''
     Construct a beamline from a given lattice.
     
     Parameters
     ----------
     hdf: Pandas dataframe
         A Pandas dataframe object containing the position, lengths and field strengths of the individual
         elements in the beamline.
+                
+    component_labels
+        A list of floats, declaring the names of the columns in which to find the combined-function components.
+        
+    component_indices
+        A list of integers, where the k-th entry denotes the index of the respective component.
         
     position_label: str, optional
         Label denoting the position of the individual elements within the dataframe.
         
     length_label: str, optional
         Label denoting the lengths of the individual elements within the dataframe.
         
@@ -97,102 +101,52 @@
         Keyworded arguments passed to the cfm element.
         
     Returns
     -------
     beamline
         A beamline object representing the sequence of elements.
     '''
-    # Preparation; ensure that no empty space exists between elements (they will be filled with drifts if necesary):
-    hdf = prepare_df(hdf, position_label=position_label, length_label=length_label, **kwargs)
+    assert len(component_labels) > 0
+    assert len(component_labels) == len(component_indices)
+    # Preparation; ensure that no empty space exists between elements (they will be filled with drifts if necessary):
+    hdf = _fill_gaps(hdf, position_label=position_label, length_label=length_label, **kwargs)
             
     # group the given elements with respect to the remaining labels & find the uniques among them
     group_labels = [c for c in hdf.columns if c != position_label] # labels by which we distinguish different elements; custom columns may be added to artifically distinguish different element groups
     group_index_label = 'group_index'
     grp = hdf.groupby(group_labels, sort=False)
     hdf[group_index_label] = grp.ngroup()
     unique_elements = hdf.drop_duplicates(group_index_label)
     
     # build the elements:
     elements = []
     group_index = 0
-    for n in tqdm(range(len(unique_elements))):
+    n_components = max(component_indices) + 1 # + 1 because of the 0th-component
+    for n in tqdm(range(len(unique_elements)), disable=kwargs.get('disable_tqdm', False)):
         row = unique_elements.iloc[n]
-        components = [row[c] for c in component_labels]
-        length = row[length_label]
-        assert group_index == row[group_index_label] # verify that the position in the element list corresponds with the group index given by ngroup.
-        elements.append(cfm(beta0=beta0, components=components, length=length, **kwargs))
+        components = [0]*n_components
+        for j in range(len(component_indices)):
+            index = component_indices[j]
+            label = component_labels[j]
+            components[index] = row.get(label, 0)
+        length = row.get(length_label, 0)
+        assert group_index == row[group_index_label] # verify that the position in the element list corresponds to the group index given by ngroup.
+
+        element = cfm(components=components, length=length, **kwargs)
+        # special case: check for rbends etc. (TODO: improve this code, as it depends on the labels E1 and E2)
+        # we add sector rotation matrices if required.
+        #e1, e2 = row.get('E1', 0), row.get('E2', 0)
+        #if e1 != 0:
+        #    elements.append(polefaceRM(rho=element.rhox, phi=e1, length=0))
+
+        elements.append(element)
+
+        #if e2 != 0:
+        #    elements.append(polefaceRM(rho=element.rhox, phi=e2, length=0))
         group_index += 1
         
     # set the ordering
-    ordering = list(hdf[group_index_label])
+    ordering = list(hdf[group_index_label])  # ONGOING: need to separate the edges in advance before determining the unique groups of elements...
             
     return beamline(*elements, ordering=ordering)
 
 
-def from_madx(filename, beta0, **kwargs):
-    '''
-    Load MAD-X lattice from file, using LatticeAdaptor module, 
-    and construct a beamline object from the data.
-    
-    Parameters
-    ----------
-    filename: str
-        The name of the MAD-X lattice to be loaded.
-        
-    beta0: float
-        The realtivistic beta-factor (related to the energy of the beam). This is required later to
-        build the Hamiltonians.
-        
-    **kwargs
-        Optional arguments passed to 'to_beamline' routine.
-        
-    Returns
-    -------
-    beamline
-        A beamline object representing the sequence of elements in the given lattice.
-        
-    Pandas dataframe
-        A Pandas dataframe object, representing the loaded sequence of the lattice.
-    '''
-    la = LatticeAdaptor()
-    la.load_from_file(filename, ftype='madx')
-    raw_df = la.table
-    
-    # MAD-X specific labels
-    position_label='at'
-    length_label='L'
-    bend_kx_label = 'K0'
-    angle_label = 'ANGLE'
-    component_labels = [bend_kx_label, 'K1', 'K2']
-    madx_default_position = 0.5 # MAD-X tends to denote the position of the elements in the center
-
-    if bend_kx_label not in raw_df.columns:
-        # add kx
-        angles = raw_df[angle_label].values
-        lengths = raw_df[length_label].values 
-        valid_indices = np.logical_and((~np.isnan(angles)), lengths > 0)
-        kx = np.zeros(len(raw_df))
-        kx[valid_indices] = angles[valid_indices]/lengths[valid_indices] # r*phi = L; kx = 1/r
-        raw_df[bend_kx_label] = kx
-    
-    # drop elements with zero length and uneccesary columns;
-    # N.B. E1 and E2 denote rotation angles of the pole-faces. If they are non-zero,
-    # they are usually half the bend angle (in the rectangular case). We will ignore rectangular
-    # bends for the time being and use s-bends here.
-    columns_oi = [position_label, length_label] + component_labels
-    # if they exist, add skew-values to the components; TODO: check & verify this numerically
-    for j in range(1, 3):
-        if f'K{j}S' in raw_df.columns:
-            raw_df[f'K{j}'] = raw_df[f'K{j}'].values + raw_df[f'K{j}S']*1j
-    raw_df = raw_df.loc[raw_df[length_label] > 0][columns_oi]
-    
-    # (TO BE CHECKED; TODO)
-    facts = factorials(3)
-    for j in range(1, 3):
-        raw_df[f'K{j}'] = raw_df[f'K{j}'].values/facts[j]
-        
-    # construct the sequence of Lie operators
-    kwargs['position'] = kwargs.get('position', madx_default_position) 
-    seq2 = to_beamline(raw_df, beta0=beta0, 
-                      component_labels=component_labels, position_label=position_label,
-                      length_label=length_label, **kwargs)
-    return seq2, raw_df
```

### Comparing `accphys-0.1.0/accphys/elements.py` & `accphys-0.1.1/accphys/elements/cfm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,241 @@
 import numpy as np
+import warnings
 
-from njet.functions import cos
-from lieops import create_coords, construct
+from .common import hard_edge_element
+from .drift import DriftHamiltonian
 
-# N.B. the length of an element will be used only later, when it comes to calculating the flow.
+def _g(components, tilt=0):
+    '''
+    Compute the g-part of the cfm. Code taken in parts from my MAD-X implementation 
+    (see https://github.com/mtitze/MAD-X/blob/master/src/trrun.f90).
+    '''
+    exp = lambda z: complex(np.exp(z)) # convert numpy.float64 back to float as precaution to prevent unpredictable results if using jets etc.
+
+    # Eq. (2.40) resp. (2.47) in Ref. [2]:
+    # (By + 1j*Bx)_(phi = phi0) = sum_k components[k] r^k,
+    # where phi0 = tilt here.
+
+    # since kx = real(components[0]) and ky = -imag(components[0]), i.e.
+    # components[0] = kx - 1j*ky,
+    # we have:
+    kappa = components[0].conjugate()
+    barkappa = components[0]
+
+    # Now fill up the g_{ij}'s for j = 0, ..., i and i = 0, ..., len(components) - 1.
+    g = {}
+    g[(0, 0)] = 0
+    g[(1, 0)] = -barkappa
+    g[(1, 1)] = -kappa # = g[(1, 0)].conjugate()
+    for k in range(1, len(components) + 1): # k reflects the order up to which we consider the G-function
+        for j in range(k):
+            # Eq. (6), in Ref. [1]
+            g[(k + 1, j + 1)] = ( barkappa*g[(k, j + 1)]*(j + 1)*(j - k + 3/2) + 
+                                 kappa*g[(k, j)]*(k - j)*(1/2 - j) )/(k - j)/(j + 1)
+        # Eq. (8) in Ref. [1]
+        sum0 = 0
+        for j in range(1, k + 1):
+            sum0 = sum0 - (k + 1 - j)*g[(k + 1, j)]*exp(-tilt*2*1j*j)
+
+        g[(k + 1, 0)] = sum0/(k + 1)
+        # Add additional contributions from components, if they exist.
+        if k < len(components) + 1:
+            real = (barkappa*exp(tilt*1j) + kappa*exp(tilt*-1j))/2 # = Re(barkappa*exp(tilt*1j))
+            fk = -2**k*exp(tilt*-1j*k)
+            g[(k + 1, 0)] += fk*real*components[k - 1]/(k + 1)
+            if k < len(components):
+                g[(k + 1, 0)] += fk*components[k]/(k + 1)
+
+        g[(k + 1, k + 1)] = g[(k + 1, 0)].conjugate()
+    return g
+
+def CFMHamiltonian(components, tilt=0, tol_drop=0, **kwargs):
+    '''
+    Compute the Hamiltonian of the cfm (without electric fields).
+    For the underlying coordinate system and further details see Refs. [1, 2] below.
+    In particular, the Hamiltonian is given by Eq. (2.16) in Ref. [2].
+
+    Parameters
+    ----------
+    components: list, optional
+        A list of complex entries, denoting the components of the cfm field.
+        The components are hereby given with respect to a transversal axis, tilted against the Serre-Frenet
+        coordinate system by an angle of choice (see tilt parameter below and Eq. (2.40) in Ref. [2]).
+
+        If K_x = 0 this transverse axis smears out a cone. The ideal trajectory is hereby given by a horizontal
+        cut of the cone with a plane.
+        
+        Attention:
+        1) 
+        Additional zeros in the list will cause the routine to compute more orders of the CFM.
+        This becomes important if the cfm contains a non-zero dipole component and some other multipole components.
+        
+        2)
+        In the case of a single entry in the cfm components, an additional zero will be added internally so that
+        the resulting object describes a physical dipole. The reason is that (internally) the order of the G-function
+        in Ref. [2] has to be at least 2 or higher (see the topmost Eq. on p.53 in Ref. [2]). To suppress this behaviour,
+        the switch _addzero can be set to False.
+        
+    tilt: float, optional
+        The tilt between the dipole component and the higher-order magnet components of the cfm.
+    
+    tol_drop: float, optional
+        Threshold below terms in the Hamiltonian will be dropped.
+    
+    **kwargs
+        Optional keyword arguments passed to 'elements.drift.DriftHamiltonian'.
+
+    Returns
+    -------
+    dict
+        A dictionary having the following keys:
+        
+        kx: float
+            The field strength of the x-component of the dipole.
+            
+        ky: float
+            The field strength of the y-component of the dipole.
+
+        H: poly
+            The Hamiltonian of the cfm up to the requested order.
 
-# Reference(s):
-# [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
-# [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
+        H_drift: poly
+            The drift part of H.
 
-class hard_edge_element:
+        H_field: poly
+            The field part of H.
+            
+        g: dict
+            The g-components in Ref. [1]
+        G: dict
+            The G-components in Ref. [1]
+
+        So that H = H_drift + H_field.
+        
+    References
+    ----------
+    [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
+    [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
+    '''
+    # Compute the Hamiltonian of the drift
+    DH = DriftHamiltonian(tol_drop=tol_drop, **kwargs)
+    x, y, sigma, px, py, psigma = DH['coords']
+    # Compute the CFM vector potential
+    # G = (1 + Kx*x + Ky*y)*A_t near Eq. (2).
+    # Here G := G*e/p0 (The factor e/p0 can be absorbed in the coefficients later; see also the comment on page 4, right column)
+    g = _g(components=components, tilt=tilt)
+    rp = (x + y*1j)/2
+    rm = rp.conjugate()
+    G = sum([rp**(k - j)*rm**j*g[(k, j)] for k, j in g.keys()]) # N.B.: We need to multiply g[(k, j)] from right in case their entries are jetpoly objects etc. They need to be added as the coefficients of the Lie polynomials. 
     
-    def __init__(self, *args, length=1, **kwargs):
-        '''
-        Class to model the Hamiltonian of a 6D hard-edge element.
-        '''
-        self.length = length
-        if 'beta0' in kwargs.keys():
-            self.calcHamiltonian(*args, **kwargs)
-        if hasattr(self, 'full_hamiltonian'):
-            self.setHamiltonian(**kwargs)
+    # Also compute the derivatives of G
+    drp_G = sum([(k - j)*rp**(k - j - 1)*rm**j*g[(k, j)] for k, j in g.keys() if k != j]) # the partial derivative of G with respect to r_+
+    drm_G = sum([j*rp**(k - j)*rm**(j - 1)*g[(k, j)] for k, j in g.keys() if j != 0])
+    dx_G = (drp_G + drm_G)/2
+    dy_G = (-drp_G + drm_G)/2/1j
+    
+    # Assemble output Hamiltonians
+    lamb0 = components[0]
+    kx = (lamb0 + lamb0.conjugate())/2 # lamb0.real; .conjugate() works with floats and other objects better than .real etc.
+    ky = (lamb0.conjugate() - lamb0)/2/1j # -lamb0.imag
+    # N.B.: Hfull = psigma - (1 + kx*x + ky*y)*drift - G
+    drift_s = DH['drift_sqrt'] # the square root expression in the Hamiltonian belonging to the drift
+    H_drift = psigma - drift_s
+    H_field = - drift_s*(x*kx + y*ky) - G
+    H_full = H_drift + H_field
+    
+    # remove any remaining constants; they do not affect the equations of motion. Also drop all terms below the given threshold.
+    H_full = H_full.pop((0, 0, 0, 0, 0, 0), None).above(tol_drop)
+    H_drift = H_drift.pop((0, 0, 0, 0, 0, 0), None).above(tol_drop)
+    H_field = H_field.pop((0, 0, 0, 0, 0, 0), None).above(tol_drop)
+
+    out = DH
+    out['components'] = components
+    out['tilt'] = tilt
+    out['kx'] = kx
+    out['ky'] = ky
+    out['full'] = H_full
+    out['kick'] = H_field
+    out['G'] = G
+    out['drp_G'] = drp_G
+    out['drm_G'] = drm_G
+    out['dx_G'] = dx_G
+    out['dy_G'] = dy_G
+    out['g'] = g
+    out['hamiltonian'] = H_full
+    
+    if kx != 0:
+        out['rhox'] = 1/kx # kx = 1/r
+    else:
+        out['rhox'] = float(np.inf)
+        
+    if ky != 0:
+        out['rhoy'] = 1/ky
+    else:
+        out['rhoy'] = float(np.inf)
+    
+    return out
+    
+def _map(CFMH, x, y, sigma, px, py, psigma, ds):
+    r'''
+    An implementation of map (2.33) in Ref. [2].
+    
+    Parameters
+    ----------
+    CFMH: dict
+        The output of CFMHamiltonian, containing the Hamiltonian of the combined-function-magnet and additional information.
+    
+    ds: float
+        \delta_s according to Eq. (2.33) in Ref. [2].
         
-    def calcHamiltonian(self, beta0, sqrtexp: int=2, **kwargs):
-        '''
-        Compute the Hamiltonian of a drift.
-        For the underlying coordinate system and further details see Refs. [1, 2] below.
-        In particular, the Hamiltonian is given by Eq. (2.16) in Ref. [2].
+    References
+    ----------
+    [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
+    [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
+    '''
+    dx_G_map, dy_G_map = CFMH['dx_G'], CFMH['dy_G']
+    
+    sqrt2 = float(np.sqrt(2))
+    xi1 = (x + px*1j)/sqrt2
+    xi2 = (y + py*1j)/sqrt2
+    xi3 = (sigma + psigma*1j)/sqrt2
+    eta1 = (x - px*1j)/sqrt2
+    eta2 = (y - py*1j)/sqrt2
+    eta3 = (sigma - psigma*1j)/sqrt2
+    
+    dx_G = dx_G_map(xi1, xi2, xi3, eta1, eta2, eta3)
+    dy_G = dy_G_map(xi1, xi2, xi3, eta1, eta2, eta3)
+    
+    ux = px + dx_G*ds
+    uy = py + dy_G*ds
+    
+    # Preparation steps
+    beta0 = CFMH['beta0']
+    dE_E = psigma*beta0**2 # = eta in Ref. [2].
+    one_hateta2 = ((1 + dE_E)**2 - 1 + beta0**2)/beta0**2 # (1 + \hat \eta)**2; Eq. (2.17) in Ref. [2].
+    kx, ky = CFMH['kx'], CFMH['ky']
+    denominator = 1 + (kx**2 + ky**2)*ds**2
+    XI = (ux*kx + uy*ky)/denominator*2*ds
+    ZETA = (ux**2 + uy**2 - one_hateta2)/denominator
+    h = -XI/2 + np.sqrt(XI**2/4 - ZETA)
+    curv = 1 + kx*x + ky*y
+    
+    # Map (2.33) in Ref. [2]:
+    xf = x + ds*curv*(ux/h + ds*kx)
+    yf = y + ds*curv*(uy/h + ds*ky)
+    sigmaf = sigma + ds - ds*curv*(1 + dE_E)/h
+    pxf = ux + ds*kx*h
+    pyf = uy + ds*ky*h
+    psigmaf = psigma
+    
+    return xf, yf, sigmaf, pxf, pyf, psigmaf
+
 
-        Parameters
-        ----------
-        sqrtexp or power: int, optional
-            Power up to which the square root of the drift should be expanded. 
-        '''
-        assert 0 < beta0 and beta0 < 1
-        kwargs['power'] = kwargs.get('power', sqrtexp)
-        # Compute the CFM drift part
-        x, y, sigma, px, py, psigma = create_coords(3, real=True, **kwargs)
-        one_hateta2 = lambda ps: ((1 + ps*beta0**2)**2 - 1 + beta0**2)/beta0**2 # Eqs. (15c) and (17) in Ref. [1]
-        sqrt = lambda p1, p2, ps: (one_hateta2(ps) - p1**2 - p2**2)**(1/2)
-        drift_s = construct(sqrt, px, py, psigma, **kwargs) # expand sqrt around [px, py, psigma] = [0, 0, 0] up to power
-        hamiltonian = psigma - drift_s
-        hamiltonian.pop((0, 0, 0, 0, 0, 0), None)
-        self.full_hamiltonian = hamiltonian
-        self._prop = {}
-        self._prop['beta0'] = beta0
-        self._prop['sqrtexp'] = sqrtexp
-        self._prop['drift'] = hamiltonian
-        self._prop['drift_sqrt'] = drift_s
-        self._prop['full'] = hamiltonian
-        self._prop['coords'] = x, y, sigma, px, py, psigma
-        
-    def setHamiltonian(self, *projection, **kwargs):
-        '''
-        Set Hamiltonian by dropping components associated with terms not in given list.
-        
-        self.hamiltonian will be updated.
-        
-        !! Attention !!
-        After this operation it may become necessary to re-caclulate flows and the one-turn map again.
-        
-        Parameters
-        ----------
-        projection: int
-            The indices of the coordinates of interest. Must reach from 0 to self.full_hamiltonian.dim.
-            If there are no arguments given, then the default Hamiltonian will be restored.
-        '''
-        # consistency checks
-        new_dim = len(projection)
-        ham = self.full_hamiltonian
-        if new_dim == 0: # default: 6D Hamiltonian
-            projection = range(ham.dim)
-            new_dim = ham.dim
-        assert new_dim <= ham.dim and max(projection) < ham.dim, 'Number of spatial dimensions too large.'
-        projection = list(projection) + [p + ham.dim for p in projection] # the eta-components duplicate the indices.
-        complement = [k for k in range(2*ham.dim) if not k in projection]
-        new_values = {}
-        for k, v in ham.items():
-            if any([k[p] != 0 for p in complement]): # only keep those coefficients which do not couple to other directions
-                continue
-            new_values[tuple([k[p] for p in projection])] = v
-        self.hamiltonian = ham.__class__(values=new_values, dim=new_dim, max_power=ham.max_power)
-        
-    def copy(self):
-        result = self.__class__(length=self.length)
-        # copy all the fields
-        for field, value in self.__dict__.items():
-            setattr(result, field, value)
-        return result
-        
-class phaserot(hard_edge_element):
-    def __init__(self, *tunes, length=1, **kwargs):
-        '''
-        A generic uncoupled phase (space) rotation.
-        
-        Parameters
-        ----------
-        tunes: float or array_like
-            Tune(s) defining the phase rotation.
-        '''
-        self.tunes = tunes
-        self.length = length
-        if len(tunes) > 0:
-            self.calcHamiltonian(*tunes, **kwargs)
-        if hasattr(self, 'full_hamiltonian'):
-            self.setHamiltonian(**kwargs)
-        
-    def calcHamiltonian(self, *tunes, **kwargs):
-        dim = len(tunes)
-        xieta = create_coords(dim=dim)
-        self.full_hamiltonian = sum([-tunes[k]*xieta[k]*xieta[k + dim] for k in range(dim)])
-        
-        
 class cfm(hard_edge_element):
-    def __init__(self, components=[0], tilt=0, *args, **kwargs):
+    def __init__(self, components=[0], tilt=0, warn=True, **kwargs):
         '''
         Class to model a combined-function-magnetc (cfm).
 
         Parameters
         ----------
         beta0: float
             Relativistic beta = v/c of the reference trajectory.
@@ -125,233 +244,118 @@
             A list of complex entries, denoting the components of the cfm field.
             The components are hereby given with respect to a transversal axis, tilted against the Serre-Frenet
             coordinate system by an angle of choice (see tilt parameter below and Eq. (2.40) in Ref. [2]).
 
             If K_x = 0 this transverse axis smears out a cone. The ideal trajectory is hereby given by a horizontal
             cut of the cone with a plane.
             
-            Note that additional zeros in the list will cause the routine to compute more orders of the CFM.
+            Attention:
+            1) 
+            Additional zeros in the list will cause the routine to compute more orders of the CFM.
+            This becomes important if the cfm contains a non-zero dipole component and some other multipole components.
             
+            2)
+            In the case of a single entry in the cfm components, an additional zero will be added internally so that
+            the resulting object describes a physical dipole. The reason is that (internally) the order of the G-function
+            in Ref. [2] has to be at least 2 or higher (see the topmost Eq. on p.53 in Ref. [2]). To suppress this behaviour,
+            the switch _addzero can be set to False.
+                        
         tilt: float, optional
             The tilt between the dipole component and the higher-order magnet components of the cfm.
             
-        **kwargs
-            Optional arguments passed to self.calcHamiltonian and self.setHamiltonian.
+        References
+        ----------
+        [1] M. Titze: "Approach to Combined-function magnets via symplectic slicing", Phys. Rev. STAB 19 054002 (2016)
+        [2] M. Titze: "Space Charge Modeling at the Integer Resonance for the CERN PS and SPS", PhD Thesis (2019)
         '''
+        assert len(components) > 0
         self.components = components
         self.tilt = tilt
-        hard_edge_element.__init__(self, *args, **kwargs)
-        
-    def setHamiltonian(self, *args, **kwargs):
+        hard_edge_element.__init__(self, warn=False, **kwargs)
+
+        # also compute the overal bend angles, if a length has been provided:
+        if hasattr(self, 'length'):
+            self.phix = self.length*self.kx # r*phi = L; kx = 1/r
+            self.phiy = self.length*self.ky
+        else:
+            if warn:
+                warnings.warn('Length of dipole not specified. Bend angle can not be determined.')
+
+
+    def setStyle(self, *args, **kwargs):
         '''
-        Set self.hamiltonian to requested dimension.
-        
         Parameters
         ----------
         style: str, optional
-            Name of the key in self._prop denoting the Hamiltonian to be used.
+            Name of the field in 'self', denoting the Hamiltonian to be used.
             Supported options are:
             'full': use the full Hamiltonian (default)
             'kick': Only use the Hamiltonian containing field-components (see Eq. (2.36) in Ref. [2])
             'drift': Only the drift part of the Hamiltonian is used, i.e. all fields switched off.
         '''
         supported_styles = ['full', 'kick', 'drift']
         if not hasattr(self, '_style') or 'style' in kwargs.keys():
             self._style = kwargs.get('style', 'full')
         if not self._style in supported_styles:
             raise RuntimeError(f"Style '{self._style}' not recognized. Supported styles:\n{supported_styles}")
-        self.full_hamiltonian = self._prop[self._style]
-        hard_edge_element.setHamiltonian(self, *args, **kwargs)
-    
-    def _g(self):
-        '''
-        Compute the g-part of the cfm. Code taken in parts from my MAD-X implementation 
-        (see https://github.com/mtitze/MAD-X/blob/master/src/trrun.f90).
-        '''
-        exp = lambda z: complex(np.exp(z)) # convert numpy.float64 back to float as precaution to prevent unpredictable results if using jets etc.
-
-        # Eq. (2.40) resp. (2.47) in Ref. [2]:
-        # (By + 1j*Bx)_(phi = phi0) = sum_k components[k] r^k,
-        # where phi0 = tilt here.
-
-        # since kx = real(components[0]) and ky = -imag(components[0]), i.e.
-        # components[0] = kx - 1j*ky,
-        # we have:
-        kappa = self.components[0].conjugate()
-        barkappa = self.components[0]
-
-        nord = len(self.components) - 1
-        # Now fill up the g_{ij}'s for j = 0, ..., i and i = 0, ..., nord + 1.
-        g = {}
-        g[(0, 0)] = 0
-        g[(1, 0)] = -barkappa
-        g[(1, 1)] = -kappa # = g[(1, 0)].conjugate()
-        for k in range(1, nord + 1):
-            for j in range(k):
-                # Eq. (6), in Ref. [1]
-                g[(k + 1, j + 1)] = ( barkappa*g[(k, j + 1)]*(j + 1)*(j - k + 3/2) + 
-                                     kappa*g[(k, j)]*(k - j)*(1/2 - j) )/(k - j)/(j + 1)
-            # Eq. (8) in Ref. [1]
-            sum0 = 0
-            for j in range(1, k + 1):
-                sum0 = sum0 - (k + 1 - j)*g[(k + 1, j)]*exp(-self.tilt*2*1j*j)
-            g[(k + 1, 0)] = ( sum0 - 2**k*exp(-self.tilt*1j*k)*( self.components[k] 
-                            + 1/2*(barkappa*exp(self.tilt*1j) + kappa*exp(self.tilt*-1j))*self.components[k - 1] ) )/(k + 1)
-            g[(k + 1, k + 1)] = g[(k + 1, 0)].conjugate()
-        return g
+        self.hamiltonian = getattr(self, self._style)
 
     def calcHamiltonian(self, **kwargs):
         '''
-        Compute the Hamiltonian of the cfm (without electric fields).
-        For the underlying coordinate system and further details see Refs. [1, 2] below.
-        In particular, the Hamiltonian is given by Eq. (2.16) in Ref. [2].
-
-        Parameters
-        ----------
-        **kwargs
-            Optional keyword arguments passed to 'construct' routine.
-
-        Returns
-        -------
-        dict
-            A dictionary having the following keys:
-            
-            kx: float
-                The field strength of the x-component of the dipole.
-                
-            ky: float
-                The field strength of the y-component of the dipole.
-
-            H: liepoly
-                The Hamiltonian of the cfm up to the requested order.
-
-            H_drift: liepoly
-                The drift part of H.
-
-            H_field: liepoly
-                The field part of H.
-                
-            g: dict
-                The g-components in Ref. [1]
-            G: dict
-                The G-components in Ref. [1]
-
-            So that H = H_drift + H_field.
+        Calculate the Hamiltonian of the combined-function magnet.
         '''
-        # compute the Hamiltonian of the drift
-        hard_edge_element.calcHamiltonian(self, **kwargs)
-        x, y, sigma, px, py, psigma = self._prop['coords']
-        # Compute the CFM vector potential
-        # G = (1 + Kx*x + Ky*y)*A_t near Eq. (2).
-        # Here G := G*e/p0 (The factor e/p0 can be absorbed in the coefficients later; see also the comment on page 4, right column)
-        g = self._g()
-        rp = (x + y*1j)/2
-        rm = rp.conjugate()
-        G = sum([rp**(k - j)*rm**j*g[(k, j)] for k, j in g.keys()]) # N.B.: We need to multiply g[(k, j)] from right in case their entries are jetpoly objects etc. They need to be added as the coefficients of the Lie polynomials. 
-        
-        # Assemble output Hamiltonians
-        out = {}
-        lamb0 = self.components[0]
-        kx = (lamb0 + lamb0.conjugate())/2 # lamb0.real; .conjugate() works with floats and other objects better than .real etc.
-        ky = (lamb0.conjugate() - lamb0)/2/1j # -lamb0.imag
-        # N.B.: Hfull = psigma - (1 + kx*x + ky*y)*drift - G
-        drift_s = self._prop['drift_sqrt'] # the square root expression in the Hamiltonian belonging to the drift
-        H_drift = psigma - drift_s
-        H_field = - drift_s*(x*kx + y*ky) - G
-        H_full = H_drift + H_field
-        
-        # remove any remaining constants; they do not affect the equations of motion.
-        H_full.pop((0, 0, 0, 0, 0, 0), None)
-        H_drift.pop((0, 0, 0, 0, 0, 0), None)
-        H_field.pop((0, 0, 0, 0, 0, 0), None)
-
-        out = {}
-        out['kx'] = kx
-        out['ky'] = ky
-        out['full'] = H_full
-        out['kick'] = H_field
-        out['G'] = G
-        out['g'] = g
-        self._prop.update(out)
-        self.full_hamiltonian = H_full
+        kwargs = self.__dict__
+        kwargs['components'] = self.components
+        kwargs['tilt'] = self.tilt
+        cfmh = CFMHamiltonian(**kwargs)
+        for k, v in cfmh.items():
+            setattr(self, k, v)
 
 class multipole(cfm):
-    def __init__(self, str=0, n: int=0, *args, **kwargs):
+    def __init__(self, fs=0, n: int=0, *args, **kwargs):
         '''
         Model of a multipole with exactly 2*n pole faces.
         
         Parameters
         ----------
+        fs: float or complex, optional
+            The field strength of the multipole. The real and imaginary part of 'fs' are understood to define the normal and skew components.
+            These components are given with respect to the x-axis (tilt 0) and an axis which is rotated relative to x by an angle of pi/2/n.
+        
         n: int, optional
             Defines the number 2*n of pole faces.
-
-         
-        expansion: int, optional
-            An additional parameter (>= n) by which one can control the number of terms in the expansion of the field.
         '''
         if n == 0: # drift case
             components = [0]
         else: # n > 0
             components = [0]*max([2, n]) # max([2, n]) because if n = 1 (the dipole case) then, since (1 + Kx*x + Ky*y)*(By + 1j*Bx) = - \partial_x G + 1j*\partial_y G (see p. 53 top in Ref. [2]), G must be of order <= 2.
-            # The real and imaginary part of 'str' are understood to define the normal and skew components of the sextupole.
-            # These components are given with respect to the x-axis (tilt 0) and an axis which is rotated relative to x by an angle of pi/2/n.
             #
             # Equivalently, these components are given by the real and imaginary parts of c_n with B_y + i B_x = c_n*(x + iy)**(n - 1), see e.g.
             # Eq. (1.8) in Ref. [2], using y=0 here. The c_n are just the components of the cfm.
             # Therefore:
-            components[n - 1] = str
-        cfm.__init__(self, components=components, *args, **kwargs)
+            components[n - 1] = fs
+        kwargs['components'] = components
+        cfm.__init__(self, *args, **kwargs)
+
         
 class drift(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=0, **kwargs)
         
 class dipole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=1, **kwargs)
         
 class quadrupole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=2, **kwargs)
         
+        
 class sextupole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=3, **kwargs)
+        
     
 class octupole(multipole):
     def __init__(self, *args, **kwargs):
         multipole.__init__(self, *args, n=4, **kwargs)
-        
-class rfc(hard_edge_element):
-    
-    def __init__(self, voltage, phase, frequency, beta0, *args, **kwargs):
-        '''
-        A generic RF cavity based on the simplest of all models.
-                
-        Reference(s):
-        [1] A. Wolski: Beam Dynamics in High Energy Particle Accelerators.
-        '''
-        assert 0 < beta0 and beta0 < 1
-        self.voltage = voltage
-        self.phase = phase
-        self.frequency = frequency # Actually, translated to: k = 2*np.pi/constants.speed_of_light*1/T
-        self.beta0 = beta0
-        hard_edge_element.__init__(self, *args, beta0=beta0, **kwargs)
-        
-    def calcHamiltonian(self, p=10, **kwargs):
-        '''
-        The Hamiltonian of a simplified RF cavity., see Ref. [1], Eq. (3.138) p. 112.
-        '''
-        hard_edge_element.calcHamiltonian(self, **kwargs)
-        x, y, sigma, px, py, psigma = self._prop['coords']
-        #k = 2*np.pi*self.frequency/constants.speed_of_light # 2.40483/radius # Eq. (3.132) in [1] and earlier: omega = k/c
-        #hamiltonian = construct(cos, sigma/beta0*-k + self.phase, **kwargs)*self.voltage
-        rf_potential = construct(cos, -sigma/self.beta0*self.frequency + self.phase, power=p, **kwargs)*self.voltage/float(np.pi)
-        hamiltonian = self._prop['full'] - rf_potential
-        hamiltonian.pop((0, 0, 0, 0, 0, 0), None) # remove any constant term
-        self.full_hamiltonian = hamiltonian
-        
-        
-        
-    
-
```

### Comparing `accphys-0.1.0/accphys/nf.py` & `accphys-0.1.1/accphys/nf.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         kind = getattr(self, '_transform_kind', kind_inp)
         if kind != kind_inp:
             self.transform(kind=kind_inp)
         # 2. Determine requested integration length    
         t_nf = kwargs.get('t_nf', self.t_nf)
         if self.t_nf != t_nf:
             # re-calculate inner NF rotation with the new length
-            self._setup_nfRot(t_nf=t_nf)
+            self._setup_nfRot(t_nf=t_nf) # also sets self.t_nf
         
         # Tracking
         points = [self._transform_A2_inv(*self._transform_A2(*xieta))] # Applying A2 and back again ensures that the output will be in a common format (e.g. if one component is given in terms of a numpy array and the other component a float etc.
         xieta = self._transform_A2(*xieta) # apply the linear map first
         xi_nf = self.A(*xieta)
         for k in range(n_reps):
             xi_nf = self.nfRot(*xi_nf)
@@ -132,8 +132,9 @@
         
     def oneTurnMap(self, *xieta, **kwargs):
         kwargs['n_reps'] = 1
         return self.multiturn(*xieta, **kwargs)[-1]
     
     def __call__(self, *xieta, **kwargs):
         return self.oneTurnMap(*xieta, **kwargs)
-    
+
+
```

### Comparing `accphys-0.1.0/accphys/tools.py` & `accphys-0.1.1/accphys/.ipynb_checkpoints/tools-checkpoint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,17 @@
 # Collection of some common routines, used to plot and perform standard tasks
+import numpy as np
+from scipy import constants
+
+def energy2beta0(gev):
+    # Convert energy in GeV to beta0 (for electrons)
+    energy_joule = gev*1e9*constants.electron_volt
+    m = constants.electron_mass
+    c = constants.speed_of_light
+    return np.sqrt(1 - m**2*c**4/energy_joule**2)
 
 def f_identity(*x):
     return x
 
 def f_compose(f, g):
     return lambda *x: f(*g(*x))
 
@@ -112,7 +121,24 @@
                     if p[j] == 0: # Ensures that 0**0 = 1 so that e.g. (0, 0) (the constant term) is included
                         continue
                     prod *= action[j]**p[j]
                 sumk += prod*v
             out.append(sumk*s)
         return out
     return pa
+
+def get_optics(bl_optics, tol=1e-11):
+    '''
+    Obtain optics functions from the driving terms of a lattice.
+    '''
+    dterms = bl_optics
+    optics = {}
+    optics['betax'] = []
+    for pos in range(len(dterms)):
+        Sinv_pos = dterms[pos]['bnfout']['nfdict']['Sinv']
+        if tol > 0: # consistency check if Sinv_pos is purely imaginary
+            check = np.linalg.norm(Sinv_pos.imag)
+            assert check < tol, f'Matrix at {pos} not purely real: {check} >= {tol} (tol); point unstable?'
+        s00 = Sinv_pos.real[0, 0]
+        optics['betax'].append(1/s00**2)
+        
+    return optics
```

### Comparing `accphys-0.1.0/pyproject.toml` & `accphys-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 [tool.poetry]
 name = "accphys"
-version = "0.1.0"
+version = "0.1.1"
 description = "Analyze non-linear single-particle storage ring dynamics"
 authors = ["Malte Titze <mtitze@users.noreply.github.com>"]
 license = "GPL v3"
 
 [tool.poetry.dependencies]
 python = "^3.8, <3.11"
 lieops = "^0.1.1"
 scipy = "^1.8.0"
-pandas = "^1.4.2"
-matplotlib = "^3.5.1"
 tqdm = "^4.64.0"
-#ipykernel = "^6.13.0"
 ipykernel = "^5.5.5"
-latticeadaptor = ">=0.3.9"
-#latticeadaptor = { git = "https://github.com/mtitze/latticeadaptor.git", branch = "main" }
+cpymad = ">=1.10.0"
 
 [tool.poetry.dev-dependencies]
 #ipykernel = "^6.13.0"
 ipykernel = "^5.5.5"
 ipywidgets = "^7.7.0"
 
 [build-system]
```

### Comparing `accphys-0.1.0/setup.py` & `accphys-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['accphys',
  'accphys..ipynb_checkpoints',
- 'accphys.solver',
- 'accphys.solver..ipynb_checkpoints']
+ 'accphys.elements',
+ 'accphys.elements..ipynb_checkpoints',
+ 'accphys.io',
+ 'accphys.io..ipynb_checkpoints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ipykernel>=5.5.5,<6.0.0',
- 'latticeadaptor>=0.3.9',
+['cpymad>=1.10.0',
+ 'ipykernel>=5.5.5,<6.0.0',
  'lieops>=0.1.1,<0.2.0',
- 'matplotlib>=3.5.1,<4.0.0',
- 'pandas>=1.4.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'tqdm>=4.64.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'accphys',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Analyze non-linear single-particle storage ring dynamics',
     'long_description': None,
     'author': 'Malte Titze',
     'author_email': 'mtitze@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `accphys-0.1.0/PKG-INFO` & `accphys-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: accphys
-Version: 0.1.0
+Version: 0.1.1
 Summary: Analyze non-linear single-particle storage ring dynamics
 License: GPL v3
 Author: Malte Titze
 Author-email: mtitze@users.noreply.github.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: cpymad (>=1.10.0)
 Requires-Dist: ipykernel (>=5.5.5,<6.0.0)
-Requires-Dist: latticeadaptor (>=0.3.9)
 Requires-Dist: lieops (>=0.1.1,<0.2.0)
-Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
-Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
```

