# Comparing `tmp/hojichar-0.8.1.tar.gz` & `tmp/hojichar-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.8.1.tar", max compression
+gzip compressed data, was "hojichar-0.9.0.tar", max compression
```

## Comparing `hojichar-0.8.1.tar` & `hojichar-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-08-04 01:32:14.808367 hojichar-0.8.1/LICENSE
--rw-r--r--   0        0        0    14271 2023-08-04 01:32:14.808367 hojichar-0.8.1/README.md
--rw-r--r--   0        0        0      547 2023-08-04 01:32:35.280477 hojichar-0.8.1/hojichar/__init__.py
--rw-r--r--   0        0        0     5819 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/cli.py
--rw-r--r--   0        0        0       42 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/__init__.py
--rw-r--r--   0        0        0     5039 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/composition.py
--rw-r--r--   0        0        0     5638 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     6221 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/inspection.py
--rw-r--r--   0        0        0     1087 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    12104 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    23939 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1606 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2530 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3380 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1920 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/process.py
--rw-r--r--   0        0        0     1788 2023-08-04 01:32:35.276477 hojichar-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    15042 1970-01-01 00:00:00.000000 hojichar-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-08 11:44:23.892481 hojichar-0.9.0/LICENSE
+-rw-r--r--   0        0        0    17274 2023-08-08 11:44:23.892481 hojichar-0.9.0/README.md
+-rw-r--r--   0        0        0      665 2023-08-08 11:44:42.416801 hojichar-0.9.0/hojichar/__init__.py
+-rw-r--r--   0        0        0     4506 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/cli.py
+-rw-r--r--   0        0        0       42 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     5039 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5638 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     6787 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/core/models.py
+-rw-r--r--   0        0        0     6197 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/core/parallel.py
+-rw-r--r--   0        0        0      147 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23939 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-08-08 11:44:23.892481 hojichar-0.9.0/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1788 2023-08-08 11:44:42.412801 hojichar-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    18045 1970-01-01 00:00:00.000000 hojichar-0.9.0/PKG-INFO
```

### Comparing `hojichar-0.8.1/LICENSE` & `hojichar-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/README.md` & `hojichar-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -117,17 +117,102 @@
 ```
 
 The `p` argument passed to the `document_filters.AcceptJapanese` constructor determines the probability of applying the filter; with a probability of `1-p`, it acts as an identity function. This behavior is defined in the parent class `hojichar.Filter`.
 
 ## Additional Notes on Compose
 
 - Even though the behavior of a `Compose` object when called is a text-in, text-out function, `Compose` itself also inherits from the `Filter` class. Therefore, applying the `apply` method to a `Compose` object results in `hojihcar.Document` class being used as input and output.
-- You can access various statistics regarding the processing performed by `Compose` through `Compose.statistics`, which returns a dictionary.
+- `Compose` class behaves like a Filter. If you add a Compose object as one of the filters in the constructor of Compose, the filter will be unfolded recursively.
+- You can access various statistics regarding the processing performed by `Compose` through `Compose.statistics` or `Compose.statistics_obj`.
+  - `Compose.statistics` is a dictionary like above.
+
+    ```json
+    {
+    "total_info": {
+        "processed_num": 10928,
+        "discard_num": 5513,
+        "input_MB": 104.514584,
+        "output_MB": 25.33024,
+        "cumulative_time": 114.071047143,
+        "total_token_num": 0
+    },
+    "layers_info": [
+        {
+        "name": "0-JSONLoader",
+        "discard_num": 0,
+        "diff_MB": -1.9647932052612305,
+        "cumulative_time": 0.420034328,
+        "params": {
+            "name": "JSONLoader",
+            "p": 1,
+            "skip_rejected": true,
+            "key": "text",
+            "ignore": true
+        }
+        },
+        {
+        "name": "1-DocumentNormalizer",
+        "discard_num": 0,
+        "diff_MB": -1.5221118927001953,
+        "cumulative_time": 8.286988707,
+        "params": {
+            "name": "DocumentNormalizer",
+            "p": 1,
+            "skip_rejected": true
+        }
+        },
+        {
+        "name": "2-DocumentLengthFilter",
+        "discard_num": 344,
+        "diff_MB": -0.05566596984863281,
+        "cumulative_time": 0.093768306,
+        "params": {
+            "name": "DocumentLengthFilter",
+            "p": 1,
+            "skip_rejected": true,
+            "min_doc_len": 100,
+            "max_doc_len": null
+        }
+        },
+    ]
+    }
+    ```
+
+- `Compose.statistics_obj` is a `hojichar.StatsContainer` class. The `hojichar.StatsContainer` class stores the raw values of the statistics dictionary, and addition operations are defined to easily calculate the total statistics processed with the same filter. You can get the statistics dictionary by calling `Compose.statistics_obj.get_human_readable_values()`.
+
+## Parallel application of `Compose`
+
+The `hojichar.Parallel` class allows for the application of `Compose` to an iterable of `Document` concurrently. This class empowers users to process vast collections of documents by harnessing the power of multiple CPU cores.
+
+Example usage of `Parallel` class to proces a very large JSON Lines file concurrently.
+
+```python
+import hojichar
+
+input_file = "your_text.jsonl"
+input_doc_iter = (hojichar.Document(line) for line in open(input_file))
+
+cleaner = hojichar.Compose([
+    hojichar.document_filters.JSONLoader(),
+    hojichar.document_filters.DocumentNormalizer(),
+    # Insert your filters
+    hojichar.document_filters.JSONDumper(),
+])
+
+with hojichar.Parallel(cleaner, num_jobs=10) as pfilter:
+    out_doc_iter = pfilter.imap_apply(input_doc_iter)
+    with open("your_processed_text.jsonl", "w") as fp:
+        for doc in out_doc_iter:
+            fp.write(doc.text + "\n")
 
-It might be helpful to add examples demonstrating the use of `Compose
+```
+
+- Always use the `Parallel` class within a `with` statement.
+- `Parallel.imap_apply(doc_iter)` processes an iterator of `Document` and returns an iterator of the processed documents.
+- For additional options and details about the `Parallel` class, please refer to the official documentation.
 
 ## CLI tool and preprocessing profile
 
 - HojiChar provides CLI tools for text preprocess pipeline.
 - User defines a series of preprocessing into a python file as profile.
 
 - Example:
```

### Comparing `hojichar-0.8.1/hojichar/__init__.py` & `hojichar-0.9.0/hojichar/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
+from .core.inspection import StatsContainer
 from .core.models import Document, Token
+from .core.parallel import Parallel
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.8.1"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.9.0"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "utils",
     "Compose",
     "Filter",
     "TokenFilter",
     "Document",
     "Token",
+    "Parallel",
+    "StatsContainer",
     "deduplication",
     "document_filters",
     "token_filters",
     "tokenization",
 ]
```

### Comparing `hojichar-0.8.1/hojichar/core/composition.py` & `hojichar-0.9.0/hojichar/core/composition.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/core/filter_interface.py` & `hojichar-0.9.0/hojichar/core/filter_interface.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/core/inspection.py` & `hojichar-0.9.0/hojichar/core/inspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,20 @@
             self.name,
             self.discard_num + other.discard_num,
             self.diff_bytes + other.diff_bytes,
             self.cumulative_time_ns + other.cumulative_time_ns,
             self.params,
         )
 
+    def reset(self) -> FilterStatistics:
+        self.discard_num = 0
+        self.diff_bytes = 0
+        self.cumulative_time_ns = 0
+        return self
+
 
 @dataclasses.dataclass
 class DocStatistics:
     processed_num: int = 0
     discard_num: int = 0
     input_bytes: int = 0
     output_bytes: int = 0
@@ -91,14 +97,23 @@
             self.discard_num + other.discard_num,
             self.input_bytes + other.input_bytes,
             self.output_bytes + other.output_bytes,
             self.cumulative_time_ns + other.cumulative_time_ns,
             self.total_token_num + other.total_token_num,
         )
 
+    def reset(self) -> DocStatistics:
+        self.processed_num = 0
+        self.discard_num = 0
+        self.input_bytes = 0
+        self.output_bytes = 0
+        self.cumulative_time_ns = 0
+        self.total_token_num = 0
+        return self
+
 
 @dataclasses.dataclass
 class StatsContainer:
     total_info: DocStatistics
     layers_info: Dict[str, FilterStatistics]  # Key of the dict is filter name.
 
     def __add__(self, other: StatsContainer) -> StatsContainer:
@@ -112,14 +127,20 @@
         return {
             "total_info": self.total_info.get_human_readable_values(),
             "layers_info": [
                 layer.get_human_readable_values() for layer in self.layers_info.values()
             ],
         }
 
+    def reset(self) -> StatsContainer:
+        self.total_info.reset
+        for layer in self.layers_info.values():
+            layer.reset()
+        return self
+
 
 class StatisticsCounter:
     def __init__(self, inspectors: List[Inspector]) -> None:
         counts = dict()
         for inspector in inspectors:
             counts[inspector.target] = FilterStatistics(
                 name=inspector.target,
```

### Comparing `hojichar-0.8.1/hojichar/core/models.py` & `hojichar-0.9.0/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.9.0/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.9.0/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.9.0/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.9.0/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.9.0/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/filters/__init__.py` & `hojichar-0.9.0/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/filters/deduplication.py` & `hojichar-0.9.0/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/filters/document_filters.py` & `hojichar-0.9.0/hojichar/filters/document_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/filters/token_filters.py` & `hojichar-0.9.0/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/filters/tokenization.py` & `hojichar-0.9.0/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/utils/__init__.py` & `hojichar-0.9.0/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/utils/io_iter.py` & `hojichar-0.9.0/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/hojichar/utils/load_compose.py` & `hojichar-0.9.0/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.1/pyproject.toml` & `hojichar-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.8.1"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.9.0"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
```

### Comparing `hojichar-0.8.1/PKG-INFO` & `hojichar-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.8.1
+Version: 0.9.0
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -138,17 +138,102 @@
 ```
 
 The `p` argument passed to the `document_filters.AcceptJapanese` constructor determines the probability of applying the filter; with a probability of `1-p`, it acts as an identity function. This behavior is defined in the parent class `hojichar.Filter`.
 
 ## Additional Notes on Compose
 
 - Even though the behavior of a `Compose` object when called is a text-in, text-out function, `Compose` itself also inherits from the `Filter` class. Therefore, applying the `apply` method to a `Compose` object results in `hojihcar.Document` class being used as input and output.
-- You can access various statistics regarding the processing performed by `Compose` through `Compose.statistics`, which returns a dictionary.
+- `Compose` class behaves like a Filter. If you add a Compose object as one of the filters in the constructor of Compose, the filter will be unfolded recursively.
+- You can access various statistics regarding the processing performed by `Compose` through `Compose.statistics` or `Compose.statistics_obj`.
+  - `Compose.statistics` is a dictionary like above.
+
+    ```json
+    {
+    "total_info": {
+        "processed_num": 10928,
+        "discard_num": 5513,
+        "input_MB": 104.514584,
+        "output_MB": 25.33024,
+        "cumulative_time": 114.071047143,
+        "total_token_num": 0
+    },
+    "layers_info": [
+        {
+        "name": "0-JSONLoader",
+        "discard_num": 0,
+        "diff_MB": -1.9647932052612305,
+        "cumulative_time": 0.420034328,
+        "params": {
+            "name": "JSONLoader",
+            "p": 1,
+            "skip_rejected": true,
+            "key": "text",
+            "ignore": true
+        }
+        },
+        {
+        "name": "1-DocumentNormalizer",
+        "discard_num": 0,
+        "diff_MB": -1.5221118927001953,
+        "cumulative_time": 8.286988707,
+        "params": {
+            "name": "DocumentNormalizer",
+            "p": 1,
+            "skip_rejected": true
+        }
+        },
+        {
+        "name": "2-DocumentLengthFilter",
+        "discard_num": 344,
+        "diff_MB": -0.05566596984863281,
+        "cumulative_time": 0.093768306,
+        "params": {
+            "name": "DocumentLengthFilter",
+            "p": 1,
+            "skip_rejected": true,
+            "min_doc_len": 100,
+            "max_doc_len": null
+        }
+        },
+    ]
+    }
+    ```
 
-It might be helpful to add examples demonstrating the use of `Compose
+- `Compose.statistics_obj` is a `hojichar.StatsContainer` class. The `hojichar.StatsContainer` class stores the raw values of the statistics dictionary, and addition operations are defined to easily calculate the total statistics processed with the same filter. You can get the statistics dictionary by calling `Compose.statistics_obj.get_human_readable_values()`.
+
+## Parallel application of `Compose`
+
+The `hojichar.Parallel` class allows for the application of `Compose` to an iterable of `Document` concurrently. This class empowers users to process vast collections of documents by harnessing the power of multiple CPU cores.
+
+Example usage of `Parallel` class to proces a very large JSON Lines file concurrently.
+
+```python
+import hojichar
+
+input_file = "your_text.jsonl"
+input_doc_iter = (hojichar.Document(line) for line in open(input_file))
+
+cleaner = hojichar.Compose([
+    hojichar.document_filters.JSONLoader(),
+    hojichar.document_filters.DocumentNormalizer(),
+    # Insert your filters
+    hojichar.document_filters.JSONDumper(),
+])
+
+with hojichar.Parallel(cleaner, num_jobs=10) as pfilter:
+    out_doc_iter = pfilter.imap_apply(input_doc_iter)
+    with open("your_processed_text.jsonl", "w") as fp:
+        for doc in out_doc_iter:
+            fp.write(doc.text + "\n")
+
+```
+
+- Always use the `Parallel` class within a `with` statement.
+- `Parallel.imap_apply(doc_iter)` processes an iterator of `Document` and returns an iterator of the processed documents.
+- For additional options and details about the `Parallel` class, please refer to the official documentation.
 
 ## CLI tool and preprocessing profile
 
 - HojiChar provides CLI tools for text preprocess pipeline.
 - User defines a series of preprocessing into a python file as profile.
 
 - Example:
```

