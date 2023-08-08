# Comparing `tmp/poismf-0.4.0.post7.tar.gz` & `tmp/poismf-0.4.0.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poismf-0.4.0.post7.tar", last modified: Mon Jul  3 18:48:43 2023, max compression
+gzip compressed data, was "poismf-0.4.0.post8.tar", last modified: Tue Aug  8 19:45:25 2023, max compression
```

## Comparing `poismf-0.4.0.post7.tar` & `poismf-0.4.0.post8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/
--rw-r--r--   0 david     (1000) david     (1000)     1322 2022-02-23 22:22:19.000000 poismf-0.4.0.post7/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      656 2021-08-24 23:08:41.000000 poismf-0.4.0.post7/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      232 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/PKG-INFO
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/poismf/
--rw-r--r--   0 david     (1000) david     (1000)    51161 2023-07-03 18:46:03.000000 poismf-0.4.0.post7/poismf/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      120 2023-03-19 16:12:38.000000 poismf-0.4.0.post7/poismf/cfuns_double.pyx
--rw-r--r--   0 david     (1000) david     (1000)      118 2023-03-19 16:12:36.000000 poismf-0.4.0.post7/poismf/cfuns_float.pyx
--rw-r--r--   0 david     (1000) david     (1000)    13270 2022-02-23 21:18:16.000000 poismf-0.4.0.post7/poismf/poismf_c_wrapper.pxi
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/poismf.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      232 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      386 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       32 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        7 2023-07-03 18:48:43.000000 poismf-0.4.0.post7/poismf.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       95 2021-06-24 17:47:12.000000 poismf-0.4.0.post7/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       40 2023-07-03 18:41:24.000000 poismf-0.4.0.post7/requirements.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    11208 2023-07-03 18:41:07.000000 poismf-0.4.0.post7/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:48:43.306506 poismf-0.4.0.post7/src/
--rw-r--r--   0 david     (1000) david     (1000)    13888 2022-02-23 22:22:28.000000 poismf-0.4.0.post7/src/nonnegcg.c
--rw-r--r--   0 david     (1000) david     (1000)    23148 2022-02-23 22:22:34.000000 poismf-0.4.0.post7/src/poismf.c
--rw-r--r--   0 david     (1000) david     (1000)    10465 2022-02-23 22:22:40.000000 poismf-0.4.0.post7/src/poismf.h
--rw-r--r--   0 david     (1000) david     (1000)     9812 2022-02-23 22:22:48.000000 poismf-0.4.0.post7/src/pred.c
--rw-r--r--   0 david     (1000) david     (1000)    66204 2021-07-27 17:42:06.000000 poismf-0.4.0.post7/src/tnc.c
--rw-r--r--   0 david     (1000) david     (1000)     7485 2020-05-29 15:47:53.000000 poismf-0.4.0.post7/src/tnc.h
--rw-r--r--   0 david     (1000) david     (1000)     9976 2022-02-23 22:55:21.000000 poismf-0.4.0.post7/src/topN.c
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:45:25.235770 poismf-0.4.0.post8/
+-rw-r--r--   0 david     (1000) david     (1000)     1322 2022-02-23 22:22:19.000000 poismf-0.4.0.post8/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      656 2021-08-24 23:08:41.000000 poismf-0.4.0.post8/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      232 2023-08-08 19:45:25.235770 poismf-0.4.0.post8/PKG-INFO
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:45:25.231770 poismf-0.4.0.post8/poismf/
+-rw-r--r--   0 david     (1000) david     (1000)    51161 2023-07-03 18:46:03.000000 poismf-0.4.0.post8/poismf/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      120 2023-03-19 16:12:38.000000 poismf-0.4.0.post8/poismf/cfuns_double.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      118 2023-03-19 16:12:36.000000 poismf-0.4.0.post8/poismf/cfuns_float.pyx
+-rw-r--r--   0 david     (1000) david     (1000)    13504 2023-08-08 19:37:01.000000 poismf-0.4.0.post8/poismf/poismf_c_wrapper.pxi
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:45:25.231770 poismf-0.4.0.post8/poismf.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      232 2023-08-08 19:45:25.000000 poismf-0.4.0.post8/poismf.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      386 2023-08-08 19:45:25.000000 poismf-0.4.0.post8/poismf.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-08-08 19:45:25.000000 poismf-0.4.0.post8/poismf.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       32 2023-08-08 19:45:25.000000 poismf-0.4.0.post8/poismf.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        7 2023-08-08 19:45:25.000000 poismf-0.4.0.post8/poismf.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       91 2023-08-08 19:37:54.000000 poismf-0.4.0.post8/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       40 2023-07-03 18:41:24.000000 poismf-0.4.0.post8/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-08-08 19:45:25.235770 poismf-0.4.0.post8/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    10683 2023-08-08 19:37:30.000000 poismf-0.4.0.post8/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:45:25.235770 poismf-0.4.0.post8/src/
+-rw-r--r--   0 david     (1000) david     (1000)    13888 2022-02-23 22:22:28.000000 poismf-0.4.0.post8/src/nonnegcg.c
+-rw-r--r--   0 david     (1000) david     (1000)    23148 2022-02-23 22:22:34.000000 poismf-0.4.0.post8/src/poismf.c
+-rw-r--r--   0 david     (1000) david     (1000)    10465 2022-02-23 22:22:40.000000 poismf-0.4.0.post8/src/poismf.h
+-rw-r--r--   0 david     (1000) david     (1000)     9812 2022-02-23 22:22:48.000000 poismf-0.4.0.post8/src/pred.c
+-rw-r--r--   0 david     (1000) david     (1000)    66204 2021-07-27 17:42:06.000000 poismf-0.4.0.post8/src/tnc.c
+-rw-r--r--   0 david     (1000) david     (1000)     7485 2020-05-29 15:47:53.000000 poismf-0.4.0.post8/src/tnc.h
+-rw-r--r--   0 david     (1000) david     (1000)     9976 2022-02-23 22:55:21.000000 poismf-0.4.0.post8/src/topN.c
```

### Comparing `poismf-0.4.0.post7/LICENSE` & `poismf-0.4.0.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/MANIFEST.in` & `poismf-0.4.0.post8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/poismf/__init__.py` & `poismf-0.4.0.post8/poismf/__init__.py`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/poismf/poismf_c_wrapper.pxi` & `poismf-0.4.0.post8/poismf/poismf_c_wrapper.pxi`

 * *Files 8% similar despite different names*

```diff
@@ -5,55 +5,55 @@
 
 cdef extern from "../src/poismf.h":
     ctypedef size_t sparse_ix
     ctypedef enum Method:
         tncg = 1
         cg = 2
         pg = 3
-    bint get_has_openmp() nogil
+    bint get_has_openmp() noexcept nogil
     int run_poismf(
         real_t *A, real_t *Xr, sparse_ix *Xr_indptr, sparse_ix *Xr_indices,
         real_t *B, real_t *Xc, sparse_ix *Xc_indptr, sparse_ix *Xc_indices,
         const size_t dimA, const size_t dimB, const size_t k,
         const real_t l2_reg, const real_t l1_reg, const real_t w_mult, real_t step_size,
         const Method method, const bint limit_step, const size_t numiter, const size_t maxupd,
         const bint early_stop, const bint reuse_prev,
-        const bint handle_interrupt, const int nthreads) nogil
+        const bint handle_interrupt, const int nthreads) noexcept nogil
     int factors_single(
         real_t *out, size_t k,
         real_t *Amean, bint reuse_mean,
         real_t *X, sparse_ix X_ind[], size_t nnz,
         real_t *B, real_t *Bsum,
         int maxupd, real_t l2_reg, real_t l1_new, real_t l1_old,
         real_t w_mult
-    ) nogil
+    ) noexcept nogil
     void predict_multiple(
         real_t *out,
         real_t *A, real_t *B,
         sparse_ix *ixA, sparse_ix *ixB,
         size_t n, int k,
         int nthreads
-    ) nogil
+    ) noexcept nogil
     int factors_multiple(
         real_t *A, real_t *B,
         real_t *Bsum, real_t *Amean,
         real_t *Xr, sparse_ix *Xr_indptr, sparse_ix *Xr_indices,
         int k, size_t dimA,
         real_t l2_reg, real_t w_mult,
         real_t step_size, size_t niter, size_t maxupd,
         Method method, bint limit_step, bint reuse_mean,
         int nthreads
-    ) nogil
+    ) noexcept nogil
     int topN(
         real_t *a_vec, real_t *B, int k,
         sparse_ix *include_ix, size_t n_include,
         sparse_ix *exclude_ix, size_t n_exclude,
         sparse_ix *outp_ix, real_t *outp_score,
         size_t n_top, size_t n, int nthreads
-    ) nogil
+    ) noexcept nogil
 
 def _get_has_openmp():
     return get_has_openmp()
 
 def _run_poismf(
     np.ndarray[real_t, ndim=1] Xr,
     np.ndarray[size_t, ndim=1] Xr_indices,
@@ -250,25 +250,25 @@
 ###################
 #### Cblas Wrappers
 #### Do not move to a new file as otherwise it doesn't compile,
 #### due to generating duplicated file names between headers and C files
 from scipy.linalg.cython_blas cimport ddot, daxpy, dscal, dnrm2, dgemv
 from scipy.linalg.cython_blas cimport sdot, saxpy, sscal, snrm2, sgemv
 
-ctypedef double (*ddot_)(const int*, const double*, const int*, const double*, const int*) nogil
-ctypedef void (*daxpy_)(const int*, const double*, const double*, const int*, double*, const int*) nogil
-ctypedef void (*dscal_)(const int*, const double*, double*, const int*) nogil
-ctypedef double (*dnrm2_)(const int*, const double*, const int*) nogil
-ctypedef void (*dgemv_)(const char*, const int*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) nogil
-
-ctypedef float (*sdot_)(const int*, const float*, const int*, const float*, const int*) nogil
-ctypedef void (*saxpy_)(const int*, const float*, const float*, const int*, float*, const int*) nogil
-ctypedef void (*sscal_)(const int*, const float*, float*, const int*) nogil
-ctypedef float (*snrm2_)(const int*, const float*, const int*) nogil
-ctypedef void (*sgemv_)(const char*, const int*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) nogil
+ctypedef double (*ddot_)(const int*, const double*, const int*, const double*, const int*) noexcept nogil
+ctypedef void (*daxpy_)(const int*, const double*, const double*, const int*, double*, const int*) noexcept nogil
+ctypedef void (*dscal_)(const int*, const double*, double*, const int*) noexcept nogil
+ctypedef double (*dnrm2_)(const int*, const double*, const int*) noexcept nogil
+ctypedef void (*dgemv_)(const char*, const int*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) noexcept nogil
+
+ctypedef float (*sdot_)(const int*, const float*, const int*, const float*, const int*) noexcept nogil
+ctypedef void (*saxpy_)(const int*, const float*, const float*, const int*, float*, const int*) noexcept nogil
+ctypedef void (*sscal_)(const int*, const float*, float*, const int*) noexcept nogil
+ctypedef float (*snrm2_)(const int*, const float*, const int*) noexcept nogil
+ctypedef void (*sgemv_)(const char*, const int*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) noexcept nogil
 
 ctypedef enum CBLAS_ORDER:
     CblasRowMajor = 101
     CblasColMajor = 102
 
 ctypedef CBLAS_ORDER CBLAS_LAYOUT
 
@@ -286,29 +286,29 @@
     CblasNonUnit=131
     CblasUnit=132
 
 ctypedef enum CBLAS_SIDE:
     CblasLeft=141
     CblasRight=142
 
-cdef public double cblas_ddot(const int n, const double *x, const int incx, const double *y, const int incy) nogil:
+cdef public double cblas_ddot(const int n, const double *x, const int incx, const double *y, const int incy) noexcept nogil:
     return (<ddot_>ddot)(&n, x, &incx, y, &incy)
 
-cdef public void cblas_daxpy(const int n, const double alpha, const double *x, const int incx, double *y, const int incy) nogil:
+cdef public void cblas_daxpy(const int n, const double alpha, const double *x, const int incx, double *y, const int incy) noexcept nogil:
     (<daxpy_>daxpy)(&n, &alpha, x, &incx, y, &incy)
 
-cdef public void cblas_dscal(const int N, const double alpha, double *X, const int incX) nogil:
+cdef public void cblas_dscal(const int N, const double alpha, double *X, const int incX) noexcept nogil:
     (<dscal_>dscal)(&N, &alpha, X, &incX)
 
-cdef public double cblas_dnrm2(const int n, const double *x, const int incx) nogil:
+cdef public double cblas_dnrm2(const int n, const double *x, const int incx) noexcept nogil:
     return (<dnrm2_>dnrm2)(&n, x, &incx)
 
 ### Note: Cython refuses to compile a public cdef'd function with enum arguments
 cdef public void cblas_dgemv(const int order,  const int TransA,  const int m, const int n,
-     const double alpha, const double  *a, const int lda,  const double  *x, const int incx,  const double beta,  double  *y, const int incy) nogil:
+     const double alpha, const double  *a, const int lda,  const double  *x, const int incx,  const double beta,  double  *y, const int incy) noexcept nogil:
     cdef char trans
     if (order == CblasColMajor):
         if (TransA == CblasNoTrans):
             trans = 'N';
         elif (TransA == CblasTrans):
             trans = 'T'
         else:
@@ -323,29 +323,29 @@
         else:
             trans = 'N'
 
         (<dgemv_>dgemv)(&trans, &n, &m, &alpha, a, &lda, x, &incx, &beta, y, &incy)
 
 ##################
 
-cdef public float cblas_sdot(const int n, const float *x, const int incx, const float *y, const int incy) nogil:
+cdef public float cblas_sdot(const int n, const float *x, const int incx, const float *y, const int incy) noexcept nogil:
     return (<sdot_>sdot)(&n, x, &incx, y, &incy)
 
-cdef public void cblas_saxpy(const int n, const float alpha, const float *x, const int incx, float *y, const int incy) nogil:
+cdef public void cblas_saxpy(const int n, const float alpha, const float *x, const int incx, float *y, const int incy) noexcept nogil:
     (<saxpy_>saxpy)(&n, &alpha, x, &incx, y, &incy)
 
-cdef public void cblas_sscal(const int N, const float alpha, float *X, const int incX) nogil:
+cdef public void cblas_sscal(const int N, const float alpha, float *X, const int incX) noexcept nogil:
     (<sscal_>sscal)(&N, &alpha, X, &incX)
 
-cdef public float cblas_snrm2(const int n, const float *x, const int incx) nogil:
+cdef public float cblas_snrm2(const int n, const float *x, const int incx) noexcept nogil:
     return (<snrm2_>snrm2)(&n, x, &incx)
 
 ### Note: Cython refuses to compile a public cdef'd function with enum arguments
 cdef public void cblas_sgemv(const int order,  const int TransA,  const int m, const int n,
-     const float alpha, const float  *a, const int lda,  const float  *x, const int incx,  const float beta,  float  *y, const int incy) nogil:
+     const float alpha, const float  *a, const int lda,  const float  *x, const int incx,  const float beta,  float  *y, const int incy) noexcept nogil:
     cdef char trans
     if (order == CblasColMajor):
         if (TransA == CblasNoTrans):
             trans = 'N';
         elif (TransA == CblasTrans):
             trans = 'T'
         else:
```

### Comparing `poismf-0.4.0.post7/setup.py` & `poismf-0.4.0.post8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,62 +208,51 @@
         try:
             os.remove(fname)
         except Exception:
             pass
         return is_supported
 
 
-from_rtd = os.environ.get('READTHEDOCS') == 'True'
-if not from_rtd:
-    setup(
-        name  = "poismf",
-        packages = ["poismf"],
-        author = 'David Cortes',
-        url = 'https://github.com/david-cortes/poismf',
-        version = '0.4.0-7',
-        install_requires = ['numpy', 'pandas>=0.24', 'cython', 'scipy'],
-        description = 'Fast and memory-efficient Poisson factorization for sparse count matrices',
-        cmdclass = {'build_ext': build_ext_subclass},
-        ext_modules = [
-            Extension("poismf.c_funs_double",
-                sources=["poismf/cfuns_double.pyx",
-                         "src/poismf.c", "src/topN.c", "src/pred.c",
-                         "src/nonnegcg.c", "src/tnc.c"],
-                include_dirs=[numpy.get_include(), "src/"],
-                define_macros = [
-                    ("_FOR_PYTHON", None),
-                    ("NDEBUG", None),
-                ]),
-            Extension("poismf.c_funs_float",
-                sources=["poismf/cfuns_float.pyx",
-                         "src/poismf.c", "src/topN.c", "src/pred.c",
-                         "src/nonnegcg.c", "src/tnc.c"],
-                include_dirs=[numpy.get_include(), "src/"],
-                define_macros = [
-                    ("_FOR_PYTHON", None),
-                    ("NDEBUG", None),
-                    ("USE_FLOAT", None)
-                ])
-            ]
-    )
+setup(
+    name  = "poismf",
+    packages = ["poismf"],
+    author = 'David Cortes',
+    url = 'https://github.com/david-cortes/poismf',
+    version = '0.4.0-8',
+    install_requires = ['numpy', 'pandas>=0.24', 'cython', 'scipy'],
+    description = 'Fast and memory-efficient Poisson factorization for sparse count matrices',
+    cmdclass = {'build_ext': build_ext_subclass},
+    ext_modules = [
+        Extension("poismf.c_funs_double",
+            sources=["poismf/cfuns_double.pyx",
+                     "src/poismf.c", "src/topN.c", "src/pred.c",
+                     "src/nonnegcg.c", "src/tnc.c"],
+            include_dirs=[numpy.get_include(), "src/"],
+            define_macros = [
+                ("_FOR_PYTHON", None),
+                ("NDEBUG", None),
+                ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"),
+            ]),
+        Extension("poismf.c_funs_float",
+            sources=["poismf/cfuns_float.pyx",
+                     "src/poismf.c", "src/topN.c", "src/pred.c",
+                     "src/nonnegcg.c", "src/tnc.c"],
+            include_dirs=[numpy.get_include(), "src/"],
+            define_macros = [
+                ("_FOR_PYTHON", None),
+                ("NDEBUG", None),
+                ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"),
+                ("USE_FLOAT", None),
+            ])
+        ]
+)
 
-    if not found_omp:
-        omp_msg  = "\n\n\nCould not detect OpenMP. Package will be built without multi-threading capabilities. "
-        omp_msg += " To enable multi-threading, first install OpenMP"
-        if (sys.platform[:3] == "dar"):
-            omp_msg += " - for macOS: 'brew install libomp'\n"
-        else:
-            omp_msg += " modules for your compiler. "
-        
-        omp_msg += "Then reinstall this package from scratch: 'pip install --upgrade --no-deps --force-reinstall poismf'.\n"
-        warnings.warn(omp_msg)
-else:
-    setup(
-        name  = "poismf",
-        packages = ["poismf"],
-        author = 'David Cortes',
-        author_email = 'david.cortes.rivera@gmail.com',
-        url = 'https://github.com/david-cortes/poismf',
-        version = '0.4.0-6',
-        install_requires = ['numpy', 'scipy', 'pandas>=0.24', 'cython'],
-        description = 'Fast and memory-efficient Poisson factorization for sparse count matrices',
-    )
+if not found_omp:
+    omp_msg  = "\n\n\nCould not detect OpenMP. Package will be built without multi-threading capabilities. "
+    omp_msg += " To enable multi-threading, first install OpenMP"
+    if (sys.platform[:3] == "dar"):
+        omp_msg += " - for macOS: 'brew install libomp'\n"
+    else:
+        omp_msg += " modules for your compiler. "
+    
+    omp_msg += "Then reinstall this package from scratch: 'pip install --upgrade --no-deps --force-reinstall poismf'.\n"
+    warnings.warn(omp_msg)
```

### Comparing `poismf-0.4.0.post7/src/nonnegcg.c` & `poismf-0.4.0.post8/src/nonnegcg.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/src/poismf.c` & `poismf-0.4.0.post8/src/poismf.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/src/poismf.h` & `poismf-0.4.0.post8/src/poismf.h`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/src/pred.c` & `poismf-0.4.0.post8/src/pred.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/src/tnc.c` & `poismf-0.4.0.post8/src/tnc.c`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/src/tnc.h` & `poismf-0.4.0.post8/src/tnc.h`

 * *Files identical despite different names*

### Comparing `poismf-0.4.0.post7/src/topN.c` & `poismf-0.4.0.post8/src/topN.c`

 * *Files identical despite different names*

