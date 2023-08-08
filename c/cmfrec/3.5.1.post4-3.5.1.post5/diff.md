# Comparing `tmp/cmfrec-3.5.1.post4.tar.gz` & `tmp/cmfrec-3.5.1.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmfrec-3.5.1.post4.tar", last modified: Sat Mar 25 17:01:26 2023, max compression
+gzip compressed data, was "cmfrec-3.5.1.post5.tar", last modified: Tue Aug  8 19:58:01 2023, max compression
```

## Comparing `cmfrec-3.5.1.post4.tar` & `cmfrec-3.5.1.post5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 17:01:26.132945 cmfrec-3.5.1.post4/
--rw-r--r--   0 david     (1000) david     (1000)     1096 2022-02-09 23:25:39.000000 cmfrec-3.5.1.post4/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      400 2021-08-24 23:05:22.000000 cmfrec-3.5.1.post4/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      276 2023-03-25 17:01:26.132945 cmfrec-3.5.1.post4/PKG-INFO
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 17:01:26.132945 cmfrec-3.5.1.post4/cmfrec/
--rw-r--r--   0 david     (1000) david     (1000)   397031 2023-03-20 17:47:32.000000 cmfrec-3.5.1.post4/cmfrec/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      121 2023-03-19 15:54:26.000000 cmfrec-3.5.1.post4/cmfrec/cfuns_double.pyx
--rw-r--r--   0 david     (1000) david     (1000)      148 2023-03-19 15:54:21.000000 cmfrec-3.5.1.post4/cmfrec/cfuns_double_plusblas.pyx
--rw-r--r--   0 david     (1000) david     (1000)      119 2023-03-19 15:54:37.000000 cmfrec-3.5.1.post4/cmfrec/cfuns_float.pyx
--rw-r--r--   0 david     (1000) david     (1000)      146 2023-03-19 15:54:34.000000 cmfrec-3.5.1.post4/cmfrec/cfuns_float_plusblas.pyx
--rw-r--r--   0 david     (1000) david     (1000)    17487 2022-12-28 19:01:49.000000 cmfrec-3.5.1.post4/cmfrec/cython_cblas.pxi
--rw-r--r--   0 david     (1000) david     (1000)   129895 2022-05-30 20:02:07.000000 cmfrec-3.5.1.post4/cmfrec/wrapper_untyped.pxi
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 17:01:26.132945 cmfrec-3.5.1.post4/cmfrec.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      276 2023-03-25 17:01:26.000000 cmfrec-3.5.1.post4/cmfrec.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      537 2023-03-25 17:01:26.000000 cmfrec-3.5.1.post4/cmfrec.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-03-25 17:01:26.000000 cmfrec-3.5.1.post4/cmfrec.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       49 2023-03-25 17:01:26.000000 cmfrec-3.5.1.post4/cmfrec.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        7 2023-03-25 17:01:26.000000 cmfrec-3.5.1.post4/cmfrec.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)      107 2021-06-25 17:44:40.000000 cmfrec-3.5.1.post4/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       79 2023-03-25 17:01:26.136945 cmfrec-3.5.1.post4/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    16764 2023-03-25 17:00:57.000000 cmfrec-3.5.1.post4/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 17:01:26.132945 cmfrec-3.5.1.post4/src/
--rw-r--r--   0 david     (1000) david     (1000)     3817 2022-01-11 13:28:13.000000 cmfrec-3.5.1.post4/src/arithmetic_ansi.h
--rw-r--r--   0 david     (1000) david     (1000)    11498 2022-02-09 23:25:49.000000 cmfrec-3.5.1.post4/src/cblas_wrappers.c
--rw-r--r--   0 david     (1000) david     (1000)   106348 2022-07-09 11:08:02.000000 cmfrec-3.5.1.post4/src/cmfrec.h
--rw-r--r--   0 david     (1000) david     (1000)   427130 2022-11-22 20:24:17.000000 cmfrec-3.5.1.post4/src/collective.c
--rw-r--r--   0 david     (1000) david     (1000)   214819 2022-11-22 17:24:17.000000 cmfrec-3.5.1.post4/src/common.c
--rw-r--r--   0 david     (1000) david     (1000)    56169 2023-03-17 20:06:45.000000 cmfrec-3.5.1.post4/src/helpers.c
--rw-r--r--   0 david     (1000) david     (1000)    45747 2022-01-05 15:17:19.000000 cmfrec-3.5.1.post4/src/lbfgs.c
--rw-r--r--   0 david     (1000) david     (1000)    32915 2020-10-27 15:53:49.000000 cmfrec-3.5.1.post4/src/lbfgs.h
--rw-r--r--   0 david     (1000) david     (1000)   124562 2023-03-17 20:06:27.000000 cmfrec-3.5.1.post4/src/offsets.c
--rw-r--r--   0 david     (1000) david     (1000)    44043 2022-02-09 21:37:36.000000 cmfrec-3.5.1.post4/src/ziggurat.h
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:58:01.603568 cmfrec-3.5.1.post5/
+-rw-r--r--   0 david     (1000) david     (1000)     1096 2022-02-09 23:25:39.000000 cmfrec-3.5.1.post5/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      400 2021-08-24 23:05:22.000000 cmfrec-3.5.1.post5/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      276 2023-08-08 19:58:01.603568 cmfrec-3.5.1.post5/PKG-INFO
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:58:01.603568 cmfrec-3.5.1.post5/cmfrec/
+-rw-r--r--   0 david     (1000) david     (1000)   397031 2023-03-20 17:47:32.000000 cmfrec-3.5.1.post5/cmfrec/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      121 2023-03-19 15:54:26.000000 cmfrec-3.5.1.post5/cmfrec/cfuns_double.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      148 2023-03-19 15:54:21.000000 cmfrec-3.5.1.post5/cmfrec/cfuns_double_plusblas.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      119 2023-03-19 15:54:37.000000 cmfrec-3.5.1.post5/cmfrec/cfuns_float.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      146 2023-03-19 15:54:34.000000 cmfrec-3.5.1.post5/cmfrec/cfuns_float_plusblas.pyx
+-rw-r--r--   0 david     (1000) david     (1000)    18063 2023-08-08 19:21:52.000000 cmfrec-3.5.1.post5/cmfrec/cython_cblas.pxi
+-rw-r--r--   0 david     (1000) david     (1000)   130183 2023-08-08 19:24:12.000000 cmfrec-3.5.1.post5/cmfrec/wrapper_untyped.pxi
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:58:01.603568 cmfrec-3.5.1.post5/cmfrec.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      276 2023-08-08 19:58:01.000000 cmfrec-3.5.1.post5/cmfrec.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      537 2023-08-08 19:58:01.000000 cmfrec-3.5.1.post5/cmfrec.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-08-08 19:58:01.000000 cmfrec-3.5.1.post5/cmfrec.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       49 2023-08-08 19:58:01.000000 cmfrec-3.5.1.post5/cmfrec.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        7 2023-08-08 19:58:01.000000 cmfrec-3.5.1.post5/cmfrec.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)      103 2023-08-08 19:25:01.000000 cmfrec-3.5.1.post5/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       79 2023-08-08 19:58:01.603568 cmfrec-3.5.1.post5/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    16922 2023-08-08 19:27:44.000000 cmfrec-3.5.1.post5/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 19:58:01.603568 cmfrec-3.5.1.post5/src/
+-rw-r--r--   0 david     (1000) david     (1000)     3817 2022-01-11 13:28:13.000000 cmfrec-3.5.1.post5/src/arithmetic_ansi.h
+-rw-r--r--   0 david     (1000) david     (1000)    11498 2022-02-09 23:25:49.000000 cmfrec-3.5.1.post5/src/cblas_wrappers.c
+-rw-r--r--   0 david     (1000) david     (1000)   106348 2022-07-09 11:08:02.000000 cmfrec-3.5.1.post5/src/cmfrec.h
+-rw-r--r--   0 david     (1000) david     (1000)   427130 2022-11-22 20:24:17.000000 cmfrec-3.5.1.post5/src/collective.c
+-rw-r--r--   0 david     (1000) david     (1000)   214819 2023-04-18 17:52:03.000000 cmfrec-3.5.1.post5/src/common.c
+-rw-r--r--   0 david     (1000) david     (1000)    56169 2023-06-26 18:44:08.000000 cmfrec-3.5.1.post5/src/helpers.c
+-rw-r--r--   0 david     (1000) david     (1000)    45747 2022-01-05 15:17:19.000000 cmfrec-3.5.1.post5/src/lbfgs.c
+-rw-r--r--   0 david     (1000) david     (1000)    32915 2020-10-27 15:53:49.000000 cmfrec-3.5.1.post5/src/lbfgs.h
+-rw-r--r--   0 david     (1000) david     (1000)   124562 2023-03-17 20:06:27.000000 cmfrec-3.5.1.post5/src/offsets.c
+-rw-r--r--   0 david     (1000) david     (1000)    44043 2022-02-09 21:37:36.000000 cmfrec-3.5.1.post5/src/ziggurat.h
```

### Comparing `cmfrec-3.5.1.post4/LICENSE` & `cmfrec-3.5.1.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/cmfrec/__init__.py` & `cmfrec-3.5.1.post5/cmfrec/__init__.py`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/cmfrec/cython_cblas.pxi` & `cmfrec-3.5.1.post5/cmfrec/cython_cblas.pxi`

 * *Files 7% similar despite different names*

```diff
@@ -3,58 +3,58 @@
     sdot, scopy, saxpy, sscal, ssyr, ssyrk, snrm2, sgemm, sgemv, ssymv, sger
 )
 from scipy.linalg.cython_lapack cimport (
     dlacpy, dposv, dpotrf, dpotrs, dgelsd,
     slacpy, sposv, spotrf, spotrs, sgelsd
 )
 
-ctypedef double (*ddot_)(const int*, const double*, const int*, const double*, const int*) nogil
-ctypedef void (*dcopy_)(const int*, const double*, const int*, const double*, const int*) nogil
-ctypedef void (*daxpy_)(const int*, const double*, const double*, const int*, double*, const int*) nogil
-ctypedef void (*dscal_)(const int*, const double*, double*, const int*) nogil
-ctypedef void (*dsyr_)(const char*, const int*, const double*, const double*, const int*, double*, const int*) nogil
-ctypedef void (*dsyrk_)(const char*, const char*, const int*, const int*, const double*, const double*, const int*, const double*, double*, const int*) nogil
-ctypedef double (*dnrm2_)(const int*, const double*, const int*) nogil
-ctypedef void (*dgemm_)(const char*, const char*, const int*, const int*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) nogil
-ctypedef void (*dgemv_)(const char*, const int*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) nogil
-ctypedef void (*dsymv_)(const char*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) nogil
-ctypedef void (*dger_)(const int*, const int*, const double*, const double*, const int*, const double*, const int*, double*, const int*) nogil
-
-ctypedef void (*dposv__)(const char*, const int*, const int*, double*, const int*, double*, const int*, int*) nogil
-ctypedef void (*dlacpy__)(const char*, const int*, const int*, const double*, const int*, double*, const int*) nogil
-ctypedef void (*dpotrf__)(const char*, const int*, double*, const int*, int*) nogil
-ctypedef void (*dpotrs__)(const char*, const int*, const int*, const double*, const int*, double*, const int*, int*) nogil
+ctypedef double (*ddot_)(const int*, const double*, const int*, const double*, const int*) noexcept nogil
+ctypedef void (*dcopy_)(const int*, const double*, const int*, const double*, const int*) noexcept nogil
+ctypedef void (*daxpy_)(const int*, const double*, const double*, const int*, double*, const int*) noexcept nogil
+ctypedef void (*dscal_)(const int*, const double*, double*, const int*) noexcept nogil
+ctypedef void (*dsyr_)(const char*, const int*, const double*, const double*, const int*, double*, const int*) noexcept nogil
+ctypedef void (*dsyrk_)(const char*, const char*, const int*, const int*, const double*, const double*, const int*, const double*, double*, const int*) noexcept nogil
+ctypedef double (*dnrm2_)(const int*, const double*, const int*) noexcept nogil
+ctypedef void (*dgemm_)(const char*, const char*, const int*, const int*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) noexcept nogil
+ctypedef void (*dgemv_)(const char*, const int*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) noexcept nogil
+ctypedef void (*dsymv_)(const char*, const int*, const double*, const double*, const int*, const double*, const int*, const double*, double*, const int*) noexcept nogil
+ctypedef void (*dger_)(const int*, const int*, const double*, const double*, const int*, const double*, const int*, double*, const int*) noexcept nogil
+
+ctypedef void (*dposv__)(const char*, const int*, const int*, double*, const int*, double*, const int*, int*) noexcept nogil
+ctypedef void (*dlacpy__)(const char*, const int*, const int*, const double*, const int*, double*, const int*) noexcept nogil
+ctypedef void (*dpotrf__)(const char*, const int*, double*, const int*, int*) noexcept nogil
+ctypedef void (*dpotrs__)(const char*, const int*, const int*, const double*, const int*, double*, const int*, int*) noexcept nogil
 ctypedef void (*dgelsd__)(const int*, const int*, const int*,
              double*, const int*,
              double*, const int*,
              double*, const double*, int*, double*,
-             const int*, int*, int*) nogil
+             const int*, int*, int*) noexcept nogil
 
 
-ctypedef float (*sdot_)(const int*, const float*, const int*, const float*, const int*) nogil
-ctypedef void (*scopy_)(const int*, const float*, const int*, const float*, const int*) nogil
-ctypedef void (*saxpy_)(const int*, const float*, const float*, const int*, float*, const int*) nogil
-ctypedef void (*sscal_)(const int*, const float*, float*, const int*) nogil
-ctypedef void (*ssyr_)(const char*, const int*, const float*, const float*, const int*, float*, const int*) nogil
-ctypedef void (*ssyrk_)(const char*, const char*, const int*, const int*, const float*, const float*, const int*, const float*, float*, const int*) nogil
-ctypedef float (*snrm2_)(const int*, const float*, const int*) nogil
-ctypedef void (*sgemm_)(const char*, const char*, const int*, const int*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) nogil
-ctypedef void (*sgemv_)(const char*, const int*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) nogil
-ctypedef void (*ssymv_)(const char*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) nogil
-ctypedef float (*sger_)(const int*, const int*, const float*, const float*, const int*, const float*, const int*, float*, const int*) nogil
-
-ctypedef void (*sposv__)(const char*, const int*, const int*, float*, const int*, float*, const int*, int*) nogil
-ctypedef void (*slacpy__)(const char*, const int*, const int*, const float*, const int*, float*, const int*) nogil
-ctypedef void (*spotrf__)(const char*, const int*, float*, const int*, int*) nogil
-ctypedef void (*spotrs__)(const char*, const int*, const int*, const float*, const int*, float*, const int*, int*) nogil
+ctypedef float (*sdot_)(const int*, const float*, const int*, const float*, const int*) noexcept nogil
+ctypedef void (*scopy_)(const int*, const float*, const int*, const float*, const int*) noexcept nogil
+ctypedef void (*saxpy_)(const int*, const float*, const float*, const int*, float*, const int*) noexcept nogil
+ctypedef void (*sscal_)(const int*, const float*, float*, const int*) noexcept nogil
+ctypedef void (*ssyr_)(const char*, const int*, const float*, const float*, const int*, float*, const int*) noexcept nogil
+ctypedef void (*ssyrk_)(const char*, const char*, const int*, const int*, const float*, const float*, const int*, const float*, float*, const int*) noexcept nogil
+ctypedef float (*snrm2_)(const int*, const float*, const int*) noexcept nogil
+ctypedef void (*sgemm_)(const char*, const char*, const int*, const int*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) noexcept nogil
+ctypedef void (*sgemv_)(const char*, const int*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) noexcept nogil
+ctypedef void (*ssymv_)(const char*, const int*, const float*, const float*, const int*, const float*, const int*, const float*, float*, const int*) noexcept nogil
+ctypedef float (*sger_)(const int*, const int*, const float*, const float*, const int*, const float*, const int*, float*, const int*) noexcept nogil
+
+ctypedef void (*sposv__)(const char*, const int*, const int*, float*, const int*, float*, const int*, int*) noexcept nogil
+ctypedef void (*slacpy__)(const char*, const int*, const int*, const float*, const int*, float*, const int*) noexcept nogil
+ctypedef void (*spotrf__)(const char*, const int*, float*, const int*, int*) noexcept nogil
+ctypedef void (*spotrs__)(const char*, const int*, const int*, const float*, const int*, float*, const int*, int*) noexcept nogil
 ctypedef void (*sgelsd__)(const int*, const int*, const int*,
              float*, const int*,
              float*, const int*,
              float*, const float*, int*, float*,
-             const int*, int*, int*) nogil
+             const int*, int*, int*) noexcept nogil
 
 ctypedef enum CBLAS_ORDER:
     CblasRowMajor = 101
     CblasColMajor = 102
 
 ctypedef CBLAS_ORDER CBLAS_LAYOUT
 
@@ -72,27 +72,27 @@
     CblasNonUnit=131
     CblasUnit=132
 
 ctypedef enum CBLAS_SIDE:
     CblasLeft=141
     CblasRight=142
 
-cdef public double cblas_ddot(const int n, const double  *x, const int incx, const double  *y, const int incy) nogil:
+cdef public double cblas_ddot(const int n, const double  *x, const int incx, const double  *y, const int incy) noexcept nogil:
     return (<ddot_>ddot)(&n, x, &incx, y, &incy)
 
-cdef public void cblas_dcopy(const int n, const double *x, const int incx, double *y, const int incy) nogil:
+cdef public void cblas_dcopy(const int n, const double *x, const int incx, double *y, const int incy) noexcept nogil:
     (<dcopy_>dcopy)(&n, x, &incx, y, &incy)
 
-cdef public void cblas_daxpy(const int n, const double alpha, const double *x, const int incx, double *y, const int incy) nogil:
+cdef public void cblas_daxpy(const int n, const double alpha, const double *x, const int incx, double *y, const int incy) noexcept nogil:
     (<daxpy_>daxpy)(&n, &alpha, x, &incx, y, &incy)
 
-cdef public void cblas_dscal(const int N, const double alpha, double *X, const int incX) nogil:
+cdef public void cblas_dscal(const int N, const double alpha, double *X, const int incX) noexcept nogil:
     (<dscal_>dscal)(&N, &alpha, X, &incX)
 
-cdef public void cblas_dsyr(const int order, const int Uplo, const int N, const double alpha, const double *X, const int incX, double *A, const int lda) nogil:
+cdef public void cblas_dsyr(const int order, const int Uplo, const int N, const double alpha, const double *X, const int incX, double *A, const int lda) noexcept nogil:
     cdef char uplo = 0#'\0'
     if (order == CblasColMajor):
         if (Uplo == CblasLower):
             uplo = 76#'L'
         else:
             uplo = 85#'U'
 
@@ -100,15 +100,15 @@
         if (Uplo == CblasLower):
             uplo = 85#'U'
         else:
             uplo = 76#'L'
     (<dsyr_>dsyr)(&uplo, &N, &alpha, X, &incX, A, &lda)
 
 cdef public void cblas_dsyrk(const int Order, const int Uplo, const int Trans,
-         const int N, const int K, const double alpha, const double *A, const int lda, const double beta, double *C, const int ldc) nogil:
+         const int N, const int K, const double alpha, const double *A, const int lda, const double beta, double *C, const int ldc) noexcept nogil:
     cdef char uplo = 0#'\0'
     cdef char trans = 0#'\0'
     if (Order == CblasColMajor):
         if (Uplo == CblasUpper):
             uplo = 85#'U'
         else:
             uplo = 76#'L'
@@ -131,19 +131,19 @@
         elif (Trans == CblasConjTrans):
             trans = 78#'N'
         else:
             trans = 84#'T'
 
     (<dsyrk_>dsyrk)(&uplo, &trans, &N, &K, &alpha, A, &lda, &beta, C, &ldc)
 
-cdef public double cblas_dnrm2 (const int N, const double  *X, const int incX) nogil:
+cdef public double cblas_dnrm2 (const int N, const double  *X, const int incX) noexcept nogil:
     return (<dnrm2_>dnrm2)(&N, X, &incX)
 
 cdef public void cblas_dgemm(const int Order, const int TransA, const int TransB, const int M, const int N, const int K,
-         const double alpha, const double *A, const int lda, const double *B, const int ldb, const double beta, double *C, const int ldc) nogil:
+         const double alpha, const double *A, const int lda, const double *B, const int ldb, const double beta, double *C, const int ldc) noexcept nogil:
     cdef char transA = 0#'\0'
     cdef char transB = 0#'\0'
     if (Order == CblasColMajor):
         if (TransA == CblasTrans):
             transA = 84#'T'
         elif (TransA == CblasConjTrans):
             transA = 67#'C'
@@ -173,15 +173,15 @@
             transA = 67#'C'
         else:
             transA = 78#'N'
 
         (<dgemm_>dgemm)(&transA, &transB, &N, &M, &K, &alpha, B, &ldb, A, &lda, &beta, C, &ldc)
 
 cdef public void cblas_dgemv(const int order,  const int TransA,  const int m, const int n,
-         const double alpha, const double  *a, const int lda,  const double  *x, const int incx,  const double beta,  double  *y, const int incy) nogil:
+         const double alpha, const double  *a, const int lda,  const double  *x, const int incx,  const double beta,  double  *y, const int incy) noexcept nogil:
     cdef char trans = 0#'\0'
     if (order == CblasColMajor):
         if (TransA == CblasNoTrans):
             trans = 78#'N'
         elif (TransA == CblasTrans):
             trans = 84#'T'
         else:
@@ -196,15 +196,15 @@
             trans = 78#'N'
         else:
             trans = 78#'N'
 
         (<dgemv_>dgemv)(&trans, &n, &m, &alpha, a, &lda, x, &incx, &beta, y, &incy);
 
 cdef public void cblas_dsymv(const int order, const int Uplo, const int N, const double alpha, const double *A,
-                 const int lda, const double *X, const int incX, const double beta, double *Y, const int incY) nogil:
+                 const int lda, const double *X, const int incX, const double beta, double *Y, const int incY) noexcept nogil:
     cdef char uplo = 0#'\0';
     if (order == CblasColMajor):
         if (Uplo == CblasUpper):
             uplo = 85#'U'
         else:
             uplo = 76#'L'
 
@@ -213,55 +213,55 @@
             uplo = 76#'L'
         else:
             uplo = 85#'U'
 
     (<dsymv_>dsymv)(&uplo, &N, &alpha, A, &lda, X, &incX, &beta, Y, &incY)
 
 cdef public void cblas_dger(const int order, const int m, const int n, const double alpha,
-                const double *x, const int incx, const double *y, const int incy, double *a, const int lda) nogil:
+                const double *x, const int incx, const double *y, const int incy, double *a, const int lda) noexcept nogil:
     if (order == CblasColMajor):
         (<dger_>dger)(&m, &n, &alpha, x, &incx, y, &incy, a, &lda);
 
     else:
         (<dger_>dger)(&n, &m, &alpha, y, &incy, x, &incx, a, &lda);
 
-cdef public void dposv_(const char* uplo, const int* m, const int* n, double* x, const int* ldx, double* y, const int* ldy, int* info) nogil:
+cdef public void dposv_(const char* uplo, const int* m, const int* n, double* x, const int* ldx, double* y, const int* ldy, int* info) noexcept nogil:
     (<dposv__>dposv)(uplo, m, n, x, ldx, y, ldy, info)
 
-cdef public void dlacpy_(const char* uplo, const int* m, const int* n, const double* x, const int* ldx, double* y, const int* ldy) nogil:
+cdef public void dlacpy_(const char* uplo, const int* m, const int* n, const double* x, const int* ldx, double* y, const int* ldy) noexcept nogil:
     (<dlacpy__>dlacpy)(uplo, m, n, x, ldx, y, ldy)
 
-cdef public void dpotrf_(const char* a1, const int* a2, double* a3, const int* a4, int* a5) nogil:
+cdef public void dpotrf_(const char* a1, const int* a2, double* a3, const int* a4, int* a5) noexcept nogil:
     (<dpotrf__>dpotrf)(a1, a2, a3, a4, a5)
 
-cdef public void dpotrs_(const char* a1, const int* a2, const int* a3, const double* a4, const int* a5, double* a6, const int* a7, int* a8) nogil:
+cdef public void dpotrs_(const char* a1, const int* a2, const int* a3, const double* a4, const int* a5, double* a6, const int* a7, int* a8) noexcept nogil:
     (<dpotrs__>dpotrs)(a1, a2, a3, a4, a5, a6, a7, a8)
 
 cdef public void dgelsd_(const int* a1, const int* a2, const int* a3,
              double* a4, const int* a5,
              double* a6, const int* a7,
              double* a8, const double* a9, int* a10, double* a11,
-             const int* a12, int* a13, int* a14) nogil:
+             const int* a12, int* a13, int* a14) noexcept nogil:
     (<dgelsd__>dgelsd)(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14)
 
 ########################
 
-cdef public float cblas_sdot(const int n, const float  *x, const int incx, const float  *y, const int incy) nogil:
+cdef public float cblas_sdot(const int n, const float  *x, const int incx, const float  *y, const int incy) noexcept nogil:
     return (<sdot_>sdot)(&n, x, &incx, y, &incy)
 
-cdef public void cblas_scopy(const int n, const float *x, const int incx, float *y, const int incy) nogil:
+cdef public void cblas_scopy(const int n, const float *x, const int incx, float *y, const int incy) noexcept nogil:
     (<scopy_>scopy)(&n, x, &incx, y, &incy)
 
-cdef public void cblas_saxpy(const int n, const float alpha, const float *x, const int incx, float *y, const int incy) nogil:
+cdef public void cblas_saxpy(const int n, const float alpha, const float *x, const int incx, float *y, const int incy) noexcept nogil:
     (<saxpy_>saxpy)(&n, &alpha, x, &incx, y, &incy)
 
-cdef public void cblas_sscal(const int N, const float alpha, float *X, const int incX) nogil:
+cdef public void cblas_sscal(const int N, const float alpha, float *X, const int incX) noexcept nogil:
     (<sscal_>sscal)(&N, &alpha, X, &incX)
 
-cdef public void cblas_ssyr(const int order, const int Uplo, const int N, const float alpha, const float *X, const int incX, float *A, const int lda) nogil:
+cdef public void cblas_ssyr(const int order, const int Uplo, const int N, const float alpha, const float *X, const int incX, float *A, const int lda) noexcept nogil:
     cdef char uplo = 0#'\0'
     if (order == CblasColMajor):
         if (Uplo == CblasLower):
             uplo = 76#'L'
         else:
             uplo = 85#'U'
 
@@ -269,15 +269,15 @@
         if (Uplo == CblasLower):
             uplo = 85#'U'
         else:
             uplo = 76#'L'
     (<ssyr_>ssyr)(&uplo, &N, &alpha, X, &incX, A, &lda)
 
 cdef public void cblas_ssyrk(const int Order, const int Uplo, const int Trans,
-         const int N, const int K, const float alpha, const float *A, const int lda, const float beta, float *C, const int ldc) nogil:
+         const int N, const int K, const float alpha, const float *A, const int lda, const float beta, float *C, const int ldc) noexcept nogil:
     cdef char uplo = 0#'\0'
     cdef char trans = 0#'\0'
     if (Order == CblasColMajor):
         if (Uplo == CblasUpper):
             uplo = 85#'U'
         else:
             uplo = 76#'L'
@@ -300,19 +300,19 @@
         elif (Trans == CblasConjTrans):
             trans = 78#'N'
         else:
             trans = 84#'T'
 
     (<ssyrk_>ssyrk)(&uplo, &trans, &N, &K, &alpha, A, &lda, &beta, C, &ldc)
 
-cdef public float cblas_snrm2 (const int N, const float  *X, const int incX) nogil:
+cdef public float cblas_snrm2 (const int N, const float  *X, const int incX) noexcept nogil:
     return (<snrm2_>snrm2)(&N, X, &incX)
 
 cdef public void cblas_sgemm(const int Order, const int TransA, const int TransB, const int M, const int N, const int K,
-         const float alpha, const float *A, const int lda, const float *B, const int ldb, const float beta, float *C, const int ldc) nogil:
+         const float alpha, const float *A, const int lda, const float *B, const int ldb, const float beta, float *C, const int ldc) noexcept nogil:
     cdef char transA = 0#'\0'
     cdef char transB = 0#'\0'
     if (Order == CblasColMajor):
         if (TransA == CblasTrans):
             transA = 84#'T'
         elif (TransA == CblasConjTrans):
             transA = 67#'C'
@@ -342,15 +342,15 @@
             transA = 67#'C'
         else:
             transA = 78#'N'
 
         (<sgemm_>sgemm)(&transA, &transB, &N, &M, &K, &alpha, B, &ldb, A, &lda, &beta, C, &ldc)
 
 cdef public void cblas_sgemv(const int order,  const int TransA,  const int m, const int n,
-         const float alpha, const float  *a, const int lda,  const float  *x, const int incx,  const float beta,  float  *y, const int incy) nogil:
+         const float alpha, const float  *a, const int lda,  const float  *x, const int incx,  const float beta,  float  *y, const int incy) noexcept nogil:
     cdef char trans = 0#'\0'
     if (order == CblasColMajor):
         if (TransA == CblasNoTrans):
             trans = 78#'N'
         elif (TransA == CblasTrans):
             trans = 84#'T'
         else:
@@ -365,15 +365,15 @@
             trans = 78#'N'
         else:
             trans = 78#'N'
 
         (<sgemv_>sgemv)(&trans, &n, &m, &alpha, a, &lda, x, &incx, &beta, y, &incy);
 
 cdef public void cblas_ssymv(const int order, const int Uplo, const int N, const float alpha, const float *A,
-                 const int lda, const float *X, const int incX, const float beta, float *Y, const int incY) nogil:
+                 const int lda, const float *X, const int incX, const float beta, float *Y, const int incY) noexcept nogil:
     cdef char uplo = 0#'\0';
     if (order == CblasColMajor):
         if (Uplo == CblasUpper):
             uplo = 85#'U'
         else:
             uplo = 76#'L'
 
@@ -382,33 +382,33 @@
             uplo = 76#'L'
         else:
             uplo = 85#'U'
 
     (<ssymv_>ssymv)(&uplo, &N, &alpha, A, &lda, X, &incX, &beta, Y, &incY)
 
 cdef public void cblas_sger(const int order, const int m, const int n, const float alpha,
-                const float *x, const int incx, const float *y, const int incy, float *a, const int lda) nogil:
+                const float *x, const int incx, const float *y, const int incy, float *a, const int lda) noexcept nogil:
     if (order == CblasColMajor):
         (<sger_>sger)(&m, &n, &alpha, x, &incx, y, &incy, a, &lda);
 
     else:
         (<sger_>sger)(&n, &m, &alpha, y, &incy, x, &incx, a, &lda);
 
-cdef public void sposv_(const char* uplo, const int* m, const int* n, float* x, const int* ldx, float* y, const int* ldy, int* info) nogil:
+cdef public void sposv_(const char* uplo, const int* m, const int* n, float* x, const int* ldx, float* y, const int* ldy, int* info) noexcept nogil:
     (<sposv__>sposv)(uplo, m, n, x, ldx, y, ldy, info)
 
-cdef public void slacpy_(const char* uplo, const int* m, const int* n, const float* x, const int* ldx, float* y, const int* ldy) nogil:
+cdef public void slacpy_(const char* uplo, const int* m, const int* n, const float* x, const int* ldx, float* y, const int* ldy) noexcept nogil:
     (<slacpy__>slacpy)(uplo, m, n, x, ldx, y, ldy)
 
-cdef public void spotrf_(const char* a1, const int* a2, float* a3, const int* a4, int* a5) nogil:
+cdef public void spotrf_(const char* a1, const int* a2, float* a3, const int* a4, int* a5) noexcept nogil:
     (<spotrf__>spotrf)(a1, a2, a3, a4, a5)
 
-cdef public void spotrs_(const char* a1, const int* a2, const int* a3, const float* a4, const int* a5, float* a6, const int* a7, int* a8) nogil:
+cdef public void spotrs_(const char* a1, const int* a2, const int* a3, const float* a4, const int* a5, float* a6, const int* a7, int* a8) noexcept nogil:
     (<spotrs__>spotrs)(a1, a2, a3, a4, a5, a6, a7, a8)
 
 cdef public void sgelsd_(const int* a1, const int* a2, const int* a3,
              float* a4, const int* a5,
              float* a6, const int* a7,
              float* a8, const float* a9, int* a10, float* a11,
-             const int* a12, int* a13, int* a14) nogil:
+             const int* a12, int* a13, int* a14) noexcept nogil:
     (<sgelsd__>sgelsd)(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14)
```

### Comparing `cmfrec-3.5.1.post4/cmfrec/wrapper_untyped.pxi` & `cmfrec-3.5.1.post5/cmfrec/wrapper_untyped.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         int_t k_main, int_t k_user, int_t k_item,
         real_t w_main, real_t w_user, real_t w_item,
         int_t n_corr_pairs, size_t maxiter, int_t seed,
         int nthreads, bint prefer_onepass,
         bint verbose, int_t print_every, bint handle_interrupt,
         int_t *niter, int_t *nfev,
         real_t *B_plus_bias
-    ) nogil
+    ) noexcept nogil
 
     int_t fit_offsets_explicit_lbfgs_internal(
         real_t *values, bint reset_values,
         real_t *glob_mean,
         int_t m, int_t n, int_t k,
         int_t ixA[], int_t ixB[], real_t *X, size_t nnz,
         real_t *Xfull,
@@ -60,15 +60,15 @@
         real_t w_user, real_t w_item,
         int_t n_corr_pairs, size_t maxiter, int_t seed,
         int nthreads, bint prefer_onepass,
         bint verbose, int_t print_every, bint handle_interrupt,
         int_t *niter, int_t *nfev,
         real_t *Am, real_t *Bm,
         real_t *B_plus_bias
-    ) nogil
+    ) noexcept nogil
 
     int_t fit_collective_explicit_als(
         real_t *biasA, real_t *biasB,
         real_t *A, real_t *B,
         real_t *C, real_t *D,
         real_t *Ai, real_t *Bi,
         bint add_implicit_features,
@@ -102,15 +102,15 @@
         real_t *precomputedTransBtBinvBt,
         real_t *precomputedBtXbias,
         real_t *precomputedBeTBeChol,
         real_t *precomputedBiTBi,
         real_t *precomputedTransCtCinvCt,
         real_t *precomputedCtCw,
         real_t *precomputedCtUbias
-    ) nogil
+    ) noexcept nogil
 
     int_t fit_collective_implicit_als(
         real_t *A, real_t *B,
         real_t *C, real_t *D,
         bint reset_values, int_t seed,
         real_t *U_colmeans, real_t *I_colmeans,
         int_t m, int_t n, int_t k,
@@ -131,15 +131,15 @@
         bint use_cg, int_t max_cg_steps, bint precondition_cg, bint finalize_chol,
         bint nonneg, int_t max_cd_steps, bint nonneg_C, bint nonneg_D,
         bint precompute_for_predictions,
         real_t *precomputedBtB,
         real_t *precomputedBeTBe,
         real_t *precomputedBeTBeChol,
         real_t *precomputedCtUbias
-    ) nogil
+    ) noexcept nogil
 
     int_t fit_offsets_als(
         real_t *biasA, real_t *biasB,
         real_t *A, real_t *B,
         real_t *C, real_t *C_bias,
         real_t *D, real_t *D_bias,
         bint reset_values, int_t seed,
@@ -159,15 +159,15 @@
         int_t max_cg_steps, bint finalize_chol,
         bint verbose, bint handle_interrupt,
         bint precompute_for_predictions,
         real_t *Am, real_t *Bm,
         real_t *Bm_plus_bias,
         real_t *precomputedBtB,
         real_t *precomputedTransBtBinvBt
-    ) nogil
+    ) noexcept nogil
 
     int_t precompute_collective_explicit(
         real_t *B, int_t n, int_t n_max, bint include_all_X,
         real_t *C, int_t p,
         real_t *Bi, bint add_implicit_features,
         real_t *biasB, real_t glob_mean, bint NA_as_zero_X,
         real_t *U_colmeans, bint NA_as_zero_U,
@@ -183,87 +183,87 @@
         real_t *TransBtBinvBt,
         real_t *BtXbias,
         real_t *BeTBeChol,
         real_t *BiTBi,
         real_t *TransCtCinvCt,
         real_t *CtCw,
         real_t *CtUbias
-    ) nogil
+    ) noexcept nogil
 
     int_t precompute_collective_implicit(
         real_t *B, int_t n,
         real_t *C, int_t p,
         real_t *U_colmeans, bint NA_as_zero_U,
         int_t k, int_t k_user, int_t k_item, int_t k_main,
         real_t lam, real_t w_main, real_t w_user, real_t w_main_multiplier,
         bint nonneg,
         bint extra_precision,
         real_t *BtB,
         real_t *BeTBe,
         real_t *BeTBeChol,
         real_t *CtUbias
-    ) nogil
+    ) noexcept nogil
 
     int_t offsets_factors_cold(
         real_t *a_vec,
         real_t *u_vec,
         int_t u_vec_ixB[], real_t *u_vec_sp, size_t nnz_u_vec,
         real_t *C, int_t p,
         real_t *C_bias,
         int_t k, int_t k_sec, int_t k_main,
         real_t w_user
-    ) nogil
+    ) noexcept nogil
 
     void predict_multiple(
         real_t *A, int_t k_user,
         real_t *B, int_t k_item,
         real_t *biasA, real_t *biasB,
         real_t glob_mean,
         int_t k, int_t k_main,
         int_t m, int_t n,
         int_t predA[], int_t predB[], size_t nnz,
         real_t *outp,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t predict_X_old_collective_explicit(
         int_t row[], int_t col[], real_t *predicted, size_t n_predict,
         real_t *A, real_t *biasA,
         real_t *B, real_t *biasB,
         real_t glob_mean,
         int_t k, int_t k_user, int_t k_item, int_t k_main,
         int_t m, int_t n_max,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t topN(
         real_t *a_vec, int_t k_user,
         real_t *B, int_t k_item,
         real_t *biasB,
         real_t glob_mean, real_t biasA,
         int_t k, int_t k_main,
         int_t *include_ix, int_t n_include,
         int_t *exclude_ix, int_t n_exclude,
         int_t *outp_ix, real_t *outp_score,
         int_t n_top, int_t n, int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t topN_new_content_based(
         int_t k, int_t n_new,
         real_t *u_vec, int_t p,
         real_t *u_vec_sp, int_t u_vec_ixB[], size_t nnz_u_vec,
         real_t *II, int_t q,
         int_t I_row[], int_t I_col[], real_t *I_sp, size_t nnz_I,
         size_t I_csr_p[], int_t I_csr_i[], real_t *I_csr,
         real_t *C, real_t *C_bias,
         real_t *D, real_t *D_bias,
         real_t glob_mean,
         int_t *outp_ix, real_t *outp_score,
         int_t n_top, int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t fit_most_popular(
         real_t *biasA, real_t *biasB,
         real_t *glob_mean,
         real_t lam_user, real_t lam_item,
         bint scale_lam, bint scale_bias_const,
         real_t alpha,
@@ -271,15 +271,15 @@
         int_t ixA[], int_t ixB[], real_t *X, size_t nnz,
         real_t *Xfull,
         real_t *weight,
         bint implicit, bint adjust_weight, bint apply_log_transf,
         bint nonneg, bint NA_as_zero,
         real_t *w_main_multiplier,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t impute_X_collective_explicit(
         int_t m, bint user_bias,
         real_t *U, int_t m_u, int_t p,
         bint NA_as_zero_U,
         bint nonneg,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
@@ -304,30 +304,30 @@
         real_t *BeTBeChol,
         real_t *BiTBi,
         real_t *TransCtCinvCt,
         real_t *CtCw,
         real_t *CtUbias,
         real_t *B_plus_bias,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t predict_X_old_content_based(
         real_t *predicted, size_t n_predict,
         int_t m_new, int_t k,
         int_t row[],
         int_t col[],
         int_t m_orig, int_t n_orig,
         real_t *U, int_t p,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
         size_t U_csr_p[], int_t U_csr_i[], real_t *U_csr,
         real_t *C, real_t *C_bias,
         real_t *Bm, real_t *biasB,
         real_t glob_mean,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t predict_X_new_content_based(
         real_t *predicted, size_t n_predict,
         int_t m_new, int_t n_new, int_t k,
         int_t row[], int_t col[],
         real_t *U, int_t p,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
@@ -335,22 +335,22 @@
         real_t *II, int_t q,
         int_t I_row[], int_t I_col[], real_t *I_sp, size_t nnz_I,
         size_t I_csr_p[], int_t I_csr_i[], real_t *I_csr,
         real_t *C, real_t *C_bias,
         real_t *D, real_t *D_bias,
         real_t glob_mean,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_content_based_single(
         real_t *a_vec, int_t k,
         real_t *u_vec, int_t p,
         real_t *u_vec_sp, int_t u_vec_ixB[], size_t nnz_u_vec,
         real_t *C, real_t *C_bias
-    ) nogil
+    ) noexcept nogil
 
     int_t fit_content_based_lbfgs(
         real_t *biasA, real_t *biasB,
         real_t *C, real_t *C_bias,
         real_t *D, real_t *D_bias,
         bint start_with_ALS, bint reset_values, int_t seed,
         real_t *glob_mean,
@@ -366,15 +366,15 @@
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
         int_t I_row[], int_t I_col[], real_t *I_sp, size_t nnz_I,
         int_t n_corr_pairs, size_t maxiter,
         int nthreads, bint prefer_onepass,
         bint verbose, int_t print_every, bint handle_interrupt,
         int_t *niter, int_t *nfev,
         real_t *Am, real_t *Bm
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_collective_explicit_single(
         real_t *a_vec, real_t *a_bias,
         real_t *u_vec, int_t p,
         real_t *u_vec_sp, int_t u_vec_ixB[], size_t nnz_u_vec,
         real_t *u_bin_vec, int_t pbin,
         bint NA_as_zero_U, bint NA_as_zero_X,
@@ -399,15 +399,15 @@
         real_t *BtXbias,
         real_t *BeTBeChol,
         real_t *BiTBi,
         real_t *CtCw,
         real_t *TransCtCinvCt,
         real_t *CtUbias,
         real_t *B_plus_bias
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_collective_implicit_single(
         real_t *a_vec,
         real_t *u_vec, int_t p,
         real_t *u_vec_sp, int_t u_vec_ixB[], size_t nnz_u_vec,
         bint NA_as_zero_U,
         bint nonneg,
@@ -418,15 +418,15 @@
         real_t lam, real_t l1_lam, real_t alpha, real_t w_main, real_t w_user,
         real_t w_main_multiplier,
         bint apply_log_transf,
         real_t *BeTBe,
         real_t *BtB,
         real_t *BeTBeChol,
         real_t *CtUbias
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_collective_explicit_multiple(
         real_t *A, real_t *biasA, int_t m,
         real_t *U, int_t m_u, int_t p,
         bint NA_as_zero_U, bint NA_as_zero_X,
         bint nonneg,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
@@ -454,15 +454,15 @@
         real_t *BeTBeChol,
         real_t *BiTBi,
         real_t *TransCtCinvCt,
         real_t *CtCw,
         real_t *CtUbias,
         real_t *B_plus_bias,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_collective_implicit_multiple(
         real_t *A, int_t m,
         real_t *U, int_t m_u, int_t p,
         bint NA_as_zero_U,
         bint nonneg,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
@@ -477,15 +477,15 @@
         real_t w_main_multiplier,
         bint apply_log_transf,
         real_t *BeTBe,
         real_t *BtB,
         real_t *BeTBeChol,
         real_t *CtUbias,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_offsets_explicit_single(
         real_t *a_vec, real_t *a_bias, real_t *output_a,
         real_t *u_vec, int_t p,
         real_t *u_vec_sp, int_t u_vec_ixB[], size_t nnz_u_vec,
         real_t *Xa, int_t ixB[], size_t nnz,
         real_t *Xa_dense, int_t n,
@@ -496,29 +496,29 @@
         int_t k, int_t k_sec, int_t k_main,
         real_t w_user,
         real_t lam, real_t *lam_unique,
         bint exact,
         real_t *precomputedTransBtBinvBt,
         real_t *precomputedBtB,
         real_t *Bm_plus_bias
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_offsets_implicit_single(
         real_t *a_vec,
         real_t *u_vec, int_t p,
         real_t *u_vec_sp, int_t u_vec_ixB[], size_t nnz_u_vec,
         real_t *Xa, int_t ixB[], size_t nnz,
         real_t *Bm, real_t *C,
         real_t *C_bias,
         int_t k, int_t n,
         real_t lam, real_t alpha,
         bint apply_log_transf,
         real_t *precomputedBtB,
         real_t *output_a
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_offsets_explicit_multiple(
         real_t *Am, real_t *biasA,
         real_t *A, int_t m,
         real_t *U, int_t p,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
         size_t U_csr_p[], int_t U_csr_i[], real_t *U_csr,
@@ -532,15 +532,15 @@
         int_t k, int_t k_sec, int_t k_main,
         real_t w_user,
         real_t lam, real_t *lam_unique, bint exact,
         real_t *precomputedTransBtBinvBt,
         real_t *precomputedBtB,
         real_t *Bm_plus_bias,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
     int_t factors_offsets_implicit_multiple(
         real_t *Am, int_t m,
         real_t *A,
         real_t *U, int_t p,
         int_t U_row[], int_t U_col[], real_t *U_sp, size_t nnz_U,
         size_t U_csr_p[], int_t U_csr_i[], real_t *U_csr,
@@ -549,24 +549,24 @@
         real_t *Bm, real_t *C,
         real_t *C_bias,
         int_t k, int_t n,
         real_t lam, real_t alpha,
         bint apply_log_transf,
         real_t *precomputedBtB,
         int nthreads
-    ) nogil
+    ) noexcept nogil
 
-    # void py_set_threads(int) nogil
-    # int py_get_threads() nogil
+    # void py_set_threads(int) noexcept nogil
+    # int py_get_threads() noexcept nogil
 
-cdef public void cy_printf(char *msg) nogil:
+cdef public void cy_printf(char *msg) noexcept nogil:
     with gil:
         python_printmsg(msg)
         stdout.flush()
-cdef public void cy_errprintf(char *msg) nogil:
+cdef public void cy_errprintf(char *msg) noexcept nogil:
     with gil:
         python_printerrmsg(msg)
         stderr.flush()
 
 def _get_has_openmp():
     return get_has_openmp()
 
@@ -3837,22 +3837,22 @@
             nthreads
         )
     if retval == 1:
         raise MemoryError("Could not allocate sufficient memory.")
 
     return Xfull
 
-cdef public void py_set_threads(int nthreads) nogil:
+cdef public void py_set_threads(int nthreads) noexcept nogil:
     with gil:
         try:
             threadpoolctl.threadpool_limits(limits=nthreads, user_api="blas")
         except Exception:
             pass
 
-cdef public int py_get_threads() nogil:
+cdef public int py_get_threads() noexcept nogil:
     with gil:
         try:
             res = threadpoolctl.threadpool_info()
             for el in res:
                 if el["user_api"] == "blas":
                     return el["num_threads"]
             return 1
```

### Comparing `cmfrec-3.5.1.post4/cmfrec.egg-info/SOURCES.txt` & `cmfrec-3.5.1.post5/cmfrec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/setup.py` & `cmfrec-3.5.1.post5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
     custom_blas_link_args = ["-lopenblas"]
     from Cython.Distutils import build_ext
     build_ext_with_blas = build_ext
 
 setup(
     name  = "cmfrec",
     packages = ["cmfrec"],
-    version = '3.5.1-4',
+    version = '3.5.1-5',
     description = 'Collective matrix factorization',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/cmfrec',
     keywords = ['collaborative filtering', 'collective matrix factorization',
                 'relational learning'],
     install_requires=[
         'cython',
@@ -368,26 +368,28 @@
                      "src/collective.c", "src/common.c",
                      "src/offsets.c", "src/helpers.c", "src/lbfgs.c",
                      "src/cblas_wrappers.c"],
             include_dirs=[np.get_include(), "src"],
             define_macros = [("_FOR_PYTHON", None),
                              ("USE_DOUBLE", None),
                              ("NDEBUG", None),
+                             ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"),
                              ("USE_FINDBLAS" if use_findblas else "NO_FINDBLAS", None),
                              ("USE_BLAS_SYR" if use_findblas else "AVOID_BLAS_SYR", None)]
             ),
         Extension("cmfrec.wrapper_float",
             sources=["cmfrec/cfuns_float.pyx" if use_findblas else "cmfrec/cfuns_float_plusblas.pyx",
                      "src/collective.c", "src/common.c",
                      "src/offsets.c", "src/helpers.c", "src/lbfgs.c",
                      "src/cblas_wrappers.c"],
             include_dirs=[np.get_include(), "src"],
             define_macros = [("_FOR_PYTHON", None),
                              ("USE_FLOAT", None),
                              ("NDEBUG", None),
+                             ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION"),
                              ("USE_FINDBLAS" if use_findblas else "NO_FINDBLAS", None),
                              ("USE_BLAS_SYR" if use_findblas else "AVOID_BLAS_SYR", None)]
             ),
         ]
 )
 
 if not found_omp:
```

### Comparing `cmfrec-3.5.1.post4/src/arithmetic_ansi.h` & `cmfrec-3.5.1.post5/src/arithmetic_ansi.h`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/cblas_wrappers.c` & `cmfrec-3.5.1.post5/src/cblas_wrappers.c`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/cmfrec.h` & `cmfrec-3.5.1.post5/src/cmfrec.h`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/collective.c` & `cmfrec-3.5.1.post5/src/collective.c`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/common.c` & `cmfrec-3.5.1.post5/src/common.c`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/helpers.c` & `cmfrec-3.5.1.post5/src/helpers.c`

 * *Files 0% similar despite different names*

```diff
@@ -1233,15 +1233,15 @@
 (
     int_t m, int_t n,
     real_t *restrict A, int_t lda,
     real_t *restrict B, int_t ldb
 )
 {
     char uplo = '?';
-    if (m == 0 && n == 0) return;
+    if (m == 0 || n == 0) return;
 
     if (ldb == n && lda == n)
         memcpy(B, A, (size_t)m*(size_t)n*sizeof(real_t));
     else
         tlacpy_(&uplo, &n, &m, A, &lda, B, &ldb);
 }
 
@@ -1259,28 +1259,28 @@
     for (size_t row = 0; row < m; row++)
         for (size_t col = 0; col < n; col++)
             B[col + row*ldb] += A[col + row*lda];
 }
 
 void transpose_mat2(real_t *restrict A, size_t m, size_t n, real_t *restrict outp)
 {
-    for (size_t row = 0; row < m; row++)
-        for (size_t col = 0; col < n; col++)
+    for (size_t col = 0; col < n; col++)
+        for (size_t row = 0; row < m; row++)
             outp[row + col*m] = A[col + row*n];
 }
 
 void transpose_mat3
 (
     real_t *restrict A, size_t lda,
     size_t m, size_t n,
     real_t *restrict outp, size_t ldb
 )
 {
-    for (size_t row = 0; row < m; row++)
-        for (size_t col = 0; col < n; col++)
+    for (size_t col = 0; col < n; col++)
+        for (size_t row = 0; row < m; row++)
             outp[row + col*ldb] = A[col + row*lda];
 }
 
 int_t coo_to_csr_plus_alloc
 (
     int_t *restrict Xrow, int_t *restrict Xcol, real_t *restrict Xval,
     real_t *restrict W,
```

### Comparing `cmfrec-3.5.1.post4/src/lbfgs.c` & `cmfrec-3.5.1.post5/src/lbfgs.c`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/lbfgs.h` & `cmfrec-3.5.1.post5/src/lbfgs.h`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/offsets.c` & `cmfrec-3.5.1.post5/src/offsets.c`

 * *Files identical despite different names*

### Comparing `cmfrec-3.5.1.post4/src/ziggurat.h` & `cmfrec-3.5.1.post5/src/ziggurat.h`

 * *Files identical despite different names*

