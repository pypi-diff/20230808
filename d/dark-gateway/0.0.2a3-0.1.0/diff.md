# Comparing `tmp/dark-gateway-0.0.2a3.tar.gz` & `tmp/dark-gateway-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark-gateway-0.0.2a3.tar", last modified: Sat Jul  8 15:47:39 2023, max compression
+gzip compressed data, was "dark-gateway-0.1.0.tar", last modified: Tue Aug  8 18:34:39 2023, max compression
```

## Comparing `dark-gateway-0.0.2a3.tar` & `dark-gateway-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/dark/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/dark/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/gateway/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/pid_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/dark/util/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/util/core_bc_libs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/util/libs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-08 15:47:36.000000 dark-gateway-0.0.2a3/dark/util/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/dark_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-08 15:47:39.000000 dark-gateway-0.0.2a3/dark_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-08 15:47:39.000000 dark-gateway-0.0.2a3/dark_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:47:39.000000 dark-gateway-0.0.2a3/dark_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 15:47:39.000000 dark-gateway-0.0.2a3/dark_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:47:39.812218 dark-gateway-0.0.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-08 15:47:39.000000 dark-gateway-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/dark/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/gateway/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/pid_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/dark/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/util/core_bc_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/util/libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-08-08 18:34:33.000000 dark-gateway-0.1.0/dark/util/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/dark_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-08 18:34:39.000000 dark-gateway-0.1.0/dark_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 18:34:39.000000 dark-gateway-0.1.0/dark_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:34:39.000000 dark-gateway-0.1.0/dark_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 18:34:39.000000 dark-gateway-0.1.0/dark_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:34:39.724123 dark-gateway-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-08 18:34:38.000000 dark-gateway-0.1.0/setup.py
```

### Comparing `dark-gateway-0.0.2a3/LICENSE` & `dark-gateway-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.2a3/dark/pid_modules.py` & `dark-gateway-0.1.0/dark/pid_modules.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from web3 import Web3
+from hexbytes.main import HexBytes
 # from web3._utils.datatypes import Contract
 
 class DarkPid:
 
-    def __init__(self,pid_hash,ark_id,externa_pid_list,payload,owner) -> None:
-        self.pid_hash = pid_hash
+    def __init__(self,pid_hash,ark_id,externa_pid_list,externa_url_list,payload,owner) -> None:
+        
+        if type(pid_hash) == HexBytes:
+            self.pid_hash = pid_hash
+        else:
+            self.pid_hash = HexBytes(pid_hash)
+
         self.ark = ark_id
         self.externa_pid_list = externa_pid_list
+        self.externa_url = externa_url_list
         self.payload = payload
         self.responsible = owner
-    
+
     def to_dict(self):
         """
         Converts the attributes of the class object into a dictionary.
 
         Returns:
             dict: A dictionary representation of the class object's attributes.
         """
@@ -26,70 +33,77 @@
         Parameters:
             output (tuple): The output to be validated.
 
         Returns:
             bool: True if the output is valid, False otherwise.
         """
 
-        if len(bc_output) != 10:
+        if len(bc_output) != 6:
             return False
 
         if not isinstance(bc_output[0], bytes) or not isinstance(bc_output[1], str):
             return False
 
-        if not isinstance(bc_output[2], list) or not isinstance(bc_output[3], list):
-            return False
-
-        if not isinstance(bc_output[4], int) or not isinstance(bc_output[5], list):
+        if not isinstance(bc_output[2], list) or not isinstance(bc_output[3], bytes):
             return False
 
-        if not isinstance(bc_output[6], int) or not isinstance(bc_output[7], tuple):
-            return False
-
-        if not isinstance(bc_output[8], str) or not isinstance(bc_output[9], str):
+        if not isinstance(bc_output[4], str):
             return False
 
         return True
 
 
-    def populateDark(dark_object,epid_db_contract):
+    def populateDark(dark_object,epid_db_contract,url_db_contract):
         assert DarkPid.__is_bc_valid(dark_object) == True, "Invalid Blockchain Output"
         # TODO: VALIDADE epid_db_contract
         # assert type(epid_db_contract) == Contract, "epid_db_contract must be web3._utils.datatypes.Contract type"
 
         # populate external pids
         external_pids = []
-        for ext_pid in dark_object[3]:
+        for ext_pid in dark_object[2]:
             ext_pid = Web3.toHex(ext_pid)
             # epid = epid_db.functions.get(ext_pid).call()
             get_func = epid_db_contract.get_function_by_signature('get(bytes32)')
             epid = get_func(ext_pid).call()
 
-            pid_object = {'id': ext_pid, 
-                            'schema:' : epid[3] , 'value' : epid[2], 
+            pid_object = {'hash_id': ext_pid, 
+                            'value' : epid[2], 
                             'owner:' : epid[-1]
                         }
             external_pids.append(pid_object)
         
         # deprecated
-        # external_links = []
-        # for ext_link in dark_object[5]:
-        #     external_links.append(ext_link)
+
+        zbytes32 = dark_object[3].hex().rstrip("0")
+        if len(zbytes32) % 2 != 0:
+            zbytes32 = zbytes32 + '0'
+        try:    
+            zbytes32 = bytes.fromhex(zbytes32).decode('utf8')
+            externa_url_list = ''
+        except UnicodeDecodeError:
+            get_url = url_db_contract.get_function_by_signature('get(bytes32)')
+            url_obj = get_url(Web3.toHex(dark_object[3])).call()
+            externa_url_list = url_obj[2]
+
+        # if len(zbytes32) != 0:
+        #     externa_url_list = zbytes32
+        # else:
+        #     externa_url_list = ''
+        # for ext_link in dark_object[3]:
+        #     externa_url_list.append(ext_link)
 
         pid_hash_id = Web3.toHex(dark_object[0])
         pid_ark_id = dark_object[1]
         payload = dark_object[-2]
         owner = dark_object[-1]
         
 
-        return DarkPid(pid_hash_id,pid_ark_id,external_pids,payload,owner)
+        return DarkPid(pid_hash_id,pid_ark_id,external_pids,externa_url_list,payload,owner)
 
         
-
-
 class ExeternalPid:
     def __init__(self,id_hash,schema,value,creator) -> None:
         self.id = id_hash
         self.schema = schema
         self.pid_str_value = value
         self.creator_addr = creator
```

### Comparing `dark-gateway-0.0.2a3/dark/util/core_bc_libs.py` & `dark-gateway-0.1.0/dark/util/core_bc_libs.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,8 +15,17 @@
                     signed_tx):
         
         assert type(dark_gateway) == DarkGateway, "dark_gateway must be a DarkGateway object"
 
         # signed_tx = dark_gateway.signTransaction(smart_contract,method,*args)
         tx_hash = dark_gateway.w3.eth.sendRawTransaction(signed_tx.rawTransaction)
         receipt = dark_gateway.w3.eth.wait_for_transaction_receipt(tx_hash)
-        return receipt, tx_hash
+        return receipt, tx_hash
+
+def invoke_contract_async(dark_gateway: DarkGateway,
+                    signed_tx):
+        
+        assert type(dark_gateway) == DarkGateway, "dark_gateway must be a DarkGateway object"
+
+        # signed_tx = dark_gateway.signTransaction(smart_contract,method,*args)
+        tx_hash = dark_gateway.w3.eth.sendRawTransaction(signed_tx.rawTransaction)
+        return tx_hash
```

### Comparing `dark-gateway-0.0.2a3/dark/util/libs.py` & `dark-gateway-0.1.0/dark/util/libs.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.2a3/dark/util/setup.py` & `dark-gateway-0.1.0/dark/util/setup.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.2a3/setup.py` & `dark-gateway-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 local = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(local, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 # This gets deployed when a new release is made by github actions
-VERSION = '0.0.2a3'
+VERSION = '0.1.0'
 # VERSION = '0.0.1'
 
 # CHANGEME VARS
 PACKAGE_NAME = "dark-gateway"
 DESCRIPTION = 'dARK Gateway libs'
 LONG_DESCRIPTION = 'dARK web3 libs to connect applications to the dARK'
 AUTHOR_NAME = "Thiago Nóbrega"
@@ -26,21 +26,25 @@
 
 # Read more about classifiers at https://pypi.org/classifiers/
 CLASSIFIERS = [
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
             "Operating System :: OS Independent"]
 
+EXCLUDE_LIST = [
+            'docs.*',
+]
+
 setuptools.setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author=AUTHOR_NAME,
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
     url = PROJECT_URL,
     long_description=long_description,
     long_description_content_type="text/markdown",
     # install_requires=REQUIRED_PACKAGES,
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=EXCLUDE_LIST),
     keywords=PROJECT_KEYWORDS,
     classifiers=CLASSIFIERS,
 )
```

