# Comparing `tmp/twinlab-1.1.6.tar.gz` & `tmp/twinlab-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.1.6.tar", max compression
+gzip compressed data, was "twinlab-1.2.0.tar", max compression
```

## Comparing `twinlab-1.1.6.tar` & `twinlab-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.6/LICENSE
--rw-r--r--   0        0        0     2038 2023-08-07 13:01:26.283451 twinlab-1.1.6/README.md
--rw-r--r--   0        0        0      918 2023-08-08 08:09:27.328810 twinlab-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      610 2023-08-07 13:43:44.946573 twinlab-1.1.6/twinlab/__init__.py
--rw-r--r--   0        0        0      130 2023-08-07 13:01:26.329604 twinlab-1.1.6/twinlab/_version.py
--rw-r--r--   0        0        0    15457 2023-08-08 08:29:39.891281 twinlab-1.1.6/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.6/twinlab/plotting.py
--rw-r--r--   0        0        0      866 2023-08-07 13:01:26.330439 twinlab-1.1.6/twinlab/settings.py
--rw-r--r--   0        0        0     4957 2023-08-08 08:38:37.275490 twinlab-1.1.6/twinlab/utils.py
--rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 twinlab-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4141 2023-07-27 16:36:18.090352 twinlab-1.2.0/README.md
+-rw-r--r--   0        0        0      971 2023-07-27 16:36:18.092899 twinlab-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-07-27 16:36:18.125512 twinlab-1.2.0/twinlab/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-27 16:36:18.125824 twinlab-1.2.0/twinlab/_version.py
+-rw-r--r--   0        0        0     5422 2023-07-27 16:36:18.125924 twinlab-1.2.0/twinlab/api.py
+-rw-r--r--   0        0        0    18545 2023-07-27 16:36:18.126106 twinlab-1.2.0/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.2.0/twinlab/plotting.py
+-rw-r--r--   0        0        0     1608 2023-07-27 16:36:18.126350 twinlab-1.2.0/twinlab/settings.py
+-rw-r--r--   0        0        0     4041 2023-07-27 16:36:18.126482 twinlab-1.2.0/twinlab/utils.py
+-rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 twinlab-1.2.0/PKG-INFO
```

### Comparing `twinlab-1.1.6/LICENSE` & `twinlab-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.6/pyproject.toml` & `twinlab-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.1.6"
+version = "1.2.0"
 description = "Client interface for twinLab machine-learning in the cloud."
 license = "MIT"
 homepage = "https://www.digilab.co.uk/"
 repository = "https://github.com/digiLab-ai/twinLab-client"
 documentation = "https://digilab-ai.github.io/twinLab-client"
 authors = ["DigiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
@@ -13,18 +13,21 @@
     "Jordan Hart <jordan@digilab.co.uk>",
 ]
 keywords = ["machine-learning", "AI", "cloud", "twinLab", "digiLab"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-numpy = "^1.25.1"
+numpy = "^1.25.0"
 pandas = "^1.5.3"
 pydantic = { version = "^1.10.7", extras = ["dotenv"] }
 requests = "^2.28.2"
+typeguard = "^4.0.0"
+
+[tool.poetry.dev-dependencies]
 ipykernel = "^6.22.0"
 IPython = "^8.11"
 matplotlib = "^3.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `twinlab-1.1.6/twinlab/client.py` & `twinlab-1.2.0/twinlab/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,492 +1,668 @@
 # Standard imports
 import io
 import json
+from typing import Union, Tuple
 from pprint import pprint
-from typing import Union
+import time
 
 # Third-party imports
-import requests
 import pandas as pd
+from typeguard import typechecked
 
 # Project imports
+from . import api
 from . import utils
-from .settings import ENV
+from . import settings
+
+
+### Utility functions ###
+
+# TODO: Move to utils.py?
+
+
+def _status_campaign(campaign_id: str, verbose=False, debug=False) -> dict:
+    response = api.status_model(campaign_id, verbose=debug)
+    if verbose:
+        message = _get_message(response)
+        print(message)
+    return response
+
+
+def _use_campaign(filepath_or_df: Union[str, pd.DataFrame], campaign_id: str,
+                  method: str, n_samples=None,
+                  verbose=False, debug=False) -> pd.DataFrame:
+
+    if type(filepath_or_df) is str:
+        filepath = filepath_or_df
+        eval_csv = open(filepath, "rb").read()
+    else:
+        df = filepath_or_df
+        buffer = io.BytesIO()
+        df.to_csv(buffer, index=False)
+        eval_csv = buffer.getvalue()
+    if settings.CHECK_DATASETS:
+        utils.check_dataset(eval_csv.decode("utf-8"))
+    output_csv = api.use_model(eval_csv, campaign_id, method=method,
+                               processor="cpu", verbose=debug)
+    df = pd.read_csv(io.StringIO(output_csv), sep=",")
+    return df
+
+
+def _get_message(response: dict) -> str:
+    # TODO: This could be a method of the response object
+    # TODO: This should be better
+    try:
+        message = response["message"]
+    except:
+        message = response
+    return message
+
+### ###
+
+### General functions ###
+
+
+@typechecked
+def get_user_information(verbose=False, debug=False) -> dict:
+    """
+    # Get user information
+
+    Get information about the user
+
+    ## Arguments
+
+    - `verbose`: `bool` determining level of information returned to the user
+    - `debug`: `bool` determining level of information logged on the server
+
+    ## Returns
+
+    - `dict` containing user information
+
+    ## Example
+    ```
+    import twinlab as tl
+
+    user_info = tl.get_user_information()
+    print(user_info)
+    ```
+    """
+    user_info = api.get_user(verbose=debug)
+    if verbose:
+        print("User information:")
+        pprint(user_info, compact=True, sort_dicts=False)
+    return user_info
+
+
+@typechecked
+def get_versions(verbose=False, debug=False) -> dict:
+    """
+    # Get versions
+
+    Get information about the twinLab version being used
+
+    ## Arguments
+
+    - `verbose`: `bool` determining level of information returned to the user
+    - `debug`: `bool` determining level of information logged on the server
+
+    ## Returns
+
+    - `dict` containing version information
+
+    ## Example
+    ```
+    import twinlab as tl
+
+    version_info = tl.get_versions()
+    print(version_info)
+    ```
+    """
+    version_info = api.get_versions(verbose=debug)
+    if verbose:
+        print("Version information:")
+        pprint(version_info, compact=True, sort_dicts=False)
+    return version_info
+
+### ###
 
 ### Dataset functions ###
 
 
-def upload_dataset(filepath_or_df: Union[str, pd.DataFrame], dataset_name: str, verbose=False, debug=False) -> None:
+@typechecked
+def upload_dataset(filepath_or_df: Union[str, pd.DataFrame], dataset_id: str,
+                   verbose=False, debug=False) -> None:
     """
     # Upload dataset
 
     Upload a dataset to the `twinLab` cloud so that it can be queried and used for training.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
     - `filepath_or_df`: `str` | `Dataframe`; location of csv dataset on local machine or `pandas` dataframe
-    - `dataset_name`: `str`; name for the dataset when saved to the twinLab cloud
+    - `dataset_id`: `str`; name for the dataset when saved to the twinLab cloud
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
-    **NOTE:** Local data must be a CSV file. If a `pandas` dataframe is uploaded then a `dataset_name` must be provided. 
-    If a local file is uploaded then the filename with the directories removed will be the uploaded file name, 
-    unless a value of `dataset_name` is provided, which will be used preferentially.
+    **NOTE:** Local data must be a CSV file, working data should be a pandas Dataframe. 
+    In either case a `dataset_id` must be provided.
 
     ## Examples
 
     Upload a local file:
     ```python
     import twinlab as tl
 
-    dataset_filepath = "resources/data/my_data.csv"
-    dataset_name = "my_data"
-    tl.upload_dataset(dataset_filepath, dataset_name)
+    data_filepath = "resources/data/my_data.csv"
+    tl.upload_dataset(data_filepath, "my_dataset") # This will be my_data.csv in the cloud
     ```
 
     Upload a `pandas` dataframe:
     ```python
     import pandas as pd
     import twinlab as tl
 
-    dataset = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    dataset_name = "my_data"
-    tl.upload_dataset(dataset, dataset_name)
+    dataframe = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+    tl.upload_dataset(dataframe, "my_dataset")
     ```
     """
 
-    # Sort-out dataset_name
-    if ("/" in dataset_name) or ("\\" in dataset_name):
-        raise ValueError("Dataset name cannot contain '/' or '\\'")
+    # Upload the file (either via link or directly)
+    if settings.USE_UPLOAD_URL:
+        upload_url = api.generate_upload_url(dataset_id, verbose=debug)
+        if type(filepath_or_df) is str:
+            filepath = filepath_or_df
+            utils.upload_file_to_presigned_url(
+                filepath, upload_url, verbose=verbose, check=settings.CHECK_DATASETS)
+        elif type(filepath_or_df) is pd.DataFrame:
+            df = filepath_or_df
+            utils.upload_dataframe_to_presigned_url(
+                df, upload_url, verbose=verbose, check=settings.CHECK_DATASETS)
+        else:
+            raise ValueError(
+                "filepath_or_df must be a string or pandas dataframe")
+        if verbose:
+            print("Processing dataset.")
+        response = api.process_uploaded_dataset(dataset_id, verbose=debug)
 
-    # Get the upload URL
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Dataset"] = dataset_name
-    lambda_url = ENV.TWINLAB_SERVER + "/generate_upload_url"
-    r = requests.get(lambda_url, headers=headers)
-    utils.check_response(r)
-
-    # Upload the file
-    if verbose:
-        utils.print_response_message(r)
-    upload_url = r.json()["url"]
-    if type(filepath_or_df) is str:
-        filepath = filepath_or_df
-        utils.upload_file_to_presigned_url(
-            filepath, upload_url, verbose=verbose)
     else:
-        df = filepath_or_df
-        utils.upload_dataframe_to_presigned_url(
-            df, upload_url, verbose=verbose)
-    if verbose:
-        print(f"Uploading {dataset_name}")
+        if type(filepath_or_df) is str:
+            filepath = filepath_or_df
+            csv_string = open(filepath, "rb").read()
+        elif type(filepath_or_df) is pd.DataFrame:
+            df = filepath_or_df
+            buffer = io.BytesIO()
+            df.to_csv(buffer, index=False)
+            csv_string = buffer.getvalue()
+        else:
+            raise ValueError(
+                "filepath_or_df must be a string or pandas dataframe")
+        if settings.CHECK_DATASETS:
+            utils.check_dataset(csv_string.decode("utf-8"))
+        response = api.upload_dataset(csv_string, dataset_id, verbose=debug)
 
-    # Process the uploaded dataset remotely
-    process_url = ENV.TWINLAB_SERVER + "/process_uploaded_dataset"
-    r = requests.post(process_url, headers=headers)
     if verbose:
-        utils.print_response_message(r)
+        message = _get_message(response)
+        print(message)
 
 
-def query_dataset(dataset_name: str, verbose=False, debug=False) -> pd.DataFrame:
+@typechecked
+def list_datasets(verbose=False, debug=False) -> list:
     """
-    # Query dataset
+    # List datasets
 
-    Query a dataset that exists on the `twinLab` cloud by printing summary statistics.
+    List datasets that have been uploaded to the `twinLab` cloud
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
-    - `dataset_name`: `str`; name of dataset on S3
+    - `verbose`: `bool` determining level of information returned to the user
+    - `debug`: `bool` determining level of information logged on the server
+
+    ## Example
+
+    ```python
+    import twinlab as tl
+
+    datasets = tl.list_datasets()
+    print(datasets)
+    ```
+    """
+    datasets = api.list_datasets(verbose=debug)
+    if verbose:
+        print("Datasets:")
+        pprint(datasets, compact=True, sort_dicts=False)
+    return datasets
+
+
+@typechecked
+def view_dataset(dataset_id: str, verbose=False, debug=False) -> pd.DataFrame:
+    """
+    # View dataset
+
+    View a dataset that exists on the twinLab cloud.
+
+    ## Arguments
+
+    - `dataset_id`: `str`; name for the dataset when saved to the twinLab cloud
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     ## Returns
 
-    `pandas` dataframe containing summary statistics for the dataset.
+    - `pandas.DataFrame` of the dataset.
 
-    ## Example
+
+   ## Example
 
     ```python
     import twinlab as tl
 
-    dataset_name = "my_dataset.csv"
-    df = tl.query_dataset(dataset_name)
+    df = tl.view_dataset("my_dataset")
     print(df)
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/query_dataset"
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Dataset"] = dataset_name
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    df = utils.extract_csv_from_response(r, "summary")
+    response = api.view_dataset(dataset_id, verbose=debug)
+    csv_string = io.StringIO(response)
+    df = pd.read_csv(csv_string, sep=",")
     if verbose:
-        utils.print_response_message(r)
-        print("Summary:\n", df)
+        print("Dataset:")
+        print(df)
     return df
 
 
-def list_datasets(verbose=False, debug=False) -> Union[list, None]:
+@typechecked
+def query_dataset(dataset_id: str, verbose=False, debug=False) -> pd.DataFrame:
     """
-    # List datasets
+    # Query dataset
 
-    List datasets that have been uploaded to the `twinLab` cloud
+    Query a dataset that exists on the `twinLab` cloud by printing summary statistics.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
+    - `dataset_id`: `str`; name of dataset on S3 (same as the uploaded file name)
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
+    ## Returns
+
+    - `pandas.DataFrame` containing summary statistics for the dataset.
+
     ## Example
 
     ```python
     import twinlab as tl
 
-    datasets = tl.list_datasets()
-    print(datasets)
+    df = tl.query_dataset("my_dataset")
+    print(df)
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/list_datasets"
-    headers = utils.construct_standard_headers(debug=debug)
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
-    datasets = r.json()["datasets"]
-    if verbose and datasets:
-        print("Datasets:")
-        pprint(datasets, compact=True)
-    return datasets
+    response = api.summarise_dataset(dataset_id, verbose=debug)
+    csv_string = io.StringIO(response)
+    df = pd.read_csv(csv_string, sep=",")
+    if verbose:
+        print("Dataset summary:")
+        print(df)
+    return df
 
 
-def delete_dataset(dataset_name: str, verbose=False, debug=False) -> None:
+@typechecked
+def delete_dataset(dataset_id: str, verbose=False, debug=False) -> None:
     """
     # Delete dataset
 
     Delete a dataset from the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
-    - `dataset_name`: `str`; name of dataset to delete from the cloud
+    - `dataset_id`: `str`; name of dataset to delete from the cloud
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
+    ## Returns
+
+    - `list` of `str` dataset ids
+
     ## Example
 
     ```python
     import twinlab as tl
 
-    dataset_name = "my_dataset.csv"
-    tl.delete_dataset(dataset_name)
+    tl.delete_dataset("my_dataset")
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/delete_dataset"
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Dataset"] = dataset_name
-    r = requests.post(url, headers=headers)
-    utils.check_response(r)
+    response = api.delete_dataset(dataset_id, verbose=debug)
     if verbose:
-        utils.print_response_message(r)
+        message = _get_message(response)
+        print(message)
 
 ###  ###
 
 ### Campaign functions ###
 
 
-def train_campaign(filepath_or_params: Union[str, dict], campaign_name: str, verbose=False, debug=False) -> None:
+@typechecked
+def train_campaign(filepath_or_params: Union[str, dict], campaign_id: str,
+                   verbose=False, debug=False) -> None:
     """
     # Train campaign
 
     Train a campaign in the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
     - `filepath_or_params`: `str` | `dict`; filepath to local json or parameters dictionary for training
-    - `campaign_name`: `str`; name for the final trained model
+    - `campaign_id`: `str`; name for the final trained campaign
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     ## Example
 
     Train using a local `json` parameters file:
     ```python
-    tl.train_campaign("params.json", "my_campaign", verbose=True)
+    import twinlab as tl
+
+    tl.train_campaign("path/to/params.json", "my_campaign")
     ```
 
     Train via a `python` dictionary:
     ```python
+    import twinlab as tl
+
     params = {
-        "dataset": "my_dataset",
-        "inputs": ["X1", "X2"],
-        "outputs": ["y1", "y2"],
+        "dataset_id": "my_dataset",
+        "inputs": ["X"],
+        "outputs": ["y"],
     }
-    tl.train_campaign(params, "my_campaign", verbose=True)
+    tl.train_campaign(params, "my_campaign")
     ```
     """
-    long_training_server = ENV.TWINLAB_TRAINING_SERVER
-    training_server = ENV.TWINLAB_SERVER + "/train_campaign"
-    url = long_training_server if long_training_server else training_server
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Campaign"] = campaign_name
-    if isinstance(filepath_or_params, str):
+    if type(filepath_or_params) is dict:
+        params = filepath_or_params
+    elif type(filepath_or_params) is str:
         filepath = filepath_or_params
-        with open(filepath) as f:
-            params = json.load(f)
+        params = json.load(open(filepath))
     else:
-        params = filepath_or_params
+        print("Type:", type(filepath_or_params))
+        raise ValueError(
+            "filepath_or_params must be either a string or a dictionary")
     params = utils.coerce_params_dict(params)
-    r = requests.post(url, json=params, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
+    params_str = json.dumps(params)
+    response = api.train_model(
+        params_str, campaign_id, processor="cpu", verbose=debug)
+    if verbose:
+        message = _get_message(response)
+        print(message)
+
+    # Wait for job to complete
+    complete = False
+    while not complete:
+        status = _status_campaign(campaign_id, verbose=False, debug=debug)
+        complete = status["job_complete"]
+        time.sleep(settings.WAIT_TIME)
 
 
-def query_campaign(campaign_name: str, verbose=False, debug=False) -> dict:
+@typechecked
+def list_campaigns(verbose=False, debug=False) -> list:
     """
-    # Query campaign
+    # List datasets
 
-    Get summary statistics for a pre-trained campaign in the `twinLab` cloud.
+    List campaigns that have been completed to the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
-    - `campaign_name`: `str`; name of trained model to query
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     ## Returns
 
-    dictionary containing summary statistics for the dataset.
+    - A `list` of `str` campaign ids
 
     ## Example
 
     ```python
-    import twinlab_client as tl
+    import twinlab as tl
+
+    campaigns = tl.list_campaigns()
+    print(campaigns)
+    ```
+    """
+    campaigns = api.list_models(verbose=debug)
+    if verbose:
+        print("Trained models:")
+        pprint(campaigns, compact=True, sort_dicts=False)
+    return campaigns
+
+
+@typechecked
+def view_campaign(campaign_id: str, verbose=False, debug=False) -> dict:
+    """
+    # View dataset
+
+    View a campaign that exists on the twinLab cloud.
+
+    ## Arguments
+
+    - `campaign_id`: `str`; name for the model when saved to the twinLab cloud
+    - `verbose`: `bool` determining level of information returned to the user
+    - `debug`: `bool` determining level of information logged on the server
+
+    ## Returns
+
+    - `dict` containing the campaign training parameters.
+
+   ## Example
+
+    ```python
+    import twinlab as tl
 
-    campaign = "my_campaign"
-    tl.query_campaign(campaign)
+    params = tl.view_campaign("my_campaign")
+    print(params)
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/query_campaign"
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Campaign"] = campaign_name
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    metadata = utils.extract_item_from_response(r, "metadata")
+    query = api.view_model(campaign_id, verbose=debug)
     if verbose:
-        utils.print_response_message(r)
-        print("Metadata:")
-        pprint(metadata, compact=True, sort_dicts=False)
-    return metadata
+        print("Campaign summary:")
+        pprint(query, compact=True, sort_dicts=False)
+    return query
 
 
-def list_campaigns(verbose=False, debug=False) -> Union[list, None]:
+@typechecked
+def query_campaign(campaign_id: str, verbose=False, debug=False) -> dict:
     """
-    # List datasets
+    # Query campaign
 
-    List datasets that have been uploaded to the `twinLab` cloud.
+    Get summary statistics for a pre-trained campaign in the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
+    - `campaign_id`: `str`; name of trained campaign to query
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     ## Returns
 
-    A list of `str` dataset names, or `None` if there are no datasets
+    - dictionary containing summary statistics for the dataset.
 
     ## Example
 
     ```python
     import twinlab as tl
 
-    datasets = tl.list_datasets()
-    print(datasets)
+    info = tl.query_campaign("my_campaign")
+    print(info)
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/list_campaigns"
-    headers = utils.construct_standard_headers(debug=debug)
-    r = requests.get(url, headers=headers)
-    utils.check_response(r)
-    if verbose:
-        utils.print_response_message(r)
-    campaigns = r.json()["campaigns"]
-    if verbose and campaigns:
-        print("Campaigns:")
-        pprint(campaigns)
-    return campaigns
+    # TODO: This should eventually return a proper dictionary
+    summary = api.summarise_model(campaign_id, verbose=debug)
+    summary = {"diagnostics": summary}  #  TODO: Remove this hack
+    if verbose:
+        print("Model summary:")
+        pprint(summary, compact=True, sort_dicts=False)
+    return summary
 
 
-def predict_campaign(filepath_or_df: Union[str, pd.DataFrame], campaign_name: str,
-                     verbose=False, debug=False) -> tuple:
+@typechecked
+def predict_campaign(filepath_or_df: Union[str, pd.DataFrame], campaign_id: str,
+                     verbose=False, debug=False) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     # Predict campaign
 
     Predict from a pre-trained campaign that exists on the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
     - `filepath_or_df`: `str`; location of csv dataset on local machine for evaluation or `pandas` dataframe
-    - `campaign_name`: `str`; name of pre-trained model to use for predictions
+    - `campaign_id`: `str`; name of pre-trained campaign to use for predictions
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     **NOTE:** Evaluation data must be a CSV file, or a `pandas` dataframe that is interpretable as a CSV.
 
     ## Returns
 
-    `tuple` containing:
-    - `df_mean`: `pandas` dataframe containing mean predictions
-    - `df_stdv`: `pandas` dataframe containing standard deviation predictions
+    - `tuple` containing:
+        - `df_mean`: `pandas.DataFrame` containing mean predictions
+        - `df_std`: `pandas.DataFrame` containing standard deviation predictions
+
 
     ## Example
 
-    Use a local file:
+    Using a local file:
     ```python
-    import twinlab_client as tl
+    import twinlab as tl
 
     filepath = "resources/data/eval.csv" # Local
-    campaign_name = "my_campaign" # Pre-trained
-    df_mean, df_stdv = tl.predict_campaign(file, campaign_name)
+    campaign_id = "my_campaign" # Pre-trained
+    df_mean, df_std = tl.predict_campaign(file, campaign_id)
     ```
 
-    Use a `pandas` dataframe:
+    Using a `pandas` dataframe:
     ```python
     import pandas as pd
     import twinlab as tl
 
-    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]}
-    campaign_name = "my_campaign" # Pre-trained
-    df_mean, df_stdv = tl.predict_campaign(file, campaign_name)
+    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
+    tl.predict_campaign(df, "my_campaign")
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/predict_campaign"
-    if isinstance(filepath_or_df, pd.DataFrame):  # Data frames
-        buffer = io.BytesIO()
-        filepath_or_df.to_csv(buffer, index=False)
-        buffer = buffer.getvalue()
-        files = {"file": ("tmp.csv", buffer, "text/csv")}
-    else:  # File paths
-        files = {"file": (filepath_or_df, open(
-            filepath_or_df, "rb"), "text/csv")}
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Campaign"] = campaign_name
-    r = requests.post(url, files=files, headers=headers)
-    utils.check_response(r)
-    df_mean = utils.extract_csv_from_response(r, "y_mean")
-    df_stdv = utils.extract_csv_from_response(r, "y_std")
-    if verbose:
-        utils.print_response_message(r)
-        print("Mean: \n", df_mean, "\n")
-        print("Stdv: \n", df_stdv)
-    return df_mean, df_stdv
+
+    df = _use_campaign(filepath_or_df, campaign_id, method="predict",
+                       verbose=verbose, debug=debug)
+
+    n = len(df.columns)
+    df_mean, df_std = df.iloc[:, :n//2], df.iloc[:, n//2:]
+    df_std.columns = df_std.columns.str.removesuffix(" [std_dev]")
+    if verbose:
+        print("Mean predictions:")
+        print(df_mean)
+        print("Standard deviation predictions:")
+        print(df_std)
+
+    return df_mean, df_std
 
 
-def sample_campaign(filepath_or_df: Union[str, pd.DataFrame], campaign_name: str, n_samples: int,
+@typechecked
+def sample_campaign(filepath_or_df: Union[str, pd.DataFrame], campaign_id: str, n_samples: int,
                     verbose=False, debug=False) -> pd.DataFrame:
     """
-    # Predict campaign
+    # Sample campaign
 
-    Sample from the posterior of a pre-trained campaign that exists on the `twinLab` cloud.
+    Draw samples from a pre-trained campaign that exists on the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
     - `filepath_or_df`: `str`; location of csv dataset on local machine for evaluation or `pandas` dataframe
-    - `campaign_name`: `str`; name of pre-trained model to use for predictions
-    - `n_samples`: `int`; number of samples to draw from the posterior
+    - `campaign_id`: `str`; name of pre-trained campaign to use for predictions
+    - `n_samples`: `int`; number of samples to draw for each row of the evaluation data
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     **NOTE:** Evaluation data must be a CSV file, or a `pandas` dataframe that is interpretable as a CSV.
 
     ## Returns
 
-    - `df_sample`: multi-indexed `pandas` dataframe containing samples
+    - `tuple` containing:
+        - `df_mean`: `pandas.DataFrame` containing mean predictions
+        - `df_std`: `pandas.DataFrame` containing standard deviation predictions
+
 
     ## Example
 
-    Use a local file:
+    Using a local file:
     ```python
-    import twinlab_client as tl
+    import twinlab as tl
 
     filepath = "resources/data/eval.csv" # Local
-    campaign_name = "my_campaign" # Pre-trained
-    df_samples = tl.sample_campaign(file, campaign_name, 10)
+    campaign_id = "my_campaign" # Pre-trained
+    n = 10
+    df_mean, df_std = tl.sample_campaign(file, campaign_id, n)
     ```
 
-    Use a `pandas` dataframe:
+    Using a `pandas` dataframe:
     ```python
     import pandas as pd
     import twinlab as tl
 
-    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]}
-    campaign_name = "my_campaign" # Pre-trained
-    df_samples = tl.sample_campaign(df, campaign_name, 10)
+    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
+    n = 10
+    tl.sample_campaign(df, "my_campaign", n)
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/sample_campaign"
-    if isinstance(filepath_or_df, pd.DataFrame):  # Data frames
-        buffer = io.BytesIO()
-        filepath_or_df.to_csv(buffer, index=False)
-        buffer = buffer.getvalue()
-        files = {"file": ("tmp.csv", buffer, "text/csv")}
-    else:  # File paths
-        files = {"file": (filepath_or_df, open(
-            filepath_or_df, "rb"), "text/csv")}
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Campaign"] = campaign_name
-    r = requests.post(url, files=files, headers=headers)
-    utils.check_response(r)
-    df_samples = utils.extract_csv_from_response(r, "y_samples", [0, 1])
+
+    df_samples = _use_campaign(filepath_or_df, campaign_id,
+                               method="sample", n_samples=n_samples,
+                               verbose=verbose, debug=debug)
+    # TODO: Munge to get the format correct
     if verbose:
-        utils.print_response_message(r)
-        print("Samples: \n", df_samples)
+        print("Samples:")
+        print(df_samples)
+
     return df_samples
 
 
-def delete_campaign(campaign_name: str, verbose=False, debug=False) -> None:
+@typechecked
+def delete_campaign(campaign_id: str, verbose=False, debug=False) -> None:
     """
     # Delete campaign
 
     Delete campaign from the `twinLab` cloud.
 
     **NOTE:** Your user information is automatically added to the request using the `.env` file.
 
     ## Arguments
 
-    - `campaign_name`: `str`; name of trained model to delete from the cloud
+    - `campaign_id`: `str`; name of trained campaign to delete from the cloud
     - `verbose`: `bool` determining level of information returned to the user
     - `debug`: `bool` determining level of information logged on the server
 
     ## Example
 
     ```python
     import twinlab as tl
 
-    campaign = "my_campaign"
-    tl.delete_campaign(campaign)
+    tl.delete_campaign("my_campaign")
     ```
     """
-    url = ENV.TWINLAB_SERVER + "/delete_campaign"
-    headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Campaign"] = campaign_name
-    r = requests.post(url, headers=headers)
-    utils.check_response(r)
+    response = api.delete_model(campaign_id, verbose=debug)
     if verbose:
-        utils.print_response_message(r)
+        message = _get_message(response)
+        print(message)
+
+### ###
```

### Comparing `twinlab-1.1.6/twinlab/utils.py` & `twinlab-1.2.0/twinlab/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,176 +1,120 @@
 # Standard imports
 import io
-import argparse
-import json
-from pprint import pprint
 
 # Third-party imports
 import requests
+import numpy as np
 import pandas as pd
 
 # Project imports
-from .settings import ENV
-
-# Convert these names in the params file
-PARAMS_COERCION = {
-    "test_train_split": "train_test_split",  # Common mistake
-    "num_training_examples": "train_test_split",  #  TODO: Think of something better
-    "filename": "dataset",  # Suppoprt old name
-    "filename_std": "dataset_std",  # Support old name
-}
-
+from . import settings
 
 ### Utility functions ###
 
 
-# def unwrap_payload(event: dict) -> dict:
-#     """
-#     Return payload and decode if it is base64 encoded
-#     TODO: Not used yet...
-#     """
-#     if "body" not in event:  # Get body
-#         raise Exception("No body in request")
-#     body = event["body"]
-#     if "isBase64Encoded" in event:  # Decode
-#         if event["isBase64Encoded"]:
-#             body = base64.b64decode(body)
-#     try:  # Parse
-#         payload = json.loads(body)
-#     except:
-#         raise Exception("Could not parse body as JSON")
-#     return payload
-
-
-def get_command_line_args() -> argparse.Namespace:
-    """
-    Parse command-line arguments
-    """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "server",
-        default="cloud",
-        nargs='?',
-        help="Specify whether to use local or cloud lambda function",
-    )
-    args = parser.parse_args()
-    return args
-
-
-def construct_standard_headers(debug=False) -> dict:
-    headers = {
-        "X-Group": ENV.TWINLAB_GROUPNAME,
-        "X-User": ENV.TWINLAB_USERNAME,
-        "authorizationToken": ENV.TWINLAB_TOKEN,
-        "X-Debug": str(debug).lower(),
-    }
-    return headers
-
-
 def coerce_params_dict(params: dict) -> dict:
     """
     Relabel parameters to be consistent with twinLab library
     """
-    for param in PARAMS_COERCION:
+    if "train_test_split" in params.keys() or "test_train_split" in params.keys():
+        raise TypeError(
+            "train_test_split is deprecated. Use train_test_ratio instead.")
+    for param in settings.PARAMS_COERCION:
         if param in params:
-            params[PARAMS_COERCION[param]] = params.pop(param)
+            params[settings.PARAMS_COERCION[param]] = params.pop(param)
+    if "train_test_ratio" not in params.keys():
+        params["train_test_ratio"] = settings.DEFAULT_TRAIN_TEST_RATIO
     return params
 
 
+def check_dataset(string: str) -> None:
+    """
+    Check that a sensible dataframe can be created from a CSV string.
+    """
+
+    # Can we parse the string into a dataframe?
+    try:
+        string_io = io.StringIO(string)
+        df = pd.read_csv(string_io)
+    except Exception:
+        raise TypeError("Could not parse the input into a dataframe.")
+
+    # Check that dataset has at least one column.
+    if df.shape[0] < 1:
+        raise TypeError("Dataset must have at least one column.")
+
+    # Check that dataset has no duplicate column names.
+    # TODO: Is this needed? What if the columns with identical names are not used in training?
+    if len(set(df.columns)) != len(df.columns):
+        raise TypeError("Dataset must contain no duplicate column names.")
+
+    # Check that dataset has at least one row.
+    if df.shape[1] < 1:
+        raise TypeError("Dataset must have at least one row.")
+
+    # Check that the dataset contains only numerical values.
+    if not df.applymap(lambda x: isinstance(x, (int, float))).all().all():
+        raise Warning("Dataset contains non-numerical values.")
+
+    # Warning if the dataset contains missing values.
+    if df.isnull().values.any():
+        raise Warning("Dataset contains missing values.")
+
+    # Warning if the dataset contains infinite values.
+    if not np.isfinite(df).all().all():
+        raise Warning("Dataset contains infinite values.")
+
 ### ###
 
 ### HTTP requests ###
 
 
-def upload_file_to_presigned_url(file_path: str, url: str, verbose=False) -> None:
+def upload_file_to_presigned_url(file_path: str, url: str, verbose=False, check=False) -> None:
     """
     Upload a file to the specified pre-signed URL.
     params:
         file_path: str; the path to the local file you want to upload.
         presigned_url: The pre-signed URL generated for uploading the file.
         verbose: bool
     """
-
+    if check:
+        with open(file_path, "rb") as file:
+            csv_string = file.read().decode("utf-8")
+            check_dataset(csv_string)
     with open(file_path, "rb") as file:
         headers = {"Content-Type": "application/octet-stream"}
         response = requests.put(url, data=file, headers=headers)
     if verbose:
         if response.status_code == 200:
-            print(f"File {file_path} uploaded successfully.")
+            print(f"File {file_path} is uploading.")
         else:
             print(f"File upload failed")
             print(f"Status code: {response.status_code}")
             print(f"Reason: {response.text}")
-        print()
 
 
-def upload_dataframe_to_presigned_url(df: pd.DataFrame, url: str, verbose=False) -> None:
+def upload_dataframe_to_presigned_url(df: pd.DataFrame, url: str, verbose=False, check=False) -> None:
     """
     Upload a panads dataframe to the specified pre-signed URL.
     params:
         df: The pandas dataframe to upload
-        presigned_url: The pre-signed URL generated for uploading the file.
+        url: The pre-signed URL generated for uploading the file.
+        verbose: bool
     """
+    if check:
+        csv_string = df.to_csv(index=False)
+        check_dataset(csv_string)
     headers = {"Content-Type": "application/octet-stream"}
     buffer = io.BytesIO()
     df.to_csv(buffer, index=False)
     buffer = buffer.getvalue()
     response = requests.put(url, data=buffer, headers=headers)
     if verbose:
         if response.status_code == 200:
-            print(f"Dataframe uploaded successfully.")
+            print(f"Dataframe is uploading.")
         else:
             print(f"File upload failed")
             print(f"Status code: {response.status_code}")
             print(f"Reason: {response.text}")
-        # print()
-
-
-def extract_csv_from_response(response: requests.Response, name: str, header=[0]) -> pd.DataFrame:
-    """
-    Extract CSV from response
-    """
-    body = response.json()  # Get the body of the response as a dictionary
-    data = body[name]  # Get the entry corresponding to the field name
-    df = pd.read_csv(io.StringIO(data), header=header)
-    return df
-
-
-def extract_item_from_response(response: requests.Response, name: str) -> any:
-    """
-    Extract CSV from response
-    """
-    body = response.json()  # Get the body of the response as a dictionary
-    item = body[name]  # Get the entry corresponding to the field name
-    return item
-
-
-def print_response_headers(r: requests.Response) -> None:
-    """
-    Print response headers
-    """
-    print("Response headers:")
-    pprint(dict(r.headers))
-    # print()
-
-
-def print_response_message(r: requests.Response) -> None:
-    """
-    Print response message
-    """
-    response_text = r.text
-    try:
-        response_dict = json.loads(response_text)
-        message = response_dict["message"]
-    except:
-        message = response_text
-    print("Response:", message)
-    # print()
-
-
-def check_response(r: requests.Response) -> None:
-    if r.status_code != 200:
-        print("Status code:", r.status_code)
-        print_response_message(r)
-        raise RuntimeError("Response error")
 
 ### ###
```

