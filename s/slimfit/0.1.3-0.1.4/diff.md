# Comparing `tmp/slimfit-0.1.3.tar.gz` & `tmp/slimfit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slimfit-0.1.3.tar", last modified: Sun Dec 11 14:16:47 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `slimfit-0.1.3.tar` & `slimfit-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 14:16:47.526602 slimfit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2022-12-11 14:16:37.000000 slimfit-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-11 14:16:37.000000 slimfit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-11 14:16:37.000000 slimfit-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2022-12-11 14:16:47.522602 slimfit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2022-12-11 14:16:37.000000 slimfit-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2022-12-11 14:16:37.000000 slimfit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-11 14:16:47.526602 slimfit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-12-11 14:16:37.000000 slimfit-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 14:16:47.526602 slimfit-0.1.3/slimfit/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-11 14:16:47.526602 slimfit-0.1.3/slimfit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/fitresult.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/markov.py
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2022-12-11 14:16:37.000000 slimfit-0.1.3/slimfit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 14:16:47.522602 slimfit-0.1.3/slimfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2022-12-11 14:16:47.000000 slimfit-0.1.3/slimfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-11 14:16:47.000000 slimfit-0.1.3/slimfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 14:16:47.000000 slimfit-0.1.3/slimfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-11 14:16:47.000000 slimfit-0.1.3/slimfit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-11 14:16:47.000000 slimfit-0.1.3/slimfit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 14:16:47.522602 slimfit-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21170 2022-12-11 14:16:37.000000 slimfit-0.1.3/tests/test_slimfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    83635 2022-12-11 14:16:37.000000 slimfit-0.1.3/versioneer.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 slimfit-0.1.4/.editorconfig
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 slimfit-0.1.4/.gitattributes
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 slimfit-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 slimfit-0.1.4/dependabot.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 slimfit-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 slimfit-0.1.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 slimfit-0.1.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 slimfit-0.1.4/.github/workflows/pin_requirements.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 slimfit-0.1.4/.github/workflows/pypi_main.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 slimfit-0.1.4/.github/workflows/pypi_test.yml
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 slimfit-0.1.4/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/index.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/installation.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/structure.md
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/css/styles.css
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/basic_fit.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/custom_numexpr_ivp.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/gaussian_mixture_model.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/gmm_amplitudes.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/likelihood_gaussian.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/linear_matrices.py
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/markov_chain.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/examples/markov_chain_and_GMM.py
+-rw-r--r--   0        0        0   219918 2020-02-02 00:00:00.000000 slimfit-0.1.4/docs/tutorial/basic_usage.ipynb
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/custom_numexpr_ivp.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/global_gaussian_mixture_models.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/linear_lsq.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/linear_lsq_array_parameters.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/linear_lsq_bounded.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/markov_ivp.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/readme.md
+-rw-r--r--   0        0        0    50049 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/data/GMM_dynamics.txt
+-rw-r--r--   0        0        0  1272537 2020-02-02 00:00:00.000000 slimfit-0.1.4/examples/output/scatter_and_fit.png
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 slimfit-0.1.4/interactive/interactive_ODE.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/.gitkeep
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/requirements-macOS-latest-3.10.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/requirements-macOS-latest-3.9.txt
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/requirements-ubuntu-latest-3.10.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/requirements-ubuntu-latest-3.9.txt
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/requirements-windows-latest-3.10.txt
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 slimfit-0.1.4/requirements/requirements-windows-latest-3.9.txt
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/__init__.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/__version__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/_version.py
+-rw-r--r--   0        0        0     7942 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/base.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/fit.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/fitresult.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/functions.py
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/loss.py
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/markov.py
+-rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/minimizers.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/models.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/np_funcs.py
+-rw-r--r--   0        0        0    14175 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/numerical.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/objective.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/operations.py
+-rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/parameter.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/reduce.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/symbols.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/typing.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 slimfit-0.1.4/slimfit/utils.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 slimfit-0.1.4/tests/test_operations.py
+-rw-r--r--   0        0        0    21748 2020-02-02 00:00:00.000000 slimfit-0.1.4/tests/test_slimfit.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 slimfit-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 slimfit-0.1.4/LICENSE
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 slimfit-0.1.4/README.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 slimfit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 slimfit-0.1.4/PKG-INFO
```

### Comparing `slimfit-0.1.3/CONTRIBUTING.rst` & `slimfit-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `slimfit-0.1.3/LICENSE` & `slimfit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slimfit-0.1.3/pyproject.toml` & `slimfit-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 [build-system]
-requires = [
-    "setuptools",
-    "tomli; python_version < '3.11'",
-    "versioneer[toml]"
-]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
 
 [project]
 name = "slimfit"
 description = "SymFit's little brother"
+authors = [
+  { name = "Jochem Smit", email = "jhsmit@gmail.com" },
+]
 readme = "README.md"
 license = {file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Science/Research",
-    "Topic :: Database"
 ]
 dependencies = [
     "numpy",
-    "scipy",
     "sympy",
     "tqdm",
-    "typing_extensions",
-    "pyyaml"
+    "typing-extensions",
+    "PyYAML",
+    "scipy",
+    "numdifftools",
 ]
 
 dynamic = ["version"]
 
-[project.urls]
-repository = "https://github.com/Jhsmit/slimfit"
-
 [project.optional-dependencies]
-docs = [
-    "mkdocs", "mkdocstrings[python]>=0.18", "mkdocs-material"
-]
 plot = [
-    "proplot",
-    "matplotlib==3.5.3",
+    "proplot>=0.9.7",
 ]
-interactive = [
-    "panel",
-    "bokeh",
-    "holoviz",
+docs = [
+    "mkdocs>=1.4.2",
+    "mkdocstrings[python]>=0.19.1",
+    "mkdocs-material>=8.5.11",
+    "pygments>=2.13.0",
+    "mkdocs-gen-files>=0.4.0",
+    "mkdocs-literate-nav>=0.5.0",
+    "mkdocs-jupyter>=0.22.0",
+    "jupyter>=1.0.0"
 ]
 dev = [
-    "pytest", "build", "black", "mypy"
+    "black[jupyter]>=22.12.0",
+    "setuptools-scm"
 ]
 
-[tool.setuptools]
-packages = ['slimfit']
+test = [
+    "pytest>=7.2.0",
+]
 
+[project.urls]
+Source = "https://github.com/Jhsmit/slimfit/"
+Documentation = "https://jhsmit.github.io/slimfit/"
 
-[tool.versioneer]
-VCS = "git"
-style = "pep440-pre"
-versionfile_source = "slimfit/_version.py"
-versionfile_build = "slimfit/_version.py"
-tag_prefix = "v"
-parentdir_prefix = "slimfit-"
+[tool.hatch.build]
+exclude = [
+    "_versioneer.py"
+]
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "slimfit/_version.py"
 
 [tool.flake8]
 max-line-length = 100
 ignore = "D203"
 exclude = [".git", "__pycache__", "build", "dist", "docs"]
 max-complexity = 10
 
 [tool.black]
-line-length = 100
+line-length = 100
+
+[tool.ruff]
+line-length = 100
```

### Comparing `slimfit-0.1.3/slimfit/functions.py` & `slimfit-0.1.4/slimfit/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def gaussian_numpy(
     x: np.array | float, mu: np.array | float, sig: np.array | float
 ) -> np.array | float:
     return 1 / (np.sqrt(2 * np.pi) * sig) * np.exp(-np.power((x - mu) / sig, 2) / 2)
 
 
 def gaussian_sympy(x: Symbol, mu: Symbol, sig: Symbol) -> Expr:
-    return sp.exp(-((x - mu) ** 2) / (2 * sig ** 2)) / (sp.sqrt(2 * np.pi) * sig)
+    return sp.exp(-((x - mu) ** 2) / (2 * sig**2)) / (sp.sqrt(2 * np.pi) * sig)
 
 
 def gaussian(
     x: Variable, mu: Matrix | MatrixNumExpr, sigma: Matrix | MatrixNumExpr
 ) -> Matrix | MatrixNumExpr:
     if mu.shape != sigma.shape:
         raise ValueError("Shape mismatch between 'mu' and 'sigma'")
```

### Comparing `slimfit-0.1.3/slimfit/loss.py` & `slimfit-0.1.4/slimfit/loss.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,31 @@
     mean_reduction,
     sum_reduction,
     concat_reduction,
 )
 
 
 class Loss(object):
+    """
+    Loss function base class.
+
+    Args:
+        weights: Optional dictionary of weights for each data point. Must match `ydata` in shape.
+        reduction: Reduction strategy to use. Defaults to "mean".
+
+    Attributes:
+        reduce: Callable that reduces the loss values.
+
+    """
+
     def __init__(
         self,
         weights: Optional[dict[str, npt.ArrayLike]] = None,
-        reduction: Literal["mean", "sum", "concat", "none", None] = "mean",
+        reduction: Literal["mean", "sum", "concat", "none", None] = "sum",
     ):
-
         self.weights = weights
         if reduction == "mean":
             self.reduce: ReductionStrategy = mean_reduction
         elif reduction == "sum":
             self.reduce: ReductionStrategy = sum_reduction
         elif reduction == "concat":
             self.reduce: ReductionStrategy = concat_reduction
@@ -51,36 +62,37 @@
     #     elif self.reduction in ["none", None]:
     #         return residuals
 
 
 # https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.least_squares.html#scipy.optimize.least_squares
 # https://pytorch.org/docs/stable/generated/torch.nn.MSELoss.html
 class L1Loss(Loss):
-    """L1 loss """
+    """L1 loss"""
 
+    # todo refactor ydata / ymodel?
     def __call__(
         self, dependent_data: dict[str, np.ndarray], target_data: dict[str, np.ndarray]
     ) -> np.ndarray | float:
-
         if self.weights is None:
             residuals = {k: (target_data[k] - dependent_data[k]) for k in target_data.keys()}
         else:
             residuals = {
                 k: (target_data[k] - dependent_data[k]) * self.weights[k]
                 for k in target_data.keys()
             }
 
         return self.reduce(residuals)
 
 
-class L2Loss(Loss):
+class SELoss(Loss):
+    """Squared error loss"""
+
     def __call__(
         self, y_data: dict[str, np.ndarray], y_model: dict[str, np.ndarray]
     ) -> np.ndarray | float:
-
         if self.weights is None:
             residuals = {k: (y_model[k] - y_data[k]) ** 2 for k in y_model.keys()}
         else:
             residuals = {
                 k: ((y_model[k] - y_data[k]) * self.weights[k]) ** 2 for k in y_model.keys()
             }
 
@@ -94,14 +106,15 @@
 
 class LogLoss(Loss):
     """Takes the elementwise logarithm of predicted input data
 
     Used in combination with maximum likelihood methods
 
     returns negative of the reductions are use in combination with minimizers rather than maximizers
+    #TODO move minus sign to objective
     """
 
     def __init__(
         self,
         weights: Optional[dict[str, npt.ArrayLike]] = None,
         reduction: Literal["mean", "sum", "concat"] = "sum",
     ):
@@ -112,15 +125,17 @@
         super().__init__(weights, reduction)
 
     def __call__(
         self, y_data: dict[str, np.ndarray], y_model: dict[str, np.ndarray]
     ) -> np.ndarray | float:
         if self.weights is None:
             # log_vals = {k: np.log(y_model[k]) for k in y_model.keys()}
-            log_vals = {k: np.log(np.clip(y_model[k], a_min=MIN_PROB, a_max=None)) for k in y_model.keys()}
+            log_vals = {
+                k: np.log(np.clip(y_model[k], a_min=MIN_PROB, a_max=None)) for k in y_model.keys()
+            }
 
         else:
             log_vals = {k: np.log(y_model[k] * self.weights[k]) for k in y_model.keys()}
 
         return -self.reduce(log_vals)
 
 
@@ -150,20 +165,19 @@
                 f"LogSumLoss does not support reduction {reduction!r}, only 'mean', 'sum', 'concat'"
             )
         super().__init__(weights, reduction)
 
     def __call__(
         self, y_data: dict[str, np.ndarray], y_model: dict[str, np.ndarray]
     ) -> np.ndarray | float:
-
         # from slimfit.minimizer import MIN_PROB
         if self.weights is None:
             log_vals = {
                 k: np.log(
-                    #y_model[k].sum(axis=self.sum_axis),
+                    # y_model[k].sum(axis=self.sum_axis),
                     np.clip(y_model[k].sum(axis=self.sum_axis), a_min=MIN_PROB, a_max=None)
                 )
                 for k in y_model.keys()
             }
 
         else:
             log_vals = {
```

### Comparing `slimfit-0.1.3/slimfit/markov.py` & `slimfit-0.1.4/slimfit/markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     """
     out = zeros(*m.shape)
     for i, j in np.ndindex(m.shape):
         elem = m[i, j]
         if elem == 0.0:
             continue
         else:
-            out[i, j] = base ** elem
+            out[i, j] = base**elem
 
     if sub_name is not None:
         subs = [(p, Parameter(name=sub_name(p.name))) for p in t.free_symbols]
         out = out.subs(subs)
 
     return out
```

### Comparing `slimfit-0.1.3/slimfit/minimizer.py` & `slimfit-0.1.4/slimfit/minimizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from __future__ import annotations
 
 import abc
 import time
+import warnings
 from dataclasses import asdict
 from functools import reduce, cached_property
 from operator import or_
 from typing import Optional, Any
 
 import numpy as np
 from scipy.optimize import minimize
 from sympy import Symbol
 from tqdm.auto import trange
 
 from slimfit import Model, NumExprBase
 from slimfit.fitresult import FitResult
-from slimfit.loss import Loss
+from slimfit.loss import Loss, LogSumLoss
 from slimfit.objective import ScipyObjective, pack, unpack, ScipyEMObjective
 
 # from slimfit.models import NumericalModel
 from slimfit.operations import Mul
 from slimfit.parameter import Parameters, Parameter
-from slimfit.utils import get_bounds, overlapping_model_parameters
+from slimfit.utils import get_bounds, intersecting_component_symbols
 
 # TODO parameter which needs to be inferred / set somehow
 STATE_AXIS = -2
 
+
 # dataclass?
 class Minimizer(metaclass=abc.ABCMeta):
     def __init__(
         self,
-        numerical_model: Model,
+        model: Model,
         parameters: Parameters,
         loss: Loss,
-        xdata: dict[str, np.array],
-        ydata: dict[str, np.array],
+        xdata: dict[str, np.ndarray],
+        ydata: dict[str, np.ndarray],
     ):
-        if not numerical_model.numerical:
-            raise ValueError("The given model should be numerical")
-
-        self.model = numerical_model
+        self.model = model
         self.loss = loss
         self.xdata = xdata
         self.ydata = ydata
         self.parameters = parameters
 
     # subset of parameters which are fixed
+    # TODO dont think they need to be cached
+    # and probaby we should use self.parameters.free / self.parameters.fixed
     @cached_property
     def fixed_parameters(self) -> Parameters:
         return Parameters([p for p in self.parameters if p.fixed])
 
     @cached_property
     def free_parameters(self) -> Parameters:
         return Parameters([p for p in self.parameters if not p.fixed])
@@ -61,52 +62,59 @@
         print("guess on minimizer")
         for p in self.parameters:
             print(p.name, p.fixed)
 
         return {p.name: np.asarray(p.guess) for p in self.parameters if not p.fixed}
 
     def get_bounds(self) -> list[tuple[float | None, float | None]] | None:
-        bounds = [(p.lower_bound, p.upper_bound) for p in self.free_parameters]
+        bounds = []
+        for p in self.free_parameters:
+            size = np.prod(p.shape, dtype=int)
+            bounds += [(p.lower_bound, p.upper_bound)] * size
 
         if all((None, None) == b for b in bounds):
             return None
         else:
             return bounds
 
     @abc.abstractmethod
     def execute(self, **minimizer_options) -> FitResult:
         ...
 
 
 class ScipyMinimizer(Minimizer):
-    def execute(self, **minimizer_options):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         param_shapes = {p.name: p.shape for p in self.free_parameters}
-
-        objective = ScipyObjective(
-            model=self.model,
+        self.objective = ScipyObjective(
+            model=self.model.numerical,
             loss=self.loss,
             xdata=self.xdata | self.fixed_parameters.guess,
             ydata=self.ydata,
             shapes=param_shapes,
         )
 
+    def execute(self, **minimizer_options):
         x = pack(self.free_parameters.guess.values())
 
         result = minimize(
-            objective, x, bounds=self.get_bounds(), options=self.rename_options(minimizer_options)
+            self.objective,
+            x,
+            bounds=self.get_bounds(),
+            options=self.rename_options(minimizer_options),
         )
 
         gof_qualifiers = {
             "loss": result["fun"],
         }
 
-        parameter_values = unpack(result.x, param_shapes)
+        parameter_values = unpack(result.x, self.objective.shapes)
         result_dict = dict(
-            parameters=parameter_values,
-            fixed_parameters=self.fixed_parameters,
+            fit_parameters=parameter_values,
+            fixed_parameters=self.fixed_parameters.guess,
             gof_qualifiers=gof_qualifiers,
             guess=self.free_parameters.guess,
             base_result=result,
         )
 
         # todo pass to superclass generalize fitresult function
         return FitResult(**result_dict)
@@ -124,26 +132,44 @@
 # todo refactor to EM Optimizer?
 class LikelihoodOptimizer(Minimizer):
     """
     Assumed `loss` is `LogLoss`
 
     """
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not isinstance(self.loss, LogSumLoss):
+            warnings.warn("Using non-log loss in likelihood optimizer")
+        param_shapes = {p.name: p.shape for p in self.free_parameters}
+        # TODO rename and generalize?
+        self.objective = ScipyObjective(
+            model=self.model.numerical,
+            loss=self.loss,
+            xdata=self.xdata | self.fixed_parameters.guess,
+            ydata=self.ydata,
+            shapes=param_shapes,
+        )
+
     def execute(self, max_iter=250, patience=5, stop_loss=1e-7, verbose=True) -> FitResult:
         # parameters which needs to be passed / inferred
         # Split top-level multiplications in the model as they can be optimized in log likelihood independently
+        # TODO model should have this as property / method
         components: list[tuple[Symbol, NumExprBase]] = []  # todo tuple LHS as variable
-        for lhs, rhs in self.model.items():
+        for lhs, rhs in self.model.numerical.items():
             if isinstance(rhs, Mul):
                 components += [(lhs, elem) for elem in rhs.values()]
             else:
                 components.append((lhs, rhs))
 
         # Find the sets of components which have common parameters and thus need to be optimized together
-        sub_models = overlapping_model_parameters(components, self.free_parameters.symbols)
+        sub_models = intersecting_component_symbols(components, self.free_parameters.symbols)
+
+        # Remove sub models without symbols
+        sub_models = [m for m in sub_models if m.symbols]
 
         pbar = trange(max_iter, disable=not verbose)
         t0 = time.time()
 
         parameters_current = self.free_parameters.guess  # initialize parameters
         prev_loss = 0.0
         no_progress = 0
@@ -155,35 +181,37 @@
             # posterior dict has values with shapes equal to y_model
             # which is (dataopints, states, 1)
             posterior = {k: v / v.sum(axis=STATE_AXIS, keepdims=True) for k, v in y_model.items()}
 
             # dictionary of new parameter values for in this iteration
             parameters_step = {}
             common_kwargs = dict(
-                loss=self.loss, xdata=self.xdata, ydata=self.ydata, posterior=posterior,
+                loss=self.loss,
+                xdata=self.xdata,
+                ydata=self.ydata,
+                posterior=posterior,
             )
             for sub_model in sub_models:
                 # At the moment we assume all callables in the sub models to be MatrixCallables
                 # determine the kind
-                kinds = [c.kind for c in sub_model.values()]
+                kinds = [getattr(c, "kind", None) for c in sub_model.values()]
                 # Filter the general list of parameters to reduce it down to the parameters
                 # this model accepts
                 # the sub model also needs to the fixed parameters to correctly be able to
                 # call the model; GMM also needs it for finding sigma
                 sub_parameters = sub_model.filter_parameters(self.parameters)
                 if all(k == "constant" for k in kinds):
                     # Constant optimizer doesnt use loss, xdata, ydata,
                     opt = ConstantOptimizer(sub_model, sub_parameters, **common_kwargs)
                     parameters = opt.step()
-                elif all(k == "gmm" for k in kinds):
+                elif all(k == "gmm" for k in kinds) and not sub_parameters.has_bounds:
                     # Loss is not used for GMM optimizer step
                     opt = GMMOptimizer(sub_model, sub_parameters, **common_kwargs)
                     parameters = opt.step()
                 else:
-
                     # Previous code:
                     # updated_parameters = [
                     #     Parameter(**(asdict(p) | {"guess": parameters_current.get(p.name) or self.fixed_parameters.guess[p.name]  }))
                     #     for p in sub_parameters
                     # ]
 
                     # New; needs improvement as it accesses `_names`
@@ -192,27 +220,28 @@
                     }
                     updated_parameters = sub_parameters.update_guess(current_sub)
 
                     # todo loss is not used; should be EM loss while the main loop uses Log likelihood loss
                     opt = ScipyEMOptimizer(sub_model, updated_parameters, **common_kwargs)
 
                     scipy_result = opt.execute()
-                    parameters = scipy_result.parameters
+                    parameters = scipy_result.fit_parameters
                     base_result["scipy"] = scipy_result
 
-                # collect parameters of this sub_model into parmaeters dict
+                # collect parameters of this sub_model into parameters dict
                 parameters_step |= parameters
 
             # update for next iteration
             parameters_current = parameters_step
 
             # loss
             improvement = prev_loss - loss
             prev_loss = loss
             pbar.set_postfix({"improvement": improvement})
+
             if np.isnan(improvement):
                 break
             elif improvement < stop_loss:
                 no_progress += 1
             else:
                 no_progress = 0
 
@@ -221,41 +250,41 @@
 
         tdelta = time.time() - t0
         gof_qualifiers = {
             "loss": loss,
             "log_likelihood": -loss,
             "n_iter": i + 1,
             "elapsed": tdelta,
-            "iter/s": tdelta / (i + 1),
+            "iter/s": (i + 1) / tdelta,
         }
 
         result = FitResult(
-            parameters=parameters_current,
+            fit_parameters=parameters_current,
             fixed_parameters=self.fixed_parameters.guess,
             gof_qualifiers=gof_qualifiers,
             guess=self.free_parameters.guess,
             base_result=base_result,
         )
 
         return result
 
 
 class EMOptimizer(Minimizer):
     def __init__(
         self,
-        numerical_model: Model,
-        parameters: list[Parameter],  # Parameters?
+        model: Model,
+        parameters: list[Parameter] | Parameters,  # Parameters?
         loss: Loss,
         xdata: dict[str, np.array],
         ydata: dict[str, np.array],
         posterior: dict[str, np.array],
     ):
         self.posterior = posterior
         super().__init__(
-            numerical_model=numerical_model,
+            model=model,
             parameters=parameters,
             loss=loss,
             xdata=xdata,
             ydata=ydata,
         )
 
     @abc.abstractmethod
@@ -300,16 +329,16 @@
             "log_likelihood": -loss,
             "n_iter": i,
             "elapsed": tdelta,
             "iter/s": tdelta / i,
         }
 
         result = FitResult(
-            parameters=parameters_current,
-            fixed_parameters=self.model.fixed_parameters,
+            fit_parameters=parameters_current,
+            fixed_parameters=self.model.fixed_parameters.guess,
             gof_qualifiers=gof_qualifiers,
             guess=self.guess,
             # model=self.model,
             # data={**self.xdata, **self.ydata},
         )
 
         return result
@@ -413,15 +442,14 @@
                     denom += denom_i
             parameters[parameter.name] = num / denom
 
         return parameters
 
 
 class ScipyEMOptimizer(EMOptimizer):
-
     # TODO this is an abstract method
     def step(self):
         ...
 
     def execute(self, **minimizer_options):
         param_shapes = {p.name: p.shape for p in self.free_parameters}
 
@@ -445,46 +473,45 @@
         # what about the pack / unpack?
         result = minimize(
             objective,
             x,
             # args=(self.model, self.loss, self.posterior),
             # args=(self.parameter_names, self.xdata, self.posterior, self.model, self.loss,),
             bounds=self.get_bounds(),
-            **options
+            **options,
         )
 
         gof_qualifiers = {
             "loss": result["fun"],
         }
 
         parameter_values = unpack(result.x, param_shapes)
 
         result_dict = dict(
-            parameters=parameter_values,
-            fixed_parameters=self.fixed_parameters,
+            fit_parameters=parameter_values,
+            fixed_parameters=self.fixed_parameters.guess,
             gof_qualifiers=gof_qualifiers,
             guess=self.free_parameters.guess,
             base_result=result,
         )
 
         # todo pass to superclass generalize fitresult function
         # or functional
         return FitResult(**result_dict)
 
     # TODO duplicate code
     def to_fitresult(self, result) -> FitResult:
-
         parameters = self.model.parameters.unpack(result.x)
 
         gof_qualifiers = {
             "loss": result["fun"],
         }
 
         fit_result = FitResult(
-            parameters=parameters,
+            fit_parameters=parameters,
             gof_qualifiers=gof_qualifiers,
             guess=self.guess,
             base_result=result,
         )
 
         return fit_result
 
@@ -513,12 +540,11 @@
 
 def minfunc(
     x: np.ndarray,  # array of parameters
     model: Model,
     loss: Loss,
     dependent_data: dict,  # corresponding measurements; target data
 ) -> float:
-
     parameter_values = model.parameters.unpack(x)
     predicted = model(**parameter_values)
 
     return loss(dependent_data, predicted)
```

### Comparing `slimfit-0.1.3/slimfit/models.py` & `slimfit-0.1.4/slimfit/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import itertools
 from typing import Union, ItemsView, ValuesView, KeysView, Optional
 
 import numpy.typing as npt
 from sympy import Expr, MatrixBase, Symbol
 
+import slimfit.base
 import slimfit.numerical as numerical
 from slimfit.parameter import Parameters
 
 
-class Model(numerical.CompositeExpr):
+class Model(slimfit.base.CompositeExpr):
     def __init__(
-        self, model_dict: dict[Symbol | str, Expr | numerical.NumExprBase | MatrixBase],
+        self,
+        expr: dict[Symbol | str, Expr | slimfit.base.NumExprBase | MatrixBase],
     ):
-
         # currently typing has a small problem where keys are expected to be `str`, not symbol
-        super().__init__(model_dict)
+        super().__init__(expr)
 
     def __repr__(self):
         return f"Model({self.expr.__repr__()})"
 
     # def __getitem__(self, item: Union[str, Symbol]) -> numerical.NumExprBase:
     #     if isinstance(item, str):
     #         item = self.symbols[item]
@@ -29,7 +30,37 @@
 
     @property
     def dependent_symbols(self) -> dict[str, Symbol]:
         # todo needs to be updated
         """Variables corresponding to dependent (measured) data, given as keys in the model dict"""
 
         return {symbol.name: symbol for symbol in self.expr.keys()}
+
+    @property
+    def components(self) -> dict[str, slimfit.base.NumExprBase]:
+        """all NumExprBase components in the model
+        keys should be such that their commectivity can be reconstructed ?
+        ie {Mul[0]MatMul[1]: <component> ...}
+        which tells us that this component is the second element of a matmul whose result
+        is the first component in a mul
+        """
+        raise NotImplementedError("not yet implemented")
+
+        # return {symbol.name: expr for symbol, expr in self.expr.items()}
+
+
+class Eval(slimfit.base.CompositeExpr):
+    def __init__(self, expr: Expr | slimfit.base.NumExprBase | MatrixBase):
+        super().__init__({"_y": expr})
+
+    def __call__(self, **kwargs):
+        ans = super().__call__(**kwargs)
+        return ans["_y"]
+
+    def __repr__(self) -> str:
+        return f"Eval({self.expr['_y'].__repr__()})"
+
+    def to_numerical(self):
+        args = (numerical.to_numerical(expr) for expr in self.values())
+        instance = self.__class__(*args)
+
+        return instance
```

### Comparing `slimfit-0.1.3/slimfit/numerical.py` & `slimfit-0.1.4/slimfit/numerical.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,62 @@
 from __future__ import annotations
 
-import itertools
-from functools import cached_property, reduce
-from operator import or_
+from functools import cached_property
 from typing import (
     Union,
     Callable,
     Optional,
     Any,
-    Mapping,
     Iterable,
     TYPE_CHECKING,
-    KeysView,
-    ItemsView,
-    ValuesView,
 )
 
 import numpy as np
 from scipy.integrate import solve_ivp
 from sympy import Expr, MatrixBase, lambdify, HadamardProduct, Matrix, Symbol
 
-from slimfit.base import SymbolicBase
+from slimfit.base import CompositeExpr, NumExprBase
 
 # from slimfit.base import SymbolicBase
-from slimfit.parameter import Parameters, Parameter
-from slimfit.symbols import FitSymbol
 from slimfit.typing import Shape
 
 if TYPE_CHECKING:
     from slimfit import Model
 
-# @dataclass
-class NumExprBase(SymbolicBase):
-    """Symbolic expression which allows calling cached lambified expressions
-    subclasses must implement `symbols` attribute / property
-    """
-
-    # def __init__(
-    #     self,
-    # ):
-    #
-    #     # Accepted parameters are a subset of `symbols`
-    #     # #todo property with getter / setter where setter filters parameters?
-    #     # self.parameters = Parameters({name: p for name, p in parameters.items() if name in self.symbols})
-
-    @property
-    def shape(self) -> Shape:
-        shapes = self.shapes.values()
-
-        return np.broadcast_shapes(*shapes)
-
-    def parse_kwargs(self, **kwargs) -> dict[str, np.ndarray]:
-        """Parse kwargs and take only the ones in `free_parameters`"""
-        try:
-            arguments: dict[str, np.ndarray | float] = {k: kwargs[k] for k in self.symbol_names}
-        except KeyError as e:
-            print(kwargs.keys())
-            raise KeyError(f"Missing value for parameter {e}") from e
-
-        return arguments
-
 
 class DummyNumExpr(NumExprBase):
     """Dummy callable object which returns supplied 'obj' when called
     Has no parameters or symbols
     """
 
     def __init__(self, obj: Any, *args, **kwargs):
+        #
         super().__init__(*args, **kwargs)
         self.obj = obj
 
     def __call__(self, **kwargs):
         return self.obj
 
     @property
     def symbols(self) -> set[Symbol]:
         return set()
 
-
-class ArrayNumExpr(DummyNumExpr):
     @property
     def shape(self) -> Shape:
-        return self.obj.shape
+        try:
+            return self.obj.shape
+        except AttributeError:
+            return ()
 
 
 # TODO frozen dataclass?
 class NumExpr(NumExprBase):
     def __init__(
-        self, expr: Expr,
+        self,
+        expr: Expr,
     ):
         if not isinstance(expr, (Expr, MatrixBase)):
             # TODO subclass such that typing is correct
             raise TypeError(f"Expression must be an instance of `Expr` or ")
         self.expr = expr
 
         # super().__init__()
@@ -110,15 +75,14 @@
     @cached_property
     def lambdified(self) -> Callable:
         ld = lambdify(sorted(self.symbols, key=str), self.expr)
 
         return ld
 
     def __call__(self, **kwargs: float) -> np.ndarray | float:
-
         # try:
         #     parameters: dict[str, np.ndarray | float] = {
         #         k: kwargs[k] for k in self.parameters.keys()
         #     }
         # except KeyError as e:
         #     raise KeyError(f"Missing value for parameter {e}") from e
 
@@ -129,17 +93,19 @@
         return f"NumExpr({self.expr})"
 
 
 # todo name via kwargs to super
 # = composite num expr"?
 class MatrixNumExpr(NumExpr):
     def __init__(
-        self, expr: MatrixBase, name: Optional[str] = None, kind: Optional[str] = None,
+        self,
+        expr: MatrixBase,
+        name: Optional[str] = None,
+        kind: Optional[str] = None,
     ):
-
         if not isinstance(expr, MatrixBase):
             raise TypeError("Expression must be an instance of MatrixParameter or sympy.Matrix")
         self._name = name
 
         # Callable type is used by minimizers to determine solving strategy
         if kind is None:
             self.kind = identify_expression_kind(expr)
@@ -301,126 +267,32 @@
 
     def __call__(self, **kwargs):
         m_vals = super().__call__(**kwargs)
 
         np.broadcast_to(...)
 
 
-class DummyVariableMatrix(MatrixNumExpr):
-    """
-    Matrix callable which takes an additional variable such that called returned shape is expanded to accomodate its
-    shapes
-    """
-
-    def __init__(
-        self, x: Symbol, m: Matrix, kind: Optional[str] = None, name: Optional[str] = None,
-    ):
-        raise NotImplementedError("Not implemented")
-        self.x = x
-        super().__init__(m, kind=kind, name=name)
-
-    @property
-    def symbols(self) -> dict[str, Symbol]:
-        symbols = super().symbols | {self.x}
-        return symbols
-
-
 # different class for Symbolic / Numerical ?
 class LambdaNumExpr(NumExprBase):
-    def __init__(self, func, symbols: Iterable[Symbol],) -> None:
+    def __init__(
+        self,
+        func,
+        symbols: Iterable[Symbol],
+    ) -> None:
         self.func = func
         self._symbols = set(symbols)
 
     @property
     def symbols(self):
         return self._symbols
 
     def __call__(self, **kwargs):
         return self.func(**self.parse_kwargs(**kwargs))
 
 
-# refactor to Hybrid ?
-class CompositeExpr(SymbolicBase):
-    """Can be both numerical or symbolic """
-
-    def __init__(
-        self, expr: dict[str | Symbol, NumExprBase | Expr | CompositeExpr],
-    ):
-        self.expr = expr
-
-    def __call__(self, **kwargs) -> dict[str, np.ndarray]:
-        return {expr_name: expr(**kwargs) for expr_name, expr in self.expr.items()}
-
-    def __getitem__(self, item) -> NumExprBase | Expr:
-        return self.expr.__getitem__(item)
-
-    @property
-    def numerical(self) -> bool:
-        return all(isinstance(v, (NumExprBase, CompositeExpr)) for v in self.values())
-
-    def keys(self) -> KeysView[str]:
-        return self.expr.keys()
-
-    def values(self) -> ValuesView[NumExprBase, Expr]:
-        return self.expr.values()
-
-    def items(self) -> ItemsView[str, NumExprBase, Expr]:
-        return self.expr.items()
-
-    def to_numerical(self):
-        num_expr = {str(k): to_numerical(expr) for k, expr in self.items()}
-
-        instance = self.__class__(num_expr)
-        return instance
-
-    @cached_property
-    def symbols(self) -> set[Symbol]:
-        """Return symbols in the CompositeNumExpr.
-        sorting is by dependent_variables, variables, parameters, then by alphabet
-        """
-
-        # this fails because `free_symbols` is a dict on NumExpr but `set` on Expr
-
-        symbols = set()
-        for rhs in self.values():
-            if isinstance(rhs, (Expr, MatrixBase)):
-                symbols |= rhs.free_symbols
-            else:
-                try:
-                    symbols |= set(rhs.symbols)
-                except AttributeError:
-                    # RHS doesnt have any symbols; for example might be a numpy array
-                    pass
-
-            # symbols = getattr(rhs, 'free_symbols')
-            # try:
-            #     # rhs is a sympy `Expr` and has `free_symbols` as a set
-            #     symbols |= rhs.free_symbols
-            # except TypeError:
-            #     # rhs is a slimfit `NumExpr`
-            #     symbols |= set(rhs.symbols)
-            # except AttributeError:
-            #     # RHS doesnt have any symbols; for example might be a numpy array
-            #     pass
-        return symbols
-
-    @property
-    def shapes(self) -> dict[str, Shape]:
-        """shapes of symbols"""
-        return reduce(or_(expr.shapes for expr in self.expr.values()))
-
-    @property
-    def shape(self) -> Shape:
-        """
-        Base class shape is obtained from broadcasting all expressing values together
-        """
-        shapes = (expr.shape for expr in self.values())
-        return np.broadcast_shapes(*shapes)
-
-
 class GMM(CompositeExpr):
     # todo can also be implemented as normal NumExpr but with broadcasting parameter shapes
     # important is that GMM class allows users to find oud positions of parmaeters in mu / sigma
     # matrices for EM GMM optimization.
 
     def __init__(
         self,
@@ -463,16 +335,30 @@
         return instance
 
     @property
     def shape(self) -> Shape:
         shape = super().shape
         return shape + (1,)
 
+    @property
+    def states(self) -> Optional[list[str]]:
+        """
+        List of state names, if naming scheme of mu's is of format `mu_<state_name>`.
+        """
+
+        mus, suffices = zip(*(elem.name.split("_") for elem in self["mu"]))
+
+        if all((mu == "mu" for mu in mus)):
+            return list(suffices)
+        else:
+            return None
+
     # TODO GMM should have API to find the index of the state given a symbol
-    #def state_index(self, ...):
+    # def state_index(self, ...):
+
 
 class MarkovIVP(CompositeExpr):
     """Uses scipy.integrate.solve_ivp to numerically find time evolution of a markov process
         given a transition rate matrix.
 
     Returned shape is (len(t_var), len(y0), 1), or (<datapoints>, <states>, 1)
 
@@ -482,15 +368,14 @@
         self,
         t: Symbol | NumExpr,
         trs_matrix: Matrix | MatrixNumExpr,
         y0: Matrix | MatrixNumExpr,
         domain: Optional[tuple[float, float]] = None,
         **ivp_kwargs,
     ):
-
         expr = {"t": t, "trs_matrix": trs_matrix, "y0": y0}
 
         super().__init__(expr)
 
         ivp_defaults = {"method": "Radau"}
         self.ivp_defaults = ivp_defaults | ivp_kwargs
         self.domain = domain
@@ -551,19 +436,18 @@
 
 
 def to_numerical(
     expression: Union[NumExprBase, Expr, MatrixBase | Model | CompositeExpr],
 ) -> NumExprBase | CompositeExpr:
     """Converts sympy expression to slimfit numerical expression
 
-        if the expressions already is an NumExpr; the object is modified in-place by setting
-        the parameters
+    if the expressions already is an NumExpr; the object is modified in-place by setting
+    the parameters
 
     """
-    from slimfit.models import Model
 
     if hasattr(expression, "to_numerical"):
         return expression.to_numerical()
     # elif isinstance(expression, Model):
     #     model_dict = {lhs: to_numerical(rhs) for lhs, rhs in expression.items()}
     #     from slimfit.models import NumericalModel
     #
@@ -573,12 +457,12 @@
 
         return Mul(*(to_numerical(arg) for arg in expression.args))
     elif isinstance(expression, MatrixBase):
         return MatrixNumExpr(expression)
     elif isinstance(expression, Expr):
         return NumExpr(expression)
     elif isinstance(expression, np.ndarray):
-        return ArrayNumExpr(expression)
+        return DummyNumExpr(expression)
     elif isinstance(expression, NumExprBase):
         return expression
     else:
         raise TypeError(f"Invalid type {type(expression)!r}")
```

### Comparing `slimfit-0.1.3/slimfit/parameter.py` & `slimfit-0.1.4/slimfit/parameter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 from collections import UserDict, UserList
-from dataclasses import dataclass, field, asdict
+from dataclasses import dataclass, field, asdict, replace
 from enum import Enum
 from functools import cached_property
 from typing import Iterable, Optional
 
 import numpy as np
 import numpy.typing as npt
 from sympy import Expr, Symbol
@@ -16,26 +16,25 @@
     CONTINUOUS = "continuous"
     DISCRETE = "discrete"
     BOOLEAN = "boolean"
 
 
 @dataclass(frozen=True)
 class Parameter:
-    symbol: Expr
+    symbol: Expr  # allow `str` after which __init___ finds the symbol?
     guess: float | int | np.ndarray = field(default=1.0)
     lower_bound: float | int | np.ndarray = field(default=None)
     upper_bound: float | int | np.ndarray = field(default=None)
-    # TODO partially fixing an array parameter is not supported
-    # perhaps users should use Matrix instead if they want this type of functionality
     fixed: bool = field(default=False)
 
     def __post_init__(self):
-
         # If the `guess` has a shape, it must be the same as the symbol shape,
         # if it has any.
+        if not isinstance(self.guess, (float, int, np.ndarray)):
+            raise TypeError(f"Guess must be a float, int, or ndarray, not {type(self.guess)}")
         guess_shape = getattr(self.guess, "shape", None)
         symbol_shape = getattr(self.symbol, "shape", guess_shape)
         if guess_shape != symbol_shape:
             raise ValueError(f"Guess shape for symbol {self.symbol} does not match symbol shape")
 
     @property
     def param_type(self) -> ParamType:
@@ -66,36 +65,51 @@
     def name(self) -> str:
         # Do symbols always have names?
         return self.symbol.name
 
 
 # frozen?
 # frozen might not be nessecary but fit should make a copy to prevent modification
+# currently Parameter objects are frozen / immutable
+# should be set: https://stackoverflow.com/questions/57132624/why-there-is-no-userset-class-defined-in-python
 class Parameters(UserList):
     """Parameter list object
 
     or maybe it should be a dict?
     Could potentially help the `Objective` to/from flat array of guesses for argument of scipy.minimize
     """
 
+    def __init__(self, initlist=None):
+        initlist = initlist or []
+        if not all(isinstance(p, Parameter) for p in initlist):
+            raise ValueError("All items must be of type Parameter")
+        symbols = {p.symbol for p in initlist}
+        if len(symbols) != len(initlist):
+            raise ValueError("All parameters must be unique")
+        super().__init__(initlist)
+
     @classmethod
     def from_symbols(
         cls,
         symbols: Iterable[Symbol],
         parameters: dict[str, npt.ArrayLike] | Iterable[str] | str = None,
     ) -> Parameters:
-
         symbol_dict = {symbol.name: symbol for symbol in sorted(symbols, key=str)}
 
         if isinstance(parameters, str):
             p_list = [Parameter(symbol_dict[k]) for k in re.split("; |, |\*|\s+", parameters)]
         elif isinstance(parameters, list):
             p_list = [Parameter(symbol_dict[k]) for k in parameters]
         elif isinstance(parameters, dict):
-            p_list = [Parameter(symbol_dict[k], guess=v) for k, v in parameters.items()]
+            p_list = []
+            for k, v in parameters.items():
+                if isinstance(v, (float, int)):
+                    p_list.append(Parameter(symbol_dict[k], guess=v))
+                else:
+                    p_list.append(Parameter(symbol_dict[k], guess=np.array(v)))
         elif parameters is None:
             p_list = [Parameter(symbol) for symbol in symbol_dict.values()]
         else:
             raise ValueError("Invalid values for 'parameters' or 'guess'")
         return cls(p_list)
 
     @property
@@ -112,30 +126,95 @@
         if isinstance(item, Parameter):
             return super().index(item, *args)
         elif isinstance(item, Symbol):
             return self._symbols.index(item, *args)
         else:
             return self._names.index(item, *args)
 
-    def set(self, symbol_or_name: Symbol | str, **kwargs):
+    def get(self, symbol_or_name: Symbol | str) -> Optional[Parameter]:
+        """Returns the parameter with the given symbol or name, or None if not found."""
+
+        try:
+            return self[self.index(symbol_or_name)]
+        except KeyError:
+            return None
+
+    def set(self, symbol_or_name: Symbol | str, **kwargs) -> Parameters:
+        """
+        Set attributes of a parameter in-place.
+
+        Args:
+            symbol_or_name: Symbol or name of the parameter to set.
+            **kwargs: Additional keyword arguments to set on the parameter.
+
+        Returns:
+            The `Parameters object (self).
+        """
         idx = self.index(symbol_or_name)
 
         # todo sanitize kwargs
+        # todo replace
         self[idx] = Parameter(**(asdict(self[idx]) | kwargs))
 
+        return self
+
+    def replace(self, symbol_or_name: Symbol | str, **kwargs) -> Parameters:
+        """
+        Replace a parameter fields and create a new `Parameters` object .
+
+        Args:
+            symbol_or_name: Symbol or name of the parameter to replace.
+            **kwargs: Additional keyword arguments to set on the parameter.
+
+        Returns:
+            New parameters object with replaced Parameter object.
+        """
+        idx = self.index(symbol_or_name)
+
+        new_parameters = Parameters(self)
+        new_parameters[idx] = replace(self[idx], **kwargs)
+
+        return new_parameters
+
     def update_guess(self, guess: dict[str | Symbol, np.ndarray | float]) -> Parameters:
-        """returns a new parameters object where """
+        """returns a new parameters object where guesses are updated"""
 
         p_out = Parameters(self)
         for identifier, value in guess.items():
             idx = p_out.index(identifier)
             p_out[idx] = Parameter(**(asdict(self[idx]) | dict(guess=value)))
 
         return p_out
 
     @property
     def guess(self) -> dict[str, np.ndarray]:
         return {p.name: np.asarray(p.guess) for p in self}
 
     @property
+    def shapes(self) -> dict[str, tuple[int, ...]]:
+        return {p.name: p.shape for p in self}
+
+    @property
     def symbols(self) -> set[Symbol]:
         return set(p.symbol for p in self)
+
+    @property
+    def free(self) -> Parameters:
+        """Returns a new `Parameters` object with only the free parameters."""
+        return Parameters([p for p in self if not p.fixed])
+
+    @property
+    def fixed(self) -> Parameters:
+        """Returns a new `Parameters` object with only the fixed parameters."""
+        return Parameters([p for p in self if p.fixed])
+
+    @property
+    def has_bounds(self) -> bool:
+        """Return `True` if any of the parameters has bounds."""
+
+        for p in self:
+            if p.lower_bound is not None:
+                return True
+            if p.upper_bound is not None:
+                return True
+
+        return False
```

### Comparing `slimfit-0.1.3/slimfit/reduce.py` & `slimfit-0.1.4/slimfit/reduce.py`

 * *Files identical despite different names*

### Comparing `slimfit-0.1.3/slimfit/symbols.py` & `slimfit-0.1.4/slimfit/symbols.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import itertools
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
-from sympy import Symbol, zeros, Expr, MatrixBase
+from sympy import Symbol, zeros, Expr, MatrixBase, Matrix
 from sympy.core.cache import clear_cache
 
 
 def get_symbols(*symbolic_objects) -> dict[str, Symbol]:
     """Returns a dictionary of symbols
     if no object is given, only returns FitSymbols
     otherwise returns dict of symbols in the object
@@ -18,19 +19,19 @@
     else:
         symbols = set()
         for symbolic_object in symbolic_objects:
             if isinstance(symbolic_object, dict):
                 symbols = set()
                 for entry in itertools.chain(symbolic_object.keys(), symbolic_object.values()):
                     try:
-                        # rhs is a sympy `Expr` and has `free_symbols` as a set
-                        symbols |= rhs.free_symbols
+                        # entry is a sympy `Expr` and has `free_symbols` as a set
+                        symbols |= entry.free_symbols
                     except TypeError:
                         # rhs is a slimfit `NumExpr` and has a `free_symbols` dictionary
-                        symbols |= set(rhs.free_symbols.values())
+                        symbols |= set(entry.free_symbols.values())
                 return
             elif isinstance(symbolic_object, (Expr, MatrixBase)):
                 symbols |= symbolic_object.free_symbols
                 # return {symbol.name: symbol for symbol in sorted(symbolic_object.free_symbols, key=str)}
             else:
                 raise TypeError(f"Invalid type {type(symbolic_object)!r}")
 
@@ -70,15 +71,14 @@
 
 def symbol_matrix(
     name: Optional[str] = None,
     shape: Optional[tuple[int, ...]] = None,
     names: Optional[npt.ArrayLike] = None,
     suffix: Optional[npt.ArrayLike] = None,
 ) -> Matrix:
-
     if shape is None:
         if names is not None:
             shape = (len(names), 1)
         elif suffix is not None:
             shape = (len(suffix), 1)
         else:
             raise ValueError("If 'shape' is not given, must specify 'names' or 'suffix'")
@@ -97,14 +97,16 @@
             for i, j in np.ndindex(shape):
                 names[i, j] = f"{name}_{suffix[i, j]}"
     else:
         names = np.array(names)
 
     matrix = zeros(*shape)
     for i, j in np.ndindex(shape):
-        matrix[i, j] = Symbol(name=names[i, j],)
+        matrix[i, j] = Symbol(
+            name=names[i, j],
+        )
 
     return matrix
 
 
 # SORT_PRIORITY = [Variable, Probability, Parameter]
 # SORT_KEY = lambda x: (SORT_PRIORITY.index(type(x)), x.name)
```

### Comparing `slimfit-0.1.3/slimfit/typing.py` & `slimfit-0.1.4/slimfit/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 DataType = TypeVar("DataType")
 
 
 # STRATEGY / PROTOCOL?
 # class Data(UserDict, Generic[DataType]):
 class Data(Protocol[DataType]):
-
     ...
 
     def __getitem__(self, item) -> DataType:
         return super().__getitem__(item)
 
     def __setitem__(self, key: str, value: DataType) -> None:
         return super().__setitem__(key, value)
```

### Comparing `slimfit-0.1.3/tests/test_slimfit.py` & `slimfit-0.1.4/tests/test_slimfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 from pathlib import Path
 
 import pytest
-
-# from dont_fret.em_fit.datagen import generate_dataset
-from sympy import HadamardProduct, Matrix, exp, Symbol
-
-# import numpy as np
-
+from sympy import HadamardProduct, Matrix, exp, Symbol, symbols
 from slimfit.fit import Fit
 from slimfit.functions import gaussian, gaussian_sympy, gaussian_numpy
-from slimfit.loss import LogLoss
-
-# from slimfit.markov import generate_transition_matrix, extract_states
-# from slimfit.minimizer import LikelihoodOptimizer
-from slimfit.operations import Mul, MatMul
-from slimfit.models import Model
+from slimfit.loss import LogLoss, SELoss
+from slimfit.operations import Mul, MatMul, Sum, Add
+from slimfit.models import Eval, Model
 from slimfit.numerical import MatrixNumExpr, NumExpr, GMM, to_numerical, LambdaNumExpr, MarkovIVP
 from slimfit.symbols import (
     symbol_matrix,
     clear_symbols,
     get_symbols,
 )
 from slimfit.loss import LogSumLoss
-from slimfit.minimizer import LikelihoodOptimizer
+from slimfit.minimizers import LikelihoodOptimizer
 from slimfit.markov import generate_transition_matrix, extract_states
 from slimfit.parameter import Parameters, Parameter
 import numpy as np
 
 root_dir = Path(__file__).parent.parent
 
 
@@ -35,15 +27,19 @@
         clear_symbols()
         m = symbol_matrix("A", shape=(3, 3))
 
         assert m.shape == (3, 3)
         elem = m[0, 0]
         assert elem.name == "A_0_0"
 
-        m = symbol_matrix("A", shape=(1, 3), suffix=["a", "b", "c"],)
+        m = symbol_matrix(
+            "A",
+            shape=(1, 3),
+            suffix=["a", "b", "c"],
+        )
 
         elem = m[0, 0]
         assert elem.name == "A_a"
 
         elem = m[0, 1]
         assert elem.name == "A_b"
 
@@ -176,26 +172,48 @@
         assert num_c.name == "c"
 
     def test_lambda_numexpr(self):
         clear_symbols()
         np.random.seed(43)
 
         def func(x, a):
-            return x ** 2 + a
+            return x**2 + a
 
         data = {"x": np.arange(100)}
 
-        ld = LambdaNumExpr(func, [Symbol("a"), Symbol("x")],)
+        ld = LambdaNumExpr(
+            func,
+            [Symbol("a"), Symbol("x")],
+        )
 
         # todo shape testing
         # assert ld.shape == (100,)
 
         result = ld(a=2.0, **data)
         assert np.allclose(result, data["x"] ** 2 + 2.0)
 
+    def test_operations(self):
+        clear_symbols()
+        a, k, t, b, y = symbols("a k t b y")
+
+        guess = {"a": [[1, 2, 2.5]], "k": [[3.0, 2.5, 1.2]], "b": 3.0}
+        parameters = Parameters.from_symbols((a, k, b), guess)
+        parameters.guess["a"] * np.arange(10).reshape(-1, 1)
+
+        model = Model({y: Add(Sum(a * exp(-k * t), axis=1), b)})
+        tdata = np.arange(10).reshape(-1, 1)
+
+        ans = model(t=tdata, **parameters.guess)["y"]
+        ref = (
+            np.sum(parameters.guess["a"] * np.exp(-parameters.guess["k"] * tdata), axis=1)
+            + parameters.guess["b"]
+        )
+
+        assert np.allclose(ans, ref)
+
     def test_gmm(self):
         states = ["A", "B", "C"]
         mu = symbol_matrix("mu", suffix=states, shape=(1, 3))
         sigma = symbol_matrix("sigma", suffix=states, shape=(1, 3))
         gmm = GMM(Symbol("x"), mu, sigma)
         parameters = Parameters.from_symbols(gmm.symbols, "mu_A mu_B mu_C sigma_A sigma_B sigma_C")
         data = {"x": np.linspace(-0.2, 1.2, num=25).reshape(-1, 1)}
@@ -309,22 +327,19 @@
         model = Model({Symbol("y"): xt @ y0})
 
         rate_params = Parameters.from_symbols(get_symbols(m).values())
         y0_params = Parameters.from_symbols(get_symbols(y0).values())
         parameters = rate_params + y0_params
 
         num = 50
-        xdata = {"t": np.linspace(0, 11, num=num)}
-        num_model = model.to_numerical()
-        populations = num_model(**gt_values, **xdata)["y"]
-        ydata = {
-            "y": populations + np.random.normal(0, 0.05, size=num * 3).reshape(populations.shape)
-        }
+        xdata = np.linspace(0, 11, num=num)
+        populations = Eval(xt @ y0)(**gt_values, t=xdata)
+        ydata = populations + np.random.normal(0, 0.05, size=num * 3).reshape(populations.shape)
 
-        fit = Fit(model, parameters, data={**xdata, **ydata})
+        fit = Fit(model, parameters, data=dict(t=xdata, y=ydata), loss=SELoss(reduction="mean"))
         result = fit.execute()
 
         expected = {
             "k_A_B": 1.0926495267297978,
             "k_B_A": 0.02553115392319696,
             "k_B_C": 0.48848195581215753,
             "y0_A": 1.0144580699136068,
@@ -525,15 +540,17 @@
         vars = ["x1", "x2"]
         data = {}
         Ns = [1000, 1500]
         for st, var, N in zip(states, vars, Ns):
             data[var] = np.concatenate(
                 [
                     np.random.normal(
-                        loc=gt[f"mu_{s}"], scale=gt[f"sigma_{s}"], size=int(N * gt[f"c_{s}"]),
+                        loc=gt[f"mu_{s}"],
+                        scale=gt[f"sigma_{s}"],
+                        size=int(N * gt[f"c_{s}"]),
                     )
                     for s in st
                 ]
             ).reshape(-1, 1)
 
         # todo guess is not used
         guess = {
@@ -640,26 +657,28 @@
         parameters.set("k_B_C", lower_bound=1e-3, upper_bound=1e2)
 
         # To calculate the likelihood for a measurement we need to sum the individual probabilities for all states
         # Thus we need to define which axis this is in the model
         STATE_AXIS = 1
 
         fit = Fit(model, parameters, data, loss=LogSumLoss(sum_axis=STATE_AXIS))
-        result = fit.execute(minimizer=LikelihoodOptimizer, max_iter=200, verbose=True,)
+        result = fit.execute(
+            minimizer=LikelihoodOptimizer,
+            max_iter=200,
+            verbose=True,
+        )
 
         expected = {
             "k_A_B": 0.5415993464686054,
             "k_B_A": 0.08259132883479212,
             "k_B_C": 0.2527748185081457,
             "y0_A": 0.9696231022059791,
             "mu_A": 0.822262354106825,
             "mu_B": 0.12972476836918412,
             "mu_C": 0.5518311456516388,
             "sigma_A": 0.09320689716234987,
             "sigma_B": 0.12251906102401328,
             "sigma_C": 0.07922175330380453,
         }
 
-        print(result.parameters)
-
         for k in expected:
             assert result.parameters[k] == pytest.approx(expected[k], rel=0.1)
```

