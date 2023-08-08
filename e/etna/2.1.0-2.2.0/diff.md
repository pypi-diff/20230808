# Comparing `tmp/etna-2.1.0.tar.gz` & `tmp/etna-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etna-2.1.0.tar", max compression
+gzip compressed data, was "etna-2.2.0.tar", max compression
```

## Comparing `etna-2.1.0.tar` & `etna-2.2.0.tar`

### file list

```diff
@@ -1,204 +1,215 @@
--rw-r--r--   0        0        0    11244 2023-07-03 15:27:34.976775 etna-2.1.0/LICENSE
--rw-r--r--   0        0        0    13778 2023-07-03 15:27:34.976775 etna-2.1.0/README.md
--rw-r--r--   0        0        0       49 2023-07-03 15:27:34.980775 etna-2.1.0/etna/__init__.py
--rw-r--r--   0        0        0     2388 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/__init__.py
--rw-r--r--   0        0        0      599 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/__init__.py
--rw-r--r--   0        0        0    16581 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/plots.py
--rw-r--r--   0        0        0     1189 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/search.py
--rw-r--r--   0        0        0     9835 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/utils.py
--rw-r--r--   0        0        0      475 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/eda/__init__.py
--rw-r--r--   0        0        0    26025 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/eda/plots.py
--rw-r--r--   0        0        0     4113 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/eda/utils.py
--rw-r--r--   0        0        0      472 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/__init__.py
--rw-r--r--   0        0        0     6004 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/plots.py
--rw-r--r--   0        0        0     3114 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/relevance.py
--rw-r--r--   0        0        0     4116 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/relevance_table.py
--rw-r--r--   0        0        0      654 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/utils.py
--rw-r--r--   0        0        0      213 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_selection/__init__.py
--rw-r--r--   0        0        0     5023 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_selection/mrmr_selection.py
--rw-r--r--   0        0        0      737 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/forecast/__init__.py
--rw-r--r--   0        0        0    35626 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/forecast/plots.py
--rw-r--r--   0        0        0     4142 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/forecast/utils.py
--rw-r--r--   0        0        0      517 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/__init__.py
--rw-r--r--   0        0        0     4879 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/density_outliers.py
--rw-r--r--   0        0        0    13169 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/hist_outliers.py
--rw-r--r--   0        0        0     1739 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/median_outliers.py
--rw-r--r--   0        0        0     5343 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/plots.py
--rw-r--r--   0        0        0     3878 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/prediction_interval_outliers.py
--rw-r--r--   0        0        0     1471 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/utils.py
--rw-r--r--   0        0        0       96 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/__init__.py
--rw-r--r--   0        0        0    31738 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/auto.py
--rw-r--r--   0        0        0      102 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/optuna/__init__.py
--rw-r--r--   0        0        0     4737 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/optuna/config_sampler.py
--rw-r--r--   0        0        0     2828 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/optuna/wrapper.py
--rw-r--r--   0        0        0       93 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/__init__.py
--rw-r--r--   0        0        0     1533 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/generator.py
--rw-r--r--   0        0        0     5348 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/templates.py
--rw-r--r--   0        0        0      495 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/utils.py
--rw-r--r--   0        0        0      151 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/__init__.py
--rw-r--r--   0        0        0      451 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/base.py
--rw-r--r--   0        0        0     2114 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/local.py
--rw-r--r--   0        0        0      171 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/utils.py
--rw-r--r--   0        0        0     1664 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/utils.py
--rw-r--r--   0        0        0      524 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/__init__.py
--rw-r--r--   0        0        0      686 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/base.py
--rw-r--r--   0        0        0      259 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/__init__.py
--rw-r--r--   0        0        0     3756 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/base.py
--rw-r--r--   0        0        0     4508 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/distance_matrix.py
--rw-r--r--   0        0        0     5597 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/dtw_distance.py
--rw-r--r--   0        0        0     1705 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/euclidean_distance.py
--rw-r--r--   0        0        0      289 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/__init__.py
--rw-r--r--   0        0        0     6025 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/base.py
--rw-r--r--   0        0        0     1501 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/dtw_clustering.py
--rw-r--r--   0        0        0     1561 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/euclidean_clustering.py
--rw-r--r--   0        0        0      374 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/__init__.py
--rw-r--r--   0        0        0      197 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/__main__.py
--rw-r--r--   0        0        0     4832 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/backtest_command.py
--rw-r--r--   0        0        0     6885 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/forecast_command.py
--rw-r--r--   0        0        0      281 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/resolvers.py
--rw-r--r--   0        0        0     4415 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/utils.py
--rw-r--r--   0        0        0      205 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/__init__.py
--rw-r--r--   0        0        0    11102 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/mixins.py
--rw-r--r--   0        0        0      631 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/saving.py
--rw-r--r--   0        0        0     2248 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/utils.py
--rw-r--r--   0        0        0      548 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/__init__.py
--rw-r--r--   0        0        0     8274 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/datasets_generation.py
--rw-r--r--   0        0        0     7778 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/hierarchical_structure.py
--rw-r--r--   0        0        0    62951 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/tsdataset.py
--rw-r--r--   0        0        0    10283 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/utils.py
--rw-r--r--   0        0        0      255 2023-07-03 15:27:34.984775 etna-2.1.0/etna/distributions/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-03 15:27:34.984775 etna-2.1.0/etna/distributions/distributions.py
--rw-r--r--   0        0        0      226 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/__init__.py
--rw-r--r--   0        0        0     6579 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/direct_ensemble.py
--rw-r--r--   0        0        0     4684 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/mixins.py
--rw-r--r--   0        0        0    11343 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/stacking_ensemble.py
--rw-r--r--   0        0        0     9819 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/voting_ensemble.py
--rw-r--r--   0        0        0       94 2023-07-03 15:27:34.984775 etna-2.1.0/etna/experimental/change_points/__init__.py
--rw-r--r--   0        0        0     5558 2023-07-03 15:27:34.984775 etna-2.1.0/etna/experimental/change_points/regularization_search.py
--rw-r--r--   0        0        0      242 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/__init__.py
--rw-r--r--   0        0        0      473 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/base.py
--rw-r--r--   0        0        0     4926 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/classification.py
--rw-r--r--   0        0        0      366 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/__init__.py
--rw-r--r--   0        0        0     1543 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/base.py
--rw-r--r--   0        0        0     2510 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/tsfresh.py
--rw-r--r--   0        0        0    15250 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/weasel.py
--rw-r--r--   0        0        0     3241 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/predictability.py
--rw-r--r--   0        0        0      874 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/utils.py
--rw-r--r--   0        0        0        0 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/__init__.py
--rw-r--r--   0        0        0       79 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pmdarima_utils/__init__.py
--rw-r--r--   0        0        0     7455 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pmdarima_utils/arima.py
--rw-r--r--   0        0        0      415 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pmdarima_utils/arima.pyi
--rw-r--r--   0        0        0        0 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      472 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pytorch_lightning/callbacks.py
--rw-r--r--   0        0        0      341 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/__init__.py
--rw-r--r--   0        0        0     1840 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/defaults.py
--rw-r--r--   0        0        0     1801 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/distribution.py
--rw-r--r--   0        0        0       69 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/distribution.pyi
--rw-r--r--   0        0        0    16549 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/relevance.py
--rw-r--r--   0        0        0      823 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/relevance.pyi
--rw-r--r--   0        0        0     8470 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/significance_tests.py
--rw-r--r--   0        0        0      344 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/significance_tests.pyi
--rw-r--r--   0        0        0      804 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/__init__.py
--rw-r--r--   0        0        0     4993 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/base.py
--rw-r--r--   0        0        0     2643 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/console_logger.py
--rw-r--r--   0        0        0    15309 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/file_logger.py
--rw-r--r--   0        0        0     7105 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/wandb_logger.py
--rw-r--r--   0        0        0     1230 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/__init__.py
--rw-r--r--   0        0        0     7625 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/base.py
--rw-r--r--   0        0        0     5151 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/functional_metrics.py
--rw-r--r--   0        0        0     5513 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/intervals_metrics.py
--rw-r--r--   0        0        0     9643 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/metrics.py
--rw-r--r--   0        0        0     2539 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/utils.py
--rw-r--r--   0        0        0     1729 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/__init__.py
--rw-r--r--   0        0        0     2521 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/autoarima.py
--rw-r--r--   0        0        0    23070 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/base.py
--rw-r--r--   0        0        0    16331 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/catboost.py
--rw-r--r--   0        0        0    14394 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/deadline_ma.py
--rw-r--r--   0        0        0      557 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/decorators.py
--rw-r--r--   0        0        0    33314 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/holt_winters.py
--rw-r--r--   0        0        0     8556 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/linear.py
--rw-r--r--   0        0        0    22835 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/mixins.py
--rw-r--r--   0        0        0      828 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/moving_average.py
--rw-r--r--   0        0        0     1031 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/naive.py
--rw-r--r--   0        0        0      373 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/__init__.py
--rw-r--r--   0        0        0     9896 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepar.py
--rw-r--r--   0        0        0      561 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/__init__.py
--rw-r--r--   0        0        0    12488 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/deepstate.py
--rw-r--r--   0        0        0     8808 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/linear_dynamic_system.py
--rw-r--r--   0        0        0    12191 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/state_space_model.py
--rw-r--r--   0        0        0     9163 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/mlp.py
--rw-r--r--   0        0        0    11237 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/rnn.py
--rw-r--r--   0        0        0    11486 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/tft.py
--rw-r--r--   0        0        0    12626 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/utils.py
--rw-r--r--   0        0        0    19903 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/prophet.py
--rw-r--r--   0        0        0    33250 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/sarimax.py
--rw-r--r--   0        0        0     8942 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/seasonal_ma.py
--rw-r--r--   0        0        0     3555 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/sklearn.py
--rw-r--r--   0        0        0    19716 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/tbats.py
--rw-r--r--   0        0        0     3685 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/utils.py
--rw-r--r--   0        0        0      292 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/__init__.py
--rw-r--r--   0        0        0     5437 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/assembling_pipelines.py
--rw-r--r--   0        0        0     7334 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/autoregressive_pipeline.py
--rw-r--r--   0        0        0    39081 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/base.py
--rw-r--r--   0        0        0    14000 2023-07-03 15:27:34.992775 etna-2.1.0/etna/pipeline/hierarchical_pipeline.py
--rw-r--r--   0        0        0     8460 2023-07-03 15:27:34.992775 etna-2.1.0/etna/pipeline/mixins.py
--rw-r--r--   0        0        0     5563 2023-07-03 15:27:34.992775 etna-2.1.0/etna/pipeline/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-03 15:27:34.992775 etna-2.1.0/etna/py.typed
--rw-r--r--   0        0        0      181 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/__init__.py
--rw-r--r--   0        0        0     3551 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/base.py
--rw-r--r--   0        0        0     1899 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/bottom_up.py
--rw-r--r--   0        0        0     5742 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/top_down.py
--rw-r--r--   0        0        0    10540 2023-07-03 15:27:34.992775 etna-2.1.0/etna/settings.py
--rw-r--r--   0        0        0     3286 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/__init__.py
--rw-r--r--   0        0        0    12781 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/base.py
--rw-r--r--   0        0        0     1168 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/__init__.py
--rw-r--r--   0        0        0      949 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/__init__.py
--rw-r--r--   0        0        0     7980 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/base.py
--rw-r--r--   0        0        0      250 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
--rw-r--r--   0        0        0     1886 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
--rw-r--r--   0        0        0     2171 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
--rw-r--r--   0        0        0     5666 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/detrend.py
--rw-r--r--   0        0        0     5168 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/level.py
--rw-r--r--   0        0        0      887 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
--rw-r--r--   0        0        0      732 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
--rw-r--r--   0        0        0     1311 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
--rw-r--r--   0        0        0     3397 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
--rw-r--r--   0        0        0     2496 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
--rw-r--r--   0        0        0     5478 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/segmentation.py
--rw-r--r--   0        0        0     5798 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/trend.py
--rw-r--r--   0        0        0     8552 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/detrend.py
--rw-r--r--   0        0        0     8239 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/stl.py
--rw-r--r--   0        0        0      306 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/__init__.py
--rw-r--r--   0        0        0     7512 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/categorical.py
--rw-r--r--   0        0        0     2836 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/mean_segment_encoder.py
--rw-r--r--   0        0        0     2525 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/segment_encoder.py
--rw-r--r--   0        0        0      444 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/__init__.py
--rw-r--r--   0        0        0     2469 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/base.py
--rw-r--r--   0        0        0    10158 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/feature_importance.py
--rw-r--r--   0        0        0     3434 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/filter.py
--rw-r--r--   0        0        0    14975 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/gale_shapley.py
--rw-r--r--   0        0        0     1383 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/__init__.py
--rw-r--r--   0        0        0     4821 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/add_constant.py
--rw-r--r--   0        0        0     5645 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/apply_lambda.py
--rw-r--r--   0        0        0    17152 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/differencing.py
--rw-r--r--   0        0        0     9987 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/lags.py
--rw-r--r--   0        0        0     5002 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/log.py
--rw-r--r--   0        0        0     4469 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/power.py
--rw-r--r--   0        0        0    10377 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/scalers.py
--rw-r--r--   0        0        0    11846 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/sklearn.py
--rw-r--r--   0        0        0    22772 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/statistics.py
--rw-r--r--   0        0        0      233 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/missing_values/__init__.py
--rw-r--r--   0        0        0     9573 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/missing_values/imputation.py
--rw-r--r--   0        0        0     6693 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/missing_values/resample.py
--rw-r--r--   0        0        0      301 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/outliers/__init__.py
--rw-r--r--   0        0        0     5106 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/outliers/base.py
--rw-r--r--   0        0        0     7988 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/outliers/point_outliers.py
--rw-r--r--   0        0        0      334 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/__init__.py
--rw-r--r--   0        0        0    15747 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/date_flags.py
--rw-r--r--   0        0        0     5802 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/fourier.py
--rw-r--r--   0        0        0     2848 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/holiday.py
--rw-r--r--   0        0        0     9079 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/special_days.py
--rw-r--r--   0        0        0     9478 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/time_flags.py
--rw-r--r--   0        0        0      746 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/utils.py
--rw-r--r--   0        0        0    11985 2023-07-03 15:27:35.228776 etna-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    19330 1970-01-01 00:00:00.000000 etna-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11244 2023-08-08 14:58:05.903255 etna-2.2.0/LICENSE
+-rw-r--r--   0        0        0    14786 2023-08-08 14:58:05.903255 etna-2.2.0/README.md
+-rw-r--r--   0        0        0       49 2023-08-08 14:58:05.907255 etna-2.2.0/etna/__init__.py
+-rw-r--r--   0        0        0     2388 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/__init__.py
+-rw-r--r--   0        0        0      599 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/decomposition/__init__.py
+-rw-r--r--   0        0        0    16581 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/decomposition/plots.py
+-rw-r--r--   0        0        0     1189 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/decomposition/search.py
+-rw-r--r--   0        0        0     9835 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/decomposition/utils.py
+-rw-r--r--   0        0        0      475 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/eda/__init__.py
+-rw-r--r--   0        0        0    26025 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/eda/plots.py
+-rw-r--r--   0        0        0     4113 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/eda/utils.py
+-rw-r--r--   0        0        0      472 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/feature_relevance/__init__.py
+-rw-r--r--   0        0        0     6004 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/feature_relevance/plots.py
+-rw-r--r--   0        0        0     3114 2023-08-08 14:58:05.907255 etna-2.2.0/etna/analysis/feature_relevance/relevance.py
+-rw-r--r--   0        0        0     4117 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/feature_relevance/relevance_table.py
+-rw-r--r--   0        0        0      654 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/feature_relevance/utils.py
+-rw-r--r--   0        0        0      213 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/feature_selection/__init__.py
+-rw-r--r--   0        0        0     5270 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/feature_selection/mrmr_selection.py
+-rw-r--r--   0        0        0      737 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/forecast/__init__.py
+-rw-r--r--   0        0        0    35626 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/forecast/plots.py
+-rw-r--r--   0        0        0     4142 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/forecast/utils.py
+-rw-r--r--   0        0        0      517 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/outliers/__init__.py
+-rw-r--r--   0        0        0     4879 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/outliers/density_outliers.py
+-rw-r--r--   0        0        0    13169 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/outliers/hist_outliers.py
+-rw-r--r--   0        0        0     1739 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/outliers/median_outliers.py
+-rw-r--r--   0        0        0     5343 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/outliers/plots.py
+-rw-r--r--   0        0        0     3878 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/outliers/prediction_interval_outliers.py
+-rw-r--r--   0        0        0     1471 2023-08-08 14:58:05.911255 etna-2.2.0/etna/analysis/utils.py
+-rw-r--r--   0        0        0       96 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/__init__.py
+-rw-r--r--   0        0        0    31738 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/auto.py
+-rw-r--r--   0        0        0      102 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/optuna/__init__.py
+-rw-r--r--   0        0        0     4737 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/optuna/config_sampler.py
+-rw-r--r--   0        0        0     2828 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/optuna/wrapper.py
+-rw-r--r--   0        0        0       93 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/pool/__init__.py
+-rw-r--r--   0        0        0     1533 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/pool/generator.py
+-rw-r--r--   0        0        0     5348 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/pool/templates.py
+-rw-r--r--   0        0        0      495 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/pool/utils.py
+-rw-r--r--   0        0        0      151 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/runner/__init__.py
+-rw-r--r--   0        0        0      451 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/runner/base.py
+-rw-r--r--   0        0        0     2229 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/runner/local.py
+-rw-r--r--   0        0        0      171 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/runner/utils.py
+-rw-r--r--   0        0        0     1664 2023-08-08 14:58:05.911255 etna-2.2.0/etna/auto/utils.py
+-rw-r--r--   0        0        0      524 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/__init__.py
+-rw-r--r--   0        0        0      686 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/base.py
+-rw-r--r--   0        0        0      259 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/distances/__init__.py
+-rw-r--r--   0        0        0     3756 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/distances/base.py
+-rw-r--r--   0        0        0     4508 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/distances/distance_matrix.py
+-rw-r--r--   0        0        0     5597 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/distances/dtw_distance.py
+-rw-r--r--   0        0        0     1705 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/distances/euclidean_distance.py
+-rw-r--r--   0        0        0      289 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/hierarchical/__init__.py
+-rw-r--r--   0        0        0     6025 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/hierarchical/base.py
+-rw-r--r--   0        0        0     1501 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/hierarchical/dtw_clustering.py
+-rw-r--r--   0        0        0     1561 2023-08-08 14:58:05.911255 etna-2.2.0/etna/clustering/hierarchical/euclidean_clustering.py
+-rw-r--r--   0        0        0      374 2023-08-08 14:58:05.911255 etna-2.2.0/etna/commands/__init__.py
+-rw-r--r--   0        0        0      197 2023-08-08 14:58:05.911255 etna-2.2.0/etna/commands/__main__.py
+-rw-r--r--   0        0        0     4832 2023-08-08 14:58:05.911255 etna-2.2.0/etna/commands/backtest_command.py
+-rw-r--r--   0        0        0     7266 2023-08-08 14:58:05.911255 etna-2.2.0/etna/commands/forecast_command.py
+-rw-r--r--   0        0        0      281 2023-08-08 14:58:05.911255 etna-2.2.0/etna/commands/resolvers.py
+-rw-r--r--   0        0        0     4415 2023-08-08 14:58:05.911255 etna-2.2.0/etna/commands/utils.py
+-rw-r--r--   0        0        0      205 2023-08-08 14:58:05.911255 etna-2.2.0/etna/core/__init__.py
+-rw-r--r--   0        0        0    11432 2023-08-08 14:58:05.911255 etna-2.2.0/etna/core/mixins.py
+-rw-r--r--   0        0        0      631 2023-08-08 14:58:05.911255 etna-2.2.0/etna/core/saving.py
+-rw-r--r--   0        0        0     2540 2023-08-08 14:58:05.911255 etna-2.2.0/etna/core/utils.py
+-rw-r--r--   0        0        0      548 2023-08-08 14:58:05.911255 etna-2.2.0/etna/datasets/__init__.py
+-rw-r--r--   0        0        0     8274 2023-08-08 14:58:05.911255 etna-2.2.0/etna/datasets/datasets_generation.py
+-rw-r--r--   0        0        0     7778 2023-08-08 14:58:05.911255 etna-2.2.0/etna/datasets/hierarchical_structure.py
+-rw-r--r--   0        0        0    63453 2023-08-08 14:58:05.911255 etna-2.2.0/etna/datasets/tsdataset.py
+-rw-r--r--   0        0        0    10283 2023-08-08 14:58:05.911255 etna-2.2.0/etna/datasets/utils.py
+-rw-r--r--   0        0        0      255 2023-08-08 14:58:05.911255 etna-2.2.0/etna/distributions/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-08 14:58:05.911255 etna-2.2.0/etna/distributions/distributions.py
+-rw-r--r--   0        0        0      226 2023-08-08 14:58:05.911255 etna-2.2.0/etna/ensembles/__init__.py
+-rw-r--r--   0        0        0     6579 2023-08-08 14:58:05.911255 etna-2.2.0/etna/ensembles/direct_ensemble.py
+-rw-r--r--   0        0        0     4996 2023-08-08 14:58:05.911255 etna-2.2.0/etna/ensembles/mixins.py
+-rw-r--r--   0        0        0    11343 2023-08-08 14:58:05.915255 etna-2.2.0/etna/ensembles/stacking_ensemble.py
+-rw-r--r--   0        0        0     9819 2023-08-08 14:58:05.915255 etna-2.2.0/etna/ensembles/voting_ensemble.py
+-rw-r--r--   0        0        0       94 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/change_points/__init__.py
+-rw-r--r--   0        0        0     5558 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/change_points/regularization_search.py
+-rw-r--r--   0        0        0      242 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/__init__.py
+-rw-r--r--   0        0        0      794 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/base.py
+-rw-r--r--   0        0        0     4926 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/classification.py
+-rw-r--r--   0        0        0      366 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/feature_extraction/__init__.py
+-rw-r--r--   0        0        0     1543 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/feature_extraction/base.py
+-rw-r--r--   0        0        0     2510 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/feature_extraction/tsfresh.py
+-rw-r--r--   0        0        0    15250 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/feature_extraction/weasel.py
+-rw-r--r--   0        0        0     3241 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/predictability.py
+-rw-r--r--   0        0        0      874 2023-08-08 14:58:05.915255 etna-2.2.0/etna/experimental/classification/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/__init__.py
+-rw-r--r--   0        0        0       79 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/pmdarima_utils/__init__.py
+-rw-r--r--   0        0        0     7455 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/pmdarima_utils/arima.py
+-rw-r--r--   0        0        0      415 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/pmdarima_utils/arima.pyi
+-rw-r--r--   0        0        0        0 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      472 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/pytorch_lightning/callbacks.py
+-rw-r--r--   0        0        0       48 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/statsforecast/__init__.py
+-rw-r--r--   0        0        0    20329 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/statsforecast/arima.py
+-rw-r--r--   0        0        0      341 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/__init__.py
+-rw-r--r--   0        0        0     1840 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/defaults.py
+-rw-r--r--   0        0        0     1801 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/distribution.py
+-rw-r--r--   0        0        0       69 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/distribution.pyi
+-rw-r--r--   0        0        0    16549 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/relevance.py
+-rw-r--r--   0        0        0      823 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/relevance.pyi
+-rw-r--r--   0        0        0     8470 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/significance_tests.py
+-rw-r--r--   0        0        0      344 2023-08-08 14:58:05.915255 etna-2.2.0/etna/libs/tsfresh/significance_tests.pyi
+-rw-r--r--   0        0        0      804 2023-08-08 14:58:05.915255 etna-2.2.0/etna/loggers/__init__.py
+-rw-r--r--   0        0        0     4993 2023-08-08 14:58:05.915255 etna-2.2.0/etna/loggers/base.py
+-rw-r--r--   0        0        0     2643 2023-08-08 14:58:05.915255 etna-2.2.0/etna/loggers/console_logger.py
+-rw-r--r--   0        0        0    15309 2023-08-08 14:58:05.915255 etna-2.2.0/etna/loggers/file_logger.py
+-rw-r--r--   0        0        0     7105 2023-08-08 14:58:05.915255 etna-2.2.0/etna/loggers/wandb_logger.py
+-rw-r--r--   0        0        0     1213 2023-08-08 14:58:05.915255 etna-2.2.0/etna/metrics/__init__.py
+-rw-r--r--   0        0        0    10745 2023-08-08 14:58:05.915255 etna-2.2.0/etna/metrics/base.py
+-rw-r--r--   0        0        0     8094 2023-08-08 14:58:05.915255 etna-2.2.0/etna/metrics/functional_metrics.py
+-rw-r--r--   0        0        0     5733 2023-08-08 14:58:05.915255 etna-2.2.0/etna/metrics/intervals_metrics.py
+-rw-r--r--   0        0        0    11173 2023-08-08 14:58:05.915255 etna-2.2.0/etna/metrics/metrics.py
+-rw-r--r--   0        0        0     2539 2023-08-08 14:58:05.915255 etna-2.2.0/etna/metrics/utils.py
+-rw-r--r--   0        0        0     2108 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/__init__.py
+-rw-r--r--   0        0        0     2521 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/autoarima.py
+-rw-r--r--   0        0        0    23070 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/base.py
+-rw-r--r--   0        0        0    16375 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/catboost.py
+-rw-r--r--   0        0        0    14515 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/deadline_ma.py
+-rw-r--r--   0        0        0      557 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/decorators.py
+-rw-r--r--   0        0        0    33500 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/holt_winters.py
+-rw-r--r--   0        0        0     8556 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/linear.py
+-rw-r--r--   0        0        0    22852 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/mixins.py
+-rw-r--r--   0        0        0      828 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/moving_average.py
+-rw-r--r--   0        0        0     1031 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/naive.py
+-rw-r--r--   0        0        0      545 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/nn/__init__.py
+-rw-r--r--   0        0        0     9896 2023-08-08 14:58:05.915255 etna-2.2.0/etna/models/nn/deepar.py
+-rw-r--r--   0        0        0      561 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/deepstate/__init__.py
+-rw-r--r--   0        0        0    12488 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/deepstate/deepstate.py
+-rw-r--r--   0        0        0     8808 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/deepstate/linear_dynamic_system.py
+-rw-r--r--   0        0        0    12191 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/deepstate/state_space_model.py
+-rw-r--r--   0        0        0     9163 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/mlp.py
+-rw-r--r--   0        0        0      189 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/nbeats/__init__.py
+-rw-r--r--   0        0        0     7345 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/nbeats/blocks.py
+-rw-r--r--   0        0        0     3115 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/nbeats/metrics.py
+-rw-r--r--   0        0        0    15849 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/nbeats/nbeats.py
+-rw-r--r--   0        0        0     8634 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/nbeats/nets.py
+-rw-r--r--   0        0        0     3337 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/nbeats/utils.py
+-rw-r--r--   0        0        0    13152 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/patchts.py
+-rw-r--r--   0        0        0    11237 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/rnn.py
+-rw-r--r--   0        0        0    11486 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/tft.py
+-rw-r--r--   0        0        0    12817 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/nn/utils.py
+-rw-r--r--   0        0        0    21857 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/prophet.py
+-rw-r--r--   0        0        0    34837 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/sarimax.py
+-rw-r--r--   0        0        0     9064 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/seasonal_ma.py
+-rw-r--r--   0        0        0     4893 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/sklearn.py
+-rw-r--r--   0        0        0    26698 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/statsforecast.py
+-rw-r--r--   0        0        0    20453 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/tbats.py
+-rw-r--r--   0        0        0     3685 2023-08-08 14:58:05.919255 etna-2.2.0/etna/models/utils.py
+-rw-r--r--   0        0        0      292 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/__init__.py
+-rw-r--r--   0        0        0     5437 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/assembling_pipelines.py
+-rw-r--r--   0        0        0     7334 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/autoregressive_pipeline.py
+-rw-r--r--   0        0        0    39133 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/base.py
+-rw-r--r--   0        0        0    14000 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/hierarchical_pipeline.py
+-rw-r--r--   0        0        0     8824 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/mixins.py
+-rw-r--r--   0        0        0     5563 2023-08-08 14:58:05.919255 etna-2.2.0/etna/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:58:05.919255 etna-2.2.0/etna/py.typed
+-rw-r--r--   0        0        0      181 2023-08-08 14:58:05.919255 etna-2.2.0/etna/reconciliation/__init__.py
+-rw-r--r--   0        0        0     3551 2023-08-08 14:58:05.919255 etna-2.2.0/etna/reconciliation/base.py
+-rw-r--r--   0        0        0     1899 2023-08-08 14:58:05.919255 etna-2.2.0/etna/reconciliation/bottom_up.py
+-rw-r--r--   0        0        0     5742 2023-08-08 14:58:05.919255 etna-2.2.0/etna/reconciliation/top_down.py
+-rw-r--r--   0        0        0    11101 2023-08-08 14:58:05.919255 etna-2.2.0/etna/settings.py
+-rw-r--r--   0        0        0     3351 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/__init__.py
+-rw-r--r--   0        0        0    12781 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/base.py
+-rw-r--r--   0        0        0     1244 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/__init__.py
+-rw-r--r--   0        0        0      949 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/__init__.py
+-rw-r--r--   0        0        0     7980 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/base.py
+-rw-r--r--   0        0        0      250 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
+-rw-r--r--   0        0        0     1886 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
+-rw-r--r--   0        0        0     2171 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
+-rw-r--r--   0        0        0     5666 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/detrend.py
+-rw-r--r--   0        0        0     5168 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/level.py
+-rw-r--r--   0        0        0      887 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
+-rw-r--r--   0        0        0      732 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
+-rw-r--r--   0        0        0     1311 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
+-rw-r--r--   0        0        0     3397 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
+-rw-r--r--   0        0        0     2496 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
+-rw-r--r--   0        0        0     5478 2023-08-08 14:58:05.919255 etna-2.2.0/etna/transforms/decomposition/change_points_based/segmentation.py
+-rw-r--r--   0        0        0     5798 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/decomposition/change_points_based/trend.py
+-rw-r--r--   0        0        0     7586 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/decomposition/deseasonal.py
+-rw-r--r--   0        0        0     8552 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/decomposition/detrend.py
+-rw-r--r--   0        0        0     8239 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/decomposition/stl.py
+-rw-r--r--   0        0        0      306 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/encoders/__init__.py
+-rw-r--r--   0        0        0     7512 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/encoders/categorical.py
+-rw-r--r--   0        0        0     2836 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/encoders/mean_segment_encoder.py
+-rw-r--r--   0        0        0     2525 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/encoders/segment_encoder.py
+-rw-r--r--   0        0        0      444 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2469 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/feature_selection/base.py
+-rw-r--r--   0        0        0    10158 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/feature_selection/feature_importance.py
+-rw-r--r--   0        0        0     3434 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/feature_selection/filter.py
+-rw-r--r--   0        0        0    15764 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/feature_selection/gale_shapley.py
+-rw-r--r--   0        0        0     1383 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/__init__.py
+-rw-r--r--   0        0        0     4821 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/add_constant.py
+-rw-r--r--   0        0        0     5645 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/apply_lambda.py
+-rw-r--r--   0        0        0    17152 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/differencing.py
+-rw-r--r--   0        0        0     9987 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/lags.py
+-rw-r--r--   0        0        0     5002 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/log.py
+-rw-r--r--   0        0        0     4469 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/power.py
+-rw-r--r--   0        0        0    10377 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/scalers.py
+-rw-r--r--   0        0        0    11846 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/sklearn.py
+-rw-r--r--   0        0        0    22772 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/math/statistics.py
+-rw-r--r--   0        0        0      233 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/missing_values/__init__.py
+-rw-r--r--   0        0        0     9573 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/missing_values/imputation.py
+-rw-r--r--   0        0        0     6693 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/missing_values/resample.py
+-rw-r--r--   0        0        0      301 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/outliers/__init__.py
+-rw-r--r--   0        0        0     5106 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/outliers/base.py
+-rw-r--r--   0        0        0     7988 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/outliers/point_outliers.py
+-rw-r--r--   0        0        0      334 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/timestamp/__init__.py
+-rw-r--r--   0        0        0    15747 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/timestamp/date_flags.py
+-rw-r--r--   0        0        0     5802 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/timestamp/fourier.py
+-rw-r--r--   0        0        0     3904 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/timestamp/holiday.py
+-rw-r--r--   0        0        0     9079 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/timestamp/special_days.py
+-rw-r--r--   0        0        0     9478 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/timestamp/time_flags.py
+-rw-r--r--   0        0        0      746 2023-08-08 14:58:05.923255 etna-2.2.0/etna/transforms/utils.py
+-rw-r--r--   0        0        0    12105 2023-08-08 14:58:06.147257 etna-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    20464 1970-01-01 00:00:00.000000 etna-2.2.0/PKG-INFO
```

### Comparing `etna-2.1.0/LICENSE` & `etna-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/README.md` & `etna-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -171,23 +171,27 @@
 We have also prepared a set of tutorials for an easy introduction:
 
 | Notebook     | Interactive launch  |
 |:----------|------:|
 | [Get started](https://github.com/tinkoff-ai/etna/tree/master/examples/get_started.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/get_started.ipynb) |
 | [Backtest](https://github.com/tinkoff-ai/etna/tree/master/examples/backtest.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/backtest.ipynb) |
 | [EDA](https://github.com/tinkoff-ai/etna/tree/master/examples/EDA.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/EDA.ipynb) |
-| [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) |
-| [Clustering](https://github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) |
+| [Regressors and exogenous data](https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) |
+| [Custom model and transform](https://github.com/tinkoff-ai/etna/tree/master/examples/custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/custom_transform_and_model.ipynb) |
 | [Deep learning models](https://github.com/tinkoff-ai/etna/tree/master/examples/NN_examples.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/NN_examples.ipynb) |
 | [Ensembles](https://github.com/tinkoff-ai/etna/tree/master/examples/ensembles.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/ensembles.ipynb) |
-| [Custom Transform and Model](https://github.com/tinkoff-ai/etna/tree/master/examples/custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/custom_transform_and_model.ipynb) |
-| [Exogenous data](https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) |
-| [Forecasting strategies](https://github.com/tinkoff-ai/etna/blob/master/examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecasting_strategies.ipynb) |
-| [Classification](https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/classification.ipynb) |
+| [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) |
+| [Forecasting strategies](https://github.com/tinkoff-ai/etna/tree/master/examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecasting_strategies.ipynb) |
+| [Forecast interpretation](https://github.com/tinkoff-ai/etna/tree/master/examples/forecast_interpretation.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecast_interpretation.ipynb) |
+| [Clustering](https://github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) |
+| [AutoML](https://github.com/tinkoff-ai/etna/tree/master/examples/automl.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/automl.ipynb) |
+| [Inference: using saved pipeline on a new data](https://github.com/tinkoff-ai/etna/tree/master/examples/inference.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/inference.ipynb) |
 | [Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/hierarchical_pipeline.ipynb) |
+| [Classification](https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/classification.ipynb) |
+| [Feature selection](https://github.com/tinkoff-ai/etna/blob/master/examples/feature_selection.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/feature_selection.ipynb) |
 
 ## Documentation
 
 ETNA documentation is available [here](https://etna-docs.netlify.app/).
 
 ## Community
```

#### html2text {}

```diff
@@ -75,49 +75,63 @@
 (https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/
 get_started.ipynb) | | [Backtest](https://github.com/tinkoff-ai/etna/tree/
 master/examples/backtest.ipynb) | [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
 master?filepath=examples/backtest.ipynb) | | [EDA](https://github.com/tinkoff-
 ai/etna/tree/master/examples/EDA.ipynb) | [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/EDA.ipynb) | | [Outliers](https://github.com/tinkoff-
-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/
-badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/outliers.ipynb) | | [Clustering](https://github.com/
-tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://
-mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/clustering.ipynb) | | [Deep learning models](https://
-github.com/tinkoff-ai/etna/tree/master/examples/NN_examples.ipynb) | [![Binder]
-(https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/
-etna/master?filepath=examples/NN_examples.ipynb) | | [Ensembles](https://
-github.com/tinkoff-ai/etna/tree/master/examples/ensembles.ipynb) | [![Binder]
-(https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/
-etna/master?filepath=examples/ensembles.ipynb) | | [Custom Transform and Model]
-(https://github.com/tinkoff-ai/etna/tree/master/examples/
+master?filepath=examples/EDA.ipynb) | | [Regressors and exogenous data](https:/
+/github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [!
+[Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
+tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) | | [Custom
+model and transform](https://github.com/tinkoff-ai/etna/tree/master/examples/
 custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/custom_transform_and_model.ipynb) | | [Exogenous data]
-(https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb)
-| [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
-tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) | | [Forecasting
-strategies](https://github.com/tinkoff-ai/etna/blob/master/examples/
-forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/
-badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/forecasting_strategies.ipynb) | | [Classification]
+master?filepath=examples/custom_transform_and_model.ipynb) | | [Deep learning
+models](https://github.com/tinkoff-ai/etna/tree/master/examples/
+NN_examples.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://
+mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/NN_examples.ipynb)
+| | [Ensembles](https://github.com/tinkoff-ai/etna/tree/master/examples/
+ensembles.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://
+mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/ensembles.ipynb) |
+| [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/
+outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://
+mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) | |
+[Forecasting strategies](https://github.com/tinkoff-ai/etna/tree/master/
+examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+master?filepath=examples/forecasting_strategies.ipynb) | | [Forecast
+interpretation](https://github.com/tinkoff-ai/etna/tree/master/examples/
+forecast_interpretation.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+master?filepath=examples/forecast_interpretation.ipynb) | | [Clustering](https:
+//github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [!
+[Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
+tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) | | [AutoML](https:/
+/github.com/tinkoff-ai/etna/tree/master/examples/automl.ipynb) | [![Binder]
+(https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/
+etna/master?filepath=examples/automl.ipynb) | | [Inference: using saved
+pipeline on a new data](https://github.com/tinkoff-ai/etna/tree/master/
+examples/inference.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)]
+(https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/
+inference.ipynb) | | [Hierarchical time series](https://github.com/tinkoff-ai/
+etna/blob/master/examples/hierarchical_pipeline.ipynb) | [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+master?filepath=examples/hierarchical_pipeline.ipynb) | | [Classification]
 (https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb)
 | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
-tinkoff-ai/etna/master?filepath=examples/classification.ipynb) | |
-[Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/
-examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/
-badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/hierarchical_pipeline.ipynb) | ## Documentation ETNA
-documentation is available [here](https://etna-docs.netlify.app/). ## Community
-To ask the questions or discuss the library you can join our [telegram chat]
-(https://t.me/etna_support). [Discussions section](https://github.com/tinkoff-
-ai/etna/discussions) on github is also open for this purpose. ## Resources -
+tinkoff-ai/etna/master?filepath=examples/classification.ipynb) | | [Feature
+selection](https://github.com/tinkoff-ai/etna/blob/master/examples/
+feature_selection.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)]
+(https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/
+feature_selection.ipynb) | ## Documentation ETNA documentation is available
+[here](https://etna-docs.netlify.app/). ## Community To ask the questions or
+discuss the library you can join our [telegram chat](https://t.me/
+etna_support). [Discussions section](https://github.com/tinkoff-ai/etna/
+discussions) on github is also open for this purpose. ## Resources -
 [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/
 forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium - [ETNA
 Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on
 Medium - [Time series forecasting with ETNA: first steps](https://medium.com/
 its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on
 Medium - [ETNA: Time Series Analysis. What, why and how?](https://medium.com/
 its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
```

### Comparing `etna-2.1.0/etna/analysis/__init__.py` & `etna-2.2.0/etna/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/decomposition/__init__.py` & `etna-2.2.0/etna/analysis/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/decomposition/plots.py` & `etna-2.2.0/etna/analysis/decomposition/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/decomposition/search.py` & `etna-2.2.0/etna/analysis/decomposition/search.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/decomposition/utils.py` & `etna-2.2.0/etna/analysis/decomposition/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/eda/plots.py` & `etna-2.2.0/etna/analysis/eda/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/eda/utils.py` & `etna-2.2.0/etna/analysis/eda/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/feature_relevance/plots.py` & `etna-2.2.0/etna/analysis/feature_relevance/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/feature_relevance/relevance.py` & `etna-2.2.0/etna/analysis/feature_relevance/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/feature_relevance/relevance_table.py` & `etna-2.2.0/etna/analysis/feature_relevance/relevance_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     if len(common_index) < len(df.loc[first_valid_idx:, segment]):
         warnings.warn("Exogenous or target data contains None! It will be dropped for calculating relevance.")
     return df_seg.loc[common_index], df_exog_seg.loc[common_index]
 
 
 def get_statistics_relevance_table(df: pd.DataFrame, df_exog: pd.DataFrame) -> pd.DataFrame:
     """Calculate relevance table with p-values from tsfresh.
+
     Parameters
     ----------
     df:
         dataframe with timeseries
     df_exog:
         dataframe with exogenous data
```

### Comparing `etna-2.1.0/etna/analysis/feature_relevance/utils.py` & `etna-2.2.0/etna/analysis/feature_relevance/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/feature_selection/mrmr_selection.py` & `etna-2.2.0/etna/analysis/feature_selection/mrmr_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,20 @@
         warnings.warn(
             "Option `fast_redundancy=False` was added for backward compatibility and will be removed in etna 3.0.0.",
             DeprecationWarning,
         )
     relevance_aggregation_fn = AGGREGATION_FN[AggregationMode(relevance_aggregation_mode)]
     redundancy_aggregation_fn = AGGREGATION_FN[AggregationMode(redundancy_aggregation_mode)]
 
+    # can't compute correlation of categorical column with the others
+    try:
+        regressors = regressors.astype(float)
+    except ValueError as e:
+        raise ValueError(f"Only convertible to float features are allowed! Error: {str(e)}")
+
     relevance = relevance_table.apply(relevance_aggregation_fn).fillna(0)
 
     all_features = relevance.index.to_list()
     segments = set(regressors.columns.get_level_values("segment"))
     selected_features: List[str] = []
     not_selected_features = all_features.copy()
```

### Comparing `etna-2.1.0/etna/analysis/forecast/__init__.py` & `etna-2.2.0/etna/analysis/forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/forecast/plots.py` & `etna-2.2.0/etna/analysis/forecast/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/forecast/utils.py` & `etna-2.2.0/etna/analysis/forecast/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/outliers/__init__.py` & `etna-2.2.0/etna/analysis/outliers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/outliers/density_outliers.py` & `etna-2.2.0/etna/analysis/outliers/density_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/outliers/hist_outliers.py` & `etna-2.2.0/etna/analysis/outliers/hist_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/outliers/median_outliers.py` & `etna-2.2.0/etna/analysis/outliers/median_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/outliers/plots.py` & `etna-2.2.0/etna/analysis/outliers/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/outliers/prediction_interval_outliers.py` & `etna-2.2.0/etna/analysis/outliers/prediction_interval_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/analysis/utils.py` & `etna-2.2.0/etna/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/auto/auto.py` & `etna-2.2.0/etna/auto/auto.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/auto/optuna/config_sampler.py` & `etna-2.2.0/etna/auto/optuna/config_sampler.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/auto/optuna/wrapper.py` & `etna-2.2.0/etna/auto/optuna/wrapper.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/auto/pool/generator.py` & `etna-2.2.0/etna/auto/pool/generator.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/auto/pool/templates.py` & `etna-2.2.0/etna/auto/pool/templates.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/auto/runner/local.py` & `etna-2.2.0/etna/auto/runner/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     """ParallelLocalRunner for multiple parallel runs with joblib.
 
     Notes
     -----
     Global objects behavior could be different while parallel usage because platform dependent new process start.
     Be sure that new process is started with ``fork`` via ``multiprocessing.set_start_method``.
     If it's not possible you should try define all globals before ``if __name__ == "__main__"`` scope.
+
+    Warning
+    -------
+    This class uses :py:mod:`dill` module during serialization which might be not secure.
     """
 
     def __init__(
         self,
         n_jobs: int = 1,
         backend: str = "multiprocessing",
         mmap_mode: str = "c",
```

### Comparing `etna-2.1.0/etna/auto/utils.py` & `etna-2.2.0/etna/auto/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/__init__.py` & `etna-2.2.0/etna/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/base.py` & `etna-2.2.0/etna/clustering/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/distances/base.py` & `etna-2.2.0/etna/clustering/distances/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/distances/distance_matrix.py` & `etna-2.2.0/etna/clustering/distances/distance_matrix.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/distances/dtw_distance.py` & `etna-2.2.0/etna/clustering/distances/dtw_distance.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/distances/euclidean_distance.py` & `etna-2.2.0/etna/clustering/distances/euclidean_distance.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/hierarchical/base.py` & `etna-2.2.0/etna/clustering/hierarchical/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/hierarchical/dtw_clustering.py` & `etna-2.2.0/etna/clustering/hierarchical/dtw_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/clustering/hierarchical/euclidean_clustering.py` & `etna-2.2.0/etna/clustering/hierarchical/euclidean_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/commands/backtest_command.py` & `etna-2.2.0/etna/commands/backtest_command.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/commands/forecast_command.py` & `etna-2.2.0/etna/commands/forecast_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         )
 
         horizon += delta - 1
 
     return horizon
 
 
+def update_horizon(pipeline_configs: Dict[str, Any], forecast_params: Dict[str, Any], tsdataset: TSDataset):
+    """Update the ``horizon`` parameter in the pipeline config if ``start_timestamp`` is set."""
+    for config in pipeline_configs.get("pipelines", [pipeline_configs]):
+        horizon: int = config["horizon"]  # type: ignore
+        horizon = compute_horizon(horizon=horizon, forecast_params=forecast_params, tsdataset=tsdataset)
+        config["horizon"] = horizon  # type: ignore
+
+
 def filter_forecast(forecast_ts: TSDataset, forecast_params: Dict[str, Any]) -> TSDataset:
     """Filter out forecasts before `start_timestamp` if `start_timestamp` presented in `forecast_params`.."""
     if "start_timestamp" in forecast_params:
         forecast_start_timestamp = pd.Timestamp(forecast_params["start_timestamp"], freq=forecast_ts.freq)
         forecast_ts.df = forecast_ts.df.loc[forecast_start_timestamp:, :]
 
     return forecast_ts
@@ -118,17 +126,15 @@
     if exog_path:
         df_exog = pd.read_csv(exog_path, parse_dates=["timestamp"])
         df_exog = TSDataset.to_dataset(df_exog)
         k_f = "all" if not known_future else known_future
 
     tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog, known_future=k_f)
 
-    horizon: int = pipeline_configs["horizon"]  # type: ignore
-    horizon = compute_horizon(horizon=horizon, forecast_params=forecast_params, tsdataset=tsdataset)
-    pipeline_configs["horizon"] = horizon  # type: ignore
+    update_horizon(pipeline_configs=pipeline_configs, forecast_params=forecast_params, tsdataset=tsdataset)
 
     pipeline_args = remove_params(params=pipeline_configs, to_remove=ADDITIONAL_PIPELINE_PARAMETERS)
     pipeline: Pipeline = hydra_slayer.get_from_params(**pipeline_args)
     pipeline.fit(tsdataset)
 
     # estimate number of folds if parameters set
     if forecast_params.get("estimate_n_folds", False):
```

### Comparing `etna-2.1.0/etna/commands/utils.py` & `etna-2.2.0/etna/commands/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/core/mixins.py` & `etna-2.2.0/etna/core/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         }
         metadata_str = json.dumps(metadata, indent=2, sort_keys=True)
         metadata_bytes = metadata_str.encode("utf-8")
         with archive.open("metadata.json", "w") as output_file:
             output_file.write(metadata_bytes)
 
     def _save_state(self, archive: zipfile.ZipFile):
-        with archive.open("object.pkl", "w") as output_file:
+        with archive.open("object.pkl", "w", force_zip64=True) as output_file:
             dill.dump(self, output_file)
 
     def save(self, path: pathlib.Path):
         """Save the object.
 
         Parameters
         ----------
@@ -272,14 +272,20 @@
         with archive.open("object.pkl", "r") as input_file:
             return dill.load(input_file)
 
     @classmethod
     def load(cls, path: pathlib.Path) -> Self:
         """Load an object.
 
+        Warning
+        -------
+        This method uses :py:mod:`dill` module which is not secure.
+        It is possible to construct malicious data which will execute arbitrary code during loading.
+        Never load data that could have come from an untrusted source, or that could have been tampered with.
+
         Parameters
         ----------
         path:
             Path to load object from.
 
         Returns
         -------
```

### Comparing `etna-2.1.0/etna/core/saving.py` & `etna-2.2.0/etna/core/saving.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/core/utils.py` & `etna-2.2.0/etna/core/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 from hydra_slayer import get_factory
 
 
 def load(path: pathlib.Path, **kwargs: Any) -> Any:
     """Load saved object by path.
 
+    Warning
+    -------
+    This method uses :py:mod:`dill` module which is not secure.
+    It is possible to construct malicious data which will execute arbitrary code during loading.
+    Never load data that could have come from an untrusted source, or that could have been tampered with.
+
     Parameters
     ----------
     path:
         Path to load object from.
     kwargs:
         Parameters for loading specific for the loaded object.
```

### Comparing `etna-2.1.0/etna/datasets/__init__.py` & `etna-2.2.0/etna/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/datasets/datasets_generation.py` & `etna-2.2.0/etna/datasets/datasets_generation.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/datasets/hierarchical_structure.py` & `etna-2.2.0/etna/datasets/hierarchical_structure.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/datasets/tsdataset.py` & `etna-2.2.0/etna/datasets/tsdataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1316,33 +1316,45 @@
             "num_regressors": len(self.regressors),
             "num_known_future": len(self.known_future),
             "freq": self.freq,
         }
 
         return common_dict
 
-    def _gather_segments_data(self, segments: Sequence[str]) -> Dict[str, List[Any]]:
+    def _gather_segments_data(self, segments: Optional[Sequence[str]]) -> Dict[str, pd.Series]:
         """Gather information about each segment."""
-        # gather segment information
-        segments_dict: Dict[str, list] = {
-            "start_timestamp": [],
-            "end_timestamp": [],
-            "length": [],
-            "num_missing": [],
-        }
-
-        for segment in segments:
-            segment_series = self[:, segment, "target"]
-            first_index = segment_series.first_valid_index()
-            last_index = segment_series.last_valid_index()
-            segment_series = segment_series.loc[first_index:last_index]
-            segments_dict["start_timestamp"].append(first_index)
-            segments_dict["end_timestamp"].append(last_index)
-            segments_dict["length"].append(segment_series.shape[0])
-            segments_dict["num_missing"].append(pd.isna(segment_series).sum())
+        segments_index: Union[slice, Sequence[str]]
+        if segments is None:
+            segments_index = slice(None)
+            segments = self.segments
+        else:
+            segments_index = segments
+            segments = segments
+
+        df = self.df.loc[:, (segments_index, "target")]
+
+        num_timestamps = df.shape[0]
+        not_na = ~np.isnan(df.values)
+        min_idx = np.argmax(not_na, axis=0)
+        max_idx = num_timestamps - np.argmax(not_na[::-1, :], axis=0) - 1
+
+        segments_dict = {}
+        segments_dict["start_timestamp"] = df.index[min_idx].to_series(index=segments)
+        segments_dict["end_timestamp"] = df.index[max_idx].to_series(index=segments)
+        segments_dict["length"] = pd.Series(max_idx - min_idx + 1, dtype="Int64", index=segments)
+        segments_dict["num_missing"] = pd.Series(
+            segments_dict["length"] - np.sum(not_na, axis=0), dtype="Int64", index=segments
+        )
+
+        # handle all-nans series
+        all_nans_mask = np.all(~not_na, axis=0)
+        segments_dict["start_timestamp"][all_nans_mask] = None
+        segments_dict["end_timestamp"][all_nans_mask] = None
+        segments_dict["length"][all_nans_mask] = None
+        segments_dict["num_missing"][all_nans_mask] = None
 
         return segments_dict
 
     def describe(self, segments: Optional[Sequence[str]] = None) -> pd.DataFrame:
         """Overview of the dataset that returns a DataFrame.
 
         Method describes dataset in segment-wise fashion. Description columns:
@@ -1396,23 +1408,23 @@
         >>> ts = TSDataset(df_ts_format, df_exog=df_exog_ts_format, freq="D", known_future="all")
         >>> ts.describe()
                   start_timestamp end_timestamp  length  num_missing  num_segments  num_exogs  num_regressors  num_known_future freq
         segments
         segment_0      2021-06-01    2021-06-30      30            0             2          1               1                 1    D
         segment_1      2021-06-01    2021-06-30      30            0             2          1               1                 1    D
         """
-        if segments is None:
-            segments = self.segments
-
         # gather common information
         common_dict = self._gather_common_data()
 
         # gather segment information
         segments_dict = self._gather_segments_data(segments)
 
+        if segments is None:
+            segments = self.segments
+
         # combine information
         segments_dict["num_segments"] = [common_dict["num_segments"]] * len(segments)
         segments_dict["num_exogs"] = [common_dict["num_exogs"]] * len(segments)
         segments_dict["num_regressors"] = [common_dict["num_regressors"]] * len(segments)
         segments_dict["num_known_future"] = [common_dict["num_known_future"]] * len(segments)
         segments_dict["freq"] = [common_dict["freq"]] * len(segments)
```

### Comparing `etna-2.1.0/etna/datasets/utils.py` & `etna-2.2.0/etna/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/distributions/distributions.py` & `etna-2.2.0/etna/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/ensembles/direct_ensemble.py` & `etna-2.2.0/etna/ensembles/direct_ensemble.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/ensembles/mixins.py` & `etna-2.2.0/etna/ensembles/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,14 +112,20 @@
                     pipeline.save(pipeline_save_path)
                     archive.write(pipeline_save_path, f"pipelines/{save_name}")
 
     @classmethod
     def load(cls, path: pathlib.Path, ts: Optional[TSDataset] = None) -> Self:
         """Load an object.
 
+        Warning
+        -------
+        This method uses :py:mod:`dill` module which is not secure.
+        It is possible to construct malicious data which will execute arbitrary code during loading.
+        Never load data that could have come from an untrusted source, or that could have been tampered with.
+
         Parameters
         ----------
         path:
             Path to load object from.
         ts:
             TSDataset to set into loaded pipeline.
```

### Comparing `etna-2.1.0/etna/ensembles/stacking_ensemble.py` & `etna-2.2.0/etna/ensembles/stacking_ensemble.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/ensembles/voting_ensemble.py` & `etna-2.2.0/etna/ensembles/voting_ensemble.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/change_points/regularization_search.py` & `etna-2.2.0/etna/experimental/change_points/regularization_search.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/classification/classification.py` & `etna-2.2.0/etna/experimental/classification/classification.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/classification/feature_extraction/base.py` & `etna-2.2.0/etna/experimental/classification/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/classification/feature_extraction/tsfresh.py` & `etna-2.2.0/etna/experimental/classification/feature_extraction/tsfresh.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/classification/feature_extraction/weasel.py` & `etna-2.2.0/etna/experimental/classification/feature_extraction/weasel.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/classification/predictability.py` & `etna-2.2.0/etna/experimental/classification/predictability.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/experimental/classification/utils.py` & `etna-2.2.0/etna/experimental/classification/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/libs/pmdarima_utils/arima.py` & `etna-2.2.0/etna/libs/pmdarima_utils/arima.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/libs/tsfresh/defaults.py` & `etna-2.2.0/etna/libs/tsfresh/defaults.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/libs/tsfresh/distribution.py` & `etna-2.2.0/etna/libs/tsfresh/distribution.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/libs/tsfresh/relevance.py` & `etna-2.2.0/etna/libs/tsfresh/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/libs/tsfresh/relevance.pyi` & `etna-2.2.0/etna/libs/tsfresh/relevance.pyi`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/libs/tsfresh/significance_tests.py` & `etna-2.2.0/etna/libs/tsfresh/significance_tests.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/loggers/__init__.py` & `etna-2.2.0/etna/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/loggers/base.py` & `etna-2.2.0/etna/loggers/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/loggers/console_logger.py` & `etna-2.2.0/etna/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/loggers/file_logger.py` & `etna-2.2.0/etna/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/loggers/wandb_logger.py` & `etna-2.2.0/etna/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/metrics/base.py` & `etna-2.2.0/etna/metrics/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from abc import ABC
 from abc import abstractmethod
 from enum import Enum
-from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
+from typing_extensions import Protocol
+from typing_extensions import assert_never
 
 from etna.core import BaseMixin
 from etna.datasets.tsdataset import TSDataset
 from etna.loggers import tslogger
+from etna.metrics.functional_metrics import ArrayLike
 
 
 class MetricAggregationMode(str, Enum):
     """Enum for different metric aggregation modes."""
 
     macro = "macro"
     per_segment = "per-segment"
@@ -23,14 +25,39 @@
     @classmethod
     def _missing_(cls, value):
         raise NotImplementedError(
             f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} aggregation allowed"
         )
 
 
+class MetricFunctionSignature(str, Enum):
+    """Enum for different metric function signatures."""
+
+    #: function should expect arrays of y_pred and y_true with length ``n_timestamps`` and return scalar
+    array_to_scalar = "array_to_scalar"
+
+    #: function should expect matrices of y_pred and y_true with shape ``(n_timestamps, n_segments)``
+    #: and return vector of length ``n_segments``
+    matrix_to_array = "matrix_to_array"
+
+    @classmethod
+    def _missing_(cls, value):
+        raise NotImplementedError(
+            f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} signatures allowed"
+        )
+
+
+class MetricFunction(Protocol):
+    """Protocol for ``metric_fn`` parameter."""
+
+    @abstractmethod
+    def __call__(self, y_true: ArrayLike, y_pred: ArrayLike) -> ArrayLike:
+        pass
+
+
 class AbstractMetric(ABC):
     """Abstract class for metric."""
 
     @abstractmethod
     def __call__(self, y_true: TSDataset, y_pred: TSDataset) -> Union[float, Dict[str, float]]:
         """
         Compute metric's value with ``y_true`` and ``y_pred``.
@@ -70,68 +97,79 @@
     """
     Base class for all the multi-segment metrics.
 
     How it works: Metric computes ``metric_fn`` value for each segment in given forecast
     dataset and aggregates it according to mode.
     """
 
-    def __init__(self, metric_fn: Callable[..., float], mode: str = MetricAggregationMode.per_segment, **kwargs):
+    def __init__(
+        self,
+        metric_fn: MetricFunction,
+        mode: str = MetricAggregationMode.per_segment,
+        metric_fn_signature: str = "array_to_scalar",
+        **kwargs,
+    ):
         """
         Init Metric.
 
         Parameters
         ----------
         metric_fn:
             functional metric
         mode:
             "macro" or "per-segment", way to aggregate metric values over segments:
 
             * if "macro" computes average value
 
             * if "per-segment" -- does not aggregate metrics
 
+        metric_fn_signature:
+            type of signature of ``metric_fn`` (see :py:class:`~etna.metrics.base.MetricFunctionSignature`)
         kwargs:
             functional metric's params
 
         Raises
         ------
         NotImplementedError:
-            it non existent mode is used
+            If non-existent ``mode`` is used.
+        NotImplementedError:
+            If non-existent ``metric_fn_signature`` is used.
         """
-        self.metric_fn = metric_fn
-        self.kwargs = kwargs
-        if MetricAggregationMode(mode) == MetricAggregationMode.macro:
+        if MetricAggregationMode(mode) is MetricAggregationMode.macro:
             self._aggregate_metrics = self._macro_average
-        elif MetricAggregationMode(mode) == MetricAggregationMode.per_segment:
+        elif MetricAggregationMode(mode) is MetricAggregationMode.per_segment:
             self._aggregate_metrics = self._per_segment_average
+
+        self._metric_fn_signature = MetricFunctionSignature(metric_fn_signature)
+
+        self.metric_fn = metric_fn
+        self.kwargs = kwargs
         self.mode = mode
+        self.metric_fn_signature = metric_fn_signature
 
     @property
     def name(self) -> str:
         """Name of the metric for representation."""
         return self.__class__.__name__
 
     @staticmethod
-    def _validate_segment_columns(y_true: TSDataset, y_pred: TSDataset):
-        """
-        Check if all the segments from ``y_true`` are in ``y_pred`` and vice versa.
+    def _validate_segments(y_true: TSDataset, y_pred: TSDataset):
+        """Check that segments in ``y_true`` and ``y_pred`` are the same.
 
         Parameters
         ----------
         y_true:
             y_true dataset
         y_pred:
             y_pred dataset
 
         Raises
         ------
         ValueError:
-            if there are mismatches in y_true and y_pred segments,
-        ValueError:
-            if one of segments in y_true or y_pred doesn't contain 'target' column.
+            if there are mismatches in y_true and y_pred segments
         """
         segments_true = set(y_true.df.columns.get_level_values("segment"))
         segments_pred = set(y_pred.df.columns.get_level_values("segment"))
 
         pred_diff_true = segments_pred - segments_true
         true_diff_pred = segments_true - segments_pred
         if pred_diff_true:
@@ -140,42 +178,87 @@
                 f"{', '.join(list(pred_diff_true)[:5])}"
             )
         if true_diff_pred:
             raise ValueError(
                 f"There are segments in y_true that are not in y_pred, for example: "
                 f"{', '.join(list(true_diff_pred)[:5])}"
             )
-        for segment in segments_true:
+
+    @staticmethod
+    def _validate_target_columns(y_true: TSDataset, y_pred: TSDataset):
+        """Check that all the segments from ``y_true`` and ``y_pred`` has 'target' column.
+
+        Parameters
+        ----------
+        y_true:
+            y_true dataset
+        y_pred:
+            y_pred dataset
+
+        Raises
+        ------
+        ValueError:
+            if one of segments in y_true or y_pred doesn't contain 'target' column.
+        """
+        segments = set(y_true.df.columns.get_level_values("segment"))
+
+        for segment in segments:
             for name, dataset in zip(("y_true", "y_pred"), (y_true, y_pred)):
-                if "target" not in dataset.loc[:, segment].columns:
+                if (segment, "target") not in dataset.columns:
                     raise ValueError(
                         f"All the segments in {name} should contain 'target' column. Segment {segment} doesn't."
                     )
 
     @staticmethod
-    def _validate_timestamp_columns(timestamp_true: pd.Series, timestamp_pred: pd.Series):
-        """
-        Check that ``y_true`` and ``y_pred`` have the same timestamp.
+    def _validate_index(y_true: TSDataset, y_pred: TSDataset):
+        """Check that ``y_true`` and ``y_pred`` have the same timestamps.
 
         Parameters
         ----------
-        timestamp_true:
-            y_true's timestamp column
-        timestamp_pred:
-            y_pred's timestamp column
+        y_true:
+            y_true dataset
+        y_pred:
+            y_pred dataset
 
         Raises
         ------
         ValueError:
             If there are mismatches in ``y_true`` and ``y_pred`` timestamps
         """
-        if set(timestamp_pred) != set(timestamp_true):
+        if not y_true.index.equals(y_pred.index):
             raise ValueError("y_true and y_pred have different timestamps")
 
     @staticmethod
+    def _validate_nans(y_true: TSDataset, y_pred: TSDataset):
+        """Check that ``y_true`` and ``y_pred`` doesn't have NaNs.
+
+        Parameters
+        ----------
+        y_true:
+            y_true dataset
+        y_pred:
+            y_pred dataset
+
+        Raises
+        ------
+        ValueError:
+            If there are NaNs in ``y_true`` or ``y_pred``
+        """
+        df_true = y_true.df.loc[:, pd.IndexSlice[:, "target"]]
+        df_pred = y_pred.df.loc[:, pd.IndexSlice[:, "target"]]
+
+        df_true_isna = df_true.isna().any().any()
+        if df_true_isna > 0:
+            raise ValueError("There are NaNs in y_true")
+
+        df_pred_isna = df_pred.isna().any().any()
+        if df_pred_isna > 0:
+            raise ValueError("There are NaNs in y_pred")
+
+    @staticmethod
     def _macro_average(metrics_per_segments: Dict[str, float]) -> Union[float, Dict[str, float]]:
         """
         Compute macro averaging of metrics over segment.
 
         Parameters
         ----------
         metrics_per_segments: dict of {segment: metric_value} for segments to aggregate
@@ -222,24 +305,35 @@
 
         Returns
         -------
         :
             metric's value aggregated over segments or not (depends on mode)
         """
         self._log_start()
-        self._validate_segment_columns(y_true=y_true, y_pred=y_pred)
+        self._validate_segments(y_true=y_true, y_pred=y_pred)
+        self._validate_target_columns(y_true=y_true, y_pred=y_pred)
+        self._validate_index(y_true=y_true, y_pred=y_pred)
+        self._validate_nans(y_true=y_true, y_pred=y_pred)
+
+        df_true = y_true[:, :, "target"].sort_index(axis=1)
+        df_pred = y_pred[:, :, "target"].sort_index(axis=1)
+
+        segments = df_true.columns.get_level_values("segment").unique()
+
+        metrics_per_segment: Dict[str, float]
+        if self._metric_fn_signature is MetricFunctionSignature.array_to_scalar:
+            metrics_per_segment = {}
+            for i, segment in enumerate(segments):
+                cur_y_true = df_true.iloc[:, i].values
+                cur_y_pred = df_pred.iloc[:, i].values
+                metrics_per_segment[segment] = self.metric_fn(y_true=cur_y_true, y_pred=cur_y_pred, **self.kwargs)  # type: ignore
+        elif self._metric_fn_signature is MetricFunctionSignature.matrix_to_array:
+            values = self.metric_fn(y_true=df_true.values, y_pred=df_pred.values, **self.kwargs)
+            metrics_per_segment = dict(zip(segments, values))  # type: ignore
+        else:
+            assert_never(self._metric_fn_signature)
 
-        segments = set(y_true.df.columns.get_level_values("segment"))
-        metrics_per_segment = {}
-        for segment in segments:
-            self._validate_timestamp_columns(
-                timestamp_true=y_true[:, segment, "target"].dropna().index,
-                timestamp_pred=y_pred[:, segment, "target"].dropna().index,
-            )
-            metrics_per_segment[segment] = self.metric_fn(
-                y_true=y_true[:, segment, "target"].values, y_pred=y_pred[:, segment, "target"].values, **self.kwargs
-            )
         metrics = self._aggregate_metrics(metrics_per_segment)
         return metrics
 
 
 __all__ = ["Metric", "MetricAggregationMode"]
```

### Comparing `etna-2.1.0/etna/metrics/intervals_metrics.py` & `etna-2.2.0/etna/metrics/intervals_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from typing import Union
 
 import numpy as np
 
 from etna.datasets import TSDataset
 from etna.metrics.base import Metric
 from etna.metrics.base import MetricAggregationMode
+from etna.metrics.functional_metrics import ArrayLike
 
 
-def dummy():
+def dummy(y_true: ArrayLike, y_pred: ArrayLike) -> ArrayLike:
     return np.nan
 
 
 class _QuantileMetricMixin:
     def _validate_tsdataset_quantiles(self, ts: TSDataset, quantiles: Sequence[float]) -> None:
         """Check if quantiles presented in y_pred."""
         features = set(ts.df.columns.get_level_values("feature"))
@@ -63,28 +64,31 @@
         y_pred:
             dataset with predicted time series values
 
         Returns
         -------
             metric's value aggregated over segments or not (depends on mode)
         """
-        self._validate_segment_columns(y_true=y_true, y_pred=y_pred)
+        self._validate_segments(y_true=y_true, y_pred=y_pred)
+        self._validate_target_columns(y_true=y_true, y_pred=y_pred)
+        self._validate_index(y_true=y_true, y_pred=y_pred)
+        self._validate_nans(y_true=y_true, y_pred=y_pred)
         self._validate_tsdataset_quantiles(ts=y_pred, quantiles=self.quantiles)
 
-        segments = set(y_true.df.columns.get_level_values("segment"))
-        metrics_per_segment = {}
-        for segment in segments:
-            self._validate_timestamp_columns(
-                timestamp_true=y_true[:, segment, "target"].dropna().index,
-                timestamp_pred=y_pred[:, segment, "target"].dropna().index,
-            )
-            upper_quantile_flag = y_true[:, segment, "target"] <= y_pred[:, segment, f"target_{self.quantiles[1]:.4g}"]
-            lower_quantile_flag = y_true[:, segment, "target"] >= y_pred[:, segment, f"target_{self.quantiles[0]:.4g}"]
+        df_true = y_true[:, :, "target"].sort_index(axis=1)
+        df_pred_lower = y_pred[:, :, f"target_{self.quantiles[0]:.4g}"].sort_index(axis=1)
+        df_pred_upper = y_pred[:, :, f"target_{self.quantiles[1]:.4g}"].sort_index(axis=1)
+
+        segments = df_true.columns.get_level_values("segment").unique()
+
+        upper_quantile_flag = df_true.values <= df_pred_upper.values
+        lower_quantile_flag = df_true.values >= df_pred_lower.values
+        values = np.mean(upper_quantile_flag * lower_quantile_flag, axis=0)
+        metrics_per_segment = dict(zip(segments, values))
 
-            metrics_per_segment[segment] = np.mean(upper_quantile_flag * lower_quantile_flag)
         metrics = self._aggregate_metrics(metrics_per_segment)
         return metrics
 
     @property
     def greater_is_better(self) -> None:
         """Whether higher metric value is better."""
         return None
@@ -131,28 +135,28 @@
         y_pred:
             dataset with predicted time series values
 
         Returns
         -------
             metric's value aggregated over segments or not (depends on mode)
         """
-        self._validate_segment_columns(y_true=y_true, y_pred=y_pred)
+        self._validate_segments(y_true=y_true, y_pred=y_pred)
+        self._validate_target_columns(y_true=y_true, y_pred=y_pred)
+        self._validate_index(y_true=y_true, y_pred=y_pred)
+        self._validate_nans(y_true=y_true, y_pred=y_pred)
         self._validate_tsdataset_quantiles(ts=y_pred, quantiles=self.quantiles)
 
-        segments = set(y_true.df.columns.get_level_values("segment"))
-        metrics_per_segment = {}
-        for segment in segments:
-            self._validate_timestamp_columns(
-                timestamp_true=y_true[:, segment, "target"].dropna().index,
-                timestamp_pred=y_pred[:, segment, "target"].dropna().index,
-            )
-            upper_quantile = y_pred[:, segment, f"target_{self.quantiles[1]:.4g}"]
-            lower_quantile = y_pred[:, segment, f"target_{self.quantiles[0]:.4g}"]
+        df_true = y_true[:, :, "target"].sort_index(axis=1)
+        df_pred_lower = y_pred[:, :, f"target_{self.quantiles[0]:.4g}"].sort_index(axis=1)
+        df_pred_upper = y_pred[:, :, f"target_{self.quantiles[1]:.4g}"].sort_index(axis=1)
 
-            metrics_per_segment[segment] = np.abs(lower_quantile - upper_quantile).mean()
+        segments = df_true.columns.get_level_values("segment").unique()
+
+        values = np.mean(np.abs(df_pred_upper.values - df_pred_lower.values), axis=0)
+        metrics_per_segment = dict(zip(segments, values))
 
         metrics = self._aggregate_metrics(metrics_per_segment)
         return metrics
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
```

### Comparing `etna-2.1.0/etna/metrics/metrics.py` & `etna-2.2.0/etna/metrics/metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from etna.metrics import mae
-from etna.metrics import mape
-from etna.metrics import max_deviation
-from etna.metrics import medae
-from etna.metrics import mse
-from etna.metrics import msle
-from etna.metrics import r2_score
-from etna.metrics import rmse
-from etna.metrics import sign
-from etna.metrics import smape
-from etna.metrics import wape
+from functools import partial
+
 from etna.metrics.base import Metric
 from etna.metrics.base import MetricAggregationMode
+from etna.metrics.functional_metrics import mae
+from etna.metrics.functional_metrics import mape
+from etna.metrics.functional_metrics import max_deviation
+from etna.metrics.functional_metrics import medae
+from etna.metrics.functional_metrics import mse
+from etna.metrics.functional_metrics import msle
+from etna.metrics.functional_metrics import r2_score
+from etna.metrics.functional_metrics import rmse
+from etna.metrics.functional_metrics import sign
+from etna.metrics.functional_metrics import smape
+from etna.metrics.functional_metrics import wape
 
 
 class MAE(Metric):
     """Mean absolute error metric with multi-segment computation support.
 
     .. math::
         MAE(y\_true, y\_pred) = \\frac{\\sum_{i=0}^{n-1}{\\mid y\_true_i - y\_pred_i \\mid}}{n}
@@ -30,15 +32,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=mae, **kwargs)
+        mae_per_output = partial(mae, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=mae_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -59,15 +62,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=mse, **kwargs)
+        mse_per_output = partial(mse, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=mse_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -88,15 +92,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=rmse, **kwargs)
+        rmse_per_output = partial(rmse, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=rmse_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -116,15 +121,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=r2_score, **kwargs)
+        r2_per_output = partial(r2_score, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=r2_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return True
 
 
@@ -145,15 +151,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=mape, **kwargs)
+        mape_per_output = partial(mape, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=mape_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -174,15 +181,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=smape, **kwargs)
+        smape_per_output = partial(smape, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=smape_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -203,15 +211,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=medae, **kwargs)
+        medae_per_output = partial(medae, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=medae_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -233,15 +242,16 @@
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
 
         """
-        super().__init__(mode=mode, metric_fn=msle, **kwargs)
+        msle_per_output = partial(msle, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=msle_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -262,15 +272,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=sign, **kwargs)
+        sign_per_output = partial(sign, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=sign_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> None:
         """Whether higher metric value is better."""
         return None
 
 
@@ -291,15 +302,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=max_deviation, **kwargs)
+        max_deviation_per_output = partial(max_deviation, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=max_deviation_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
 
 
@@ -319,15 +331,16 @@
         Parameters
         ----------
         mode: 'macro' or 'per-segment'
             metrics aggregation mode
         kwargs:
             metric's computation arguments
         """
-        super().__init__(mode=mode, metric_fn=wape, **kwargs)
+        wape_per_output = partial(wape, multioutput="raw_values")
+        super().__init__(mode=mode, metric_fn=wape_per_output, metric_fn_signature="matrix_to_array", **kwargs)
 
     @property
     def greater_is_better(self) -> bool:
         """Whether higher metric value is better."""
         return False
```

### Comparing `etna-2.1.0/etna/metrics/utils.py` & `etna-2.2.0/etna/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/__init__.py` & `etna-2.2.0/etna/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,7 +27,14 @@
 from etna.models.sklearn import SklearnMultiSegmentModel
 from etna.models.sklearn import SklearnPerSegmentModel
 from etna.models.tbats import BATSModel
 from etna.models.tbats import TBATSModel
 
 if SETTINGS.prophet_required:
     from etna.models.prophet import ProphetModel
+
+if SETTINGS.statsforecast_required:
+    from etna.models.statsforecast import StatsForecastARIMAModel
+    from etna.models.statsforecast import StatsForecastAutoARIMAModel
+    from etna.models.statsforecast import StatsForecastAutoCESModel
+    from etna.models.statsforecast import StatsForecastAutoETSModel
+    from etna.models.statsforecast import StatsForecastAutoThetaModel
```

### Comparing `etna-2.1.0/etna/models/autoarima.py` & `etna-2.2.0/etna/models/autoarima.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/base.py` & `etna-2.2.0/etna/models/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/catboost.py` & `etna-2.2.0/etna/models/catboost.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             List of the columns with regressors(ignored in this model)
 
         Returns
         -------
         :
             Fitted model
         """
+        df = df.sort_values(by="timestamp")
         features = df.drop(columns=["timestamp", "target"])
         target = df["target"]
         train_pool = self._prepare_pool(features, target.values)
         self.model.fit(train_pool)
         return self
 
     def predict(self, df: pd.DataFrame) -> np.ndarray:
```

### Comparing `etna-2.1.0/etna/models/deadline_ma.py` & `etna-2.2.0/etna/models/deadline_ma.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,23 @@
         Returns
         -------
         :
            Itself
         """
         return self
 
+    def _check_not_used_columns(self, ts: TSDataset):
+        columns = set(ts.columns.get_level_values("feature"))
+        columns_not_used = columns.difference({"target"})
+        if columns_not_used:
+            warnings.warn(
+                message=f"This model doesn't work with exogenous features. "
+                f"Columns {columns_not_used} won't be used."
+            )
+
     def fit(self, ts: TSDataset) -> "DeadlineMovingAverageModel":
         """Fit model.
 
         Parameters
         ----------
         ts:
             Dataset with features
@@ -105,22 +114,16 @@
             Model after fit
         """
         # we make a normalization to treat "1d" like "D"
         freq = pd.tseries.frequencies.to_offset(ts.freq).freqstr
         if freq not in self._freqs_available:
             raise ValueError(f"Freq {freq} is not supported! Use daily or hourly frequency!")
 
+        self._check_not_used_columns(ts)
         self._freq = freq
-
-        columns = set(ts.columns.get_level_values("feature"))
-        if columns != {"target"}:
-            warnings.warn(
-                message=f"{type(self).__name__} does not work with any exogenous series or features. "
-                f"It uses only target series for predict/\n "
-            )
         return self
 
     @staticmethod
     def _get_context_beginning(
         df: pd.DataFrame, prediction_size: int, seasonality: SeasonalityMode, window: int
     ) -> pd.Timestamp:
         """Get timestamp where context begins.
```

### Comparing `etna-2.1.0/etna/models/decorators.py` & `etna-2.2.0/etna/models/decorators.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/holt_winters.py` & `etna-2.2.0/etna/models/holt_winters.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,23 @@
         self._model: Optional[ExponentialSmoothing] = None
         self._result: Optional[HoltWintersResultsWrapper] = None
 
         self._first_train_timestamp: Optional[pd.Timestamp] = None
         self._last_train_timestamp: Optional[pd.Timestamp] = None
         self._train_freq: Optional[str] = None
 
+    def _check_not_used_columns(self, df: pd.DataFrame):
+        columns = df.columns
+        columns_not_used = set(columns).difference({"target", "timestamp"})
+        if columns_not_used:
+            warnings.warn(
+                message=f"This model doesn't work with exogenous features. "
+                f"Columns {columns_not_used} won't be used."
+            )
+
     def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_HoltWintersAdapter":
         """
         Fit Holt-Winters' model.
 
         Parameters
         ----------
         df:
@@ -213,16 +222,15 @@
             List of the columns with regressors(ignored in this model)
         Returns
         -------
         :
             Fitted model
         """
         self._train_freq = determine_freq(timestamps=df["timestamp"])
-
-        self._check_df(df)
+        self._check_not_used_columns(df)
 
         targets = df["target"]
         targets.index = df["timestamp"]
 
         self._model = ExponentialSmoothing(
             endog=targets,
             trend=self.trend,
@@ -264,29 +272,19 @@
         Returns
         -------
         :
             Array with predictions
         """
         if self._result is None or self._model is None:
             raise ValueError("This model is not fitted! Fit the model before calling predict method!")
-        self._check_df(df)
 
         forecast = self._result.predict(start=df["timestamp"].min(), end=df["timestamp"].max())
         y_pred = forecast.values
         return y_pred
 
-    def _check_df(self, df: pd.DataFrame):
-        columns = df.columns
-        columns_not_used = set(columns).difference({"target", "timestamp"})
-        if columns_not_used:
-            warnings.warn(
-                message=f"This model does not work with exogenous features and regressors.\n "
-                f"{columns_not_used} will be dropped"
-            )
-
     def get_model(self) -> HoltWintersResultsWrapper:
         """Get :py:class:`statsmodels.tsa.holtwinters.results.HoltWintersResultsWrapper` model that was fitted inside etna class.
 
         Returns
         -------
         :
            Internal model
@@ -299,15 +297,15 @@
 
         if model is None:
             raise ValueError("This model is not fitted!")
 
         if (model.trend is not None and model.trend == "mul") or (
             model.seasonal is not None and model.seasonal == "mul"
         ):
-            raise ValueError("Forecast decomposition is only supported for additive components!")
+            raise NotImplementedError("Forecast decomposition is only supported for additive components!")
 
     def _rescale_components(self, components: pd.DataFrame) -> pd.DataFrame:
         """Rescale components when Box-Cox transform used."""
         if self._result is None:
             raise ValueError("This model is not fitted!")
 
         pred = np.sum(components.values, axis=1)
@@ -331,23 +329,25 @@
         model = self._model
         fit_result = self._result
 
         if fit_result is None or model is None or self._train_freq is None:
             raise ValueError("This model is not fitted!")
 
         if df["timestamp"].min() <= self._last_train_timestamp:
-            raise ValueError("To estimate in-sample prediction decomposition use `predict` method.")
+            raise NotImplementedError(
+                "This model can't make forecast decomposition on history data! "
+                "Use method predict for in-sample prediction decomposition."
+            )
 
         horizon = determine_num_steps(
             start_timestamp=self._last_train_timestamp, end_timestamp=df["timestamp"].max(), freq=self._train_freq
         )
         horizon_steps = np.arange(1, horizon + 1)
 
         self._check_mul_components()
-        self._check_df(df)
 
         level = fit_result.level.values
         trend = fit_result.trend.values
         season = fit_result.season.values
 
         components = {"target_component_level": level[-1] * np.ones(horizon)}
 
@@ -400,18 +400,20 @@
         model = self._model
         fit_result = self._result
 
         if fit_result is None or model is None or self._train_freq is None:
             raise ValueError("This model is not fitted!")
 
         if df["timestamp"].min() < self._first_train_timestamp or df["timestamp"].max() > self._last_train_timestamp:
-            raise ValueError("To estimate out-of-sample prediction decomposition use `forecast` method.")
+            raise NotImplementedError(
+                "This model can't make prediction decomposition on future out-of-sample data! "
+                "Use method forecast for future out-of-sample prediction decomposition."
+            )
 
         self._check_mul_components()
-        self._check_df(df)
 
         level = fit_result.level.values
         trend = fit_result.trend.values
         season = fit_result.season.values
 
         components = {
             "target_component_level": np.concatenate([[fit_result.params["initial_level"]], level[:-1]]),
```

### Comparing `etna-2.1.0/etna/models/linear.py` & `etna-2.2.0/etna/models/linear.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/mixins.py` & `etna-2.2.0/etna/models/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,27 +626,27 @@
         """
         if not hasattr(self._base_model, "get_model"):
             raise NotImplementedError(f"get_model method is not implemented for {self._base_model.__class__.__name__}")
         return self._base_model.get_model()
 
 
 class SaveNNMixin(SaveMixin):
-    """Implementation of ``AbstractSaveable``  torch related classes.
+    """Implementation of ``AbstractSaveable`` torch related classes.
 
     It saves object to the zip archive with 2 files:
 
     * metadata.json: contains library version and class name.
 
     * object.pt: object saved by ``torch.save``.
     """
 
     def _save_state(self, archive: zipfile.ZipFile):
         import torch
 
-        with archive.open("object.pt", "w") as output_file:
+        with archive.open("object.pt", "w", force_zip64=True) as output_file:
             torch.save(self, output_file, pickle_module=dill)
 
     @classmethod
     def _load_state(cls, archive: zipfile.ZipFile) -> Self:
         import torch
 
         with archive.open("object.pt", "r") as input_file:
```

### Comparing `etna-2.1.0/etna/models/moving_average.py` & `etna-2.2.0/etna/models/moving_average.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/naive.py` & `etna-2.2.0/etna/models/naive.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/deepar.py` & `etna-2.2.0/etna/models/nn/deepar.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/deepstate/__init__.py` & `etna-2.2.0/etna/models/nn/deepstate/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/deepstate/deepstate.py` & `etna-2.2.0/etna/models/nn/deepstate/deepstate.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/deepstate/linear_dynamic_system.py` & `etna-2.2.0/etna/models/nn/deepstate/linear_dynamic_system.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/deepstate/state_space_model.py` & `etna-2.2.0/etna/models/nn/deepstate/state_space_model.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/mlp.py` & `etna-2.2.0/etna/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/rnn.py` & `etna-2.2.0/etna/models/nn/rnn.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/tft.py` & `etna-2.2.0/etna/models/nn/tft.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/models/nn/utils.py` & `etna-2.2.0/etna/models/nn/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,25 +121,24 @@
         Parameters
         ----------
         ts:
             Time series dataset.
         """
         df_flat = ts.to_pandas(flatten=True)
         df_flat = df_flat.dropna()
-        self.min_timestamp = df_flat.timestamp.min()
+
+        mapping_time_idx = {x: i for i, x in enumerate(ts.index)}
+        df_flat["time_idx"] = df_flat["timestamp"].map(mapping_time_idx)
+
+        self.min_timestamp = df_flat["timestamp"].min()
 
         if self.time_varying_known_categoricals:
             for feature_name in self.time_varying_known_categoricals:
                 df_flat[feature_name] = df_flat[feature_name].astype(str)
 
-        # making time_idx feature.
-        # it's needed for pytorch-forecasting for proper train-test split.
-        # it should be incremented by 1 for every new timestamp.
-        df_flat["time_idx"] = df_flat["timestamp"].apply(lambda x: determine_num_steps(self.min_timestamp, x, ts.freq))
-
         pf_dataset = TimeSeriesDataSet(
             df_flat,
             time_idx="time_idx",
             target="target",
             group_ids=["segment"],
             time_varying_known_reals=self.time_varying_known_reals,
             time_varying_known_categoricals=self.time_varying_known_categoricals,
@@ -188,15 +187,20 @@
                 "This method should only be called after create_train_dataset. Try to train the model that uses this builder."
             )
 
         df_flat = ts.to_pandas(flatten=True)
         df_flat = df_flat[df_flat.timestamp >= self.min_timestamp]
         df_flat["target"] = df_flat["target"].fillna(0)
 
-        df_flat["time_idx"] = df_flat["timestamp"].apply(lambda x: determine_num_steps(self.min_timestamp, x, ts.freq))
+        inference_min_timestamp = df_flat["timestamp"].min()
+        time_idx_shift = determine_num_steps(
+            start_timestamp=self.min_timestamp, end_timestamp=inference_min_timestamp, freq=ts.freq
+        )
+        mapping_time_idx = {x: i + time_idx_shift for i, x in enumerate(ts.index)}
+        df_flat["time_idx"] = df_flat["timestamp"].map(mapping_time_idx)
 
         if self.time_varying_known_categoricals:
             for feature_name in self.time_varying_known_categoricals:
                 df_flat[feature_name] = df_flat[feature_name].astype(str)
 
         # `TimeSeriesDataSet.from_parameters` in predict mode ignores `min_prediction_length`,
         # and we can change prediction size only by changing `max_prediction_length`
@@ -266,20 +270,21 @@
         first_prediction_timestamp = self._get_first_prediction_timestamp(ts=ts, horizon=horizon)
         first_timestamp_after_train = pd.date_range(self._last_train_timestamp, periods=2, freq=self._freq)[-1]
         return first_prediction_timestamp > first_timestamp_after_train
 
     def _make_target_prediction(self, ts: TSDataset, horizon: int) -> Tuple[TSDataset, DataLoader]:
         if self._is_in_sample_prediction(ts=ts, horizon=horizon):
             raise NotImplementedError(
-                "It is not possible to make in-sample predictions with DeepAR model! "
-                "In-sample predictions aren't supported by current implementation."
+                "This model can't make forecast on history data! "
+                "In-sample forecast isn't supported by current implementation."
             )
         elif self._is_prediction_with_gap(ts=ts, horizon=horizon):
             first_prediction_timestamp = self._get_first_prediction_timestamp(ts=ts, horizon=horizon)
             raise NotImplementedError(
+                "This model can't make forecast on out-of-sample data that goes after training data with a gap! "
                 "You can only forecast from the next point after the last one in the training dataset: "
                 f"last train timestamp: {self._last_train_timestamp}, first prediction timestamp is {first_prediction_timestamp}"
             )
         else:
             pass
 
         if len(ts.df) != horizon + self.encoder_length:
```

### Comparing `etna-2.1.0/etna/models/prophet.py` & `etna-2.2.0/etna/models/prophet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from copy import deepcopy
 from datetime import datetime
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
@@ -94,26 +95,69 @@
         )
 
         for seasonality_params in self.additional_seasonality_params:
             model.add_seasonality(**seasonality_params)
 
         return model
 
+    def _check_not_used_columns(self, df: pd.DataFrame):
+        if self.regressor_columns is None:
+            raise ValueError("Something went wrong, regressor_columns is None!")
+
+        columns_not_used = [col for col in df.columns if col not in ["target", "timestamp"] + self.regressor_columns]
+        if columns_not_used:
+            warnings.warn(
+                message=f"This model doesn't work with exogenous features unknown in future. "
+                f"Columns {columns_not_used} won't be used."
+            )
+
+    def _select_regressors(self, df: pd.DataFrame) -> Optional[pd.DataFrame]:
+        """Select data with regressors.
+
+        During fit there can't be regressors with NaNs, they are removed at higher level.
+        Look at the issue: https://github.com/tinkoff-ai/etna/issues/557
+
+        During prediction without validation NaNs in regressors lead to exception from the underlying model.
+
+        This model requires data to be in numeric dtype.
+        """
+        if self.regressor_columns is None:
+            raise ValueError("Something went wrong, regressor_columns is None!")
+
+        regressors_with_nans = [regressor for regressor in self.regressor_columns if df[regressor].isna().sum() > 0]
+        if regressors_with_nans:
+            raise ValueError(
+                f"Regressors {regressors_with_nans} contain NaN values. "
+                "Try to lower horizon value, or drop these regressors."
+            )
+
+        if self.regressor_columns:
+            try:
+                result = df[self.regressor_columns].apply(pd.to_numeric)
+            except ValueError as e:
+                raise ValueError(f"Only convertible to numeric features are allowed! Error: {str(e)}")
+        else:
+            result = None
+
+        return result
+
     def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_ProphetAdapter":
         """
         Fits a Prophet model.
 
         Parameters
         ----------
         df:
             Features dataframe
         regressors:
             List of the columns with regressors
         """
         self.regressor_columns = regressors
+        self._check_not_used_columns(df)
+
         prophet_df = self._prepare_prophet_df(df=df)
         for regressor in self.regressor_columns:
             if regressor not in self.predefined_regressors_names:
                 self.model.add_regressor(regressor)
         self.model.fit(prophet_df)
         return self
 
@@ -155,15 +199,19 @@
             raise ValueError("List of regressor is not set!")
 
         df = df.reset_index()
 
         prophet_df = pd.DataFrame()
         prophet_df["y"] = df["target"]
         prophet_df["ds"] = df["timestamp"]
-        prophet_df[self.regressor_columns] = df[self.regressor_columns]
+
+        regressors_data = self._select_regressors(df)
+        if regressors_data is not None:
+            prophet_df[self.regressor_columns] = regressors_data[self.regressor_columns]
+
         return prophet_df
 
     @staticmethod
     def _filter_aggregated_components(components: Iterable[str]) -> Set[str]:
         """Filter out aggregated components."""
         # aggregation of corresponding model terms, e.g. sum
         aggregated_components = {
```

### Comparing `etna-2.1.0/etna/models/sarimax.py` & `etna-2.2.0/etna/models/sarimax.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 
         Returns
         -------
         :
             Fitted model
         """
         self.regressor_columns = regressors
-
-        self._encode_categoricals(df)
-        self._check_df(df)
+        self._check_not_used_columns(df)
 
         exog_train = self._select_regressors(df)
         self._fit_results = self._get_fit_results(endog=df["target"], exog=exog_train)
 
         self._freq = determine_freq(timestamps=df["timestamp"])
         self._first_train_timestamp = df["timestamp"].min()
         self._last_train_timestamp = df["timestamp"].max()
@@ -77,19 +75,16 @@
     def _make_prediction(
         self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float], dynamic: bool
     ) -> pd.DataFrame:
         """Make predictions taking into account ``dynamic`` parameter."""
         if self._fit_results is None:
             raise ValueError("Model is not fitted! Fit the model before calling predict method!")
 
-        horizon = len(df)
-        self._encode_categoricals(df)
-        self._check_df(df, horizon)
-
         exog_future = self._select_regressors(df)
+
         start_timestamp = df["timestamp"].min()
         end_timestamp = df["timestamp"].max()
         # determine index of start_timestamp if counting from first timestamp of train
         start_idx = determine_num_steps(
             start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
         )
         # determine index of end_timestamp if counting from first timestamp of train
@@ -170,49 +165,56 @@
         """
         return self._make_prediction(df=df, prediction_interval=prediction_interval, quantiles=quantiles, dynamic=False)
 
     @abstractmethod
     def _get_fit_results(self, endog: pd.Series, exog: pd.DataFrame) -> SARIMAXResultsWrapper:
         pass
 
-    def _check_df(self, df: pd.DataFrame, horizon: Optional[int] = None):
+    def _check_not_used_columns(self, df: pd.DataFrame):
         if self.regressor_columns is None:
             raise ValueError("Something went wrong, regressor_columns is None!")
-        column_to_drop = [col for col in df.columns if col not in ["target", "timestamp"] + self.regressor_columns]
-        if column_to_drop:
+
+        columns_not_used = [col for col in df.columns if col not in ["target", "timestamp"] + self.regressor_columns]
+        if columns_not_used:
             warnings.warn(
-                message=f"SARIMAX model does not work with exogenous features (features unknown in future).\n "
-                f"{column_to_drop} will be dropped"
+                message=f"This model doesn't work with exogenous features unknown in future. "
+                f"Columns {columns_not_used} won't be used."
             )
-        if horizon:
-            short_regressors = [regressor for regressor in self.regressor_columns if df[regressor].count() < horizon]
-            if short_regressors:
-                raise ValueError(
-                    f"Regressors {short_regressors} are too short for chosen horizon value.\n "
-                    "Try lower horizon value, or drop this regressors."
-                )
 
     def _select_regressors(self, df: pd.DataFrame) -> Optional[pd.DataFrame]:
-        if self.regressor_columns:
-            exog_future = df[self.regressor_columns]
-            exog_future.index = df["timestamp"]
-        else:
-            exog_future = None
-        return exog_future
+        """Select data with regressors.
+
+        During fit there can't be regressors with NaNs, they are removed at higher level.
+        Look at the issue: https://github.com/tinkoff-ai/etna/issues/557
+
+        During prediction without validation NaNs in regressors lead to exception from the underlying model.
 
-    def _encode_categoricals(self, df: pd.DataFrame) -> None:
-        categorical_cols = df.select_dtypes(include=["category"]).columns.tolist()
-        try:
-            df.loc[:, categorical_cols] = df[categorical_cols].astype(int)
-        except ValueError:
+        This model requires data to be in numeric dtype, but doesn't support boolean, so it was decided to use float.
+        """
+        if self.regressor_columns is None:
+            raise ValueError("Something went wrong, regressor_columns is None!")
+
+        regressors_with_nans = [regressor for regressor in self.regressor_columns if df[regressor].isna().sum() > 0]
+        if regressors_with_nans:
             raise ValueError(
-                f"Categorical columns {categorical_cols} can not been converted to int.\n "
-                "Try to encode this columns manually."
+                f"Regressors {regressors_with_nans} contain NaN values. "
+                "Try to lower horizon value, or drop these regressors."
             )
 
+        if self.regressor_columns:
+            try:
+                result = df[self.regressor_columns].astype(float)
+            except ValueError as e:
+                raise ValueError(f"Only convertible to float features are allowed! Error: {str(e)}")
+            result.index = df["timestamp"]
+        else:
+            result = None
+
+        return result
+
     def get_model(self) -> SARIMAXResultsWrapper:
         """Get :py:class:`statsmodels.tsa.statespace.sarimax.SARIMAXResultsWrapper` that is used inside etna class.
 
         Returns
         -------
         :
            Internal model
@@ -299,22 +301,30 @@
             features dataframe
 
         Returns
         -------
         :
             dataframe with prediction components
         """
-        if df["timestamp"].min() < self._first_train_timestamp or df["timestamp"].max() > self._last_train_timestamp:
-            raise ValueError("To estimate out-of-sample prediction decomposition use `forecast` method.")
+        if self._fit_results is None:
+            raise ValueError("Model is not fitted! Fit the model before estimating forecast components!")
+
+        if self._last_train_timestamp < df["timestamp"].max() or self._first_train_timestamp > df["timestamp"].min():
+            raise NotImplementedError(
+                "This model can't make prediction decomposition on future out-of-sample data! "
+                "Use method forecast for future out-of-sample prediction decomposition."
+            )
 
         fit_results = self._fit_results
         model = fit_results.model
 
         if model.hamilton_representation:
-            raise ValueError("Prediction decomposition is not implemented for Hamilton representation of ARMA!")
+            raise NotImplementedError(
+                "Prediction decomposition is not implemented for Hamilton representation of ARMA!"
+            )
 
         state = fit_results.predicted_state[:, :-1]
 
         if model.mle_regression:
             components = self._mle_regression_decomposition(state=state, ssm=model.ssm, exog=model.exog)
 
         else:
@@ -341,29 +351,49 @@
             features dataframe
 
         Returns
         -------
         :
             dataframe with forecast components
         """
-        if df["timestamp"].min() <= self._last_train_timestamp:
-            raise ValueError("To estimate in-sample prediction decomposition use `predict` method.")
+        if self._fit_results is None:
+            raise ValueError("Model is not fitted! Fit the model before estimating forecast components!")
 
-        horizon = determine_num_steps(
-            start_timestamp=self._last_train_timestamp, end_timestamp=df["timestamp"].max(), freq=self._freq
+        start_timestamp = df["timestamp"].min()
+        end_timestamp = df["timestamp"].max()
+
+        if start_timestamp < self._last_train_timestamp:
+            raise NotImplementedError(
+                "This model can't make forecast decomposition on history data! "
+                "Use method predict for in-sample prediction decomposition."
+            )
+
+        # determine index of start_timestamp if counting from last timestamp of train
+        start_idx = determine_num_steps(
+            start_timestamp=self._last_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
+        )
+        # determine index of end_timestamp if counting from last timestamp of train
+        end_idx = determine_num_steps(
+            start_timestamp=self._last_train_timestamp, end_timestamp=end_timestamp, freq=self._freq  # type: ignore
         )
 
+        if start_idx > 1:
+            raise NotImplementedError(
+                "This model can't make forecast decomposition on out-of-sample data that goes after training data with a gap! "
+                "You can only forecast from the next point after the last one in the training dataset."
+            )
+
+        horizon = end_idx
         fit_results = self._fit_results
 
         model = fit_results.model
         if model.hamilton_representation:
-            raise ValueError("Prediction decomposition is not implemented for Hamilton representation of ARMA!")
-
-        self._encode_categoricals(df)
-        self._check_df(df, horizon)
+            raise NotImplementedError(
+                "Prediction decomposition is not implemented for Hamilton representation of ARMA!"
+            )
 
         exog_future = self._select_regressors(df)
 
         forecast_results = fit_results.get_forecast(horizon, exog=exog_future).prediction_results.results
         state = forecast_results.predicted_state[:, :-1]
 
         if model.mle_regression:
@@ -385,15 +415,15 @@
         )
 
         return components_df
 
 
 class _SARIMAXAdapter(_SARIMAXBaseAdapter):
     """
-    Class for holding Sarimax model.
+    Class for holding SARIMAX model.
 
     Notes
     -----
     We use SARIMAX [1] model from statsmodels package. Statsmodels package uses `exog` attribute for
     `exogenous regressors` which should be known in future, however we use exogenous for
     additional features what is not known in future, and regressors for features we do know in
     future.
@@ -505,14 +535,16 @@
             time-series may be specified here as a Pandas offset or offset string.
         missing:
             Available options are 'none', 'drop', and 'raise'. If 'none', no nan
             checking is done. If 'drop', any observations with nans are dropped.
             If 'raise', an error is raised. Default is 'none'.
         validate_specification:
             If True, validation of hyperparameters is performed.
+        **kwargs:
+            Additional parameters for :py:class:`statsmodels.tsa.sarimax.SARIMAX`.
         """
         self.order = order
         self.seasonal_order = seasonal_order
         self.trend = trend
         self.measurement_error = measurement_error
         self.time_varying_regression = time_varying_regression
         self.mle_regression = mle_regression
@@ -559,15 +591,15 @@
         return result
 
 
 class SARIMAXModel(
     PerSegmentModelMixin, PredictionIntervalContextIgnorantModelMixin, PredictionIntervalContextIgnorantAbstractModel
 ):
     """
-    Class for holding Sarimax model.
+    Class for holding SARIMAX model.
 
     Method ``predict`` can use true target values only on train data on future data autoregression
     forecasting will be made even if targets are known.
 
     Notes
     -----
     We use :py:class:`statsmodels.tsa.sarimax.SARIMAX`. Statsmodels package uses `exog` attribute for
@@ -683,14 +715,16 @@
             time-series may be specified here as a Pandas offset or offset string.
         missing:
             Available options are 'none', 'drop', and 'raise'. If 'none', no nan
             checking is done. If 'drop', any observations with nans are dropped.
             If 'raise', an error is raised. Default is 'none'.
         validate_specification:
             If True, validation of hyperparameters is performed.
+        **kwargs:
+            Additional parameters for :py:class:`statsmodels.tsa.sarimax.SARIMAX`.
         """
         self.order = order
         self.seasonal_order = seasonal_order
         self.trend = trend
         self.measurement_error = measurement_error
         self.time_varying_regression = time_varying_regression
         self.mle_regression = mle_regression
```

### Comparing `etna-2.1.0/etna/models/seasonal_ma.py` & `etna-2.2.0/etna/models/seasonal_ma.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,23 @@
         Returns
         -------
         :
            Itself
         """
         return self
 
+    def _check_not_used_columns(self, ts: TSDataset):
+        columns = set(ts.columns.get_level_values("feature"))
+        columns_not_used = columns.difference({"target"})
+        if columns_not_used:
+            warnings.warn(
+                message=f"This model doesn't work with exogenous features. "
+                f"Columns {columns_not_used} won't be used."
+            )
+
     def fit(self, ts: TSDataset) -> "SeasonalMovingAverageModel":
         """Fit model.
 
         For this model, fit does nothing.
 
         Parameters
         ----------
@@ -68,20 +77,15 @@
             Dataset with features
 
         Returns
         -------
         :
             Model after fit
         """
-        columns = set(ts.columns.get_level_values("feature"))
-        if columns != {"target"}:
-            warnings.warn(
-                message=f"{type(self).__name__} does not work with any exogenous series or features. "
-                f"It uses only target series for predict/\n "
-            )
+        self._check_not_used_columns(ts)
         return self
 
     def _validate_context(self, df: pd.DataFrame, prediction_size: int):
         """Validate that we have enough context to make prediction with given parameters."""
         expected_length = prediction_size + self.context_size
 
         if len(df) < expected_length:
```

### Comparing `etna-2.1.0/etna/models/sklearn.py` & `etna-2.2.0/etna/models/sklearn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from sklearn.base import RegressorMixin
 
@@ -13,14 +14,49 @@
 
 
 class _SklearnAdapter(BaseAdapter):
     def __init__(self, regressor: RegressorMixin):
         self.model = regressor
         self.regressor_columns: Optional[List[str]] = None
 
+    def _check_not_used_columns(self, df: pd.DataFrame):
+        if self.regressor_columns is None:
+            raise ValueError("Something went wrong, regressor_columns is None!")
+
+        columns_not_used = [col for col in df.columns if col not in ["target", "timestamp"] + self.regressor_columns]
+        if columns_not_used:
+            warnings.warn(
+                message=f"This model doesn't work with exogenous features unknown in future. "
+                f"Columns {columns_not_used} won't be used."
+            )
+
+    def _select_regressors(self, df: pd.DataFrame) -> Optional[pd.DataFrame]:
+        """Select data with regressors.
+
+        During fit there can't be regressors with NaNs, they are removed at higher level.
+        Look at the issue: https://github.com/tinkoff-ai/etna/issues/557
+
+        During prediction without validation NaNs in regressors can lead to exception from the underlying model,
+        but it depends on the model, so it was decided to not validate this.
+
+        This model requires data to be in numeric dtype.
+        """
+        if self.regressor_columns is None:
+            raise ValueError("Something went wrong, regressor_columns is None!")
+
+        if self.regressor_columns:
+            try:
+                result = df[self.regressor_columns].apply(pd.to_numeric)
+            except ValueError as e:
+                raise ValueError(f"Only convertible to numeric features are allowed! Error: {str(e)}")
+        else:
+            raise ValueError("There are not features for fitting the model!")
+
+        return result
+
     def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_SklearnAdapter":
         """
         Fit Sklearn model.
 
         Parameters
         ----------
         df:
@@ -30,18 +66,16 @@
 
         Returns
         -------
         :
             Fitted model
         """
         self.regressor_columns = regressors
-        try:
-            features = df[self.regressor_columns].apply(pd.to_numeric)
-        except ValueError:
-            raise ValueError("Only convertible to numeric features are accepted!")
+        self._check_not_used_columns(df)
+        features = self._select_regressors(df)
         target = df["target"]
         self.model.fit(features, target)
         return self
 
     def predict(self, df: pd.DataFrame) -> np.ndarray:
         """
         Compute predictions from a Sklearn model.
@@ -52,18 +86,15 @@
             Features dataframe
 
         Returns
         -------
         :
             Array with predictions
         """
-        try:
-            features = df[self.regressor_columns].apply(pd.to_numeric)
-        except ValueError:
-            raise ValueError("Only convertible to numeric features are accepted!")
+        features = self._select_regressors(df)
         pred = self.model.predict(features)
         return pred
 
     def predict_components(self, df: pd.DataFrame) -> pd.DataFrame:
         """Estimate prediction components.
 
         Parameters
```

### Comparing `etna-2.1.0/etna/models/tbats.py` & `etna-2.2.0/etna/models/tbats.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,26 @@
     def __init__(self, model: Estimator):
         self._model = model
         self._fitted_model: Optional[Model] = None
         self._first_train_timestamp = None
         self._last_train_timestamp = None
         self._freq: Optional[str] = None
 
+    def _check_not_used_columns(self, df: pd.DataFrame):
+        columns = df.columns
+        columns_not_used = set(columns).difference({"target", "timestamp"})
+        if columns_not_used:
+            warn(
+                message=f"This model doesn't work with exogenous features. "
+                f"Columns {columns_not_used} won't be used."
+            )
+
     def fit(self, df: pd.DataFrame, regressors: Iterable[str]):
         self._freq = determine_freq(timestamps=df["timestamp"])
+        self._check_not_used_columns(df)
 
         target = df["target"]
         self._fitted_model = self._model.fit(target)
         self._first_train_timestamp = df["timestamp"].min()
         self._last_train_timestamp = df["timestamp"].max()
 
         return self
@@ -70,15 +80,18 @@
             raise ValueError("Model is not fitted! Fit the model before calling predict method!")
 
         train_timestamp = pd.date_range(
             start=str(self._first_train_timestamp), end=str(self._last_train_timestamp), freq=self._freq
         )
 
         if not (set(df["timestamp"]) <= set(train_timestamp)):
-            raise NotImplementedError("Method predict isn't currently implemented for out-of-sample prediction!")
+            raise NotImplementedError(
+                "This model can't make predict on future out-of-sample data! "
+                "Use forecast method for this type of prediction."
+            )
 
         y_pred = pd.DataFrame()
         y_pred["target"] = self._fitted_model.y_hat
         y_pred["timestamp"] = train_timestamp
 
         if prediction_interval:
             for quantile in quantiles:
@@ -121,15 +134,18 @@
         :
             dataframe with forecast components
         """
         if self._fitted_model is None or self._freq is None:
             raise ValueError("Model is not fitted! Fit the model before estimating forecast components!")
 
         if df["timestamp"].min() <= self._last_train_timestamp:
-            raise ValueError("To estimate in-sample prediction decomposition use `predict` method.")
+            raise NotImplementedError(
+                "This model can't make forecast decomposition on history data! "
+                "Use method predict for in-sample prediction decomposition."
+            )
 
         self._check_components()
 
         horizon = self._get_steps_to_forecast(df=df)
         raw_components = self._decompose_forecast(horizon=horizon)
         components = self._process_components(raw_components=raw_components)
 
@@ -152,15 +168,18 @@
         :
             dataframe with prediction components
         """
         if self._fitted_model is None or self._freq is None:
             raise ValueError("Model is not fitted! Fit the model before estimating forecast components!")
 
         if self._last_train_timestamp < df["timestamp"].max() or self._first_train_timestamp > df["timestamp"].min():
-            raise ValueError("To estimate out-of-sample prediction decomposition use `forecast` method.")
+            raise NotImplementedError(
+                "This model can't make prediction decomposition on future out-of-sample data! "
+                "Use method forecast for future out-of-sample prediction decomposition."
+            )
 
         self._check_components()
 
         raw_components = self._decompose_predict()
         components = self._process_components(raw_components=raw_components)
 
         components = select_observations(
@@ -175,15 +194,15 @@
 
     def _get_steps_to_forecast(self, df: pd.DataFrame) -> int:
         if self._freq is None:
             raise ValueError("Data frequency is not set!")
 
         if df["timestamp"].min() <= self._last_train_timestamp:
             raise NotImplementedError(
-                "It is not possible to make in-sample predictions using current method implementation!"
+                "This model can't make forecast on history data! Use method predict for in-sample prediction."
             )
 
         steps_to_forecast = determine_num_steps(
             start_timestamp=self._last_train_timestamp, end_timestamp=df["timestamp"].max(), freq=self._freq
         )
         return steps_to_forecast
```

### Comparing `etna-2.1.0/etna/models/utils.py` & `etna-2.2.0/etna/models/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/pipeline/assembling_pipelines.py` & `etna-2.2.0/etna/pipeline/assembling_pipelines.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/pipeline/autoregressive_pipeline.py` & `etna-2.2.0/etna/pipeline/autoregressive_pipeline.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/pipeline/base.py` & `etna-2.2.0/etna/pipeline/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from etna.core import AbstractSaveable
 from etna.core import BaseMixin
 from etna.datasets import TSDataset
 from etna.distributions import BaseDistribution
 from etna.loggers import tslogger
 from etna.metrics import Metric
 from etna.metrics import MetricAggregationMode
+from etna.metrics.functional_metrics import ArrayLike
 
 Timestamp = Union[str, pd.Timestamp]
 
 
 class CrossValidationMode(str, Enum):
     """Enum for different cross-validation modes."""
 
@@ -297,15 +298,15 @@
 class _DummyMetric(Metric):
     """Dummy metric that is created only for implementation of BasePipeline._forecast_prediction_interval."""
 
     def __init__(self, mode: str = MetricAggregationMode.per_segment, **kwargs):
         super().__init__(mode=mode, metric_fn=self._compute_metric, **kwargs)
 
     @staticmethod
-    def _compute_metric(y_true: np.ndarray, y_pred: np.ndarray) -> float:
+    def _compute_metric(y_true: ArrayLike, y_pred: ArrayLike) -> float:
         return 0.0
 
     @property
     def greater_is_better(self) -> bool:
         return False
 
     def __call__(self, y_true: TSDataset, y_pred: TSDataset) -> Union[float, Dict[str, float]]:
```

### Comparing `etna-2.1.0/etna/pipeline/hierarchical_pipeline.py` & `etna-2.2.0/etna/pipeline/hierarchical_pipeline.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/pipeline/mixins.py` & `etna-2.2.0/etna/pipeline/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,16 @@
                 prediction_size=prediction_size,
                 prediction_interval=prediction_interval,
                 quantiles=quantiles,
                 return_components=return_components,
             )
         else:
             raise NotImplementedError(f"Unknown model type: {self.model.__class__.__name__}!")
+
+        results.inverse_transform(self.transforms)
         return results
 
 
 class ModelPipelineParamsToTuneMixin:
     """Mixin for pipelines with model inside with implementation of ``params_to_tune`` method."""
 
     model: ModelType
@@ -201,14 +203,20 @@
                     transform.save(transform_save_path)
                     archive.write(transform_save_path, f"transforms/{save_name}")
 
     @classmethod
     def load(cls, path: pathlib.Path, ts: Optional[TSDataset] = None) -> Self:
         """Load an object.
 
+        Warning
+        -------
+        This method uses :py:mod:`dill` module which is not secure.
+        It is possible to construct malicious data which will execute arbitrary code during loading.
+        Never load data that could have come from an untrusted source, or that could have been tampered with.
+
         Parameters
         ----------
         path:
             Path to load object from.
         ts:
             TSDataset to set into loaded pipeline.
```

### Comparing `etna-2.1.0/etna/pipeline/pipeline.py` & `etna-2.2.0/etna/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/reconciliation/base.py` & `etna-2.2.0/etna/reconciliation/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/reconciliation/bottom_up.py` & `etna-2.2.0/etna/reconciliation/bottom_up.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/reconciliation/top_down.py` & `etna-2.2.0/etna/reconciliation/top_down.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/settings.py` & `etna-2.2.0/etna/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -68,14 +68,22 @@
     if true_case:
         return True
     else:
         warnings.warn("etna[auto] is not available, to install it, run `pip install etna[auto]`")
         return False
 
 
+def _is_statsforecast_available():
+    if _module_available("statsforecast"):
+        return True
+    else:
+        warnings.warn("etna[statsforecast] is not available, to install it, run `pip install etna[statsforecast]`")
+        return False
+
+
 def _get_optional_value(is_required: Optional[bool], is_available_fn: Callable, assert_msg: str) -> bool:
     if is_required is None:
         return is_available_fn()
     elif is_required:
         if not is_available_fn():
             raise ImportError(assert_msg)
         return True
@@ -89,14 +97,15 @@
     def __init__(  # noqa: D107
         self,
         torch_required: Optional[bool] = None,
         prophet_required: Optional[bool] = None,
         wandb_required: Optional[bool] = None,
         classification_required: Optional[bool] = None,
         auto_required: Optional[bool] = None,
+        statsforecast_required: Optional[bool] = None,
     ):
         # True – use the package
         # None – use the package if available
         # False - block the package
         self.torch_required: bool = _get_optional_value(
             torch_required,
             _is_torch_available,
@@ -116,14 +125,19 @@
             "etna[classification] is not available, to install it, run `pip install etna[classification]`.",
         )
         self.auto_required: bool = _get_optional_value(
             auto_required,
             _is_auto_available,
             "etna[auto] is not available, to install it, run `pip install etna[auto]`.",
         )
+        self.statsforecast_required: bool = _get_optional_value(
+            statsforecast_required,
+            _is_statsforecast_available,
+            "etna[statsforecast] is not available, to install it, run `pip install etna[statsforecast]`.",
+        )
 
     @staticmethod
     def parse() -> "Settings":
         """Parse and return the settings.
 
         Returns
         -------
```

### Comparing `etna-2.1.0/etna/transforms/__init__.py` & `etna-2.2.0/etna/transforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from etna.transforms.base import ReversiblePerSegmentWrapper
 from etna.transforms.base import ReversibleTransform
 from etna.transforms.base import Transform
 from etna.transforms.decomposition import BaseChangePointsTransform
 from etna.transforms.decomposition import ChangePointsLevelTransform
 from etna.transforms.decomposition import ChangePointsSegmentationTransform
 from etna.transforms.decomposition import ChangePointsTrendTransform
+from etna.transforms.decomposition import DeseasonalityTransform
 from etna.transforms.decomposition import IrreversibleChangePointsTransform
 from etna.transforms.decomposition import LinearTrendTransform
 from etna.transforms.decomposition import ReversibleChangePointsTransform
 from etna.transforms.decomposition import STLTransform
 from etna.transforms.decomposition import TheilSenTrendTransform
 from etna.transforms.decomposition import TrendTransform
 from etna.transforms.encoders import LabelEncoderTransform
```

### Comparing `etna-2.1.0/etna/transforms/base.py` & `etna-2.2.0/etna/transforms/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/__init__.py` & `etna-2.2.0/etna/transforms/decomposition/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,10 +4,11 @@
 from etna.transforms.decomposition.change_points_based.base import BaseChangePointsTransform
 from etna.transforms.decomposition.change_points_based.base import IrreversibleChangePointsTransform
 from etna.transforms.decomposition.change_points_based.base import ReversibleChangePointsTransform
 from etna.transforms.decomposition.change_points_based.change_points_models import BaseChangePointsModelAdapter
 from etna.transforms.decomposition.change_points_based.change_points_models import RupturesChangePointsModel
 from etna.transforms.decomposition.change_points_based.level import ChangePointsLevelTransform
 from etna.transforms.decomposition.change_points_based.trend import TrendTransform
+from etna.transforms.decomposition.deseasonal import DeseasonalityTransform
 from etna.transforms.decomposition.detrend import LinearTrendTransform
 from etna.transforms.decomposition.detrend import TheilSenTrendTransform
 from etna.transforms.decomposition.stl import STLTransform
```

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/__init__.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/base.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/detrend.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/detrend.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/level.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/level.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/segmentation.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/segmentation.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/change_points_based/trend.py` & `etna-2.2.0/etna/transforms/decomposition/change_points_based/trend.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/detrend.py` & `etna-2.2.0/etna/transforms/decomposition/detrend.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/decomposition/stl.py` & `etna-2.2.0/etna/transforms/decomposition/stl.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/encoders/categorical.py` & `etna-2.2.0/etna/transforms/encoders/categorical.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/encoders/mean_segment_encoder.py` & `etna-2.2.0/etna/transforms/encoders/mean_segment_encoder.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/encoders/segment_encoder.py` & `etna-2.2.0/etna/transforms/encoders/segment_encoder.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/feature_selection/base.py` & `etna-2.2.0/etna/transforms/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/feature_selection/feature_importance.py` & `etna-2.2.0/etna/transforms/feature_selection/feature_importance.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/feature_selection/filter.py` & `etna-2.2.0/etna/transforms/feature_selection/filter.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/feature_selection/gale_shapley.py` & `etna-2.2.0/etna/transforms/feature_selection/gale_shapley.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.last_candidate = self.tmp_match_rank
 
     def get_next_candidate(self) -> Optional[str]:
         """Get name of the next feature to try.
 
         Returns
         -------
-        name: str
+        name:
             name of feature
         """
         if self.last_candidate is None:
             self.last_candidate = 0
         else:
             self.last_candidate += 1
 
@@ -109,15 +109,15 @@
         Parameters
         ----------
         segment:
             segment to check
 
         Returns
         -------
-        is_better: bool
+        is_better:
             returns True if given segment is a better candidate than current match.
         """
         if self.tmp_match is None or self.tmp_match_rank is None:
             return True
         return self.candidates_rank[segment] < self.tmp_match_rank
 
 
@@ -174,15 +174,15 @@
         Parameters
         ----------
         available_segments:
             list of segments that have no match at this iteration
 
         Returns
         -------
-        success: bool
+        success:
             True if there is at least one match attempt at the iteration
 
         Notes
         -----
         Success code is necessary because in ETNA usage we can not guarantee that number of features will be
         big enough to build matches with all the segments. In case ``n_features < n_segments`` some segments always stay
         available that can cause infinite while loop in ``__call__``.
@@ -208,33 +208,43 @@
         return [segment for segment in self.segments if segment.is_available]
 
     def __call__(self) -> Dict[str, str]:
         """Run matching.
 
         Returns
         -------
-        matching: Dict[str, str]
+        matching:
             matching dict of segment x feature
         """
         success_run = True
         available_segments = self._get_available_segments()
         while available_segments and success_run:
             success_run = self._gale_shapley_iteration(available_segments=available_segments)
             available_segments = self._get_available_segments()
         return {segment.name: segment.tmp_match for segment in self.segments if segment.tmp_match is not None}
 
 
 class GaleShapleyFeatureSelectionTransform(BaseFeatureSelectionTransform):
-    """GaleShapleyFeatureSelectionTransform provides feature filtering with Gale-Shapley matching algo according to relevance table.
-
+    """Transform that provides feature filtering by Gale-Shapley matching algorithm according to the relevance table.
 
     Notes
     -----
     Transform works with any type of features, however most of the models works only with regressors.
     Therefore, it is recommended to pass the regressors into the feature selection transforms.
+
+    As input, we have a table of relevances with size :math:`N\_{f} \times N\_{s}` where :math:`N\_{f}` -- number of features,
+    :math:`N\_{s}` -- number of segments.
+    Procedure of filtering features consist of :math:`\lceil \frac{k}{N\_{s}} \rceil` iterations.
+    Algorithm of each iteration:
+
+    - build a matching between segments and features by `Gale–Shapley algorithm <https://en.wikipedia.org/wiki/Gale%E2%80%93Shapley_algorithm>`_
+    according to the relevance table, during the matching segments send proposals to features;
+    - select features to add by taking matched feature for each segment;
+    - add selected features to accumulated list of selected features taking into account that this list shouldn't exceed the size of ``top_k``;
+    - remove added features from future consideration.
     """
 
     def __init__(
         self,
         relevance_table: RelevanceTable,
         top_k: int,
         features_to_use: Union[List[str], Literal["all"]] = "all",
@@ -286,15 +296,16 @@
         if n_features < top_k:
             warnings.warn(
                 f"Given top_k={top_k} is bigger than n_features={n_features}. " f"Transform will not filter features."
             )
             return 1
         if top_k < n_segments:
             warnings.warn(
-                f"Given top_k={top_k} is less than n_segments. Algo will filter data without Gale-Shapley run."
+                f"Given top_k={top_k} is less than n_segments={n_segments}. "
+                f"Algo will filter data without Gale-Shapley run."
             )
             return 1
         return ceil(top_k / n_segments)
 
     @staticmethod
     def _gale_shapley_iteration(
         segment_features_ranking: Dict[str, List[str]],
@@ -305,15 +316,15 @@
         Parameters
         ----------
         segment_features_ranking:
             dict of relevance segment x sorted features
 
         Returns
         -------
-        matching dict: Dict[str, str]
+        matching dict:
             dict of segment x feature
         """
         gssegments = [
             SegmentGaleShapley(
                 name=name,
                 ranked_candidates=ranked_candidates,
             )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `etna-2.1.0/etna/transforms/math/__init__.py` & `etna-2.2.0/etna/transforms/math/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/add_constant.py` & `etna-2.2.0/etna/transforms/math/add_constant.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/apply_lambda.py` & `etna-2.2.0/etna/transforms/math/apply_lambda.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/differencing.py` & `etna-2.2.0/etna/transforms/math/differencing.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/lags.py` & `etna-2.2.0/etna/transforms/math/lags.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/log.py` & `etna-2.2.0/etna/transforms/math/log.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/power.py` & `etna-2.2.0/etna/transforms/math/power.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/scalers.py` & `etna-2.2.0/etna/transforms/math/scalers.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/sklearn.py` & `etna-2.2.0/etna/transforms/math/sklearn.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/math/statistics.py` & `etna-2.2.0/etna/transforms/math/statistics.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/missing_values/imputation.py` & `etna-2.2.0/etna/transforms/missing_values/imputation.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/missing_values/resample.py` & `etna-2.2.0/etna/transforms/missing_values/resample.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/outliers/base.py` & `etna-2.2.0/etna/transforms/outliers/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/outliers/point_outliers.py` & `etna-2.2.0/etna/transforms/outliers/point_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/timestamp/date_flags.py` & `etna-2.2.0/etna/transforms/timestamp/date_flags.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/timestamp/fourier.py` & `etna-2.2.0/etna/transforms/timestamp/fourier.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/timestamp/special_days.py` & `etna-2.2.0/etna/transforms/timestamp/special_days.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/timestamp/time_flags.py` & `etna-2.2.0/etna/transforms/timestamp/time_flags.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/etna/transforms/utils.py` & `etna-2.2.0/etna/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.1.0/pyproject.toml` & `etna-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "etna"
-version = "2.1.0"
+version = "2.2.0"
 repository = "https://github.com/tinkoff-ai/etna"
 readme = "README.md"
 description = "ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun."
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -42,15 +42,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.11.0"
 scikit-learn = ">=0.24, <2"
 pandas = "^1.1"
 catboost = ">=0.21"
 ruptures = "^1.1.5"
-numba = ">=0.53.1,<0.56.0"
+numba = ">=0.53.1"
 seaborn = "^0.11.1"
 statsmodels = ">=0.12,<0.14"
 pmdarima = ">=1.8.0"
 dill = "^0.3.4"
 toml = "^0.10.2"
 loguru = "^0.5.3"
 hydra-slayer = "^0.2.0"
@@ -78,14 +78,16 @@
 pytorch-lightning = {version = "*", optional = true}
 
 wandb = {version = "^0.12.2", optional = true}
 
 optuna = {version = ">=2.5.0,<3.0.0", optional = true}
 sqlalchemy = {version = "^1.1.0", optional = true}
 
+statsforecast = {version = "1.4", optional = true}
+
 sphinx-mathjax-offline = {version = "^0.0.1", optional = true}
 nbsphinx = {version = "^0.8.2", optional = true}
 Sphinx = {version = "^4.1", optional = true}
 numpydoc = {version = "^1.1.0", optional = true}
 sphinx-rtd-theme = {version = "^0.5.1", optional = true}
 myst-parser = {version = "^0.15.0", optional = true}
 GitPython = {version = "^3.1.20", optional = true}
@@ -119,41 +121,44 @@
 [tool.poetry.extras]
 # optional deps
 prophet = ["prophet"]
 torch = ["torch", "pytorch-forecasting", "pytorch-lightning"]
 wandb = ["wandb"]
 auto = ["optuna", "sqlalchemy"]
 classification = ["pyts", "tsfresh"]
+statsforecast = ["statsforecast"]
 # dev deps
 release = ["click", "semver"]
 docs = ["Sphinx", "numpydoc", "sphinx-rtd-theme", "nbsphinx", "sphinx-mathjax-offline", "myst-parser", "GitPython"]
 tests = ["pytest-cov", "coverage", "pytest"]
 jupyter = ["jupyter", "nbconvert", "black"]
 style = ["black", "isort", "flake8", "pep8-naming", "flake8-docstrings", "mypy", "types-PyYAML", "codespell", "flake8-bugbear", "flake8-comprehensions", "types-setuptools"]
 
 all = [
     "prophet",
     "torch", "pytorch-forecasting", "pytorch-lightning",
     "wandb",
     "optuna", "sqlalchemy",
-    "pyts", "tsfresh"
+    "pyts", "tsfresh",
+    "statsforecast"
 ]
 
 all-dev = [
     "prophet",
     "torch", "pytorch-forecasting", "pytorch-lightning",
     "wandb",
     "optuna", "sqlalchemy",
     "click", "semver",
     "Sphinx", "numpydoc", "sphinx-rtd-theme", "nbsphinx", "sphinx-mathjax-offline", "myst-parser", "GitPython",
     "pytest-cov", "coverage", "pytest",
     "black", "isort", "flake8", "pep8-naming", "flake8-docstrings", "mypy", "types-PyYAML", "codespell", "flake8-bugbear", "flake8-comprehensions", "types-setuptools",
     "click", "semver",
     "jupyter", "nbconvert",
-    "pyts", "tsfresh"
+    "pyts", "tsfresh",
+    "statsforecast"
 ]
 
 [tool.poetry.scripts]
 etna = "etna.commands.__main__:app"
 
 [tool.black]
 line-length = 120
```

### Comparing `etna-2.1.0/PKG-INFO` & `etna-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etna
-Version: 2.1.0
+Version: 2.2.0
 Summary: ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun.
 Home-page: https://github.com/tinkoff-ai/etna
 License: Apache-2.0
 Author: Andrey Alekseev
 Author-email: ilekseev@gmail.com
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,14 +25,15 @@
 Provides-Extra: all-dev
 Provides-Extra: auto
 Provides-Extra: classification
 Provides-Extra: docs
 Provides-Extra: jupyter
 Provides-Extra: prophet
 Provides-Extra: release
+Provides-Extra: statsforecast
 Provides-Extra: style
 Provides-Extra: tests
 Provides-Extra: torch
 Provides-Extra: wandb
 Requires-Dist: Bottleneck (>=1.3.4,<2.0.0)
 Requires-Dist: Deprecated (==1.2.13)
 Requires-Dist: GitPython (>=3.1.20,<4.0.0) ; extra == "docs" or extra == "all-dev"
@@ -58,15 +59,15 @@
 Requires-Dist: jupyter ; extra == "jupyter" or extra == "all-dev"
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: matplotlib
 Requires-Dist: mypy (>=0.950,<2) ; extra == "style" or extra == "all-dev"
 Requires-Dist: myst-parser (>=0.15.0,<0.16.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: nbconvert ; extra == "jupyter" or extra == "all-dev"
 Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs" or extra == "all-dev"
-Requires-Dist: numba (>=0.53.1,<0.56.0)
+Requires-Dist: numba (>=0.53.1)
 Requires-Dist: numpy
 Requires-Dist: numpydoc (>=1.1.0,<2.0.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: omegaconf (>=2.1.1,<3.0.0)
 Requires-Dist: optuna (>=2.5.0,<3.0.0) ; extra == "auto" or extra == "all" or extra == "all-dev"
 Requires-Dist: pandas (>=1.1,<2.0)
 Requires-Dist: pep8-naming (>=0.12.1,<0.13.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: plotly
@@ -81,14 +82,15 @@
 Requires-Dist: scikit-learn (>=0.24,<2)
 Requires-Dist: scipy (>=1.0,<2.0)
 Requires-Dist: seaborn (>=0.11.1,<0.12.0)
 Requires-Dist: semver (>=2.13.0,<3.0.0) ; extra == "release" or extra == "all-dev" or extra == "all-dev"
 Requires-Dist: sphinx-mathjax-offline (>=0.0.1,<0.0.2) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: sqlalchemy (>=1.1.0,<2.0.0) ; extra == "auto" or extra == "all" or extra == "all-dev"
+Requires-Dist: statsforecast (==1.4) ; extra == "statsforecast" or extra == "all" or extra == "all-dev"
 Requires-Dist: statsmodels (>=0.12,<0.14)
 Requires-Dist: tbats (>=1.1.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: torch (>=1.8.0,<1.12.0) ; extra == "torch" or extra == "all" or extra == "all-dev"
 Requires-Dist: tsfresh (>=0.20.0,<0.21.0) ; extra == "classification" or extra == "all" or extra == "all-dev"
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Requires-Dist: types-Deprecated (==1.2.9)
@@ -272,23 +274,27 @@
 We have also prepared a set of tutorials for an easy introduction:
 
 | Notebook     | Interactive launch  |
 |:----------|------:|
 | [Get started](https://github.com/tinkoff-ai/etna/tree/master/examples/get_started.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/get_started.ipynb) |
 | [Backtest](https://github.com/tinkoff-ai/etna/tree/master/examples/backtest.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/backtest.ipynb) |
 | [EDA](https://github.com/tinkoff-ai/etna/tree/master/examples/EDA.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/EDA.ipynb) |
-| [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) |
-| [Clustering](https://github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) |
+| [Regressors and exogenous data](https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) |
+| [Custom model and transform](https://github.com/tinkoff-ai/etna/tree/master/examples/custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/custom_transform_and_model.ipynb) |
 | [Deep learning models](https://github.com/tinkoff-ai/etna/tree/master/examples/NN_examples.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/NN_examples.ipynb) |
 | [Ensembles](https://github.com/tinkoff-ai/etna/tree/master/examples/ensembles.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/ensembles.ipynb) |
-| [Custom Transform and Model](https://github.com/tinkoff-ai/etna/tree/master/examples/custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/custom_transform_and_model.ipynb) |
-| [Exogenous data](https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) |
-| [Forecasting strategies](https://github.com/tinkoff-ai/etna/blob/master/examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecasting_strategies.ipynb) |
-| [Classification](https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/classification.ipynb) |
+| [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) |
+| [Forecasting strategies](https://github.com/tinkoff-ai/etna/tree/master/examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecasting_strategies.ipynb) |
+| [Forecast interpretation](https://github.com/tinkoff-ai/etna/tree/master/examples/forecast_interpretation.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecast_interpretation.ipynb) |
+| [Clustering](https://github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) |
+| [AutoML](https://github.com/tinkoff-ai/etna/tree/master/examples/automl.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/automl.ipynb) |
+| [Inference: using saved pipeline on a new data](https://github.com/tinkoff-ai/etna/tree/master/examples/inference.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/inference.ipynb) |
 | [Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/hierarchical_pipeline.ipynb) |
+| [Classification](https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/classification.ipynb) |
+| [Feature selection](https://github.com/tinkoff-ai/etna/blob/master/examples/feature_selection.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/feature_selection.ipynb) |
 
 ## Documentation
 
 ETNA documentation is available [here](https://etna-docs.netlify.app/).
 
 ## Community
```

