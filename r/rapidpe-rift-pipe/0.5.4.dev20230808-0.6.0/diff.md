# Comparing `tmp/rapidpe_rift_pipe-0.5.4.dev20230808.tar.gz` & `tmp/rapidpe_rift_pipe-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230808.tar", last modified: Tue Aug  8 05:17:43 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.6.0.tar", last modified: Tue Aug  8 17:16:45 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.4.dev20230808.tar` & `rapidpe_rift_pipe-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.366299 rapidpe_rift_pipe-0.5.4.dev20230808/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1090 2023-08-08 05:17:43.367299 rapidpe_rift_pipe-0.5.4.dev20230808/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.360299 rapidpe_rift_pipe-0.5.4.dev20230808/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.362299 rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-08-08 05:17:43.368299 rapidpe_rift_pipe-0.5.4.dev20230808/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.360299 rapidpe_rift_pipe-0.5.4.dev20230808/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.364299 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.366299 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.366299 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31210 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.366299 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-08-08 05:17:30.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:17:43.366299 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-08-08 05:17:43.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-08-08 05:17:43.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 05:17:43.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-08-08 05:17:43.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-08-08 05:17:43.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-08 05:17:43.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 05:17:42.000000 rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.685182 rapidpe_rift_pipe-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-08-08 17:16:45.685182 rapidpe_rift_pipe-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.678182 rapidpe_rift_pipe-0.6.0/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.680182 rapidpe_rift_pipe-0.6.0/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2023-08-08 17:13:56.000000 rapidpe_rift_pipe-0.6.0/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-08-08 17:16:45.686182 rapidpe_rift_pipe-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.678182 rapidpe_rift_pipe-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.683182 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-08-08 17:13:56.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18558 2023-08-08 17:13:56.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.684182 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 17:16:35.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.684182 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 17:16:35.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31210 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-08-08 17:13:56.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27651 2023-08-08 17:13:56.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.685182 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 17:16:35.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-08-02 05:13:14.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 17:16:45.684182 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 17:16:45.000000 rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/COPYING` & `rapidpe_rift_pipe-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/PKG-INFO` & `rapidpe_rift_pipe-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.5.4.dev20230808
+Version: 0.6.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.6.0/bin/postscripts/compute_posterior.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 """
 Generates posterior plots from RapidPE/RIFT results
 """
 
 __author__ = "Vinaya Valsan"
 
 import os
-
-import numpy as np
 import logging
+import json
+import numpy as np
+
+import requests.exceptions
 
 import rapidpe_rift_pipe.postscript_utils as postutils
 
+from argparse import ArgumentParser
+from ligo.gracedb.rest import GraceDb
 from rapidpe_rift_pipe.config import Config
 from rapidpe_rift_pipe import pastro, utils
-from argparse import ArgumentParser
 from rapid_pe import amrlib
 from rapid_pe.amrlib import VALID_TRANSFORMS_MASS
 
 print("-------------------Plotting intrinsic posteriors----------------------")
 
 logging.basicConfig(level=logging.INFO)
 
@@ -178,45 +181,49 @@
     grid_data_dict, grid_param_list, sigma_factor, grid_level=use_grid_level
 )
 
 
 grid_levels = np.unique(grid_data_dict["iteration_level"])
 
 if config.pastro.mode == "enabled":
+    starting_gracedb_id = event_info_dict["gracedb_id"]
+    client = GraceDb(config.gracedb_url)
+    starting_gevent = client.event(starting_gracedb_id).json()
+    superevent_id = starting_gevent["superevent"]
     channel_names = event_info_dict["channel_name"]
     if "INJ" in channel_names:
         rate_dict = config.pastro.category_rates_inj
     else:
         rate_dict = config.pastro.category_rates
     prior_boundary_dict = config.pastro.prior_boundary
     evidence = postutils.compute_evidence(
         grid_data_dict,
         prior_boundary_dict,
         sigma_dict,
         prior_function="salpeter",
         distance_coordinates_str=distance_coordinates_str,
     )
+    try:
+        pastro_file = client.files(superevent_id, "gstlal.p_astro.json")
+        p_terr = json.load(pastro_file)["Terrestrial"]
+        p_astro = pastro.pastro(
+            rate_dict=rate_dict, evidence_dict=evidence, p_terr=p_terr
+        )
 
-    p_astro = pastro.pastro(
-        evidence_dict=evidence,
-        rankstatpdf_file=config.pastro.rankstat_pdf_file,
-        likelihood=event_info_dict["likelihood"],
-        rate_dict=rate_dict,
-        far_threshold=config.pastro.far_threshold,
-    )
-
-    pastro_dict = p_astro.compute_pastro()
-    pastro.plot_pastro(pastro_dict, summary_plots_dir)
-    utils.save_as_json(
-        pastro_dict, os.path.join(summary_plots_dir, "p_astro.json")
-    )
+        pastro_dict = p_astro.compute_pastro()
+        pastro.plot_pastro(pastro_dict, summary_plots_dir)
+        utils.save_as_json(
+            pastro_dict, os.path.join(summary_plots_dir, "p_astro.json")
+        )
 
-    utils.save_as_json(
-        evidence, os.path.join(summary_plots_dir, "evidence.json")
-    )
+        utils.save_as_json(
+            evidence, os.path.join(summary_plots_dir, "evidence.json")
+        )
+    except requests.exceptions.HTTPError:
+        logging.exception(f"No gstlal.p_astro.json found for {superevent_id}")
 sample_dict = postutils.get_posterior_samples(
     grid_data_dict,
     sigma_dict,
     grid_level=use_grid_level,
     spin_included=grid_in_4dimensions,
     distance_coordinates_str=distance_coordinates_str,
 )
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.6.0/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.6.0/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.6.0/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.6.0/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/setup.cfg` & `rapidpe_rift_pipe-0.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230808
+tag_build = 
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,18 +578,12 @@
         },
         "category_rates_inj": {
             "parser": parse_dict,
         },
         "prior_boundary": {
             "parser": parse_dict,
         },
-        "rankstat_pdf_file": {
-            "parser": parse_str,
-        },
-        "far_threshold": {
-            "parser": parse_float,
-        }
     },
     "disabled" : {}
 }
 
 PastroConfig = _make_config_group("PastroConfig", "Pastro", _pastro_group_spec)
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,18 +137,15 @@
             data_dict["mass2"].append(row.mass2)
             data_dict["margll"].append(row.snr)
             data_dict["iteration_level"].append(i)
             if check_spin:
                 try:
                     data_dict["spin1z"].append(row.spin1z)
                     data_dict["spin2z"].append(row.spin2z)
-                    (
-                        chi_eff,
-                        chi_a,
-                    ) = amrlib.transform_s1zs2z_chi_eff_chi_a(
+                    (chi_eff, chi_a,) = amrlib.transform_s1zs2z_chi_eff_chi_a(
                         row.mass1, row.mass2, row.spin1z, row.spin2z
                     )
                     data_dict["chi_eff"].append(chi_eff)
                     data_dict["chi_a"].append(chi_a)
                 except AttributeError:
                     check_spin = False
                     print("No spin information found in SnglInspiralTable")
@@ -326,14 +323,17 @@
     grid_data,
     prior_boundary_dict,
     sigma,
     distance_coordinates_str,
     prior_function="uniform",
     grid_level=None,
 ):
+    """
+    Computes total evidence and category-wise evidence
+    """
     prior_function = prior_function.lower()
 
     m_max_bank = prior_boundary_dict["m_max_bank"]
     m_min_bank = prior_boundary_dict["m_min_bank"]
     m_max_ns = prior_boundary_dict["m_max_ns"]
 
     count_evidence = count_bbh = count_bns = count_nsbh = 0
@@ -555,17 +555,17 @@
         count_evidence += count_evidence_i
         count_bns += count_bns_i
         count_nsbh += count_nsbh_i
         count_bbh += count_bbh_i
 
     return {
         "evidence": count_evidence,
-        "evidence_BNS": count_bns,
-        "evidence_NSBH": count_nsbh,
-        "evidence_BBH": count_bbh,
+        "BNS": count_bns,
+        "NSBH": count_nsbh,
+        "BBH": count_bbh,
     }
 
 
 def plot_grid(
     grid_data,
     param1,
     param2,
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.5.4.dev20230808
+Version: 0.6.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230808/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.6.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

