# Comparing `tmp/python3_utils_tdinoto-1.0.4.tar.gz` & `tmp/python3_utils_tdinoto-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_utils_tdinoto-1.0.4.tar", last modified: Fri Apr 28 15:45:42 2023, max compression
+gzip compressed data, was "python3_utils_tdinoto-1.0.5.tar", last modified: Tue Aug  8 09:58:24 2023, max compression
```

## Comparing `python3_utils_tdinoto-1.0.4.tar` & `python3_utils_tdinoto-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.115136 python3_utils_tdinoto-1.0.4/
--rw-rw-rw-   0        0        0     1087 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2600 2023-04-28 15:45:42.114181 python3_utils_tdinoto-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/README.md
--rw-rw-rw-   0        0        0      779 2023-04-28 15:28:37.000000 python3_utils_tdinoto-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 15:45:42.115136 python3_utils_tdinoto-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.022699 python3_utils_tdinoto-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.053829 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/
--rw-rw-rw-   0        0        0     2600 2023-04-28 15:45:41.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.113124 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/numeric.py
--rw-rw-rw-   0        0        0     8736 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_bids_dcm_dataset.py
--rw-rw-rw-   0        0        0     1641 2023-04-12 13:20:11.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_dict.py
--rw-rw-rw-   0        0        0      337 2023-04-03 13:25:55.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_io.py
--rw-rw-rw-   0        0        0    11797 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_lists.py
--rw-rw-rw-   0        0        0    13801 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_nifti_dicom.py
--rw-rw-rw-   0        0        0     5255 2023-04-14 07:30:39.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_numpy.py
--rw-rw-rw-   0        0        0     3045 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_strings.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:58:24.175671 python3_utils_tdinoto-1.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2600 2023-08-08 09:58:24.173671 python3_utils_tdinoto-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.5/README.md
+-rw-rw-rw-   0        0        0      779 2023-08-08 09:56:48.000000 python3_utils_tdinoto-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 09:58:24.175671 python3_utils_tdinoto-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 09:58:24.078187 python3_utils_tdinoto-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:58:24.090466 python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/
+-rw-rw-rw-   0        0        0     2600 2023-08-08 09:58:24.000000 python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-08-08 09:58:24.000000 python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:58:24.000000 python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-08-08 09:58:24.000000 python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-08 09:58:24.000000 python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 09:58:24.171670 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/numeric.py
+-rw-rw-rw-   0        0        0     9774 2023-08-08 09:50:22.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_bids_dcm_dataset.py
+-rw-rw-rw-   0        0        0     1641 2023-04-12 13:20:11.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_dict.py
+-rw-rw-rw-   0        0        0      337 2023-04-03 13:25:55.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_io.py
+-rw-rw-rw-   0        0        0    11797 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_lists.py
+-rw-rw-rw-   0        0        0    15167 2023-05-04 09:10:52.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_nifti_dicom.py
+-rw-rw-rw-   0        0        0     5876 2023-07-27 08:58:15.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_numpy.py
+-rw-rw-rw-   0        0        0     4646 2023-07-14 09:35:06.000000 python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_strings.py
```

### Comparing `python3_utils_tdinoto-1.0.4/LICENSE` & `python3_utils_tdinoto-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_utils_tdinoto-1.0.4/PKG-INFO` & `python3_utils_tdinoto-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3_utils_tdinoto
-Version: 1.0.4
+Version: 1.0.5
 Summary: Useful wrapper functions for the most common python data types, and for nifti/dicom arrays.
 Author-email: Tommaso Di Noto <tommydino@hotmail.it>
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `python3_utils_tdinoto-1.0.4/README.md` & `python3_utils_tdinoto-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python3_utils_tdinoto-1.0.4/pyproject.toml` & `python3_utils_tdinoto-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python3_utils_tdinoto"
-version = "1.0.4"
+version = "1.0.5"
 description = "Useful wrapper functions for the most common python data types, and for nifti/dicom arrays."
 readme = "README.md"
 authors = [{ name = "Tommaso Di Noto", email = "tommydino@hotmail.it" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/PKG-INFO` & `python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-utils-tdinoto
-Version: 1.0.4
+Version: 1.0.5
 Summary: Useful wrapper functions for the most common python data types, and for nifti/dicom arrays.
 Author-email: Tommaso Di Noto <tommydino@hotmail.it>
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/SOURCES.txt` & `python3_utils_tdinoto-1.0.5/src/python3_utils_tdinoto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/numeric.py` & `python3_utils_tdinoto-1.0.5/src/utils_tdinoto/numeric.py`

 * *Files identical despite different names*

### Comparing `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_bids_dcm_dataset.py` & `python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_bids_dcm_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 import pydicom
 from collections import Counter
 import numpy as np
 from utils_tdinoto.utils_strings import keep_only_digits
 import SimpleITK as sitk
 import pandas as pd
+from tqdm import tqdm
 from utils_tdinoto.numeric import round_half_up
+from utils_tdinoto.utils_lists import extract_unique_elements
 
 
-def print_patient_sex_and_age(bids_dir: str, bids_dcm_dir: str) -> None:
+def print_patient_sex_and_age(bids_dir: str,
+                              bids_dcm_dir: str) -> None:
     """This function loops over a pseudo-BIDS dataset dir and prints the patient sex
     Args:
         bids_dir: directory containing the BIDS dataset
         bids_dcm_dir: directory containing the dcm series of the dataset. A pseudo-BIDS organization is expected. Specifically:
             sub-000
                 |__ses-yyyymm01
                       |__dcm_series_1
@@ -43,25 +46,27 @@
     occurrence_count_sex = Counter(all_sex)
     print(f"\nSex: {occurrence_count_sex}")
     all_ages_only_numbers = [int(keep_only_digits(x)) for x in all_ages]
     mean_age, std_age = np.mean(all_ages_only_numbers), np.std(all_ages_only_numbers)
     print(f"\nAge: mean={mean_age}, std={std_age}")
 
 
-def print_median_values(df, scanner_name):
+def print_median_values(df: pd.DataFrame,
+                        scanner_name: str) -> None:
     median_tr = df['TR'].median()
     median_te = df['TE'].median()
     median_spacing_x = df['spacing_x'].median()
     median_spacing_y = df['spacing_y'].median()
     median_spacing_z = df['spacing_z'].median()
 
     print(f"\nmedian values {scanner_name}: TR = {round_half_up(median_tr)}, TE = {round_half_up(median_te)}, spacing = {median_spacing_x} x {median_spacing_y} x {median_spacing_z}")
 
 
-def find_mr_acquisition_params(bids_ds, dcm_dir):
+def find_mr_acquisition_params(bids_ds: str,
+                               dcm_dir: str) -> None:
     cnt_subs = 0
     vendor_scanner_field_strength = []
     for sub in sorted(os.listdir(bids_ds)):
         if "sub" in sub and os.path.isdir(os.path.join(bids_ds, sub)):
             sub_dir_dmc_dir = os.path.join(dcm_dir, sub)
             if os.path.isdir(sub_dir_dmc_dir):
                 cnt_subs += 1
@@ -134,17 +139,37 @@
         print_median_values(df_verio, scanner_name="Verio")
     if not df_aera.empty:
         print_median_values(df_aera, scanner_name="Aera")
     if not df_prisma.empty:
         print_median_values(df_prisma, scanner_name="Prisma")
 
 
+def print_distribution_sessions_bids_dataset(path_bids_ds: str) -> None:
+    all_sub_ses = []
+    for sub in tqdm(sorted(os.listdir(path_bids_ds))):
+        if "sub" in sub and os.path.isdir(os.path.join(path_bids_ds, sub)):
+            cnt_ses = 0
+            for ses in sorted(os.listdir(os.path.join(path_bids_ds, sub))):
+                if "ses" in ses and os.path.isdir(os.path.join(path_bids_ds, sub, ses)):
+                    cnt_ses += 1
+            all_sub_ses.append([sub, cnt_ses])
+
+    df_all_sub_ses = pd.DataFrame(all_sub_ses, columns=['sub', 'ses'])
+
+    # extract the different counts for the number of sessions
+    ses_counts = df_all_sub_ses['ses'].value_counts()
+
+    # print the distribution
+    print()
+    for nb_ses, count in ses_counts.items():
+        print(f"Subjects with {nb_ses} ses: {count}")
+
+
 def main():
     # input args
     path_bids_ds = "/path/to/BIDS_Dataset/"
-    all_dicoms = "/path/to/dir/ALL_DICOMS/"
-    print_patient_sex_and_age(path_bids_ds, all_dicoms)
-    find_mr_acquisition_params(path_bids_ds, all_dicoms)
+    # path_bids_ds = r"Z:\Database\ADNI_Controls_FDA_AI_Letter_BIDS"
+    # print_distribution_sessions_bids_dataset(path_bids_ds)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_dict.py` & `python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_dict.py`

 * *Files identical despite different names*

### Comparing `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_lists.py` & `python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_lists.py`

 * *Files identical despite different names*

### Comparing `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_nifti_dicom.py` & `python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_nifti_dicom.py`

 * *Files 8% similar despite different names*

```diff
@@ -290,7 +290,33 @@
     # 19) Series Number (0020, 0011) was already modified in MeVisLab
 
     # 20) Image Comments (0020, 4000) was already modified in MeVisLab
 
     # 21) Pixel Data (7FE0, 0010) was already modified in MeVisLab
 
     return ds
+
+
+def dcm2nii_sitk(in_dcm_dir: str,
+                 out_nii_dir: str,
+                 out_name: str) -> None:
+    """This function converts a DICOM sequence to a NIfTI file using SimpleITK.
+    Args:
+        in_dcm_dir: input directory containing the DICOM sequence
+        out_nii_dir: output directory where the NIfTI file will be saved
+        out_name: name of the NIfTI file
+    """
+    # Load DICOM sequence
+    reader = sitk.ImageSeriesReader()  # type: sitk.ImageSeriesReader # create reader
+    dicom_names = reader.GetGDCMSeriesFileNames(in_dcm_dir)  # type: list # get dicom names
+    reader.SetFileNames(dicom_names)  # set dicom names to reader
+    image = reader.Execute()  # type: sitk.Image # execute reader to get sitk image
+
+    # Convert to NIfTI format
+    img_array = sitk.GetArrayFromImage(image)  # type: np.ndarray  # convert to numpy array
+    image_nifti = sitk.GetImageFromArray(img_array)  # type: sitk.Image  # convert to sitk image
+    image_nifti.SetSpacing(image.GetSpacing())  # set spacing as in original dicom
+    image_nifti.SetDirection(image.GetDirection())  # set direction as in original dicom
+    image_nifti.SetOrigin(image.GetOrigin())  # set origin as in original dicom
+
+    # Save NIfTI file
+    sitk.WriteImage(image_nifti, os.path.join(out_nii_dir, f"{out_name}.nii.gz"))  # save nifti file
```

### Comparing `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_numpy.py` & `python3_utils_tdinoto-1.0.5/src/utils_tdinoto/utils_numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     padded_img = np.pad(input_img, pad_width=((a, aa), (b, bb)), mode='constant', constant_values=0)
 
     return padded_img
 
 
 def generate_binary_array_with_exact_proportion(array_len: int,
                                                 nb_zeros: int,
-                                                shuffle: bool = True):
+                                                shuffle: bool = True) -> np.ndarray:
     """This function creates a 1D binary array with an exact proportion of 0s and 1s.
     The array will contain exactly nb_zeros 0s, and (array_len - nb_zeros) 1s. By
     default, the generated array is shuffled.
     Args:
         array_len: length of generated array
         nb_zeros: number of 0s in the generated array (the rest will be 1s)
         shuffle: whether to shuffle the generated array
@@ -138,7 +138,22 @@
         input_array: input array that we want to inspect
     Returns:
         array_is_empty: True if input_array is empty; False otherwise
     """
     array_is_empty = input_array.size == 0
 
     return array_is_empty
+
+
+def binarize_array(input_array: np.ndarray,
+                   threshold: float = 0.5) -> np.ndarray:
+    """This function binarizes the input array by converting values to either 0 or 1 based on the threshold.
+    Args:
+        input_array (numpy.ndarray or list): The input array to be binarized.
+        threshold: The threshold value to use for binarization. Default is 0.5.
+    Returns:
+        binarized_array: The binarized array.
+    """
+    # Apply binarization using element-wise comparison
+    binarized_array = (input_array >= threshold).astype(int)
+
+    return binarized_array
```

