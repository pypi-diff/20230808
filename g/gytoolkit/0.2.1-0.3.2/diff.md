# Comparing `tmp/gytoolkit-0.2.1.tar.gz` & `tmp/gytoolkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytoolkit-0.2.1.tar", max compression
+gzip compressed data, was "gytoolkit-0.3.2.tar", max compression
```

## Comparing `gytoolkit-0.2.1.tar` & `gytoolkit-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.2.1/LICENSE
--rw-r--r--   0        0        0      483 2023-08-01 10:58:00.116507 gytoolkit-0.2.1/README.md
--rw-r--r--   0        0        0      415 2023-08-01 10:58:43.516501 gytoolkit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-08-01 07:49:38.216504 gytoolkit-0.2.1/src/gytoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.2.1/src/gytoolkit/mailparser/__init__.py
--rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.2.1/src/gytoolkit/mailparser/constant.py
--rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.2.1/src/gytoolkit/mailparser/mailparser.py
--rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.2.1/src/gytoolkit/mailparser/utils.py
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 gytoolkit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.3.2/LICENSE
+-rw-r--r--   0        0        0      483 2023-08-01 10:58:00.116507 gytoolkit-0.3.2/README.md
+-rw-r--r--   0        0        0      558 2023-08-08 04:59:37.866255 gytoolkit-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-08-07 11:01:29.200914 gytoolkit-0.3.2/src/gytoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.3.2/src/gytoolkit/mailparser/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.3.2/src/gytoolkit/mailparser/constant.py
+-rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.3.2/src/gytoolkit/mailparser/mailparser.py
+-rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.3.2/src/gytoolkit/mailparser/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:41:01.939594 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/__init__.py
+-rw-r--r--   0        0        0     1950 2023-08-07 10:39:02.480910 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/constants.py
+-rw-r--r--   0        0        0    24537 2023-08-07 10:52:08.460913 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/inquire.py
+-rw-r--r--   0        0        0     1730 2023-08-07 11:06:14.830912 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 05:05:56.099594 gytoolkit-0.3.2/src/gytoolkit/reports/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:14:00.069592 gytoolkit-0.3.2/src/gytoolkit/reports/managerjudge.py
+-rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 gytoolkit-0.3.2/PKG-INFO
```

### Comparing `gytoolkit-0.2.1/LICENSE` & `gytoolkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.2.1/src/gytoolkit/mailparser/constant.py` & `gytoolkit-0.3.2/src/gytoolkit/mailparser/constant.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.2.1/src/gytoolkit/mailparser/mailparser.py` & `gytoolkit-0.3.2/src/gytoolkit/mailparser/mailparser.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.2.1/PKG-INFO` & `gytoolkit-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: gytoolkit
-Version: 0.2.1
+Version: 0.3.2
 Summary: 用于PB业务管理的工具集
 Home-page: https://gitee.com/xuan_qi/gytoolkit
 License: MIT
 Author: XUAN Qi
 Author-email: xuan.q@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cx-oracle (>=8.3.0,<9.0.0)
+Requires-Dist: jqdatasdk (>=1.9.0,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.3)
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://gitee.com/xuan_qi/gytoolkit
 Description-Content-Type: text/markdown
 
 # gytoolkit
 
 #### 介绍
```

