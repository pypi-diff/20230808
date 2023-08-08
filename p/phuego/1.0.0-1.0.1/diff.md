# Comparing `tmp/phuego-1.0.0.tar.gz` & `tmp/phuego-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phuego-1.0.0.tar", max compression
+gzip compressed data, was "phuego-1.0.1.tar", max compression
```

## Comparing `phuego-1.0.0.tar` & `phuego-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35148 2023-06-24 00:39:29.939522 phuego-1.0.0/LICENSE
--rw-r--r--   0        0        0    12797 2023-07-27 13:58:04.976766 phuego-1.0.0/README.md
--rw-r--r--   0        0        0     8261 2023-07-28 12:18:35.207468 phuego-1.0.0/phuego/CLI.py
--rw-r--r--   0        0        0      378 2023-07-28 11:43:56.516703 phuego-1.0.0/phuego/__init__.py
--rw-r--r--   0        0        0     1732 2023-07-06 14:06:11.571686 phuego-1.0.0/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt
--rw-r--r--   0        0        0     7993 2023-07-28 12:01:25.498832 phuego-1.0.0/phuego/ego.py
--rw-r--r--   0        0        0     4154 2023-07-28 12:02:56.330253 phuego-1.0.0/phuego/ego2module.py
--rw-r--r--   0        0        0    11293 2023-08-01 09:10:35.379460 phuego-1.0.0/phuego/generate_net.py
--rw-r--r--   0        0        0     2588 2023-07-06 11:02:58.380783 phuego-1.0.0/phuego/load_seeds.py
--rw-r--r--   0        0        0     9723 2023-07-29 23:03:51.496384 phuego-1.0.0/phuego/network_rwr.py
--rw-r--r--   0        0        0     9160 2023-07-31 14:40:44.672550 phuego-1.0.0/phuego/phuego.py
--rw-r--r--   0        0        0    27357 2023-07-30 13:23:28.032031 phuego-1.0.0/phuego/phuego_mock.py
--rw-r--r--   0        0        0    12036 2023-07-30 14:33:29.762559 phuego-1.0.0/phuego/utils.py
--rw-r--r--   0        0        0     3177 2023-07-28 11:05:51.934526 phuego-1.0.0/phuego/utils_CLI.py
--rw-r--r--   0        0        0      956 2023-07-28 12:18:45.976867 phuego-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    13823 1970-01-01 00:00:00.000000 phuego-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-24 00:39:29.939522 phuego-1.0.1/LICENSE
+-rw-r--r--   0        0        0    21048 2023-08-08 09:35:50.484393 phuego-1.0.1/README.md
+-rw-r--r--   0        0        0     8261 2023-08-08 09:19:45.986357 phuego-1.0.1/phuego/CLI.py
+-rw-r--r--   0        0        0      378 2023-07-28 11:43:56.516703 phuego-1.0.1/phuego/__init__.py
+-rw-r--r--   0        0        0     1732 2023-07-06 14:06:11.571686 phuego-1.0.1/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt
+-rw-r--r--   0        0        0     7993 2023-07-28 12:01:25.498832 phuego-1.0.1/phuego/ego.py
+-rw-r--r--   0        0        0     4154 2023-07-28 12:02:56.330253 phuego-1.0.1/phuego/ego2module.py
+-rw-r--r--   0        0        0    11293 2023-08-01 09:10:35.379460 phuego-1.0.1/phuego/generate_net.py
+-rw-r--r--   0        0        0     2588 2023-07-06 11:02:58.380783 phuego-1.0.1/phuego/load_seeds.py
+-rw-r--r--   0        0        0     9723 2023-07-29 23:03:51.496384 phuego-1.0.1/phuego/network_rwr.py
+-rw-r--r--   0        0        0     9160 2023-07-31 14:40:44.672550 phuego-1.0.1/phuego/phuego.py
+-rw-r--r--   0        0        0    27357 2023-07-30 13:23:28.032031 phuego-1.0.1/phuego/phuego_mock.py
+-rw-r--r--   0        0        0    12036 2023-07-30 14:33:29.762559 phuego-1.0.1/phuego/utils.py
+-rw-r--r--   0        0        0     3177 2023-07-28 11:05:51.934526 phuego-1.0.1/phuego/utils_CLI.py
+-rw-r--r--   0        0        0      956 2023-08-08 09:19:55.474108 phuego-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    22074 1970-01-01 00:00:00.000000 phuego-1.0.1/PKG-INFO
```

### Comparing `phuego-1.0.0/LICENSE` & `phuego-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/CLI.py` & `phuego-1.0.1/phuego/CLI.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .utils_CLI import load_test_example
 from .utils_CLI import dataprep
 from .phuego import phuego
 from .phuego_mock import phuego_mock
 import click
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 '''
 This is the CLI tool for phuego.
 '''
 @click.command()
 # Folders.
 @click.option("--support_data_folder", "-sf", type=str, required=False,
```

### Comparing `phuego-1.0.0/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt` & `phuego-1.0.1/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/ego.py` & `phuego-1.0.1/phuego/ego.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/ego2module.py` & `phuego-1.0.1/phuego/ego2module.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/generate_net.py` & `phuego-1.0.1/phuego/generate_net.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/load_seeds.py` & `phuego-1.0.1/phuego/load_seeds.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/network_rwr.py` & `phuego-1.0.1/phuego/network_rwr.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/phuego.py` & `phuego-1.0.1/phuego/phuego.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/phuego_mock.py` & `phuego-1.0.1/phuego/phuego_mock.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/utils.py` & `phuego-1.0.1/phuego/utils.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/phuego/utils_CLI.py` & `phuego-1.0.1/phuego/utils_CLI.py`

 * *Files identical despite different names*

### Comparing `phuego-1.0.0/pyproject.toml` & `phuego-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phuego"
-version = "1.0.0"
+version = "1.0.1"
 description = "Propagation of phosphoproteomics signals"
 authors = [
     "Girolamo Giudice <Girolamo.Giudice@gmail.com>",
     "Haoqi Chen <haoqichen20@gmail.com>",
     "Evangelia Petsalaki <petsalaki@ebi.ac.uk>"
 ]
 readme = "README.md"
```

### Comparing `phuego-1.0.0/PKG-INFO` & `phuego-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,142 +1,148 @@
-Metadata-Version: 2.1
-Name: phuego
-Version: 1.0.0
-Summary: Propagation of phosphoproteomics signals
-Home-page: https://github.com/haoqichen20/phuego
-License: GPL-3.0-only
-Keywords: Phosphoproteomics,network propagation
-Author: Girolamo Giudice
-Author-email: Girolamo.Giudice@gmail.com
-Maintainer: Haoqi Chen
-Maintainer-email: haoqichen20@gmail.com
-Requires-Python: >=3.9,<3.13
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3)
-Requires-Dist: igraph (>=0.10.2)
-Requires-Dist: leidenalg (>=0.9.0)
-Requires-Dist: numpy (>=1.24.3)
-Requires-Dist: pandas (>=2.0.1)
-Requires-Dist: requests (>2.29.0)
-Requires-Dist: scikit-learn (>=1.2.2)
-Requires-Dist: scipy (>=1.10.1)
-Project-URL: Repository, https://github.com/haoqichen20/phuego
-Description-Content-Type: text/markdown
-
 <img src="https://github.com/haoqichen20/phuego/blob/master/docs/images/logo.png" width="400">
 
 ### phuEGO: a network-based method to reconstruct active signalling pathways from phosphoproteomics datasets
 ---
 
-phuego is a network-based method to reconstruct active signalling pathways from phosphoproteomics datasets. It combines three-layer network propagation with ego network decomposition to provide small networks comprising active functional signalling modules. PhuEGO boosts the signal-to-noise ratio from global phosphoproteomics datasets, enriches the resulting networks for functional phosphosites and allows the improved comparison and integration across datasets.
+phuEGO is a network-based method to reconstruct active signalling pathways from phosphoproteomics datasets. It combines three-layer network propagation with ego network decomposition to provide small networks comprising active functional signalling modules. PhuEGO boosts the signal-to-noise ratio from global phosphoproteomics datasets, enriches the resulting networks for functional phosphosites and allows the improved comparison and integration across datasets.
 
-To run phuego, the user can either directly calls the CLI application from command line, or integrate the python functions into their own script. Both methods work equivalently, and it's up to the user to decide which method suits their work.
+To run phuEGO, the user can either directly calls the [CLI](#2-using-the-cli) application from command line, or integrate the [python functions](#3-using-the-python-package) into their own script. We recommend the user to use the CLI and submit jobs to a server where possible, to ensure robust execution of the tasks.
 
-## Installation
+## 1. Installation
 
 ```bash
-# Install phuego in your python environment with 3.13 > python > 3.9
+# Install phuEGO in your python environment with 3.13 > python > 3.9
 pip install phuego
 # Check version to ensure successful installation.
 phuego --version
 # Check all parameters of CLI application.
 phuego --help
 ```
 
-## Using the CLI
+## 2. Using the CLI
+
+The CLI application is an easy way to run phuEGO on single or a whole batch of dataset directly from the command line. 
 
-The CLI application is an easy way to run phuego on single or a whole batch of dataset directly from the command line. 
+**Specific note for Windows users**: please provide the paths with forward slash '/' instead of backward slash '\\'.
 
-### 1. Downloading supporting dataset.
-When using phuego **for the first time**, a support dataset that contains three files (https://zenodo.org/record/8094690) need to be downloaded. After that, the user could always refer to the support data folder for running phuego. 
+### 1). Downloading supporting dataset
+When using phuEGO **for the first time**, a support dataset that contains three zipped files (https://zenodo.org/record/8094690) need to be downloaded. After that, the user could always refer to the support data folder for running phuEGO. 
 
 To download using the CLI application, the user could run the following. Make sure the target disk has at least **20 gb** of free space. 
 
 ```bash
 # Download all three dataset, compare md5 checksum, unzip and removed zip files.
 phuego -sf "path/to/desired/folder/" --need_fisher True --need_gic_sim True --need_networks True --remove_zip_file True
 
 # If one of the file does not successfully download, for example the network file, then rerun above with only the missing file.
 phuego -sf "path/to/desired/folder/" --need_networks True --remove_zip_file True
 ```
 
-### 2. Performing a test/mock run with the phuego test dataset.
-phuego contains a test dataset, which is a list of differentially phosphorylated proteins between untreated cells and those treated with epidermal growth factor (EGF) (PMID: 19651622). 
-
-To understand the input and output of phuego, the user could perform a test run or a mock run using the test dataset. A test run is a complete run with 1000 propagation on randomized networks, and typically takes > 1hr to finish. A mock run performs 10 propagations and thus isn't sufficient for reliable statistical testing, but it typically finish within a few minutes and can help understand the format of input and output. 
+### 2). Performing a test/mock run with the phuEGO test dataset
+Phuego contains a test dataset, which is a list of differentially phosphorylated proteins between untreated cells and those treated with epidermal growth factor (EGF) (PMID: 19651622). To view the test dataset, see [here](#2-checking-the-input-data).
 
-Both test will print the head of the test dataset to standard output. To view the full test dataset, see next session "Using the python package: understanding the input data."
+To understand the [input](#2-input) and [output](#3-output) of phuEGO, the user could either perform a mock run or a test run using the test dataset. A mock run performs 10 propagations on randomized networks, and thus isn't sufficient for reliable statistics, but typically finishs within a few minutes. A test run is a complete run with 1000 propagation on randomized networks, and typically takes > 1hr to finish.
 
 ```bash
 # Performing a mock run.
-phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -mock -c2f
+phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" --run_mock
+
+# Performing a mock run, with two kde_cutoff and two geneset database for geneset enrichment analysis.
+phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" --run_mock -k 0.85 -k 0.9 -fg "K" -fg "B"
 
 # Performing a test run.
-phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -test True
+phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" --run_test
 ```
 
-### 3. Running your own protein list.
-To run phuego using your own list of protein, the data should be formatted in the same way as the test dataset. For detailed explanation of parameters, see section "Further documentations".
+### 3). Running your own protein list, reusing rwr results
+To run phuEGO using your own list of protein, provide the input file path to phuEGO.
 
-**Important:** the network propagation step (rwr, random walk with restart) is the most time consuming step of phuego. For each protein list and each damping factor, a separate propagation would be run and the result will be stored in the provided result folder (pvalues.txt, rwr_scores.txt, start_seeds.txt). After this, the user can reuse the results (so make sure you don't delete them!) to test different KDE cutoff and perform gene set enrichment analysis with various geneset by setting **-ru True**.
+**Important:** the network propagation (rwr) step is the most time consuming step of phuEGO. For each combination of protein list and damping factor, a separate propagation would be run and the result will be stored in the provided result folder (pvalues.txt, rwr_scores.txt, start_seeds.txt). After this, the user can reuse the results (so make sure you don't delete them!) and test other parameters by providing flag **-ru**.
 
 ```bash
-# Performing a run for the first time with example parameters. 
-phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -tpath "path/to/protein_list.txt" -ru False -d 0.85 -k 0.85 -fg "B"
+# Performing a run for the first time. Set damping factor to be 0.85, kde_cutoff to be 0.85, and genesets to be 'KEGG'.
+phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -tpath "path/to/protein_list.txt" -d 0.85 -k 0.85 -fg "K"
 
-# Performing a run reusing network propagation result, testing two different KDE values, and two different gene sets.
-phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -tpath "path/to/protein_list.txt" -ru True -k 0.8 -k 0.9 -fg "C" -fg "K"
+# Performing a run reusing network propagation result, testing two different KDE values, and two different gene sets, and export the network in a different format.
+phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -tpath "path/to/protein_list.txt" -ru -k 0.8 -k 0.9 -fg "C" -fg "B" -nf "edgelist"
 ```
 
-### 4. (optional) Batch job submission (LSF cluster).
-Each phuego run works with one protein list and one damping factor. If you have multiple protein lists (e.g., from a set of experiment), and/or would like to test multiple damping factors, you could use a .sh script to call phuego multiple times, and submit jobs in batch manner. Below we provide a .sh script for a LSF cluster as an example.
+### 4). Batch job submission (LSF cluster)
+Each phuEGO run works with one protein list and one damping factor. If you have multiple protein lists (e.g., from a set of experiment), and/or would like to test multiple damping factors, you could use a .sh script to call phuEGO multiple times, and submit jobs in batch manner. Below we provide a .sh script for a LSF cluster as an example.
 
 To do so, first create a test_datasets.txt file that store the path to all your protein list files:
 
 ```text
 path/to/protein_list_1.txt
 path/to/protein_list_2.txt
 path/to/protein_list_3.txt
 ```
 
-Then submit your jobs using the following .sh script:
+Then submit your jobs using the following .sh script. The output will be organized into a two-layer folder structure under your specified result_dir. Modify argument value to suit your need.
 
 ```bash
 #!/bin/bash
 
-dataset_file="path/to/test_datasets.txt"  # Path to the dataset file
+# Path to the dataset file
+dataset_file="path/to/test_datasets.txt"
 
 # Read dataset names from the file into an array
 readarray -t datasets < "$dataset_file"
 
-# Iterate over each dataset and submit a job
-for (( i=0; i<${#datasets[@]}; i++ )); do
-    dataset="${datasets[i]}"
-    job_name="job_$((i+1))"  # Use numeric index as the job name
-    result_dir="./result/$job_name/"
+# Result folder.
+result_dir="path/to/result_dir"
+
+# Run phuEGO.
+i=0
+for line in "${datasets[@]}"; do
+    # Create numerical job name.
+    job_name="job_$((i+1))"
+    ((i++))
 
-    # Create the result directory for the current job
-    mkdir -p "$result_dir"
+    # Extract the last level from the input.
+    experiment=$(echo "$line" | rev | cut -d'/' -f1 | rev)
     
-    # Submit the job using bsub with the desired job configuration and dataset
-    bsub -q standard -n 4 -M 4096 -R "rusage[mem=4096]" -o log_ph.txt -e err_ph.txt -J "$job_name" phuego -sf "./support_data/" -rf "$result_dir" -ru False -tpath "$dataset" -d 0.85 -k 0.85 -k 0.9 
+    # Create the experiment dir.
+    exp_dir="$pub_dir/$experiment"
+
+    dampings=(0.5 0.7 0.85)
+    for damping in "${dampings[@]}"; do
+        # Create the damping dir.
+        damping_dir="$exp_dir/$damping"
+        mkdir -p $damping_dir
+
+        # Run phuEGO with this damping factor, intact background and two kde_cutoff. 
+        # Run with 4 cores to increase the speed.
+        bsub -n 4 -M 4096 -R "rusage[mem=4096]" -o log.txt -e err.txt -J "$job_name"\
+        phuego -sf "Path/to/support_data/" -rf "$damping_dir" -tpath "$line" \
+        -d $damping -k 0.85 -k 0.9 -fg "B" -fg "K" -nf "graphml"
+    done
 done
 ```
 
+### 5). Running phuEGO with removed network nodes
+In a drugging or a knockout experiment, one might want to removed the knocked out targets from the reference network before performing network propagation, assuming that they are no longer functional. To do so, one could specify a .csv file as below, and provide to phuEGO:
 
+```text
+UniprotID_1,UniprotID_2,UniprotID_3
+UniprotID_1,UniprotID_2,UniprotID_3
+```
+
+Here, row 1 is a list of targets to be removed from the network propagation of upregulated input proteins, and row 2 for downregulated. Normally, one would expect these to be the same. The list can be provided as following:
+
+```bash
+# Performing a run for the first time. Set damping factor to be 0.85, kde_cutoff to be 0.85, and genesets to be 'KEGG'.
+phuego -sf "path/to/support_data_folder/" -rf "path/to/desired_result_folder/" -tpath "path/to/protein_list.txt" -ipath "path/to/targets_list.csv" -d 0.85 -k 0.85 -fg "K" 
+```
 
-## Using the python package.
+## 3. Using the python package
 
-The functions in the phuego package can be imported and used in your own python scripts. This makes it easier for integrating phuego into your own workflow.
+The functions in the phuEGO package can be imported and used in your own python scripts. This makes it easier for integrating phuEGO into your own workflow.
 
-### 1. Downloading supporting dataset.
+### 1). Downloading supporting dataset
 
 ```python
 from phuego import dataprep
 
 support_data_folder = "path/to/support_data_folder/"
 
 # Download support dataset. If the user wish the keep the zip files for easier 
@@ -145,61 +151,67 @@
 dataprep(support_data_folder=support_data_folder, 
             need_fisher=True, 
             need_gic_sim=True, 
             need_networks=True,
             remove_zip_file=True)
 ```
 
-### 2. Understanding the input data.
+### 2). Checking the input data
 ```python
 from phuego import load_test_example
 
 # The function return the absolute path of the test dataset, and the dataset itself as a dataframe.
 test_path, test_df = load_test_example()
 print(test_df)
 ```
 
-### 3. Performing a test/mock run with the phuego test dataset.
+### 3). Performing a test/mock run with the phuEGO test dataset
 
 Performing a mock run.
 
 ```python
 from phuego import phuego_mock
 
 # User input: paths.
 support_data_folder = "path/to/support_data_folder/"
 res_folder = "path/to/desired_result_folder/"
 
 # Loading the test dataset.
 test_path, test_df = load_test_example()
 
 # When calling the functions, the user need to manually set all parameters.
-fisher_geneset = ["C","F","D","P","R","K","RT","B"]
+fisher_geneset = ["B"]
 fisher_threshold = 0.05
 fisher_background = "intact"
 ini_pos = ["False"]
 ini_neg = ["False"]
 damping = 0.85
 kde_cutoff = [0.85]
 use_existing_rwr = False
+convert2folder=True
+include_isolated_egos_in_KDE_net=False
+net_format="graphml"
 
-# Run phuego mock.
+# Run phuEGO mock.
 print("Run phuego_mock with test dataset, whose first few lines are: \n",test_df.head())
 phuego_mock(
     support_data_folder=support_data_folder,
     res_folder=res_folder,
     test_path=test_path,
     fisher_geneset=fisher_geneset,
     fisher_threshold=fisher_threshold,
     fisher_background=fisher_background,
     ini_pos=ini_pos,
     ini_neg=ini_neg,
     damping=damping,
     kde_cutoff=kde_cutoff,
     use_existing_rwr=use_existing_rwr,
+    convert2folder=convert2folder,
+    include_isolated_egos_in_KDE_net=include_isolated_egos_in_kde_net,
+    net_format=net_format,
     )
 ```
 
 Performing a full test run.
 
 ```python
 from phuego import phuego
@@ -214,112 +226,193 @@
 # When calling the functions, the user need to manually set all parameters.
 fisher_geneset = ["B"]
 fisher_threshold = 0.05
 fisher_background = "intact"
 ini_pos = ["False"]
 ini_neg = ["False"]
 damping = 0.85
+rwr_threshold = 0.05
 kde_cutoff = [0.85]
 use_existing_rwr = False
+convert2folder=True
+include_isolated_egos_in_KDE_net=False
+net_format="graphml"
 
-# Run phuego with test dataset..
-print("Run phuego with test dataset, whose first few lines are: \n",test_df.head())
+# Run phuEGO with test dataset..
+print("Run phuEGO with test dataset, whose first few lines are: \n",test_df.head())
 phuego(
     support_data_folder=support_data_folder,
     res_folder=res_folder,
     test_path=test_path,
     fisher_geneset=fisher_geneset,
     fisher_threshold=fisher_threshold,
     fisher_background=fisher_background,
     ini_pos=ini_pos,
     ini_neg=ini_neg,
     damping=damping,
+    rwr_threshold=rwr_threshold,
     kde_cutoff=kde_cutoff,
     use_existing_rwr=use_existing_rwr,
+    convert2folder=convert2folder,
+    include_isolated_egos_in_KDE_net=include_isolated_egos_in_kde_net,
+    net_format=net_format,
     )
 ```
 
-### 4. Running your own protein list.
-To run phuego on your own protein list, simply provide the **test_path** to the above code, and remove the **load_test_example()** line. 
+### 4). Running your own protein list
+To run phuEGO on your own protein list, simply provide the **test_path** to the above code, and remove the **load_test_example()** line. 
 
 To reuse network propagation result and explore different KDE cutoff / genesets, set **use_existing_rwr = True** (also see above).
 
-## Detailed documentations.
-### Supporting dataset. 
-#### gic_sim folder, gic_sim_std.txt
-some text
-#### networks folder
-some text
-#### proteome and intact
-some text
-#### uniprot_to_gene.tab
-some text
-#### pfam_domains.txt
-some text
-
-### Input
-phuEGO accept in input a .txt file where first column are uniprot Ids and second columns are LFC or values associated to the importance of the protein in the first column.
-
-### Output
-#### pvalues.txt
-This file contains the pvalues for each node of the network. It is divided in seven columns, the first column refers to the uniprot ids.
+
+## 4. Data and results
+### 1). Supporting dataset. 
+The supporting datasets contain the base network, randomized networks, semantic similarity, geneset database etc. For details, refer to the associated [publication](#6-citation).
+
+### 2). Input
+phuEGO accept in input a .txt file where first column are uniprot Ids and second columns are LFC or values associated to the importance of the protein in the first column, such as the following. The user can also provide a .csv file for removed nodes, as explained [above](#5-running-phuego-with-removed-network-nodes).
+
+```text
+P29317	2.1043
+P00533	1.36255
+P10398	0.7655
+Q9UHY1	0.585
+P53999	-1.3219
+Q96II8	-1.3219
+P17096	-1.0
+P32519	-1.0
+```
+
+### 3). Output - overview
+Phuego output numerous files generated at each steps of the algorithm, organized into a folder structure. If the user prefer to navigate the files without the folder structure, they could set the flag **--dont_convert2folder** when using the CLI, or set **convert2folder=False** when using the python functions.
+
+phuEGO processed the user input in two regulation directions: 
+
+    - increased
+    - decreased
+
+In each direction, there are four levels of phuEGO output: 
+
+    - seeds
+    - rwr
+    - ego (subjected to KDE_cutoff)
+    - modules (subjected to KDE_cutoff)
+
+Depending on the levels, three types of files could be provided:
+
+    - protein lists
+    - networks
+    - fisher's exact test results
+
+In brief, a user input protein list (seeds) is divided into two directions using the scores (e.g., log2FCs). On each direction, it is expanded through network propagation into a very large list (rwr). Then this list is narrowed down (depending on where the user set the KDE_cutoff) by extracting only Ego network of seed nodes (ego), and further filtered by keeping inter-linked egos (modules). **The [modules](#4-output---module-networks) are considered the final result of phuEGO.** For details, refer to [publication](#6-citation).
+
+### 4). Output - module networks
+
+Module networks, generated by the Python igraph package, in an user specified format (via CLI parameter **-nf**). The default .graphml format contains information for module annotation, and can be readily imported into other software such as Cytoscape.
+
+    - decreased/KDE_cutoff/networks/module_net.graphml
+    - increased/KDE_cutoff/networks/module_net.graphml
+
+Files contains redundant information of the module networks in a more human-readable format.
+
+    - decreased/KDE_cutoff/networks/module_net_edgelist.csv
+    - decreased/KDE_cutoff/networks/module_net_nodes_attribute.csv
+    - increased/KDE_cutoff/networks/module_net_edgelist.csv
+    - increased/KDE_cutoff/networks/module_net_nodes_attribute.csv
+
+The network of the ego is also output at: 
+
+    - decreased/KDE_cutoff/networks/KDE.graphml
+    - increased/KDE_cutoff/networks/KDE.graphml
+
+### 5). Output - GSEA
+On each level, geneset enrichment analysis (fisher's exact test) are performed on the protein list, against an user specified geneset database. Through this, the user can examine whether phuEGO retrieves a more meaningful protein list from the seeds. The geneset database are part of the supporting database. In total, 8 databases are included, and one or more databases can be specified by providing abbreviation to the CLI arguments **--fg**. 
+
+    -P: enrichment against Gene Ontology biological process. Output file: Pfisher.txt
+    -F: enrichment against Gene Ontology functional . Output file: Ffisher.txt
+    -C: enrichment against Gene Ontology cellular component. Output file: Cfisher.txt
+    -K: enrichment against KEGG. Output file: Kfisher.txt
+    -R: enrichment against Reactome when only the leaves are consider as annotation. Output file: Rfisher.txt
+    -R: enrichment against Reactome when all the hierarchy is considered. Output file: Rfisher.txt
+    -D: enrichment against DisGenenet. Output file: Dfisher.txt
+    -B: enrichment against Bioplanet. Output file: Bfisher.txt
+
+They are distributed across the following paths:
+
+    - seeds: decreased/seed_fisher; increased/seed_fisher
+    - rwr: decreased/rwr_fisher; increased/rwr_fisher
+    - ego: decreased/KDE_cutoff/fisher; increased/KDE_cutoff/fisher
+    - modules: decreased/KDE_cutoff/modules/module_N/fisher; increased/KDE_cutoff/modules/module_N/fisher
+
+### 6). Output - protein list
+On the ego level, a text file summarize the protein list within ego network of each seed on a separate row. The first column is a seed node, the remaining column are the neighbors associated with the seed nodes. If **-ie** is provided to CLI, then rows with only the seeds will be excluded during network generation.
+
+    - decreased/KDE_cutoff/KDE_egos.txt
+    - increased/KDE_cutoff/KDE_egos.txt
+
+On the module level, for each module, a similar text file is generated, containing only module-specific seeds and the associated nodes.
+
+    - decreased/KDE_cutoff/modules/module_N/module_egos.txt
+    - increased/KDE_cutoff/modules/module_N/module_egos.txt
+
+### 7). Output - network propagation results
+Three files are stored on the top layers of the result folder. These files can be reused by phuEGO to save time, when the user provide the flag **-ru** to CLI.
+
+    - pvalues.txt
+    - rwr_scores.txt
+    - start_seeds.txt
+
+The pvalues.txt file contains the pvalues for each node of the network. It is divided in seven columns, the first column refers to the uniprot ids.
+
 Columns from 2,3,and 4 refers to the pvalues associated with the increased phosphorylation nodes pvalues, of which:
     -second column refers to the pvalues when increased phosphorilated tyrosine are used as seed nodes 
     -third column refers to the pvalues when all the other increased phosphorilated kinases are used as seed nodes, 
     -fourth column refers to the pvalues when the increased phosphorilated substrates are used as seed nodes.
 
 Columns from 5,6 and 7 refers to the pvalues associated with the decreased phosphorylated nodes pvalues, of which:
     -fifth column refers to the pvalues when decreased phosphorilated tyrosine are used as seed nodes 
     -sixt column refers to the pvalues when all the other decreased phosphorilated kinases are used as seed nodes, 
     -seventh column refers to the pvalues when the decreased phosphorilated substrates are used as seed nodes.
 
-A value greater than 950 indicates a pvalues<0.05 as well as a values greater than 990 indicates a pvalues<0.01
-#### rwr_scores.txt
-This file has the same format of pvalues.txt with the difference that values indicates rwr scores 
-
-#### start_seeds.txt 
-First column is uniprot id, second column is phosphorylation LFC (is it exactly the same as the user input?)
+A value greater than 950 indicates a pvalues<0.05 as well as a values greater than 990 indicates a pvalues<0.01. 
 
-#### KDE_egos.txt
-First column is a seed node, the remaining column are the neighbors associated with the seed nodes. 
+The rwr_scores.txt file has the same format of pvalues.txt with the difference that values indicates rwr scores.
 
-#### module_egos.txt
-Has the same format of KDE_egos.txt but refers to the module specific nodes associated to the seed nodes.
+The start_seeds.txt is basically the same as the user input.
 
-#### Fisher test
-Inside the fishers folder 8 files are can be found:
-Pfisher.txt refers to the enriched terms against Gene Ontology biological process
-Ffisher.txt refers to the enriched terms against Gene Ontology functional 
-Cfisher.txt refers to the enriched terms against Gene Ontology cellular component
-Kfisher.txt refers to the enriched terms against KEGG
-Rfisher.txt refers to the enriched terms against Reactome when only the leaves are consider as annotation
-RTfisher.txt refers to the enriched terms against Reactome when all the hierarchy is considered
-Dfisher.txt refers to the enriched terms against DisGenenet
-Bfisher.txt refers to the enriched terms against Bioplanet
+## 5. Development
 
-#### Networks
-The most interesting results that the user should be looking at is: 
+### Future development
 
-### phuego function variables
-#### iteam A
-#### iteam B
+phuEGO can be integrated into any phosphoproteomics analysis pipeline. It will eventually become available through NF-core/Nextflow for easier pipeline integration.
 
-### Additional phuego CLI variables
-#### iteam A
-#### iteam B
+### Changelog
 
-## Development
+For a detailed history of changes, see the [Changelog](https://github.com/haoqichen20/phuego/blob/master/CHANGELOG.md).
 
-phuego can be integrated into any phosphoproteomics analysis pipeline. It will soon become available through NF-core/Nextflow for easier pipeline integration.
+## 6. Citation
 
-## Citation
+Please cite phuEGO if you use it in your analysis.
 
-Please cite phuego if you use it in your analysis.
+> **phuEGO: A network-based method to reconstruct active signalling pathways from phosphoproteomics datasets** <br> _Girolamo Giudice, Haoqi Chen, Evangelia Petsalaki_ <br>
+> bioRxiv, 2023 <br>
+> doi: [10.1101/2023.08.07.552249](https://doi.org/10.1101/2023.08.07.552249) <br>
 
 ```BibTeX
+@article{giudice_phuego_2023,
+	title = {{phuEGO}: {A} network-based method to reconstruct active signalling pathways from phosphoproteomics datasets},
+	url = {https://www.biorxiv.org/content/early/2023/08/07/2023.08.07.552249},
+	doi = {10.1101/2023.08.07.552249},
+	abstract = {Signalling networks are critical for virtually all cell functions. Our current knowledge of cell signalling has been summarised in signalling pathway databases, which, while useful, are highly biassed towards well-studied processes, and don’t capture context specific network wiring or pathway cross-talk. Mass spectrometry-based phosphoproteomics data can provide a more unbiased view of active cell signalling processes in a given context, however, it suffers from low signal-to-noise ratio and poor reproducibility across experiments. Methods to extract active signalling signatures from such data struggle to produce unbiased and interpretable networks that can be used for hypothesis generation and designing downstream experiments. Here we present phuEGO, which combines three-layer network propagation with ego network decomposition to provide small networks comprising active functional signalling modules. PhuEGO boosts the signal-to-noise ratio from global phosphoproteomics datasets, enriches the resulting networks for functional phosphosites and allows the improved comparison and integration across datasets. We applied phuEGO to five phosphoproteomics data sets from cell lines collected upon infection with SARS CoV2. PhuEGO was better able to identify common active functions across datasets and to point to a subnetwork enriched for known COVID-19 targets. Overall, phuEGO provides a tool to the community for the improved functional interpretation of global phosphoproteomics datasets.Competing Interest StatementThe authors have declared no competing interest.},
+	journal = {bioRxiv},
+	author = {Giudice, Girolamo and Chen, Haoqi and Petsalaki, Evangelia},
+	year = {2023},
+	note = {Publisher: Cold Spring Harbor Laboratory
+\_eprint: https://www.biorxiv.org/content/early/2023/08/07/2023.08.07.552249.full.pdf},
+}
 ```
 
-## Contributors
+## 7. Contributors
 
-The algorithm and initial scripts of phuego are developed by Girolamo Giudice ([@girolamogiudice](https://github.com/girolamogiudice)) and Evangelia Petsalaki at [@EMBL-EBI] (https://www.ebi.ac.uk/).
+The algorithm and initial scripts of phuEGO are developed by Girolamo Giudice ([@girolamogiudice](https://github.com/girolamogiudice)) and Evangelia Petsalaki at [EMBL-EBI](https://www.ebi.ac.uk/).
 
-The Python package and CLI application are developed by Haoqi Chen ([@haoqichen20] (https://github.com/haoqichen20) at [@EMBL-EBI] (https://www.ebi.ac.uk/)).
+The Python package and CLI application are developed by Haoqi Chen ([@haoqichen20](https://github.com/haoqichen20)) at [EMBL-EBI](https://www.ebi.ac.uk/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

