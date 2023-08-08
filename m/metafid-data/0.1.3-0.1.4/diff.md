# Comparing `tmp/metafid_data-0.1.3-py3-none-any.whl.zip` & `tmp/metafid_data-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 10493 bytes, number of entries: 20
+Zip file size: 10843 bytes, number of entries: 20
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mf_data/__init__.py
 -rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 mf_data/ise/__init__.py
--rw-r--r--  2.0 unx      696 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard.py
+-rw-r--r--  2.0 unx     1054 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard.py
 -rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/__init__.py
--rw-r--r--  2.0 unx      973 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/clean_and_extend_data.py
--rw-r--r--  2.0 unx      322 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/columns.py
--rw-r--r--  2.0 unx      252 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/constants.py
+-rw-r--r--  2.0 unx     2332 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/clean_and_extend_data.py
+-rw-r--r--  2.0 unx     1024 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/columns.py
+-rw-r--r--  2.0 unx      458 b- defN 80-Jan-01 00:00 mf_data/ise/rahavard_utils/constants.py
 -rw-r--r--  2.0 unx     3708 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc.py
 -rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc_utils/__init__.py
 -rw-r--r--  2.0 unx     3637 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc_utils/clean_and_extend_data.py
 -rw-r--r--  2.0 unx     3763 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc_utils/columns.py
 -rw-r--r--  2.0 unx     2750 b- defN 80-Jan-01 00:00 mf_data/ise/tsetmc_utils/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mf_data/tgju/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mf_data/tgju/tgju.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 mf_data/utils/__init__.py
 -rw-r--r--  2.0 unx      992 b- defN 80-Jan-01 00:00 mf_data/utils/async_.py
 -rw-r--r--  2.0 unx      278 b- defN 80-Jan-01 00:00 mf_data/utils/get.py
--rw-r--r--  2.0 unx     1086 b- defN 80-Jan-01 00:00 metafid_data-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 metafid_data-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1687 b- defN 16-Jan-01 00:00 metafid_data-0.1.3.dist-info/RECORD
-20 files, 20495 bytes uncompressed, 7699 bytes compressed:  62.4%
+-rw-r--r--  2.0 unx     1137 b- defN 80-Jan-01 00:00 metafid_data-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 metafid_data-0.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1690 b- defN 16-Jan-01 00:00 metafid_data-0.1.4.dist-info/RECORD
+20 files, 23174 bytes uncompressed, 8049 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -45,17 +45,17 @@
 
 Filename: mf_data/utils/async_.py
 Comment: 
 
 Filename: mf_data/utils/get.py
 Comment: 
 
-Filename: metafid_data-0.1.3.dist-info/METADATA
+Filename: metafid_data-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: metafid_data-0.1.3.dist-info/WHEEL
+Filename: metafid_data-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: metafid_data-0.1.3.dist-info/RECORD
+Filename: metafid_data-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mf_data/ise/rahavard.py

```diff
@@ -16,7 +16,15 @@
         df = pd.json_normalize(self.stock()["asset_data_list"])[["asset.trade_symbol", "asset.id"]]
         df.set_index("asset.trade_symbol", inplace=True)
         return df.to_dict()["asset.id"]
 
     def balance_sheet(self, symbol_far):
         t = get(self.url.balance_sheet(symbol_id=self.symbol_id_.get(symbol_far)), verify=None).text
         return ced.balance_sheet(t)
+
+    def income_statements(self, symbol_far):
+        t = get(self.url.income_statements(symbol_id=self.symbol_id_.get(symbol_far)), verify=None).text
+        return ced.income_statements(t)
+
+    def cash_flow(self, symbol_far):
+        t = get(self.url.cash_flow(symbol_id=self.symbol_id_.get(symbol_far)), verify=None).text
+        return ced.cash_flow(t)
```

## mf_data/ise/rahavard_utils/clean_and_extend_data.py

```diff
@@ -1,29 +1,55 @@
 import jdatetime
 from collections import namedtuple
 import re
 import json
 import pandas as pd
 from .columns import cols
 
-Ced = namedtuple("RahavardCed", ["parser", "balance_sheet"])
+Ced = namedtuple("RahavardCed", ["parser", "balance_sheet", "income_statements", "cash_flow"])
 
 
 # ------------ Rahavard 356 -------------
-def rahavard_parser(t):
-    t = t.split("var layoutModel =")[1].split(";")[0].strip()
+def rahavard_parser(t, split0="var layoutModel =", split1=";"):
+    t = t.split(split0)[1].split(split1)[0].strip()
     return json.loads(t)
 
 
 def balance_sheet(bs: json):
     bs = rahavard_parser(bs)
     meta = pd.json_normalize(bs.get("balance_sheets") * len(bs.get("balance_sheet_field_items")))
     data = pd.json_normalize(bs.get("balance_sheet_field_items"), record_path="items")
     df = meta.join(data)
     df = df.pivot_table(index=["date_time", "jalali_date_time", "fiscal_year", "jalali_fiscal_year"],
                         columns='field.english_title', values=["value"])
     df.columns = df.columns.get_level_values(1)
     df.reset_index(inplace=True)
-    return df.rename(columns=cols.bs.rename)
+    return df.rename(columns=cols.balance_sheet.rename)
 
 
-ced = Ced(parser=rahavard_parser, balance_sheet=balance_sheet)
+def income_statements(is_: json):
+    is_ = rahavard_parser(is_, split0="var viewModel =")
+    meta = pd.json_normalize(is_.get("profit_losses") * len(is_.get("profit_loss_field_items")))
+    data = pd.json_normalize(is_.get("profit_loss_field_items"), record_path="items")
+    df = meta.join(data)
+    df = df.pivot_table(index=["date_time", "jalali_date_time", "fiscal_year", "jalali_fiscal_year"],
+                        columns='field.english_title', values=["value"])
+    df.columns = df.columns.get_level_values(1)
+    df.reset_index(inplace=True)
+    return df.rename(columns=cols.income_statements.rename)
+
+
+def cash_flow(cf: json):
+    cf = rahavard_parser(cf)
+    meta = pd.json_normalize(cf.get("cash_flows") * len(cf.get("cash_flow_field_items")))
+    data = pd.json_normalize(cf.get("cash_flow_field_items"), record_path="items")
+    print(data["fild"])
+    df = meta.join(data)
+    print(df.columns)
+    df = df.pivot_table(index=["date_time", "jalali_date_time", "fiscal_year", "jalali_fiscal_year"],
+                        columns='field.english_title', values=["value"])
+    df.columns = df.columns.get_level_values(1)
+    df.reset_index(inplace=True)
+    return df.rename(columns=cols.cash_flow.rename)
+
+
+ced = Ced(parser=rahavard_parser, balance_sheet=balance_sheet, income_statements=income_statements, cash_flow= cash_flow)
```

## mf_data/ise/rahavard_utils/columns.py

```diff
@@ -1,13 +1,19 @@
 from collections import namedtuple
 
-
 Cols = namedtuple(
-    "Cols", ["bs",]
+    "Cols", ["balance_sheet", "income_statements", "cash_flow"]
 )
 Property = namedtuple("Property", ["rename", "drop", "rep"])
 
-_bs = {"rename":{"date_time":"issue_date", "jalali_date_time":"j_issue_date"}}
+_balance_sheet = {"rename": {"date_time": "issue_date", "jalali_date_time": "j_issue_date"}}
+_income_statements = {"rename": {"date_time": "issue_date", "jalali_date_time": "j_issue_date"}}
+_cash_flow = {"rename": {"date_time": "issue_date", "jalali_date_time": "j_issue_date"}}
 
-bs = Property(rename=_bs.get("rename"), drop=_bs.get("drop"), rep=_bs.get("rep"))
+balance_sheet = Property(rename=_balance_sheet.get("rename"), drop=_balance_sheet.get("drop"),
+                         rep=_balance_sheet.get("rep"))
+income_statements = Property(rename=_income_statements.get("rename"), drop=_income_statements.get("drop"),
+                             rep=_income_statements.get("rep"))
+cash_flow = Property(rename=_cash_flow.get("rename"), drop=_cash_flow.get("drop"),
+                             rep=_cash_flow.get("rep"))
 
-cols = Cols(bs=bs)
+cols = Cols(balance_sheet=balance_sheet, income_statements=income_statements, cash_flow=cash_flow)
```

## mf_data/ise/rahavard_utils/constants.py

```diff
@@ -3,7 +3,13 @@
         self.base_url = "https://rahavard365.com/"
 
     def stock(self):
         return f"{self.base_url}stock"
 
     def balance_sheet(self, symbol_id):
         return f"{self.base_url}asset/{symbol_id}/balancesheet"
+
+    def income_statements(self, symbol_id):
+        return f"{self.base_url}/asset/{symbol_id}/profitloss"
+
+    def cash_flow(self, symbol_id):
+        return f"{self.base_url}/asset/{symbol_id}/cashflow"
```

## Comparing `metafid_data-0.1.3.dist-info/METADATA` & `metafid_data-0.1.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: metafid-data
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/yghaderi/metafid-data
 Author: Yaghoub Ghadri
 Author-email: y.ghaderi@outlook.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jdatetime (>=4.1.1,<5.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/yghaderi/metafid-data
 Description-Content-Type: text/markdown
 
 # metafid
 
 ## install 
 ```bash
```

