# Comparing `tmp/viking-log-keeper-0.3.0.tar.gz` & `tmp/viking-log-keeper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viking-log-keeper-0.3.0.tar", last modified: Thu Aug  3 21:41:29 2023, max compression
+gzip compressed data, was "viking-log-keeper-0.4.0.tar", last modified: Mon Aug  7 23:27:47 2023, max compression
```

## Comparing `viking-log-keeper-0.3.0.tar` & `viking-log-keeper-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:41:29.834356 viking-log-keeper-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-03 21:41:29.834356 viking-log-keeper-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-03 21:41:17.000000 viking-log-keeper-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 21:41:17.000000 viking-log-keeper-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:41:29.834356 viking-log-keeper-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:41:29.830356 viking-log-keeper-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:41:29.830356 viking-log-keeper-0.3.0/src/log_keeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:41:17.000000 viking-log-keeper-0.3.0/src/log_keeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-08-03 21:41:17.000000 viking-log-keeper-0.3.0/src/log_keeper/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:41:29.834356 viking-log-keeper-0.3.0/src/viking_log_keeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-03 21:41:29.000000 viking-log-keeper-0.3.0/src/viking_log_keeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 21:41:29.000000 viking-log-keeper-0.3.0/src/viking_log_keeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:41:29.000000 viking-log-keeper-0.3.0/src/viking_log_keeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 21:41:29.000000 viking-log-keeper-0.3.0/src/viking_log_keeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 21:41:29.000000 viking-log-keeper-0.3.0/src/viking_log_keeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:27:47.377712 viking-log-keeper-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 23:27:47.377712 viking-log-keeper-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-07 23:27:36.000000 viking-log-keeper-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-07 23:27:36.000000 viking-log-keeper-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 23:27:47.377712 viking-log-keeper-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:27:47.373711 viking-log-keeper-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:27:47.377712 viking-log-keeper-0.4.0/src/log_keeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:27:36.000000 viking-log-keeper-0.4.0/src/log_keeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-07 23:27:36.000000 viking-log-keeper-0.4.0/src/log_keeper/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-08-07 23:27:36.000000 viking-log-keeper-0.4.0/src/log_keeper/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:27:47.377712 viking-log-keeper-0.4.0/src/viking_log_keeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 23:27:47.000000 viking-log-keeper-0.4.0/src/viking_log_keeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-07 23:27:47.000000 viking-log-keeper-0.4.0/src/viking_log_keeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:27:47.000000 viking-log-keeper-0.4.0/src/viking_log_keeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 23:27:47.000000 viking-log-keeper-0.4.0/src/viking_log_keeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 23:27:47.000000 viking-log-keeper-0.4.0/src/viking_log_keeper.egg-info/top_level.txt
```

### Comparing `viking-log-keeper-0.3.0/pyproject.toml` & `viking-log-keeper-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "viking-log-keeper"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Michael Jennings", email="mjennings061@gmail.com" },
 ]
 description = "661 VGS - Function to collate 2965D log sheets into a master log and database."
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
@@ -16,15 +16,18 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pandas==2.0.2",
     "pymongo[srv]==4.4.1",
     "xlsxwriter==3.1.2",
-    "openpyxl==3.1.2"
+    "openpyxl==3.1.2",
+    "cryptography==41.0.3",
+    "inquirer==3.1.3",
+    "python-dotenv==1.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mjennings061/viking-log-keeper"
 "Repository" = "https://github.com/mjennings061/viking-log-keeper.git"
 
 [project.optional-dependencies]
```

### Comparing `viking-log-keeper-0.3.0/src/log_keeper/main.py` & `viking-log-keeper-0.4.0/src/log_keeper/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 """
 
 # Get packages.
 from pathlib import Path
 import pandas as pd
 import warnings
 from datetime import datetime
-import json
 from pymongo.mongo_client import MongoClient
 from pymongo.server_api import ServerApi
 
+# Get modules.
+from log_keeper.get_config import get_config, remove_config
+
 # Project constants.
 PROJECT_NAME = "viking-log-keeper"
 
 
 def ingest_log_sheet(file_path):
     """
     Extract data from an excel log sheet.
@@ -104,15 +106,14 @@
         except Exception as e:
             if file_path.name != "2965D_YYMMDD_ZEXXX.xlsx":
                 warnings.warn(f"Log sheet invalid: {file_path.name}", RuntimeWarning)
                 print(e)
 
 
     collated_df = sanitise_log_sheets(log_sheet_df)
-
     return collated_df
 
 
 def launches_to_excel(launches_df, output_file_path):
     """Save the master log dataframe to an excel table."""
 
     # Sheet the table should be inserted into.
@@ -166,39 +167,37 @@
     # Close the Pandas Excel writer and output the Excel file.
     writer.close()
 
     # Print success message.
     print(f"{PROJECT_NAME}: Saved to {output_file_path.name}")
 
 
-def launches_to_db(launches_df):
+def launches_to_db(launches_df, db_config):
     """Save the master log dataframe to a MongoDB."""
     # Get environment variables.
-    DB_CONFIG_PATH = ".config/database-config.json"
-    config_filepath = Path(__file__).resolve().parent / DB_CONFIG_PATH
-    with open(Path(DB_CONFIG_PATH).resolve(), 'r') as f:
-        DB_CONFIG = json.load(f)
-        DB_URL = DB_CONFIG["DB_URL"]
-        DB_USERNAME = DB_CONFIG["DB_USERNAME"] 
-        DB_PASSWORD = DB_CONFIG["DB_PASSWORD"]
-        DB_COLLECTION_NAME = DB_CONFIG["DB_COLLECTION_NAME"]
-        DB_NAME = DB_CONFIG["DB_NAME"]
+    DB_HOSTNAME = db_config["DB_HOSTNAME"]
+    DB_USERNAME = db_config["DB_USERNAME"]
+    DB_PASSWORD = db_config["DB_PASSWORD"]
+    DB_COLLECTION_NAME = db_config["DB_COLLECTION_NAME"]
+    DB_NAME = db_config["DB_NAME"]
 
     # Format dataframe to be saved.
     master_dict = launches_df.to_dict('records')
 
     # Create the DB connection URL
-    db_url = f"mongodb+srv://{DB_USERNAME}:{DB_PASSWORD}@{DB_URL}/?retryWrites=true&w=majority"
+    db_url = f"mongodb+srv://{DB_USERNAME}:{DB_PASSWORD}@{DB_HOSTNAME}/?retryWrites=true&w=majority"
 
     # Create a new client and connect to the server
     client = MongoClient(db_url, server_api=ServerApi('1'))
 
-    # Connect to the DB.
-    client.admin.command('ping')
-    print(f"{PROJECT_NAME}: Connected to DB.")
+    # Print success message if ping is successful.
+    if client.admin.command('ping')['ok'] == 1.0:
+        print(f"{PROJECT_NAME}: Connected to DB.")
+    else:
+        raise ConnectionError(f"{PROJECT_NAME}: Could not connect to DB.")
 
     # Get the database.
     db = client[DB_NAME]
 
     # Get all collections in the DB.
     collections = db.list_collection_names()
 
@@ -223,58 +222,81 @@
     collection.insert_many(master_dict)
     print(f"{PROJECT_NAME}: Saved to DB.")
     
     # Close DB session.
     client.close()
 
 
-def main():
-    # Initial comment.
-    print(f"{PROJECT_NAME}: Starting...")
+def find_directory(start_path, search_string):
+    """Find a directory."""
+    # Search for the directory.
+    for dir in start_path.iterdir():
+        if dir.is_dir() and search_string in dir.name:
+            return dir
+        
+    # Raise an error if the directory is not found.
+    raise FileNotFoundError("Could not find OneDrive directory.")
+
 
-    # Get the file path.
+def get_onedrive_path():
+    """Get the path to OneDrive."""
+    # Name of the onedrive directory to search for.
+    ONEDRIVE_SEARCH_STRING = "Royal Air Force Air Cadets"
+    DOCUMENTS_SEARCH_STRING = "Documents"
+    
+    # Search for the onedrive from home.
     root_dir = Path.home()
+    onedrive_path = find_directory(root_dir, ONEDRIVE_SEARCH_STRING)
 
-    # Path to the sharepoint directory.
-    SHAREPOINT_DIR = Path(
-        root_dir, 
-        "Royal Air Force Air Cadets",
-        "661 VGS - RAF Kirknewton - 661 Documents",
-    )
+    # Now get the path to the documents directory.
+    documents_path = find_directory(onedrive_path, DOCUMENTS_SEARCH_STRING)
+    return documents_path
 
-    # If the path does not exist, its probably the squadron laptop.
-    # There is definitely a better way of doing this.
-    if SHAREPOINT_DIR.exists() == False:
-        SHAREPOINT_DIR = Path(
-            root_dir, 
-            "Onedrive - Royal Air Force Air Cadets",
-            "661 Documents",
-        )
+
+def main():
+    # Initial comment.
+    print(f"{PROJECT_NAME}: Starting...")
+
+    # Get the file paths.
+    onedrive_path = get_onedrive_path()
 
     # Path to the log sheets directory.
-    LOG_SHEETS_DIR = Path(
-        SHAREPOINT_DIR, 
+    log_sheets_dir = Path(
+        onedrive_path, 
         "Log Sheets"
     )
 
     # Output file path.
-    OUTPUT_FILE = Path(
-        SHAREPOINT_DIR,
-        "Stats",
-        "MASTER-LOG.xlsx"
+    master_log_filepath = Path(
+        log_sheets_dir,
+        "Master Log.xlsx"
     )
 
     # Create a dataframe of all log sheets.
-    launches_df = collate_log_sheets(LOG_SHEETS_DIR)
+    launches_df = collate_log_sheets(log_sheets_dir)
 
     # Save the launches to excel.
-    launches_to_excel(launches_df, OUTPUT_FILE)
+    launches_to_excel(launches_df, master_log_filepath)
+
+    # Get the config filepath, or use the CLI interface to create one.
+    db_config = get_config()
 
     # Save the master log to MongoDB Atlas.
-    launches_to_db(launches_df)
+    try:
+        launches_to_db(launches_df, db_config)
+    except Exception as e:
+        # Filter a ConnectionError.
+        if isinstance(e, ConnectionError):
+            print(e)
+        else:
+            # Remove the config file and try again.
+            print(f"{PROJECT_NAME}: Could not save to DB. Try changing the config file.")
+            remove_config()
+            db_config = get_config()
+            launches_to_db(launches_df, db_config)
 
     # Print success message.
     print(f"{PROJECT_NAME}: Success!")
 
 
 if __name__ == "__main__":
     main()
```

