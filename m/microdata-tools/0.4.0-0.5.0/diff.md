# Comparing `tmp/microdata_tools-0.4.0.tar.gz` & `tmp/microdata_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_tools-0.4.0.tar", max compression
+gzip compressed data, was "microdata_tools-0.5.0.tar", max compression
```

## Comparing `microdata_tools-0.4.0.tar` & `microdata_tools-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1074 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     2238 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/README.md
--rw-r--r--   0        0        0      384 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/__init__.py
--rw-r--r--   0        0        0     4372 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/__init__.py
--rw-r--r--   0        0        0     6072 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/_decrypt.py
--rw-r--r--   0        0        0     4950 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/_encrypt.py
--rw-r--r--   0        0        0     1188 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/_utils.py
--rw-r--r--   0        0        0      238 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/exceptions/__init__.py
--rw-r--r--   0        0        0     5345 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/__init__.py
--rw-r--r--   0        0        0     2557 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/adapter/local_storage.py
--rw-r--r--   0        0        0     5776 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/temporal_attributes.py
--rw-r--r--   0        0        0      757 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_id_types.py
--rw-r--r--   0        0        0     1609 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
--rw-r--r--   0        0        0     2091 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json
--rw-r--r--   0        0        0     1525 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json
--rw-r--r--   0        0        0     2124 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json
--rw-r--r--   0        0        0     1429 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/JOBB.json
--rw-r--r--   0        0        0     1378 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json
--rw-r--r--   0        0        0   232471 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json
--rw-r--r--   0        0        0     1242 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KURS.json
--rw-r--r--   0        0        0     1202 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/PERSON.json
--rw-r--r--   0        0        0     1535 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json
--rw-r--r--   0        0        0     1181 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/__init__.py
--rw-r--r--   0        0        0      502 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/exceptions/__init__.py
--rw-r--r--   0        0        0      915 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/model/__init__.py
--rw-r--r--   0        0        0     5733 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/model/metadata.py
--rw-r--r--   0        0        0     5278 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/steps/data_reader.py
--rw-r--r--   0        0        0    12162 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/steps/dataset_validator.py
--rw-r--r--   0        0        0     1652 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/steps/metadata_reader.py
--rw-r--r--   0        0        0      603 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 microdata_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     2238 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/README.md
+-rw-r--r--   0        0        0      384 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/__init__.py
+-rw-r--r--   0        0        0     4372 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/packaging/__init__.py
+-rw-r--r--   0        0        0     6072 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/packaging/_decrypt.py
+-rw-r--r--   0        0        0     4950 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/packaging/_encrypt.py
+-rw-r--r--   0        0        0     1188 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/packaging/_utils.py
+-rw-r--r--   0        0        0      238 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/packaging/exceptions/__init__.py
+-rw-r--r--   0        0        0     5385 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/__init__.py
+-rw-r--r--   0        0        0     2557 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/adapter/local_storage.py
+-rw-r--r--   0        0        0     5776 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/temporal_attributes.py
+-rw-r--r--   0        0        0      757 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_id_types.py
+-rw-r--r--   0        0        0     1609 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
+-rw-r--r--   0        0        0     2091 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1525 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     2124 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1429 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1378 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232471 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1242 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1202 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1535 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1181 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0      490 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/exceptions/__init__.py
+-rw-r--r--   0        0        0      907 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/model/__init__.py
+-rw-r--r--   0        0        0     5733 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/model/metadata.py
+-rw-r--r--   0        0        0     4369 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/steps/data_reader.py
+-rw-r--r--   0        0        0    11701 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/steps/dataset_validator.py
+-rw-r--r--   0        0        0      680 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/steps/metadata_enricher.py
+-rw-r--r--   0        0        0     1501 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/microdata_tools/validation/steps/metadata_reader.py
+-rw-r--r--   0        0        0      603 2023-08-08 09:56:07.087554 microdata_tools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 microdata_tools-0.5.0/PKG-INFO
```

### Comparing `microdata_tools-0.4.0/LICENSE.md` & `microdata_tools-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/README.md` & `microdata_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/packaging/__init__.py` & `microdata_tools-0.5.0/microdata_tools/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/packaging/_decrypt.py` & `microdata_tools-0.5.0/microdata_tools/packaging/_decrypt.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/packaging/_encrypt.py` & `microdata_tools-0.5.0/microdata_tools/packaging/_encrypt.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/packaging/_utils.py` & `microdata_tools-0.5.0/microdata_tools/packaging/_utils.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/__init__.py` & `microdata_tools-0.5.0/microdata_tools/validation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from pathlib import Path
 import string
-from pyarrow import parquet
+from pyarrow import parquet, dataset
 from typing import List, Union
 from microdata_tools.validation.components import unit_id_types
 from microdata_tools.validation.exceptions import ValidationError
 from microdata_tools.validation.adapter import local_storage
 from microdata_tools.validation.steps import (
     metadata_reader,
     dataset_validator,
     data_reader,
+    metadata_enricher,
 )
 
 
 def _validate_dataset_name(dataset_name: str) -> None:
     """
     Validates that the name of the dataset only contains valid
     characters (uppercase A-Z, numbers 0-9 and _)
@@ -46,62 +47,57 @@
     input_directory: str = "",
     keep_temporary_files: bool = False,
 ) -> List[str]:
     """
     Validate a dataset and return a list of errors.
     If the dataset is valid, the list will be empty.
     """
+    data_errors = []
     try:
         _validate_dataset_name(dataset_name)
-
-        input_directory_path = Path(input_directory)
-        metadata_file_path = (
-            input_directory_path / dataset_name / f"{dataset_name}.json"
-        )
         (
             working_directory_path,
             working_directory_was_generated,
         ) = local_storage.resolve_working_directory(working_directory)
-
-        data_errors = []
+        input_dataset_directory = Path(input_directory) / dataset_name
+        input_metadata_path = input_dataset_directory / f"{dataset_name}.json"
+        input_data_path = input_dataset_directory / f"{dataset_name}.csv"
 
         # Read and validate metadata
         metadata_dict = metadata_reader.run_reader(
-            dataset_name, metadata_file_path
+            dataset_name, input_metadata_path
         )
         measure_data_type = metadata_dict["measureVariables"][0]["dataType"]
         temporality_type = metadata_dict["temporalityType"]
         code_list = metadata_dict["measureVariables"][0]["valueDomain"].get(
             "codeList"
         )
         sentinel_list = metadata_dict["measureVariables"][0][
             "valueDomain"
         ].get("sentinelAndMissingValues")
 
         # Read data
-        table = data_reader.run_reader(
-            dataset_name, input_directory_path, measure_data_type
-        )
+        table = data_reader.run_reader(input_data_path, measure_data_type)
 
         # Enrich metadata with temporal data
         temporal_data = data_reader.get_temporal_data(table, temporality_type)
-        data_reader.metadata_update_temporal_coverage(
+        metadata_enricher.enrich_with_temporal_coverage(
             metadata_dict, temporal_data
         )
 
         # Write files to working directory
         parquet_path = working_directory_path / f"{dataset_name}.parquet"
         parquet.write_table(table, parquet_path)
         local_storage.write_json(
             working_directory_path / f"{dataset_name}.json", metadata_dict
         )
 
         # Validate data
         dataset_validator.validate_dataset(
-            parquet_path,
+            dataset.dataset(parquet_path),
             measure_data_type,
             code_list,
             sentinel_list,
             temporality_type,
         )
     except ValidationError as e:
         data_errors = e.errors
@@ -125,30 +121,26 @@
     working_directory: str = "",
     keep_temporary_files: bool = False,
 ) -> List[dict]:
     """
     Validate metadata and return a list of errors.
     If the metadata is valid, the list will be empty.
     """
+    data_errors = []
     try:
-        data_errors = []
-
         _validate_dataset_name(dataset_name)
-
-        input_directory_path = Path(input_directory)
         (
             working_directory_path,
             working_directory_was_generated,
         ) = local_storage.resolve_working_directory(working_directory)
+        input_dataset_directory = Path(input_directory) / dataset_name
+        input_metadata_path = input_dataset_directory / f"{dataset_name}.json"
 
-        metadata_file_path = (
-            input_directory_path / dataset_name / f"{dataset_name}.json"
-        )
         metadata_dict = metadata_reader.run_reader(
-            dataset_name, metadata_file_path
+            dataset_name, input_metadata_path
         )
         local_storage.write_json(
             working_directory_path / f"{dataset_name}.json", metadata_dict
         )
     except ValidationError as e:
         data_errors = e.errors
     except Exception as e:
```

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/adapter/local_storage.py` & `microdata_tools-0.5.0/microdata_tools/validation/adapter/local_storage.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/temporal_attributes.py` & `microdata_tools-0.5.0/microdata_tools/validation/components/temporal_attributes.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_id_types.py` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_id_types.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/JOBB.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/JOBB.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KURS.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/KURS.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/PERSON.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/PERSON.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/__init__.py` & `microdata_tools-0.5.0/microdata_tools/validation/components/unit_type_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/model/__init__.py` & `microdata_tools-0.5.0/microdata_tools/validation/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     try:
         return Metadata(**metadata_json)
     except pydantic.ValidationError as e:
         logger.exception(e)
         error_messages = [
             _format_pydantic_error(error) for error in e.errors()
         ]
-        raise ValidationError("Invalid metadata file", errors=error_messages)
+        raise ValidationError("metadata file", errors=error_messages)
     except Exception as e:
         logger.exception(e)
         raise e
```

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/model/metadata.py` & `microdata_tools-0.5.0/microdata_tools/validation/model/metadata.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/steps/data_reader.py` & `microdata_tools-0.5.0/microdata_tools/validation/steps/data_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -133,34 +133,10 @@
             "start_year",
             "start_epoch_days",
             "stop_epoch_days",
         ],
     )
 
 
-def metadata_update_temporal_coverage(
-    metadata: dict, temporal_data: dict
-) -> None:
-    logger.debug(
-        "Append temporal coverage (start, stop, status dates) to metadata"
-    )
-    data_revision = metadata["dataRevision"]
-    temporality_type = metadata["temporalityType"]
-    data_revision["temporalCoverageStart"] = temporal_data["start"]
-    data_revision["temporalCoverageLatest"] = temporal_data["latest"]
-    if temporality_type == "STATUS":
-        temporal_status_dates_list = temporal_data["statusDates"]
-        temporal_status_dates_list.sort()
-        data_revision["temporalStatusDates"] = temporal_status_dates_list
-
-
-def run_reader(
-    dataset_name: str, input_directory: Path, measure_data_type: str
-) -> pyarrow.Table:
-    input_dataset_dir = input_directory / dataset_name
-    input_data_path = input_dataset_dir / f"{dataset_name}.csv"
-
-    logger.debug(f'Start reading dataset "{dataset_name}"')
+def run_reader(input_data_path: Path, measure_data_type: str) -> pyarrow.Table:
     table = _sanitize_data(input_data_path, measure_data_type)
-
-    logger.debug(f'OK - reading dataset "{dataset_name}"')
     return table
```

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/steps/dataset_validator.py` & `microdata_tools-0.5.0/microdata_tools/validation/steps/dataset_validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Union
 from pyarrow import dataset, compute, Table
+from pyarrow.dataset import FileSystemDataset
 
 from microdata_tools.validation.exceptions import ValidationError
 
 
 def _get_error_list(invalid_rows: Table, message: str):
     invalid_identifiers = (
         invalid_rows.column("unit_id").slice(0, 5).to_pylist()
@@ -11,15 +12,15 @@
     return [
         f"{message} for row with identifier: {identifier}"
         for identifier in invalid_identifiers
     ]
 
 
 def _valid_value_column_check(
-    parquet_path: str,
+    data: FileSystemDataset,
     data_type: str,
     code_list: Union[list, None],
     sentinel_list: Union[List, None],
 ):
     """
     Any given cell in the value column is valid only if:
     * The cell contains a a valid non-null value
@@ -29,20 +30,20 @@
     is_null_filter = dataset.field("value").is_null()
     is_empty_string_filter = dataset.field("value") == ""
     invalid_rows_filter = (
         (is_null_filter | is_empty_string_filter)
         if data_type == "STRING"
         else is_null_filter
     )
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=invalid_rows_filter, columns=["unit_id"]
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "Invalid value in #2 column",
+        raise ValidationError(
+            "#2 column",
             errors=_get_error_list(invalid_rows, "Invalid value in #2 column"),
         )
 
     if code_list:
         unique_codes = list(
             set(code_list_item["code"] for code_list_item in code_list)
         )
@@ -50,162 +51,161 @@
             unique_codes += list(
                 set(
                     sentinel_list_item["code"]
                     for sentinel_list_item in sentinel_list
                 )
             )
         invalid_code_filter = ~dataset.field("value").isin(unique_codes)
-        invalid_rows = dataset.dataset(parquet_path).to_table(
+        invalid_rows = data.to_table(
             filter=invalid_code_filter, columns=["value"]
         )
         if len(invalid_rows) > 0:
-            raise ValueError(
-                "Value in #2 column not in code list",
-                errors=_get_error_list(
-                    invalid_rows, "Value in #2 column not in code list"
-                ),
+            invalid_codes = (
+                invalid_rows.column("value").slice(0, 5).to_pylist()
+            )
+            raise ValidationError(
+                "#2 column",
+                errors=[f"{code} not in code list" for code in invalid_codes],
             )
 
 
-def _valid_unit_id_check(parquet_path: str):
+def _valid_unit_id_check(data: FileSystemDataset):
     """
     Any given cell in the unit_id column is valid only if:
     * The cell contains a a valid non-null value
     * The cell does not contain an empty string
     """
     is_null_filter = dataset.field("unit_id").is_null()
     is_empty_string_filter = dataset.field("unit_id") == ""
     invalid_rows_filter = is_null_filter | is_empty_string_filter
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=invalid_rows_filter, columns=["unit_id"]
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "Invalid identifier in #1 column",
+        raise ValidationError(
+            "#1 column",
             errors=_get_error_list(
                 invalid_rows, "Invalid identifier in #1 column"
             ),
         )
 
 
-def _fixed_temporal_variables_check(parquet_path: str):
+def _fixed_temporal_variables_check(data: FileSystemDataset):
     """
     Any given row in a table with temporalityType=FIXED is valid only if:
     * The start_epoch_days column contains null (empty)
     * The stop_epoch_days column contains a non-null value (int32)
     """
     start_is_valid_filter = dataset.field("start_epoch_days").is_valid()
     stop_is_null_filter = dataset.field("stop_epoch_days").is_null()
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=start_is_valid_filter | stop_is_null_filter,
         columns=["unit_id"],
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "Invalid #3 and/or #4 columns",
+        raise ValidationError(
+            "#3 and #4 columns",
             errors=_get_error_list(
                 invalid_rows, "Invalid #3 and/or #4 columns"
             ),
         )
 
 
-def _status_temporal_variables_check(parquet_path: str):
+def _status_temporal_variables_check(data: FileSystemDataset):
     """
     Any given row in a table with temporalityType=STATUS is valid only if:
     * The start_epoch_days column contains a non-null value (int32)
     * The stop_epoch_days column contains a non-null value (int32)
     * The start_epoch_days and stop_epoch_days columns contain the same value
       for any given row
     """
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=(
             dataset.field("stop_epoch_days").is_null()
             | dataset.field("start_epoch_days").is_null()
         ),
         columns=["unit_id"],
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "Invalid #3 and/or #4 columns",
+        raise ValidationError(
+            "#3 and #4 columns",
             errors=_get_error_list(
                 invalid_rows, "Invalid #3 and/or #4 columns"
             ),
         )
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=dataset.field("start_epoch_days")
         != dataset.field("stop_epoch_days"),
         columns=["unit_id"],
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "#3 column not equal to #4 column",
+        raise ValidationError(
+            "#3 and #4 columns",
             errors=_get_error_list(
                 invalid_rows, "#3 column not equal to #4 column"
             ),
         )
 
 
-def _event_temporal_variables_check(parquet_path: str):
+def _event_temporal_variables_check(data: FileSystemDataset):
     """
     Any given row in a table with temporalityType=EVENT is valid only if:
     * The start_epoch_days column contains a non-null value (int32)
     * The stop_epoch_days is either a non-null value bigger than
       start_epoch_days (int32), or null (empty)
     """
     start_is_null_filter = dataset.field("start_epoch_days").is_null()
     start_be_stop_filter = dataset.field("start_epoch_days") >= dataset.field(
         "stop_epoch_days"
     )  # If stop_epoch_days is null this test will be ignored by pyarrow
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=(start_is_null_filter | start_be_stop_filter),
         columns=["unit_id"],
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "Invalid #3 and/or #4 columns",
+        raise ValidationError(
+            "#3 and #4 columns",
             errors=_get_error_list(
                 invalid_rows, "Invalid #3 and/or #4 columns"
             ),
         )
 
 
-def _accumulated_temporal_variables_check(parquet_path: str):
+def _accumulated_temporal_variables_check(data: FileSystemDataset):
     """
     Any given row in a table with temporalityType=ACCUMULATED is valid only if:
     * The start_epoch_days column contains a non-null value (int32)
     * The stop_epoch_days is non-null (int32) value bigger than start_epoch_days
     """
     start_is_null_filter = dataset.field("start_epoch_days").is_null()
     stop_is_null_filter = dataset.field("stop_epoch_days").is_null()
     start_be_stop_filter = dataset.field("start_epoch_days") >= dataset.field(
         "stop_epoch_days"
     )
-    invalid_rows = dataset.dataset(parquet_path).to_table(
+    invalid_rows = data.to_table(
         filter=(
             start_is_null_filter | stop_is_null_filter | start_be_stop_filter
         ),
         columns=["unit_id"],
     )
     if len(invalid_rows) > 0:
-        raise ValueError(
-            "Invalid #3 and/or #4 columns",
+        raise ValidationError(
+            "#3 and #4 columns",
             errors=_get_error_list(
                 invalid_rows, "Invalid #3 and/or #4 columns"
             ),
         )
 
 
-def _only_unique_identifiers_check(parquet_path: str):
+def _only_unique_identifiers_check(data: FileSystemDataset):
     """
     A table with temporalityType=FIXED is only valid if all
     cells in the unit_id column are unique.
     """
-    identifiers = dataset.dataset(parquet_path).to_table(
-        columns=["unit_id"],
-    )
+    identifiers = data.to_table(columns=["unit_id"])
     identifiers = Table.from_arrays(
         [
             compute.utf8_slice_codeunits(
                 identifiers["unit_id"], start=0, stop=1
             ),
             identifiers["unit_id"],
         ],
@@ -215,47 +215,44 @@
     for unique_bucket in unique_buckets:
         bucket_table = identifiers.filter(
             dataset.field("bucket") == unique_bucket
         )
         bucket_row_count = len(bucket_table)
         unique_identifiers_count = len(compute.unique(bucket_table["unit_id"]))
         if unique_identifiers_count != bucket_row_count:
-            raise ValueError(
-                "Duplicate identifiers in #1 column",
+            raise ValidationError(
+                "#1 column",
                 errors=["Duplicate identifiers in #1 column"],
             )
 
 
-def _status_uniquesness_check(parquet_path: str):
+def _status_uniquesness_check(data: FileSystemDataset):
     """
     A table with temporalityType=STATUS is valid only if all
     cells in the unit_id column are unique per status date.
     """
-    all_status_dates = dataset.dataset(parquet_path).to_table(
-        columns=["start_epoch_days"],
-    )
+    all_status_dates = data.to_table(columns=["start_epoch_days"])
     unique_status_dates = compute.unique(all_status_dates["start_epoch_days"])
     for status_date in unique_status_dates:
-        status_table = dataset.dataset(parquet_path).to_table(
+        status_table = data.to_table(
             columns=["unit_id"],
             filter=dataset.field("start_epoch_days") == status_date,
         )
         unique_identifiers = compute.unique(status_table["unit_id"])
         if len(unique_identifiers) != len(status_table):
-            raise ValueError(
-                "Same unit_id (#1 Column) has duplicate dates "
-                "(#3 and #4 column)",
+            raise ValidationError(
+                "#1, #3 and #4 columns",
                 errors=[
                     "Same unit_id (#1 Column) has duplicate dates "
                     "(#3 and #4 column)"
                 ],
             )
 
 
-def _no_overlapping_timespans_check(parquet_path: str):
+def _no_overlapping_timespans_check(data: FileSystemDataset):
     """
     A table with temporalityType=(EVENT|ACCUMULATED) is valid
     only if all rows for a given identifier contains no overlapping
     timespans in the start_epoch_days and stop_epoch_days columns.
     """
 
     def find_overlap(start_list, stop_list):
@@ -271,20 +268,18 @@
                 return True
         return False
 
     def batch(iterable, batch_size):
         for index in range(0, len(iterable), batch_size):
             yield iterable[index : index + batch_size]
 
-    identifiers = dataset.dataset(parquet_path).to_table(
-        columns=["unit_id"],
-    )
+    identifiers = data.to_table(columns=["unit_id"])
     unique_identifiers = compute.unique(identifiers["unit_id"])
     for identifier_batch in batch(unique_identifiers, 5_000_000):
-        identifier_time_spans = dataset.dataset(parquet_path).to_table(
+        identifier_time_spans = data.to_table(
             filter=dataset.field("unit_id").isin(identifier_batch),
             columns=["unit_id", "start_epoch_days", "stop_epoch_days"],
         )
         identifier_time_spans = identifier_time_spans.sort_by(
             [("start_epoch_days", "ascending")]
         )
         identifier_time_spans = identifier_time_spans.group_by(
@@ -294,38 +289,38 @@
         )
         for i in range(len(identifier_time_spans)):
             if find_overlap(
                 identifier_time_spans["start_epoch_days_list"][i].as_py(),
                 identifier_time_spans["stop_epoch_days_list"][i].as_py(),
             ):
                 raise ValidationError(
-                    "Found overlapping timespans for dataset",
+                    "#1, #3 and #4 columns",
                     errors=[
                         "Invalid overlapping timespans for identifier"
                         f' "{identifier_time_spans["unit_id"][i]}"'
                     ],
                 )
 
 
 def validate_dataset(
-    parquet_path: str,
+    data: FileSystemDataset,
     measure_data_type: str,
     code_list: Union[List, None],
     sentinel_list: Union[List, None],
     temporality_type: str,
 ) -> None:
-    _valid_unit_id_check(parquet_path)
+    _valid_unit_id_check(data)
     _valid_value_column_check(
-        parquet_path, measure_data_type, code_list, sentinel_list
+        data, measure_data_type, code_list, sentinel_list
     )
     if temporality_type == "FIXED":
-        _fixed_temporal_variables_check(parquet_path)
-        _only_unique_identifiers_check(parquet_path)
+        _fixed_temporal_variables_check(data)
+        _only_unique_identifiers_check(data)
     elif temporality_type == "STATUS":
-        _status_temporal_variables_check(parquet_path)
-        _status_uniquesness_check(parquet_path)
+        _status_temporal_variables_check(data)
+        _status_uniquesness_check(data)
     elif temporality_type == "ACCUMULATED":
-        _accumulated_temporal_variables_check(parquet_path)
-        _no_overlapping_timespans_check(parquet_path)
+        _accumulated_temporal_variables_check(data)
+        _no_overlapping_timespans_check(data)
     elif temporality_type == "EVENT":
-        _event_temporal_variables_check(parquet_path)
-        _no_overlapping_timespans_check(parquet_path)
+        _event_temporal_variables_check(data)
+        _no_overlapping_timespans_check(data)
```

### Comparing `microdata_tools-0.4.0/microdata_tools/validation/steps/metadata_reader.py` & `microdata_tools-0.5.0/microdata_tools/validation/steps/metadata_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-import logging
 from pathlib import Path
+from typing import Dict
 
 from microdata_tools.validation.model import validate_metadata_model
-from microdata_tools.validation.model.metadata import Metadata
 from microdata_tools.validation.adapter import local_storage
 from microdata_tools.validation.components import (
     temporal_attributes,
     unit_type_variables,
 )
 
 
-logger = logging.getLogger()
-
-
 def _insert_centralized_variable_definitions(metadata: dict):
     metadata["identifierVariables"] = [
         unit_type_variables.get(metadata["identifierVariables"][0]["unitType"])
     ]
     measure_variable = metadata["measureVariables"][0]
     if "unitType" in measure_variable:
         insert_measure = unit_type_variables.get(measure_variable["unitType"])
@@ -26,15 +22,14 @@
     temporality_type = metadata["temporalityType"]
     metadata["attributeVariables"] = [
         temporal_attributes.generate_start_time_attribute(temporality_type),
         temporal_attributes.generate_stop_time_attribute(temporality_type),
     ] + metadata.get("attributeVariables", [])
 
 
-def run_reader(dataset_name: str, metadata_file_path: Path) -> Metadata:
-    logger.debug("Validating metadata JSON with JSON schema")
+def run_reader(dataset_name: str, metadata_file_path: Path) -> Dict:
     metadata_dict = local_storage.load_json(metadata_file_path)
     validate_metadata_model(metadata_dict)
     _insert_centralized_variable_definitions(metadata_dict)
     metadata_dict["shortName"] = dataset_name
     metadata_dict["measureVariables"][0]["shortName"] = dataset_name
     return metadata_dict
```

### Comparing `microdata_tools-0.4.0/pyproject.toml` & `microdata_tools-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microdata-tools"
-version = "0.4.0"
+version = "0.5.0"
 description = "Tools for the microdata.no platform"
 authors = ["microdata-developers"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "microdata_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `microdata_tools-0.4.0/PKG-INFO` & `microdata_tools-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdata-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for the microdata.no platform
 License: MIT
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

