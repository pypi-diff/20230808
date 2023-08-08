# Comparing `tmp/gytoolkit-0.3.2.tar.gz` & `tmp/gytoolkit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytoolkit-0.3.2.tar", max compression
+gzip compressed data, was "gytoolkit-0.3.3.tar", max compression
```

## Comparing `gytoolkit-0.3.2.tar` & `gytoolkit-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.3.2/LICENSE
--rw-r--r--   0        0        0      483 2023-08-01 10:58:00.116507 gytoolkit-0.3.2/README.md
--rw-r--r--   0        0        0      558 2023-08-08 04:59:37.866255 gytoolkit-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      125 2023-08-07 11:01:29.200914 gytoolkit-0.3.2/src/gytoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.3.2/src/gytoolkit/mailparser/__init__.py
--rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.3.2/src/gytoolkit/mailparser/constant.py
--rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.3.2/src/gytoolkit/mailparser/mailparser.py
--rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.3.2/src/gytoolkit/mailparser/utils.py
--rw-r--r--   0        0        0        0 2023-08-02 02:41:01.939594 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/__init__.py
--rw-r--r--   0        0        0     1950 2023-08-07 10:39:02.480910 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/constants.py
--rw-r--r--   0        0        0    24537 2023-08-07 10:52:08.460913 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/inquire.py
--rw-r--r--   0        0        0     1730 2023-08-07 11:06:14.830912 gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/utils.py
--rw-r--r--   0        0        0        0 2023-08-02 05:05:56.099594 gytoolkit-0.3.2/src/gytoolkit/reports/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 07:14:00.069592 gytoolkit-0.3.2/src/gytoolkit/reports/managerjudge.py
--rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 gytoolkit-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.3.3/LICENSE
+-rw-r--r--   0        0        0      483 2023-08-01 10:58:00.116507 gytoolkit-0.3.3/README.md
+-rw-r--r--   0        0        0      558 2023-08-08 05:50:02.246255 gytoolkit-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-08-07 11:01:29.200914 gytoolkit-0.3.3/src/gytoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.3.3/src/gytoolkit/mailparser/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.3.3/src/gytoolkit/mailparser/constant.py
+-rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.3.3/src/gytoolkit/mailparser/mailparser.py
+-rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.3.3/src/gytoolkit/mailparser/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:41:01.939594 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/__init__.py
+-rw-r--r--   0        0        0     1950 2023-08-07 10:39:02.480910 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/constants.py
+-rw-r--r--   0        0        0    22633 2023-08-08 05:47:49.016255 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/inquire.py
+-rw-r--r--   0        0        0     1730 2023-08-07 11:06:14.830912 gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 05:05:56.099594 gytoolkit-0.3.3/src/gytoolkit/reports/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:14:00.069592 gytoolkit-0.3.3/src/gytoolkit/reports/managerjudge.py
+-rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 gytoolkit-0.3.3/PKG-INFO
```

### Comparing `gytoolkit-0.3.2/LICENSE` & `gytoolkit-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.2/pyproject.toml` & `gytoolkit-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gytoolkit"
-version = "0.3.2"
+version = "0.3.3"
 description = "用于PB业务管理的工具集"
 authors = ["XUAN Qi <xuan.q@foxmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://gitee.com/xuan_qi/gytoolkit"
```

### Comparing `gytoolkit-0.3.2/src/gytoolkit/mailparser/constant.py` & `gytoolkit-0.3.3/src/gytoolkit/mailparser/constant.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.2/src/gytoolkit/mailparser/mailparser.py` & `gytoolkit-0.3.3/src/gytoolkit/mailparser/mailparser.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/constants.py` & `gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/constants.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/inquire.py` & `gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/inquire.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from typing import Union, List
+from typing import List, Union
+
 import pandas as pd
 from sqlalchemy import select
+
 from .constants import (
+    AUM_MAPPER,
+    FUNDTYPE_PPW_MAP,
     SECOND_STRATEGY_PPW_MAP,
     STRATEGY_PPW_MAP,
     THIRD_STRATEGY_PPW_MAP,
-    AUM_MAPPER,
-    FUNDTYPE_PPW_MAP,
 )
 from .utils import DBConnection
 
 
 class Inquirer:
     def __init__(self, db: DBConnection) -> None:
         self.db = db
@@ -348,43 +350,14 @@
 
         stmt = select(t_qr_summary)
         if qr_ids is not None:
             stmt = stmt.where(t_qr_summary.c.qr_id.in_(qr_ids))
 
         return pd.read_sql(stmt, self.conn, index_col="id")
 
-    # 无此表
-    # def _get_company_grow_history(
-    #     self,
-    #     company_name: str = None,  # 管理人名称,模糊查询
-    #     company_ids: Union[str, List[str]] = None, # 排排网管理人id批量查询
-    # ):
-    #     """
-    #     管理人大事记
-    #     pvn_cm_company_grow_statis
-    #     """
-    #     t_company_grow_history = self.db.tables['smppw.pvn_cm_company_grow_statis']
-
-    #     if isinstance(company_ids, str):
-    #         company_ids = [company_ids]
-
-    #     stmt = select(
-    #         t_company_grow_history
-    #     )
-
-    #     if company_name is not None:
-    #         stmt = stmt.where(
-    #             t_company_grow_history.c.company_name.like(f'%{company_name}%'))
-
-    #     if company_ids is not None:
-    #         stmt = stmt.where(
-    #             t_company_grow_history.c.company_id.in_(company_ids))
-
-    #     return pd.read_sql(stmt, self.conn, index_col="company_id")
-
     def get_all_fund(
         self,
         types=["私募证券"],
         date=None,
     ):
         fund_type = [FUNDTYPE_PPW_MAP[type_name] for type_name in types]
 
@@ -609,65 +582,49 @@
         )
 
         most_recent_report_idx = reports.groupby("company_id")["report_date"].idxmax()
 
         summary = self._get_qr_summary(most_recent_report_idx)
 
         def desc_mertics(subdf):
-            metrics = {}
 
-            metrics["公司概况"] = subdf.query(
-                "second_root_name=='公司概况'"
-            ).node_name_content.squeeze()
-            metrics["股东情况"] = subdf.query(
-                "second_root_name=='股东情况'"
-            ).node_name_content.squeeze()
-            metrics["组织架构"] = subdf.query(
-                "second_root_name=='组织架构'"
-            ).node_name_content.squeeze()
-            metrics["核心人员背景"] = subdf.query(
-                "second_root_name=='核心人员背景'"
-            ).node_name_content.squeeze()
-            metrics["其他人员背景"] = subdf.query(
-                "second_root_name=='其他人员背景'"
-            ).node_name_content.squeeze()
-
-            metrics["策略类型"] = subdf.query(
-                "node_name=='策略类型'"
-            ).node_name_content.squeeze()
-            metrics["配置逻辑"] = subdf.query(
-                "node_name=='配置逻辑'"
-            ).node_name_content.squeeze()
-            metrics["持仓特征"] = subdf.query(
-                "node_name=='持仓特征'"
-            ).node_name_content.squeeze()
-            metrics["交易风格"] = subdf.query(
-                "node_name=='交易风格'"
-            ).node_name_content.squeeze()
-
-            metrics["风控手段"] = subdf.query(
-                "second_root_name=='风控手段'"
-            ).node_name_content.squeeze()
-            metrics["风控效果"] = subdf.query(
-                "second_root_name=='风控效果'"
-            ).node_name_content.squeeze()
-
-            metrics["管理规模"] = subdf.query(
-                "second_root_name=='管理规模'"
-            ).node_name_content.squeeze()
-            metrics["产品概述"] = subdf.query(
-                "second_root_name=='产品概述'"
-            ).node_name_content.squeeze()
-            metrics["代表产品"] = subdf.query(
-                "second_root_name=='代表产品'"
-            ).node_name_content.squeeze()
-            metrics["其他产品"] = subdf.query(
-                "second_root_name=='其他产品'"
-            ).node_name_content.squeeze()
+            def process_query(subdf,query_arg,levl_name):
+                rlt = subdf.query(f"{levl_name}=='{query_arg}'")
+                if rlt.empty:
+                    return None
+                else:
+                    return rlt.node_name_content.squeeze()
+            
+            metrics = {}
+            
+            querys = {
+                "公司概况":"second_root_name",
+                "股东情况":"second_root_name",
+                "组织架构":"second_root_name",
+                "核心人员背景":"second_root_name",
+                "其他人员背景":"second_root_name",
+
+                "策略类型":"node_name",
+                "配置逻辑":"node_name",
+                "持仓特征":"node_name",
+                "交易风格":"node_name",
+
+                "风控手段":"second_root_name",
+                "风控效果":"second_root_name",
+                "管理规模":"second_root_name",
+                "产品概述":"second_root_name",
+                "代表产品":"second_root_name",
+                "其他产品":"second_root_name",
+
+                "结论":"root_name",                
+            }
+
+            for query_arg,levl_name in querys.items():
+                rlt = process_query(subdf,query_arg,levl_name)
+                metrics[query_arg] = rlt
 
-            metrics["结论"] = subdf.query("root_name=='结论'").node_name_content.squeeze()
             return pd.Series(metrics)
 
         metrics = summary.groupby("qr_id").apply(desc_mertics)
         metrics["company_id"] = reports.loc[metrics.index].company_id
         metrics.set_index("company_id", drop=True, inplace=True)
         return metrics
```

### Comparing `gytoolkit-0.3.2/src/gytoolkit/ppwdbapi/utils.py` & `gytoolkit-0.3.3/src/gytoolkit/ppwdbapi/utils.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.3.2/PKG-INFO` & `gytoolkit-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gytoolkit
-Version: 0.3.2
+Version: 0.3.3
 Summary: 用于PB业务管理的工具集
 Home-page: https://gitee.com/xuan_qi/gytoolkit
 License: MIT
 Author: XUAN Qi
 Author-email: xuan.q@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

