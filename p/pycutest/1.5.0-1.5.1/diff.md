# Comparing `tmp/pycutest-1.5.0.tar.gz` & `tmp/pycutest-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutest-1.5.0.tar", last modified: Wed Feb 22 11:38:10 2023, max compression
+gzip compressed data, was "pycutest-1.5.1.tar", last modified: Tue Aug  8 12:10:20 2023, max compression
```

## Comparing `pycutest-1.5.0.tar` & `pycutest-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 11:38:10.943684 pycutest-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-22 11:38:10.000000 pycutest-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-02-22 11:38:10.943684 pycutest-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-02-22 11:38:10.000000 pycutest-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 11:38:10.939684 pycutest-1.5.0/pycutest/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/build_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    70681 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/c_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/install_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    43016 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/problem_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/python_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/sifdecode_extras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/system_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 11:38:10.943684 pycutest-1.5.0/pycutest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 11:38:10.000000 pycutest-1.5.0/pycutest.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 11:38:10.943684 pycutest-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-02-22 11:38:10.000000 pycutest-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:20.833127 pycutest-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-08 12:10:19.000000 pycutest-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-08 12:10:20.833127 pycutest-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-08-08 12:10:19.000000 pycutest-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:20.833127 pycutest-1.5.1/pycutest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/build_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70681 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/install_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43134 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/problem_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/python_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/sifdecode_extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/system_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:10:19.000000 pycutest-1.5.1/pycutest/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:10:20.833127 pycutest-1.5.1/pycutest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-08 12:10:20.000000 pycutest-1.5.1/pycutest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-08 12:10:20.000000 pycutest-1.5.1/pycutest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:10:20.000000 pycutest-1.5.1/pycutest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 12:10:20.000000 pycutest-1.5.1/pycutest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 12:10:20.000000 pycutest-1.5.1/pycutest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:10:20.000000 pycutest-1.5.1/pycutest.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:10:20.833127 pycutest-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-08 12:10:19.000000 pycutest-1.5.1/setup.py
```

### Comparing `pycutest-1.5.0/LICENSE` & `pycutest-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/PKG-INFO` & `pycutest-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycutest
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Python wrapper to the CUTEst optimization test environment
 Home-page: https://github.com/jfowkes/pycutest/
 Author: Jaroslav Fowkes and Lindon Roberts
 Author-email: jaroslav.fowkes@maths.ox.ac.uk
 License: GNU GPL
 Download-URL: https://github.com/jfowkes/pycutest/releases/
 Project-URL: Bug Tracker, https://github.com/jfowkes/pycutest/issues/
```

### Comparing `pycutest-1.5.0/README.rst` & `pycutest-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/pycutest/__init__.py` & `pycutest-1.5.1/pycutest/__init__.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/pycutest/build_interface.py` & `pycutest-1.5.1/pycutest/build_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,20 +133,14 @@
       ``-param key=str(value)`` to the sifdecode's command line options.
     * *sifOptions* -- additional options passed to sifdecode given in the form of a list of strings.
     * *quiet* -- supress output (default ``True``)
 
     *destination* must not contain dots because it is a part of a Python module name.
     """
 
-    # Define FileNotFoundError on Python 2
-    try:
-        FileNotFoundError
-    except NameError:
-        FileNotFoundError = OSError
-
     # Default destination
     if destination is None:
         destination=problemName
 
     # The problem's cache entry
     problemDir = get_problem_directory(destination, sifParams=sifParams)
 
@@ -159,22 +153,26 @@
 
     # Additional args
     args=[]
 
     # Handle params
     if sifParams is not None:
         for (key, value) in sifParams.items():
-            if type(key) is not str and type(key) is not unicode:
+            if type(key) is not str:
+                if fromDir is not None:
+                    os.chdir(fromDir) # Go back to original work directory
                 raise Exception("sifParams keys must be strings")
             args+=['-param', key+"="+str(value)]
 
     # Handle options
     if sifOptions is not None:
         for opt in sifOptions:
-            if type(opt) is not str and type(key) is not unicode:
+            if type(opt) is not str:
+                if fromDir is not None:
+                    os.chdir(fromDir) # Go back to original work directory
                 raise Exception("sifOptions must consist of strings")
             args+=[str(opt)]
 
     # Call sifdecode
     spawnOK=True
     try:
         # Start sifdecode
@@ -204,30 +202,36 @@
     for l in msg_lines:
         if 'WARNING' in l:
             param_error = l.replace('WARNING: ', '').replace(' -- skipping', '')
         if not spawnOK or not quiet:
             print(l)
     if not spawnOK:
         clear_cache(problemName, sifParams=sifParams)
+        if fromDir is not None:
+            os.chdir(fromDir) # Go back to original work directory
         raise RuntimeError('SIFDECODE failed, check output printed above')
     if param_error is not None:
         clear_cache(problemName, sifParams=sifParams)
+        if fromDir is not None:
+            os.chdir(fromDir) # Go back to original work directory
         raise RuntimeError('SIFDECODE error: %s' % param_error)
 
     # Collect all .f files
     filelist=glob('*.f')
 
     # Compile FORTRAN files
     for filename in filelist:
         cmd=['gfortran', '-fPIC', '-c', filename]
         if not quiet:
             for s in cmd:
                 print(s, end=' ')
             print()
         if subprocess.call(cmd)!=0:
+            if fromDir is not None:
+                os.chdir(fromDir) # Go back to original work directory
             raise RuntimeError("gfortran call failed for "+filename)
 
     # Collect list of all object files (.o)
     objFileList=glob('*.o')
 
     # Go back to original work directory
     if fromDir is not None:
@@ -289,18 +293,20 @@
     if quiet:
         quietopt=['-q']
     else:
         quietopt=[]
 
     # Call 'python setup.py build'
     if subprocess.call([sys.executable, 'setup.py']+quietopt+['build'])!=0:
+        os.chdir(fromDir) # Go back to original work directory
         raise RuntimeError("Failed to build the Python interface module")
 
     # Call 'python setup.py build_ext --inplace'
     if subprocess.call([sys.executable, 'setup.py']+quietopt+['build_ext', '--inplace'])!=0:
+        os.chdir(fromDir) # Go back to original work directory
         raise RuntimeError("Failed to install the Python interface module")
 
     # Create __init__.py
     f=open('__init__.py', 'w+')
     f.write(get_init_script(problemName, efirst, lfirst, nvfirst, sifParams, sifOptions))
     f.close()
```

### Comparing `pycutest-1.5.0/pycutest/c_interface.py` & `pycutest-1.5.1/pycutest/c_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/pycutest/install_scripts.py` & `pycutest-1.5.1/pycutest/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/pycutest/problem_class.py` & `pycutest-1.5.1/pycutest/problem_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,24 +345,24 @@
         if gradient:
             if index is None:
                 c, J = self._module.cons(self.free_to_all(x), True)
                 return c, J[:, self.idx_free]
             else:
                 assert 0 <= index <= self.m - 1, "Invalid constraint index %g (must be in 0..%g)" % (index, self.m-1)
                 ci, Ji = self._module.cons(self.free_to_all(x), True, index)
-                ci = float(ci)  # convert from 1x1 NumPy array to float
+                ci = ci[0]  # convert from 1x1 NumPy array to float
                 return ci, self.all_to_free(Ji)
         else:
             if index is None:
                 c = self._module.cons(self.free_to_all(x))
                 return c
             else:
                 assert 0 <= index <= self.m - 1, "Invalid constraint index %g (must be in 0..%g)" % (index, self.m - 1)
                 ci = self._module.cons(self.free_to_all(x), False, index)
-                ci = float(ci)  # convert from 1x1 NumPy array to float
+                ci = ci[0]  # convert from 1x1 NumPy array to float
                 return ci
 
     def lagjac(self, x, v=None):
         """
         Evaluate gradient of objective or Lagrangian, and Jacobian of constraints.
 
         .. code-block:: python
@@ -608,27 +608,27 @@
 
         Input
         x -- 1D array of length n with the values of variables
         i -- integer index of constraint (between 0 and m-1)
 
         Output
         c  -- 1D array of length m holding the values of constraints at x
-        J  -- a scipy.sparse.coo_matrix of size m-by-n holding the Jacobian at x
+        J  -- a scipy.sparse.coo_matrix of size m-by-n_full holding the Jacobian at x
         ci -- 1D array of length 1 holding the value of i-th constraint at x
-        gi -- a scipy.sparse.coo_matrix of size 1-by-n holding the gradient of i-th constraint at x
+        gi -- a scipy.sparse.coo_matrix of size 1-by-n_full holding the gradient of i-th constraint at x
 
         This function is a wrapper for scons().
         """
 
         if i is None:
             (c, Ji, Jif, Jv)=self._module.scons(x)
-            return (c, coo_matrix((Jv, (Jif, Ji)), shape=(self.m, self.n)))
+            return (c, coo_matrix((Jv, (Jif, Ji)), shape=(self.m, self.n_full)))
         else:
             (c, gi, gv)=self._module.scons(x, i)
-            return (c, coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n)))
+            return (c, coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n_full)))
 
     def scons(self, x, index=None, gradient=False):
         """
         Evaluate the constraints (and optionally their sparse Jacobian or gradient).
 
         .. code-block:: python
 
@@ -666,15 +666,15 @@
             if gradient:
                 return c, sparse_mat_extract_columns(J, self.idx_free)
             else:
                 return c
         else:
             assert 0 <= index <= self.m - 1, "Invalid constraint index %g (must be in 0..%g)" % (index, self.m - 1)
             ci, Ji = self.__scons(self.free_to_all(x), index)
-            ci = float(ci)  # convert from 1x1 NumPy array to float
+            ci = ci[0]  # convert from 1x1 NumPy array to float
             if gradient:
                 return ci, sparse_vec_extract_indices(Ji, self.idx_free)
             else:
                 return ci
 
     # slagjac() wrapper
     def __slagjac(self, x, v=None):
@@ -685,29 +685,29 @@
         (g, J)=__slagjac(x, v) -- Lagrangian gradient and Jacobian
 
         Input
         x -- 1D array of length n with the values of variables
         v -- 1D array of length m with the values of Lagrange multipliers
 
         Output
-        g -- a scipy.sparse.coo_matrix of size 1-by-n holding the gradient of objective at x or
+        g -- a scipy.sparse.coo_matrix of size 1-by-n_full holding the gradient of objective at x or
             the gradient of Lagrangian at (x, v)
-        J -- a scipy.sparse.coo_matrix of size m-by-n holding the sparse Jacobian
+        J -- a scipy.sparse.coo_matrix of size m-by-n_full holding the sparse Jacobian
             of constraints at x
 
         This function is a wrapper for slagjac().
         """
 
         if v is None:
             (gi, gv, Ji, Jfi, Jv)=self._module.slagjac(x)
         else:
             (gi, gv, Ji, Jfi, Jv)=self._module.slagjac(x, v)
         return (
-            coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n)),
-            coo_matrix((Jv, (Jfi, Ji)), shape=(self.m, self.n))
+            coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n_full)),
+            coo_matrix((Jv, (Jfi, Ji)), shape=(self.m, self.n_full))
         )
 
     def slagjac(self, x, v=None):
         """
         Evaluate sparse gradient of objective or Lagrangian, and sparse Jacobian of constraints.
 
         .. code-block:: python
@@ -754,25 +754,25 @@
         H=__sphess(x, v) -- Hessian of Lagrangian (constrained problems)
 
         Input
         x -- 1D array of length n with the values of variables
         v -- 1D array of length m with the values of Lagrange multipliers
 
         Output
-        H -- a scipy.sparse.coo_matrix of size n-by-n holding the sparse Hessian
+        H -- a scipy.sparse.coo_matrix of size n_full-by-n_full holding the sparse Hessian
             of objective at x or the sparse Hessian of the Lagrangian at (x, v)
 
         This function is a wrapper for sphess().
         """
 
         if v is None:
             (Hi, Hj, Hv)=self._module.sphess(x)
         else:
             (Hi, Hj, Hv)=self._module.sphess(x, v)
-        return coo_matrix((Hv, (Hi, Hj)), shape=(self.n, self.n))
+        return coo_matrix((Hv, (Hi, Hj)), shape=(self.n_full, self.n_full))
 
     def sphess(self, x, v=None):
         """
         Evaluate sparse Hessian of objective or Lagrangian.
         For constrained problems, the Hessian is L_{x,x}(x,v).
 
         .. code-block:: python
@@ -820,25 +820,25 @@
         H=__isphess(x, i) -- Hessian of i-th constraint
 
         Input
         x -- 1D array of length n with the values of variables
         i -- integer holding the index of constraint (between 0 and m-1)
 
         Output
-        H -- a scipy.sparse.coo_matrix of size n-by-n holding the sparse Hessian
+        H -- a scipy.sparse.coo_matrix of size n_full-by-n_full holding the sparse Hessian
             of objective or the sparse Hessian i-th constraint at x
 
         This function is a wrapper for isphess().
         """
 
         if i is None:
             (Hi, Hj, Hv)=self._module.isphess(x)
         else:
             (Hi, Hj, Hv)=self._module.isphess(x, i)
-        return coo_matrix((Hv, (Hi, Hj)), shape=(self.n, self.n))
+        return coo_matrix((Hv, (Hi, Hj)), shape=(self.n_full, self.n_full))
 
     def isphess(self, x, cons_index=None):
         """
         Evaluate the sparse Hessian of the objective or the i-th constraint.
 
         .. code-block:: python
 
@@ -881,33 +881,33 @@
         x     -- 1D array of length n with the values of variables
         v     -- 1D array of length m with the values of Lagrange multipliers
         gradl -- boolean flag. If False the gradient of the objective is returned,
                 if True the gradient of the Lagrangian is returned.
                 Default is False
 
         Output
-        g -- a scipy.sparse.coo_matrix of size 1-by-n holding the gradient of objective at x or
+        g -- a scipy.sparse.coo_matrix of size 1-by-n_full holding the gradient of objective at x or
             the gradient of Lagrangian at (x, v)
-        J -- a scipy.sparse.coo_matrix of size m-by-n holding the sparse Jacobian
+        J -- a scipy.sparse.coo_matrix of size m-by-n_full holding the sparse Jacobian
             of constraints at x
-        H -- a scipy.sparse.coo_matrix of size n-by-n holding the sparse Hessian
+        H -- a scipy.sparse.coo_matrix of size n_full-by-n_full holding the sparse Hessian
             of objective at x or the sparse Hessian of the Lagrangian at (x, v)
 
         This function is a wrapper for gradsphess().
         """
 
         if v is None:
             (g, Hi, Hj, Hv)=self._module.gradsphess(x)
-            return (coo_matrix(g), coo_matrix((Hv, (Hi, Hj)), shape=(self.n, self.n)))
+            return (coo_matrix(g), coo_matrix((Hv, (Hi, Hj)), shape=(self.n_full, self.n_full)))
         else:
             (gi, gv, Ji, Jfi, Jv, Hi, Hj, Hv)=self._module.gradsphess(x, v, lagrFlag)
             return (
-                coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n)),
-                coo_matrix((Jv, (Jfi, Ji)), shape=(self.m, self.n)),
-                coo_matrix((Hv, (Hi, Hj)), shape=(self.n, self.n))
+                coo_matrix((gv, (np.zeros(len(gv)), gi)), shape=(1, self.n_full)),
+                coo_matrix((Jv, (Jfi, Ji)), shape=(self.m, self.n_full)),
+                coo_matrix((Hv, (Hi, Hj)), shape=(self.n_full, self.n_full))
             )
 
     def gradsphess(self, x, v=None, gradient_of_lagrangian=True):
         """
         Evaluate the sparse gradient of objective or Lagrangian, sparse Jacobian of constraints, and sparse Hessian of objective or Lagrangian.
         For constrained problems, the gradient is L_{x}(x,v) and the Hessian is L_{x,x}(x,v).
```

### Comparing `pycutest-1.5.0/pycutest/python_interface.py` & `pycutest-1.5.1/pycutest/python_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/pycutest/sifdecode_extras.py` & `pycutest-1.5.1/pycutest/sifdecode_extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     * ``Q`` .. quadratic objective function
     * ``S`` .. objective function is a sum of squares
     * ``O`` .. none of the above
 
     *C* (single letter) - type of constraints
 
     * ``U`` .. unconstrained
-    * ``X`` .. equality constraints on variables
+    * ``X`` .. fixed variables
     * ``B`` .. bounds on variables
     * ``N`` .. constraints represent the adjacency matrix of a (linear) network
     * ``L`` .. linear constraints
     * ``Q`` .. quadratic constraints
     * ``O`` .. more general than any of the above
 
     *R* (single letter) - problem regularity
@@ -182,15 +182,15 @@
     'objective': {'N' : 'none',
                   'C' : 'constant',
                   'L' : 'linear',
                   'Q' : 'quadratic',
                   'S' : 'sum of squares',
                   'O' : 'other'},
     'constraints': {'U' : 'unconstrained',
-                    'X' : 'equality',
+                    'X' : 'fixed',
                     'B' : 'bound',
                     'N' : 'adjacency',
                     'L' : 'linear',
                     'Q' : 'quadratic',
                     'O' : 'other'},
     'origin': {'A' : 'academic',
                'M' : 'modelling',
@@ -262,15 +262,15 @@
     Problems with a user-settable number of variables/constraints match any given n / m.
 
     Returns the problem names of problems that matched the given requirements.
 
     If a requirement is not given, it is not applied. See below for details on the requirements.
 
     :param objective: a string containing one or more substrings (``'none'``, ``'constant'``, ``'linear'``, ``'quadratic'``, ``'sum of squares'``, ``'other'``) specifying the type of the objective function
-    :param constraints: a string containing one or more substrings (``'unconstrained'``, ``'equality'``, ``'bound'``, ``'adjacency'``, ``'linear'``, ``'quadratic'``, ``'other'``) specifying the type of the constraints
+    :param constraints: a string containing one or more substrings (``'unconstrained'``, ``'fixed'``, ``'bound'``, ``'adjacency'``, ``'linear'``, ``'quadratic'``, ``'other'``) specifying the type of the constraints
     :param regular: a boolean, ``True`` if the problem must be regular, ``False`` if it must be irregular
     :param degree: list of the form ``[min, max]`` specifying the minimum and the maximum number of analytically available derivatives
     :param origin: a string containing one or more substrings (``'academic'``, ``'modelling'``, ``'real-world'``) specifying the origin of the problem
     :param internal: a boolean, ``True`` if the problem must have internal variables, ``False`` if internal variables are not allowed
     :param n: a list of the form ``[min, max]`` specifying the lowest and the highest allowed number of variables
     :param userN: ``True`` if the problems must have user settable number of variables, ``False`` if the number must be hardcoded
     :param m: a list of the form ``[min, max]`` specifying the lowest and the highest allowed number of constraints
```

### Comparing `pycutest-1.5.0/pycutest/system_paths.py` & `pycutest-1.5.1/pycutest/system_paths.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.5.0/pycutest.egg-info/PKG-INFO` & `pycutest-1.5.1/pycutest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycutest
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Python wrapper to the CUTEst optimization test environment
 Home-page: https://github.com/jfowkes/pycutest/
 Author: Jaroslav Fowkes and Lindon Roberts
 Author-email: jaroslav.fowkes@maths.ox.ac.uk
 License: GNU GPL
 Download-URL: https://github.com/jfowkes/pycutest/releases/
 Project-URL: Bug Tracker, https://github.com/jfowkes/pycutest/issues/
```

### Comparing `pycutest-1.5.0/setup.py` & `pycutest-1.5.1/setup.py`

 * *Files identical despite different names*

