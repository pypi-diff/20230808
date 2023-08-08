# Comparing `tmp/kingfisher-0.2.1.tar.gz` & `tmp/kingfisher-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingfisher-0.2.1.tar", last modified: Wed May 24 00:29:42 2023, max compression
+gzip compressed data, was "kingfisher-0.2.2.tar", last modified: Tue Aug  8 02:05:11 2023, max compression
```

## Comparing `kingfisher-0.2.1.tar` & `kingfisher-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:29:42.503583 kingfisher-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-24 00:29:26.000000 kingfisher-0.2.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-24 00:29:42.503583 kingfisher-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 00:29:26.000000 kingfisher-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:29:42.503583 kingfisher-0.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14749 2023-05-24 00:29:26.000000 kingfisher-0.2.1/bin/kingfisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:29:42.503583 kingfisher-0.2.1/kingfisher/
--rw-r--r--   0 runner    (1001) docker     (123)    38156 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:29:42.503583 kingfisher-0.2.1/kingfisher/data/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/data/asperaweb_id_dsa.openssh
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/ena.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/md5sum.py
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/sra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 00:29:26.000000 kingfisher-0.2.1/kingfisher/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:29:42.503583 kingfisher-0.2.1/kingfisher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-24 00:29:42.000000 kingfisher-0.2.1/kingfisher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 00:29:42.000000 kingfisher-0.2.1/kingfisher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:29:42.000000 kingfisher-0.2.1/kingfisher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 00:29:42.000000 kingfisher-0.2.1/kingfisher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 00:29:42.000000 kingfisher-0.2.1/kingfisher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:29:42.503583 kingfisher-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-24 00:29:26.000000 kingfisher-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:29:42.503583 kingfisher-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-24 00:29:26.000000 kingfisher-0.2.1/test/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-24 00:29:26.000000 kingfisher-0.2.1/test/test_ena.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-05-24 00:29:26.000000 kingfisher-0.2.1/test/test_get_sra_and_aws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:05:11.245332 kingfisher-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-08 02:04:49.000000 kingfisher-0.2.2/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 02:05:11.245332 kingfisher-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-08 02:04:49.000000 kingfisher-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:05:11.241332 kingfisher-0.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14845 2023-08-08 02:04:49.000000 kingfisher-0.2.2/bin/kingfisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:05:11.241332 kingfisher-0.2.2/kingfisher/
+-rw-r--r--   0 runner    (1001) docker     (123)    38156 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:05:11.241332 kingfisher-0.2.2/kingfisher/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/data/asperaweb_id_dsa.openssh
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/ena.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/sra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 02:04:49.000000 kingfisher-0.2.2/kingfisher/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:05:11.241332 kingfisher-0.2.2/kingfisher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 02:05:11.000000 kingfisher-0.2.2/kingfisher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 02:05:11.000000 kingfisher-0.2.2/kingfisher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:05:11.000000 kingfisher-0.2.2/kingfisher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 02:05:11.000000 kingfisher-0.2.2/kingfisher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 02:05:11.000000 kingfisher-0.2.2/kingfisher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:05:11.245332 kingfisher-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-08 02:04:49.000000 kingfisher-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:05:11.245332 kingfisher-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-08 02:04:49.000000 kingfisher-0.2.2/test/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-08-08 02:04:49.000000 kingfisher-0.2.2/test/test_ena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-08 02:04:49.000000 kingfisher-0.2.2/test/test_get_sra_and_aws.py
```

### Comparing `kingfisher-0.2.1/LICENCE.txt` & `kingfisher-0.2.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/PKG-INFO` & `kingfisher-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingfisher
-Version: 0.2.1
+Version: 0.2.2
 Summary: Download/extract biological FASTA/Q read data and metadata
 Home-page: https://github.com/wwood/kingfisher-download
 Author: Ben Woodcroft
 Author-email: benjwoodcroft@gmail.com
 License: GPL3+
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `kingfisher-0.2.1/bin/kingfisher` & `kingfisher-0.2.2/bin/kingfisher`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
     annotate_parser.add_argument(
         '-r','--run-identifiers','--run_identifiers',
         help='Run number to download/extract e.g. ERR1739691',
         nargs='+',
     )
     annotate_parser.add_argument(
-        '--run-identifiers-list','--run_identifiers_list',
+        '--run-identifiers-list','--run_identifiers_list','--run-accession-list','--run_accession_list','--run-identifiers-list','--run_identifiers_list',
         help='Text file containing a newline-separated list of run identifiers i.e. a 1 column CSV file.',
     )
     annotate_parser.add_argument(
         '-p','--bioproject',
         help='BioProject IDs number(s) to download/extract from e.g. PRJNA621514 or SRP260223')
     annotate_parser.add_argument(
         '-o','--output-file',
```

### Comparing `kingfisher-0.2.1/kingfisher/__init__.py` & `kingfisher-0.2.2/kingfisher/__init__.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/kingfisher/data/asperaweb_id_dsa.openssh` & `kingfisher-0.2.2/kingfisher/data/asperaweb_id_dsa.openssh`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/kingfisher/ena.py` & `kingfisher-0.2.2/kingfisher/ena.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/kingfisher/location.py` & `kingfisher-0.2.2/kingfisher/location.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/kingfisher/sra_metadata.py` & `kingfisher-0.2.2/kingfisher/sra_metadata.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/kingfisher.egg-info/PKG-INFO` & `kingfisher-0.2.2/kingfisher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingfisher
-Version: 0.2.1
+Version: 0.2.2
 Summary: Download/extract biological FASTA/Q read data and metadata
 Home-page: https://github.com/wwood/kingfisher-download
 Author: Ben Woodcroft
 Author-email: benjwoodcroft@gmail.com
 License: GPL3+
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `kingfisher-0.2.1/setup.py` & `kingfisher-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/test/test_annotate.py` & `kingfisher-0.2.2/test/test_annotate.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,31 +40,31 @@
     'SRR13774710,PRJNA630999,10.342,WGS,RANDOM,Illumina NovaSeq 6000,SCB2WXA,human gut metagenome'))
 
 class Tests(unittest.TestCase):
     maxDiff = None
     
     def test_one_sample_annotate(self):
         self.assertEqual(
-            'run        | study_accession | Gbp   | library_strategy | library_selection | model               | sample_name | taxon_name\n' \
-            '---------- | --------------- | ----- | ---------------- | ----------------- | ------------------- | ----------- | ----------\n' \
-            'ERR1739691 | ERP017539       | 2.382 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_1       | metagenome\n',
+            'run        | bioproject | Gbp   | library_strategy | library_selection | model               | sample_name | taxon_name\n' \
+            '---------- | ---------- | ----- | ---------------- | ----------------- | ------------------- | ----------- | ----------\n' \
+            'ERR1739691 | PRJEB15706 | 2.382 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_1       | metagenome\n',
             extern.run('{} annotate -r ERR1739691 --debug'.format(kingfisher)))
 
     def test_one_project_annotate(self):
-        self.assertEqual('run        | study_accession | Gbp   | library_strategy | library_selection | model               | sample_name | taxon_name\n' \
-        '---------- | --------------- | ----- | ---------------- | ----------------- | ------------------- | ----------- | ----------\n' \
-        'ERR1739691 | ERP017539       | 2.382 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_1       | metagenome\n' \
-        'ERR1739692 | ERP017539       | 2.382 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_2       | metagenome\n' \
-        'ERR1739693 | ERP017539       | 2.364 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_3       | metagenome\n' \
-        'ERR1739694 | ERP017539       | 2.501 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_4       | metagenome\n' \
-        'ERR1739695 | ERP017539       | 2.379 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_5       | metagenome\n' \
-        'ERR1739696 | ERP017539       | 2.351 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_6       | metagenome\n' \
-        'ERR1739697 | ERP017539       | 2.524 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_7       | metagenome\n' \
-        'ERR1739698 | ERP017539       | 2.358 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_8       | metagenome\n' \
-        'ERR1739699 | ERP017539       | 2.465 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_9       | metagenome\n',
+        self.assertEqual('run        | bioproject | Gbp   | library_strategy | library_selection | model               | sample_name | taxon_name\n' \
+        '---------- | ---------- | ----- | ---------------- | ----------------- | ------------------- | ----------- | ----------\n' \
+        'ERR1739691 | PRJEB15706 | 2.382 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_1       | metagenome\n' \
+        'ERR1739692 | PRJEB15706 | 2.382 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_2       | metagenome\n' \
+        'ERR1739693 | PRJEB15706 | 2.364 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_3       | metagenome\n' \
+        'ERR1739694 | PRJEB15706 | 2.501 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_4       | metagenome\n' \
+        'ERR1739695 | PRJEB15706 | 2.379 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_5       | metagenome\n' \
+        'ERR1739696 | PRJEB15706 | 2.351 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_6       | metagenome\n' \
+        'ERR1739697 | PRJEB15706 | 2.524 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_7       | metagenome\n' \
+        'ERR1739698 | PRJEB15706 | 2.358 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_8       | metagenome\n' \
+        'ERR1739699 | PRJEB15706 | 2.465 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_9       | metagenome\n',
             extern.run('{} annotate -p PRJEB15706 --debug'.format(kingfisher)))
 
     def test_one_sample_annotate_csv(self):
         self.assertEqual('run,bioproject,Gbp,library_strategy,library_selection,model,sample_name,taxon_name,experiment_accession,experiment_title,library_name,library_source,submitter,study_accession,study_alias,study_centre_project_name,organisation,organisation_department,organisation_institution,organisation_street,organisation_city,organisation_country,organisation_contact_name,organisation_contact_email,sample_description,sample_alias,sample_accession,ENA first public,ENA last update,External Id,INSDC center alias,INSDC center name,INSDC first public,INSDC last update,INSDC status,Submitter Id,collection date,depth,environment (biome),environment (feature),environment (material),geographic location (country and/or sea),geographic location (depth),geographic location (elevation),geographic location (latitude),geographic location (longitude),investigation type,microbial mat/biofilm environmental package,project name,sample name,sample storage duration,sample storage temperature,sequencing method,study_title,design_description,study_abstract,study_links,number_of_runs_for_sample,spots,bases,run_size,published,read1_length_average,read1_length_stdev,read2_length_average,read2_length_stdev\n' \
             'ERR1739691,PRJEB15706,2.382,WGS,RANDOM,Illumina HiSeq 2500,MM1_1,metagenome,ERX1809317,Illumina HiSeq 2500 paired end sequencing,unspecified,METAGENOMIC,European Nucleotide Archive,ERP017539,ena-STUDY-NIOZ-10-10-2016-11:18:17:022-1157,Minimal Mat 1,Royal Netherlands Institute for Sea Research,,,,,, ,,"artificial minimal coastal microbial mats at dilution 0, replicate 1",SAMEA4497179,ERS1396358,2017-06-08,2016-11-23,SAMEA4497179,NIOZ,Royal Netherlands Institute for Sea Research,2017-06-08T17:01:18Z,2016-11-23T11:15:32Z,public,MM1_1,2015-11,0.01,Microbial Mat Material,Beach,soil,Netherlands,0,0,53.489606,6.139913,metagenome,microbial mat/biofilm,Minimal Mat,MM1_1,10,20,illumina PE100,construction of minimal coastal microbial mats,,"Minimal coastal microbial mats were created with diluted coastal mat samples obtained from the Dutch barrier island of Schiermonnikoog. The MM\'s were inoculated in fresh sterilized sand in glass containers contained in a MicroBox. The MicroBox has a transparent lid (allowing photosynthetic growth) and a gas exchange filter. The MM\'s are propagated under laboratory conditions at a 16h light / 8h dark regime and at a constant 23 C. Serial dilutions used for this data-set are 0, 3 and 5-fold.",[],1,7938968,2381690400,936643449,2017-06-13 08:05:22,150,0,150,0\n',
             extern.run('{} annotate -r ERR1739691 -f csv --all-columns'.format(kingfisher)))
```

### Comparing `kingfisher-0.2.1/test/test_ena.py` & `kingfisher-0.2.2/test/test_ena.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.2.1/test/test_get_sra_and_aws.py` & `kingfisher-0.2.2/test/test_get_sra_and_aws.py`

 * *Files identical despite different names*

