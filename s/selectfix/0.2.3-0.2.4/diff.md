# Comparing `tmp/selectfix-0.2.3.tar.gz` & `tmp/selectfix-0.2.4.tar.gz`

## Comparing `selectfix-0.2.3.tar` & `selectfix-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.3/Cargo.toml
--rw-r--r--   0     1001      123     1272 2023-08-04 02:22:20.000000 selectfix-0.2.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1046 2023-08-04 02:22:20.000000 selectfix-0.2.3/.github/workflows/_workflow.yml
--rw-r--r--   0     1001      123      685 2023-08-04 02:22:20.000000 selectfix-0.2.3/.gitignore
--rw-r--r--   0     1001      123      125 2023-08-04 02:22:20.000000 selectfix-0.2.3/README.md
--rw-r--r--   0     1001      123      313 2023-08-04 02:22:20.000000 selectfix-0.2.3/pyproject.toml
--rw-r--r--   0     1001      123    12925 2023-08-04 02:22:20.000000 selectfix-0.2.3/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-08-04 02:22:20.000000 selectfix-0.2.3/tests/__init__.py
--rw-r--r--   0     1001      123     3281 2023-08-04 02:22:20.000000 selectfix-0.2.3/tests/test_selectfix.py
--rw-r--r--   0     1001      123     8559 2023-08-04 02:22:20.000000 selectfix-0.2.3/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      123     1272 2023-08-08 05:01:22.000000 selectfix-0.2.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1046 2023-08-08 05:01:22.000000 selectfix-0.2.4/.github/workflows/_workflow.yml
+-rw-r--r--   0     1001      123      685 2023-08-08 05:01:22.000000 selectfix-0.2.4/.gitignore
+-rw-r--r--   0     1001      123      125 2023-08-08 05:01:22.000000 selectfix-0.2.4/README.md
+-rw-r--r--   0     1001      123      313 2023-08-08 05:01:22.000000 selectfix-0.2.4/pyproject.toml
+-rw-r--r--   0     1001      123    12922 2023-08-08 05:01:22.000000 selectfix-0.2.4/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-08-08 05:01:22.000000 selectfix-0.2.4/tests/__init__.py
+-rw-r--r--   0     1001      123     3278 2023-08-08 05:01:22.000000 selectfix-0.2.4/tests/test_selectfix.py
+-rw-r--r--   0     1001      123     8559 2023-08-08 05:01:22.000000 selectfix-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.4/PKG-INFO
```

### Comparing `selectfix-0.2.3/.github/workflows/CI.yml` & `selectfix-0.2.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.3/.github/workflows/_workflow.yml` & `selectfix-0.2.4/.github/workflows/_workflow.yml`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.3/.gitignore` & `selectfix-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.3/src/lib.rs` & `selectfix-0.2.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 /// x = {"x1": 0.0, "x2": 2.0, "x3": 0.0}
 /// selectfix(x) # 0.0
 /// ```
 ///
 /// ## Ranges
 /// A range of values can be penalized for an unfixed variable.
 /// ```py
-/// selectfix = SelectFix(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (1.0, 2.0), "x2": (3.0, 4.0)}, None, 0.0)
+/// selectfix = SelectFix(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (1.0, 2.0), "x2": (3.0, 4.0)}, 1, 0.0)
 /// ```
 /// This adds a penalty if x1 is chosen as an unfixed variable and x1 is not in the range 1.0~2.0.
 /// ```py
 /// x = {"x1": 3.0, "x2": 3.0, "x3": 0.0}
 /// selectfix(x) # -1.0
 /// x = {"x1": 1.5, "x2": 3.0, "x3": 0.0}
 /// selectfix(x) # 0.0
@@ -195,15 +195,15 @@
                     OrderedFloat(0.0)
                 }
             })
             .collect::<Vec<_>>();
         additional_penalty_indices.sort_by_key(|i| additional_penalties[*i - self.n_select_min]);
         let additional_penalty_indices = additional_penalty_indices
             .into_iter()
-            .take(num_candidates - self.n_select_max.unwrap_or(self.n_select_min))
+            .take(num_candidates - self.n_select_max.unwrap_or(num_candidates))
             .collect::<Vec<_>>();
         (
             additional_penalty_indices
                 .iter()
                 .map(|i| additional_penalties[*i - self.n_select_min])
                 .collect::<Vec<_>>(),
             additional_penalty_indices,
@@ -217,15 +217,15 @@
     ///
     /// # Arguments
     /// * `n_select_min` - The minimum number of variables to be selected to fix.
     /// * `candidates` - Candidates for selection.
     /// * `excluded_unfixed_combinations` - Combinations you want to exclude among unfixed variables.
     /// * `fixed_val` - Target value of variable to be fixed.
     /// * `ranges` - Range to be set on unfixed variables.
-    /// * `n_select_max` - The maximum number of variable to be selected to fix. If None, n_select_max = n_select_min.
+    /// * `n_select_max` - The maximum number of variable to be selected to fix. If None, n_select_max = len(candidates).
     /// * `eps` - Tolerance for fixed variables and fixed_val.
     #[new]
     fn new(
         n_select_min: usize,
         candidates: Vec<String>,
         excluded_unfixed_combinations: Vec<Vec<String>>,
         fixed_val: f64,
```

### Comparing `selectfix-0.2.3/tests/test_selectfix.py` & `selectfix-0.2.4/tests/test_selectfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         assert val == -24
         np.testing.assert_array_equal(
             sel.jacobian({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10}), np.array([1, 0, 0, 0, 1])
         )
         np.testing.assert_array_equal(sel.hessian({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10}), np.zeros((5, 5)))
 
     def test_selectfix_using_range_penalty(self):
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, None, 0.0)
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, 1, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0})
         assert val == -10
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0}), np.array([1, 0, 1]))
 
     def test_selectfix_using_range_penalty_and_n_select_max(self):
         sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, 2, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0})
```

### Comparing `selectfix-0.2.3/Cargo.lock` & `selectfix-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "selectfix"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "anyhow",
  "bincode",
  "indexmap",
  "ordered-float",
  "pyo3",
  "serde",
```

