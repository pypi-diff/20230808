# Comparing `tmp/torch_harmonics-0.6.1.tar.gz` & `tmp/torch_harmonics-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_harmonics-0.6.1.tar", last modified: Thu Jun  8 14:37:34 2023, max compression
+gzip compressed data, was "torch_harmonics-0.6.2.tar", last modified: Tue Aug  8 09:48:35 2023, max compression
```

## Comparing `torch_harmonics-0.6.1.tar` & `torch_harmonics-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.145497 torch_harmonics-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/tests/test_distributed_backward_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/tests/test_distributed_forward_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.145497 torch_harmonics-0.6.1/torch_harmonics/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/torch_harmonics/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27471 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/distributed/distributed_sht.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/distributed/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/torch_harmonics/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/pde_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/contractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/factorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/sfno.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/examples/shallow_water_equations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/legendre.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/random_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/sht.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-08 14:36:54.000000 torch_harmonics-0.6.1/torch_harmonics/test_torch_harmonics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:37:34.149497 torch_harmonics-0.6.1/torch_harmonics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-08 14:37:34.000000 torch_harmonics-0.6.1/torch_harmonics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-08 14:37:34.000000 torch_harmonics-0.6.1/torch_harmonics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:37:34.000000 torch_harmonics-0.6.1/torch_harmonics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 14:37:34.000000 torch_harmonics-0.6.1/torch_harmonics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 14:37:34.000000 torch_harmonics-0.6.1/torch_harmonics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 09:47:48.000000 torch_harmonics-0.6.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 09:47:48.000000 torch_harmonics-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-08-08 09:47:48.000000 torch_harmonics-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/tests/test_distributed_backward_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/tests/test_distributed_forward_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/torch_harmonics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/torch_harmonics/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27471 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/distributed/distributed_sht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/distributed/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/torch_harmonics/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/pde_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/contractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/factorizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/sfno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/examples/shallow_water_equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/legendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/random_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/sht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-08 09:47:49.000000 torch_harmonics-0.6.2/torch_harmonics/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:48:35.295697 torch_harmonics-0.6.2/torch_harmonics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-08-08 09:48:35.000000 torch_harmonics-0.6.2/torch_harmonics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-08 09:48:35.000000 torch_harmonics-0.6.2/torch_harmonics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:48:35.000000 torch_harmonics-0.6.2/torch_harmonics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 09:48:35.000000 torch_harmonics-0.6.2/torch_harmonics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 09:48:35.000000 torch_harmonics-0.6.2/torch_harmonics.egg-info/top_level.txt
```

### Comparing `torch_harmonics-0.6.1/LICENSE` & `torch_harmonics-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/PKG-INFO` & `torch_harmonics-0.6.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: torch_harmonics
-Version: 0.6.1
-Summary: A differentiable spherical harmonic transform for PyTorch.
-Home-page: https://github.com/NVIDIA/torch-harmonics
-License: Modified BSD
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: sfno
-License-File: LICENSE
-License-File: AUTHORS
-
 <!-- 
 SPDX-FileCopyrightText: Copyright (c) 2022 The torch-harmonics Authors. All rights reserved.
 
 SPDX-License-Identifier: BSD-3-Clause
  
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
@@ -40,33 +25,40 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 -->
 
 <p align="center">
-    <img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/logo/logo.png"  width="568">
+    <img src="https://raw.githubusercontent.com/NVIDIA/torch-harmonics/main/images/logo/logo.png"  width="568">
+    <br>
+    <a href="https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml"><img src="https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml/badge.svg"></a>
+    <a href="https://pypi.org/project/torch_harmonics/"><img src="https://img.shields.io/pypi/v/torch_harmonics"></a>
 </p>
 
+<!--
+[![pypi](https://img.shields.io/pypi/v/torch_harmonics)](https://pypi.org/project/torch_harmonics/)
+-->
+
 <!-- # torch-harmonics: differentiable harmonic transforms -->
 
 <!-- ## What is torch-harmonics? -->
 
-`torch_harmonics` is a differentiable implementation of the Spherical Harmonic transform in PyTorch. It was originally implemented to enable Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute the projection onto the associated Legendre polynomials and FFTs for the projection onto the harmonic basis. This algorithm tends to outperform others with better asymptotic scaling for most practical purposes.
+`torch-harmonics` is a differentiable implementation of the Spherical Harmonic transform in PyTorch. It was originally implemented to enable Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute the projection onto the associated Legendre polynomials and FFTs for the projection onto the harmonic basis. This algorithm tends to outperform others with better asymptotic scaling for most practical purposes.
 
-`torch_harmonics` uses PyTorch primitives to implement these operations, making it fully differentiable. Moreover, the quadrature can be distributed onto multiple ranks making it spatially distributed.
+`torch-harmonics` uses PyTorch primitives to implement these operations, making it fully differentiable. Moreover, the quadrature can be distributed onto multiple ranks making it spatially distributed.
 
-`torch_harmonics` has been used to implement a variety of differentiable PDE solvers which generated the animations below. Moreover, it has enabled the development of Spherical Fourier Neural Operators (SFNOs) [1].
+`torch-harmonics` has been used to implement a variety of differentiable PDE solvers which generated the animations below. Moreover, it has enabled the development of Spherical Fourier Neural Operators (SFNOs) [1].
 
 
 <table border="0" cellspacing="0" cellpadding="0">
     <tr>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/sfno.gif"  width="240"></td>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/zonal_jet.gif"  width="240"></td>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/allen-cahn.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/sfno.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/zonal_jet.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/allen-cahn.gif"  width="240"></td>
     </tr>
 <!--     <tr>
         <td style="text-align:center; border-style : hidden!important;">Shallow Water Eqns.</td>
         <td style="text-align:center; border-style : hidden!important;">Ginzburg-Landau Eqn.</td>
         <td style="text-align:center; border-style : hidden!important;">Allen-Cahn Eqn.</td>
     </tr>  -->
 </table>
@@ -79,22 +71,23 @@
 pip install torch-harmonics
 ```
 
 Build in your environment using the Python package:
 
 ```
 git clone git@github.com:NVIDIA/torch-harmonics.git
-pip install ./torch_harmonics
+cd torch-harmonics
+pip install -e .
 ```
 
 Alternatively, use the Dockerfile to build your custom container after cloning:
 
 ```
 git clone git@github.com:NVIDIA/torch-harmonics.git
-cd torch_harmonics
+cd torch-harmonics
 docker build . -t torch_harmonics
 docker run --gpus all -it --rm --ipc=host --ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics
 ```
 
 ## Contributors
 
  - Boris Bonev (bbonev@nvidia.com)
@@ -158,20 +151,20 @@
 
 nlat = 512
 nlon = 2*nlat
 batch_size = 32
 signal = torch.randn(batch_size, nlat, nlon)
 
 # transform data on an equiangular grid
-sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device).float()
+sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device)
 
 coeffs = sht(signal)
 ```
 
-`torch_harmonics` also implements a distributed variant of the SHT located in `torch-harmonics.distributed`.
+To enable scalable model-parallelism, `torch-harmonics` implements a distributed variant of the SHT located in `torch_harmonics.distributed`.
 
 ### Cite us
 
 If you use `torch-harmonics` in an academic paper, please cite [1]
 
 ```
 @misc{bonev2023spherical,
@@ -196,9 +189,7 @@
 Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations;
 G3: Geochemistry, Geophysics, Geosystems, 2013.
 
 <a id="1">[3]</a> 
 Wang B., Wang L., Xie Z.;
 Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids;
 Adv Comput Math, 2018.
-
-
```

#### html2text {}

```diff
@@ -1,70 +1,67 @@
-Metadata-Version: 2.1 Name: torch_harmonics Version: 0.6.1 Summary: A
-differentiable spherical harmonic transform for PyTorch. Home-page: https://
-github.com/NVIDIA/torch-harmonics License: Modified BSD Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering Classifier: License :: OSI Approved
-:: BSD License Classifier: Programming Language :: Python :: 3 Description-
-Content-Type: text/markdown Provides-Extra: sfno License-File: LICENSE License-
-File: AUTHORS
-  [https://github.com/NVIDIA/torch-harmonics/blob/main/images/logo/logo.png]
-  `torch_harmonics` is a differentiable implementation of the Spherical
+  [https://raw.githubusercontent.com/NVIDIA/torch-harmonics/main/images/logo/
+                                  logo.png]
+    [https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml/
+          badge.svg] [https://img.shields.io/pypi/v/torch_harmonics]
+   `torch-harmonics` is a differentiable implementation of the Spherical
 Harmonic transform in PyTorch. It was originally implemented to enable
 Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute
 the projection onto the associated Legendre polynomials and FFTs for the
 projection onto the harmonic basis. This algorithm tends to outperform others
-with better asymptotic scaling for most practical purposes. `torch_harmonics`
+with better asymptotic scaling for most practical purposes. `torch-harmonics`
 uses PyTorch primitives to implement these operations, making it fully
 differentiable. Moreover, the quadrature can be distributed onto multiple ranks
-making it spatially distributed. `torch_harmonics` has been used to implement a
+making it spatially distributed. `torch-harmonics` has been used to implement a
 variety of differentiable PDE solvers which generated the animations below.
 Moreover, it has enabled the development of Spherical Fourier Neural Operators
 (SFNOs) [1].
-[https://github.com/       [https://github.com/    [https://github.com/NVIDIA/
-NVIDIA/torch-harmonics/    NVIDIA/torch-harmonics/ torch-harmonics/blob/main/
-blob/main/images/sfno.gif] blob/main/images/       images/allen-cahn.gif]
-                           zonal_jet.gif]
+[https://                    [https://                    [https://
+media.githubusercontent.com/ media.githubusercontent.com/ media.githubusercontent.com/
+media/NVIDIA/torch-          media/NVIDIA/torch-          media/NVIDIA/torch-
+harmonics/main/images/       harmonics/main/images/       harmonics/main/images/allen-
+sfno.gif]                    zonal_jet.gif]               cahn.gif]
 ## Installation Download directyly from PyPI: ``` pip install torch-harmonics
 ``` Build in your environment using the Python package: ``` git clone
-git@github.com:NVIDIA/torch-harmonics.git pip install ./torch_harmonics ```
-Alternatively, use the Dockerfile to build your custom container after cloning:
-``` git clone git@github.com:NVIDIA/torch-harmonics.git cd torch_harmonics
-docker build . -t torch_harmonics docker run --gpus all -it --rm --ipc=host --
-ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics ``` ## Contributors -
-Boris Bonev (bbonev@nvidia.com) - Thorsten Kurth (tkurth@nvidia.com) -
-Christian Hundt (chundt@nvidia.com) - Nikola Kovachki (nkovachki@nvidia.com) -
-Jean Kossaifi (jkossaifi@nvidia.com) ## Implementation The implementation
-follows the algorithm as presented in [2]. ### Spherical harmonic transform The
-truncated series expansion of a function $f$ defined on the surface of a sphere
-can be written as $$ f(\theta, \lambda) = \sum_{m=-M}^{M} \exp(im\lambda) \sum_
-{n=|m|}^{M} F_n^m \bar{P}_n^m (\cos \theta), $$ where $\theta$ is the
-colatitude, $\lambda$ the longitude, $\bar{P}_n^m$ the normalized, associated
-Legendre polynomials and $F_n^m$, the expansion coefficient associated to the
-mode $(m,n)$. A direct spherical harmonic transform can be accomplished by a
-Fourier transform $$ F^m(\theta) = \frac{1}{2 \pi} \int_{0}^{2\pi} f(\theta,
-\lambda) \exp(-im\lambda) \mathrm{d}\lambda $$ in longitude and a Legendre
-transform $$ F_n^m = \frac{1}{2} \int_{-1}^1 F^m(\theta) \bar{P}_n^m(\cos
-\theta) \mathrm{d} \cos \theta $$ in latitude. ### Discrete Legendre transform
-in order to apply the Legendre transfor, we shall use Gauss-Legendre points in
-the latitudinal direction. The integral $$ F_n^m = \int_{0}^\pi F^m(\theta)
-\bar{P}_n^m(\cos \theta) \sin \theta \mathrm{d} \theta $$ is approximated by
-the sum $$ F_n^m = \sum_{j=1}^{N_\theta} F^m(\theta_j) \bar{P}_n^m(\cos
-\theta_j) w_j $$ ## Usage ### Getting started The main functionality of
-`torch_harmonics` is provided in the form of `torch.nn.Modules` for
-composability. A minimum example is given by: ```python import torch import
-torch_harmonics as th device = torch.device('cuda' if torch.cuda.is_available()
-else 'cpu') nlat = 512 nlon = 2*nlat batch_size = 32 signal = torch.randn
-(batch_size, nlat, nlon) # transform data on an equiangular grid sht =
-th.RealSHT(nlat, nlon, grid="equiangular").to(device).float() coeffs = sht
-(signal) ``` `torch_harmonics` also implements a distributed variant of the SHT
-located in `torch-harmonics.distributed`. ### Cite us If you use `torch-
-harmonics` in an academic paper, please cite [1] ``` @misc{bonev2023spherical,
-title={Spherical Fourier Neural Operators: Learning Stable Dynamics on the
-Sphere}, author={Boris Bonev and Thorsten Kurth and Christian Hundt and Jaideep
-Pathak and Maximilian Baust and Karthik Kashinath and Anima Anandkumar}, year=
-{2023}, eprint={2306.03838}, archivePrefix={arXiv}, primaryClass={cs.LG} } ```
-## References [1] Bonev B., Kurth T., Hundt C., Pathak, J., Baust M., Kashinath
-K., Anandkumar A.; Spherical Fourier Neural Operators: Learning Stable Dynamics
-on the Sphere; arXiv 2306.0383, 2023. [2] Schaeffer N.; Efficient spherical
-harmonic transforms aimed at pseudospectral numerical simulations; G3:
-Geochemistry, Geophysics, Geosystems, 2013. [3] Wang B., Wang L., Xie Z.;
-Accurate calculation of spherical and vector spherical harmonic expansions via
-spectral element grids; Adv Comput Math, 2018.
+git@github.com:NVIDIA/torch-harmonics.git cd torch-harmonics pip install -e .
+``` Alternatively, use the Dockerfile to build your custom container after
+cloning: ``` git clone git@github.com:NVIDIA/torch-harmonics.git cd torch-
+harmonics docker build . -t torch_harmonics docker run --gpus all -it --rm --
+ipc=host --ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics ``` ##
+Contributors - Boris Bonev (bbonev@nvidia.com) - Thorsten Kurth
+(tkurth@nvidia.com) - Christian Hundt (chundt@nvidia.com) - Nikola Kovachki
+(nkovachki@nvidia.com) - Jean Kossaifi (jkossaifi@nvidia.com) ## Implementation
+The implementation follows the algorithm as presented in [2]. ### Spherical
+harmonic transform The truncated series expansion of a function $f$ defined on
+the surface of a sphere can be written as $$ f(\theta, \lambda) = \sum_{m=-M}^
+{M} \exp(im\lambda) \sum_{n=|m|}^{M} F_n^m \bar{P}_n^m (\cos \theta), $$ where
+$\theta$ is the colatitude, $\lambda$ the longitude, $\bar{P}_n^m$ the
+normalized, associated Legendre polynomials and $F_n^m$, the expansion
+coefficient associated to the mode $(m,n)$. A direct spherical harmonic
+transform can be accomplished by a Fourier transform $$ F^m(\theta) = \frac{1}
+{2 \pi} \int_{0}^{2\pi} f(\theta, \lambda) \exp(-im\lambda) \mathrm{d}\lambda
+$$ in longitude and a Legendre transform $$ F_n^m = \frac{1}{2} \int_{-1}^1 F^m
+(\theta) \bar{P}_n^m(\cos \theta) \mathrm{d} \cos \theta $$ in latitude. ###
+Discrete Legendre transform in order to apply the Legendre transfor, we shall
+use Gauss-Legendre points in the latitudinal direction. The integral $$ F_n^m =
+\int_{0}^\pi F^m(\theta) \bar{P}_n^m(\cos \theta) \sin \theta \mathrm{d} \theta
+$$ is approximated by the sum $$ F_n^m = \sum_{j=1}^{N_\theta} F^m(\theta_j)
+\bar{P}_n^m(\cos \theta_j) w_j $$ ## Usage ### Getting started The main
+functionality of `torch_harmonics` is provided in the form of
+`torch.nn.Modules` for composability. A minimum example is given by: ```python
+import torch import torch_harmonics as th device = torch.device('cuda' if
+torch.cuda.is_available() else 'cpu') nlat = 512 nlon = 2*nlat batch_size = 32
+signal = torch.randn(batch_size, nlat, nlon) # transform data on an equiangular
+grid sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device) coeffs = sht
+(signal) ``` To enable scalable model-parallelism, `torch-harmonics` implements
+a distributed variant of the SHT located in `torch_harmonics.distributed`. ###
+Cite us If you use `torch-harmonics` in an academic paper, please cite [1] ```
+@misc{bonev2023spherical, title={Spherical Fourier Neural Operators: Learning
+Stable Dynamics on the Sphere}, author={Boris Bonev and Thorsten Kurth and
+Christian Hundt and Jaideep Pathak and Maximilian Baust and Karthik Kashinath
+and Anima Anandkumar}, year={2023}, eprint={2306.03838}, archivePrefix={arXiv},
+primaryClass={cs.LG} } ``` ## References [1] Bonev B., Kurth T., Hundt C.,
+Pathak, J., Baust M., Kashinath K., Anandkumar A.; Spherical Fourier Neural
+Operators: Learning Stable Dynamics on the Sphere; arXiv 2306.0383, 2023. [2]
+Schaeffer N.; Efficient spherical harmonic transforms aimed at pseudospectral
+numerical simulations; G3: Geochemistry, Geophysics, Geosystems, 2013. [3] Wang
+B., Wang L., Xie Z.; Accurate calculation of spherical and vector spherical
+harmonic expansions via spectral element grids; Adv Comput Math, 2018.
```

### Comparing `torch_harmonics-0.6.1/README.md` & `torch_harmonics-0.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: torch_harmonics
+Version: 0.6.2
+Summary: A differentiable spherical harmonic transform for PyTorch.
+Home-page: https://github.com/NVIDIA/torch-harmonics
+License: Modified BSD
+Platform: UNKNOWN
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Provides-Extra: sfno
+License-File: LICENSE
+License-File: AUTHORS
+
 <!-- 
 SPDX-FileCopyrightText: Copyright (c) 2022 The torch-harmonics Authors. All rights reserved.
 
 SPDX-License-Identifier: BSD-3-Clause
  
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
@@ -25,33 +40,40 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 -->
 
 <p align="center">
-    <img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/logo/logo.png"  width="568">
+    <img src="https://raw.githubusercontent.com/NVIDIA/torch-harmonics/main/images/logo/logo.png"  width="568">
+    <br>
+    <a href="https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml"><img src="https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml/badge.svg"></a>
+    <a href="https://pypi.org/project/torch_harmonics/"><img src="https://img.shields.io/pypi/v/torch_harmonics"></a>
 </p>
 
+<!--
+[![pypi](https://img.shields.io/pypi/v/torch_harmonics)](https://pypi.org/project/torch_harmonics/)
+-->
+
 <!-- # torch-harmonics: differentiable harmonic transforms -->
 
 <!-- ## What is torch-harmonics? -->
 
-`torch_harmonics` is a differentiable implementation of the Spherical Harmonic transform in PyTorch. It was originally implemented to enable Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute the projection onto the associated Legendre polynomials and FFTs for the projection onto the harmonic basis. This algorithm tends to outperform others with better asymptotic scaling for most practical purposes.
+`torch-harmonics` is a differentiable implementation of the Spherical Harmonic transform in PyTorch. It was originally implemented to enable Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute the projection onto the associated Legendre polynomials and FFTs for the projection onto the harmonic basis. This algorithm tends to outperform others with better asymptotic scaling for most practical purposes.
 
-`torch_harmonics` uses PyTorch primitives to implement these operations, making it fully differentiable. Moreover, the quadrature can be distributed onto multiple ranks making it spatially distributed.
+`torch-harmonics` uses PyTorch primitives to implement these operations, making it fully differentiable. Moreover, the quadrature can be distributed onto multiple ranks making it spatially distributed.
 
-`torch_harmonics` has been used to implement a variety of differentiable PDE solvers which generated the animations below. Moreover, it has enabled the development of Spherical Fourier Neural Operators (SFNOs) [1].
+`torch-harmonics` has been used to implement a variety of differentiable PDE solvers which generated the animations below. Moreover, it has enabled the development of Spherical Fourier Neural Operators (SFNOs) [1].
 
 
 <table border="0" cellspacing="0" cellpadding="0">
     <tr>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/sfno.gif"  width="240"></td>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/zonal_jet.gif"  width="240"></td>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/allen-cahn.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/sfno.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/zonal_jet.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/allen-cahn.gif"  width="240"></td>
     </tr>
 <!--     <tr>
         <td style="text-align:center; border-style : hidden!important;">Shallow Water Eqns.</td>
         <td style="text-align:center; border-style : hidden!important;">Ginzburg-Landau Eqn.</td>
         <td style="text-align:center; border-style : hidden!important;">Allen-Cahn Eqn.</td>
     </tr>  -->
 </table>
@@ -64,22 +86,23 @@
 pip install torch-harmonics
 ```
 
 Build in your environment using the Python package:
 
 ```
 git clone git@github.com:NVIDIA/torch-harmonics.git
-pip install ./torch_harmonics
+cd torch-harmonics
+pip install -e .
 ```
 
 Alternatively, use the Dockerfile to build your custom container after cloning:
 
 ```
 git clone git@github.com:NVIDIA/torch-harmonics.git
-cd torch_harmonics
+cd torch-harmonics
 docker build . -t torch_harmonics
 docker run --gpus all -it --rm --ipc=host --ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics
 ```
 
 ## Contributors
 
  - Boris Bonev (bbonev@nvidia.com)
@@ -143,20 +166,20 @@
 
 nlat = 512
 nlon = 2*nlat
 batch_size = 32
 signal = torch.randn(batch_size, nlat, nlon)
 
 # transform data on an equiangular grid
-sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device).float()
+sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device)
 
 coeffs = sht(signal)
 ```
 
-`torch_harmonics` also implements a distributed variant of the SHT located in `torch-harmonics.distributed`.
+To enable scalable model-parallelism, `torch-harmonics` implements a distributed variant of the SHT located in `torch_harmonics.distributed`.
 
 ### Cite us
 
 If you use `torch-harmonics` in an academic paper, please cite [1]
 
 ```
 @misc{bonev2023spherical,
@@ -181,7 +204,9 @@
 Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations;
 G3: Geochemistry, Geophysics, Geosystems, 2013.
 
 <a id="1">[3]</a> 
 Wang B., Wang L., Xie Z.;
 Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids;
 Adv Comput Math, 2018.
+
+
```

#### html2text {}

```diff
@@ -1,63 +1,74 @@
-  [https://github.com/NVIDIA/torch-harmonics/blob/main/images/logo/logo.png]
-  `torch_harmonics` is a differentiable implementation of the Spherical
+Metadata-Version: 2.1 Name: torch_harmonics Version: 0.6.2 Summary: A
+differentiable spherical harmonic transform for PyTorch. Home-page: https://
+github.com/NVIDIA/torch-harmonics License: Modified BSD Platform: UNKNOWN
+Classifier: Topic :: Scientific/Engineering Classifier: License :: OSI Approved
+:: BSD License Classifier: Programming Language :: Python :: 3 Description-
+Content-Type: text/markdown Provides-Extra: sfno License-File: LICENSE License-
+File: AUTHORS
+  [https://raw.githubusercontent.com/NVIDIA/torch-harmonics/main/images/logo/
+                                  logo.png]
+    [https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml/
+          badge.svg] [https://img.shields.io/pypi/v/torch_harmonics]
+   `torch-harmonics` is a differentiable implementation of the Spherical
 Harmonic transform in PyTorch. It was originally implemented to enable
 Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute
 the projection onto the associated Legendre polynomials and FFTs for the
 projection onto the harmonic basis. This algorithm tends to outperform others
-with better asymptotic scaling for most practical purposes. `torch_harmonics`
+with better asymptotic scaling for most practical purposes. `torch-harmonics`
 uses PyTorch primitives to implement these operations, making it fully
 differentiable. Moreover, the quadrature can be distributed onto multiple ranks
-making it spatially distributed. `torch_harmonics` has been used to implement a
+making it spatially distributed. `torch-harmonics` has been used to implement a
 variety of differentiable PDE solvers which generated the animations below.
 Moreover, it has enabled the development of Spherical Fourier Neural Operators
 (SFNOs) [1].
-[https://github.com/       [https://github.com/    [https://github.com/NVIDIA/
-NVIDIA/torch-harmonics/    NVIDIA/torch-harmonics/ torch-harmonics/blob/main/
-blob/main/images/sfno.gif] blob/main/images/       images/allen-cahn.gif]
-                           zonal_jet.gif]
+[https://                    [https://                    [https://
+media.githubusercontent.com/ media.githubusercontent.com/ media.githubusercontent.com/
+media/NVIDIA/torch-          media/NVIDIA/torch-          media/NVIDIA/torch-
+harmonics/main/images/       harmonics/main/images/       harmonics/main/images/allen-
+sfno.gif]                    zonal_jet.gif]               cahn.gif]
 ## Installation Download directyly from PyPI: ``` pip install torch-harmonics
 ``` Build in your environment using the Python package: ``` git clone
-git@github.com:NVIDIA/torch-harmonics.git pip install ./torch_harmonics ```
-Alternatively, use the Dockerfile to build your custom container after cloning:
-``` git clone git@github.com:NVIDIA/torch-harmonics.git cd torch_harmonics
-docker build . -t torch_harmonics docker run --gpus all -it --rm --ipc=host --
-ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics ``` ## Contributors -
-Boris Bonev (bbonev@nvidia.com) - Thorsten Kurth (tkurth@nvidia.com) -
-Christian Hundt (chundt@nvidia.com) - Nikola Kovachki (nkovachki@nvidia.com) -
-Jean Kossaifi (jkossaifi@nvidia.com) ## Implementation The implementation
-follows the algorithm as presented in [2]. ### Spherical harmonic transform The
-truncated series expansion of a function $f$ defined on the surface of a sphere
-can be written as $$ f(\theta, \lambda) = \sum_{m=-M}^{M} \exp(im\lambda) \sum_
-{n=|m|}^{M} F_n^m \bar{P}_n^m (\cos \theta), $$ where $\theta$ is the
-colatitude, $\lambda$ the longitude, $\bar{P}_n^m$ the normalized, associated
-Legendre polynomials and $F_n^m$, the expansion coefficient associated to the
-mode $(m,n)$. A direct spherical harmonic transform can be accomplished by a
-Fourier transform $$ F^m(\theta) = \frac{1}{2 \pi} \int_{0}^{2\pi} f(\theta,
-\lambda) \exp(-im\lambda) \mathrm{d}\lambda $$ in longitude and a Legendre
-transform $$ F_n^m = \frac{1}{2} \int_{-1}^1 F^m(\theta) \bar{P}_n^m(\cos
-\theta) \mathrm{d} \cos \theta $$ in latitude. ### Discrete Legendre transform
-in order to apply the Legendre transfor, we shall use Gauss-Legendre points in
-the latitudinal direction. The integral $$ F_n^m = \int_{0}^\pi F^m(\theta)
-\bar{P}_n^m(\cos \theta) \sin \theta \mathrm{d} \theta $$ is approximated by
-the sum $$ F_n^m = \sum_{j=1}^{N_\theta} F^m(\theta_j) \bar{P}_n^m(\cos
-\theta_j) w_j $$ ## Usage ### Getting started The main functionality of
-`torch_harmonics` is provided in the form of `torch.nn.Modules` for
-composability. A minimum example is given by: ```python import torch import
-torch_harmonics as th device = torch.device('cuda' if torch.cuda.is_available()
-else 'cpu') nlat = 512 nlon = 2*nlat batch_size = 32 signal = torch.randn
-(batch_size, nlat, nlon) # transform data on an equiangular grid sht =
-th.RealSHT(nlat, nlon, grid="equiangular").to(device).float() coeffs = sht
-(signal) ``` `torch_harmonics` also implements a distributed variant of the SHT
-located in `torch-harmonics.distributed`. ### Cite us If you use `torch-
-harmonics` in an academic paper, please cite [1] ``` @misc{bonev2023spherical,
-title={Spherical Fourier Neural Operators: Learning Stable Dynamics on the
-Sphere}, author={Boris Bonev and Thorsten Kurth and Christian Hundt and Jaideep
-Pathak and Maximilian Baust and Karthik Kashinath and Anima Anandkumar}, year=
-{2023}, eprint={2306.03838}, archivePrefix={arXiv}, primaryClass={cs.LG} } ```
-## References [1] Bonev B., Kurth T., Hundt C., Pathak, J., Baust M., Kashinath
-K., Anandkumar A.; Spherical Fourier Neural Operators: Learning Stable Dynamics
-on the Sphere; arXiv 2306.0383, 2023. [2] Schaeffer N.; Efficient spherical
-harmonic transforms aimed at pseudospectral numerical simulations; G3:
-Geochemistry, Geophysics, Geosystems, 2013. [3] Wang B., Wang L., Xie Z.;
-Accurate calculation of spherical and vector spherical harmonic expansions via
-spectral element grids; Adv Comput Math, 2018.
+git@github.com:NVIDIA/torch-harmonics.git cd torch-harmonics pip install -e .
+``` Alternatively, use the Dockerfile to build your custom container after
+cloning: ``` git clone git@github.com:NVIDIA/torch-harmonics.git cd torch-
+harmonics docker build . -t torch_harmonics docker run --gpus all -it --rm --
+ipc=host --ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics ``` ##
+Contributors - Boris Bonev (bbonev@nvidia.com) - Thorsten Kurth
+(tkurth@nvidia.com) - Christian Hundt (chundt@nvidia.com) - Nikola Kovachki
+(nkovachki@nvidia.com) - Jean Kossaifi (jkossaifi@nvidia.com) ## Implementation
+The implementation follows the algorithm as presented in [2]. ### Spherical
+harmonic transform The truncated series expansion of a function $f$ defined on
+the surface of a sphere can be written as $$ f(\theta, \lambda) = \sum_{m=-M}^
+{M} \exp(im\lambda) \sum_{n=|m|}^{M} F_n^m \bar{P}_n^m (\cos \theta), $$ where
+$\theta$ is the colatitude, $\lambda$ the longitude, $\bar{P}_n^m$ the
+normalized, associated Legendre polynomials and $F_n^m$, the expansion
+coefficient associated to the mode $(m,n)$. A direct spherical harmonic
+transform can be accomplished by a Fourier transform $$ F^m(\theta) = \frac{1}
+{2 \pi} \int_{0}^{2\pi} f(\theta, \lambda) \exp(-im\lambda) \mathrm{d}\lambda
+$$ in longitude and a Legendre transform $$ F_n^m = \frac{1}{2} \int_{-1}^1 F^m
+(\theta) \bar{P}_n^m(\cos \theta) \mathrm{d} \cos \theta $$ in latitude. ###
+Discrete Legendre transform in order to apply the Legendre transfor, we shall
+use Gauss-Legendre points in the latitudinal direction. The integral $$ F_n^m =
+\int_{0}^\pi F^m(\theta) \bar{P}_n^m(\cos \theta) \sin \theta \mathrm{d} \theta
+$$ is approximated by the sum $$ F_n^m = \sum_{j=1}^{N_\theta} F^m(\theta_j)
+\bar{P}_n^m(\cos \theta_j) w_j $$ ## Usage ### Getting started The main
+functionality of `torch_harmonics` is provided in the form of
+`torch.nn.Modules` for composability. A minimum example is given by: ```python
+import torch import torch_harmonics as th device = torch.device('cuda' if
+torch.cuda.is_available() else 'cpu') nlat = 512 nlon = 2*nlat batch_size = 32
+signal = torch.randn(batch_size, nlat, nlon) # transform data on an equiangular
+grid sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device) coeffs = sht
+(signal) ``` To enable scalable model-parallelism, `torch-harmonics` implements
+a distributed variant of the SHT located in `torch_harmonics.distributed`. ###
+Cite us If you use `torch-harmonics` in an academic paper, please cite [1] ```
+@misc{bonev2023spherical, title={Spherical Fourier Neural Operators: Learning
+Stable Dynamics on the Sphere}, author={Boris Bonev and Thorsten Kurth and
+Christian Hundt and Jaideep Pathak and Maximilian Baust and Karthik Kashinath
+and Anima Anandkumar}, year={2023}, eprint={2306.03838}, archivePrefix={arXiv},
+primaryClass={cs.LG} } ``` ## References [1] Bonev B., Kurth T., Hundt C.,
+Pathak, J., Baust M., Kashinath K., Anandkumar A.; Spherical Fourier Neural
+Operators: Learning Stable Dynamics on the Sphere; arXiv 2306.0383, 2023. [2]
+Schaeffer N.; Efficient spherical harmonic transforms aimed at pseudospectral
+numerical simulations; G3: Geochemistry, Geophysics, Geosystems, 2013. [3] Wang
+B., Wang L., Xie Z.; Accurate calculation of spherical and vector spherical
+harmonic expansions via spectral element grids; Adv Comput Math, 2018.
```

### Comparing `torch_harmonics-0.6.1/setup.py` & `torch_harmonics-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     'long_description': README,
     'long_description_content_type' : 'text/markdown',
     'url' : 'https://github.com/NVIDIA/torch-harmonics',
     'authors': [
         {'name': "Boris Bonev", 'email': "bbonev@nvidia.com"},
         ],
     'version': VERSION,
-    'install_requires': ['torch','numpy'],
+    'install_requires': ['torch', 'numpy'],
     'extras_require': {
         'sfno':  ['tensorly', 'tensorly-torch'],
     },
     'license': 'Modified BSD',
     'scripts': [],
     'include_package_data': True,
     'classifiers': [
```

### Comparing `torch_harmonics-0.6.1/tests/test_distributed_backward_transform.py` & `torch_harmonics-0.6.2/tests/test_distributed_backward_transform.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/tests/test_distributed_forward_transform.py` & `torch_harmonics-0.6.2/tests/test_distributed_forward_transform.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/__init__.py` & `torch_harmonics-0.6.2/torch_harmonics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '0.6.1'
+__version__ = '0.6.2'
 
 from .sht import RealSHT, InverseRealSHT, RealVectorSHT, InverseRealVectorSHT
 from . import quadrature
 from . import random_fields
-import examples
+from . import examples
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/distributed/__init__.py` & `torch_harmonics-0.6.2/torch_harmonics/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/distributed/distributed_sht.py` & `torch_harmonics-0.6.2/torch_harmonics/distributed/distributed_sht.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/distributed/primitives.py` & `torch_harmonics-0.6.2/torch_harmonics/distributed/primitives.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/distributed/utils.py` & `torch_harmonics-0.6.2/torch_harmonics/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/__init__.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/pde_sphere.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/pde_sphere.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,29 +26,19 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 
-import sys
-sys.path.append("..")
-sys.path.append(".")
-
 import torch
 import torch.nn as nn
 import torch_harmonics as harmonics
 
 import numpy as np
-import matplotlib.pyplot as plt
-
-try:
-    import cartopy.crs as ccrs
-except ImportError:
-    ccrs = None
 
 
 class SphereSolver(nn.Module):
     """
     Solver class on the sphere. Can solve the following PDEs:
     - Allen-Cahn eq
     """
@@ -136,14 +126,15 @@
         return rspec
 
 
     def plot_griddata(self, data, fig, cmap='twilight_shifted', vmax=None, vmin=None, projection='3d', title=None, antialiased=False):
         """
         plotting routine for data on the grid. Requires cartopy for 3d plots.
         """
+        import matplotlib.pyplot as plt
 
         lons = self.lons.squeeze() - torch.pi
         lats = self.lats.squeeze()
 
         if data.is_cuda:
             data = data.cpu()
             lons = lons.cpu()
@@ -161,16 +152,15 @@
             ax.set_xticklabels([])
             ax.set_yticklabels([])
             plt.colorbar(im, orientation='horizontal')
             plt.title(title)
 
         elif projection == '3d':
 
-            if ccrs is None:
-                raise ImportError("Couldn't import Cartopy")
+            import cartopy.crs as ccrs
 
             proj = ccrs.Orthographic(central_longitude=0.0, central_latitude=25.0)
 
             #ax = plt.gca(projection=proj, frameon=True)
             ax = fig.add_subplot(projection=proj)
             Lons = Lons*180/np.pi
             Lats = Lats*180/np.pi
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/__init__.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/__init__.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/activations.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/activations.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/contractions.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/contractions.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/factorizations.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/factorizations.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/layers.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,19 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-from functools import partial
-from collections import OrderedDict
-from copy import Error, deepcopy
-from re import S
-from numpy.lib.arraypad import pad
-import numpy as np
-
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 import torch.fft
-from torch.nn.modules.container import Sequential
-from torch.utils.checkpoint import checkpoint, checkpoint_sequential
+from torch.utils.checkpoint import checkpoint
 from torch.cuda import amp
-from typing import Optional
 import math
 
 from torch_harmonics import *
 from .contractions import *
 from .activations import *
 
 from .factorizations import get_contract_fun
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/sfno/models/sfno.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/sfno/models/sfno.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics/examples/shallow_water_equations.py` & `torch_harmonics-0.6.2/torch_harmonics/examples/shallow_water_equations.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,30 +26,21 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 
-import sys
-sys.path.append("..")
-sys.path.append(".")
-
 import torch
 import torch.nn as nn
 import torch_harmonics as harmonics
 from torch_harmonics.quadrature import *
 
 import numpy as np
-import matplotlib.pyplot as plt
 
-try:
-    import cartopy.crs as ccrs
-except ImportError:
-    ccrs = None
 
 class ShallowWaterSolver(nn.Module):
     """
     SWE solver class. Interface inspired bu pyspharm and SHTns
     """
 
     def __init__(self, nlat, nlon, dt, lmax=None, mmax=None, grid='legendre-gauss', radius=6.37122E6, \
@@ -333,14 +324,15 @@
         return out
 
 
     def plot_griddata(self, data, fig, cmap='twilight_shifted', vmax=None, vmin=None, projection='3d', title=None, antialiased=False):
         """
         plotting routine for data on the grid. Requires cartopy for 3d plots.
         """
+        import matplotlib.pyplot as plt
 
         lons = self.lons.squeeze() - torch.pi
         lats = self.lats.squeeze()
 
         if data.is_cuda:
             data = data.cpu()
             lons = lons.cpu()
@@ -358,16 +350,15 @@
             ax.set_xticklabels([])
             ax.set_yticklabels([])
             plt.colorbar(im, orientation='horizontal')
             plt.title(title)
 
         elif projection == '3d':
 
-            if ccrs is None:
-                raise ImportError("Couldn't import Cartopy")
+            import cartopy.crs as ccrs
 
             proj = ccrs.Orthographic(central_longitude=0.0, central_latitude=25.0)
 
             #ax = plt.gca(projection=proj, frameon=True)
             ax = fig.add_subplot(projection=proj)
             Lons = Lons*180/np.pi
             Lats = Lats*180/np.pi
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/legendre.py` & `torch_harmonics-0.6.2/torch_harmonics/legendre.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """
     defines the normalization factor to orthonormalize the Spherical Harmonics
     """
     return np.sqrt((2*l + 1) / 4 / np.pi) * np.sqrt(np.math.factorial(l-m) / np.math.factorial(l+m))
 
 
 def precompute_legpoly(mmax, lmax, t, norm="ortho", inverse=False, csphase=True):
-    """
+    r"""
     Computes the values of (-1)^m c^l_m P^l_m(\cos \theta) at the positions specified by x (theta)
     The resulting tensor has shape (mmax, lmax, len(x)).
     The Condon-Shortley Phase (-1)^m can be turned off optionally
 
     method of computation follows
     [1] Schaeffer, N.; Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations, G3: Geochemistry, Geophysics, Geosystems.
     [2] Rapp, R.H.; A Fortran Program for the Computation of Gravimetric Quantities from High Degree Spherical Harmonic Expansions, Ohio State University Columbus; report; 1982;
@@ -88,15 +88,15 @@
     if csphase:
         for m in range(1, mmax, 2):
             pct[m] *= -1
 
     return torch.from_numpy(pct)
 
 def precompute_dlegpoly(mmax, lmax, x, norm="ortho", inverse=False, csphase=True):
-    """
+    r"""
     Computes the values of the derivatives $\frac{d}{d \theta} P^m_l(\cos \theta)$
     at the positions specified by x (theta), as well as $\frac{1}{\sin \theta} P^m_l(\cos \theta)$,
     needed for the computation of the vector spherical harmonics. The resulting tensor has shape
     (2, mmax, lmax, len(x)).
 
     computation follows
     [2] Wang, B., Wang, L., Xie, Z.; Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids; Adv Comput Math.
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/quadrature.py` & `torch_harmonics-0.6.2/torch_harmonics/quadrature.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import numpy as np
 
 def legendre_gauss_weights(n, a=-1.0, b=1.0):
-    """
+    r"""
     Helper routine which returns the Legendre-Gauss nodes and weights
     on the interval [a, b]
     """
 
     xlg, wlg = np.polynomial.legendre.leggauss(n)
     xlg = (b - a) * 0.5 * xlg + (b + a) * 0.5
     wlg = wlg * (b - a) * 0.5
 
     return xlg, wlg
 
 def lobatto_weights(n, a=-1.0, b=1.0, tol=1e-16, maxiter=100):
-    """
+    r"""
     Helper routine which returns the Legendre-Gauss-Lobatto nodes and weights
     on the interval [a, b]
     """
 
     wlg = np.zeros((n,))
     tlg = np.zeros((n,))
     tmp = np.zeros((n,))
@@ -82,15 +82,15 @@
     tlg = (b - a) * 0.5 * tlg + (b + a) * 0.5
     wlg = wlg * (b - a) * 0.5
     
     return tlg, wlg
 
 
 def clenshaw_curtiss_weights(n, a=-1.0, b=1.0):
-    """
+    r"""
     Computation of the Clenshaw-Curtis quadrature nodes and weights.
     This implementation follows
 
     [1] Joerg Waldvogel, Fast Construction of the Fejer and Clenshaw-Curtis Quadrature Rules; BIT Numerical Mathematics, Vol. 43, No. 1, pp. 001–018.
     """
 
     assert(n > 1)
@@ -119,15 +119,15 @@
     # rescale
     tcc = (b - a) * 0.5 * tcc + (b + a) * 0.5
     wcc = wcc * (b - a) * 0.5
 
     return tcc, wcc
 
 def fejer2_weights(n, a=-1.0, b=1.0):
-    """
+    r"""
     Computation of the Fejer quadrature nodes and weights.
     This implementation follows
 
     [1] Joerg Waldvogel, Fast Construction of the Fejer and Clenshaw-Curtis Quadrature Rules; BIT Numerical Mathematics, Vol. 43, No. 1, pp. 001–018.
     """
 
     assert(n > 2)
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/random_fields.py` & `torch_harmonics-0.6.2/torch_harmonics/random_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 import torch
 from .sht import InverseRealSHT
 
 class GaussianRandomFieldS2(torch.nn.Module):
     def __init__(self, nlat, alpha=2.0, tau=3.0, sigma=None, radius=1.0, grid="equiangular", dtype=torch.float32):
         super().__init__()
-        """A mean-zero Gaussian Random Field on the sphere with Matern covariance:
+        r"""
+        A mean-zero Gaussian Random Field on the sphere with Matern covariance:
         C = sigma^2 (-Lap + tau^2 I)^(-alpha).
         
         Lap is the Laplacian on the sphere, I the identity operator,
         and sigma, tau, alpha are scalar parameters.
 
         Note: C is trace-class on L^2 if and only if alpha > 1.
     
@@ -89,15 +90,16 @@
         self.register_buffer('mean', mean)
         self.register_buffer('var', var)
 
         #Standard normal noise sampler.
         self.gaussian_noise = torch.distributions.normal.Normal(self.mean, self.var)
 
     def forward(self, N, xi=None):
-        """Sample random functions from a spherical GRF.
+        r"""
+        Sample random functions from a spherical GRF.
     
         Parameters
         ----------
         N : int
             Number of functions to sample.
         xi : torch.Tensor, default is None
             Noise is a complex tensor of size (N, nlat, nlat+1).
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/sht.py` & `torch_harmonics-0.6.2/torch_harmonics/sht.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,25 +35,25 @@
 import torch.fft
 
 from .quadrature import *
 from .legendre import *
 
 
 class RealSHT(nn.Module):
-    """
+    r"""
     Defines a module for computing the forward (real-valued) SHT.
     Precomputes Legendre Gauss nodes, weights and associated Legendre polynomials on these nodes.
     The SHT is applied to the last two dimensions of the input
 
     [1] Schaeffer, N. Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations, G3: Geochemistry, Geophysics, Geosystems.
     [2] Wang, B., Wang, L., Xie, Z.; Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids; Adv Comput Math.
     """
 
     def __init__(self, nlat, nlon, lmax=None, mmax=None, grid="lobatto", norm="ortho", csphase=True):
-        """
+        r"""
         Initializes the SHT Layer, precomputing the necessary quadrature weights
 
         Parameters:
         nlat: input grid resolution in the latitudinal direction
         nlon: input grid resolution in the longitudinal direction
         grid: grid in the latitude direction (for now only tensor product grids are supported)
         """
@@ -93,15 +93,15 @@
         pct = precompute_legpoly(self.mmax, self.lmax, tq, norm=self.norm, csphase=self.csphase)
         weights = torch.einsum('mlk,k->mlk', pct, weights)
 
         # remember quadrature weights
         self.register_buffer('weights', weights, persistent=False)
 
     def extra_repr(self):
-        """
+        r"""
         Pretty print module
         """
         return f'nlat={self.nlat}, nlon={self.nlon},\n lmax={self.lmax}, mmax={self.mmax},\n grid={self.grid}, csphase={self.csphase}'
 
     def forward(self, x: torch.Tensor):
 
         assert(x.shape[-2] == self.nlat)
@@ -116,22 +116,22 @@
         # distributed contraction: fork
         out_shape = list(x.size())
         out_shape[-3] = self.lmax
         out_shape[-2] = self.mmax
         xout = torch.zeros(out_shape, dtype=x.dtype, device=x.device)
         
         # contraction
-        xout[..., 0] = torch.einsum('...km,mlk->...lm', x[..., :self.mmax, 0], self.weights )
-        xout[..., 1] = torch.einsum('...km,mlk->...lm', x[..., :self.mmax, 1], self.weights )
+        xout[..., 0] = torch.einsum('...km,mlk->...lm', x[..., :self.mmax, 0], self.weights.to(x.dtype) )
+        xout[..., 1] = torch.einsum('...km,mlk->...lm', x[..., :self.mmax, 1], self.weights.to(x.dtype) )
         x = torch.view_as_complex(xout)
         
         return x
 
 class InverseRealSHT(nn.Module):
-    """
+    r"""
     Defines a module for computing the inverse (real-valued) SHT.
     Precomputes Legendre Gauss nodes, weights and associated Legendre polynomials on these nodes.
     nlat, nlon: Output dimensions
     lmax, mmax: Input dimensions (spherical coefficients). For convenience, these are inferred from the output dimensions
 
     [1] Schaeffer, N. Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations, G3: Geochemistry, Geophysics, Geosystems.
     [2] Wang, B., Wang, L., Xie, Z.; Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids; Adv Comput Math.
@@ -168,50 +168,50 @@
 
         pct = precompute_legpoly(self.mmax, self.lmax, t, norm=self.norm, inverse=True, csphase=self.csphase)
 
         # register buffer
         self.register_buffer('pct', pct, persistent=False)
 
     def extra_repr(self):
-        """
+        r"""
         Pretty print module
         """
         return f'nlat={self.nlat}, nlon={self.nlon},\n lmax={self.lmax}, mmax={self.mmax},\n grid={self.grid}, csphase={self.csphase}'
 
     def forward(self, x: torch.Tensor):
 
         assert(x.shape[-2] == self.lmax)
         assert(x.shape[-1] == self.mmax)
         
         # Evaluate associated Legendre functions on the output nodes
         x = torch.view_as_real(x)
         
-        rl = torch.einsum('...lm, mlk->...km', x[..., 0], self.pct )
-        im = torch.einsum('...lm, mlk->...km', x[..., 1], self.pct )
+        rl = torch.einsum('...lm, mlk->...km', x[..., 0], self.pct.to(x.dtype) )
+        im = torch.einsum('...lm, mlk->...km', x[..., 1], self.pct.to(x.dtype) )
         xs = torch.stack((rl, im), -1)
 
         # apply the inverse (real) FFT
         x = torch.view_as_complex(xs)
         x = torch.fft.irfft(x, n=self.nlon, dim=-1, norm="forward")
 
         return x
 
 
 class RealVectorSHT(nn.Module):
-    """
+    r"""
     Defines a module for computing the forward (real) vector SHT.
     Precomputes Legendre Gauss nodes, weights and associated Legendre polynomials on these nodes.
     The SHT is applied to the last three dimensions of the input.
 
     [1] Schaeffer, N. Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations, G3: Geochemistry, Geophysics, Geosystems.
     [2] Wang, B., Wang, L., Xie, Z.; Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids; Adv Comput Math.
     """
 
     def __init__(self, nlat, nlon, lmax=None, mmax=None, grid="lobatto", norm="ortho", csphase=True):
-        """
+        r"""
         Initializes the vector SHT Layer, precomputing the necessary quadrature weights
 
         Parameters:
         nlat: input grid resolution in the latitudinal direction
         nlon: input grid resolution in the longitudinal direction
         grid: type of grid the data lives on
         """
@@ -255,15 +255,15 @@
         # since the second component is imaginary, we need to take complex conjugation into account
         weights[1] = -1 * weights[1]
 
         # remember quadrature weights
         self.register_buffer('weights', weights, persistent=False)
 
     def extra_repr(self):
-        """
+        r"""
         Pretty print module
         """
         return f'nlat={self.nlat}, nlon={self.nlon},\n lmax={self.lmax}, mmax={self.mmax},\n grid={self.grid}, csphase={self.csphase}'
 
     def forward(self, x: torch.Tensor):
 
         assert(len(x.shape) >= 3)
@@ -278,34 +278,34 @@
         out_shape = list(x.size())
         out_shape[-3] = self.lmax
         out_shape[-2] = self.mmax
         xout = torch.zeros(out_shape, dtype=x.dtype, device=x.device)
 
         # contraction - spheroidal component
         # real component
-        xout[..., 0, :, :, 0] =   torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 0], self.weights[0]) \
-                                - torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 1], self.weights[1]) 
+        xout[..., 0, :, :, 0] =   torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 0], self.weights[0].to(x.dtype)) \
+                                - torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 1], self.weights[1].to(x.dtype)) 
 
         # iamg component
-        xout[..., 0, :, :, 1] =   torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 1], self.weights[0]) \
-                                + torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 0], self.weights[1]) 
+        xout[..., 0, :, :, 1] =   torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 1], self.weights[0].to(x.dtype)) \
+                                + torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 0], self.weights[1].to(x.dtype)) 
 
         # contraction - toroidal component
         # real component
-        xout[..., 1, :, :, 0] = - torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 1], self.weights[1]) \
-                                - torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 0], self.weights[0]) 
+        xout[..., 1, :, :, 0] = - torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 1], self.weights[1].to(x.dtype)) \
+                                - torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 0], self.weights[0].to(x.dtype)) 
         # imag component
-        xout[..., 1, :, :, 1] =   torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 0], self.weights[1]) \
-                                - torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 1], self.weights[0]) 
+        xout[..., 1, :, :, 1] =   torch.einsum('...km,mlk->...lm', x[..., 0, :, :self.mmax, 0], self.weights[1].to(x.dtype)) \
+                                - torch.einsum('...km,mlk->...lm', x[..., 1, :, :self.mmax, 1], self.weights[0].to(x.dtype)) 
 
         return torch.view_as_complex(xout)
 
 
 class InverseRealVectorSHT(nn.Module):
-    """
+    r"""
     Defines a module for computing the inverse (real-valued) vector SHT.
     Precomputes Legendre Gauss nodes, weights and associated Legendre polynomials on these nodes.
     
     [1] Schaeffer, N. Efficient spherical harmonic transforms aimed at pseudospectral numerical simulations, G3: Geochemistry, Geophysics, Geosystems.
     [2] Wang, B., Wang, L., Xie, Z.; Accurate calculation of spherical and vector spherical harmonic expansions via spectral element grids; Adv Comput Math.
     """
     def __init__(self, nlat, nlon, lmax=None, mmax=None, grid="lobatto", norm="ortho", csphase=True):
@@ -339,42 +339,42 @@
 
         dpct = precompute_dlegpoly(self.mmax, self.lmax, t, norm=self.norm, inverse=True, csphase=self.csphase)
 
         # register weights
         self.register_buffer('dpct', dpct, persistent=False)
 
     def extra_repr(self):
-        """
+        r"""
         Pretty print module
         """
         return f'nlat={self.nlat}, nlon={self.nlon},\n lmax={self.lmax}, mmax={self.mmax},\n grid={self.grid}, csphase={self.csphase}'
 
     def forward(self, x: torch.Tensor):
 
         assert(x.shape[-2] == self.lmax)
         assert(x.shape[-1] == self.mmax)
         
         # Evaluate associated Legendre functions on the output nodes
         x = torch.view_as_real(x)
 
         # contraction - spheroidal component
         # real component
-        srl =   torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 0], self.dpct[0]) \
-              - torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 1], self.dpct[1]) 
+        srl =   torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 0], self.dpct[0].to(x.dtype)) \
+              - torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 1], self.dpct[1].to(x.dtype)) 
         # iamg component
-        sim =   torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 1], self.dpct[0]) \
-              + torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 0], self.dpct[1]) 
+        sim =   torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 1], self.dpct[0].to(x.dtype)) \
+              + torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 0], self.dpct[1].to(x.dtype)) 
 
         # contraction - toroidal component
         # real component
-        trl = - torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 1], self.dpct[1]) \
-              - torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 0], self.dpct[0]) 
+        trl = - torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 1], self.dpct[1].to(x.dtype)) \
+              - torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 0], self.dpct[0].to(x.dtype)) 
         # imag component
-        tim =   torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 0], self.dpct[1]) \
-              - torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 1], self.dpct[0]) 
+        tim =   torch.einsum('...lm,mlk->...km', x[..., 0, :, :, 0], self.dpct[1].to(x.dtype)) \
+              - torch.einsum('...lm,mlk->...km', x[..., 1, :, :, 1], self.dpct[0].to(x.dtype)) 
         
         # reassemble
         s = torch.stack((srl, sim), -1)
         t = torch.stack((trl, tim), -1)
         xs = torch.stack((s, t), -4)
 
         # apply the inverse (real) FFT
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics/test_torch_harmonics.py` & `torch_harmonics-0.6.2/torch_harmonics/tests.py`

 * *Files identical despite different names*

### Comparing `torch_harmonics-0.6.1/torch_harmonics.egg-info/PKG-INFO` & `torch_harmonics-0.6.2/torch_harmonics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-harmonics
-Version: 0.6.1
+Version: 0.6.2
 Summary: A differentiable spherical harmonic transform for PyTorch.
 Home-page: https://github.com/NVIDIA/torch-harmonics
 License: Modified BSD
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -40,33 +40,40 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 -->
 
 <p align="center">
-    <img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/logo/logo.png"  width="568">
+    <img src="https://raw.githubusercontent.com/NVIDIA/torch-harmonics/main/images/logo/logo.png"  width="568">
+    <br>
+    <a href="https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml"><img src="https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml/badge.svg"></a>
+    <a href="https://pypi.org/project/torch_harmonics/"><img src="https://img.shields.io/pypi/v/torch_harmonics"></a>
 </p>
 
+<!--
+[![pypi](https://img.shields.io/pypi/v/torch_harmonics)](https://pypi.org/project/torch_harmonics/)
+-->
+
 <!-- # torch-harmonics: differentiable harmonic transforms -->
 
 <!-- ## What is torch-harmonics? -->
 
-`torch_harmonics` is a differentiable implementation of the Spherical Harmonic transform in PyTorch. It was originally implemented to enable Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute the projection onto the associated Legendre polynomials and FFTs for the projection onto the harmonic basis. This algorithm tends to outperform others with better asymptotic scaling for most practical purposes.
+`torch-harmonics` is a differentiable implementation of the Spherical Harmonic transform in PyTorch. It was originally implemented to enable Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute the projection onto the associated Legendre polynomials and FFTs for the projection onto the harmonic basis. This algorithm tends to outperform others with better asymptotic scaling for most practical purposes.
 
-`torch_harmonics` uses PyTorch primitives to implement these operations, making it fully differentiable. Moreover, the quadrature can be distributed onto multiple ranks making it spatially distributed.
+`torch-harmonics` uses PyTorch primitives to implement these operations, making it fully differentiable. Moreover, the quadrature can be distributed onto multiple ranks making it spatially distributed.
 
-`torch_harmonics` has been used to implement a variety of differentiable PDE solvers which generated the animations below. Moreover, it has enabled the development of Spherical Fourier Neural Operators (SFNOs) [1].
+`torch-harmonics` has been used to implement a variety of differentiable PDE solvers which generated the animations below. Moreover, it has enabled the development of Spherical Fourier Neural Operators (SFNOs) [1].
 
 
 <table border="0" cellspacing="0" cellpadding="0">
     <tr>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/sfno.gif"  width="240"></td>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/zonal_jet.gif"  width="240"></td>
-        <td><img src="https://github.com/NVIDIA/torch-harmonics/blob/main/images/allen-cahn.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/sfno.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/zonal_jet.gif"  width="240"></td>
+        <td><img src="https://media.githubusercontent.com/media/NVIDIA/torch-harmonics/main/images/allen-cahn.gif"  width="240"></td>
     </tr>
 <!--     <tr>
         <td style="text-align:center; border-style : hidden!important;">Shallow Water Eqns.</td>
         <td style="text-align:center; border-style : hidden!important;">Ginzburg-Landau Eqn.</td>
         <td style="text-align:center; border-style : hidden!important;">Allen-Cahn Eqn.</td>
     </tr>  -->
 </table>
@@ -79,22 +86,23 @@
 pip install torch-harmonics
 ```
 
 Build in your environment using the Python package:
 
 ```
 git clone git@github.com:NVIDIA/torch-harmonics.git
-pip install ./torch_harmonics
+cd torch-harmonics
+pip install -e .
 ```
 
 Alternatively, use the Dockerfile to build your custom container after cloning:
 
 ```
 git clone git@github.com:NVIDIA/torch-harmonics.git
-cd torch_harmonics
+cd torch-harmonics
 docker build . -t torch_harmonics
 docker run --gpus all -it --rm --ipc=host --ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics
 ```
 
 ## Contributors
 
  - Boris Bonev (bbonev@nvidia.com)
@@ -158,20 +166,20 @@
 
 nlat = 512
 nlon = 2*nlat
 batch_size = 32
 signal = torch.randn(batch_size, nlat, nlon)
 
 # transform data on an equiangular grid
-sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device).float()
+sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device)
 
 coeffs = sht(signal)
 ```
 
-`torch_harmonics` also implements a distributed variant of the SHT located in `torch-harmonics.distributed`.
+To enable scalable model-parallelism, `torch-harmonics` implements a distributed variant of the SHT located in `torch_harmonics.distributed`.
 
 ### Cite us
 
 If you use `torch-harmonics` in an academic paper, please cite [1]
 
 ```
 @misc{bonev2023spherical,
```

#### html2text {}

```diff
@@ -1,70 +1,74 @@
-Metadata-Version: 2.1 Name: torch-harmonics Version: 0.6.1 Summary: A
+Metadata-Version: 2.1 Name: torch-harmonics Version: 0.6.2 Summary: A
 differentiable spherical harmonic transform for PyTorch. Home-page: https://
 github.com/NVIDIA/torch-harmonics License: Modified BSD Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering Classifier: License :: OSI Approved
 :: BSD License Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown Provides-Extra: sfno License-File: LICENSE License-
 File: AUTHORS
-  [https://github.com/NVIDIA/torch-harmonics/blob/main/images/logo/logo.png]
-  `torch_harmonics` is a differentiable implementation of the Spherical
+  [https://raw.githubusercontent.com/NVIDIA/torch-harmonics/main/images/logo/
+                                  logo.png]
+    [https://github.com/NVIDIA/torch-harmonics/actions/workflows/tests.yml/
+          badge.svg] [https://img.shields.io/pypi/v/torch_harmonics]
+   `torch-harmonics` is a differentiable implementation of the Spherical
 Harmonic transform in PyTorch. It was originally implemented to enable
 Spherical Fourier Neural Operators (SFNO). It uses quadrature rules to compute
 the projection onto the associated Legendre polynomials and FFTs for the
 projection onto the harmonic basis. This algorithm tends to outperform others
-with better asymptotic scaling for most practical purposes. `torch_harmonics`
+with better asymptotic scaling for most practical purposes. `torch-harmonics`
 uses PyTorch primitives to implement these operations, making it fully
 differentiable. Moreover, the quadrature can be distributed onto multiple ranks
-making it spatially distributed. `torch_harmonics` has been used to implement a
+making it spatially distributed. `torch-harmonics` has been used to implement a
 variety of differentiable PDE solvers which generated the animations below.
 Moreover, it has enabled the development of Spherical Fourier Neural Operators
 (SFNOs) [1].
-[https://github.com/       [https://github.com/    [https://github.com/NVIDIA/
-NVIDIA/torch-harmonics/    NVIDIA/torch-harmonics/ torch-harmonics/blob/main/
-blob/main/images/sfno.gif] blob/main/images/       images/allen-cahn.gif]
-                           zonal_jet.gif]
+[https://                    [https://                    [https://
+media.githubusercontent.com/ media.githubusercontent.com/ media.githubusercontent.com/
+media/NVIDIA/torch-          media/NVIDIA/torch-          media/NVIDIA/torch-
+harmonics/main/images/       harmonics/main/images/       harmonics/main/images/allen-
+sfno.gif]                    zonal_jet.gif]               cahn.gif]
 ## Installation Download directyly from PyPI: ``` pip install torch-harmonics
 ``` Build in your environment using the Python package: ``` git clone
-git@github.com:NVIDIA/torch-harmonics.git pip install ./torch_harmonics ```
-Alternatively, use the Dockerfile to build your custom container after cloning:
-``` git clone git@github.com:NVIDIA/torch-harmonics.git cd torch_harmonics
-docker build . -t torch_harmonics docker run --gpus all -it --rm --ipc=host --
-ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics ``` ## Contributors -
-Boris Bonev (bbonev@nvidia.com) - Thorsten Kurth (tkurth@nvidia.com) -
-Christian Hundt (chundt@nvidia.com) - Nikola Kovachki (nkovachki@nvidia.com) -
-Jean Kossaifi (jkossaifi@nvidia.com) ## Implementation The implementation
-follows the algorithm as presented in [2]. ### Spherical harmonic transform The
-truncated series expansion of a function $f$ defined on the surface of a sphere
-can be written as $$ f(\theta, \lambda) = \sum_{m=-M}^{M} \exp(im\lambda) \sum_
-{n=|m|}^{M} F_n^m \bar{P}_n^m (\cos \theta), $$ where $\theta$ is the
-colatitude, $\lambda$ the longitude, $\bar{P}_n^m$ the normalized, associated
-Legendre polynomials and $F_n^m$, the expansion coefficient associated to the
-mode $(m,n)$. A direct spherical harmonic transform can be accomplished by a
-Fourier transform $$ F^m(\theta) = \frac{1}{2 \pi} \int_{0}^{2\pi} f(\theta,
-\lambda) \exp(-im\lambda) \mathrm{d}\lambda $$ in longitude and a Legendre
-transform $$ F_n^m = \frac{1}{2} \int_{-1}^1 F^m(\theta) \bar{P}_n^m(\cos
-\theta) \mathrm{d} \cos \theta $$ in latitude. ### Discrete Legendre transform
-in order to apply the Legendre transfor, we shall use Gauss-Legendre points in
-the latitudinal direction. The integral $$ F_n^m = \int_{0}^\pi F^m(\theta)
-\bar{P}_n^m(\cos \theta) \sin \theta \mathrm{d} \theta $$ is approximated by
-the sum $$ F_n^m = \sum_{j=1}^{N_\theta} F^m(\theta_j) \bar{P}_n^m(\cos
-\theta_j) w_j $$ ## Usage ### Getting started The main functionality of
-`torch_harmonics` is provided in the form of `torch.nn.Modules` for
-composability. A minimum example is given by: ```python import torch import
-torch_harmonics as th device = torch.device('cuda' if torch.cuda.is_available()
-else 'cpu') nlat = 512 nlon = 2*nlat batch_size = 32 signal = torch.randn
-(batch_size, nlat, nlon) # transform data on an equiangular grid sht =
-th.RealSHT(nlat, nlon, grid="equiangular").to(device).float() coeffs = sht
-(signal) ``` `torch_harmonics` also implements a distributed variant of the SHT
-located in `torch-harmonics.distributed`. ### Cite us If you use `torch-
-harmonics` in an academic paper, please cite [1] ``` @misc{bonev2023spherical,
-title={Spherical Fourier Neural Operators: Learning Stable Dynamics on the
-Sphere}, author={Boris Bonev and Thorsten Kurth and Christian Hundt and Jaideep
-Pathak and Maximilian Baust and Karthik Kashinath and Anima Anandkumar}, year=
-{2023}, eprint={2306.03838}, archivePrefix={arXiv}, primaryClass={cs.LG} } ```
-## References [1] Bonev B., Kurth T., Hundt C., Pathak, J., Baust M., Kashinath
-K., Anandkumar A.; Spherical Fourier Neural Operators: Learning Stable Dynamics
-on the Sphere; arXiv 2306.0383, 2023. [2] Schaeffer N.; Efficient spherical
-harmonic transforms aimed at pseudospectral numerical simulations; G3:
-Geochemistry, Geophysics, Geosystems, 2013. [3] Wang B., Wang L., Xie Z.;
-Accurate calculation of spherical and vector spherical harmonic expansions via
-spectral element grids; Adv Comput Math, 2018.
+git@github.com:NVIDIA/torch-harmonics.git cd torch-harmonics pip install -e .
+``` Alternatively, use the Dockerfile to build your custom container after
+cloning: ``` git clone git@github.com:NVIDIA/torch-harmonics.git cd torch-
+harmonics docker build . -t torch_harmonics docker run --gpus all -it --rm --
+ipc=host --ulimit memlock=-1 --ulimit stack=67108864 torch_harmonics ``` ##
+Contributors - Boris Bonev (bbonev@nvidia.com) - Thorsten Kurth
+(tkurth@nvidia.com) - Christian Hundt (chundt@nvidia.com) - Nikola Kovachki
+(nkovachki@nvidia.com) - Jean Kossaifi (jkossaifi@nvidia.com) ## Implementation
+The implementation follows the algorithm as presented in [2]. ### Spherical
+harmonic transform The truncated series expansion of a function $f$ defined on
+the surface of a sphere can be written as $$ f(\theta, \lambda) = \sum_{m=-M}^
+{M} \exp(im\lambda) \sum_{n=|m|}^{M} F_n^m \bar{P}_n^m (\cos \theta), $$ where
+$\theta$ is the colatitude, $\lambda$ the longitude, $\bar{P}_n^m$ the
+normalized, associated Legendre polynomials and $F_n^m$, the expansion
+coefficient associated to the mode $(m,n)$. A direct spherical harmonic
+transform can be accomplished by a Fourier transform $$ F^m(\theta) = \frac{1}
+{2 \pi} \int_{0}^{2\pi} f(\theta, \lambda) \exp(-im\lambda) \mathrm{d}\lambda
+$$ in longitude and a Legendre transform $$ F_n^m = \frac{1}{2} \int_{-1}^1 F^m
+(\theta) \bar{P}_n^m(\cos \theta) \mathrm{d} \cos \theta $$ in latitude. ###
+Discrete Legendre transform in order to apply the Legendre transfor, we shall
+use Gauss-Legendre points in the latitudinal direction. The integral $$ F_n^m =
+\int_{0}^\pi F^m(\theta) \bar{P}_n^m(\cos \theta) \sin \theta \mathrm{d} \theta
+$$ is approximated by the sum $$ F_n^m = \sum_{j=1}^{N_\theta} F^m(\theta_j)
+\bar{P}_n^m(\cos \theta_j) w_j $$ ## Usage ### Getting started The main
+functionality of `torch_harmonics` is provided in the form of
+`torch.nn.Modules` for composability. A minimum example is given by: ```python
+import torch import torch_harmonics as th device = torch.device('cuda' if
+torch.cuda.is_available() else 'cpu') nlat = 512 nlon = 2*nlat batch_size = 32
+signal = torch.randn(batch_size, nlat, nlon) # transform data on an equiangular
+grid sht = th.RealSHT(nlat, nlon, grid="equiangular").to(device) coeffs = sht
+(signal) ``` To enable scalable model-parallelism, `torch-harmonics` implements
+a distributed variant of the SHT located in `torch_harmonics.distributed`. ###
+Cite us If you use `torch-harmonics` in an academic paper, please cite [1] ```
+@misc{bonev2023spherical, title={Spherical Fourier Neural Operators: Learning
+Stable Dynamics on the Sphere}, author={Boris Bonev and Thorsten Kurth and
+Christian Hundt and Jaideep Pathak and Maximilian Baust and Karthik Kashinath
+and Anima Anandkumar}, year={2023}, eprint={2306.03838}, archivePrefix={arXiv},
+primaryClass={cs.LG} } ``` ## References [1] Bonev B., Kurth T., Hundt C.,
+Pathak, J., Baust M., Kashinath K., Anandkumar A.; Spherical Fourier Neural
+Operators: Learning Stable Dynamics on the Sphere; arXiv 2306.0383, 2023. [2]
+Schaeffer N.; Efficient spherical harmonic transforms aimed at pseudospectral
+numerical simulations; G3: Geochemistry, Geophysics, Geosystems, 2013. [3] Wang
+B., Wang L., Xie Z.; Accurate calculation of spherical and vector spherical
+harmonic expansions via spectral element grids; Adv Comput Math, 2018.
```

### Comparing `torch_harmonics-0.6.1/torch_harmonics.egg-info/SOURCES.txt` & `torch_harmonics-0.6.2/torch_harmonics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 tests/test_distributed_backward_transform.py
 tests/test_distributed_forward_transform.py
 torch_harmonics/__init__.py
 torch_harmonics/legendre.py
 torch_harmonics/quadrature.py
 torch_harmonics/random_fields.py
 torch_harmonics/sht.py
-torch_harmonics/test_torch_harmonics.py
+torch_harmonics/tests.py
 torch_harmonics.egg-info/PKG-INFO
 torch_harmonics.egg-info/SOURCES.txt
 torch_harmonics.egg-info/dependency_links.txt
 torch_harmonics.egg-info/requires.txt
 torch_harmonics.egg-info/top_level.txt
 torch_harmonics/distributed/__init__.py
 torch_harmonics/distributed/distributed_sht.py
```

