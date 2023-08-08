# Comparing `tmp/option_trader-0.2.3.tar.gz` & `tmp/option_trader-0.2.4.tar.gz`

## Comparing `option_trader-0.2.3.tar` & `option_trader-0.2.4.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/.vscode/launch.json
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/.vscode/settings.json
--rw-r--r--   0        0        0    85832 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/account.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/option_summary.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/position.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/quote.py
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/site.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/transaction.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/admin/user.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/option/butterfly.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/option/credit_iron_condor.py
--rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/option/single_option.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/option/spread.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/option/strategy.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/stock/bollingerBands.py
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/stock/macd.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/stock/mfi.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/backtest/stock/rsi.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/consts/asset.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/consts/predictor.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/consts/rgb.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/consts/strategy.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/jobs/account.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/jobs/core.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/jobs/site.py
--rw-r--r--   0        0        0    25258 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/Ananlyzer.ipynb
--rw-r--r--   0        0        0   431156 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/ML_TensorFlow_good.ipynb
--rw-r--r--   0        0        0   370663 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/ML_ochl.ipynb
--rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/MP_TensorFlow_bad.ipynb
--rw-r--r--   0        0        0   224231 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/admin.ipynb
--rw-r--r--   0        0        0   193512 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/ib.ipynb
--rw-r--r--   0        0        0   266277 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/ml.ipynb
--rw-r--r--   0        0        0    64170 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/option_geeks.ipynb
--rw-r--r--   0        0        0    58956 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/option_tools.ipynb
--rw-r--r--   0        0        0    28065 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/watchlist.ipynb
--rw-r--r--   0        0        0   251657 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb
--rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb
--rw-r--r--   0        0        0   370671 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb
--rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0    37481 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb
--rw-r--r--   0        0        0    25565 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb
--rw-r--r--   0        0        0    46403 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb
--rw-r--r--   0        0        0    44140 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/app_settings.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/ib_config.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/log_config.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/logging.conf
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/schema.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/ta_strategy.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/settings/trade_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/shell/analyzer.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/shell/backtester.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/shell/dataset_tool.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/shell/line.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/calc_prob.py
--rw-r--r--   0        0        0    72828 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/data_getter.py
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/data_getter_ib.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/line_norify.py
--rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/monitor.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/option_tool.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 option_trader-0.2.3/option_trader/utils/predictor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 option_trader-0.2.3/.gitignore
--rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 option_trader-0.2.3/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 option_trader-0.2.3/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 option_trader-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 option_trader-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    25258 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/Ananlyzer.ipynb
+-rw-r--r--   0        0        0   431156 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/ML_TensorFlow_good.ipynb
+-rw-r--r--   0        0        0   370663 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/ML_ochl.ipynb
+-rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/MP_TensorFlow_bad.ipynb
+-rw-r--r--   0        0        0   118262 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/admin.ipynb
+-rw-r--r--   0        0        0   193512 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/ib.ipynb
+-rw-r--r--   0        0        0   266277 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/ml.ipynb
+-rw-r--r--   0        0        0    64170 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/option_geeks.ipynb
+-rw-r--r--   0        0        0    58956 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/option_tools.ipynb
+-rw-r--r--   0        0        0    28065 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/watchlist.ipynb
+-rw-r--r--   0        0        0   251657 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb
+-rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb
+-rw-r--r--   0        0        0   370671 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb
+-rw-r--r--   0        0        0   359863 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0    37481 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb
+-rw-r--r--   0        0        0    25565 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb
+-rw-r--r--   0        0        0    46403 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb
+-rw-r--r--   0        0        0    44140 2020-02-02 00:00:00.000000 option_trader-0.2.4/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/.vscode/launch.json
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/.vscode/settings.json
+-rw-r--r--   0        0        0    87391 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/account.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/option_summary.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/position.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/quote.py
+-rw-r--r--   0        0        0    14922 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/site.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/transaction.py
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/tests/__init__.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/admin/tests/test_admin.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/option/butterfly.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/option/credit_iron_condor.py
+-rw-r--r--   0        0        0    10029 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/option/single_option.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/option/spread.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/option/strategy.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/stock/bollingerBands.py
+-rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/stock/macd.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/stock/mfi.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/backtest/stock/rsi.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/consts/asset.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/consts/predictor.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/consts/rgb.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/consts/strategy.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/jobs/account.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/jobs/core.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/jobs/site.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/app_settings.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/ib_config.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/log_config.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/logging.conf
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/schema.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/ta_strategy.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/settings/trade_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/shell/analyzer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/shell/backtester.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/shell/dataset_tool.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/shell/line.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/calc_prob.py
+-rw-r--r--   0        0        0    72730 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/data_getter.py
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/data_getter_ib.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/line_norify.py
+-rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/monitor.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/option_tool.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 option_trader-0.2.4/option_trader/utils/predictor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 option_trader-0.2.4/.gitignore
+-rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 option_trader-0.2.4/LICENSE
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 option_trader-0.2.4/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 option_trader-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 option_trader-0.2.4/PKG-INFO
```

### Comparing `option_trader-0.2.3/option_trader/.vscode/launch.json` & `option_trader-0.2.4/option_trader/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/admin/account.py` & `option_trader-0.2.4/option_trader/admin/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,32 @@
 
 account_profile_schema = "user_name TEXT, account_name TEXT NOT NULL PRIMARY KEY,equaty_percentage REAL,\
         available_to_tread REAL,available_to_trade_wo_margin REAL,non_margin_buy_power REAL,\
         margin_buy_power REAL,available_to_withdraw REAL,cash_only REAL,cash_and_margin REAL,\
         house_surplus REAL,sma REAL,exchange_surplue REAL,cash_core REAL,cash_credit_debit REAL,\
         margin_credit_debit REA,market_value_securities REAL,held_in_cash REAL, held_in_margin REAL,\
         cash_buy_power REAL,settled_cash REAL,initial_balance REAL,risk_mgr TEXT, entry_crit TEXT,\
-        market_condition TEXT, runtime_config TEXT,default_strategy TEXT, default_predictor TEXT,\
+        market_condition TEXT, runtime_config TEXT, default_strategy_list TEXT, default_watchlist TEXT, default_predictor TEXT,\
         FOREIGN KEY(user_name) REFERENCES user(name)"   
 
 class account():
 
-    def __init__(self, user, account_name, watchlist_name="", initial_balance=app_settings.DEFAULT_ACCOUNT_INITIAL_BALANCE):        
+    def __init__(self, user, account_name, initial_balance=app_settings.DEFAULT_ACCOUNT_INITIAL_BALANCE):        
         self.user = user
         self.account_name = account_name        
         self.logger = logging.getLogger(__name__)
 
         if settings.DATABASES == 'sqlite3':
             try:
                 self.db_path = user.user_home_dir + "/"+account_name+"_account.db"                
 
                 if os.path.exists(self.db_path) :
                     self.db_conn  = sqlite3.connect(self.db_path)                     
-                    self.strategy_list = self.get_default_strategy()             
-
-                    if watchlist_name == "" or watchlist_name not in self.user.get_watchlist_name_list():
-                        self.watchlist = self.user.get_watchlist('default')
-                    else:
-                        self.watchlist = self.user.get_watchlist(watchlist_name)                                    
+                    self.strategy_list = self.get_default_strategy_list()             
+                    self.watchlist     = self.get_default_watchlist()                                         
                     self.entry_crit = self.get_default_entry_crit()
                     self.risk_mgr = self.get_default_risk_mgr()
                     self.runtime_config = self.get_default_runtime_config()
                     self.market_condition = self.get_default_market_condition()
                     self.initial_balace = self.get_initial_balance()
                     self.cash_position = self.get_cash_position()
                     self.margin_position = self.get_margin_position()                    
@@ -73,36 +69,30 @@
                 self.db_conn  = sqlite3.connect(self.db_path)  
                 cursor = self.db_conn.cursor()
                 cursor.execute("CREATE TABLE IF NOT EXISTS account_profile("+account_profile_schema+")")
                 cursor.execute("CREATE TABLE IF NOT EXISTS optionSummary("+option_summary.schema+")")
                 cursor.execute("CREATE TABLE IF NOT EXISTS position("+position.schema+")")
                 cursor.execute("CREATE TABLE IF NOT EXISTS transactions("+transaction.schema+")")
 
-                default_strategy = self.user.get_default_strategy()
-                self.strategy_list =  default_strategy             
-                self.update_default_strategy(default_strategy)                      
+                self.strategy_list = self.user.get_default_strategy_list()
+                self.watchlist = self.user.get_default_watchlist()                               
                 self.entry_crit = entryCrit()
                 self.risk_mgr = riskManager()
                 self.runtime_config = runtimeConfig()
                 self.market_condition = marketCondition()
-
-                if watchlist_name == "" or watchlist_name not in self.user.get_watchlist_name_list():
-                    self.watchlist = self.user.get_watchlist('default')
-                else:
-                    self.watchlist = self.user.get_watchlist(watchlist_name) 
-
-                sql = "INSERT INTO account_profile (user_name, account_name, initial_balance, default_strategy, entry_crit, runtime_config, risk_mgr, market_condition) VALUES (?, ?, ?, ?, ?, ?, ?, ?)"              
+                sql = "INSERT INTO account_profile (user_name, account_name, initial_balance, default_strategy_list, entry_crit, runtime_config, risk_mgr, market_condition, default_watchlist) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)"              
                 cursor.execute(sql, [user.user_name, 
                                     account_name, 
                                     initial_balance,
-                                    json.dumps(default_strategy),
+                                    json.dumps(self.strategy_list),
                                     json.dumps(vars(entryCrit())),
                                     json.dumps(vars(runtimeConfig())),
                                     json.dumps(vars(riskManager())),
-                                    json.dumps(vars(marketCondition()))                                     
+                                    json.dumps(vars(marketCondition())),
+                                    json.dumps(self.watchlist)                                     
                                 ])               
                 sql = 'INSERT INTO position (symbol, quantity) VALUES(?,?)' 
                 cursor.execute(sql, [asset.CASH, initial_balance])
                 cursor.execute(sql, [asset.MARGIN, 0])                
                 self.cash_position = initial_balance
                 self.margin_position = 0
                 self.db_conn.commit()       
@@ -144,32 +134,58 @@
                 self.db_conn.commit()      
                 self.update_cash_position(initial_balance)
             except Exception as e:
                 self.logger.exception(e)             
         else:
             self.logger.error("sqlite3 only for now %s")
 
-    def get_default_strategy(self):
+    def get_default_strategy_list(self):
         if settings.DATABASES == 'sqlite3':                 
             try:    
-                sql = "SELECT default_strategy FROM account_profile"                
+                sql = "SELECT default_strategy_list FROM account_profile"                
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                return json.loads(cursor.fetchone()[0])                   
+            except Exception as e:
+                self.logger.exception(e)   
+                return []
+        else:
+            self.logger.error("sqlite3 only for now %s")
+
+    def get_default_watchlist(self):
+        if settings.DATABASES == 'sqlite3':                 
+            try:    
+                sql = "SELECT default_watchlist FROM account_profile"                
                 cursor = self.db_conn.cursor()                    
                 cursor.execute(sql)
                 return json.loads(cursor.fetchone()[0])                   
             except Exception as e:
                 self.logger.exception(e)   
                 return []
         else:
             self.logger.error("sqlite3 only for now %s")
 
     def update_default_strategy(self, strategy_list):
         self.strategy_list = strategy_list    
         if settings.DATABASES == 'sqlite3':
             try:
-                sql = "UPDATE account_profile SET default_strategy='"+json.dumps(strategy_list)+"' WHERE account_name='"+self.account_name+"'"                    
+                sql = "UPDATE account_profile SET default_strategy_list='"+json.dumps(strategy_list)+"' WHERE account_name='"+self.account_name+"'"                    
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                self.db_conn.commit()      
+            except Exception as e:
+                self.logger.exception(e)       
+        else:
+            self.logger.error('unsupported database engine %s' % settings.DATABASES)
+
+    def update_default_watchlist(self, watchlist):
+        self.watchlist = watchlist    
+        if settings.DATABASES == 'sqlite3':
+            try:
+                sql = "UPDATE account_profile SET default_watchlist='"+json.dumps(watchlist)+"' WHERE account_name='"+self.account_name+"'"                    
                 cursor = self.db_conn.cursor()                    
                 cursor.execute(sql)
                 self.db_conn.commit()      
             except Exception as e:
                 self.logger.exception(e)       
         else:
             self.logger.error('unsupported database engine %s' % settings.DATABASES)
@@ -184,14 +200,28 @@
             except Exception as e:
                 self.logger.exception(e)   
         else:
             self.logger.error("sqlite3 only for now %s")
 
         return None
 
+    def get_default_entry_crit(self):
+        if settings.DATABASES == 'sqlite3':                 
+            try:    
+                sql = "SELECT entry_crit FROM account_profile"                
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                return entryCrit(json.loads(cursor.fetchone()[0]))                 
+            except Exception as e:
+                self.logger.exception(e)   
+        else:
+            self.logger.error("sqlite3 only for now %s")
+
+        return None
+    
     def update_default_entry_crit(self, entry_crit):
 
         self.entry_crit = entry_crit
         if settings.DATABASES == 'sqlite3':                 
             try:    
                 sql = "UPDATE account_profile SET entry_crit='"+json.dumps(vars(entry_crit))+"' WHERE account_name='"+self.account_name+"'"                                 
                 cursor = self.db_conn.cursor()                    
@@ -613,15 +643,15 @@
 
         hostname = socket.gethostname()
                 
         if afterHours():
             msg = "[%s|%s|%s] CREATE PENDING [%s|%s|%s] [pri:%.2f|pnl:%.2f|prob:%.2f|q:%d] %s" % (hostname, self.user.user_name, self.account_name,\
                             strategy, symbol, exp_date, open_price, pnl, win_prob, quantity, self.print_legs(legs_desc))
             self.logger.info(msg)
-            lineNotifyMessage( msg)    
+            lineNotifyMessage( msg, token=self.user.notification_token)    
             return
         
         cash_position = self.get_cash_position()
         margin_position = self.get_margin_position()          
         if credit:        
             if math.isnan(margin_position):
                 margin_position = 0.0
@@ -653,15 +683,15 @@
         self.db_conn.commit()    
 
         msg = "[%s|%s|%s] CREATE [%s|%s|%s] [pri:%.2f|pnl:%.2f|prob:%.2f|q:%d] %s" % (hostname, self.user.user_name, self.account_name,\
                             strategy, symbol, exp_date, open_price, pnl, win_prob, quantity, self.print_legs(legs_desc))
 
         self.logger.info(msg)
 
-        lineNotifyMessage( msg)
+        lineNotifyMessage( msg, token=self.user.notification_token)    
                        
     def expire_optionSummary(self, srow):
         uuid = srow[option_summary.UUID]
         pdf= pd.read_sql_query("SELECT * FROM position WHERE uuid = '"+uuid+"'", self.db_conn)
 
         last_price = 0
         for i, prow in pdf.iterrows():
@@ -708,15 +738,15 @@
         hostname = socket.gethostname()
         
         msg = "[%s|%s|%s] EXPIRE [%s|%s|%s] [prof:%.2f|gain:%.2f|q:%d] %s" % (hostname, self.user.user_name, self.account_name,\
                             strategy, symbol, exp_date, pl, gain, quantity, self.print_legs(legs))
 
         self.logger.info(msg)                
 
-        lineNotifyMessage( msg)
+        lineNotifyMessage( msg, token=self.user.notification_token)    
 
     def roll_optionSummary(self, symbol, exp_date, strategy):
 
         today = datetime.now(timezone(app_settings.TIMEZONE))
 
         earning_date = get_next_earning_date(symbol)
         if earning_date is not None:
@@ -848,15 +878,15 @@
 
                 hostname = socket.gethostname()
 
                 if afterHours():
                     msg = "[%s|%s|%s] STOP PENDING [%s|%s|%s] [open days %d|reason:%s|pl:%.2f|gain:%.2f|q:%d] %s" % (hostname, self.user.user_name, self.account_name,\
                                 strategy, symbol, exp_date, days_open, stop_reason, pl, gain, quantity, self.print_legs(legs))   
                     self.logger.info(msg)             
-                    lineNotifyMessage(msg)  
+                    lineNotifyMessage( msg, token=self.user.notification_token)    
                 else:
                     for i, prow in ppdf.iterrows():
                         self.close_position(prow)
 
                     if credit:             
                         margin =  (quantity * 100 * srow[option_summary.MARGIN])      
                         margin_position = self.get_margin_position() - margin
@@ -871,39 +901,37 @@
                     data = (last_price, pl, gain, last_quote_date, stop_date, stop_reason, asset.CLOSED, stock_price, uuid)                                
                     cursor = self.db_conn.cursor()    
                     cursor.execute(sql, data)     
                     self.db_conn.commit()   
                     msg = "[%s|%s|%s] STOP [%s|%s|%s] [open days %d|reason:%s|pl:%.2f|gain:%.2f|q:%d] %s" % (hostname, self.user.user_name, self.account_name,\
                                 strategy, symbol, exp_date, days_open, stop_reason, pl, gain, quantity, self.print_legs(legs))   
                     self.logger.info(msg)             
-                    lineNotifyMessage(msg)             
+                    lineNotifyMessage( msg, token=self.user.notification_token)            
                     if roll:            
                         self.roll_optionSummary(symbol, exp_date, strategy)                    
             else:
                 if afterHours() == False:
                     sql = """update optionSummary set last_price=?, pl=?, gain=?, last_quote_date=?, last_stock_price=? where uuid==?"""        
                     data = (last_price, pl, gain, today.strftime("%Y-%m-%d %H:%M:%S %Z"), stock_price, uuid)
                     cursor = self.db_conn.cursor()    
                     cursor.execute(sql, data)     
                     self.db_conn.commit()   
             
-
     def print_legs(self, leg_list):
         output_str = ''
     
         legs = json.loads(leg_list)
 
         for leg in legs:
             ld = json.loads(leg)
             leg_desc = ' [%s|%s|%.2f|%d|%s] ' % (ld['OPEN_ACTION'], ld['OTYPE'], ld['STRIKE'], ld['QUANTITY'], ld['EXP_DATE'])
             output_str += leg_desc
     
         return output_str
     
-
     def get_optionSummary(self, get_leg_dedail=True):    
         if settings.DATABASES == 'sqlite3':             
             df = pd.read_sql_query("SELECT * FROM optionSummary", self.db_conn)   
 
             if get_leg_dedail:
                 for i, row in df.iterrows():
                     index = 0                
@@ -947,15 +975,15 @@
             self.logger.error('Unsupported database engine %s' % settings.DATABASES)    
             return pd.DataFrame()        
 
     def try_open_new_strategy_positions(self, watchlist=[], strategy_list=[]):
         
         if settings.DATABASES == 'sqlite3':                         
                
-            watchlist = watchlist if len(watchlist) > 0 else self.user.get_watchlist('default')
+            watchlist = watchlist if len(watchlist) > 0 else self.get_default_watchlist()
  
             strategy_list = strategy_list if len(strategy_list) > 0 else self.get_default_strategy()
 
             df = pd.read_sql_query("SELECT * FROM optionSummary WHERE status = '"+asset.OPENED+"'", self.db_conn)   
             
             candidates = self.pick_strategy_candidates(watchlist, strategy_list)
```

### Comparing `option_trader-0.2.3/option_trader/admin/option_summary.py` & `option_trader-0.2.4/option_trader/admin/option_summary.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/admin/position.py` & `option_trader-0.2.4/option_trader/admin/position.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/admin/quote.py` & `option_trader-0.2.4/option_trader/admin/quote.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/admin/site.py` & `option_trader-0.2.4/option_trader/admin/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,219 +1,253 @@
 
-import sqlite3
-from pathlib import Path
-import os
-import json      
-
 import pandas as pd
+import os
+import json   
 
-import logging
-
-
-from option_trader.settings import app_settings   
+from option_trader.settings import app_settings  as settings    
 from option_trader.settings import schema as schema  
-from option_trader.admin import user
-from option_trader.utils.monitor import refresh_monitor_list
-from option_trader.consts import strategy 
-from option_trader.consts import asset
 
+from option_trader.utils.line_norify import lineNotifyMessage 
+from option_trader.admin.account import account
+from option_trader.settings import app_settings
+import re
+import sqlite3
+
+from pathlib import Path
 
+import logging
 
-class site():
+class user():  
 
-    def __init__(self, site_name, default_strategy=[]):        
+    def __init__(self, site, user_name):
         
-        self.site_name = site_name
-        self.user_root = app_settings.USER_ROOT_DIR
-        self.site_root = app_settings.SITE_ROOT_DIR
-        self.data_root = app_settings.DATA_ROOT_DIR
+        self.site = site
+        self.user_name = user_name
+        self.email = ""
+    
         self.logger = logging.getLogger(__name__)
+ 
+        self.user_home_dir = site.user_root + '/'+ self.user_name        
 
-        if app_settings.DATABASES == 'sqlite3':
-            try:                
-                self.db_path = app_settings.SITE_ROOT_DIR+"/"+site_name+"_site.db"
-
-                if os.path.exists(self.db_path ):
-                    self.db_conn   = sqlite3.connect(self.db_path)  
-                    if len(default_strategy) > 0:
-                        self.update_default_strategy(default_strategy)                        
-                    return
-                 
-                self.db_conn   = sqlite3.connect(self.db_path)  
-                cursor = self.db_conn.cursor()
-                cursor.execute("CREATE TABLE IF NOT EXISTS site_profile("+schema.site_profile+")")
-                cursor.execute("CREATE TABLE IF NOT EXISTS user_list("+schema.user_list+")")
-                cursor.execute("CREATE TABLE IF NOT EXISTS monitor("+schema.site_monitor_db+")")                                             
-                sql = "INSERT INTO site_profile (site_name, default_strategy) VALUES (?, ?)"              
-                if len(default_strategy) == 0:
-                    default_strategy = strategy.ALL_STRATEGY
-                cursor.execute(sql, [site_name, json.dumps(default_strategy)])
-                self.db_conn.commit()    
+        if settings.DATABASES == 'sqlite3':      
+            self.db_path = self.user_home_dir+"/"+self.user_name+"_user.db"                     
+            try:   
+                if os.path.exists(self.db_path): 
+                    self.db_conn  = sqlite3.connect(self.db_path)                   
+                    self.email = self.get_user_email()
+                    self.default_strategy_list = self.get_default_strategy_list()
+                    self.default_watchlist = self.get_default_watchlist()
+                    self.notification_token = self.get_notification_token()
+                else:                                         
+                    if os.path.exists(self.user_home_dir) == False:        
+                        os.mkdir(self.user_home_dir)                    
+                    self.default_strategy_list  = site.get_default_strategy_list()
+                    self.default_watchlist      = site.get_default_watchlist()
+                    self.notification_token     = site.get_default_notification_token()                
+                    self.db_conn  = sqlite3.connect(self.db_path)  
+                    cursor = self.db_conn.cursor()
+                    cursor.execute("CREATE TABLE IF NOT EXISTS user_profile("+schema.user_profile+")")
+                    cursor.execute("CREATE TABLE IF NOT EXISTS account_list("+schema.account_list+")")
+                    #cursor.execute("CREATE TABLE IF NOT EXISTS watchlist("+schema.watchlist+")")                                             
+                    sql = "INSERT INTO user_profile (name, email, default_strategy_list, default_watchlist, notification_token) VALUES (?, ?, ?, ?, ?)"                              
+                    self.email = "askme@outlook.com"
+                    cursor.execute(sql, [user_name, self.email, json.dumps(self.default_strategy_list), json.dumps(self.default_watchlist), self.notification_token])
+                    self.db_conn.commit()                 
             except Exception as e:
-                self.logger.exception(e)    
-        return
+                self.logger.error(e)       
+                raise e
+        else:
+            self.logger.error('Unsupported database engine %s' % settings.DATABASES)
 
     def __enter__(self):
         return self
  
     def __exit__(self, *args):
         try:
             self.db_conn.close()
         except Exception as ex:
             self.logger.exception(ex)
             raise ex
                     
-    def create_user(self, user_name):        
-        if user_name in self.get_user_list():
-            self.logger.error('User %s already exists return existing user' % user_name)
-            return user.user(self, user_name)
-        
-        if app_settings.DATABASES == 'sqlite3':        
-            try:
-                u = user.user(self, user_name)                
-                sql = "INSERT INTO user_list VALUES (?,?)"       
-                cursor = self.db_conn.cursor()
-                cursor.execute(sql, [user_name, u.db_path]) 
-                self.db_conn.commit()
-                return u                
+    # create new account        
+    def get_user_profile(self):
+        if settings.DATABASES == 'sqlite3':                 
+            try:    
+                sql = "SELECT email, default_strategy FROM user_profile"                
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                profile = cursor.fetchone()
+                return profile[0], json.loads(profile[1]) 
             except Exception as e:
-                self.logger.exception(e)   
-                return False
-        else:
-            self.logger.error('Unsupported database engine %s' % app_settings.DATABASES)
-
-    def get_user(self, user_name):        
-        if app_settings.DATABASES == 'sqlite3':        
-            user_list = self.get_user_list()
-            if user_name not in user_list:
-                self.logger.error('User %s not found in this site' % user_name)
-                return None                                                      
+                self.logger.exception(e)
+                raise e
         else:
-            self.logger.error('Unsupported database engine %s' % app_settings.DATABASES)
-
-        return user.user(self, user_name=user_name)    
-        
-    def get_user_list(self):
-        if app_settings.DATABASES == 'sqlite3':                
-            try:
+            self.logger.error("sqlite3 only for now %s")
+        return None, None
+    
+    def get_default_strategy_list(self):
+        if settings.DATABASES == 'sqlite3':                 
+            try:    
+                sql = "SELECT default_strategy_list FROM user_profile"                
                 cursor = self.db_conn.cursor()                    
-                users = [name[0] for name in cursor.execute("SELECT user_name FROM user_list")]
-                return users
+                cursor.execute(sql)
+                return json.loads(cursor.fetchone()[0])                   
             except Exception as e:
-                self.logger.exception(e)   
-                return []
+                self.logger.exception(e)
+                raise e
         else:
-            self.logger.error('Unsupported database engine %s' % app_settings.DATABASES)
-            return []
-        
-    def expand_monitor_list(self, asset_list):
-        if app_settings.DATABASES == 'sqlite3':                 
-            monitor_list = self.get_monitor_list()
-            cursor = self.db_conn.cursor()
-            filter=[]               
-            for symbol in asset_list:
-                if symbol in monitor_list:
-                    continue             
-                #cursor.execute("CREATE TABLE IF NOT EXISTS monitor("+schema.site_monitor_db+")")                                             
-                sql = "INSERT INTO monitor ("+asset.SYMBOL+") VALUES (?)"              
-                try:
-                    cursor.execute(sql, [symbol])
-                    self.db_conn.commit()
-                except Exception as e:                    
-                    self.logger.warning('Add %s failed %s' % (symbol, str(e)))
-                    continue
-                filter.append(symbol)                
+            self.logger.error("sqlite3 only for now %s")
+           
+    def get_default_watchlist(self):
+        if settings.DATABASES == 'sqlite3':                 
+            try:    
+                sql = "SELECT default_watchlist FROM user_profile"                
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                return json.loads(cursor.fetchone()[0])                   
+            except Exception as e:
+                self.logger.exception(e)
+                raise e
         else:
             self.logger.error("sqlite3 only for now %s")
 
-        if len(filter) > 0:
-            self.refresh_site_monitor_list(filter=filter)
+    def get_notification_token(self):
+        if settings.DATABASES == 'sqlite3':                 
+            try:    
+                sql = "SELECT notification_token FROM user_profile"                
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                return cursor.fetchone()[0]                   
+            except Exception as e:
+                self.logger.exception(e)
+                raise e
+        else:
+            self.logger.error("sqlite3 only for now %s")
 
-    def get_default_strategy(self):
-        if app_settings.DATABASES == 'sqlite3':                 
+    def get_user_email(self):
+        if settings.DATABASES == 'sqlite3':                 
             try:    
-                sql = "SELECT default_strategy FROM site_profile"                
+                sql = "SELECT email FROM user_profile"                
                 cursor = self.db_conn.cursor()                    
                 cursor.execute(sql)
-                return json.loads(cursor.fetchone()[0])                
+                return cursor.fetchone()[0]
             except Exception as e:
-                self.logger.exception(e)   
-                return []
+                self.logger.exception(e)
+                raise e
         else:
             self.logger.error("sqlite3 only for now %s")
-           
-    def update_default_strategy(self, default_strategy):
-        if len(default_strategy) == 0:
-            return
-        
-        if app_settings.DATABASES == 'sqlite3':                 
+
+    def update_default_strategy_list(self, strategy_list):
+        if len(strategy_list) == 0:
+            self.logger.error('Cannot set empty default strategy list')
+            return [] 
+              
+        if settings.DATABASES == 'sqlite3':                 
             try:                              
-                sql = "UPDATE site_profile SET default_strategy='"+json.dumps(default_strategy)+"' WHERE site_name='"+self.site_name+"'"                    
+                sql = "UPDATE user_profile SET default_strategy_lisst='"+json.dumps(strategy_list)+"' WHERE name='"+self.user_name+"'"                    
                 cursor = self.db_conn.cursor()                    
                 cursor.execute(sql)
                 self.db_conn.commit()                 
+                self.default_strategy_list = strategy_list
             except Exception as e:
-                self.logger.exception(e)   
+                self.logger.exception(e)
                 return []
         else:
             self.logger.error("sqlite3 only for now %s")
 
-    def get_monitor_list(self):
-        if app_settings.DATABASES == 'sqlite3':                 
-            try:    
+    def update_default_watchlist(self, watchlist):
+            
+        if len(watchlist) == 0:
+            self.logger.error('Cannot set empty default watchlist!')
+            return []
+        
+        if settings.DATABASES == 'sqlite3':                 
+            try:                              
+                sql = "UPDATE user_profile SET default_watchlist='"+json.dumps(watchlist)+"' WHERE name='"+self.user_name+"'"                    
                 cursor = self.db_conn.cursor()                    
-                symbols = [symbol[0] for symbol in cursor.execute("SELECT "+asset.SYMBOL+ " FROM monitor")]
-                return symbols
+                cursor.execute(sql)
+                self.db_conn.commit()
+                self.default_watchlist = watchlist         
+                return watchlist        
             except Exception as e:
-                self.logger.exception(e)   
-                return []
+                self.logger.exception(e)
+                raise e
         else:
             self.logger.error("sqlite3 only for now %s")
 
-    def get_monitor_df(self, filter=[]):
-        if app_settings.DATABASES == 'sqlite3':                 
-            try:    
-                import pandas as pd                
-                df = pd.read_sql_query("SELECT * FROM monitor", self.db_conn)                           
-                df = df[df[asset.SYMBOL].isin(filter)] if len(filter)>0 else df           
-                #df[asset.IV1] = pd.to_numeric(df[asset.IV1], errors='coerce')
-                #df[asset.HV] = pd.to_numeric(df[asset.HV], errors='coerce')
-                return df
+    def update_notification_token(self, token):
+            
+        if len(token) != len(app_settings.LINE_NOTIFICATION_TOKEN):
+            self.logger.error('Invalid notification token %s' %token)
+
+        if settings.DATABASES == 'sqlite3':                 
+            try:                              
+                sql = "UPDATE user_profile SET default_strategy='"+token+"' WHERE name='"+self.user_name+"'"                    
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                self.db_conn.commit()         
+                self.notification_token = token
+                return token        
             except Exception as e:
-                self.logger.exception(e)   
-                return []
+                self.logger.exception(e)
+                raise e
         else:
             self.logger.error("sqlite3 only for now %s")
+            return ''
 
-    def refresh_site_monitor_list(self, filter=[]):    
-        if app_settings.DATABASES == 'sqlite3':                 
-            try:
-                import pandas as pd                
-                df = pd.read_sql_query("SELECT * FROM monitor", self.db_conn)                          
-                refresh_monitor_list(df, filter=filter)                
-                df.to_sql('monitor', self.db_conn, if_exists='replace', index=False, schema=schema.site_monitor_db)
-                self.db_conn.commit()                
-                return df
-            except Exception as e:
-                self.logger.exception(e)   
-                raise e
-                #return []
+    def update_user_email(self, email):
+
+        if len(email) == 0:
+            return    
+            
+        if settings.DATABASES == 'sqlite3':                 
+            try:                              
+                sql = "UPDATE user_profile SET email='"+email+"' WHERE name='"+self.user_name+"'"                    
+                cursor = self.db_conn.cursor()                    
+                cursor.execute(sql)
+                self.db_conn.commit()                 
+            except Exception as e:
+                self.logger.exception(e)
+                raise e
         else:
             self.logger.error("sqlite3 only for now %s")
+                
+    def create_account(self, account_name, initial_balance=app_settings.DEFAULT_ACCOUNT_INITIAL_BALANCE):       
+        if settings.DATABASES == 'sqlite3':                
+            try:
+                account_list = self.get_account_list()
+                if account_name in account_list:
+                    self.logger.error('Account %s alreadt exist return existing one' % account_name)
+                    return account(self, account_name)
+                
+                a = account(self, account_name, initial_balance=initial_balance)             
+                sql = "INSERT INTO account_list VALUES (?,?)"       
+                cursor = self.db_conn.cursor()
+                cursor.execute(sql, [account_name, a.db_path]) 
+                self.db_conn.commit()
+                return a
+            except Exception as e:
+                self.logger.exception(e)
+                raise e     
 
-    def select_high_IV_HV_ratio_asset(self, ratio, filter=[]):
-        df = self.get_monitor_df(filter=filter)
-        df[asset.IV1] = pd.to_numeric(df[asset.IV1], errors='coerce')
-        df[asset.HV] = pd.to_numeric(df[asset.HV], errors='coerce')
-        dd = df[df[asset.IV1]/df[asset.HV] >= ratio]
-        return dd[asset.SYMBOL].to_list()  
-
-    def select_low_IV_HV_ratio_asset(self, ratio, filter=[]):
-        df = self.get_monitor_df(filter=filter)
-        df[asset.IV1] = pd.to_numeric(df[asset.IV1], errors='coerce')
-        df[asset.HV] = pd.to_numeric(df[asset.HV], errors='coerce')
-        dd = df[df[asset.IV1]/df[asset.HV] <= ratio]
-        return dd[asset.SYMBOL].to_list()  
+    def get_account_list(self):
+        if settings.DATABASES == 'sqlite3':                
+            try:
+                cursor = self.db_conn.cursor()                    
+                account_name_list = [account_name[0] for account_name in cursor.execute("SELECT account_name FROM account_list")]
+                return account_name_list
+            except Exception as e:
+                self.logger.exception(e)
+                raise e
+        else:
+            self.logger.error('Unsupported database engine %s' % settings.DATABASES)
+
+    def get_account(self, account_name):
+        return account(self.user_name, account_name)
     
 
-        
+if __name__ == '__main__':
 
+    from option_trader.admin import user as u              
+    me = u.user('jihuang')
+    me.update_account('condor')
+    #me.update_account('spread')
```

### Comparing `option_trader-0.2.3/option_trader/admin/transaction.py` & `option_trader-0.2.4/option_trader/admin/transaction.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/option/butterfly.py` & `option_trader-0.2.4/option_trader/backtest/option/butterfly.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/option/credit_iron_condor.py` & `option_trader-0.2.4/option_trader/backtest/option/credit_iron_condor.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/option/single_option.py` & `option_trader-0.2.4/option_trader/backtest/option/single_option.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/option/spread.py` & `option_trader-0.2.4/option_trader/backtest/option/spread.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/option/strategy.py` & `option_trader-0.2.4/option_trader/backtest/option/strategy.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/stock/bollingerBands.py` & `option_trader-0.2.4/option_trader/backtest/stock/bollingerBands.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/stock/macd.py` & `option_trader-0.2.4/option_trader/backtest/stock/macd.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/stock/mfi.py` & `option_trader-0.2.4/option_trader/backtest/stock/mfi.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/backtest/stock/rsi.py` & `option_trader-0.2.4/option_trader/backtest/stock/rsi.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/consts/asset.py` & `option_trader-0.2.4/option_trader/consts/asset.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/consts/strategy.py` & `option_trader-0.2.4/option_trader/consts/strategy.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/jobs/account.py` & `option_trader-0.2.4/option_trader/jobs/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 
-import sys
-
-sys.path.append(r'/Users/jimhu/option_trader/src')
-    
-
 from option_trader.jobs import core
 from option_trader.admin.site    import site
 from option_trader.admin.user    import user
 from option_trader.admin.account import account
 
 from option_trader.utils.data_getter import afterHours
 
@@ -57,15 +52,14 @@
         with site(self.site_name) as mysite:
             with user(user_name=self.user_name, site=mysite) as this_user:
                 with account(this_user, self.account_name) as this_account:
                     this_account.try_open_new_strategy_positions()
                                         
         return
 
-
 if __name__ == '__main__':
     
     from logging.handlers import RotatingFileHandler
     
     FORMAT = '%(asctime)s-%(levelname)s (%(message)s) %(filename)s-%(lineno)s-%(funcName)s'
         
     ch = logging.StreamHandler()    
@@ -95,29 +89,29 @@
     logging.getLogger('yfinance').setLevel(logging.WARN)
 
 
     #logger.debug('processing single')
     #t =  trade('mysite', 'jihuang', 'single')
     #t.execute()
 
-    #print('processing spread')    
-    #t=  trade('mysite', 'jihuang', 'spread')
-    #t.execute()
+    print('trade spread')    
+    t=  trade('mysite', 'jihuang', 'spread')
+    t.execute()
 
     #print('processing iron_condor')
     #t =  trade('mysite', 'jihuang', 'iron_condor')
     #t.execute()
 
     #print('processing butterfly')
     #t =  trade('mysite', 'jihuang', 'butterfly')
     #t.execute()
 
-    print('processing butterfly')
-    t =  update_position('mysite', 'jihuang', 'butterfly')
-    t.execute()
+    #print('update butterfly')
+    #t =  update_position('mysite', 'jihuang', 'butterfly')
+    #t.execute()
 
 
     #print('processing single')
     #t =  update_position('mysite', 'jihuang', 'single')
     #t.execute()
 
     #print('processing spread')
```

### Comparing `option_trader-0.2.3/option_trader/jobs/site.py` & `option_trader-0.2.4/option_trader/jobs/site.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/Ananlyzer.ipynb` & `option_trader-0.2.4/notebook/Ananlyzer.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/ML_TensorFlow_good.ipynb` & `option_trader-0.2.4/notebook/ML_TensorFlow_good.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/ML_ochl.ipynb` & `option_trader-0.2.4/notebook/ML_ochl.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/MP_TensorFlow_bad.ipynb` & `option_trader-0.2.4/notebook/MP_TensorFlow_bad.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/ib.ipynb` & `option_trader-0.2.4/notebook/ib.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/ml.ipynb` & `option_trader-0.2.4/notebook/ml.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/option_geeks.ipynb` & `option_trader-0.2.4/notebook/option_geeks.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/option_tools.ipynb` & `option_trader-0.2.4/notebook/option_tools.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/watchlist.ipynb` & `option_trader-0.2.4/notebook/watchlist.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/Ananlyzer-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/ML_TensorFlow_good-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/ML_ochl-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/MP_TensorFlow_bad-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/admin-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/ib-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/ml-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/option_geeks-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/option_tools-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb` & `option_trader-0.2.4/notebook/.ipynb_checkpoints/watchlist-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/settings/log_config.py` & `option_trader-0.2.4/option_trader/settings/log_config.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/settings/logging.conf` & `option_trader-0.2.4/option_trader/settings/logging.conf`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/settings/schema.py` & `option_trader-0.2.4/option_trader/settings/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 
 # site.db
-site_profile = "site_name TEXT NOT NULL PRIMARY KEY, region TEXT, default_strategy TEXT"
+site_profile = "site_name TEXT NOT NULL PRIMARY KEY, region TEXT, default_strategy_list TEXT, default_watchlist TEXT, default_notification_token TEXT"
 
 site_monitor_db = "symbol TEXT NOT NULL PRIMARY KEY, last_price REAL, support REAL, resistence REAL,\
     rating REAL, trend TEXT, slope REAL, bb_pos TEXT, bb_link TEXT, rsi TEXT, rsi_link TEXT,\
     macd TEXT, macd_link TEXT, mfi TEXT, mfi_link TEXT, earning TEXT, day_range_pos REAL,\
     fifty_weeks_range_pos REAL, volume_range_pos REAL, forward_PE REAL, HV REAL,\
     IV1 REAL, delta1 REAL,IV2 REAL, delta2 REAL,IV3 REAL, delta3 REAL,IV4 REAL, delta4 REAL,\
     quote_time TEXT"
 
 user_list = "user_name TEXT NOT NULL PRIMARY KEY, db_path TEXT NOT NULL"
 
 # user.db
-user_profile = "name TEXT NOT NULL PRIMARY KEY, email TEXT, default_strategy TEXT, billing TEXT"
-watchlist   = "name TEXT NOT NULL PRIMARY KEY, symbol_list TEXT"
+user_profile = "name TEXT NOT NULL PRIMARY KEY, email TEXT, default_strategy_list TEXT, default_watchlist TEXT, notification_token TEXT,  billing TEXT"
+
+#watchlist   =  "name TEXT NOT NULL PRIMARY KEY, symbol_list TEXT"
+
 account_list = "account_name TEXT NOT NULL PRIMARY KEY, db_path TEXT NOT NULL"
 
 '''
 # account.db
-account_profile = "user_name TEXT, account_name TEXT NOT NULL PRIMARY KEY,equaty_percentage REAL,\
+account_profile_schema = "user_name TEXT, account_name TEXT NOT NULL PRIMARY KEY,equaty_percentage REAL,\
         available_to_tread REAL,available_to_trade_wo_margin REAL,non_margin_buy_power REAL,\
         margin_buy_power REAL,available_to_withdraw REAL,cash_only REAL,cash_and_margin REAL,\
         house_surplus REAL,sma REAL,exchange_surplue REAL,cash_core REAL,cash_credit_debit REAL,\
         margin_credit_debit REA,market_value_securities REAL,held_in_cash REAL, held_in_margin REAL,\
         cash_buy_power REAL,settled_cash REAL,initial_balance REAL,risk_mgr TEXT, entry_crit TEXT,\
-        market_condition TEXT, runtime_config TEXT,default_strategy TEXT, default_predictor TEXT,\
-        FOREIGN KEY(user_name) REFERENCES user(name)"   
+        market_condition TEXT, runtime_config TEXT,default_strategy_list TEXT, default_watchlist TEXT, default_predictor TEXT,\
+        FOREIGN KEY(user_name) REFERENCES user(name)"    
 
 
 positionSummary = "symbol TEXT,strategy TEXT,status TEXT,\
         spread REAL, open_price REAL,breakeven_l REAL, breakeven_h REAL,\
         max_prifit REAL, max_loss REAL,pnl REAL,win_prob REAL,\
         trade_date REAL,earning_date TRXT,trade_stock_price REAL,\
         margin REAL,quantity REAL,option_legs TEXT,\
```

### Comparing `option_trader-0.2.3/option_trader/settings/trade_config.py` & `option_trader-0.2.4/option_trader/settings/trade_config.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/shell/analyzer.py` & `option_trader-0.2.4/option_trader/shell/analyzer.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/shell/backtester.py` & `option_trader-0.2.4/option_trader/shell/backtester.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/shell/dataset_tool.py` & `option_trader-0.2.4/option_trader/shell/dataset_tool.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/shell/line.py` & `option_trader-0.2.4/option_trader/shell/line.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/utils/calc_prob.py` & `option_trader-0.2.4/option_trader/utils/calc_prob.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/utils/data_getter.py` & `option_trader-0.2.4/option_trader/utils/data_getter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1174,18 +1174,14 @@
             max_loss = price            
             breakeven_h =  strike-price
             breakeven_l =  np.nan
             win_prob = calc_prob_lower_than(predList, breakeven_h)
 
     pnl = max_profit / max_loss
 
-    #max_profit = price if credit else np.nan
-
-    #max_loss =   np.nan if credit else price
-
     dt[option_summary.SYMBOL]            = [symbol]
     dt[option_summary.EXP_DATE]          = [exp_date]
     dt[option_summary.OPEN_PRICE]        = [price]
     dt[option_summary.PNL]               = [pnl]
     dt[option_summary.WIN_PROB]          = [win_prob]
     dt[option_summary.MAX_LOSS]          = [max_loss]
     dt[option_summary.MAX_PROFIT]        = [max_profit]
```

### Comparing `option_trader-0.2.3/option_trader/utils/data_getter_ib.py` & `option_trader-0.2.4/option_trader/utils/data_getter_ib.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/utils/line_norify.py` & `option_trader-0.2.4/option_trader/utils/line_norify.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+#https://respond.io/blog/line-notification
+
 import requests
 
 import logging
 
 from option_trader.settings import app_settings    
 
 
-def lineNotifyMessage(msg, token=app_settings.LINE_NOTIFICATION_TOKEN):
+#def lineNotifyMessage(msg, token=app_settings.LINE_NOTIFICATION_TOKEN):
+def lineNotifyMessage(msg, token=app_settings.DEFAULT_SITE_NOTIFICATION_TOKEN):
 
     headers = {
         "Authorization": "Bearer " + token, 
         "Content-Type" : "application/x-www-form-urlencoded"
     }
 
     payload = {'message': msg }
+    
     r = requests.post("https://notify-api.line.me/api/notify", headers = headers, params = payload)
     return r.status_code
 
 
 if __name__ == "__main__":
 
   #'Df0tC09dtPoshq3psJaeen3ubXXH5e94u74FezQEalb'
```

### Comparing `option_trader-0.2.3/option_trader/utils/monitor.py` & `option_trader-0.2.4/option_trader/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/utils/option_tool.py` & `option_trader-0.2.4/option_trader/utils/option_tool.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/option_trader/utils/predictor.py` & `option_trader-0.2.4/option_trader/utils/predictor.py`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/LICENSE` & `option_trader-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `option_trader-0.2.3/pyproject.toml` & `option_trader-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "option_trader"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Jim Huang", email="jim.huang.taipei@outlook.com" },
 ]
 description = "Option Trading Robot package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

