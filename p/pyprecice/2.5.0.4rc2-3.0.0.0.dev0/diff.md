# Comparing `tmp/pyprecice-2.5.0.4rc2.tar.gz` & `tmp/pyprecice-3.0.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprecice-2.5.0.4rc2.tar", last modified: Tue Aug  8 18:46:49 2023, max compression
+gzip compressed data, was "pyprecice-3.0.0.0.dev0.tar", last modified: Wed Jun 21 08:35:58 2023, max compression
```

## Comparing `pyprecice-2.5.0.4rc2.tar` & `pyprecice-3.0.0.0.dev0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/cyprecice/
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/cyprecice/SolverInterface.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/cyprecice/cyprecice.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    61686 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/cyprecice/cyprecice.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/precice/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/precice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/precice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/pyprecice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-08-08 18:46:49.000000 pyprecice-2.5.0.4rc2/pyprecice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 18:46:49.000000 pyprecice-2.5.0.4rc2/pyprecice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:46:49.000000 pyprecice-2.5.0.4rc2/pyprecice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:46:49.000000 pyprecice-2.5.0.4rc2/pyprecice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 18:46:49.000000 pyprecice-2.5.0.4rc2/pyprecice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 18:46:49.000000 pyprecice-2.5.0.4rc2/pyprecice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:46:49.785678 pyprecice-2.5.0.4rc2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    30685 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/test/test_bindings_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    86677 2023-08-08 18:46:35.000000 pyprecice-2.5.0.4rc2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/cyprecice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/cyprecice/Participant.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/cyprecice/cyprecice.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    40061 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/cyprecice/cyprecice.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.865335 pyprecice-3.0.0.0.dev0/precice/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/precice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 08:35:58.865335 pyprecice-3.0.0.0.dev0/precice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 08:35:58.865335 pyprecice-3.0.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27225 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/test/test_bindings_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70208 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/versioneer.py
```

### Comparing `pyprecice-2.5.0.4rc2/CHANGELOG.md` & `pyprecice-3.0.0.0.dev0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Changelog of Python language bindings for preCICE
 
 All notable changes to this project will be documented in this file.
 
-## 2.5.0.3
+## 3.0.0.0dev0
 
-* Update from versioneer 0.19 to 0.29.
-* Add `cimport numpy` to avoid a segmentation fault originating from using Cython v3.0.0. https://github.com/precice/python-bindings/issues/182
+* Update to API introduced in preCICE v3.0.0. https://github.com/precice/python-bindings/pull/169 https://github.com/precice/python-bindings/pull/174 https://github.com/precice/python-bindings/pull/179
 
 ## 2.5.0.2
 
 * Add Waveform API introduced in preCICE v2.4.0.
 
 ## 2.5.0.1
```

### Comparing `pyprecice-2.5.0.4rc2/LICENSE.txt` & `pyprecice-3.0.0.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyprecice-2.5.0.4rc2/PKG-INFO` & `pyprecice-3.0.0.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,177 +1,201 @@
 Metadata-Version: 2.1
 Name: pyprecice
-Version: 2.5.0.4rc2
+Version: 3.0.0.0.dev0
 Summary: Python language bindings for the preCICE coupling library
 Home-page: https://github.com/precice/python-bindings
 Author: the preCICE developers
 Author-email: info@precice.org
 License: LGPL-3.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
+# Python language bindings for the C++ library preCICE
 
-Python language bindings for the C++ library preCICE
-----------------------------------------------------
+⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
 This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
 
-# User documentation
+## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
-# Required dependencies
+## Required dependencies
 
 **preCICE**: Refer to [the preCICE documentation](https://precice.org/installation-overview.html) for information on building and installation.
 
 **C++**: A working C++ compiler, e.g., `g++`.
 
 **MPI**: `mpi4py` requires MPI to be installed on your system.
 
-# Installing the package
+## Installing the package
 
 We recommend using pip3 (version 19.0.0 or newer required) for the sake of simplicity. You can check your pip3 version via `pip3 --version`. To update pip3, use the following line:
 
-```
+```bash
 $ pip3 install --user --upgrade pip
 ```
 
-## Using pip3
+### Using pip3
 
-### preCICE system installs
+#### preCICE system installs
 
 For system installs of preCICE, installation works out of the box. There are different ways how pip can be used to install pyprecice. pip will fetch cython and other build-time dependencies, compile the bindings and finally install the package pyprecice.
 
 * (recommended) install [pyprecice from PyPI](https://pypi.org/project/pyprecice/)
 
-  ```
+  ```bash
   $ pip3 install --user pyprecice
   ```
 
 * provide the link to this repository to pip (replace `<branch>` with the branch you want to use, preferably `master` or `develop`)
 
-  ```
+  ```bash
   $ pip3 install --user https://github.com/precice/python-bindings/archive/<branch>.zip
   ```
 
 * if you already cloned this repository, execute the following command from this directory:
 
-  ```
+  ```bash
   $ pip3 install --user .
   ```
+
   *note the dot at the end of the line*
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 If preCICE (the C++ library) was installed in a custom prefix, or only built but not installed at all, you have to extend the following environment variables:
 
-- `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
-- `CPATH` either to the `src` directory or the `$prefix/include`
+* `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
+* `CPATH` either to the `src` directory or the `$prefix/include`
 
 The preCICE documentation provides more informaiton on [linking preCICE](https://precice.org/installation-linking.html).
 
-## Using Spack
+### Using Spack
 
 You can also install the python language bindings for preCICE via Spack by installing the Spack package `py-pyprecice`. Refer to [our installation guide for preCICE via Spack](https://precice.org/installation-spack.html) for getting started with Spack.
 
-## Using setup.py
+### Using setup.py
 
-### preCICE system installs
+#### preCICE system installs
 
 In this directory, execute:
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 see above. Then run
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (explicit include path, library path)
+#### preCICE at custom location (explicit include path, library path)
 
 1. Install cython and other dependencies via pip3
-   ```
+
+   ```bash
    $ pip3 install --user setuptools wheel cython packaging numpy
    ```
+
 2. Open terminal in this folder.
 3. Build the bindings
-   ```
+
+   ```bash
    $ python3 setup.py build_ext --include-dirs=$PRECICE_ROOT/src --library-dirs=$PRECICE_ROOT/build/last
    ```
 
-  **Options:**
-  - `--include-dirs=`, default: `''` 
-    Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
-  
-  **NOTES:**
-  
-  - If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
-  - It is recommended to use preCICE as a shared library here.
+   **Options:**
+   * `--include-dirs=`, default: `''`
+     Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
+
+   **NOTES:**
+
+   * If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
+   * It is recommended to use preCICE as a shared library here.
 
 4. Install the bindings
-   ```
+
+   ```bash
    $ python3 setup.py install --user
    ```
 
-5. Clean-up _optional_
-   ```
+5. Clean-up *optional*
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
-# Test the installation
+## Test the installation
 
 Update `LD_LIBRARY_PATH` such that python can find `precice.so`
 
-```
+```bash
 $ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$PRECICE_ROOT/build/last
 ```
 
 Run the following to test the installation:
 
-```
+```bash
 $ python3 -c "import precice"
 ```
 
-## Unit tests
+### Unit tests
 
-1. Clean-up __mandatory__ (because we must not link against the real `precice.so`, but we use a mocked version)
-   ```
+1. Clean-up **mandatory** (because we must not link against the real `precice.so`, but we use a mocked version)
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
 2. Set `CPLUS_INCLUDE_PATH` (we cannot use `build_ext` and the `--include-dirs` option here)
-   ```
+
+   ```bash
    $ export CPLUS_INCLUDE_PATH=$CPLUS_INCLUDE_PATH:$PRECICE_ROOT/src
    ```
 
 3. Run tests with
-   ```
+
+   ```bash
    $ python3 setup.py test
    ```
 
-# Usage
+## Usage
 
-You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python). 
+You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python).
 
 **Note** The python package that is installed is called `pyprecice`. It provides the python module `precice` that can be use in your code via `import precice`, for example.
 
-# Troubleshooting & miscellaneous
+## Troubleshooting & miscellaneous
 
 ### preCICE is not found
 
 The following error shows up during installation, if preCICE is not found:
 
+```bash
+  /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/Participant.hpp: No such file or directory
+    643 | #include "precice/Participant.hpp"
+        |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
+  ----------------------------------------
+  ERROR: Failed building wheel for pyprecice
+Failed to build pyprecice
+ERROR: Could not build wheels for pyprecice which use PEP 517 and cannot be installed directly
 ```
+
+Or, for preCICE v2:
+
+```bash
   /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/SolverInterface.hpp: No such file or directory
     643 | #include "precice/SolverInterface.hpp"
         |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
   ----------------------------------------
   ERROR: Failed building wheel for pyprecice
@@ -186,31 +210,31 @@
 
 ### Version of Cython is too old
 
 In case the compilation fails with `shared_ptr.pxd not found` messages, check if you use the latest version of Cython.
 
 ### `Python.h` missing
 
-```
+```bash
 $ python3 -m pip install pyprecice
 Collecting pyprecice
 ...
   /tmp/pip-build-7rj4_h93/pyprecice/precice.cpp:25:20: fatal error: Python.h: No such file or directory
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
 
   ----------------------------------------
-  Failed building wheel for pyprecice 
+  Failed building wheel for pyprecice
 ```
 
 Please try to install `python3-dev`. E.g. via `apt install python3-dev`. Please make sure that you use the correct version (e.g. `python3.5-dev` or `python3.6-dev`). You can check your version via `python3 --version`.
 
 ### `libprecice.so` is not found at runtime
 
-```
+```bash
 $ python3 -c "import precice"
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
 ImportError: libprecice.so.2: cannot open shared object file: No such file or directory
 ```
 
 Make sure that your `LD_LIBRARY_PATH` includes the directory that contains `libprecice.so`. The actual path depends on how you installed preCICE. Example: If preCICE was installed using `sudo make install` and you did not define a `CMAKE_INSTALL_PREFIX` the library path is `/usr/local/lib`. This means you have to `export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH`.
@@ -224,81 +248,94 @@
 *Note that the instructions in this section are outdated and refer to the deprecated python bindings. Until we have updated information on the installation procedure for the python bindings under this use-case, we will keep these instructions, since they might still be very useful* (Originally contributed by [huangq1234553](https://github.com/huangq1234553) to the precice wiki in [`precice/precice/wiki:8bb74b7`](https://github.com/precice/precice/wiki/Dependencies/8bb74b78a7ebc54983f4822af82fb3d638021faa).)
 
 <details><summary>show details</summary>
 
 This guide provides steps to install python bindings for precice-1.6.1 for a conda environment Python 2.7.17 on the CoolMUC. Note that preCICE no longer supports Python 2 after v1.4.0. Hence, some modifications to the python setup code was necessary. Most steps are similar if not identical to the basic guide without petsc or python above. This guide assumes that the Eigen dependencies have already been installed.
 
 Load the prerequisite libraries:
-```
+
+```bash
 module load gcc/7
 module unload mpi.intel
 module load mpi.intel/2018_gcc
 module load cmake/3.12.1
 ```
+
 At the time of this writing `module load boost/1.68.0` is no longer available. Instead
-boost 1.65.1 was installed per the `boost and yaml-cpp` guide above. 
+boost 1.65.1 was installed per the `boost and yaml-cpp` guide above.
 
 In order to have the right python dependencies, a packaged conda environment was transferred to
 SuperMUC. The following dependencies were installed:
-- numpy
-- mpi4py
+
+* numpy
+* mpi4py
 
 With the python environment active, we have to feed the right python file directories to the cmake command.
 Note that -DPYTHON_LIBRARY expects a python shared library. You can likely modify the version to fit what is required.
-```
+
+```bash
 mkdir build && cd build
 cmake -DBUILD_SHARED_LIBS=ON -DPRECICE_PETScMapping=OFF -DPRECICE_PythonActions=ON -DCMAKE_INSTALL_PREFIX=/path/to/precice -DCMAKE_BUILD_TYPE=Debug .. -DPYTHON_INCLUDE_DIR=$(python -c "from distutils.sysconfig import get_python_inc; print(get_python_inc())")  -DPYTHON_LIBRARY=$(python -c "import distutils.sysconfig as sysconfig; print(sysconfig.get_config_var('LIBDIR')+'/libpython2.7.so')") -DNumPy_INCLUDE_DIR=$(python -c "import numpy; print(numpy.get_include())")
 make -j 12
 make install
 ```
+
 After installing, make sure you add the preCICE installation paths to your `.bashrc`, so that other programs can find it:
-```
+
+```bash
 export PRECICE_ROOT="path/to/precice_install"
 export PKG_CONFIG_PATH="path/to/precice_install/lib/pkgconfig:${PKG_CONFIG_PATH}"
 export CPLUS_INCLUDE_PATH="path/to/precice_install/include:${CPLUS_INCLUDE_PATH}"
 export LD_LIBRARY_PATH="path/to/precice_install/lib:${LD_LIBRARY_PATH}"
 ```
+
 Then, navigate to the python_future bindings script.
-```
+
+```bash
 cd /path/to/precice/src/precice/bindings/python_future
 ```
+
 Append the following to the head of the file to allow Python2 to run Python3 code. Note that
-importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals 
+importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals
 in code are interpreted as `unicode` with this import.
-```
+
+```python
 from __future__ import (absolute_import, division,
                         print_function)
 from builtins import (
          bytes, dict, int, list, object, range, str,
          ascii, chr, hex, input, next, oct, open,
          pow, round, super,
          filter, map, zip)
 ```
+
 Modify `mpicompiler_default = "mpic++"` to `mpicompiler_default = "mpicxx"` in line 100.
 Run the setup file using the default Python 2.7.17.
-```
+
+```bash
 python setup.py install --user
 ```
+
 </details>
 
 ### ValueError while importing preCICE
+
 If you face the error:
 
 ```bash
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
-
-# Contributors
+## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
 * [Benjamin Uekermann](https://github.com/uekerman)
```

### Comparing `pyprecice-2.5.0.4rc2/README.md` & `pyprecice-3.0.0.0.dev0/pyprecice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,165 +1,201 @@
-⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
+Metadata-Version: 2.1
+Name: pyprecice
+Version: 3.0.0.0.dev0
+Summary: Python language bindings for the preCICE coupling library
+Home-page: https://github.com/precice/python-bindings
+Author: the preCICE developers
+Author-email: info@precice.org
+License: LGPL-3.0
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Python language bindings for the C++ library preCICE
 
-Python language bindings for the C++ library preCICE
-----------------------------------------------------
+⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
 This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
 
-# User documentation
+## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
-# Required dependencies
+## Required dependencies
 
 **preCICE**: Refer to [the preCICE documentation](https://precice.org/installation-overview.html) for information on building and installation.
 
 **C++**: A working C++ compiler, e.g., `g++`.
 
 **MPI**: `mpi4py` requires MPI to be installed on your system.
 
-# Installing the package
+## Installing the package
 
 We recommend using pip3 (version 19.0.0 or newer required) for the sake of simplicity. You can check your pip3 version via `pip3 --version`. To update pip3, use the following line:
 
-```
+```bash
 $ pip3 install --user --upgrade pip
 ```
 
-## Using pip3
+### Using pip3
 
-### preCICE system installs
+#### preCICE system installs
 
 For system installs of preCICE, installation works out of the box. There are different ways how pip can be used to install pyprecice. pip will fetch cython and other build-time dependencies, compile the bindings and finally install the package pyprecice.
 
 * (recommended) install [pyprecice from PyPI](https://pypi.org/project/pyprecice/)
 
-  ```
+  ```bash
   $ pip3 install --user pyprecice
   ```
 
 * provide the link to this repository to pip (replace `<branch>` with the branch you want to use, preferably `master` or `develop`)
 
-  ```
+  ```bash
   $ pip3 install --user https://github.com/precice/python-bindings/archive/<branch>.zip
   ```
 
 * if you already cloned this repository, execute the following command from this directory:
 
-  ```
+  ```bash
   $ pip3 install --user .
   ```
+
   *note the dot at the end of the line*
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 If preCICE (the C++ library) was installed in a custom prefix, or only built but not installed at all, you have to extend the following environment variables:
 
-- `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
-- `CPATH` either to the `src` directory or the `$prefix/include`
+* `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
+* `CPATH` either to the `src` directory or the `$prefix/include`
 
 The preCICE documentation provides more informaiton on [linking preCICE](https://precice.org/installation-linking.html).
 
-## Using Spack
+### Using Spack
 
 You can also install the python language bindings for preCICE via Spack by installing the Spack package `py-pyprecice`. Refer to [our installation guide for preCICE via Spack](https://precice.org/installation-spack.html) for getting started with Spack.
 
-## Using setup.py
+### Using setup.py
 
-### preCICE system installs
+#### preCICE system installs
 
 In this directory, execute:
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 see above. Then run
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (explicit include path, library path)
+#### preCICE at custom location (explicit include path, library path)
 
 1. Install cython and other dependencies via pip3
-   ```
+
+   ```bash
    $ pip3 install --user setuptools wheel cython packaging numpy
    ```
+
 2. Open terminal in this folder.
 3. Build the bindings
-   ```
+
+   ```bash
    $ python3 setup.py build_ext --include-dirs=$PRECICE_ROOT/src --library-dirs=$PRECICE_ROOT/build/last
    ```
 
-  **Options:**
-  - `--include-dirs=`, default: `''` 
-    Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
-  
-  **NOTES:**
-  
-  - If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
-  - It is recommended to use preCICE as a shared library here.
+   **Options:**
+   * `--include-dirs=`, default: `''`
+     Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
+
+   **NOTES:**
+
+   * If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
+   * It is recommended to use preCICE as a shared library here.
 
 4. Install the bindings
-   ```
+
+   ```bash
    $ python3 setup.py install --user
    ```
 
-5. Clean-up _optional_
-   ```
+5. Clean-up *optional*
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
-# Test the installation
+## Test the installation
 
 Update `LD_LIBRARY_PATH` such that python can find `precice.so`
 
-```
+```bash
 $ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$PRECICE_ROOT/build/last
 ```
 
 Run the following to test the installation:
 
-```
+```bash
 $ python3 -c "import precice"
 ```
 
-## Unit tests
+### Unit tests
 
-1. Clean-up __mandatory__ (because we must not link against the real `precice.so`, but we use a mocked version)
-   ```
+1. Clean-up **mandatory** (because we must not link against the real `precice.so`, but we use a mocked version)
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
 2. Set `CPLUS_INCLUDE_PATH` (we cannot use `build_ext` and the `--include-dirs` option here)
-   ```
+
+   ```bash
    $ export CPLUS_INCLUDE_PATH=$CPLUS_INCLUDE_PATH:$PRECICE_ROOT/src
    ```
 
 3. Run tests with
-   ```
+
+   ```bash
    $ python3 setup.py test
    ```
 
-# Usage
+## Usage
 
-You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python). 
+You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python).
 
 **Note** The python package that is installed is called `pyprecice`. It provides the python module `precice` that can be use in your code via `import precice`, for example.
 
-# Troubleshooting & miscellaneous
+## Troubleshooting & miscellaneous
 
 ### preCICE is not found
 
 The following error shows up during installation, if preCICE is not found:
 
+```bash
+  /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/Participant.hpp: No such file or directory
+    643 | #include "precice/Participant.hpp"
+        |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
+  ----------------------------------------
+  ERROR: Failed building wheel for pyprecice
+Failed to build pyprecice
+ERROR: Could not build wheels for pyprecice which use PEP 517 and cannot be installed directly
 ```
+
+Or, for preCICE v2:
+
+```bash
   /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/SolverInterface.hpp: No such file or directory
     643 | #include "precice/SolverInterface.hpp"
         |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
   ----------------------------------------
   ERROR: Failed building wheel for pyprecice
@@ -174,31 +210,31 @@
 
 ### Version of Cython is too old
 
 In case the compilation fails with `shared_ptr.pxd not found` messages, check if you use the latest version of Cython.
 
 ### `Python.h` missing
 
-```
+```bash
 $ python3 -m pip install pyprecice
 Collecting pyprecice
 ...
   /tmp/pip-build-7rj4_h93/pyprecice/precice.cpp:25:20: fatal error: Python.h: No such file or directory
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
 
   ----------------------------------------
-  Failed building wheel for pyprecice 
+  Failed building wheel for pyprecice
 ```
 
 Please try to install `python3-dev`. E.g. via `apt install python3-dev`. Please make sure that you use the correct version (e.g. `python3.5-dev` or `python3.6-dev`). You can check your version via `python3 --version`.
 
 ### `libprecice.so` is not found at runtime
 
-```
+```bash
 $ python3 -c "import precice"
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
 ImportError: libprecice.so.2: cannot open shared object file: No such file or directory
 ```
 
 Make sure that your `LD_LIBRARY_PATH` includes the directory that contains `libprecice.so`. The actual path depends on how you installed preCICE. Example: If preCICE was installed using `sudo make install` and you did not define a `CMAKE_INSTALL_PREFIX` the library path is `/usr/local/lib`. This means you have to `export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH`.
@@ -212,81 +248,94 @@
 *Note that the instructions in this section are outdated and refer to the deprecated python bindings. Until we have updated information on the installation procedure for the python bindings under this use-case, we will keep these instructions, since they might still be very useful* (Originally contributed by [huangq1234553](https://github.com/huangq1234553) to the precice wiki in [`precice/precice/wiki:8bb74b7`](https://github.com/precice/precice/wiki/Dependencies/8bb74b78a7ebc54983f4822af82fb3d638021faa).)
 
 <details><summary>show details</summary>
 
 This guide provides steps to install python bindings for precice-1.6.1 for a conda environment Python 2.7.17 on the CoolMUC. Note that preCICE no longer supports Python 2 after v1.4.0. Hence, some modifications to the python setup code was necessary. Most steps are similar if not identical to the basic guide without petsc or python above. This guide assumes that the Eigen dependencies have already been installed.
 
 Load the prerequisite libraries:
-```
+
+```bash
 module load gcc/7
 module unload mpi.intel
 module load mpi.intel/2018_gcc
 module load cmake/3.12.1
 ```
+
 At the time of this writing `module load boost/1.68.0` is no longer available. Instead
-boost 1.65.1 was installed per the `boost and yaml-cpp` guide above. 
+boost 1.65.1 was installed per the `boost and yaml-cpp` guide above.
 
 In order to have the right python dependencies, a packaged conda environment was transferred to
 SuperMUC. The following dependencies were installed:
-- numpy
-- mpi4py
+
+* numpy
+* mpi4py
 
 With the python environment active, we have to feed the right python file directories to the cmake command.
 Note that -DPYTHON_LIBRARY expects a python shared library. You can likely modify the version to fit what is required.
-```
+
+```bash
 mkdir build && cd build
 cmake -DBUILD_SHARED_LIBS=ON -DPRECICE_PETScMapping=OFF -DPRECICE_PythonActions=ON -DCMAKE_INSTALL_PREFIX=/path/to/precice -DCMAKE_BUILD_TYPE=Debug .. -DPYTHON_INCLUDE_DIR=$(python -c "from distutils.sysconfig import get_python_inc; print(get_python_inc())")  -DPYTHON_LIBRARY=$(python -c "import distutils.sysconfig as sysconfig; print(sysconfig.get_config_var('LIBDIR')+'/libpython2.7.so')") -DNumPy_INCLUDE_DIR=$(python -c "import numpy; print(numpy.get_include())")
 make -j 12
 make install
 ```
+
 After installing, make sure you add the preCICE installation paths to your `.bashrc`, so that other programs can find it:
-```
+
+```bash
 export PRECICE_ROOT="path/to/precice_install"
 export PKG_CONFIG_PATH="path/to/precice_install/lib/pkgconfig:${PKG_CONFIG_PATH}"
 export CPLUS_INCLUDE_PATH="path/to/precice_install/include:${CPLUS_INCLUDE_PATH}"
 export LD_LIBRARY_PATH="path/to/precice_install/lib:${LD_LIBRARY_PATH}"
 ```
+
 Then, navigate to the python_future bindings script.
-```
+
+```bash
 cd /path/to/precice/src/precice/bindings/python_future
 ```
+
 Append the following to the head of the file to allow Python2 to run Python3 code. Note that
-importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals 
+importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals
 in code are interpreted as `unicode` with this import.
-```
+
+```python
 from __future__ import (absolute_import, division,
                         print_function)
 from builtins import (
          bytes, dict, int, list, object, range, str,
          ascii, chr, hex, input, next, oct, open,
          pow, round, super,
          filter, map, zip)
 ```
+
 Modify `mpicompiler_default = "mpic++"` to `mpicompiler_default = "mpicxx"` in line 100.
 Run the setup file using the default Python 2.7.17.
-```
+
+```bash
 python setup.py install --user
 ```
+
 </details>
 
 ### ValueError while importing preCICE
+
 If you face the error:
 
 ```bash
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
-
-# Contributors
+## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
 * [Benjamin Uekermann](https://github.com/uekerman)
```

### Comparing `pyprecice-2.5.0.4rc2/pyprecice.egg-info/PKG-INFO` & `pyprecice-3.0.0.0.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,177 +1,189 @@
-Metadata-Version: 2.1
-Name: pyprecice
-Version: 2.5.0.4rc2
-Summary: Python language bindings for the preCICE coupling library
-Home-page: https://github.com/precice/python-bindings
-Author: the preCICE developers
-Author-email: info@precice.org
-License: LGPL-3.0
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# Python language bindings for the C++ library preCICE
 
 ⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
-Python language bindings for the C++ library preCICE
-----------------------------------------------------
-
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
 This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
 
-# User documentation
+## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
-# Required dependencies
+## Required dependencies
 
 **preCICE**: Refer to [the preCICE documentation](https://precice.org/installation-overview.html) for information on building and installation.
 
 **C++**: A working C++ compiler, e.g., `g++`.
 
 **MPI**: `mpi4py` requires MPI to be installed on your system.
 
-# Installing the package
+## Installing the package
 
 We recommend using pip3 (version 19.0.0 or newer required) for the sake of simplicity. You can check your pip3 version via `pip3 --version`. To update pip3, use the following line:
 
-```
+```bash
 $ pip3 install --user --upgrade pip
 ```
 
-## Using pip3
+### Using pip3
 
-### preCICE system installs
+#### preCICE system installs
 
 For system installs of preCICE, installation works out of the box. There are different ways how pip can be used to install pyprecice. pip will fetch cython and other build-time dependencies, compile the bindings and finally install the package pyprecice.
 
 * (recommended) install [pyprecice from PyPI](https://pypi.org/project/pyprecice/)
 
-  ```
+  ```bash
   $ pip3 install --user pyprecice
   ```
 
 * provide the link to this repository to pip (replace `<branch>` with the branch you want to use, preferably `master` or `develop`)
 
-  ```
+  ```bash
   $ pip3 install --user https://github.com/precice/python-bindings/archive/<branch>.zip
   ```
 
 * if you already cloned this repository, execute the following command from this directory:
 
-  ```
+  ```bash
   $ pip3 install --user .
   ```
+
   *note the dot at the end of the line*
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 If preCICE (the C++ library) was installed in a custom prefix, or only built but not installed at all, you have to extend the following environment variables:
 
-- `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
-- `CPATH` either to the `src` directory or the `$prefix/include`
+* `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
+* `CPATH` either to the `src` directory or the `$prefix/include`
 
 The preCICE documentation provides more informaiton on [linking preCICE](https://precice.org/installation-linking.html).
 
-## Using Spack
+### Using Spack
 
 You can also install the python language bindings for preCICE via Spack by installing the Spack package `py-pyprecice`. Refer to [our installation guide for preCICE via Spack](https://precice.org/installation-spack.html) for getting started with Spack.
 
-## Using setup.py
+### Using setup.py
 
-### preCICE system installs
+#### preCICE system installs
 
 In this directory, execute:
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 see above. Then run
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (explicit include path, library path)
+#### preCICE at custom location (explicit include path, library path)
 
 1. Install cython and other dependencies via pip3
-   ```
+
+   ```bash
    $ pip3 install --user setuptools wheel cython packaging numpy
    ```
+
 2. Open terminal in this folder.
 3. Build the bindings
-   ```
+
+   ```bash
    $ python3 setup.py build_ext --include-dirs=$PRECICE_ROOT/src --library-dirs=$PRECICE_ROOT/build/last
    ```
 
-  **Options:**
-  - `--include-dirs=`, default: `''` 
-    Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
-  
-  **NOTES:**
-  
-  - If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
-  - It is recommended to use preCICE as a shared library here.
+   **Options:**
+   * `--include-dirs=`, default: `''`
+     Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
+
+   **NOTES:**
+
+   * If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
+   * It is recommended to use preCICE as a shared library here.
 
 4. Install the bindings
-   ```
+
+   ```bash
    $ python3 setup.py install --user
    ```
 
-5. Clean-up _optional_
-   ```
+5. Clean-up *optional*
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
-# Test the installation
+## Test the installation
 
 Update `LD_LIBRARY_PATH` such that python can find `precice.so`
 
-```
+```bash
 $ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$PRECICE_ROOT/build/last
 ```
 
 Run the following to test the installation:
 
-```
+```bash
 $ python3 -c "import precice"
 ```
 
-## Unit tests
+### Unit tests
 
-1. Clean-up __mandatory__ (because we must not link against the real `precice.so`, but we use a mocked version)
-   ```
+1. Clean-up **mandatory** (because we must not link against the real `precice.so`, but we use a mocked version)
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
 2. Set `CPLUS_INCLUDE_PATH` (we cannot use `build_ext` and the `--include-dirs` option here)
-   ```
+
+   ```bash
    $ export CPLUS_INCLUDE_PATH=$CPLUS_INCLUDE_PATH:$PRECICE_ROOT/src
    ```
 
 3. Run tests with
-   ```
+
+   ```bash
    $ python3 setup.py test
    ```
 
-# Usage
+## Usage
 
-You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python). 
+You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python).
 
 **Note** The python package that is installed is called `pyprecice`. It provides the python module `precice` that can be use in your code via `import precice`, for example.
 
-# Troubleshooting & miscellaneous
+## Troubleshooting & miscellaneous
 
 ### preCICE is not found
 
 The following error shows up during installation, if preCICE is not found:
 
+```bash
+  /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/Participant.hpp: No such file or directory
+    643 | #include "precice/Participant.hpp"
+        |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
+  ----------------------------------------
+  ERROR: Failed building wheel for pyprecice
+Failed to build pyprecice
+ERROR: Could not build wheels for pyprecice which use PEP 517 and cannot be installed directly
 ```
+
+Or, for preCICE v2:
+
+```bash
   /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/SolverInterface.hpp: No such file or directory
     643 | #include "precice/SolverInterface.hpp"
         |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
   ----------------------------------------
   ERROR: Failed building wheel for pyprecice
@@ -186,31 +198,31 @@
 
 ### Version of Cython is too old
 
 In case the compilation fails with `shared_ptr.pxd not found` messages, check if you use the latest version of Cython.
 
 ### `Python.h` missing
 
-```
+```bash
 $ python3 -m pip install pyprecice
 Collecting pyprecice
 ...
   /tmp/pip-build-7rj4_h93/pyprecice/precice.cpp:25:20: fatal error: Python.h: No such file or directory
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
 
   ----------------------------------------
-  Failed building wheel for pyprecice 
+  Failed building wheel for pyprecice
 ```
 
 Please try to install `python3-dev`. E.g. via `apt install python3-dev`. Please make sure that you use the correct version (e.g. `python3.5-dev` or `python3.6-dev`). You can check your version via `python3 --version`.
 
 ### `libprecice.so` is not found at runtime
 
-```
+```bash
 $ python3 -c "import precice"
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
 ImportError: libprecice.so.2: cannot open shared object file: No such file or directory
 ```
 
 Make sure that your `LD_LIBRARY_PATH` includes the directory that contains `libprecice.so`. The actual path depends on how you installed preCICE. Example: If preCICE was installed using `sudo make install` and you did not define a `CMAKE_INSTALL_PREFIX` the library path is `/usr/local/lib`. This means you have to `export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH`.
@@ -224,81 +236,94 @@
 *Note that the instructions in this section are outdated and refer to the deprecated python bindings. Until we have updated information on the installation procedure for the python bindings under this use-case, we will keep these instructions, since they might still be very useful* (Originally contributed by [huangq1234553](https://github.com/huangq1234553) to the precice wiki in [`precice/precice/wiki:8bb74b7`](https://github.com/precice/precice/wiki/Dependencies/8bb74b78a7ebc54983f4822af82fb3d638021faa).)
 
 <details><summary>show details</summary>
 
 This guide provides steps to install python bindings for precice-1.6.1 for a conda environment Python 2.7.17 on the CoolMUC. Note that preCICE no longer supports Python 2 after v1.4.0. Hence, some modifications to the python setup code was necessary. Most steps are similar if not identical to the basic guide without petsc or python above. This guide assumes that the Eigen dependencies have already been installed.
 
 Load the prerequisite libraries:
-```
+
+```bash
 module load gcc/7
 module unload mpi.intel
 module load mpi.intel/2018_gcc
 module load cmake/3.12.1
 ```
+
 At the time of this writing `module load boost/1.68.0` is no longer available. Instead
-boost 1.65.1 was installed per the `boost and yaml-cpp` guide above. 
+boost 1.65.1 was installed per the `boost and yaml-cpp` guide above.
 
 In order to have the right python dependencies, a packaged conda environment was transferred to
 SuperMUC. The following dependencies were installed:
-- numpy
-- mpi4py
+
+* numpy
+* mpi4py
 
 With the python environment active, we have to feed the right python file directories to the cmake command.
 Note that -DPYTHON_LIBRARY expects a python shared library. You can likely modify the version to fit what is required.
-```
+
+```bash
 mkdir build && cd build
 cmake -DBUILD_SHARED_LIBS=ON -DPRECICE_PETScMapping=OFF -DPRECICE_PythonActions=ON -DCMAKE_INSTALL_PREFIX=/path/to/precice -DCMAKE_BUILD_TYPE=Debug .. -DPYTHON_INCLUDE_DIR=$(python -c "from distutils.sysconfig import get_python_inc; print(get_python_inc())")  -DPYTHON_LIBRARY=$(python -c "import distutils.sysconfig as sysconfig; print(sysconfig.get_config_var('LIBDIR')+'/libpython2.7.so')") -DNumPy_INCLUDE_DIR=$(python -c "import numpy; print(numpy.get_include())")
 make -j 12
 make install
 ```
+
 After installing, make sure you add the preCICE installation paths to your `.bashrc`, so that other programs can find it:
-```
+
+```bash
 export PRECICE_ROOT="path/to/precice_install"
 export PKG_CONFIG_PATH="path/to/precice_install/lib/pkgconfig:${PKG_CONFIG_PATH}"
 export CPLUS_INCLUDE_PATH="path/to/precice_install/include:${CPLUS_INCLUDE_PATH}"
 export LD_LIBRARY_PATH="path/to/precice_install/lib:${LD_LIBRARY_PATH}"
 ```
+
 Then, navigate to the python_future bindings script.
-```
+
+```bash
 cd /path/to/precice/src/precice/bindings/python_future
 ```
+
 Append the following to the head of the file to allow Python2 to run Python3 code. Note that
-importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals 
+importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals
 in code are interpreted as `unicode` with this import.
-```
+
+```python
 from __future__ import (absolute_import, division,
                         print_function)
 from builtins import (
          bytes, dict, int, list, object, range, str,
          ascii, chr, hex, input, next, oct, open,
          pow, round, super,
          filter, map, zip)
 ```
+
 Modify `mpicompiler_default = "mpic++"` to `mpicompiler_default = "mpicxx"` in line 100.
 Run the setup file using the default Python 2.7.17.
-```
+
+```bash
 python setup.py install --user
 ```
+
 </details>
 
 ### ValueError while importing preCICE
+
 If you face the error:
 
 ```bash
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
-
-# Contributors
+## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
 * [Benjamin Uekermann](https://github.com/uekerman)
```

### Comparing `pyprecice-2.5.0.4rc2/setup.py` & `pyprecice-3.0.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,27 @@
 
 PYTHON_BINDINGS_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_extensions(is_test):
     compile_args = []
     link_args = []
-    compile_args.append("-std=c++11")
+    compile_args.append("-std=c++17")
     compile_args.append("-I{}".format(numpy.get_include()))
 
     bindings_sources = [os.path.join(PYTHON_BINDINGS_PATH, "cyprecice",
                                      "cyprecice" + ".pyx")]
 
     compile_args += pkgconfig.cflags('libprecice').split()
 
     if not is_test:
         link_args += pkgconfig.libs('libprecice').split()
     if is_test:
         bindings_sources.append(os.path.join(PYTHON_BINDINGS_PATH, "test",
-                                             "SolverInterface.cpp"))
+                                             "Participant.cpp"))
 
     return [
         Extension(
             "cyprecice",
             sources=bindings_sources,
             libraries=[],
             language="c++",
```

### Comparing `pyprecice-2.5.0.4rc2/versioneer.py` & `pyprecice-3.0.0.0.dev0/versioneer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,36 @@
 
-# Version: 0.29
+# Version: 0.19
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain (Unlicense)
-* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
+* License: Public Domain
+* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in setuptools-based
+This is a tool for managing a recorded version number in distutils-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-Versioneer provides two installation modes. The "classic" vendored mode installs
-a copy of versioneer into your repository. The experimental build-time dependency mode
-is intended to allow you to skip this step and simplify the process of upgrading.
-
-### Vendored mode
-
-* `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-   * Note that you will need to add `tomli; python_version < "3.11"` to your
-     build-time dependencies if you use `pyproject.toml`
-* run `versioneer install --vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
-
-### Build-time dependency mode
-
 * `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
-  to the `requires` key of the `build-system` table in `pyproject.toml`:
-  ```toml
-  [build-system]
-  requires = ["setuptools", "versioneer[toml]"]
-  build-backend = "setuptools.build_meta"
-  ```
-* run `versioneer install --no-vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
+* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
+* run `versioneer install` in your source tree, commit the results
+* Verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -255,18 +227,17 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg` and `pyproject.toml`, if necessary,
-  to include any new configuration settings indicated by the release notes.
-  See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install --[no-]vendor` in your source tree, to replace
+* edit `setup.cfg`, if necessary, to include any new configuration settings
+  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -281,257 +252,187 @@
 
 ## Similar projects
 
 * [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
   dependency
 * [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
   versioneer
-* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
-  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the "Unlicense", as described in
-https://unlicense.org/.
+Specifically, both are released under the Creative Commons "Public Domain
+Dedication" license (CC0-1.0), as described in
+https://creativecommons.org/publicdomain/zero/1.0/ .
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
-# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
-# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
-# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
-# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
-# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
-from pathlib import Path
-from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
-from typing import NoReturn
-import functools
-
-have_tomllib = True
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    try:
-        import tomli as tomllib
-    except ImportError:
-        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
-    VCS: str
-    style: str
-    tag_prefix: str
-    versionfile_source: str
-    versionfile_build: Optional[str]
-    parentdir_prefix: Optional[str]
-    verbose: Optional[bool]
 
-
-def get_root() -> str:
+def get_root():
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
-    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (
-        os.path.exists(setup_py)
-        or os.path.exists(pyproject_toml)
-        or os.path.exists(versioneer_py)
-    ):
+    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
-        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (
-        os.path.exists(setup_py)
-        or os.path.exists(pyproject_toml)
-        or os.path.exists(versioneer_py)
-    ):
+    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         err = ("Versioneer was unable to run the project root directory. "
                "Versioneer requires setup.py to be executed from "
                "its immediate directory (like 'python setup.py COMMAND'), "
                "or in a way that lets it use sys.argv[0] to find the root "
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        my_path = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
+        me = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
+        if me_dir != vsr_dir:
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+                  % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root: str) -> VersioneerConfig:
+def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise OSError (if setup.cfg is missing), or
+    # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    root_pth = Path(root)
-    pyproject_toml = root_pth / "pyproject.toml"
-    setup_cfg = root_pth / "setup.cfg"
-    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
-    if pyproject_toml.exists() and have_tomllib:
-        try:
-            with open(pyproject_toml, 'rb') as fobj:
-                pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
-        except (tomllib.TOMLDecodeError, KeyError) as e:
-            print(f"Failed to load config from {pyproject_toml}: {e}")
-            print("Try to load it from setup.cfg")
-    if not section:
-        parser = configparser.ConfigParser()
-        with open(setup_cfg) as cfg_file:
-            parser.read_file(cfg_file)
-        parser.get("versioneer", "VCS")  # raise error if missing
-
-        section = parser["versioneer"]
-
-    # `cast`` really shouldn't be used, but its simplest for the
-    # common VersioneerConfig users at the moment. We verify against
-    # `None` values elsewhere where it matters
-
+    setup_cfg = os.path.join(root, "setup.cfg")
+    parser = configparser.ConfigParser()
+    with open(setup_cfg, "r") as f:
+        parser.read_file(f)
+    VCS = parser.get("versioneer", "VCS")  # mandatory
+
+    def get(parser, name):
+        if parser.has_option("versioneer", name):
+            return parser.get("versioneer", name)
+        return None
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
-    cfg.style = section.get("style", "")
-    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
-    cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
-    if cfg.tag_prefix in ("''", '""', None):
+    cfg.VCS = VCS
+    cfg.style = get(parser, "style") or ""
+    cfg.versionfile_source = get(parser, "versionfile_source")
+    cfg.versionfile_build = get(parser, "versionfile_build")
+    cfg.tag_prefix = get(parser, "tag_prefix")
+    if cfg.tag_prefix in ("''", '""'):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = section.get("parentdir_prefix")
-    if isinstance(section, configparser.SectionProxy):
-        # Make sure configparser translates to bool
-        cfg.verbose = section.getboolean("verbose")
-    else:
-        cfg.verbose = section.get("verbose")
-
+    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
+    cfg.verbose = get(parser, "verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
+LONG_VERSION_PY = {}
+HANDLERS = {}
 
 
-def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f: Callable) -> Callable:
+    def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        HANDLERS.setdefault(vcs, {})[method] = f
+        if vcs not in HANDLERS:
+            HANDLERS[vcs] = {}
+        HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(
-    commands: List[str],
-    args: List[str],
-    cwd: Optional[str] = None,
-    verbose: bool = False,
-    hide_stderr: bool = False,
-    env: Optional[Dict[str, str]] = None,
-) -> Tuple[Optional[str], Optional[int]]:
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    process = None
-
-    popen_kwargs: Dict[str, Any] = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
-    for command in commands:
+    p = None
+    for c in commands:
         try:
-            dispcmd = str([command] + args)
+            dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
-        except OSError as e:
+        except EnvironmentError:
+            e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = process.communicate()[0].strip().decode()
-    if process.returncode != 0:
+    stdout = p.communicate()[0].strip().decode()
+    if p.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, process.returncode
-    return stdout, process.returncode
+        return None, p.returncode
+    return stdout, p.returncode
 
 
 LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain.
-# Generated by versioneer-0.29
-# https://github.com/python-versioneer/python-versioneer
+# This file is released into the public domain. Generated by
+# versioneer-0.19 (https://github.com/python-versioneer/python-versioneer)
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
-from typing import Any, Callable, Dict, List, Optional, Tuple
-import functools
 
 
-def get_keywords() -> Dict[str, str]:
+def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -539,23 +440,16 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
-    VCS: str
-    style: str
-    tag_prefix: str
-    parentdir_prefix: str
-    versionfile_source: str
-    verbose: bool
-
 
-def get_config() -> VersioneerConfig:
+def get_config():
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -565,142 +459,123 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
+LONG_VERSION_PY = {}
+HANDLERS = {}
 
 
-def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f: Callable) -> Callable:
+    def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(
-    commands: List[str],
-    args: List[str],
-    cwd: Optional[str] = None,
-    verbose: bool = False,
-    hide_stderr: bool = False,
-    env: Optional[Dict[str, str]] = None,
-) -> Tuple[Optional[str], Optional[int]]:
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    process = None
-
-    popen_kwargs: Dict[str, Any] = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
-    for command in commands:
+    p = None
+    for c in commands:
         try:
-            dispcmd = str([command] + args)
+            dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
-        except OSError as e:
+        except EnvironmentError:
+            e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = process.communicate()[0].strip().decode()
-    if process.returncode != 0:
+    stdout = p.communicate()[0].strip().decode()
+    if p.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, process.returncode
-    return stdout, process.returncode
+        return None, p.returncode
+    return stdout, p.returncode
 
 
-def versions_from_parentdir(
-    parentdir_prefix: str,
-    root: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for _ in range(3):
+    for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        rootdirs.append(root)
-        root = os.path.dirname(root)  # up a level
+        else:
+            rootdirs.append(root)
+            root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
+def git_get_keywords(versionfile_abs):
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords: Dict[str, str] = {}
+    keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith("git_refnames ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["date"] = mo.group(1)
-    except OSError:
+        f = open(versionfile_abs, "r")
+        for line in f.readlines():
+            if line.strip().startswith("git_refnames ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["refnames"] = mo.group(1)
+            if line.strip().startswith("git_full ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["full"] = mo.group(1)
+            if line.strip().startswith("git_date ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["date"] = mo.group(1)
+        f.close()
+    except EnvironmentError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(
-    keywords: Dict[str, str],
-    tag_prefix: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
+    if not keywords:
+        raise NotThisMethod("no keywords at all, weird")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
         date = date.splitlines()[-1]
 
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
@@ -711,41 +586,36 @@
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
-            # Filter out refs that exactly match prefix or that don't start
-            # with a number once the prefix is stripped (mostly a concern
-            # when prefix is '')
-            if not re.match(r'\d', r):
-                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -753,97 +623,52 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(
-    tag_prefix: str,
-    root: str,
-    verbose: bool,
-    runner: Callable = run_command
-) -> Dict[str, Any]:
+def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%%s*" %% tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces: Dict[str, Any] = {}
+    pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
-    # --abbrev-ref was added in git-1.6.3
-    if rc != 0 or branch_name is None:
-        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
-    branch_name = branch_name.strip()
-
-    if branch_name == "HEAD":
-        # If we aren't exactly on a branch, pick a branch which represents
-        # the current commit. If all else fails, we are on a branchless
-        # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
-        # --contains was added in git-1.5.4
-        if rc != 0 or branches is None:
-            raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
-
-        # Remove the first line if we're running detached
-        if "(" in branches[0]:
-            branches.pop(0)
-
-        # Strip off the leading "* " from the list of branches.
-        branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
-        elif not branches:
-            branch_name = None
-        else:
-            # Pick the first branch that is returned. Good or bad.
-            branch_name = branches[0]
-
-    pieces["branch"] = branch_name
-
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -852,15 +677,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparsable. Maybe git-describe is misbehaving?
+            # unparseable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -877,35 +702,37 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
+                       cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces: Dict[str, Any]) -> str:
+def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces: Dict[str, Any]) -> str:
+def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -922,79 +749,31 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
-
-    The ".dev0" means not master branch. Note that .dev0 sorts backwards
-    (a feature branch will appear "older" than the master branch).
-
-    Exceptions:
-    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
-    """Split pep440 version string at the post-release segment.
-
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
-    """
-    vc = str.split(ver, ".post")
-    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
-
-
-def render_pep440_pre(pieces: Dict[str, Any]) -> str:
-    """TAG[.postN.devDISTANCE] -- No -dirty.
+def render_pep440_pre(pieces):
+    """TAG[.post0.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
-            rendered = tag_version
-            if post_version is not None:
-                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
-            else:
-                rendered += ".post0.dev%%d" %% (pieces["distance"])
-        else:
-            # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
+            rendered += ".post0.dev%%d" %% pieces["distance"]
     else:
         # exception #1
         rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces: Dict[str, Any]) -> str:
+def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1013,44 +792,15 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
-
-    The ".dev0" means not master branch.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%%d" %% pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%%s" %% pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0.post%%d" %% pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%%s" %% pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_old(pieces: Dict[str, Any]) -> str:
+def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1064,15 +814,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces: Dict[str, Any]) -> str:
+def render_git_describe(pieces):
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1084,15 +834,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces: Dict[str, Any]) -> str:
+def render_git_describe_long(pieces):
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1104,51 +854,47 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
+def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
-        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
-        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions() -> Dict[str, Any]:
+def get_versions():
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -1161,15 +907,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for _ in cfg.versionfile_source.split('/'):
+        for i in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -1188,50 +934,47 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
+def git_get_keywords(versionfile_abs):
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords: Dict[str, str] = {}
+    keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith("git_refnames ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["date"] = mo.group(1)
-    except OSError:
+        f = open(versionfile_abs, "r")
+        for line in f.readlines():
+            if line.strip().startswith("git_refnames ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["refnames"] = mo.group(1)
+            if line.strip().startswith("git_full ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["full"] = mo.group(1)
+            if line.strip().startswith("git_date ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["date"] = mo.group(1)
+        f.close()
+    except EnvironmentError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(
-    keywords: Dict[str, str],
-    tag_prefix: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
+    if not keywords:
+        raise NotThisMethod("no keywords at all, weird")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
         date = date.splitlines()[-1]
 
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
@@ -1242,41 +985,36 @@
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
-            # Filter out refs that exactly match prefix or that don't start
-            # with a number once the prefix is stripped (mostly a concern
-            # when prefix is '')
-            if not re.match(r'\d', r):
-                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1284,97 +1022,52 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(
-    tag_prefix: str,
-    root: str,
-    verbose: bool,
-    runner: Callable = run_command
-) -> Dict[str, Any]:
+def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%s*" % tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces: Dict[str, Any] = {}
+    pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
-    # --abbrev-ref was added in git-1.6.3
-    if rc != 0 or branch_name is None:
-        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
-    branch_name = branch_name.strip()
-
-    if branch_name == "HEAD":
-        # If we aren't exactly on a branch, pick a branch which represents
-        # the current commit. If all else fails, we are on a branchless
-        # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
-        # --contains was added in git-1.5.4
-        if rc != 0 or branches is None:
-            raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
-
-        # Remove the first line if we're running detached
-        if "(" in branches[0]:
-            branches.pop(0)
-
-        # Strip off the leading "* " from the list of branches.
-        branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
-        elif not branches:
-            branch_name = None
-        else:
-            # Pick the first branch that is returned. Good or bad.
-            branch_name = branches[0]
-
-    pieces["branch"] = branch_name
-
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1383,15 +1076,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparsable. Maybe git-describe is misbehaving?
+            # unparseable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1408,95 +1101,94 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
+                       cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
+def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [versionfile_source]
+    files = [manifest_in, versionfile_source]
     if ipy:
         files.append(ipy)
-    if "VERSIONEER_PEP518" not in globals():
-        try:
-            my_path = __file__
-            if my_path.endswith((".pyc", ".pyo")):
-                my_path = os.path.splitext(my_path)[0] + ".py"
-            versioneer_file = os.path.relpath(my_path)
-        except NameError:
-            versioneer_file = "versioneer.py"
-        files.append(versioneer_file)
+    try:
+        me = __file__
+        if me.endswith(".pyc") or me.endswith(".pyo"):
+            me = os.path.splitext(me)[0] + ".py"
+        versioneer_file = os.path.relpath(me)
+    except NameError:
+        versioneer_file = "versioneer.py"
+    files.append(versioneer_file)
     present = False
     try:
-        with open(".gitattributes", "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith(versionfile_source):
-                    if "export-subst" in line.strip().split()[1:]:
-                        present = True
-                        break
-    except OSError:
+        f = open(".gitattributes", "r")
+        for line in f.readlines():
+            if line.strip().startswith(versionfile_source):
+                if "export-subst" in line.strip().split()[1:]:
+                    present = True
+        f.close()
+    except EnvironmentError:
         pass
     if not present:
-        with open(".gitattributes", "a+") as fobj:
-            fobj.write(f"{versionfile_source} export-subst\n")
+        f = open(".gitattributes", "a+")
+        f.write("%s export-subst\n" % versionfile_source)
+        f.close()
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(
-    parentdir_prefix: str,
-    root: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for _ in range(3):
+    for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        rootdirs.append(root)
-        root = os.path.dirname(root)  # up a level
+        else:
+            rootdirs.append(root)
+            root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.29) from
+# This file was generated by 'versioneer.py' (0.19) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1505,49 +1197,50 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename: str) -> Dict[str, Any]:
+def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except OSError:
+    except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
+def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
+    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
                           indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces: Dict[str, Any]) -> str:
+def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces: Dict[str, Any]) -> str:
+def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1564,79 +1257,31 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
-
-    The ".dev0" means not master branch. Note that .dev0 sorts backwards
-    (a feature branch will appear "older" than the master branch).
-
-    Exceptions:
-    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
-    """Split pep440 version string at the post-release segment.
-
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
-    """
-    vc = str.split(ver, ".post")
-    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
-
-
-def render_pep440_pre(pieces: Dict[str, Any]) -> str:
-    """TAG[.postN.devDISTANCE] -- No -dirty.
+def render_pep440_pre(pieces):
+    """TAG[.post0.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
-            rendered = tag_version
-            if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
-            else:
-                rendered += ".post0.dev%d" % (pieces["distance"])
-        else:
-            # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
+            rendered += ".post0.dev%d" % pieces["distance"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces: Dict[str, Any]) -> str:
+def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1655,44 +1300,15 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
-
-    The ".dev0" means not master branch.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%s" % pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%s" % pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_old(pieces: Dict[str, Any]) -> str:
+def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1706,15 +1322,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces: Dict[str, Any]) -> str:
+def render_git_describe(pieces):
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1726,15 +1342,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces: Dict[str, Any]) -> str:
+def render_git_describe_long(pieces):
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1746,36 +1362,32 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
+def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
-        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
-        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1786,30 +1398,30 @@
             "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose: bool = False) -> Dict[str, Any]:
+def get_versions(verbose=False):
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
+    verbose = verbose or cfg.verbose
     assert cfg.versionfile_source is not None, \
         "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
@@ -1862,21 +1474,21 @@
         print("unable to compute version")
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
-def get_version() -> str:
+def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
-    """Get the custom setuptools subclasses used by Versioneer.
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools/distutils subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1886,128 +1498,118 @@
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
+        # See https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to setuptools
-    from setuptools import Command
+    # we add "version" to both distutils and setuptools
+    from distutils.core import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options: List[Tuple[str, str, str]] = []
-        boolean_options: List[str] = []
+        user_options = []
+        boolean_options = []
 
-        def initialize_options(self) -> None:
+        def initialize_options(self):
             pass
 
-        def finalize_options(self) -> None:
+        def finalize_options(self):
             pass
 
-        def run(self) -> None:
+        def run(self):
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in setuptools
+    # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
-    # pip install -e . and setuptool/editable_wheel will invoke build_py
-    # but the build_py command is not expected to copy any files.
-
     # we override different "build_py" commands for both environments
     if 'build_py' in cmds:
-        _build_py: Any = cmds['build_py']
-    else:
+        _build_py = cmds['build_py']
+    elif "setuptools" in sys.modules:
         from setuptools.command.build_py import build_py as _build_py
+    else:
+        from distutils.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self) -> None:
+        def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
-            if getattr(self, "editable_mode", False):
-                # During editable installs `.py` and data files are
-                # not copied to build_lib
-                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
     if 'build_ext' in cmds:
-        _build_ext: Any = cmds['build_ext']
-    else:
+        _build_ext = cmds['build_ext']
+    elif "setuptools" in sys.modules:
         from setuptools.command.build_ext import build_ext as _build_ext
+    else:
+        from distutils.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
-        def run(self) -> None:
+        def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
             if self.inplace:
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
-            if not cfg.versionfile_build:
-                return
             target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
-            if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
-                return
+                                              cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
+        from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self) -> None:
+            def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -2022,21 +1624,18 @@
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
-        try:
-            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
-        except ImportError:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
+        from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
-            def run(self) -> None:
+            def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -2049,67 +1648,32 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
-    # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info: Any = cmds['egg_info']
-    else:
-        from setuptools.command.egg_info import egg_info as _egg_info
-
-    class cmd_egg_info(_egg_info):
-        def find_sources(self) -> None:
-            # egg_info.find_sources builds the manifest list and writes it
-            # in one shot
-            super().find_sources()
-
-            # Modify the filelist and normalize it
-            root = get_root()
-            cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
-            if cfg.versionfile_source:
-                # There are rare cases where versionfile_source might not be
-                # included by default, so we must be explicit
-                self.filelist.append(cfg.versionfile_source)
-            self.filelist.sort()
-            self.filelist.remove_duplicates()
-
-            # The write method is hidden in the manifest_maker instance that
-            # generated the filelist and was thrown away
-            # We will instead replicate their final normalization (to unicode,
-            # and POSIX-style paths)
-            from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
-
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
-
-    cmds['egg_info'] = cmd_egg_info
-
     # we override different "sdist" commands for both environments
     if 'sdist' in cmds:
-        _sdist: Any = cmds['sdist']
-    else:
+        _sdist = cmds['sdist']
+    elif "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
+    else:
+        from distutils.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self) -> None:
+        def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
+        def make_release_tree(self, base_dir, files):
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -2154,34 +1718,29 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-OLD_SNIPPET = """
+INIT_PY_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
-INIT_PY_SNIPPET = """
-from . import {0}
-__version__ = {0}.get_versions()['version']
-"""
 
-
-def do_setup() -> int:
+def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
+    except (EnvironmentError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (OSError, configparser.NoSectionError)):
+        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -2193,45 +1752,70 @@
                         "TAG_PREFIX": cfg.tag_prefix,
                         "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                         "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
-    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except OSError:
+        except EnvironmentError:
             old = ""
-        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
-        snippet = INIT_PY_SNIPPET.format(module)
-        if OLD_SNIPPET in old:
-            print(" replacing boilerplate in %s" % ipy)
-            with open(ipy, "w") as f:
-                f.write(old.replace(OLD_SNIPPET, snippet))
-        elif snippet not in old:
+        if INIT_PY_SNIPPET not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(snippet)
+                f.write(INIT_PY_SNIPPET)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        maybe_ipy = None
+        ipy = None
+
+    # Make sure both the top-level "versioneer.py" and versionfile_source
+    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
+    # they'll be copied into source distributions. Pip won't be able to
+    # install the package without this.
+    manifest_in = os.path.join(root, "MANIFEST.in")
+    simple_includes = set()
+    try:
+        with open(manifest_in, "r") as f:
+            for line in f:
+                if line.startswith("include "):
+                    for include in line.split()[1:]:
+                        simple_includes.add(include)
+    except EnvironmentError:
+        pass
+    # That doesn't cover everything MANIFEST.in can do
+    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
+    # it might give some false negatives. Appending redundant 'include'
+    # lines is safe, though.
+    if "versioneer.py" not in simple_includes:
+        print(" appending 'versioneer.py' to MANIFEST.in")
+        with open(manifest_in, "a") as f:
+            f.write("include versioneer.py\n")
+    else:
+        print(" 'versioneer.py' already in MANIFEST.in")
+    if cfg.versionfile_source not in simple_includes:
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
+        with open(manifest_in, "a") as f:
+            f.write("include %s\n" % cfg.versionfile_source)
+    else:
+        print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(cfg.versionfile_source, maybe_ipy)
+    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
     return 0
 
 
-def scan_setup_py() -> int:
+def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -2260,18 +1844,14 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
-def setup_command() -> NoReturn:
-    """Set up Versioneer and exit with appropriate error code."""
-    errors = do_setup()
-    errors += scan_setup_py()
-    sys.exit(1 if errors else 0)
-
-
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        setup_command()
+        errors = do_setup()
+        errors += scan_setup_py()
+        if errors:
+            sys.exit(1)
```

