# Comparing `tmp/get-reads-taxonomy-0.0.1.tar.gz` & `tmp/get-reads-taxonomy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-reads-taxonomy-0.0.1.tar", last modified: Tue Aug  8 04:33:28 2023, max compression
+gzip compressed data, was "get-reads-taxonomy-0.0.2.tar", last modified: Tue Aug  8 12:55:16 2023, max compression
```

## Comparing `get-reads-taxonomy-0.0.1.tar` & `get-reads-taxonomy-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:33:28.685102 get-reads-taxonomy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 04:33:28.685102 get-reads-taxonomy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:33:28.685102 get-reads-taxonomy-0.0.1/get_reads_taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 04:33:28.685102 get-reads-taxonomy-0.0.1/get_reads_taxonomy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:33:28.685102 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 04:33:28.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 04:33:28.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 04:33:28.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 04:33:28.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 04:33:28.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 04:33:28.000000 get-reads-taxonomy-0.0.1/get_reads_taxonomy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 04:33:28.685102 get-reads-taxonomy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 04:33:24.000000 get-reads-taxonomy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:55:16.781124 get-reads-taxonomy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 12:55:16.781124 get-reads-taxonomy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:55:16.781124 get-reads-taxonomy-0.0.2/get_reads_taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 12:55:16.781124 get-reads-taxonomy-0.0.2/get_reads_taxonomy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:55:16.781124 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 12:55:16.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 12:55:16.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:55:16.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 12:55:16.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:55:16.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 12:55:16.000000 get-reads-taxonomy-0.0.2/get_reads_taxonomy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 12:55:16.781124 get-reads-taxonomy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 12:55:11.000000 get-reads-taxonomy-0.0.2/setup.py
```

### Comparing `get-reads-taxonomy-0.0.1/LICENSE` & `get-reads-taxonomy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `get-reads-taxonomy-0.0.1/README.md` & `get-reads-taxonomy-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 conda activate get-reads-taxonomy
 pip install -e .
 ```
 
 
 # Usage
 
-getRTax will take a TSV file produced from [metaDMG](https://metadmg-dev.github.io/metaDMG-core/) and extract the reads from a BAM file. One can select a list of taxa and ranks to extract the reads from.
+getRTax will take a BAM file and a taxonomy TSV file and extract the reads that map to each of the selected taxa. One can select a list of taxa and ranks to extract the reads from.
 
 For a complete list of options:
 
 ```bash
 $ getRTax --help
 usage: getRTax [-h] -b BAM [-p PREFIX] [--only-read-ids] [--combine] [--unique] -T
                TAXONOMY_FILE -r RANK [-M SORT_MEMORY] [-t THREADS] [--chunk-size CHUNK_SIZE]
```

### Comparing `get-reads-taxonomy-0.0.1/get_reads_taxonomy/__main__.py` & `get-reads-taxonomy-0.0.2/get_reads_taxonomy/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         if not samfile.has_index():
             index_bam_file(
                 bam=bam,
                 suffix="bam",
                 max_chr_length=max_chr_length,
                 threads=args.threads,
             )
+            samfile = pysam.AlignmentFile(bam, "rb", threads=args.threads)
 
     # rnames = defaultdict(int)
     # for aln in samfile.fetch(multiple_iterators=False, until_eof=True):
     #     rnames[aln.qname] += 1
 
     # samfile.close()
     # print(len(rnames))
```

### Comparing `get-reads-taxonomy-0.0.1/get_reads_taxonomy/defaults.py` & `get-reads-taxonomy-0.0.2/get_reads_taxonomy/defaults.py`

 * *Files identical despite different names*

### Comparing `get-reads-taxonomy-0.0.1/get_reads_taxonomy/extract.py` & `get-reads-taxonomy-0.0.2/get_reads_taxonomy/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def index_bam_file(bam, suffix, max_chr_length, threads=1):
     logging.info("Indexing BAM file...")
     samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
     if samfile.has_index():
         sorted_bam_index_bai = bam.replace(suffix, f"{suffix}.bam.bai")
-        sorted_bam_index_csi = bam.replace(suffix, f"{suffix}.bacsi")
+        sorted_bam_index_csi = bam.replace(suffix, f"{suffix}.bam.csi")
         if os.path.exists(sorted_bam_index_bai):
             os.remove(sorted_bam_index_bai)
         elif os.path.exists(sorted_bam_index_csi):
             os.remove(sorted_bam_index_csi)
 
     if max_chr_length > 536870912:
         logging.info("A reference is longer than 2^29, indexing with csi")
```

### Comparing `get-reads-taxonomy-0.0.1/get_reads_taxonomy/lib.py` & `get-reads-taxonomy-0.0.2/get_reads_taxonomy/lib.py`

 * *Files identical despite different names*

### Comparing `get-reads-taxonomy-0.0.1/get_reads_taxonomy/utils.py` & `get-reads-taxonomy-0.0.2/get_reads_taxonomy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from get_reads_taxonomy import __version__
 import time
 import json
 from get_reads_taxonomy.defaults import mdmg_header, valid_ranks, filterBAM_header
 from collections import defaultdict
 import re
 from itertools import chain
+from pathlib import Path
 
 log = logging.getLogger("my_logger")
 log.setLevel(logging.INFO)
 timestr = time.strftime("%Y%m%d-%H%M%S")
 
 
 def is_debug():
@@ -303,39 +304,49 @@
     with open(devnull, "w") as fnull:
         with redirect_stderr(fnull) as err, redirect_stdout(fnull) as out:
             yield (err, out)
 
 
 def create_output_files(prefix, bam, taxon=None, combined=False):
     if prefix is None:
-        prefix = bam.split(".")[0]
+        prefix = Path(bam).with_suffix("").name.split(".")[0]
+        
     # create output files
     out_files = defaultdict(defaultdict)
+    cwd = Path().resolve()
+
     for k, v in taxon.items():
         for i in v:
             r = splitkeep(i, "__")
             i = re.sub("[^0-9a-zA-Z]+", "_", r[1])
-            out_files[f"{k}{i}"]["fname"] = f"{prefix}.{k}{i}.fastq.gz"
+            out_files[f"{k}{i}"]["fname"] = os.path.join(
+                cwd, f"{prefix}.{k}{i}.fastq.gz"
+            )
 
             if os.path.exists(out_files[f"{k}{i}"]["fname"]):
                 out_files[f"{k}{i}"]["exists"] = True
             else:
                 out_files[f"{k}{i}"]["exists"] = False
-            out_files[f"{k}{i}_read_ids"]["fname"] = f"{prefix}.{k}{i}.read_ids.txt.gz"
+            out_files[f"{k}{i}_read_ids"]["fname"] = os.path.join(
+                cwd, f"{prefix}.{k}{i}.read_ids.txt.gz"
+            )
             if os.path.exists(out_files[f"{k}{i}_read_ids"]["fname"]):
                 out_files[f"{k}{i}_read_ids"]["exists"] = True
             else:
                 out_files[f"{k}{i}_read_ids"]["exists"] = False
 
-    out_files["fastq_combined"]["fname"] = f"{prefix}.fastq.gz"
+    out_files["fastq_combined"]["fname"] = os.path.join(cwd, f"{prefix}.fastq.gz")
     if os.path.exists(out_files["fastq_combined"]["fname"]):
         out_files["fastq_combined"]["exists"] = True
     else:
         out_files["fastq_combined"]["exists"] = False
-    out_files["fastq_combined_read_ids"]["fname"] = f"{prefix}.read_ids.txt.gz"
+
+    out_files["fastq_combined_read_ids"]["fname"] = os.path.join(
+        cwd, f"{prefix}.read_ids.txt.gz"
+    )
     if os.path.exists(out_files["fastq_combined_read_ids"]["fname"]):
         out_files["fastq_combined_read_ids"]["exists"] = True
     else:
         out_files["fastq_combined_read_ids"]["exists"] = False
 
     return out_files
```

### Comparing `get-reads-taxonomy-0.0.1/setup.cfg` & `get-reads-taxonomy-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `get-reads-taxonomy-0.0.1/setup.py` & `get-reads-taxonomy-0.0.2/setup.py`

 * *Files identical despite different names*

