# Comparing `tmp/lamin_utils-0.9.6.tar.gz` & `tmp/lamin_utils-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_utils-0.9.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_utils-0.9.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_utils-0.9.6.tar` & `lamin_utils-0.9.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.6/.gitignore
--rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.6/LICENSE
--rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.6/README.md
--rw-r--r--   0        0        0     7427 2023-08-07 21:21:21.089473 lamin_utils-0.9.6/docs/changelog.md
--rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.6/docs/quickstart.ipynb
--rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.6/lamin-project.yaml
--rw-r--r--   0        0        0      161 2023-08-07 21:21:25.502331 lamin_utils-0.9.6/lamin_utils/__init__.py
--rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.6/lamin_utils/_core.py
--rw-r--r--   0        0        0     6297 2023-08-07 21:20:51.602321 lamin_utils-0.9.6/lamin_utils/_inspect.py
--rw-r--r--   0        0        0     7658 2023-08-07 19:41:59.385758 lamin_utils-0.9.6/lamin_utils/_logger.py
--rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.6/lamin_utils/_lookup.py
--rw-r--r--   0        0        0     6843 2023-08-06 16:55:32.281387 lamin_utils-0.9.6/lamin_utils/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.6/lamin_utils/_python_version.py
--rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.6/lamin_utils/_search.py
--rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.6/noxfile.py
--rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.6/pyproject.toml
--rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.6/tests/test_base.py
--rw-r--r--   0        0        0     5167 2023-08-07 21:20:51.602628 lamin_utils-0.9.6/tests/test_inspect.py
--rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.6/tests/test_lookup.py
--rw-r--r--   0        0        0     5700 2023-08-07 21:20:51.602941 lamin_utils-0.9.6/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.6/tests/test_notebooks.py
--rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.6/tests/test_search.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.7/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.7/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.7/.gitignore
+-rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.7/LICENSE
+-rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.7/README.md
+-rw-r--r--   0        0        0     7582 2023-08-08 16:12:27.486317 lamin_utils-0.9.7/docs/changelog.md
+-rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.7/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.7/lamin-project.yaml
+-rw-r--r--   0        0        0      161 2023-08-08 16:13:04.031652 lamin_utils-0.9.7/lamin_utils/__init__.py
+-rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.7/lamin_utils/_core.py
+-rw-r--r--   0        0        0     7270 2023-08-08 16:12:27.486674 lamin_utils-0.9.7/lamin_utils/_inspect.py
+-rw-r--r--   0        0        0     7658 2023-08-07 19:41:59.385758 lamin_utils-0.9.7/lamin_utils/_logger.py
+-rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.7/lamin_utils/_lookup.py
+-rw-r--r--   0        0        0     6843 2023-08-06 16:55:32.281387 lamin_utils-0.9.7/lamin_utils/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.7/lamin_utils/_python_version.py
+-rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.7/lamin_utils/_search.py
+-rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.7/noxfile.py
+-rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.7/tests/test_base.py
+-rw-r--r--   0        0        0     5150 2023-08-08 16:12:27.486990 lamin_utils-0.9.7/tests/test_inspect.py
+-rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.7/tests/test_lookup.py
+-rw-r--r--   0        0        0     5700 2023-08-07 21:20:51.602941 lamin_utils-0.9.7/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.7/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.7/tests/test_search.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.7/PKG-INFO
```

### Comparing `lamin_utils-0.9.6/.github/workflows/build.yml` & `lamin_utils-0.9.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/.github/workflows/latest-changes.yml` & `lamin_utils-0.9.7/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/.gitignore` & `lamin_utils-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/.pre-commit-config.yaml` & `lamin_utils-0.9.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/LICENSE` & `lamin_utils-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/docs/changelog.md` & `lamin_utils-0.9.7/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Refactored validate and inspect | [52](https://github.com/laminlabs/lamin-utils/pull/52) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-08 |
 ✨ Add InspectResult | [51](https://github.com/laminlabs/lamin-utils/pull/51) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-07 |
 🎨 Rename download to save logging level | [50](https://github.com/laminlabs/lamin-utils/pull/50) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-07 | 0.9.5
 🎨 Simplified params in inspect | [48](https://github.com/laminlabs/lamin-utils/pull/48) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-06 | 0.9.4
 🚸 Introduce success-level verbosity | [49](https://github.com/laminlabs/lamin-utils/pull/49) | [falexwolf](https://github.com/falexwolf) | 2023-08-06 |
 Round percentages for mapping | [47](https://github.com/laminlabs/lamin-utils/pull/47) | [Zethson](https://github.com/Zethson) | 2023-07-31 |
 🐛 Fix for categorical index | [45](https://github.com/laminlabs/lamin-utils/pull/45) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.3
 ✨ Added italic and underline | [44](https://github.com/laminlabs/lamin-utils/pull/44) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.2
```

### Comparing `lamin_utils-0.9.6/docs/quickstart.ipynb` & `lamin_utils-0.9.7/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/lamin_utils/_core.py` & `lamin_utils-0.9.7/lamin_utils/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/lamin_utils/_logger.py` & `lamin_utils-0.9.7/lamin_utils/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/lamin_utils/_lookup.py` & `lamin_utils-0.9.7/lamin_utils/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/lamin_utils/_map_synonyms.py` & `lamin_utils-0.9.7/lamin_utils/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/lamin_utils/_python_version.py` & `lamin_utils-0.9.7/lamin_utils/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/lamin_utils/_search.py` & `lamin_utils-0.9.7/lamin_utils/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/pyproject.toml` & `lamin_utils-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/tests/test_inspect.py` & `lamin_utils-0.9.7/tests/test_inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,12 +180,12 @@
         case_sensitive=True,
     ).tolist() == [True, False]
     assert validate(
         identifiers=["A1CF", "a1cf"],
         field_values=df["symbol"],
         case_sensitive=False,
         return_df=True,
-    )["__validated__"].tolist() == [True, True]
+    ).tolist() == [True, True]
     assert validate(
         identifiers=df["symbol"],
         field_values=df["symbol"],
     ).tolist() == [True, True, True]
```

### Comparing `lamin_utils-0.9.6/tests/test_lookup.py` & `lamin_utils-0.9.7/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/tests/test_map_synonyms.py` & `lamin_utils-0.9.7/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/tests/test_search.py` & `lamin_utils-0.9.7/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.6/PKG-INFO` & `lamin_utils-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_utils
-Version: 0.9.6
+Version: 0.9.7
 Summary: Lamin Utils.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

