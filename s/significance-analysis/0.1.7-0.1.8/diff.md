# Comparing `tmp/significance_analysis-0.1.7.tar.gz` & `tmp/significance_analysis-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "significance_analysis-0.1.7.tar", max compression
+gzip compressed data, was "significance_analysis-0.1.8.tar", max compression
```

## Comparing `significance_analysis-0.1.7.tar` & `significance_analysis-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1098 2023-03-14 12:16:41.279913 significance_analysis-0.1.7/LICENSE
--rw-r--r--   0        0        0     6449 2023-04-08 09:34:04.468105 significance_analysis-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3224 2023-04-08 09:35:02.256878 significance_analysis-0.1.7/README.md
--rw-r--r--   0        0        0       83 2023-03-27 11:46:33.759635 significance_analysis-0.1.7/src/significance_analysis/__init__.py
--rw-r--r--   0        0        0    17154 2023-04-08 09:34:17.693170 significance_analysis-0.1.7/src/significance_analysis/significance_analysis_function.py
--rw-r--r--   0        0        0     4262 1970-01-01 00:00:00.000000 significance_analysis-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-04-25 22:45:54.520491 significance_analysis-0.1.8/LICENSE
+-rw-r--r--   0        0        0     6449 2023-08-08 00:02:12.333975 significance_analysis-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3282 2023-04-25 22:45:54.520491 significance_analysis-0.1.8/README.md
+-rw-r--r--   0        0        0       83 2023-04-25 22:45:54.577000 significance_analysis-0.1.8/src/significance_analysis/__init__.py
+-rw-r--r--   0        0        0    19081 2023-08-07 23:57:14.278172 significance_analysis-0.1.8/src/significance_analysis/significance_analysis_function.py
+-rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 significance_analysis-0.1.8/PKG-INFO
```

### Comparing `significance_analysis-0.1.7/LICENSE` & `significance_analysis-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `significance_analysis-0.1.7/pyproject.toml` & `significance_analysis-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "significance_analysis"
-version = "v0.1.7"
+version = "v0.1.8"
 description = "Significance Analysis for HPO-algorithms performing on multiple benchmarks"
 authors = ["Anton Merlin Geburek <gebureka@cs.uni-freiburg.de>",
 "Danny Stoll <stolld@cs.uni-freiburg.de>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["Hyperparameter Optimization", "AutoML"]
 classifiers = [
```

### Comparing `significance_analysis-0.1.7/README.md` & `significance_analysis-0.1.8/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# Significance Analysis
-
-[![PyPI version](https://img.shields.io/pypi/v/significance-analysis?color=informational)](https://pypi.org/project/significance-analysis/)
-[![Python versions](https://img.shields.io/pypi/pyversions/significance-analysis)](https://pypi.org/project/significance-analysis/)
-[![License](https://img.shields.io/pypi/l/significance-analysis?color=informational)](LICENSE)
-
-This package is used to analyse datasets of different HPO-algorithms performing on multiple benchmarks.
-
-## Note
-
-As indicated with the `v0.x.x` version number, Significance Analysis is early stage code and APIs might change in the future.
-
-## Documentation
-
-Please have a look at our [example](significance_analysis_example/example_analysis.py).
-The dataset should have the following format:
-
-| system_id<br>(algorithm name) | input_id<br>(benchmark name) | metric<br>(mean/estimate) | optional: bin_id<br>(budget/traininground) |
-| ----------------------------- | ---------------------------- | ------------------------- | ------------------------------------------ |
-| Algorithm1                    | Benchmark1                   | x.xxx                     | 1                                          |
-| Algorithm1                    | Benchmark1                   | x.xxx                     | 2                                          |
-| Algorithm1                    | Benchmark2                   | x.xxx                     | 1                                          |
-| ...                           | ...                          | ...                       | ...                                        |
-| Algorithm2                    | Benchmark2                   | x..xxx                    | 2                                          |
-
-In this dataset, there are two different algorithms, trained on two benchmarks for two iterations each. The variable-names (system_id, input_id...) can be customized, but have to be consistent throughout the dataset, i.e. not "mean" for one benchmark and "estimate" for another. The `conduct_analysis` function is then called with the dataset and the variable-names as parameters.
-Optionally the dataset can be binned according to a fourth variable (bin_id) and the analysis is conducted on each of the bins seperately, as shown in the code example above. To do this, provide the name of the bin_id-variable and if wanted the exact bins and bin labels. Otherwise a bin for each unique value will be created.
-
-## Installation
-
-Using R, >=4.0.0
-install packages: Matrix, emmeans, lmerTest and lme4
-
-Using pip
-
-```bash
-pip install significance-analysis
-```
-
-## Usage
-
-1. Generate data from HPO-algorithms on benchmarks, saving data according to our format.
-1. Call function `conduct_analysis` on dataset, while specifying variable-names
-
-In code, the usage pattern can look like this:
-
-```python
-import pandas as pd
-from signficance_analysis import conduct_analysis
-
-# 1. Generate/import dataset
-data = pd.read_csv("./significance_analysis_example/exampleDataset.csv")
-
-# 2. Analyse dataset
-conduct_analysis(data, "mean", "acquisition", "benchmark")
-```
-
-For more details and features please have a look at our [example](significance_analysis_example/example_analysis.py).
+# Significance Analysis
+
+[![PyPI version](https://img.shields.io/pypi/v/significance-analysis?color=informational)](https://pypi.org/project/significance-analysis/)
+[![Python versions](https://img.shields.io/pypi/pyversions/significance-analysis)](https://pypi.org/project/significance-analysis/)
+[![License](https://img.shields.io/pypi/l/significance-analysis?color=informational)](LICENSE)
+
+This package is used to analyse datasets of different HPO-algorithms performing on multiple benchmarks.
+
+## Note
+
+As indicated with the `v0.x.x` version number, Significance Analysis is early stage code and APIs might change in the future.
+
+## Documentation
+
+Please have a look at our [example](significance_analysis_example/example_analysis.py).
+The dataset should have the following format:
+
+| system_id<br>(algorithm name) | input_id<br>(benchmark name) | metric<br>(mean/estimate) | optional: bin_id<br>(budget/traininground) |
+| ----------------------------- | ---------------------------- | ------------------------- | ------------------------------------------ |
+| Algorithm1                    | Benchmark1                   | x.xxx                     | 1                                          |
+| Algorithm1                    | Benchmark1                   | x.xxx                     | 2                                          |
+| Algorithm1                    | Benchmark2                   | x.xxx                     | 1                                          |
+| ...                           | ...                          | ...                       | ...                                        |
+| Algorithm2                    | Benchmark2                   | x..xxx                    | 2                                          |
+
+In this dataset, there are two different algorithms, trained on two benchmarks for two iterations each. The variable-names (system_id, input_id...) can be customized, but have to be consistent throughout the dataset, i.e. not "mean" for one benchmark and "estimate" for another. The `conduct_analysis` function is then called with the dataset and the variable-names as parameters.
+Optionally the dataset can be binned according to a fourth variable (bin_id) and the analysis is conducted on each of the bins seperately, as shown in the code example above. To do this, provide the name of the bin_id-variable and if wanted the exact bins and bin labels. Otherwise a bin for each unique value will be created.
+
+## Installation
+
+Using R, >=4.0.0
+install packages: Matrix, emmeans, lmerTest and lme4
+
+Using pip
+
+```bash
+pip install significance-analysis
+```
+
+## Usage
+
+1. Generate data from HPO-algorithms on benchmarks, saving data according to our format.
+1. Call function `conduct_analysis` on dataset, while specifying variable-names
+
+In code, the usage pattern can look like this:
+
+```python
+import pandas as pd
+from signficance_analysis import conduct_analysis
+
+# 1. Generate/import dataset
+data = pd.read_csv("./significance_analysis_example/exampleDataset.csv")
+
+# 2. Analyse dataset
+conduct_analysis(data, "mean", "acquisition", "benchmark")
+```
+
+For more details and features please have a look at our [example](significance_analysis_example/example_analysis.py).
```

### Comparing `significance_analysis-0.1.7/src/significance_analysis/significance_analysis_function.py` & `significance_analysis-0.1.8/src/significance_analysis/significance_analysis_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,147 +1,204 @@
+"""Imports for analysis method"""
 import typing
 
 import matplotlib.pyplot as plt
 import pandas as pd
-import scipy.stats as stats
 from pymer4.models import Lmer
+from scipy import stats
+
+
+def glrt(mod1: Lmer, mod2: Lmer) -> dict[str, typing.Any]:
+    """Generalized Likelihood Ratio Test on two Liner Mixed Effect Models from R
+
+    Args:
+        mod1 (Lmer): First, simple model, Null-Hypothesis assumes that this model contains not significantly less information as the second model
+        mod2 (Lmer): Second model, Alternative Hypothesis assumes that this model contains significant new information
+
+    Returns:
+        dict[str,typing.Any]: Result dictionary with Chi-Square-Score, Degrees of Freedom and p-value of the test
+    """
+    assert (
+        mod1.logLike
+        and mod2.logLike
+        and mod1.coefs is not None
+        and mod2.coefs is not None
+    )
+    chi_square = 2 * abs(mod1.logLike - mod2.logLike)
+    delta_params = abs(len(mod1.coefs) - len(mod2.coefs))
+    return {
+        "chi_square": chi_square,
+        "df": delta_params,
+        "p": 1 - stats.chi2.cdf(chi_square, df=delta_params),
+    }
 
 
 def conduct_analysis(
     data: pd.DataFrame,
     metric: str,
     system_id: str,
     input_id: str,
-    bin_id: str = None,
-    bins: typing.Union[list[list[str]], list[float]] = None,
-    bin_labels: list[str] = None,
-    subset: typing.Tuple[str, typing.Union[str, list[str], list[list[str]]]] = None,
+    bin_id: typing.Optional[str] = None,
+    bins: typing.Optional[typing.Union[list[list[str]], list[float]]] = None,
+    bin_labels: typing.Optional[list[str]] = None,
+    subset: typing.Optional[
+        typing.Union[
+            str,
+            typing.Tuple[
+                str, typing.Union[dict[str, typing.Any], str, list[str], list[list[str]]]
+            ],
+        ]
+    ] = None,
     show_plots: bool = True,
     summarize: bool = True,
-) -> typing.Tuple[dict[str, any], typing.Tuple[any, pd.DataFrame]]:
+    show_contrasts: bool = True,
+) -> typing.Union[
+    typing.Union[
+        typing.Tuple[
+            dict[str, typing.Any],
+            typing.Union[typing.Any, typing.Tuple[typing.Any, pd.DataFrame]],
+        ],
+        dict[str, typing.Any],
+    ],
+    dict[
+        str,
+        typing.Union[
+            typing.Tuple[
+                dict[str, typing.Any],
+                typing.Union[typing.Any, typing.Tuple[typing.Any, pd.DataFrame]],
+            ],
+            dict[str, typing.Any],
+        ],
+    ],
+]:
     """LMER-Based Performance Analysis
 
     Args:
         data (pd.DataFrame): Dataset
         metric (str): Column name of metric (e.g. Mean) in dataset
         system_id (str): Column name of system (e.g. Algorithm) in dataset
         input_id (str): Column name of input (e.g. Benchmark) in dataset
         bin_id (str, optional): Column name of bin (e.g. Budget). Defaults to None.
         bins (typing.Union[list[list[str]], list[float]], optional): Specified bins: If None, bins for every unique value are used. If list of float, numeric variable gets binned into intervals according to list. If list of list of str, variable gets binned into bins according to sublists. Defaults to None.
         bin_labels (list[str], optional): Labels for bins. If None, bins are named after content/interval borders. If list of str, bins are named according to list. Defaults to None.
-        subset (typing.Tuple[str, typing.Union[str, list[str], list[list[str]]]], optional): Subset of dataset that should be used for analysis. First entry of tuple is name of variable that defines subset. Second entry is either list of entries that should be analysed iteratively (single entries or groups), or "all"/"a" for all entries. Defaults to None.
+        subset (typing.Union[str,typing.Tuple[str, typing.Union[dict[str, any], str, list[str], list[list[str]]]]], optional): Subset of dataset that should be used for analysis. Only name of variable that defines subset to create subgroup for each entry or: First entry of tuple is name of variable, second entry is either list of entries that should be analysed iteratively (single entries or groups), or "all"/"a" for all entries. Defaults to None.
         show_plots (bool, optional): Show plots. First entry is boxplot comparing systems, second entry is graph showing systems in all bins. Defaults to True.
         summarize (bool, optional): Print results while analysing. Defaults to True.
+        show_contrasts (bool, optional): Develop contrasts between systems
 
     Raises:
         SystemExit: If Subset-Value is not in Dataset.
         SystemExit: If the number of Labels does not fit the number of numeric Bins.
         SystemExit: If the number of Labels does not fit the number of categorical Bins.
 
     Returns:
-        typing.Tuple[dict[str,any],typing.Tuple[any,pd.DataFrame]]: First the result-dictionary of the GLRT and second the post_hoc-analysis of the LMEM.
+        typing.Union[typing.Union[typing.Tuple[dict[str,typing.Any],typing.Union[typing.Any,typing.Tuple[typing.Any,pd.DataFrame]]],dict[str,typing.Any]],dict[str,typing.Union[typing.Tuple[dict[str,typing.Any],typing.Union[typing.Any,typing.Tuple[typing.Any,pd.DataFrame]]],dict[str,typing.Any]]]]: Result tuple, first the result-dictionary of the GLRT and second the post_hoc-analysis of the LMEM, consisting of first the estimated means for each system and second the contrasts. If a subsets are used, returns dictionary with full results for each subset. If contrasts are turned off, only returns estimated means as second tuple-entry. If post-hoc-analysis failed, only returns GLRT-Results.
     """
 
     if subset is not None:
-        if isinstance(subset[1], str):
-            if subset[1] in ["all", "a", "All", "A"]:
+        if isinstance(subset, str):
+            subset = (subset, "a")
+        if isinstance(subset[1], (str, dict)):
+            if isinstance(subset[1], dict):
+                new_dict = {}
+                for key, value in subset[1].items():
+                    if value not in new_dict:
+                        new_dict[value] = [key]
+                    else:
+                        if value in new_dict:
+                            new_dict[value].append(key)
+                subset_list = list(new_dict.values())
+            elif subset[1] in ["all", "a", "All", "A"]:
                 subset_list = list(data[subset[0]].unique())
             else:
                 subset_list = [subset[1]]
         else:
             subset_list = subset[1]
+        return_dict = {}
         for subset_item in subset_list:
             print(f"Analysis for {subset_item}")
             if isinstance(subset_item, str):
                 subset_item = [subset_item]
             if any(item not in data[subset[0]].unique() for item in subset_item):
                 raise SystemExit(
                     f"A Subset-Value of {subset_item} is not in Dataset. Choose from {data[subset[0]].unique()}"
                 )
-            conduct_analysis(
+            return_dict["__".join(subset_item)] = conduct_analysis(
                 data.loc[data[subset[0]].isin(subset_item)],
                 metric,
                 system_id,
                 input_id,
                 bin_id,
                 bins=bins,
                 bin_labels=bin_labels,
                 show_plots=show_plots,
                 summarize=summarize,
+                show_contrasts=show_contrasts,
             )
-    else:
-
-        def GLRT(mod1, mod2):
-            chi_square = 2 * abs(mod1.logLike - mod2.logLike)
-            delta_params = abs(len(mod1.coefs) - len(mod2.coefs))
-            return {
-                "chi_square": chi_square,
-                "df": delta_params,
-                "p": 1 - stats.chi2.cdf(chi_square, df=delta_params),
-            }
-
-        pd.options.mode.chained_assignment = None
-        pd.set_option("display.max_rows", 5000)
-        pd.set_option("display.max_columns", 5000)
-        pd.set_option("display.width", 10000)
-
-        if bin_id is None:
-            if len(data[input_id].unique()) == 1:
-                data.loc[data.sample(1).index, input_id] = (
-                    data[input_id].unique()[0] + "_d"
-                )
+        return return_dict
 
-            if show_plots:
-                _, ax = plt.subplots()
-                ax.boxplot(
-                    [group[metric] for _, group in data.groupby(system_id)],
-                    labels=data[system_id].unique(),
-                )
-                plt.yscale("log")
-                plt.show()
-
-            # System-identifier: system_id
-            # Input-Identifier: input_id
-            # Two models, "different"-Model assumes significant difference between performance of groups, divided by system-identifier
-            # Formula has form: "metric ~ system_id + (1 | input_id)"
-            differentMeans_model = Lmer(
-                formula=f"{metric}~{system_id}+(1|{input_id})", data=data
+    pd.set_option("chained_assignment", None)
+    pd.set_option("display.max_rows", 5000)
+    pd.set_option("display.max_columns", 5000)
+    pd.set_option("display.width", 10000)
+
+    if not bin_id:
+        if len(data[input_id].unique()) == 1:
+            data.loc[data.sample(1).index, input_id] = data[input_id].unique()[0] + "_d"
+
+        if show_plots:
+            _, axis = plt.subplots()
+            axis.boxplot(
+                [group[metric] for _, group in data.groupby(system_id)],
+                labels=list(data[system_id].unique()),
             )
-
-            # factors specifies names of system_identifier, i.e. Baseline, or Algorithm1
-            differentMeans_model.fit(
-                factors={system_id: list(data[system_id].unique())},
-                REML=False,
-                summarize=False,
+            plt.yscale("log")
+            plt.xticks(rotation=-45, ha="right")
+            plt.show()
+
+        # System-identifier: system_id
+        # Input-Identifier: input_id
+        # Two models, "different"-Model assumes significant difference between performance of groups, divided by system-identifier
+        # Formula has form: "metric ~ system_id + (1 | input_id)"
+        different_means_model = Lmer(
+            formula=f"{metric}~{system_id}+(1|{input_id})", data=data
+        )
+
+        # factors specifies names of system_identifier, i.e. Baseline, or Algorithm1
+        different_means_model.fit(
+            factors={system_id: list(data[system_id].unique())},
+            REML=False,
+            summarize=False,
+        )
+
+        # "Common"-Model assumes no significant difference, which is why the system-identifier is not included
+        common_mean_model = Lmer(formula=f"{metric}~ (1 | {input_id})", data=data)
+        common_mean_model.fit(REML=False, summarize=False)
+
+        # Signficant p-value shows, that different-Model fits data sign. better, i.e.
+        # There is signficant difference in system-identifier
+        result_glrt_dm_cm = glrt(different_means_model, common_mean_model)
+        p_value = result_glrt_dm_cm["p"]
+        print(f"P-value: {p_value}")
+        if result_glrt_dm_cm["p"] < 0.05:
+            print(
+                f"\nAs the p-value {p_value} is smaller than 0.05, we can reject the Null-Hypothesis that the model "
+                f"that does not consider the {system_id} describes the data as well as the one that does. Therefore "
+                f"there is significant difference within {system_id}.\n"
+            )
+        else:
+            print(
+                f"\nAs the p-value {p_value} is not smaller than 0.05, we cannot reject the Null-Hypothesis that the model "
+                f"that does not consider the {system_id} describes the data as well as the one that does. Therefore "
+                f"there is no significant difference within {system_id}\n."
             )
 
-            # "Common"-Model assumes no significant difference, which is why the system-identifier is not included
-            commonMean_model = Lmer(formula=f"{metric}~ (1 | {input_id})", data=data)
-            commonMean_model.fit(REML=False, summarize=False)
-
-            # Signficant p-value shows, that different-Model fits data sign. better, i.e.
-            # There is signficant difference in system-identifier
-            result_GLRT_dM_cM = GLRT(differentMeans_model, commonMean_model)
-            p_value = result_GLRT_dM_cM["p"]
-            print(f"P-value: {p_value}")
-            if result_GLRT_dM_cM["p"] < 0.05:
-                print(
-                    f"\nAs the p-value {p_value} is smaller than 0.05, we can reject the Null-Hypothesis that the model "
-                    f"that does not consider the {system_id} describes the data as well as the one that does. Therefore "
-                    f"there is significant difference within {system_id}.\n"
-                )
-            else:
-                print(
-                    f"\nAs the p-value {p_value} is not smaller than 0.05, we cannot reject the Null-Hypothesis that the model "
-                    f"that does not consider the {system_id} describes the data as well as the one that does. Therefore "
-                    f"there is no significant difference within {system_id}\n."
-                )
-
-            # Post hoc divides the "different"-Model into its three systems
-            post_hoc_results = differentMeans_model.post_hoc(marginal_vars=[system_id])
+        # Post hoc divides the "different"-Model into its three systems
+        post_hoc_results = different_means_model.post_hoc(marginal_vars=[system_id])
+        if post_hoc_results:
             contrasts = post_hoc_results[1]
             for pair in contrasts["Contrast"]:
                 contrasts.loc[
                     contrasts["Contrast"] == pair, system_id + "_1"
                 ] = pair.split(" - ")[0]
                 contrasts.loc[
                     contrasts["Contrast"] == pair, system_id + "_2"
@@ -152,15 +209,16 @@
             column = contrasts.pop(system_id + "_1")
             contrasts.insert(0, system_id + "_1", column)
 
             if summarize:
                 # [0] shows group-means, i.e. performance of the single system-groups
                 print(post_hoc_results[0])  # cell (group) means
                 # [1] shows the pairwise comparisons, i.e. improvements over each other, with p-value
-                print(contrasts)  # contrasts (group differences)
+                if show_contrasts:
+                    print(contrasts)  # contrasts (group differences)
 
             best_system_id = post_hoc_results[0].loc[
                 post_hoc_results[0]["Estimate"].idxmin()
             ][system_id]
 
             contenders = []
             for _, row in contrasts.iterrows():
@@ -182,105 +240,106 @@
                     f"The best performing {system_id} is {best_system_id}, but {contenders} are only insignificantly worse.\n"
                 )
             else:
                 print(
                     f"The best performing {system_id} is {best_system_id}, all other perform significantly worse.\n"
                 )
 
-            return result_GLRT_dM_cM, post_hoc_results
+            if show_contrasts:
+                return result_glrt_dm_cm, post_hoc_results
+            return result_glrt_dm_cm, post_hoc_results[0]
+        return result_glrt_dm_cm
 
-        else:
-            if bins is None:
-                data[f"{bin_id}_bins"] = data[bin_id]
+    if not bins:
+        data[f"{bin_id}_bins"] = data[bin_id]
+    else:
+        if isinstance(bins, list) and all(isinstance(bin, (float, int)) for bin in bins):
+            bins_set = set(bins)
+            bins_set.add(data[bin_id].min())
+            bins_set.add(data[bin_id].max())
+            complete_bins = sorted(list(bins_set))
+            if bin_labels is None:
+                bin_labels = [
+                    f"{complete_bins[i]}_{complete_bins[i+1]}"
+                    for i in range(len(complete_bins) - 1)
+                ]
             else:
-                if isinstance(bins, list) and all(
-                    isinstance(bin, (float, int)) for bin in bins
-                ):
-                    bins_set = set(bins)
-                    bins_set.add(data[bin_id].min())
-                    bins_set.add(data[bin_id].max())
-                    bins = sorted(list(bins_set))
-                    if bin_labels is None:
-                        bin_labels = [
-                            f"{bins[i]}_{bins[i+1]}" for i in range(len(bins) - 1)
-                        ]
-                    else:
-                        if len(bin_labels) != len(bins) + 1:
-                            raise SystemExit(
-                                f"Too many or too few labels ({len(bin_labels)} labels and {len(bins)} bins)"
-                            )
-                    data[f"{bin_id}_bins"] = pd.cut(
-                        data[bin_id], bins=bins, labels=bin_labels, include_lowest=True
+                if len(bin_labels) != len(bins) + 1:
+                    raise SystemExit(
+                        f"Too many or too few labels ({len(bin_labels)} labels and {len(complete_bins)} bins)"
                     )
-                else:
-                    if bin_labels is not None:
-                        if len(bin_labels) != len(bins):
-                            raise SystemExit(
-                                f"Too many or too few labels ({len(bin_labels)} labels and {len(bins)} bins)"
-                            )
-                        data[f"{bin_id}_bins"] = data[bin_id].apply(
-                            lambda x: bin_labels[
-                                bins.index([s for s in bins if x in s][0])
-                            ]
-                        )
-                    else:
-                        data[f"{bin_id}_bins"] = data[bin_id].apply(
-                            lambda x: "_".join([s for s in bins if x in s][0])
-                        )
-
-            # New model "expanded": Divides into system AND bin-classes (Term system:bin_id allows for Cartesian Product, i.e. different Mean for each system and bin-class)
-            model_expanded = Lmer(
-                f"{metric} ~  {system_id} + {bin_id}_bins + {system_id}:{bin_id}_bins + (1 | {input_id})",
-                data=data,
-            )
-            model_expanded.fit(
-                factors={
-                    system_id: list(data[system_id].unique()),
-                    f"{bin_id}_bins": list(data[f"{bin_id}_bins"].unique()),
-                },
-                REML=False,
-                summarize=False,
-            )
-            # Second model "nointeraction" lacks system:src-Term to hypothesise no interaction, i.e. no difference when changing bin-class
-            model_nointeraction = Lmer(
-                f"{metric} ~ {system_id} + {bin_id}_bins + (1 | {input_id})",
-                data=data,
-            )
-            model_nointeraction.fit(
-                factors={
-                    system_id: list(data[system_id].unique()),
-                    f"{bin_id}_bins": list(data[f"{bin_id}_bins"].unique()),
-                },
-                REML=False,
-                summarize=False,
+            data[f"{bin_id}_bins"] = pd.cut(
+                data[bin_id], bins=complete_bins, labels=bin_labels, include_lowest=True
             )
-
-            # If it's significant, look at if different systems perform better at different bin-classes
-            result_GLRT_ex_ni = GLRT(model_expanded, model_nointeraction)
-            p_value = result_GLRT_ex_ni["p"]
-            print(f"P-value: {p_value}")
-            if p_value < 0.05:
-                print(
-                    f"\nAs the p-value {p_value} is smaller than 0.05, we can reject the Null-Hypothesis that the model "
-                    f"that does not consider the {system_id} and the {bin_id} describes the data as well as the one that does. Therefore "
-                    f"there is significant difference within {system_id} and the {bin_id}.\n"
+        else:
+            if bin_labels:
+                if len(bin_labels) != len(bins):
+                    raise SystemExit(
+                        f"Too many or too few labels ({len(bin_labels)} labels and {len(bins)} bins)"
+                    )
+                data[f"{bin_id}_bins"] = data[bin_id].apply(
+                    lambda x: bin_labels[bins.index([s for s in bins if x in s][0])]
                 )
             else:
-                print(
-                    f"\nAs the p-value {p_value} is not smaller than 0.05, we cannot reject the Null-Hypothesis that the model "
-                    f"that does not consider the {system_id} and the {bin_id} describes the data as well as the one that does. Therefore "
-                    f"there is no significant difference within {system_id} and {bin_id}\n."
+                data[f"{bin_id}_bins"] = data[bin_id].apply(
+                    lambda x: "_".join([s for s in bins if x in s][0])
                 )
 
-            post_hoc_results = model_expanded.post_hoc(
-                marginal_vars=system_id, grouping_vars=f"{bin_id}_bins"
-            )
-            if summarize:
-                # Means of each combination
-                print(post_hoc_results[0])
+    # New model "expanded": Divides into system AND bin-classes (Term system:bin_id allows for Cartesian Product, i.e. different Mean for each system and bin-class)
+    model_expanded = Lmer(
+        f"{metric} ~  {system_id} + {bin_id}_bins + {system_id}:{bin_id}_bins + (1 | {input_id})",
+        data=data,
+    )
+    model_expanded.fit(
+        factors={
+            system_id: list(data[system_id].unique()),
+            f"{bin_id}_bins": list(data[f"{bin_id}_bins"].unique()),
+        },
+        REML=False,
+        summarize=False,
+    )
+    # Second model "nointeraction" lacks system:src-Term to hypothesise no interaction, i.e. no difference when changing bin-class
+    model_nointeraction = Lmer(
+        f"{metric} ~ {system_id} + {bin_id}_bins + (1 | {input_id})",
+        data=data,
+    )
+    model_nointeraction.fit(
+        factors={
+            system_id: list(data[system_id].unique()),
+            f"{bin_id}_bins": list(data[f"{bin_id}_bins"].unique()),
+        },
+        REML=False,
+        summarize=False,
+    )
+
+    # If it's significant, look at if different systems perform better at different bin-classes
+    result_glrt_ex_ni = glrt(model_expanded, model_nointeraction)
+    p_value = result_glrt_ex_ni["p"]
+    print(f"P-value: {p_value}")
+    if p_value < 0.05:
+        print(
+            f"\nAs the p-value {p_value} is smaller than 0.05, we can reject the Null-Hypothesis that the model "
+            f"that does not consider the {system_id} and the {bin_id} describes the data as well as the one that does. Therefore "
+            f"there is significant difference within {system_id} and the {bin_id}.\n"
+        )
+    else:
+        print(
+            f"\nAs the p-value {p_value} is not smaller than 0.05, we cannot reject the Null-Hypothesis that the model "
+            f"that does not consider the {system_id} and the {bin_id} describes the data as well as the one that does. Therefore "
+            f"there is no significant difference within {system_id} and {bin_id}\n."
+        )
+
+    post_hoc_results = model_expanded.post_hoc(
+        marginal_vars=system_id, grouping_vars=f"{bin_id}_bins"
+    )
+    if post_hoc_results:
+        if summarize:
+            # Means of each combination
+            print(post_hoc_results[0])
+        if show_contrasts:
             # Comparisons for each combination
             for group in data[f"{bin_id}_bins"].unique():
                 contrasts = post_hoc_results[1].query(f"{bin_id}_bins == '{group}'")
 
                 for pair in contrasts["Contrast"]:
                     contrasts.loc[
                         contrasts["Contrast"] == pair, system_id + "_1"
@@ -290,21 +349,15 @@
                     ] = pair.split(" - ")[1]
                 contrasts = contrasts.drop("Contrast", axis=1)
                 column = contrasts.pop(system_id + "_2")
                 contrasts.insert(0, system_id + "_2", column)
                 column = contrasts.pop(system_id + "_1")
                 contrasts.insert(0, system_id + "_1", column)
                 if summarize:
-                    print(
-                        contrasts[
-                            (contrasts["Sig"] == "***")
-                            | (contrasts["Sig"] == "**")
-                            | (contrasts["Sig"] == "*")
-                        ]
-                    )
+                    print(contrasts[contrasts["Sig"] != ""])
                 best_system_id = (
                     post_hoc_results[0]
                     .query(f"{bin_id}_bins == '{group}'")
                     .loc[
                         post_hoc_results[0]
                         .query(f"{bin_id}_bins == '{group}'")["Estimate"]
                         .idxmin()
@@ -331,26 +384,29 @@
                     )
                 else:
                     print(
                         f"The best performing {system_id} in {bin_id}-class {group} is {best_system_id}, all other perform significantly worse.\n"
                     )
 
             if show_plots:
-                _, ax = plt.subplots(figsize=(10, 6))
+                _, axis = plt.subplots(figsize=(10, 6))
                 for sys_id, group in post_hoc_results[0].groupby(system_id):
-                    ax.errorbar(
+                    axis.errorbar(
                         group[f"{bin_id}_bins"],
                         group["Estimate"],
                         yerr=group["SE"],
                         fmt="o-",
                         capsize=3,
                         label=sys_id,
                         lolims=group["2.5_ci"],
                         uplims=group["97.5_ci"],
                     )
-                ax.set_xlabel(bin_id)
-                ax.set_ylabel("Estimate")
-                ax.set_title(f"Estimates by {system_id} and {bin_id}")
-                ax.legend()
+                axis.set_xlabel(bin_id)
+                axis.set_ylabel("Estimate")
+                axis.set_title(f"Estimates by {system_id} and {bin_id}")
+                axis.legend()
                 plt.show()
 
-            return result_GLRT_ex_ni, post_hoc_results
+        if show_contrasts:
+            return result_glrt_ex_ni, post_hoc_results
+        return result_glrt_ex_ni, post_hoc_results[0]
+    return result_glrt_ex_ni
```

### Comparing `significance_analysis-0.1.7/PKG-INFO` & `significance_analysis-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: significance-analysis
-Version: 0.1.7
+Version: 0.1.8
 Summary: Significance Analysis for HPO-algorithms performing on multiple benchmarks
 License: MIT
 Keywords: Hyperparameter Optimization,AutoML
 Author: Anton Merlin Geburek
 Author-email: gebureka@cs.uni-freiburg.de
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: matplotlib (<3.7.0)
 Requires-Dist: pymer4 (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
 
 # Significance Analysis
```

