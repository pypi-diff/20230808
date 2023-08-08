# Comparing `tmp/gpjax-0.6.7.tar.gz` & `tmp/gpjax-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpjax-0.6.7.tar", max compression
+gzip compressed data, was "gpjax-0.6.8.tar", max compression
```

## Comparing `gpjax-0.6.7.tar` & `gpjax-0.6.8.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0    11357 2023-06-24 11:03:02.854511 gpjax-0.6.7/LICENSE
--rw-r--r--   0        0        0     7471 2023-06-24 11:03:02.854717 gpjax-0.6.7/README.md
--rw-r--r--   0        0        0     3030 2023-06-24 11:03:02.895374 gpjax-0.6.7/gpjax/__init__.py
--rw-r--r--   0        0        0     3030 2023-06-24 14:10:44.518544 gpjax-0.6.7/gpjax/__init__.py.7db73aa22d01f7c08551d972cc1ef366.tmp
--rw-r--r--   0        0        0     1068 2023-06-24 11:03:02.895569 gpjax-0.6.7/gpjax/base/__init__.py
--rw-r--r--   0        0        0    12487 2023-06-24 11:03:02.895888 gpjax-0.6.7/gpjax/base/module.py
--rw-r--r--   0        0        0     2271 2023-06-24 11:03:02.895995 gpjax-0.6.7/gpjax/base/param.py
--rw-r--r--   0        0        0     5078 2023-06-24 11:03:02.896105 gpjax-0.6.7/gpjax/citation.py
--rw-r--r--   0        0        0     3452 2023-06-24 11:03:02.896217 gpjax-0.6.7/gpjax/dataset.py
--rw-r--r--   0        0        0     8216 2023-06-24 11:03:02.896347 gpjax-0.6.7/gpjax/fit.py
--rw-r--r--   0        0        0     9121 2023-06-24 11:03:02.896479 gpjax-0.6.7/gpjax/gaussian_distribution.py
--rw-r--r--   0        0        0    29097 2023-06-24 11:03:02.896666 gpjax-0.6.7/gpjax/gps.py
--rw-r--r--   0        0        0     5701 2023-06-24 11:03:02.896795 gpjax-0.6.7/gpjax/integrators.py
--rw-r--r--   0        0        0     1815 2023-06-24 11:03:02.896966 gpjax-0.6.7/gpjax/kernels/__init__.py
--rw-r--r--   0        0        0       68 2023-06-24 11:03:02.897139 gpjax-0.6.7/gpjax/kernels/approximations/__init__.py
--rw-r--r--   0        0        0     3274 2023-06-24 11:03:02.897261 gpjax-0.6.7/gpjax/kernels/approximations/rff.py
--rw-r--r--   0        0        0     6680 2023-06-24 11:03:02.897380 gpjax-0.6.7/gpjax/kernels/base.py
--rw-r--r--   0        0        0     1379 2023-06-24 11:03:02.897543 gpjax-0.6.7/gpjax/kernels/computations/__init__.py
--rw-r--r--   0        0        0     2585 2023-06-24 11:03:02.897665 gpjax-0.6.7/gpjax/kernels/computations/base.py
--rw-r--r--   0        0        0     2411 2023-06-24 11:03:02.897759 gpjax-0.6.7/gpjax/kernels/computations/basis_functions.py
--rw-r--r--   0        0        0     2830 2023-06-24 11:03:02.897840 gpjax-0.6.7/gpjax/kernels/computations/constant_diagonal.py
--rw-r--r--   0        0        0     1661 2023-06-24 11:03:02.897929 gpjax-0.6.7/gpjax/kernels/computations/dense.py
--rw-r--r--   0        0        0     2383 2023-06-24 11:03:02.898024 gpjax-0.6.7/gpjax/kernels/computations/diagonal.py
--rw-r--r--   0        0        0     2165 2023-06-24 11:03:02.898126 gpjax-0.6.7/gpjax/kernels/computations/eigen.py
--rw-r--r--   0        0        0      790 2023-06-24 11:03:02.898270 gpjax-0.6.7/gpjax/kernels/non_euclidean/__init__.py
--rw-r--r--   0        0        0     3511 2023-06-24 11:03:02.898391 gpjax-0.6.7/gpjax/kernels/non_euclidean/graph.py
--rw-r--r--   0        0        0     1620 2023-06-24 11:03:02.898489 gpjax-0.6.7/gpjax/kernels/non_euclidean/utils.py
--rw-r--r--   0        0        0      930 2023-06-24 11:03:02.898617 gpjax-0.6.7/gpjax/kernels/nonstationary/__init__.py
--rw-r--r--   0        0        0     4078 2023-06-24 11:03:02.898731 gpjax-0.6.7/gpjax/kernels/nonstationary/arccosine.py
--rw-r--r--   0        0        0     2016 2023-06-24 11:03:02.898850 gpjax-0.6.7/gpjax/kernels/nonstationary/linear.py
--rw-r--r--   0        0        0     2384 2023-06-24 11:03:02.898995 gpjax-0.6.7/gpjax/kernels/nonstationary/polynomial.py
--rw-r--r--   0        0        0     1323 2023-06-24 11:03:02.899124 gpjax-0.6.7/gpjax/kernels/stationary/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-24 11:03:02.899238 gpjax-0.6.7/gpjax/kernels/stationary/matern12.py
--rw-r--r--   0        0        0     2723 2023-06-24 11:03:02.899325 gpjax-0.6.7/gpjax/kernels/stationary/matern32.py
--rw-r--r--   0        0        0     2792 2023-06-24 11:03:02.899402 gpjax-0.6.7/gpjax/kernels/stationary/matern52.py
--rw-r--r--   0        0        0     2420 2023-06-24 11:03:02.899487 gpjax-0.6.7/gpjax/kernels/stationary/periodic.py
--rw-r--r--   0        0        0     2674 2023-06-24 11:03:02.899592 gpjax-0.6.7/gpjax/kernels/stationary/powered_exponential.py
--rw-r--r--   0        0        0     2389 2023-06-24 11:03:02.899708 gpjax-0.6.7/gpjax/kernels/stationary/rational_quadratic.py
--rw-r--r--   0        0        0     2440 2023-06-24 11:03:02.899818 gpjax-0.6.7/gpjax/kernels/stationary/rbf.py
--rw-r--r--   0        0        0     2226 2023-06-24 11:03:02.899918 gpjax-0.6.7/gpjax/kernels/stationary/utils.py
--rw-r--r--   0        0        0     2072 2023-06-24 11:03:02.900031 gpjax-0.6.7/gpjax/kernels/stationary/white.py
--rw-r--r--   0        0        0     8015 2023-06-24 11:03:02.900168 gpjax-0.6.7/gpjax/likelihoods.py
--rw-r--r--   0        0        0     1609 2023-06-24 11:03:02.900320 gpjax-0.6.7/gpjax/linops/__init__.py
--rw-r--r--   0        0        0     6259 2023-06-24 11:03:02.900443 gpjax-0.6.7/gpjax/linops/constant_diagonal_linear_operator.py
--rw-r--r--   0        0        0     6201 2023-06-24 11:03:02.900586 gpjax-0.6.7/gpjax/linops/dense_linear_operator.py
--rw-r--r--   0        0        0     7179 2023-06-24 11:03:02.900698 gpjax-0.6.7/gpjax/linops/diagonal_linear_operator.py
--rw-r--r--   0        0        0     3607 2023-06-24 11:03:02.900799 gpjax-0.6.7/gpjax/linops/identity_linear_operator.py
--rw-r--r--   0        0        0     7131 2023-06-24 11:03:02.900917 gpjax-0.6.7/gpjax/linops/linear_operator.py
--rw-r--r--   0        0        0     3187 2023-06-24 11:03:02.901049 gpjax-0.6.7/gpjax/linops/triangular_linear_operator.py
--rw-r--r--   0        0        0     3443 2023-06-24 11:03:02.901152 gpjax-0.6.7/gpjax/linops/utils.py
--rw-r--r--   0        0        0     5939 2023-06-24 11:03:02.901255 gpjax-0.6.7/gpjax/linops/zero_linear_operator.py
--rw-r--r--   0        0        0     6081 2023-06-24 11:03:02.901409 gpjax-0.6.7/gpjax/mean_functions.py
--rw-r--r--   0        0        0    14868 2023-06-24 11:03:02.901579 gpjax-0.6.7/gpjax/objectives.py
--rw-r--r--   0        0        0     4407 2023-06-24 11:03:02.901686 gpjax-0.6.7/gpjax/progress_bar.py
--rw-r--r--   0        0        0     5506 2023-06-24 11:03:02.901809 gpjax-0.6.7/gpjax/scan.py
--rw-r--r--   0        0        0     1694 2023-06-24 11:03:02.901918 gpjax-0.6.7/gpjax/typing.py
--rw-r--r--   0        0        0    26453 2023-06-24 11:03:02.902143 gpjax-0.6.7/gpjax/variational_families.py
--rw-r--r--   0        0        0     5302 2023-06-24 14:10:29.233467 gpjax-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 gpjax-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 19:04:23.359578 gpjax-0.6.8/LICENSE
+-rw-r--r--   0        0        0     7616 2023-08-08 18:07:36.172397 gpjax-0.6.8/README.md
+-rw-r--r--   0        0        0     3030 2023-08-08 18:08:37.046840 gpjax-0.6.8/gpjax/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-30 19:04:23.413913 gpjax-0.6.8/gpjax/base/__init__.py
+-rw-r--r--   0        0        0    12487 2023-06-18 06:38:02.950803 gpjax-0.6.8/gpjax/base/module.py
+-rw-r--r--   0        0        0     2271 2023-06-18 06:38:02.951225 gpjax-0.6.8/gpjax/base/param.py
+-rw-r--r--   0        0        0     5078 2023-06-22 21:16:21.055892 gpjax-0.6.8/gpjax/citation.py
+-rw-r--r--   0        0        0     4193 2023-08-08 18:07:36.183898 gpjax-0.6.8/gpjax/dataset.py
+-rw-r--r--   0        0        0     8216 2023-06-22 20:51:02.847293 gpjax-0.6.8/gpjax/fit.py
+-rw-r--r--   0        0        0     9121 2023-06-18 06:38:02.953908 gpjax-0.6.8/gpjax/gaussian_distribution.py
+-rw-r--r--   0        0        0    28950 2023-08-08 18:07:36.184456 gpjax-0.6.8/gpjax/gps.py
+-rw-r--r--   0        0        0     5701 2023-06-22 21:16:21.057438 gpjax-0.6.8/gpjax/integrators.py
+-rw-r--r--   0        0        0     1843 2023-08-08 18:07:36.184753 gpjax-0.6.8/gpjax/kernels/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-30 19:04:23.415113 gpjax-0.6.8/gpjax/kernels/approximations/__init__.py
+-rw-r--r--   0        0        0     3333 2023-08-08 18:07:36.185149 gpjax-0.6.8/gpjax/kernels/approximations/rff.py
+-rw-r--r--   0        0        0     6651 2023-08-08 18:07:36.185844 gpjax-0.6.8/gpjax/kernels/base.py
+-rw-r--r--   0        0        0     1379 2023-05-30 19:04:23.415474 gpjax-0.6.8/gpjax/kernels/computations/__init__.py
+-rw-r--r--   0        0        0     2877 2023-08-08 18:07:36.186008 gpjax-0.6.8/gpjax/kernels/computations/base.py
+-rw-r--r--   0        0        0     2944 2023-08-08 18:07:36.186163 gpjax-0.6.8/gpjax/kernels/computations/basis_functions.py
+-rw-r--r--   0        0        0     3145 2023-08-08 18:07:36.186291 gpjax-0.6.8/gpjax/kernels/computations/constant_diagonal.py
+-rw-r--r--   0        0        0     1839 2023-08-08 18:07:36.186431 gpjax-0.6.8/gpjax/kernels/computations/dense.py
+-rw-r--r--   0        0        0     2617 2023-08-08 18:07:36.186558 gpjax-0.6.8/gpjax/kernels/computations/diagonal.py
+-rw-r--r--   0        0        0     2272 2023-08-08 18:07:36.186695 gpjax-0.6.8/gpjax/kernels/computations/eigen.py
+-rw-r--r--   0        0        0      865 2023-08-08 18:07:36.186860 gpjax-0.6.8/gpjax/kernels/non_euclidean/__init__.py
+-rw-r--r--   0        0        0     5334 2023-08-08 18:07:36.186985 gpjax-0.6.8/gpjax/kernels/non_euclidean/categorical.py
+-rw-r--r--   0        0        0     3539 2023-08-08 18:07:36.187134 gpjax-0.6.8/gpjax/kernels/non_euclidean/graph.py
+-rw-r--r--   0        0        0     1620 2023-06-18 06:38:02.972061 gpjax-0.6.8/gpjax/kernels/non_euclidean/utils.py
+-rw-r--r--   0        0        0      930 2023-05-30 19:04:23.416456 gpjax-0.6.8/gpjax/kernels/nonstationary/__init__.py
+-rw-r--r--   0        0        0     4078 2023-06-18 06:38:02.972634 gpjax-0.6.8/gpjax/kernels/nonstationary/arccosine.py
+-rw-r--r--   0        0        0     2016 2023-06-18 06:38:02.973171 gpjax-0.6.8/gpjax/kernels/nonstationary/linear.py
+-rw-r--r--   0        0        0     2384 2023-06-18 06:38:02.973519 gpjax-0.6.8/gpjax/kernels/nonstationary/polynomial.py
+-rw-r--r--   0        0        0     1323 2023-05-30 19:04:23.416936 gpjax-0.6.8/gpjax/kernels/stationary/__init__.py
+-rw-r--r--   0        0        0     2522 2023-08-08 18:07:36.187346 gpjax-0.6.8/gpjax/kernels/stationary/matern12.py
+-rw-r--r--   0        0        0     2708 2023-08-08 18:07:36.187474 gpjax-0.6.8/gpjax/kernels/stationary/matern32.py
+-rw-r--r--   0        0        0     2792 2023-06-18 06:38:02.974170 gpjax-0.6.8/gpjax/kernels/stationary/matern52.py
+-rw-r--r--   0        0        0     2479 2023-08-08 18:07:36.187644 gpjax-0.6.8/gpjax/kernels/stationary/periodic.py
+-rw-r--r--   0        0        0     2674 2023-06-22 21:16:21.058450 gpjax-0.6.8/gpjax/kernels/stationary/powered_exponential.py
+-rw-r--r--   0        0        0     2389 2023-06-18 06:38:02.975157 gpjax-0.6.8/gpjax/kernels/stationary/rational_quadratic.py
+-rw-r--r--   0        0        0     2442 2023-08-08 18:07:36.187775 gpjax-0.6.8/gpjax/kernels/stationary/rbf.py
+-rw-r--r--   0        0        0     2226 2023-06-18 06:38:02.975520 gpjax-0.6.8/gpjax/kernels/stationary/utils.py
+-rw-r--r--   0        0        0     2086 2023-08-08 18:07:36.187939 gpjax-0.6.8/gpjax/kernels/stationary/white.py
+-rw-r--r--   0        0        0     8015 2023-06-22 21:16:21.058918 gpjax-0.6.8/gpjax/likelihoods.py
+-rw-r--r--   0        0        0     1609 2023-05-30 19:04:23.417969 gpjax-0.6.8/gpjax/linops/__init__.py
+-rw-r--r--   0        0        0     6259 2023-06-18 06:38:02.976793 gpjax-0.6.8/gpjax/linops/constant_diagonal_linear_operator.py
+-rw-r--r--   0        0        0     6201 2023-06-18 06:38:02.977233 gpjax-0.6.8/gpjax/linops/dense_linear_operator.py
+-rw-r--r--   0        0        0     7179 2023-06-18 06:38:02.977702 gpjax-0.6.8/gpjax/linops/diagonal_linear_operator.py
+-rw-r--r--   0        0        0     3607 2023-06-18 06:38:02.978023 gpjax-0.6.8/gpjax/linops/identity_linear_operator.py
+-rw-r--r--   0        0        0     7131 2023-06-18 06:38:02.978352 gpjax-0.6.8/gpjax/linops/linear_operator.py
+-rw-r--r--   0        0        0     3187 2023-06-18 06:38:02.978857 gpjax-0.6.8/gpjax/linops/triangular_linear_operator.py
+-rw-r--r--   0        0        0     3443 2023-06-18 06:38:02.979139 gpjax-0.6.8/gpjax/linops/utils.py
+-rw-r--r--   0        0        0     5939 2023-06-18 06:38:02.979349 gpjax-0.6.8/gpjax/linops/zero_linear_operator.py
+-rw-r--r--   0        0        0     6081 2023-06-22 21:16:21.059208 gpjax-0.6.8/gpjax/mean_functions.py
+-rw-r--r--   0        0        0    14868 2023-06-22 21:16:21.059539 gpjax-0.6.8/gpjax/objectives.py
+-rw-r--r--   0        0        0     4407 2023-06-18 06:38:02.980778 gpjax-0.6.8/gpjax/progress_bar.py
+-rw-r--r--   0        0        0     5506 2023-06-18 06:38:02.980992 gpjax-0.6.8/gpjax/scan.py
+-rw-r--r--   0        0        0     1694 2023-06-18 06:38:02.981248 gpjax-0.6.8/gpjax/typing.py
+-rw-r--r--   0        0        0    26453 2023-06-18 06:38:02.982018 gpjax-0.6.8/gpjax/variational_families.py
+-rw-r--r--   0        0        0     5303 2023-08-08 18:08:37.044645 gpjax-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     8951 1970-01-01 00:00:00.000000 gpjax-0.6.8/setup.py
+-rw-r--r--   0        0        0     8837 1970-01-01 00:00:00.000000 gpjax-0.6.8/PKG-INFO
```

### Comparing `gpjax-0.6.7/LICENSE` & `gpjax-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/README.md` & `gpjax-0.6.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,
 the maintenance of GPJax is undertaken by [Thomas
 Pinder](https://github.com/thomaspinder) and [Daniel
 Dodd](https://github.com/Daniel-Dodd).
 
 We would be delighted to receive contributions from interested individuals and
 groups. To learn how you can get involved, please read our [guide for
-contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).
+contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/main/docs/contributing.md).
 If you have any questions, we encourage you to [open an
 issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For
 broader conversations, such as best GP fitting practices or questions about the
 mathematics of GPs, we invite you to [open a
 discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
 
 Feel free to join our [Slack
@@ -50,28 +50,29 @@
 
 > - [**Conjugate Inference**](https://docs.jaxgaussianprocesses.com/examples/regression/)
 > - [**Classification with MCMC**](https://docs.jaxgaussianprocesses.com/examples/classification/)
 > - [**Sparse Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/collapsed_vi/)
 > - [**Stochastic Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/uncollapsed_vi/)
 > - [**BlackJax Integration**](https://docs.jaxgaussianprocesses.com/examples/classification/#mcmc-inference)
 > - [**Laplace Approximation**](https://docs.jaxgaussianprocesses.com/examples/classification/#laplace-approximation)
-> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/constructing_new_kernels/#custom-kernel)
 > - [**Inference on Graphs**](https://docs.jaxgaussianprocesses.com/examples/graph_kernels/)
 > - [**Pathwise Sampling**](https://docs.jaxgaussianprocesses.com/examples/spatial/)
 > - [**Learning Gaussian Process Barycentres**](https://docs.jaxgaussianprocesses.com/examples/barycentres/)
 > - [**Deep Kernel Regression**](https://docs.jaxgaussianprocesses.com/examples/deep_kernels/)
 > - [**Poisson Regression**](https://docs.jaxgaussianprocesses.com/examples/poisson/)
+> - [**Bayesian Optimisation**](https://docs.jaxgaussianprocesses.com/examples/bayesian_optimisation/)
 
 ## Guides for customisation
 >
-> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/constructing_new_kernels/#custom-kernel)
 > - [**UCI regression**](https://docs.jaxgaussianprocesses.com/examples/yacht/)
 
 ## Conversion between `.ipynb` and `.py`
-Above examples are stored in [examples](examples) directory in the double
+Above examples are stored in [examples](docs/examples) directory in the double
 percent (`py:percent`) format. Checkout [jupytext
 using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more
 info.
 
 * To convert `example.py` to `example.ipynb`, run:
 
 ```bash
```

### Comparing `gpjax-0.6.7/gpjax/__init__.py` & `gpjax-0.6.8/gpjax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     WhitenedVariationalGaussian,
 )
 
 __license__ = "MIT"
 __description__ = "Didactic Gaussian processes in JAX"
 __url__ = "https://github.com/JaxGaussianProcesses/GPJax"
 __contributors__ = "https://github.com/JaxGaussianProcesses/GPJax/graphs/contributors"
-__version__ = "0.0.0"
+__version__ = "0.6.8"
 
 __all__ = [
     "Module",
     "param_field",
     "cite",
     "kernels",
     "fit",
```

### Comparing `gpjax-0.6.7/gpjax/__init__.py.7db73aa22d01f7c08551d972cc1ef366.tmp` & `gpjax-0.6.8/gpjax/kernels/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,66 @@
-# Copyright 2022 The GPJax Contributors. All Rights Reserved.
+# Copyright 2022 The JaxGaussianProcesses Contributors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from gpjax import integrators
-from gpjax.base import (
-    Module,
-    param_field,
-)
-from gpjax.citation import cite
-from gpjax.dataset import Dataset
-from gpjax.fit import fit
-from gpjax.gps import (
-    Prior,
-    construct_posterior,
-)
-from gpjax.kernels import (
-    RBF,
-    RFF,
+
+"""JaxKern."""
+from gpjax.kernels.approximations import RFF
+from gpjax.kernels.base import (
     AbstractKernel,
+    ProductKernel,
+    SumKernel,
+)
+from gpjax.kernels.computations import (
     BasisFunctionComputation,
     ConstantDiagonalKernelComputation,
     DenseKernelComputation,
     DiagonalKernelComputation,
     EigenKernelComputation,
-    GraphKernel,
+)
+from gpjax.kernels.non_euclidean import GraphKernel, CatKernel
+from gpjax.kernels.nonstationary import (
+    ArcCosine,
     Linear,
+    Polynomial,
+)
+from gpjax.kernels.stationary import (
+    RBF,
     Matern12,
     Matern32,
     Matern52,
     Periodic,
-    Polynomial,
     PoweredExponential,
-    ProductKernel,
     RationalQuadratic,
-    SumKernel,
     White,
 )
-from gpjax.likelihoods import (
-    Bernoulli,
-    Gaussian,
-    Poisson,
-)
-from gpjax.mean_functions import (
-    Constant,
-    Zero,
-)
-from gpjax.objectives import (
-    ELBO,
-    CollapsedELBO,
-    ConjugateMLL,
-    LogPosteriorDensity,
-    NonConjugateMLL,
-)
-from gpjax.variational_families import (
-    CollapsedVariationalGaussian,
-    ExpectationVariationalGaussian,
-    NaturalVariationalGaussian,
-    VariationalGaussian,
-    WhitenedVariationalGaussian,
-)
-
-__license__ = "MIT"
-__description__ = "Didactic Gaussian processes in JAX"
-__url__ = "https://github.com/JaxGaussianProcesses/GPJax"
-__contributors__ = "https://github.com/JaxGaussianProcesses/GPJax/graphs/contributors"
-__version__ = "0.6.7"
 
 __all__ = [
-    "Module",
-    "param_field",
-    "cite",
-    "kernels",
-    "fit",
-    "Prior",
-    "construct_posterior",
-    "integrators",
+    "AbstractKernel",
+    "ArcCosine",
     "RBF",
     "GraphKernel",
+    "CatKernel",
     "Matern12",
     "Matern32",
     "Matern52",
+    "Linear",
     "Polynomial",
     "ProductKernel",
     "SumKernel",
-    "Bernoulli",
-    "Gaussian",
-    "Poisson",
-    "Constant",
-    "Zero",
-    "Dataset",
-    "CollapsedVariationalGaussian",
-    "ExpectationVariationalGaussian",
-    "NaturalVariationalGaussian",
-    "VariationalGaussian",
-    "WhitenedVariationalGaussian",
-    "CollapsedVI",
-    "StochasticVI",
-    "ConjugateMLL",
-    "NonConjugateMLL",
-    "LogPosteriorDensity",
-    "CollapsedELBO",
-    "ELBO",
-    "AbstractKernel",
-    "Linear",
     "DenseKernelComputation",
     "DiagonalKernelComputation",
     "ConstantDiagonalKernelComputation",
     "EigenKernelComputation",
     "PoweredExponential",
     "Periodic",
     "RationalQuadratic",
```

### Comparing `gpjax-0.6.7/gpjax/base/__init__.py` & `gpjax-0.6.8/gpjax/base/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/base/module.py` & `gpjax-0.6.8/gpjax/base/module.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/base/param.py` & `gpjax-0.6.8/gpjax/base/param.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/citation.py` & `gpjax-0.6.8/gpjax/citation.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/dataset.py` & `gpjax-0.6.8/gpjax/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from dataclasses import dataclass
+import warnings
 
 from beartype.typing import Optional
 import jax.numpy as jnp
 from jaxtyping import Num
 from simple_pytree import Pytree
 
 from gpjax.typing import Array
@@ -33,16 +34,18 @@
         y (Optional[Num[Array, "N Q"]]): Output data.
     """
 
     X: Optional[Num[Array, "N D"]] = None
     y: Optional[Num[Array, "N Q"]] = None
 
     def __post_init__(self) -> None:
-        r"""Checks that the shapes of $`X`$ and $`y`$ are compatible."""
+        r"""Checks that the shapes of $`X`$ and $`y`$ are compatible,
+        and provides warnings regarding the precision of $`X`$ and $`y`$."""
         _check_shape(self.X, self.y)
+        _check_precision(self.X, self.y)
 
     def __repr__(self) -> str:
         r"""Returns a string representation of the dataset."""
         repr = (
             f"- Number of observations: {self.n}\n- Input dimension:"
             f" {self.in_dim}\n- Output dimension: {self.out_dim}"
         )
@@ -102,10 +105,29 @@
 
     if y is not None and y.ndim != 2:
         raise ValueError(
             f"Outputs, y, must be a 2-dimensional array. Got y.ndim={y.ndim}."
         )
 
 
+def _check_precision(
+    X: Optional[Num[Array, "..."]], y: Optional[Num[Array, "..."]]
+) -> None:
+    r"""Checks the precision of $`X`$ and $`y`."""
+    if X is not None and X.dtype != jnp.float64:
+        warnings.warn(
+            "X is not of type float64. "
+            f"Got X.dtype={X.dtype}. This may lead to numerical instability. ",
+            stacklevel=2,
+        )
+
+    if y is not None and y.dtype != jnp.float64:
+        warnings.warn(
+            "y is not of type float64."
+            f"Got y.dtype={y.dtype}. This may lead to numerical instability.",
+            stacklevel=2,
+        )
+
+
 __all__ = [
     "Dataset",
 ]
```

### Comparing `gpjax-0.6.7/gpjax/fit.py` & `gpjax-0.6.8/gpjax/fit.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/gaussian_distribution.py` & `gpjax-0.6.8/gpjax/gaussian_distribution.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/gps.py` & `gpjax-0.6.8/gpjax/gps.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,15 @@
     and [kernel](https://docs.jaxgaussianprocesses.com/api/kernels/base/)
     function.
 
     A Gaussian process prior parameterised by a mean function $`m(\cdot)`$ and a kernel
     function $`k(\cdot, \cdot)`$ is given by
     $`p(f(\cdot)) = \mathcal{GP}(m(\cdot), k(\cdot, \cdot))`$.
 
-    To invoke a `Prior` distribution, only a kernel function is required. By
-    default, the mean function will be set to zero. In general, this assumption
-    will be reasonable assuming the data being modelled has been centred.
+    To invoke a `Prior` distribution, a kernel and mean function must be specified.
 
     Example:
     ```python
         >>> import gpjax as gpx
 
         >>> kernel = gpx.kernels.RBF()
         >>> meanf = gpx.mean_functions.Zero()
```

### Comparing `gpjax-0.6.7/gpjax/integrators.py` & `gpjax-0.6.8/gpjax/integrators.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/__init__.py` & `gpjax-0.6.8/gpjax/kernels/computations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,61 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-"""JaxKern."""
-from gpjax.kernels.approximations import RFF
-from gpjax.kernels.base import (
-    AbstractKernel,
-    ProductKernel,
-    SumKernel,
-)
-from gpjax.kernels.computations import (
-    BasisFunctionComputation,
+from gpjax.kernels.computations.base import AbstractKernelComputation
+from gpjax.kernels.computations.basis_functions import BasisFunctionComputation
+from gpjax.kernels.computations.constant_diagonal import (
     ConstantDiagonalKernelComputation,
-    DenseKernelComputation,
-    DiagonalKernelComputation,
-    EigenKernelComputation,
-)
-from gpjax.kernels.non_euclidean import GraphKernel
-from gpjax.kernels.nonstationary import (
-    ArcCosine,
-    Linear,
-    Polynomial,
-)
-from gpjax.kernels.stationary import (
-    RBF,
-    Matern12,
-    Matern32,
-    Matern52,
-    Periodic,
-    PoweredExponential,
-    RationalQuadratic,
-    White,
 )
+from gpjax.kernels.computations.dense import DenseKernelComputation
+from gpjax.kernels.computations.diagonal import DiagonalKernelComputation
+from gpjax.kernels.computations.eigen import EigenKernelComputation
 
 __all__ = [
-    "AbstractKernel",
-    "ArcCosine",
-    "RBF",
-    "GraphKernel",
-    "Matern12",
-    "Matern32",
-    "Matern52",
-    "Linear",
-    "Polynomial",
-    "ProductKernel",
-    "SumKernel",
+    "AbstractKernelComputation",
+    "BasisFunctionComputation",
+    "ConstantDiagonalKernelComputation",
     "DenseKernelComputation",
     "DiagonalKernelComputation",
-    "ConstantDiagonalKernelComputation",
     "EigenKernelComputation",
-    "PoweredExponential",
-    "Periodic",
-    "RationalQuadratic",
-    "White",
-    "BasisFunctionComputation",
-    "RFF",
 ]
```

### Comparing `gpjax-0.6.7/gpjax/kernels/approximations/rff.py` & `gpjax-0.6.8/gpjax/kernels/approximations/rff.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,24 +33,26 @@
     - 'Random Features for Large-Scale Kernel Machines' by Rahimi and Recht (2008).
     - 'On the Error of Random Fourier Features' by Sutherland and Schneider (2015).
     """
 
     base_kernel: AbstractKernel = None
     num_basis_fns: int = static_field(50)
     frequencies: Float[Array, "M 1"] = param_field(None, bijector=tfb.Identity())
+    compute_engine: BasisFunctionComputation = static_field(
+        BasisFunctionComputation(), repr=False
+    )
     key: KeyArray = static_field(PRNGKey(123))
 
     def __post_init__(self) -> None:
         r"""Post-initialisation function.
 
         This function is called after the initialisation of the kernel. It is used to
         set the computation engine to be the basis function computation engine.
         """
         self._check_valid_base_kernel(self.base_kernel)
-        self.compute_engine = BasisFunctionComputation
 
         if self.frequencies is None:
             n_dims = self.base_kernel.ndims
             self.frequencies = self.base_kernel.spectral_density.sample(
                 seed=self.key, sample_shape=(self.num_basis_fns, n_dims)
             )
         self.name = f"{self.base_kernel.name} (RFF)"
@@ -79,8 +81,8 @@
         Args:
             x: A $`N \times D`$ array of inputs.
 
         Returns
         -------
             Float[Array, "N L"]: A $`N \times L`$ array of features where $`L = 2M`$.
         """
-        return self.compute_engine(self).compute_features(x)
+        return self.compute_engine.compute_features(self, x)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/base.py` & `gpjax-0.6.8/gpjax/kernels/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-
 import abc
 from dataclasses import dataclass
 from functools import partial
 
 from beartype.typing import (
     Callable,
     List,
     Optional,
-    Type,
     Union,
 )
 import jax.numpy as jnp
 from jaxtyping import (
     Float,
     Num,
 )
@@ -47,29 +45,27 @@
 )
 
 
 @dataclass
 class AbstractKernel(Module):
     r"""Base kernel class."""
 
-    compute_engine: Type[AbstractKernelComputation] = static_field(
-        DenseKernelComputation
-    )
+    compute_engine: AbstractKernelComputation = static_field(DenseKernelComputation())
     active_dims: Optional[List[int]] = static_field(None)
     name: str = static_field("AbstractKernel")
 
     @property
     def ndims(self):
         return 1 if not self.active_dims else len(self.active_dims)
 
     def cross_covariance(self, x: Num[Array, "N D"], y: Num[Array, "M D"]):
-        return self.compute_engine(self).cross_covariance(x, y)
+        return self.compute_engine.cross_covariance(self, x, y)
 
     def gram(self, x: Num[Array, "N D"]):
-        return self.compute_engine(self).gram(x)
+        return self.compute_engine.gram(self, x)
 
     def slice_input(self, x: Float[Array, "... D"]) -> Float[Array, "... Q"]:
         r"""Slice out the relevant columns of the input matrix.
 
         Select the relevant columns of the supplied matrix to be used within the
         kernel's evaluation.
```

### Comparing `gpjax-0.6.7/gpjax/kernels/computations/base.py` & `gpjax-0.6.8/gpjax/kernels/computations/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,73 +11,80 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import abc
 from dataclasses import dataclass
+import typing as tp
 
 from jax import vmap
 from jaxtyping import (
     Float,
     Num,
 )
 
 from gpjax.linops import (
     DenseLinearOperator,
     DiagonalLinearOperator,
     LinearOperator,
 )
 from gpjax.typing import Array
 
+Kernel = tp.TypeVar("Kernel", bound="gpjax.kernels.base.AbstractKernel")  # noqa: F821
+
 
 @dataclass
 class AbstractKernelComputation:
     r"""Abstract class for kernel computations."""
 
-    kernel: "gpjax.kernels.base.AbstractKernel"  # noqa: F821
-
     def gram(
         self,
+        kernel: Kernel,
         x: Num[Array, "N D"],
     ) -> LinearOperator:
         r"""Compute Gram covariance operator of the kernel function.
 
         Args:
+            kernel (AbstractKernel): the kernel function.
             x (Float[Array, "N N"]): The inputs to the kernel function.
 
         Returns
         -------
             LinearOperator: Gram covariance operator of the kernel function.
         """
-        Kxx = self.cross_covariance(x, x)
+        Kxx = self.cross_covariance(kernel, x, x)
         return DenseLinearOperator(Kxx)
 
     @abc.abstractmethod
     def cross_covariance(
-        self, x: Num[Array, "N D"], y: Num[Array, "M D"]
+        self, kernel: Kernel, x: Num[Array, "N D"], y: Num[Array, "M D"]
     ) -> Float[Array, "N M"]:
         r"""For a given kernel, compute the NxM gram matrix on an a pair
         of input matrices with shape NxD and MxD.
 
         Args:
+            kernel (AbstractKernel): the kernel function.
             x (Float[Array,"N D"]): The first input matrix.
             y (Float[Array,"M D"]): The second input matrix.
 
         Returns
         -------
             Float[Array, "N M"]: The computed cross-covariance.
         """
         raise NotImplementedError
 
-    def diagonal(self, inputs: Num[Array, "N D"]) -> DiagonalLinearOperator:
+    def diagonal(
+        self, kernel: Kernel, inputs: Num[Array, "N D"]
+    ) -> DiagonalLinearOperator:
         r"""For a given kernel, compute the elementwise diagonal of the
         NxN gram matrix on an input matrix of shape NxD.
 
         Args:
+            kernel (AbstractKernel): the kernel function.
             inputs (Float[Array, "N D"]): The input matrix.
 
         Returns
         -------
             DiagonalLinearOperator: The computed diagonal variance entries.
         """
-        return DiagonalLinearOperator(diag=vmap(lambda x: self.kernel(x, x))(inputs))
+        return DiagonalLinearOperator(diag=vmap(lambda x: kernel(x, x))(inputs))
```

### Comparing `gpjax-0.6.7/gpjax/kernels/computations/basis_functions.py` & `gpjax-0.6.8/gpjax/kernels/computations/basis_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,83 @@
 from dataclasses import dataclass
+import typing as tp
 
 import jax.numpy as jnp
 from jaxtyping import Float
 
 from gpjax.kernels.computations.base import AbstractKernelComputation
 from gpjax.linops import DenseLinearOperator
 from gpjax.typing import Array
 
+Kernel = tp.TypeVar("Kernel", bound="gpjax.kernels.base.AbstractKernel")  # noqa: F821
+
 
 @dataclass
 class BasisFunctionComputation(AbstractKernelComputation):
     r"""Compute engine class for finite basis function approximations to a kernel."""
 
-    num_basis_fns: int = None
-
     def cross_covariance(
-        self, x: Float[Array, "N D"], y: Float[Array, "M D"]
+        self, kernel: Kernel, x: Float[Array, "N D"], y: Float[Array, "M D"]
     ) -> Float[Array, "N M"]:
         r"""Compute an approximate cross-covariance matrix.
 
         For a pair of inputs, compute the cross covariance matrix between the inputs.
 
         Args:
+            kernel (Kernel): the kernel function.
             x: (Float[Array, "N D"]): A $`N \times D`$ array of inputs.
             y: (Float[Array, "M D"]): A $`M \times D`$ array of inputs.
 
         Returns:
             Float[Array, "N M"]: A $N \times M$ array of cross-covariances.
         """
-        z1 = self.compute_features(x)
-        z2 = self.compute_features(y)
-        return self.scaling * jnp.matmul(z1, z2.T)
+        z1 = self.compute_features(kernel, x)
+        z2 = self.compute_features(kernel, y)
+        return self.scaling(kernel) * jnp.matmul(z1, z2.T)
 
-    def gram(self, inputs: Float[Array, "N D"]) -> DenseLinearOperator:
+    def gram(self, kernel: Kernel, inputs: Float[Array, "N D"]) -> DenseLinearOperator:
         r"""Compute an approximate Gram matrix.
 
         For the Gram matrix, we can save computations by computing only one matrix
         multiplication between the inputs and the scaled frequencies.
 
         Args:
+            kernel (Kernel): the kernel function.
             inputs (Float[Array, "N D"]): A $`N x D`$ array of inputs.
 
         Returns:
             DenseLinearOperator: A dense linear operator representing the
                 $`N \times N`$ Gram matrix.
         """
-        z1 = self.compute_features(inputs)
-        return DenseLinearOperator(self.scaling * jnp.matmul(z1, z1.T))
+        z1 = self.compute_features(kernel, inputs)
+        return DenseLinearOperator(self.scaling(kernel) * jnp.matmul(z1, z1.T))
 
-    def compute_features(self, x: Float[Array, "N D"]) -> Float[Array, "N L"]:
+    def compute_features(
+        self, kernel: Kernel, x: Float[Array, "N D"]
+    ) -> Float[Array, "N L"]:
         r"""Compute the features for the inputs.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array, "N D"]): A $`N \times D`$ array of inputs.
 
         Returns
         -------
             Float[Array, "N L"]: A $`N \times L`$ array of features where $`L = 2M`$.
         """
-        frequencies = self.kernel.frequencies
-        scaling_factor = self.kernel.base_kernel.lengthscale
+        frequencies = kernel.frequencies
+        scaling_factor = kernel.base_kernel.lengthscale
         z = jnp.matmul(x, (frequencies / scaling_factor).T)
         z = jnp.concatenate([jnp.cos(z), jnp.sin(z)], axis=-1)
         return z
 
-    @property
-    def scaling(self):
-        return self.kernel.base_kernel.variance / self.kernel.num_basis_fns
+    def scaling(self, kernel: Kernel):
+        r"""Compute the scaling factor for the covariance matrix.
+
+        Args:
+            kernel (Kernel): the kernel function.
+
+        Returns
+        -------
+            Float[Array, ""]: A scalar array.
+        """
+        return kernel.base_kernel.variance / kernel.num_basis_fns
```

### Comparing `gpjax-0.6.7/gpjax/kernels/computations/constant_diagonal.py` & `gpjax-0.6.8/gpjax/kernels/computations/constant_diagonal.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,71 +9,82 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+import typing as tp
+
 from jax import vmap
 import jax.numpy as jnp
 from jaxtyping import Float
 
-from gpjax.kernels.computations.base import AbstractKernelComputation
+from gpjax.kernels.computations import AbstractKernelComputation
 from gpjax.linops import (
     ConstantDiagonalLinearOperator,
     DiagonalLinearOperator,
 )
 from gpjax.typing import Array
 
+Kernel = tp.TypeVar("Kernel", bound="gpjax.kernels.base.AbstractKernel")  # noqa: F821
+
 
 class ConstantDiagonalKernelComputation(AbstractKernelComputation):
-    def gram(self, x: Float[Array, "N D"]) -> ConstantDiagonalLinearOperator:
+    def gram(
+        self, kernel: Kernel, x: Float[Array, "N D"]
+    ) -> ConstantDiagonalLinearOperator:
         r"""Compute the Gram matrix.
 
         Compute Gram covariance operator of the kernel function.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array, "N N"]): The inputs to the kernel function.
         """
-        value = self.kernel(x[0], x[0])
+        value = kernel(x[0], x[0])
 
         return ConstantDiagonalLinearOperator(
             value=jnp.atleast_1d(value), size=x.shape[0]
         )
 
-    def diagonal(self, inputs: Float[Array, "N D"]) -> DiagonalLinearOperator:
+    def diagonal(
+        self, kernel: Kernel, inputs: Float[Array, "N D"]
+    ) -> DiagonalLinearOperator:
         r"""Compute the diagonal Gram matrix's entries.
 
         For a given kernel, compute the elementwise diagonal of the
         NxN gram matrix on an input matrix of shape $`N\times D`$.
 
         Args:
+            kernel (Kernel): the kernel function.
             inputs (Float[Array, "N D"]): The input matrix.
 
         Returns
         -------
             DiagonalLinearOperator: The computed diagonal variance entries.
         """
-        diag = vmap(lambda x: self.kernel(x, x))(inputs)
+        diag = vmap(lambda x: kernel(x, x))(inputs)
 
         return DiagonalLinearOperator(diag=diag)
 
     def cross_covariance(
-        self, x: Float[Array, "N D"], y: Float[Array, "M D"]
+        self, kernel: Kernel, x: Float[Array, "N D"], y: Float[Array, "M D"]
     ) -> Float[Array, "N M"]:
         r"""Compute the cross-covariance matrix.
 
         For a given kernel, compute the NxM covariance matrix on a pair of input
         matrices of shape NxD and MxD.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array,"N D"]): The input matrix.
             y (Float[Array,"M D"]): The input matrix.
 
         Returns
         -------
             Float[Array, "N M"]: The computed square Gram matrix.
         """
         # TODO: This is currently a dense implementation. We should implement
         # a sparse LinearOperator for non-square cross-covariance matrices.
-        cross_cov = vmap(lambda x: vmap(lambda y: self.kernel(x, y))(y))(x)
+        cross_cov = vmap(lambda x: vmap(lambda y: kernel(x, y))(y))(x)
         return cross_cov
```

### Comparing `gpjax-0.6.7/gpjax/kernels/computations/dense.py` & `gpjax-0.6.8/gpjax/kernels/computations/dense.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,37 +9,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+import beartype.typing as tp
 from jax import vmap
 from jaxtyping import Float
 
 from gpjax.kernels.computations.base import AbstractKernelComputation
 from gpjax.typing import Array
 
+Kernel = tp.TypeVar("Kernel", bound="gpjax.kernels.base.AbstractKernel")  # noqa: F821
+
 
 class DenseKernelComputation(AbstractKernelComputation):
     r"""Dense kernel computation class. Operations with the kernel assume
     a dense gram matrix structure.
     """
 
     def cross_covariance(
-        self, x: Float[Array, "N D"], y: Float[Array, "M D"]
+        self, kernel: Kernel, x: Float[Array, "N D"], y: Float[Array, "M D"]
     ) -> Float[Array, "N M"]:
         r"""Compute the cross-covariance matrix.
 
         For a given kernel, compute the NxM covariance matrix on a pair of input
         matrices of shape $`NxD`$ and $`MxD`$.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array,"N D"]): The input matrix.
             y (Float[Array,"M D"]): The input matrix.
 
         Returns
         -------
             Float[Array, "N M"]: The computed cross-covariance.
         """
-        cross_cov = vmap(lambda x: vmap(lambda y: self.kernel(x, y))(y))(x)
+        cross_cov = vmap(lambda x: vmap(lambda y: kernel(x, y))(y))(x)
         return cross_cov
```

### Comparing `gpjax-0.6.7/gpjax/kernels/computations/diagonal.py` & `gpjax-0.6.8/gpjax/kernels/computations/diagonal.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,54 +9,59 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+import beartype.typing as tp
 from jax import vmap
 from jaxtyping import Float
 
-from gpjax.kernels.computations.base import AbstractKernelComputation
+from gpjax.kernels.computations import AbstractKernelComputation
 from gpjax.linops import DiagonalLinearOperator
 from gpjax.typing import Array
 
+Kernel = tp.TypeVar("Kernel", bound="gpjax.kernels.base.AbstractKernel")  # noqa: F821
+
 
 class DiagonalKernelComputation(AbstractKernelComputation):
     r"""Diagonal kernel computation class. Operations with the kernel assume
     a diagonal Gram matrix.
     """
 
-    def gram(self, x: Float[Array, "N D"]) -> DiagonalLinearOperator:
+    def gram(self, kernel: Kernel, x: Float[Array, "N D"]) -> DiagonalLinearOperator:
         r"""Compute the Gram matrix.
 
         For a kernel with diagonal structure, compute the $`N\times N`$ Gram matrix on
         an input matrix of shape $`N\times D`$.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array, "N D"]): The input matrix.
 
         Returns
         -------
             DiagonalLinearOperator: The computed square Gram matrix.
         """
-        return DiagonalLinearOperator(diag=vmap(lambda x: self.kernel(x, x))(x))
+        return DiagonalLinearOperator(diag=vmap(lambda x: kernel(x, x))(x))
 
     def cross_covariance(
-        self, x: Float[Array, "N D"], y: Float[Array, "M D"]
+        self, kernel: Kernel, x: Float[Array, "N D"], y: Float[Array, "M D"]
     ) -> Float[Array, "N M"]:
         r"""Compute the cross-covariance matrix.
 
         For a given kernel, compute the $`N\times M`$ covariance matrix on a pair of
         input matrices of shape $`N\times D`$ and $`M\times D`$.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array,"N D"]): The input matrix.
             y (Float[Array,"M D"]): The input matrix.
 
         Returns
         -------
             Float[Array, "N M"]: The computed cross-covariance.
         """
         # TODO: This is currently a dense implementation. We should implement a sparse LinearOperator for non-square cross-covariance matrices.
-        cross_cov = vmap(lambda x: vmap(lambda y: self.kernel(x, y))(y))(x)
+        cross_cov = vmap(lambda x: vmap(lambda y: kernel(x, y))(y))(x)
         return cross_cov
```

### Comparing `gpjax-0.6.7/gpjax/kernels/computations/eigen.py` & `gpjax-0.6.8/gpjax/kernels/computations/eigen.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,52 +12,53 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 from dataclasses import dataclass
 
+import beartype.typing as tp
 import jax.numpy as jnp
 from jaxtyping import (
     Float,
     Num,
 )
 
 from gpjax.kernels.computations.base import AbstractKernelComputation
 from gpjax.typing import Array
 
+Kernel = tp.TypeVar("Kernel", bound="gpjax.kernels.base.AbstractKernel")  # noqa: F821
+
 
 @dataclass
 class EigenKernelComputation(AbstractKernelComputation):
     r"""Eigen kernel computation class. Kernels who operate on an
     eigen-decomposed structure should use this computation object.
     """
 
     def cross_covariance(
-        self, x: Num[Array, "N D"], y: Num[Array, "M D"]
+        self, kernel: Kernel, x: Num[Array, "N D"], y: Num[Array, "M D"]
     ) -> Float[Array, "N M"]:
         r"""Compute the cross-covariance matrix.
 
         For an $`N\times D`$ and $`M\times D`$ pair of matrices, evaluate the $`N \times M`$
         cross-covariance matrix.
 
         Args:
+            kernel (Kernel): the kernel function.
             x (Float[Array,"N D"]): The input matrix.
             y (Float[Array,"M D"]): The input matrix.
 
         Returns:
             _type_: _description_
         """
         # Transform the eigenvalues of the graph Laplacian according to the
         # RBF kernel's SPDE form.
         S = jnp.power(
-            self.kernel.eigenvalues
-            + 2
-            * self.kernel.smoothness
-            / self.kernel.lengthscale
-            / self.kernel.lengthscale,
-            -self.kernel.smoothness,
+            kernel.eigenvalues
+            + 2 * kernel.smoothness / kernel.lengthscale / kernel.lengthscale,
+            -kernel.smoothness,
         )
-        S = jnp.multiply(S, self.kernel.num_vertex / jnp.sum(S))
+        S = jnp.multiply(S, kernel.num_vertex / jnp.sum(S))
         # Scale the transform eigenvalues by the kernel variance
-        S = jnp.multiply(S, self.kernel.variance)
-        return self.kernel(x, y, S=S)
+        S = jnp.multiply(S, kernel.variance)
+        return kernel(x, y, S=S)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/non_euclidean/__init__.py` & `gpjax-0.6.8/gpjax/kernels/non_euclidean/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from gpjax.kernels.non_euclidean.graph import GraphKernel
+from gpjax.kernels.non_euclidean.categorical import CatKernel
 
-__all__ = ["GraphKernel"]
+__all__ = ["GraphKernel", "CatKernel"]
```

### Comparing `gpjax-0.6.7/gpjax/kernels/non_euclidean/graph.py` & `gpjax-0.6.8/gpjax/kernels/non_euclidean/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     laplacian: Num[Array, "N N"] = static_field(None)
     lengthscale: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
     smoothness: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
     eigenvalues: Float[Array, " N"] = static_field(None)
     eigenvectors: Float[Array, "N N"] = static_field(None)
     num_vertex: ScalarInt = static_field(None)
-    compute_engine: AbstractKernelComputation = static_field(EigenKernelComputation)
+    compute_engine: AbstractKernelComputation = static_field(
+        EigenKernelComputation(), repr=False
+    )
     name: str = "Graph Matérn"
 
     def __post_init__(self):
         if self.laplacian is None:
             raise ValueError("Graph laplacian must be specified")
 
         evals, self.eigenvectors = jnp.linalg.eigh(self.laplacian)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/non_euclidean/utils.py` & `gpjax-0.6.8/gpjax/kernels/non_euclidean/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/nonstationary/__init__.py` & `gpjax-0.6.8/gpjax/kernels/nonstationary/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/nonstationary/arccosine.py` & `gpjax-0.6.8/gpjax/kernels/nonstationary/arccosine.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/nonstationary/linear.py` & `gpjax-0.6.8/gpjax/kernels/nonstationary/linear.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/nonstationary/polynomial.py` & `gpjax-0.6.8/gpjax/kernels/nonstationary/polynomial.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/__init__.py` & `gpjax-0.6.8/gpjax/kernels/stationary/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/matern12.py` & `gpjax-0.6.8/gpjax/kernels/stationary/matern12.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
         r"""Compute the Matérn 1/2 kernel between a pair of arrays.
 
         Evaluate the kernel on a pair of inputs $`(x, y)`$ with
         lengthscale parameter $`\ell`$ and variance $`\sigma^2`$.
         ```math
-        (x, y) = \sigma^2\exp\Bigg(-\frac{\lvert x-y \rvert}{2\ell^2}\Bigg)
+        k(x, y) = \sigma^2\exp\Bigg(-\frac{\lvert x-y \rvert}{2\ell^2}\Bigg)
         ```
 
         Args:
             x (Float[Array, " D"]): The left hand argument of the kernel function's call.
             y (Float[Array, " D"]): The right hand argument of the kernel function's call
         Returns:
             ScalarFloat: The value of $`k(x, y)`$
```

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/matern32.py` & `gpjax-0.6.8/gpjax/kernels/stationary/matern52.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,47 +30,46 @@
 from gpjax.typing import (
     Array,
     ScalarFloat,
 )
 
 
 @dataclass
-class Matern32(AbstractKernel):
-    r"""The Matérn kernel with smoothness parameter fixed at 1.5."""
+class Matern52(AbstractKernel):
+    r"""The Matérn kernel with smoothness parameter fixed at 2.5."""
 
     lengthscale: Union[ScalarFloat, Float[Array, " D"]] = param_field(
         jnp.array(1.0), bijector=tfb.Softplus()
     )
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
-    name: str = "Matérn32"
+    name: str = "Matérn52"
 
-    def __call__(
-        self,
-        x: Float[Array, " D"],
-        y: Float[Array, " D"],
-    ) -> ScalarFloat:
-        r"""Compute the Matérn 3/2 kernel between a pair of arrays.
+    def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
+        r"""Compute the Matérn 5/2 kernel between a pair of arrays.
 
         Evaluate the kernel on a pair of inputs $`(x, y)`$ with
-        lengthscale parameter $\ell$ and variance $`\sigma^2`$.
-
+        lengthscale parameter $`\ell`$ and variance $`\sigma^2`$.
         ```math
-            k(x, y) = \\sigma^2 \\exp \\Bigg(1+ \\frac{\\sqrt{3}\\lvert x-y \\rvert}{\\ell^2}  \\Bigg)\\exp\\Bigg(-\\frac{\\sqrt{3}\\lvert x-y\\rvert}{\\ell^2} \\Bigg)
+        k(x, y) = \sigma^2 \exp \Bigg(1+ \frac{\sqrt{5}\lvert x-y \rvert}{\ell^2} + \frac{5\lvert x - y \rvert^2}{3\ell^2} \Bigg)\exp\Bigg(-\frac{\sqrt{5}\lvert x-y\rvert}{\ell^2} \Bigg)
         ```
 
         Args:
             x (Float[Array, " D"]): The left hand argument of the kernel function's call.
             y (Float[Array, " D"]): The right hand argument of the kernel function's call.
 
         Returns
         -------
-            ScalarFloat: The value of $k(x, y)$.
+            ScalarFloat: The value of $`k(x, y)`$.
         """
         x = self.slice_input(x) / self.lengthscale
         y = self.slice_input(y) / self.lengthscale
         tau = euclidean_distance(x, y)
-        K = self.variance * (1.0 + jnp.sqrt(3.0) * tau) * jnp.exp(-jnp.sqrt(3.0) * tau)
+        K = (
+            self.variance
+            * (1.0 + jnp.sqrt(5.0) * tau + 5.0 / 3.0 * jnp.square(tau))
+            * jnp.exp(-jnp.sqrt(5.0) * tau)
+        )
         return K.squeeze()
 
     @property
     def spectral_density(self) -> tfd.Distribution:
-        return build_student_t_distribution(nu=3)
+        return build_student_t_distribution(nu=5)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/matern52.py` & `gpjax-0.6.8/gpjax/kernels/stationary/matern32.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,46 +30,47 @@
 from gpjax.typing import (
     Array,
     ScalarFloat,
 )
 
 
 @dataclass
-class Matern52(AbstractKernel):
-    r"""The Matérn kernel with smoothness parameter fixed at 2.5."""
+class Matern32(AbstractKernel):
+    r"""The Matérn kernel with smoothness parameter fixed at 1.5."""
 
     lengthscale: Union[ScalarFloat, Float[Array, " D"]] = param_field(
         jnp.array(1.0), bijector=tfb.Softplus()
     )
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
-    name: str = "Matérn52"
+    name: str = "Matérn32"
 
-    def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
-        r"""Compute the Matérn 5/2 kernel between a pair of arrays.
+    def __call__(
+        self,
+        x: Float[Array, " D"],
+        y: Float[Array, " D"],
+    ) -> ScalarFloat:
+        r"""Compute the Matérn 3/2 kernel between a pair of arrays.
 
         Evaluate the kernel on a pair of inputs $`(x, y)`$ with
         lengthscale parameter $`\ell`$ and variance $`\sigma^2`$.
+
         ```math
-        k(x, y) = \sigma^2 \exp \Bigg(1+ \frac{\sqrt{5}\lvert x-y \rvert}{\ell^2} + \frac{5\lvert x - y \rvert^2}{3\ell^2} \Bigg)\exp\Bigg(-\frac{\sqrt{5}\lvert x-y\rvert}{\ell^2} \Bigg)
+            k(x, y) = \sigma^2 \exp \Bigg(1+ \frac{\sqrt{3}\lvert x-y \rvert}{\ell^2}  \Bigg)\exp\Bigg(-\frac{\sqrt{3}\lvert x-y\rvert}{\ell^2} \Bigg)
         ```
 
         Args:
             x (Float[Array, " D"]): The left hand argument of the kernel function's call.
             y (Float[Array, " D"]): The right hand argument of the kernel function's call.
 
         Returns
         -------
-            ScalarFloat: The value of $`k(x, y)`$.
+            ScalarFloat: The value of $k(x, y)$.
         """
         x = self.slice_input(x) / self.lengthscale
         y = self.slice_input(y) / self.lengthscale
         tau = euclidean_distance(x, y)
-        K = (
-            self.variance
-            * (1.0 + jnp.sqrt(5.0) * tau + 5.0 / 3.0 * jnp.square(tau))
-            * jnp.exp(-jnp.sqrt(5.0) * tau)
-        )
+        K = self.variance * (1.0 + jnp.sqrt(3.0) * tau) * jnp.exp(-jnp.sqrt(3.0) * tau)
         return K.squeeze()
 
     @property
     def spectral_density(self) -> tfd.Distribution:
-        return build_student_t_distribution(nu=5)
+        return build_student_t_distribution(nu=3)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/periodic.py` & `gpjax-0.6.8/gpjax/kernels/stationary/rbf.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,50 +15,52 @@
 
 from dataclasses import dataclass
 
 from beartype.typing import Union
 import jax.numpy as jnp
 from jaxtyping import Float
 import tensorflow_probability.substrates.jax.bijectors as tfb
+import tensorflow_probability.substrates.jax.distributions as tfd
 
 from gpjax.base import param_field
 from gpjax.kernels.base import AbstractKernel
+from gpjax.kernels.stationary.utils import squared_distance
 from gpjax.typing import (
     Array,
     ScalarFloat,
 )
 
 
 @dataclass
-class Periodic(AbstractKernel):
-    r"""The periodic kernel.
-
-    Key reference is MacKay 1998 - "Introduction to Gaussian processes".
-    """
+class RBF(AbstractKernel):
+    r"""The Radial Basis Function (RBF) kernel."""
 
     lengthscale: Union[ScalarFloat, Float[Array, " D"]] = param_field(
         jnp.array(1.0), bijector=tfb.Softplus()
     )
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
-    period: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
-    name: str = "Periodic"
+    name: str = "RBF"
 
     def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
-        r"""Compute the Periodic kernel between a pair of arrays.
+        r"""Compute the RBF kernel between a pair of arrays.
 
-        TODO: update docstring
-        Evaluate the kernel on a pair of inputs $`(x, y)`$ with length-scale parameter $\ell$ and variance $\sigma$.
+        Evaluate the kernel on a pair of inputs $`(x, y)`$ with lengthscale parameter
+        $`\ell`$ and variance $`\sigma^2`$:
         ```math
-        k(x, y) = \sigma^2 \exp \Bigg( -0.5 \sum_{i=1}^{d} \Bigg)
+        k(x,y)=\sigma^2\exp\Bigg(- \frac{\lVert x - y \rVert^2_2}{2 \ell^2} \Bigg)
         ```
 
         Args:
             x (Float[Array, " D"]): The left hand argument of the kernel function's call.
-            y (Float[Array, " D"]): The right hand argument of the kernel function's call
+            y (Float[Array, " D"]): The right hand argument of the kernel function's call.
+
         Returns:
             ScalarFloat: The value of $`k(x, y)`$.
         """
-        x = self.slice_input(x)
-        y = self.slice_input(y)
-        sine_squared = (jnp.sin(jnp.pi * (x - y) / self.period) / self.lengthscale) ** 2
-        K = self.variance * jnp.exp(-0.5 * jnp.sum(sine_squared, axis=0))
+        x = self.slice_input(x) / self.lengthscale
+        y = self.slice_input(y) / self.lengthscale
+        K = self.variance * jnp.exp(-0.5 * squared_distance(x, y))
         return K.squeeze()
+
+    @property
+    def spectral_density(self) -> tfd.Normal:
+        return tfd.Normal(loc=0.0, scale=1.0)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/powered_exponential.py` & `gpjax-0.6.8/gpjax/kernels/stationary/powered_exponential.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/rational_quadratic.py` & `gpjax-0.6.8/gpjax/kernels/stationary/rational_quadratic.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/rbf.py` & `gpjax-0.6.8/gpjax/kernels/stationary/periodic.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,52 +15,50 @@
 
 from dataclasses import dataclass
 
 from beartype.typing import Union
 import jax.numpy as jnp
 from jaxtyping import Float
 import tensorflow_probability.substrates.jax.bijectors as tfb
-import tensorflow_probability.substrates.jax.distributions as tfd
 
 from gpjax.base import param_field
 from gpjax.kernels.base import AbstractKernel
-from gpjax.kernels.stationary.utils import squared_distance
 from gpjax.typing import (
     Array,
     ScalarFloat,
 )
 
 
 @dataclass
-class RBF(AbstractKernel):
-    r"""The Radial Basis Function (RBF) kernel."""
+class Periodic(AbstractKernel):
+    r"""The periodic kernel.
+
+    Key reference is MacKay 1998 - "Introduction to Gaussian processes".
+    """
 
     lengthscale: Union[ScalarFloat, Float[Array, " D"]] = param_field(
         jnp.array(1.0), bijector=tfb.Softplus()
     )
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
-    name: str = "RBF"
+    period: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
+    name: str = "Periodic"
 
     def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
-        r"""Compute the RBF kernel between a pair of arrays.
+        r"""Compute the Periodic kernel between a pair of arrays.
 
-        Evaluate the kernel on a pair of inputs $`(x, y)`$ with lengthscale parameter
-        $`\ell`$ and variance $`\sigma^2`$:
+        Evaluate the kernel on a pair of inputs $`(x, y)`$ with length-scale parameter $`\ell`$, variance $`\sigma^2`$
+        and period $`p`$.
         ```math
-        k(x,y)=\sigma^2\exp\Bigg(\frac{\lVert x - y \rVert^2_2}{2 \ell^2} \Bigg)
+        k(x, y) = \sigma^2 \exp \left( -\frac{1}{2} \sum_{i=1}^{D} \left(\frac{\sin (\pi (x_i - y_i)/p)}{\ell}\right)^2 \right)
         ```
 
         Args:
             x (Float[Array, " D"]): The left hand argument of the kernel function's call.
-            y (Float[Array, " D"]): The right hand argument of the kernel function's call.
-
+            y (Float[Array, " D"]): The right hand argument of the kernel function's call
         Returns:
             ScalarFloat: The value of $`k(x, y)`$.
         """
-        x = self.slice_input(x) / self.lengthscale
-        y = self.slice_input(y) / self.lengthscale
-        K = self.variance * jnp.exp(-0.5 * squared_distance(x, y))
+        x = self.slice_input(x)
+        y = self.slice_input(y)
+        sine_squared = (jnp.sin(jnp.pi * (x - y) / self.period) / self.lengthscale) ** 2
+        K = self.variance * jnp.exp(-0.5 * jnp.sum(sine_squared, axis=0))
         return K.squeeze()
-
-    @property
-    def spectral_density(self) -> tfd.Normal:
-        return tfd.Normal(loc=0.0, scale=1.0)
```

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/utils.py` & `gpjax-0.6.8/gpjax/kernels/stationary/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/kernels/stationary/white.py` & `gpjax-0.6.8/gpjax/kernels/stationary/white.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 )
 
 
 @dataclass
 class White(AbstractKernel):
     variance: ScalarFloat = param_field(jnp.array(1.0), bijector=tfb.Softplus())
     compute_engine: AbstractKernelComputation = static_field(
-        ConstantDiagonalKernelComputation
+        ConstantDiagonalKernelComputation(), repr=False
     )
     name: str = "White"
 
     def __call__(self, x: Float[Array, " D"], y: Float[Array, " D"]) -> ScalarFloat:
         r"""Compute the White noise kernel between a pair of arrays.
 
         Evaluate the kernel on a pair of inputs $`(x, y)`$ with variance $`\sigma^2`$:
```

### Comparing `gpjax-0.6.7/gpjax/likelihoods.py` & `gpjax-0.6.8/gpjax/likelihoods.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/__init__.py` & `gpjax-0.6.8/gpjax/linops/__init__.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/constant_diagonal_linear_operator.py` & `gpjax-0.6.8/gpjax/linops/constant_diagonal_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/dense_linear_operator.py` & `gpjax-0.6.8/gpjax/linops/dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/diagonal_linear_operator.py` & `gpjax-0.6.8/gpjax/linops/diagonal_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/identity_linear_operator.py` & `gpjax-0.6.8/gpjax/linops/identity_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/linear_operator.py` & `gpjax-0.6.8/gpjax/linops/linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/triangular_linear_operator.py` & `gpjax-0.6.8/gpjax/linops/triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/utils.py` & `gpjax-0.6.8/gpjax/linops/utils.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/linops/zero_linear_operator.py` & `gpjax-0.6.8/gpjax/linops/zero_linear_operator.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/mean_functions.py` & `gpjax-0.6.8/gpjax/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/objectives.py` & `gpjax-0.6.8/gpjax/objectives.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/progress_bar.py` & `gpjax-0.6.8/gpjax/progress_bar.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/scan.py` & `gpjax-0.6.8/gpjax/scan.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/typing.py` & `gpjax-0.6.8/gpjax/typing.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/gpjax/variational_families.py` & `gpjax-0.6.8/gpjax/variational_families.py`

 * *Files identical despite different names*

### Comparing `gpjax-0.6.7/pyproject.toml` & `gpjax-0.6.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpjax"
-version = "0.6.7" # Merely a placeholder, will be replaced by the dynamic versioning plugin
+version = "0.6.8" # Merely a placeholder, will be replaced by the dynamic versioning plugin
 description = "Gaussian processes in JAX."
 authors = ["Thomas Pinder <tompinder@live.co.uk>", "Daniel Dodd <daniel_dodd@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JaxGaussianProcesses/GPJax"
 repository = "https://github.com/JaxGaussianProcesses/GPJax"
 include = [
@@ -188,15 +188,15 @@
 data_file = "reports/.coverage"
 source = ["src"]
 
 [tool.coverage.xml]  # https://coverage.readthedocs.io/en/latest/config.html#xml
 output = "reports/coverage.xml"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["gpjax/__init__.py"]
 
 [tool.codespell]
 ignore-words-list = "fro" # Frobenius
```

### Comparing `gpjax-0.6.7/PKG-INFO` & `gpjax-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpjax
-Version: 0.6.7
+Version: 0.6.8
 Summary: Gaussian processes in JAX.
 Home-page: https://github.com/JaxGaussianProcesses/GPJax
 License: Apache-2.0
 Keywords: gaussian-processes jax machine-learning bayesian
 Author: Thomas Pinder
 Author-email: tompinder@live.co.uk
 Requires-Python: >=3.8,<3.12
@@ -58,15 +58,15 @@
 GPJax was founded by [Thomas Pinder](https://github.com/thomaspinder). Today,
 the maintenance of GPJax is undertaken by [Thomas
 Pinder](https://github.com/thomaspinder) and [Daniel
 Dodd](https://github.com/Daniel-Dodd).
 
 We would be delighted to receive contributions from interested individuals and
 groups. To learn how you can get involved, please read our [guide for
-contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/master/CONTRIBUTING.md).
+contributing](https://github.com/JaxGaussianProcesses/GPJax/blob/main/docs/contributing.md).
 If you have any questions, we encourage you to [open an
 issue](https://github.com/JaxGaussianProcesses/GPJax/issues/new/choose). For
 broader conversations, such as best GP fitting practices or questions about the
 mathematics of GPs, we invite you to [open a
 discussion](https://github.com/JaxGaussianProcesses/GPJax/discussions).
 
 Feel free to join our [Slack
@@ -80,28 +80,29 @@
 
 > - [**Conjugate Inference**](https://docs.jaxgaussianprocesses.com/examples/regression/)
 > - [**Classification with MCMC**](https://docs.jaxgaussianprocesses.com/examples/classification/)
 > - [**Sparse Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/collapsed_vi/)
 > - [**Stochastic Variational Inference**](https://docs.jaxgaussianprocesses.com/examples/uncollapsed_vi/)
 > - [**BlackJax Integration**](https://docs.jaxgaussianprocesses.com/examples/classification/#mcmc-inference)
 > - [**Laplace Approximation**](https://docs.jaxgaussianprocesses.com/examples/classification/#laplace-approximation)
-> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**Inference on Non-Euclidean Spaces**](https://docs.jaxgaussianprocesses.com/examples/constructing_new_kernels/#custom-kernel)
 > - [**Inference on Graphs**](https://docs.jaxgaussianprocesses.com/examples/graph_kernels/)
 > - [**Pathwise Sampling**](https://docs.jaxgaussianprocesses.com/examples/spatial/)
 > - [**Learning Gaussian Process Barycentres**](https://docs.jaxgaussianprocesses.com/examples/barycentres/)
 > - [**Deep Kernel Regression**](https://docs.jaxgaussianprocesses.com/examples/deep_kernels/)
 > - [**Poisson Regression**](https://docs.jaxgaussianprocesses.com/examples/poisson/)
+> - [**Bayesian Optimisation**](https://docs.jaxgaussianprocesses.com/examples/bayesian_optimisation/)
 
 ## Guides for customisation
 >
-> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/kernels/#custom-kernel)
+> - [**Custom kernels**](https://docs.jaxgaussianprocesses.com/examples/constructing_new_kernels/#custom-kernel)
 > - [**UCI regression**](https://docs.jaxgaussianprocesses.com/examples/yacht/)
 
 ## Conversion between `.ipynb` and `.py`
-Above examples are stored in [examples](examples) directory in the double
+Above examples are stored in [examples](docs/examples) directory in the double
 percent (`py:percent`) format. Checkout [jupytext
 using-cli](https://jupytext.readthedocs.io/en/latest/using-cli.html) for more
 info.
 
 * To convert `example.py` to `example.ipynb`, run:
 
 ```bash
```

