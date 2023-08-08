# Comparing `tmp/cloudflare_gateway_adblocking-0.1.0.tar.gz` & `tmp/cloudflare_gateway_adblocking-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_gateway_adblocking-0.1.0.tar", max compression
+gzip compressed data, was "cloudflare_gateway_adblocking-0.1.1.tar", max compression
```

## Comparing `cloudflare_gateway_adblocking-0.1.0.tar` & `cloudflare_gateway_adblocking-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-08-06 22:34:07.954833 cloudflare_gateway_adblocking-0.1.0/LICENSE
--rw-r--r--   0        0        0     2586 2023-08-06 22:34:38.416593 cloudflare_gateway_adblocking-0.1.0/README.md
--rw-r--r--   0        0        0      766 2023-08-06 22:34:38.418182 cloudflare_gateway_adblocking-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-06 22:34:38.418364 cloudflare_gateway_adblocking-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     4373 2023-08-06 22:34:38.418694 cloudflare_gateway_adblocking-0.1.0/src/__main__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:34:38.418805 cloudflare_gateway_adblocking-0.1.0/src/utils/__init__.py
--rw-r--r--   0        0        0     2000 2023-08-06 22:34:38.419037 cloudflare_gateway_adblocking-0.1.0/src/utils/delete.py
--rw-r--r--   0        0        0     3923 2023-08-06 22:36:21.968262 cloudflare_gateway_adblocking-0.1.0/src/utils/upload.py
--rw-r--r--   0        0        0     3814 2023-08-06 22:34:38.419606 cloudflare_gateway_adblocking-0.1.0/src/utils/utils.py
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 cloudflare_gateway_adblocking-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2624 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/README.md
+-rw-r--r--   0        0        0      784 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     4765 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/src/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/src/utils/__init__.py
+-rw-r--r--   0        0        0     2229 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/src/utils/delete.py
+-rw-r--r--   0        0        0     4100 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/src/utils/upload.py
+-rw-r--r--   0        0        0     3710 2023-08-08 20:26:22.773980 cloudflare_gateway_adblocking-0.1.1/src/utils/utils.py
+-rw-r--r--   0        0        0     3498 1970-01-01 00:00:00.000000 cloudflare_gateway_adblocking-0.1.1/PKG-INFO
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/LICENSE` & `cloudflare_gateway_adblocking-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_gateway_adblocking-0.1.0/README.md` & `cloudflare_gateway_adblocking-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 Serverless adblocking via Cloudflare Zero Trust Gateway  
 
 ### What is this?  
 This is a serverless adblocking solution that uses Cloudflare's Zero Trust Gateway to block ads by parsing a hosts file and creating a firewall rule to block the domains. It can be used as an alternative to Pi-Hole or other adblocking solutions.  
 This project was heavily inspired by [this blog post](https://blog.marcolancini.it/2022/blog-serverless-ad-blocking-with-cloudflare-gateway/)  
 
 
-### Pre-requisites
+### Prerequisites
 * Python > 3.10  
 * A Cloudflare account with Zero Trust enabled  
 * A Cloudflare API tolken with the following permissions:  
     * Zero Trust: Edit  
     * Account Firewall Access Rules: Edit  
     * Access: Apps and Policies: Edit  
 * A device with the WARP client installed and configured to use a Zero Trust account  
 
-<!-- 
+
 ### Installation  
 #### From PyPi  
-`pip install cloudflare-gateway-adblocking`
- -->
+`pip install cloudflare-gateway-adblocking`  
+
 
 ### Usage   
 #### Setting Cloudflare credentials  
 ##### Environment variables  
 The following environment variables can be used to set the Cloudflare credentials:  
 * `CLOUDFLARE_ACCOUNT_ID`
 * `CLOUDFLARE_TOKEN`  
@@ -39,8 +39,10 @@
 #### Uploading blocklists and creating a firewall policy
 To upload the blocklists to Cloudflare and create a firewall policy, use the `upload` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking upload`  
 #### Deleting blocklists and firewall policy  
 To delete the blocklists from Cloudflare and delete the firewall policy, use the `delete` subcommand.  
 For example:  
-`cloudflare-gateway-adblocking delete`  
+`cloudflare-gateway-adblocking delete`  
+### Help  
+For help, use the `--help` flag.
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/pyproject.toml` & `cloudflare_gateway_adblocking-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloudflare-gateway-adblocking"
-version = "0.1.0"
+version = "0.1.1"
 description = "Serverless adblocking via Cloudflare Zero Trust Gateway"
 authors = ["slastechno <77907286+slashtechno@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/slashtechno/cloudflare-gateway-adblocking"
 keywords = ["cloudflare", "dns", "adblocking", "serverless"]
 
@@ -14,14 +14,15 @@
 cloudflare-gateway-adblocking = "src.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 loguru = "^0.7.0"
 python-dotenv = "^1.0.0"
+httpx = "^0.24.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.281"
 black = "^23.7.0"
 
 [build-system]
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/src/__main__.py` & `cloudflare_gateway_adblocking-0.1.1/src/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 # To run from the root project directory, run the following command:
 # python -m src.__main__
 # python -m src # also works because __main__ is the default module
 import argparse
+import asyncio
 import os
 from pathlib import Path
 from sys import exit, stderr
 
 import dotenv
 from loguru import logger
 
 from .utils import delete, upload, utils
 
 TOKEN = None
 ACCOUNT_ID = None
 
 
 def main():
-    # Setup logging
-    logger.remove()
-    # ^10 is a formatting directive to center with a padding of 10
-    logger_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</green> |<level>{level: ^10}</level>| <level>{message}</level>"  # noqa E501
-    logger.add(stderr, format=logger_format, colorize=True, level="DEBUG")
-
-    # Load .env if it exists
-    # This must precede the argparse setup as env variables are used as default values
-    if Path(".env").is_file():
-        dotenv.load_dotenv()
-        logger.info("Loaded .env file")
-    else:
-        logger.info("No .env file found")
-
     # Parse arguments
 
     # Set up argparse
     argparser = argparse.ArgumentParser(
         prog="Cloudflare Gateway Adblocking",
         description="Serverless adblocking via Cloudflare Zero Trust Gateway",
         epilog=":)",
     )
 
     # Add argument groups
     credential_args = argparser.add_argument_group("Cloudflare Credentials")
 
     # Add arguments
+
+    # General arguments
+    argparser.add_argument(
+        "--log-level", "-l", help="Log level", default="INFO"
+    )  # noqa E501
+
+    # Credential arguments
     credential_args.add_argument(
         "--account-id",
         "-a",
         help="Cloudflare account ID - environment variable: CLOUDFLARE_ACCOUNT_ID",
-        default=os.environ.get("CLOUDFLARE_ACCOUNT_ID"),
     )
     credential_args.add_argument(
         "--token",
         "-t",
         help="Cloudflare API token - environment variable: CLOUDFLARE_TOKEN",
-        default=os.environ.get("CLOUDFLARE_TOKEN"),
     )
 
     # Add subcommands
     subparsers = argparser.add_subparsers(
         title="subcommands",
         description="",
         help="Subcommands to preform operations",
@@ -74,60 +66,81 @@
         help="Either a blocklist hosts file or a directory containing blocklist hosts files",  # noqa E501
         default="blocklists",  # Not really needed because the get_blocklists function will default to this  # noqa: E501
     )
     upload_parser.add_argument(
         "--whitelists",
         "-w",
         help="Either a whitelist hosts file or a directory containing whitelist hosts files",  # noqa E501
-        default="whitelist.txt",  # Not really needed because the apply_whitelists function will default to this  # noqa: E501
+        default="whitelists",  # Not really needed because the apply_whitelists function will default to this  # noqa: E501
     )
     # Add subcommand: delete
     delete_parser = subparsers.add_parser(
         "delete", help="Delete adblock lists from Cloudflare"
     )
     delete_parser.set_defaults(func=delete_from_cloudflare)
 
     args = argparser.parse_args()
 
+    # Set up logging
+    set_primary_logger(args.log_level)
     logger.debug(args)
 
     # Load variables
     global TOKEN
     global ACCOUNT_ID
     TOKEN = args.token
     ACCOUNT_ID = args.account_id
-    # Check if variables are set
+
+    # Check if credentials are set, if they are not, attempt to load from environment variables and .env  # noqa E501
     if TOKEN is None or ACCOUNT_ID is None:
-        logger.error(
-            "No environment variables found. Please create a .env file or .envrc file"
-        )  # noqa E501
-        exit(1)
+        logger.info("No credentials provided with flags")
+        if Path(".env").is_file():
+            logger.debug("Loading .env")
+            dotenv.load_dotenv()
+        else:
+            logger.debug("No .env file found")
+        try:
+            TOKEN = os.environ["CLOUDFLARE_TOKEN"]
+            ACCOUNT_ID = os.environ["CLOUDFLARE_ACCOUNT_ID"]
+            logger.info("Loaded credentials from environment variables")
+        except KeyError:
+            logger.error("No credentials provided")
+            argparser.print_help()
+            exit(1)
+
     try:
         args.func(args)
-    except AttributeError as e:
+    except AttributeError:
         logger.error("No subcommand specified")
         argparser.print_help()
         exit(1)
 
 
 def upload_to_cloudflare(args):
     logger.info("Uploading to Cloudflare")
     blocklists = upload.get_blocklists(args.blocklists)
     blocklists = upload.apply_whitelists(blocklists, args.whitelists)
     lists = upload.split_list(blocklists)
-    upload.upload_to_cloudflare(lists, ACCOUNT_ID, TOKEN)
+    asyncio.run(upload.upload_to_cloudflare(lists, ACCOUNT_ID, TOKEN))
     cloud_lists = utils.get_lists(ACCOUNT_ID, TOKEN)
     cloud_lists = utils.filter_adblock_lists(cloud_lists)
     upload.create_dns_policy(cloud_lists, ACCOUNT_ID, TOKEN)
 
 
 def delete_from_cloudflare(args):
     logger.info("Deleting from Cloudflare")
     rules = utils.get_gateway_rules(ACCOUNT_ID, TOKEN)
     delete.delete_adblock_policy(rules, ACCOUNT_ID, TOKEN)
     lists = utils.get_lists(ACCOUNT_ID, TOKEN)
     lists = utils.filter_adblock_lists(lists)
-    delete.delete_adblock_list(lists, ACCOUNT_ID, TOKEN)
+    asyncio.run(delete.delete_adblock_list(lists, ACCOUNT_ID, TOKEN))
+
+
+def set_primary_logger(log_level):
+    logger.remove()
+    # ^10 is a formatting directive to center with a padding of 10
+    logger_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</green> |<level>{level: ^10}</level>| <level>{message}</level>"  # noqa E501
+    logger.add(stderr, format=logger_format, colorize=True, level=log_level)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/src/utils/delete.py` & `cloudflare_gateway_adblocking-0.1.1/src/utils/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This is a scriprt to undo the changes made by adblock-zerotrust.py
 
+import asyncio
+
+import httpx
 import requests
 
 from . import utils
 
 
-def delete_adblock_list(lists: dict, account_id: str, token: str):
+async def delete_adblock_list(lists: dict, account_id: str, token: str):
     try:
-        for lst in lists:
-            url = f'https://api.cloudflare.com/client/v4/accounts/{account_id}/gateway/lists/{lst["id"]}'
-            headers = {
-                "Authorization": f"Bearer {token}",
-                "Content-Type": "application/json",
-            }
-            response = requests.delete(url, headers=headers, timeout=10)
-            if response.status_code != 200:
-                print(f"Error deleting list: {response.text}")
-            else:
-                print(f'Deleted list {lst["name"]}')
+        async with httpx.AsyncClient() as client:
+            for lst in lists:
+                url = f'https://api.cloudflare.com/client/v4/accounts/{account_id}/gateway/lists/{lst["id"]}'
+                headers = {
+                    "Authorization": f"Bearer {token}",
+                    "Content-Type": "application/json",
+                }
+                # response = requests.delete(url, headers=headers, timeout=10)
+                response = await client.delete(url, headers=headers, timeout=10)
+                if response.status_code != 200:
+                    print(f"Error deleting list: {response.text}")
+                else:
+                    print(f'Deleted list {lst["name"]}')
     except TypeError as e:
         if str(e) == "'NoneType' object is not iterable":
             print("No lists found")
         else:
             raise e
 
 
@@ -44,15 +49,15 @@
 
 
 def main():
     account_id = input("Enter your Cloudflare account ID: ")
     token = input("Enter your Cloudflare API token: ")
 
     rules = utils.get_gateway_rules(account_id, token)
-    delete_adblock_policy(rules, account_id, token)
+    asyncio.run(utils.delete_adblock_list(rules, account_id, token))
     lists = utils.get_lists(account_id, token)
     lists = utils.filter_adblock_lists(lists)
     delete_adblock_list(lists, account_id, token)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/src/utils/upload.py` & `cloudflare_gateway_adblocking-0.1.1/src/utils/upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import asyncio
 import pathlib
 
+import httpx
 import requests
 
 from . import utils
 
 
 def get_blocklists(hosts_path: str = "blocklists"):
     blocklists = []
@@ -42,41 +44,41 @@
     )  # This is the same as the for loop below
     # for i in range(0, len(blocklists), 1000):
     # This continues to append lists of 1000 items to the lists list via slicing
     #     lists.append(blocklists[i:i + 1000])
     return lists
 
 
-def upload_to_cloudflare(lists, account_id: str, token: str) -> None:
-    for i, lst in enumerate(lists):
-        list_name = f"adblock-list-{i + 1}"
-        url = (
-            f"https://api.cloudflare.com/client/v4/accounts/{account_id}/gateway/lists"
-        )
-        headers = {
-            "Authorization": f"Bearer {token}",
-            "Content-Type": "application/json",
-        }
-
-        data = {
-            "name": list_name,
-            "type": "DOMAIN",
-            "description": "A blocklist of ad domains",
-            # Writing this program, I have noticed how powerful list comprehension is.
-            "items": [
-                {
-                    "value": x,
-                }
-                for x in lst
-            ],
-        }
-        response = requests.post(url, headers=headers, json=data, timeout=10)
-        print(f"Uploaded {list_name} to Cloudflare")
-        if response.status_code != 200:
-            print(f"Error uploading {list_name}: {response.text}")
+async def upload_to_cloudflare(lists, account_id: str, token: str) -> None:
+    async with httpx.AsyncClient() as client:
+        for i, lst in enumerate(lists):
+            list_name = f"adblock-list-{i + 1}"
+            url = f"https://api.cloudflare.com/client/v4/accounts/{account_id}/gateway/lists"
+            headers = {
+                "Authorization": f"Bearer {token}",
+                "Content-Type": "application/json",
+            }
+
+            data = {
+                "name": list_name,
+                "type": "DOMAIN",
+                "description": "A blocklist of ad domains",
+                # Writing this program, I have noticed how powerful list comprehension is.
+                "items": [
+                    {
+                        "value": x,
+                    }
+                    for x in lst
+                ],
+            }
+            response = await client.post(url, headers=headers, json=data)
+            print(f"Uploaded {list_name} to Cloudflare")
+            if response.status_code != 200:
+                print(f"Error uploading {list_name}: {response.text}")
+                exit(1)
 
 
 def create_dns_policy(lists, account_id: str, token: str) -> None:
     url = f"https://api.cloudflare.com/client/v4/accounts/{account_id}/gateway/rules"
     headers = {
         "Authorization": f"Bearer {token}",
         "Content-Type": "application/json",
@@ -104,15 +106,15 @@
 def main():
     account_id = input("Enter your Cloudflare account ID: ")
     token = input("Enter your Cloudflare API token: ")
 
     blocklists = get_blocklists()
     blocklists = apply_whitelists(blocklists)
     lists = split_list(blocklists)
-    upload_to_cloudflare(lists, account_id, token)
+    asyncio.run(upload_to_cloudflare(lists, account_id, token))
     cloud_lists = utils.get_lists(account_id, token)
     cloud_lists = utils.filter_adblock_lists(cloud_lists)
     create_dns_policy(cloud_lists, account_id, token)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/src/utils/utils.py` & `cloudflare_gateway_adblocking-0.1.1/src/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,38 @@
     def token(self):
         return self._token
 
     @token.setter
     def token(self, token):
         if token is None:
             raise ValueError("No token provided")
-        else:
-            url = "https://api.cloudflare.com/client/v4/user/tokens/verify"
-            headers = {
-                "Authorization": f"Bearer {token}",
-                "Content-Type": "application/json",
-            }
-            response = requests.get(url, headers=headers, timeout=10)
-            if response.json()["success"] is False:
-                raise ValueError("Invalid token")
-            else:
-                # Token needs the following scopes:
-                # Zero Trust: Read/Edit
-                # Account Firewall Access Rules: Read/Edit
-                # Access Apps and Policies: Read/Edit
-                self._token = token
+        url = "https://api.cloudflare.com/client/v4/user/tokens/verify"
+        headers = {
+            "Authorization": f"Bearer {token}",
+            "Content-Type": "application/json",
+        }
+        response = requests.get(url, headers=headers, timeout=10)
+        if response.json()["success"] is False:
+            raise ValueError("Invalid token")
+        # Token needs the following scopes:
+        # Zero Trust: Read/Edit
+        # Account Firewall Access Rules: Read/Edit
+        # Access Apps and Policies: Read/Edit
+        self._token = token
 
     @property
     def account_id(self):
         return self._account_id
 
     @account_id.setter
     def account_id(self, account_id):
         if account_id is None:
             raise ValueError("No account ID provided")
-        else:
-            # Possibly make a request to lists to check if the account ID exists
-            self._account_id = account_id
+        # Possibly make a request to lists to check if the account ID exists
+        self._account_id = account_id
 
 
 # List Utils
 
 
 # Convert a hosts file to a simple hostname list
 def convert_to_list(file: pathlib.Path) -> list:
@@ -66,26 +63,26 @@
             "ip6-localhost",
             "ip6-loopback",
             "ip6-localnet",
             "ip6-mcastprefix",
             "ip6-allnodes",
             "ip6-allrouters",
             "ip6-allhosts",
-            "0.0.0.0",
+            "0.0.0.0",  # skipcq: BAN-B104
         ]
         matches = [
             re.search(r"^(?:127\.0\.0\.1|0\.0\.0\.0|::1)\s+(.+?)(?:\s+#.+)?$", line)
             for line in f
         ]
         hosts = [
             match.group(1)
             for match in matches
             if match and match.group(1) not in loopback
         ]
-        print(f"First 5 hosts: {hosts[:5]}")
+        # print(f"First 5 hosts: {hosts[:5]}")
         return hosts
 
 
 # General Utils
 
 
 def get_lists(account_id, token) -> dict:
```

### Comparing `cloudflare_gateway_adblocking-0.1.0/PKG-INFO` & `cloudflare_gateway_adblocking-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: cloudflare-gateway-adblocking
-Version: 0.1.0
+Version: 0.1.1
 Summary: Serverless adblocking via Cloudflare Zero Trust Gateway
 Home-page: https://github.com/slashtechno/cloudflare-gateway-adblocking
 License: MIT
 Keywords: cloudflare,dns,adblocking,serverless
 Author: slastechno
 Author-email: 77907286+slashtechno@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/slashtechno/cloudflare-gateway-adblocking
 Description-Content-Type: text/markdown
 
 # Cloudflare Gateway Adblocking  
 Serverless adblocking via Cloudflare Zero Trust Gateway  
 
 ### What is this?  
 This is a serverless adblocking solution that uses Cloudflare's Zero Trust Gateway to block ads by parsing a hosts file and creating a firewall rule to block the domains. It can be used as an alternative to Pi-Hole or other adblocking solutions.  
 This project was heavily inspired by [this blog post](https://blog.marcolancini.it/2022/blog-serverless-ad-blocking-with-cloudflare-gateway/)  
 
 
-### Pre-requisites
+### Prerequisites
 * Python > 3.10  
 * A Cloudflare account with Zero Trust enabled  
 * A Cloudflare API tolken with the following permissions:  
     * Zero Trust: Edit  
     * Account Firewall Access Rules: Edit  
     * Access: Apps and Policies: Edit  
 * A device with the WARP client installed and configured to use a Zero Trust account  
 
-<!-- 
+
 ### Installation  
 #### From PyPi  
-`pip install cloudflare-gateway-adblocking`
- -->
+`pip install cloudflare-gateway-adblocking`  
+
 
 ### Usage   
 #### Setting Cloudflare credentials  
 ##### Environment variables  
 The following environment variables can be used to set the Cloudflare credentials:  
 * `CLOUDFLARE_ACCOUNT_ID`
 * `CLOUDFLARE_TOKEN`  
@@ -60,7 +61,9 @@
 To upload the blocklists to Cloudflare and create a firewall policy, use the `upload` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking upload`  
 #### Deleting blocklists and firewall policy  
 To delete the blocklists from Cloudflare and delete the firewall policy, use the `delete` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking delete`  
+### Help  
+For help, use the `--help` flag.
```

