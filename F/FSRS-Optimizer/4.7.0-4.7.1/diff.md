# Comparing `tmp/FSRS-Optimizer-4.7.0.tar.gz` & `tmp/FSRS-Optimizer-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.7.0.tar", last modified: Sun Aug  6 05:27:31 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.7.1.tar", last modified: Tue Aug  8 05:33:59 2023, max compression
```

## Comparing `FSRS-Optimizer-4.7.0.tar` & `FSRS-Optimizer-4.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.023194 FSRS-Optimizer-4.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.023194 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53118 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:33:59.786561 FSRS-Optimizer-4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-08 05:33:59.786561 FSRS-Optimizer-4.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 05:33:59.786561 FSRS-Optimizer-4.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:33:59.782561 FSRS-Optimizer-4.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:33:59.786561 FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-08 05:33:59.000000 FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-08 05:33:59.000000 FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:33:59.000000 FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-08 05:33:59.000000 FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 05:33:59.000000 FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:33:59.786561 FSRS-Optimizer-4.7.1/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53476 2023-08-08 05:33:43.000000 FSRS-Optimizer-4.7.1/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.7.0/LICENSE` & `FSRS-Optimizer-4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.7.0/PKG-INFO` & `FSRS-Optimizer-4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.7.0
+Version: 4.7.1
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.7.0/README.md` & `FSRS-Optimizer-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.7.1/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.7.0
+Version: 4.7.1
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.7.0/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.7.1/src/fsrs_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.7.0/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.7.1/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -550,20 +550,27 @@
                 ax.set_ylim(0, 1)
                 ax.set_xlabel('Interval')
                 ax.set_ylabel('Recall')
                 ax.set_title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
                 plots.append(fig)
                 tqdm.write(str(rating_stability))
 
+        for a, b in ((1, 2), (2, 3), (3, 4)):
+            if a in rating_stability and b in rating_stability:
+                if rating_stability[a] > rating_stability[b]:
+                    if rating_count[a] > rating_count[b]:
+                        rating_stability[b] = rating_stability[a]
+                    else:
+                        rating_stability[a] = rating_stability[b]
+
         if len(rating_stability) == 0:
             raise Exception("Not enough data for pretraining!")
         elif len(rating_stability) == 1:
             init_stability = round(list(rating_stability.values())[0], 2)
-            for i in (0, 1, 2, 3):
-                self.init_w[i] = init_stability
+            self.init_w[0:4] = [init_stability] * 4
         elif len(rating_stability) == 4:
             for rating, stability in rating_stability.items():
                 self.init_w[rating-1] = round(stability, 2)
             tqdm.write(f"Pretrain finished!")
             return plots
 
         def S0_rating_curve(rating, a, b, c):
```

