# Comparing `tmp/qcloud_setup-1.0.5.tar.gz` & `tmp/qcloud_setup-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_setup-1.0.5.tar", last modified: Fri Jul 28 08:54:35 2023, max compression
+gzip compressed data, was "qcloud_setup-1.0.6.tar", last modified: Tue Aug  8 20:55:32 2023, max compression
```

## Comparing `qcloud_setup-1.0.5.tar` & `qcloud_setup-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-28 08:54:35.589516 qcloud_setup-1.0.5/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.5/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)    16593 2023-07-28 08:54:35.589341 qcloud_setup-1.0.5/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)    15566 2023-07-17 03:57:00.000000 qcloud_setup-1.0.5/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      747 2023-07-28 08:54:20.000000 qcloud_setup-1.0.5/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-28 08:54:35.586929 qcloud_setup-1.0.5/qcloud_setup.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)    16593 2023-07-28 08:54:35.000000 qcloud_setup-1.0.5/qcloud_setup.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      422 2023-07-28 08:54:35.000000 qcloud_setup-1.0.5/qcloud_setup.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-28 08:54:35.000000 qcloud_setup-1.0.5/qcloud_setup.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       51 2023-07-28 08:54:35.000000 qcloud_setup-1.0.5/qcloud_setup.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      151 2023-07-28 08:54:35.000000 qcloud_setup-1.0.5/qcloud_setup.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       13 2023-07-28 08:54:35.000000 qcloud_setup-1.0.5/qcloud_setup.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-28 08:54:35.589557 qcloud_setup-1.0.5/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      914 2023-07-28 08:54:29.000000 qcloud_setup-1.0.5/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-28 08:54:35.585621 qcloud_setup-1.0.5/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-28 08:54:35.588579 qcloud_setup-1.0.5/src/qcloud_setup/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.5/src/qcloud_setup/__init__.py
--rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.5/src/qcloud_setup/api-gateway.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.5/src/qcloud_setup/cognito.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     5829 2023-07-25 11:18:10.000000 qcloud_setup-1.0.5/src/qcloud_setup/iam-policy.yaml
--rwxr-x---   0 agilbert   (501) staff       (20)    59621 2023-07-28 06:50:49.000000 qcloud_setup-1.0.5/src/qcloud_setup/qcloud_admin.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:55:32.377032 qcloud_setup-1.0.6/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.6/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)    16593 2023-08-08 20:55:32.376819 qcloud_setup-1.0.6/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)    15566 2023-07-17 03:57:00.000000 qcloud_setup-1.0.6/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      747 2023-08-08 20:54:55.000000 qcloud_setup-1.0.6/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:55:32.375128 qcloud_setup-1.0.6/qcloud_setup.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)    16593 2023-08-08 20:55:32.000000 qcloud_setup-1.0.6/qcloud_setup.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      422 2023-08-08 20:55:32.000000 qcloud_setup-1.0.6/qcloud_setup.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-08-08 20:55:32.000000 qcloud_setup-1.0.6/qcloud_setup.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       51 2023-08-08 20:55:32.000000 qcloud_setup-1.0.6/qcloud_setup.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      151 2023-08-08 20:55:32.000000 qcloud_setup-1.0.6/qcloud_setup.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       13 2023-08-08 20:55:32.000000 qcloud_setup-1.0.6/qcloud_setup.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-08-08 20:55:32.377074 qcloud_setup-1.0.6/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      914 2023-08-08 20:55:14.000000 qcloud_setup-1.0.6/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:55:32.373772 qcloud_setup-1.0.6/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:55:32.376551 qcloud_setup-1.0.6/src/qcloud_setup/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.6/src/qcloud_setup/__init__.py
+-rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.6/src/qcloud_setup/api-gateway.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.6/src/qcloud_setup/cognito.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     5829 2023-07-25 11:18:10.000000 qcloud_setup-1.0.6/src/qcloud_setup/iam-policy.yaml
+-rwxr-x---   0 agilbert   (501) staff       (20)    60837 2023-08-08 11:52:56.000000 qcloud_setup-1.0.6/src/qcloud_setup/qcloud_admin.py
```

### Comparing `qcloud_setup-1.0.5/LICENSE.txt` & `qcloud_setup-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.5/PKG-INFO` & `qcloud_setup-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_setup
-Version: 1.0.5
+Version: 1.0.6
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_setup-1.0.5/README.md` & `qcloud_setup-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.5/pyproject.toml` & `qcloud_setup-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_setup"
-version = "1.0.5"
+version = "1.0.6"
 description = "Q-Cloud setup utility for cluster administrators" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_setup-1.0.5/qcloud_setup.egg-info/PKG-INFO` & `qcloud_setup-1.0.6/qcloud_setup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-setup
-Version: 1.0.5
+Version: 1.0.6
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_setup-1.0.5/setup.py` & `qcloud_setup-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="qcloud_setup",
     python_requires='>=3.7',
-    version="1.0.5",
+    version="1.0.6",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="support@q-chem.com",
     description="Utility for setting up Q-Cloud administrators",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(where="src"),
```

### Comparing `qcloud_setup-1.0.5/src/qcloud_setup/api-gateway.yaml` & `qcloud_setup-1.0.6/src/qcloud_setup/api-gateway.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.5/src/qcloud_setup/cognito.yaml` & `qcloud_setup-1.0.6/src/qcloud_setup/cognito.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.5/src/qcloud_setup/iam-policy.yaml` & `qcloud_setup-1.0.6/src/qcloud_setup/iam-policy.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.5/src/qcloud_setup/qcloud_admin.py` & `qcloud_setup-1.0.6/src/qcloud_setup/qcloud_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from pprint import pprint
 from datetime import datetime, timedelta
 from collections import defaultdict, OrderedDict
 
 import importlib.resources 
 
 
-SOURCE_SNAPSHOT = "snap-07e1149ce851713a8"
+SOURCE_SNAPSHOT = "snap-06e211970f197afe9"
 SOURCE_REGION   = "us-east-1"
 VERSION         = "v6.1.0"
 
 DEBUG = False
 
 
 def debug(s):
@@ -253,28 +253,30 @@
     session = None
 
     try:
        region = config.get("AWS", "region")
        access_key = config.get("AWS", "aws_access_key_id")
        secret_key = config.get("AWS", "aws_secret_access_key")
 
+       access_masked =  '*'*12 + access_key[12:]
+       secret_masked =  '*'*32 + secret_key[32:]
        debug("Using session details:")
-       debug("  aws_access_key_id:     {}".format(access_key))
-       debug("  aws_secret_access_key: {}".format(secret_key))
+       debug("  aws_access_key_id:     {}".format(access_masked))
+       debug("  aws_secret_access_key: {}".format(secret_masked))
        debug("  region name:           {}".format(region))
 
 
        session = boto3.Session(
           aws_access_key_id = access_key, 
           aws_secret_access_key = secret_key,
           region_name = region )
 
        os.environ["AWS_DEFAULT_REGION"] = region
-       os.environ["AWS_ACCESS_KEY_ID"] = access_key
-       os.environ["AWS_SECRET_ACCESS_KEY"] = secret_key
+       #os.environ["AWS_ACCESS_KEY_ID"] = access_key
+       #os.environ["AWS_SECRET_ACCESS_KEY"] = secret_key
 
     except (botocore.exceptions.ClientError,
             botocore.exceptions.NoCredentialsError):
        raise QCloudError(mesg)
 
     return session
     
@@ -1279,27 +1281,31 @@
 
 def update_config_file(stack_name, api_bucket_name, execute_policy_arn):
     config = ConfigFile(stack_name)
     fname  = config.fname()
     
     with open(fname) as file:
          text = file.read()
-         text = text.replace('API_BUCKET_NAME', api_bucket_name)
-         text = text.replace('EXECUTE_POLICY_ARN', execute_policy_arn)
+
+    text = re.sub("BucketName:.+", "BucketName: {}".format(api_bucket_name), text)
+    text = re.sub("- Policy:.+", "- Policy: {}".format(execute_policy_arn), text)
+
     with open(fname, "w") as file:
          file.write(text)
 
 
 
 
 
 ###############################################################################################
 
 
 def add_user(session, name, username, email):
+    if not email:
+       raise QCloudError("Must specify email address with --email option")
     users = { username: email}
     create_users(session, name, users)
 
 
 
 def add_users(session, name, users_file):
     if not os.path.exists(users_file):
@@ -1610,15 +1616,15 @@
         groupNames.append(s[0])
 
     return groupNames
 
 
 
 def print_logs(session, name, log_duration):
-    client = boto3.client('logs')
+    client = session.client('logs')
 
     now = int(1000*datetime.now().timestamp()) 
     start_time = 0
     log_duration = int(log_duration)
 
     if log_duration == 0:
        start_time = 0
@@ -1635,15 +1641,14 @@
         while 'nextToken' in stream_batch:
             stream_batch = client.describe_log_streams(
                 logGroupName = group,
                 nextToken = stream_batch['nextToken']
             )
             all_streams += stream_batch['logStreams']
 
-
         stream_names = [ stream['logStreamName'] for stream in all_streams]
 
         fname = group + "_" + str(time()) + "_log.txt"
         checklist("Downloading logs for group", group)
         fname = fname.replace('/','_')
         out_file = open(fname, 'w')
         for stream in stream_names:
@@ -1668,14 +1673,46 @@
                         event.update({'group': group_name, 'stream':stream })
                         out_file.write(json.dumps(event) + '\n')
 
         checklist("Logs downloaded to", fname, True)
 
 
 
+def debug_api(session, name):
+    client = session.client("apigateway")
+    api_stack = "{}-api-gateway".format(name)
+    api_gatewayId = get_resource_id(session, api_stack, 'ApiGatewayRestApi')
+    print("{0: <24} {1}".format('ApiGateway ID', api_gatewayId))
+
+    response = client.get_deployments(
+       restApiId = api_gatewayId
+    )
+
+    for item in response["items"]:
+        print("{0: <24} {1}   {2}".format("Deployment ID", item["id"], item["createdDate"]))
+
+    response = client.get_authorizers(
+       restApiId = api_gatewayId
+    )
+
+    for item in response["items"]:
+        print("{0: <24} {1} ".format("Authorizer ID", item["id"]))
+        print("{0: <24} {1} ".format("Authorizer Name", item["name"]))
+        print("{0: <24} {1} ".format("Authorizer Type", item["type"]))
+        print("{0: <24} {1} ".format("Authorizer Provider", item["providerARNs"]))
+        print("{0: <24} {1} ".format("Authorizer Source", item["identitySource"]))
+
+    client = session.client('cognito-idp')
+
+    
+
+
+    
+
+
 ###############################################################################################
 
 
 def main():
     try: 
         parser = MyParser();
 
@@ -1775,18 +1812,16 @@
 
         if len(sys.argv)==1:
            parser.print_help(sys.stderr)
            sys.exit(1)
 
         if args.config:
             configure_cluster(session, name, interactive)
-            if args.launch:
-               launch(session, name, args.nocognito, args.email)
 
-        elif args.launch:
+        if args.launch:
             launch(session, name, args.nocognito, args.email)
             if args.license_key:
                install_license_key(session, name, args.license_key)
 
         elif args.status:
             print_all_stack_status(session, name)
 
@@ -1828,14 +1863,17 @@
 
         elif args.logs:
             print_logs(session, name, args.log_duration)
 
         elif args.list:
             list_stacks(session)
 
+        elif args.debug:
+            debug_api(session, name)
+
         else:
            print("ERROR: Invalid option specified")
            parser.print_help(sys.stderr)
             
 
 
     except KeyboardInterrupt:
```

