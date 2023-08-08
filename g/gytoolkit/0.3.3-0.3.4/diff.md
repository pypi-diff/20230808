# Comparing `tmp/gytoolkit-0.3.3.tar.gz` & `tmp/gytoolkit-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytoolkit-0.3.3.tar", max compression
+gzip compressed data, was "gytoolkit-0.3.4.tar", max compression
```

## Comparing `gytoolkit-0.3.3.tar` & `gytoolkit-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.3.3/LICENSE
--rw-r--r--   0        0        0      483 2023-08-01 10:58:00.116507 gytoolkit-0.3.3/README.md
--rw-r--r--   0        0        0      558 2023-08-08 05:50:02.246255 gytoolkit-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      125 2023-08-07 11:01:29.200914 gytoolkit-0.3.3/src/gytoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.3.3/src/gytoolkit/mailparser/__init__.py
--rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.3.3/src/gytoolkit/mailparser/constant.py
--rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.3.3/src/gytoolkit/mailparser/mailparser.py
--rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.3.3/src/gytoolkit/mailparser/utils.py
--rw-r--r--   0        0        0        0 2023-08-02 02:41:01.939594 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/__init__.py
--rw-r--r--   0        0        0     1950 2023-08-07 10:39:02.480910 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/constants.py
--rw-r--r--   0        0        0    22633 2023-08-08 05:47:49.016255 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/inquire.py
--rw-r--r--   0        0        0     1730 2023-08-07 11:06:14.830912 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/utils.py
--rw-r--r--   0        0        0        0 2023-08-02 05:05:56.099594 gytoolkit-0.3.3/src/gytoolkit/reports/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 07:14:00.069592 gytoolkit-0.3.3/src/gytoolkit/reports/managerjudge.py
--rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 gytoolkit-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.3.4/LICENSE
+-rw-r--r--   0        0        0      483 2023-08-01 10:58:00.116507 gytoolkit-0.3.4/README.md
+-rw-r--r--   0        0        0      558 2023-08-08 07:03:13.326258 gytoolkit-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-08-07 11:01:29.200914 gytoolkit-0.3.4/src/gytoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.3.4/src/gytoolkit/mailparser/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.3.4/src/gytoolkit/mailparser/constant.py
+-rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.3.4/src/gytoolkit/mailparser/mailparser.py
+-rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.3.4/src/gytoolkit/mailparser/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:41:01.939594 gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/__init__.py
+-rw-r--r--   0        0        0     1950 2023-08-07 10:39:02.480910 gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/constants.py
+-rw-r--r--   0        0        0    22898 2023-08-08 06:51:23.016256 gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/inquire.py
+-rw-r--r--   0        0        0     1730 2023-08-07 11:06:14.830912 gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 05:05:56.099594 gytoolkit-0.3.4/src/gytoolkit/reports/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:14:00.069592 gytoolkit-0.3.4/src/gytoolkit/reports/managerjudge.py
+-rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 gytoolkit-0.3.4/PKG-INFO
```

### Comparing `gytoolkit-0.3.3/LICENSE` & `gytoolkit-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.3/pyproject.toml` & `gytoolkit-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gytoolkit"
-version = "0.3.3"
+version = "0.3.4"
 description = "用于PB业务管理的工具集"
 authors = ["XUAN Qi <xuan.q@foxmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://gitee.com/xuan_qi/gytoolkit"
```

### Comparing `gytoolkit-0.3.3/src/gytoolkit/mailparser/constant.py` & `gytoolkit-0.3.4/src/gytoolkit/mailparser/constant.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.3/src/gytoolkit/mailparser/mailparser.py` & `gytoolkit-0.3.4/src/gytoolkit/mailparser/mailparser.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/constants.py` & `gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/constants.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/inquire.py` & `gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/inquire.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,29 +588,34 @@
         def desc_mertics(subdf):
 
             def process_query(subdf,query_arg,levl_name):
                 rlt = subdf.query(f"{levl_name}=='{query_arg}'")
                 if rlt.empty:
                     return None
                 else:
-                    return rlt.node_name_content.squeeze()
+                    rlt = rlt.node_name_content.squeeze()
+                    if isinstance(rlt,pd.Series):
+                        rlt = '\n'.join([f"策略{idx+1}:{val}" for idx, val in enumerate(rlt)])
+                    return rlt
             
             metrics = {}
             
             querys = {
                 "公司概况":"second_root_name",
                 "股东情况":"second_root_name",
                 "组织架构":"second_root_name",
                 "核心人员背景":"second_root_name",
                 "其他人员背景":"second_root_name",
 
                 "策略类型":"node_name",
+                "大类资产配置":"node_name",
                 "配置逻辑":"node_name",
                 "持仓特征":"node_name",
                 "交易风格":"node_name",
+                "容量":"node_name",
 
                 "风控手段":"second_root_name",
                 "风控效果":"second_root_name",
                 "管理规模":"second_root_name",
                 "产品概述":"second_root_name",
                 "代表产品":"second_root_name",
                 "其他产品":"second_root_name",
```

### Comparing `gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/utils.py` & `gytoolkit-0.3.4/src/gytoolkit/ppwdbapi/utils.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.3/PKG-INFO` & `gytoolkit-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gytoolkit
-Version: 0.3.3
+Version: 0.3.4
 Summary: 用于PB业务管理的工具集
 Home-page: https://gitee.com/xuan_qi/gytoolkit
 License: MIT
 Author: XUAN Qi
 Author-email: xuan.q@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

