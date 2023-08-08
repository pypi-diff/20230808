# Comparing `tmp/sparc_flow-0.1.1.tar.gz` & `tmp/sparc_flow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparc_flow-0.1.1.tar", last modified: Tue Aug  8 01:37:28 2023, max compression
+gzip compressed data, was "sparc_flow-1.0.0.tar", last modified: Tue Aug  8 02:02:30 2023, max compression
```

## Comparing `sparc_flow-0.1.1.tar` & `sparc_flow-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 01:37:28.428125 sparc_flow-0.1.1/
--rw-r--r--   0 clin864  (57669) staff    (20200)    11357 2023-08-07 01:18:18.000000 sparc_flow-0.1.1/LICENSE
--rw-r--r--   0 clin864  (57669) staff    (20200)      326 2023-08-08 01:37:28.428125 sparc_flow-0.1.1/PKG-INFO
--rw-r--r--   0 clin864  (57669) staff    (20200)    19610 2023-08-08 01:06:07.000000 sparc_flow-0.1.1/README.md
--rw-r--r--   0 clin864  (57669) staff    (20200)       38 2023-08-08 01:37:28.432125 sparc_flow-0.1.1/setup.cfg
--rw-r--r--   0 clin864  (57669) staff    (20200)      593 2023-08-08 01:35:08.000000 sparc_flow-0.1.1/setup.py
-drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 01:37:28.428125 sparc_flow-0.1.1/sparc_flow/
--rw-r--r--   0 clin864  (57669) staff    (20200)       64 2023-08-07 07:03:58.000000 sparc_flow-0.1.1/sparc_flow/__init__.py
-drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 01:37:28.428125 sparc_flow-0.1.1/sparc_flow/core/
--rw-r--r--   0 clin864  (57669) staff    (20200)        0 2023-08-07 01:18:18.000000 sparc_flow-0.1.1/sparc_flow/core/__init__.py
--rw-r--r--   0 clin864  (57669) staff    (20200)     6627 2023-08-08 01:20:35.000000 sparc_flow-0.1.1/sparc_flow/core/workflow.py
-drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 01:37:28.428125 sparc_flow-0.1.1/sparc_flow/utils/
--rw-r--r--   0 clin864  (57669) staff    (20200)       51 2023-08-07 01:18:18.000000 sparc_flow-0.1.1/sparc_flow/utils/__init__.py
--rw-r--r--   0 clin864  (57669) staff    (20200)      738 2023-08-07 01:18:18.000000 sparc_flow-0.1.1/sparc_flow/utils/import_code_to_sds.py
-drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 01:37:28.428125 sparc_flow-0.1.1/sparc_flow.egg-info/
--rw-r--r--   0 clin864  (57669) staff    (20200)      326 2023-08-08 01:37:28.000000 sparc_flow-0.1.1/sparc_flow.egg-info/PKG-INFO
--rw-r--r--   0 clin864  (57669) staff    (20200)      342 2023-08-08 01:37:28.000000 sparc_flow-0.1.1/sparc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 clin864  (57669) staff    (20200)        1 2023-08-08 01:37:28.000000 sparc_flow-0.1.1/sparc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 clin864  (57669) staff    (20200)       17 2023-08-08 01:37:28.000000 sparc_flow-0.1.1/sparc_flow.egg-info/requires.txt
--rw-r--r--   0 clin864  (57669) staff    (20200)       11 2023-08-08 01:37:28.000000 sparc_flow-0.1.1/sparc_flow.egg-info/top_level.txt
+drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 02:02:30.149710 sparc_flow-1.0.0/
+-rw-r--r--   0 clin864  (57669) staff    (20200)    11357 2023-08-07 01:18:18.000000 sparc_flow-1.0.0/LICENSE
+-rw-r--r--   0 clin864  (57669) staff    (20200)      326 2023-08-08 02:02:30.149710 sparc_flow-1.0.0/PKG-INFO
+-rw-r--r--   0 clin864  (57669) staff    (20200)    19611 2023-08-08 01:58:44.000000 sparc_flow-1.0.0/README.md
+-rw-r--r--   0 clin864  (57669) staff    (20200)       38 2023-08-08 02:02:30.149710 sparc_flow-1.0.0/setup.cfg
+-rw-r--r--   0 clin864  (57669) staff    (20200)      593 2023-08-08 02:02:25.000000 sparc_flow-1.0.0/setup.py
+drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 02:02:30.145710 sparc_flow-1.0.0/sparc_flow/
+-rw-r--r--   0 clin864  (57669) staff    (20200)       64 2023-08-07 07:03:58.000000 sparc_flow-1.0.0/sparc_flow/__init__.py
+drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 02:02:30.145710 sparc_flow-1.0.0/sparc_flow/core/
+-rw-r--r--   0 clin864  (57669) staff    (20200)        0 2023-08-07 01:18:18.000000 sparc_flow-1.0.0/sparc_flow/core/__init__.py
+-rw-r--r--   0 clin864  (57669) staff    (20200)     9626 2023-08-08 02:01:29.000000 sparc_flow-1.0.0/sparc_flow/core/workflow.py
+drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 02:02:30.149710 sparc_flow-1.0.0/sparc_flow/utils/
+-rw-r--r--   0 clin864  (57669) staff    (20200)       51 2023-08-07 01:18:18.000000 sparc_flow-1.0.0/sparc_flow/utils/__init__.py
+-rw-r--r--   0 clin864  (57669) staff    (20200)      738 2023-08-07 01:18:18.000000 sparc_flow-1.0.0/sparc_flow/utils/import_code_to_sds.py
+drwxr-xr-x   0 clin864  (57669) staff    (20200)        0 2023-08-08 02:02:30.145710 sparc_flow-1.0.0/sparc_flow.egg-info/
+-rw-r--r--   0 clin864  (57669) staff    (20200)      326 2023-08-08 02:02:30.000000 sparc_flow-1.0.0/sparc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 clin864  (57669) staff    (20200)      342 2023-08-08 02:02:30.000000 sparc_flow-1.0.0/sparc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 clin864  (57669) staff    (20200)        1 2023-08-08 02:02:30.000000 sparc_flow-1.0.0/sparc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 clin864  (57669) staff    (20200)       17 2023-08-08 02:02:30.000000 sparc_flow-1.0.0/sparc_flow.egg-info/requires.txt
+-rw-r--r--   0 clin864  (57669) staff    (20200)       11 2023-08-08 02:02:30.000000 sparc_flow-1.0.0/sparc_flow.egg-info/top_level.txt
```

### Comparing `sparc_flow-0.1.1/LICENSE` & `sparc_flow-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparc_flow-0.1.1/README.md` & `sparc_flow-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
   <tr>
     <th> Tutorial</th>
     <th> Description</th>
   </tr>
 </thead>
 <tbody>
   <tr>
-    <td><a href="https://github.com/SPARC-FAIR-Codeathon/sparc-flow/blob/main/tutorials/tutorial_1_download_data_and_postprocess.ipynb">
+    <td><a href="https://github.com/SPARC-FAIR-Codeathon/2023-team-3/blob/main/tutorials/tutorial_1_download_data_and_postprocess.ipynb">
     1
     </a></td>
     <td> Provides a typical data processing example that downloads an existing curated SDS dataset from the SPARC portal (<a href="https://doi.org/10.26275/vm1h-k4kq">Electrode design characterization for electrophysiology from swine peripheral nervous system</a>) using <a href="https://github.com/SPARC-FAIR-Codeathon/sparc-me">sparc-me</a> and perform post-processing to generate a new derived SDS dataset. This example will be used in subsequent tutorials</td>
   </tr>
   <tr>
     <td><a href="https://github.com/SPARC-FAIR-Codeathon/2023-team-3/blob/main/examples/tutorial_2_creating_standarised_workflow_description.ipynb">
     2
```

### Comparing `sparc_flow-0.1.1/setup.py` & `sparc_flow-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name="sparc_flow",
-    version="0.1.1",
+    version="1.0.0",
     description='A Python tool to create tools and workflows for processing SPARC datasets in accordance with FAIR principles.',
     author="Thiranja Prasad Babarenda Gamage, Chinchien Lin, Jiali Xu, Linkun Gao, Matthew French, Michael Hoffman",
     email="psam012@aucklanduni.ac.nz, clin864@aucklanduni.ac.nz",
     license="Apache-2.0",
     packages=find_packages(),
     include_package_data=True,
     package_data={'': ['resources./*']},
```

### Comparing `sparc_flow-0.1.1/sparc_flow/utils/import_code_to_sds.py` & `sparc_flow-1.0.0/sparc_flow/utils/import_code_to_sds.py`

 * *Files identical despite different names*

