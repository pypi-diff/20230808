# Comparing `tmp/zscaler_api_talkers-5.0.0.tar.gz` & `tmp/zscaler_api_talkers-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_api_talkers-5.0.0.tar", max compression
+gzip compressed data, was "zscaler_api_talkers-5.0.1.tar", max compression
```

## Comparing `zscaler_api_talkers-5.0.0.tar` & `zscaler_api_talkers-5.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2022-04-21 16:27:44.526756 zscaler_api_talkers-5.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4641 2023-07-11 14:25:40.148396 zscaler_api_talkers-5.0.0/README.md
--rw-r--r--   0        0        0      455 2023-07-18 01:31:52.736800 zscaler_api_talkers-5.0.0/pyproject.toml
--rw-r--r--   0        0        0      470 2023-07-11 14:25:40.155870 zscaler_api_talkers-5.0.0/zscaler_api_talkers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:25:40.156073 zscaler_api_talkers-5.0.0/zscaler_api_talkers/client_connector/__init__.py
--rw-r--r--   0        0        0     7610 2023-07-18 01:05:14.039703 zscaler_api_talkers-5.0.0/zscaler_api_talkers/client_connector/talker.py
--rw-r--r--   0        0        0      205 2023-07-17 12:24:00.512588 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/__init__.py
--rw-r--r--   0        0        0     8821 2023-07-17 16:09:13.247599 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/http_calls.py
--rw-r--r--   0        0        0     1724 2023-07-11 14:25:40.157783 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/logger.py
--rw-r--r--   0        0        0     6482 2023-07-11 14:25:40.157979 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/utilities.py
--rw-r--r--   0        0        0        0 2023-07-11 14:25:40.158067 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zdx/__init__.py
--rw-r--r--   0        0        0    14350 2023-07-17 12:24:00.513688 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zdx/portal_talker.py
--rw-r--r--   0        0        0        0 2023-07-11 14:25:40.158774 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/__init__.py
--rw-r--r--   0        0        0     1136 2023-07-11 14:25:40.159069 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/helpers.py
--rw-r--r--   0        0        0    13788 2023-07-11 14:25:40.159489 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/models.py
--rw-r--r--   0        0        0    43204 2023-07-17 12:24:00.514405 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/portal_talker.py
--rw-r--r--   0        0        0    80884 2023-07-17 12:24:00.515262 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/talker.py
--rw-r--r--   0        0        0        0 2023-07-11 14:25:40.161421 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/__init__.py
--rw-r--r--   0        0        0    14603 2023-07-17 12:24:00.515998 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/portal_talker.py
--rw-r--r--   0        0        0    31531 2023-07-17 12:27:01.950284 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/talker.py
--rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 zscaler_api_talkers-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-21 16:27:44.526756 zscaler_api_talkers-5.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4107 2023-08-08 19:45:06.622230 zscaler_api_talkers-5.0.1/README.md
+-rw-r--r--   0        0        0      455 2023-08-08 19:44:44.184636 zscaler_api_talkers-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0      470 2023-07-11 14:25:40.155870 zscaler_api_talkers-5.0.1/zscaler_api_talkers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.156073 zscaler_api_talkers-5.0.1/zscaler_api_talkers/client_connector/__init__.py
+-rw-r--r--   0        0        0     7610 2023-07-18 01:05:14.039703 zscaler_api_talkers-5.0.1/zscaler_api_talkers/client_connector/talker.py
+-rw-r--r--   0        0        0      205 2023-07-17 12:24:00.512588 zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/__init__.py
+-rw-r--r--   0        0        0     8821 2023-07-17 16:09:13.247599 zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/http_calls.py
+-rw-r--r--   0        0        0     1724 2023-07-11 14:25:40.157783 zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/logger.py
+-rw-r--r--   0        0        0     6482 2023-07-11 14:25:40.157979 zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/utilities.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.158067 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zdx/__init__.py
+-rw-r--r--   0        0        0    14350 2023-07-17 12:24:00.513688 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zdx/portal_talker.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.158774 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-11 14:25:40.159069 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/helpers.py
+-rw-r--r--   0        0        0    13788 2023-07-11 14:25:40.159489 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/models.py
+-rw-r--r--   0        0        0    44575 2023-08-08 19:44:44.185497 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/portal_talker.py
+-rw-r--r--   0        0        0    80884 2023-07-17 12:24:00.515262 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/talker.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.161421 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zpa/__init__.py
+-rw-r--r--   0        0        0    14603 2023-07-17 12:24:00.515998 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zpa/portal_talker.py
+-rw-r--r--   0        0        0    31531 2023-07-17 12:27:01.950284 zscaler_api_talkers-5.0.1/zscaler_api_talkers/zpa/talker.py
+-rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 zscaler_api_talkers-5.0.1/PKG-INFO
```

### Comparing `zscaler_api_talkers-5.0.0/LICENSE.txt` & `zscaler_api_talkers-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/README.md` & `zscaler_api_talkers-5.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 # Unofficial Zscaler API talkers
 
 ## API Talkers
 
 ### ZIA API Talker
 Python classes to leverage [Zscaler Internet Access API](https://help.zscaler.com/zia/api)
 
-The ZIA API talker is divided into two Class objects: **ZiaTalker** and **ZiaPortalTalker**.  ZiaTalker interacts with 
-ZIA via the published APIs; whereas ZiaPortalTalker interacts with ZIA via the URLs presented in the Portal (aka, the ZIA configuration website).
-
 ### ZPA API Talker
 Python classes to leverage [Zscaler Private Access API](https://help.zscaler.com/zpa/api-reference)
 
-The ZPA API talker is divided into two Class objects: **ZpaTalker** and **ZpaPortalTalker**.  ZpaTalker interacts with 
-ZPA via the published APIs; whereas ZpaPortalTalker interacts with ZPA via the URLs presented in the Portal (aka, the ZPA configuration website).
-
 ### Client Connector API Talker
 A Python class to leverage Zscaler Client Connector API. (Currently in Beta status.)
 
 The Client Connector API talker is accessed via the Class object named: **ClientConnectorTalker**
 
 ### ZDX API Talker
 A Python class to leverage Zscaler Digital Experience API. (Currently in development.)
```

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/client_connector/talker.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/client_connector/talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/http_calls.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/http_calls.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/logger.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/utilities.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/helpers/utilities.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zdx/portal_talker.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zdx/portal_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/helpers.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/helpers.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/models.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/models.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/portal_talker.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/portal_talker.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,37 +197,43 @@
 
     def add_pac_file(
         self,
         name: str,
         description: str,
         domain: str,
         pac_content: str,
+        pac_commit_message: str,
         editable: bool = True,
         pac_url_obfuscated: bool = True,
+        pac_version_status: str = "STAGE",
+        pac_verification_status: str = "VERIFY_NOERR"
     ) -> json:
         """
         Method to Add a PAC file
-
         :param name: (str) Name of the PAC
         :param description: (str) Description
         :param domain: (str) Domain
         :param pac_content: (str) PAC content
+        :param pac_commit_message: (str) PAC commit message
         :param editable: (bool) Default True
         :param pac_url_obfuscated: (bool) Default True
-
+        :param pac_version_status: (str) Default VERIFY_NOERR
         :return: (json)
         """
         payload = {
             "name": name,
             "editable": editable,
             "pacContent": pac_content,
             "pacUrlObfuscated": pac_url_obfuscated,
             "domain": domain,
             "description": description,
-            "pacVerificationStatus": "VERIFY_NOERR",
+            "pacCommitMessage": pac_commit_message,
+            "pacVerificationStatus": pac_verification_status,
+            "pacVersionStatus":pac_version_status,
+
         }
         url = f"/pacFiles"
         response = self.hp_http.post_call(
             url=url,
             headers=self.headers,
             payload=payload,
             cookies={
@@ -1015,15 +1021,15 @@
             headers=self.headers,
             cookies={
                 "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
         )
 
-        return response.json()
+        return response
 
     def delete_web_application_rule(
         self,
         rule_id: int,
         rule_type: str,
         **kwargs,
     ) -> requests.Response:
@@ -1411,14 +1417,35 @@
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
             **kwargs,
         )
 
         return result
 
+    def list_firewall_network_settings(
+        self,
+        **kwargs,
+    ) -> json:
+        """
+        List the configured Firewall IPS Rules
+
+        :return: (requests.Response object)
+        """
+        result = request_(
+            method="get",
+            url=f"{self.base_uri}/firewallNetworkSettings",
+            headers=self.headers,
+            cookies={
+                "JSESSIONID": self.j_session_id,
+                "ZS_SESSION_CODE": self.zs_session_code,
+            },
+            **kwargs,
+        )
+
+        return result.json()
     def delete_firewall_ips_rule(
         self,
         rule_id: int,
         **kwargs,
     ) -> requests.Response:
         """
         Delete Firewall IPS Rule
@@ -1627,7 +1654,24 @@
                 "JSESSIONID": self.j_session_id,
                 "ZS_SESSION_CODE": self.zs_session_code,
             },
             **kwargs,
         )
 
         return result
+    def list_casb_tenat(self) -> json:
+        """
+        Method to SaaS Application Tenants
+
+        :return: (json)
+        """
+        url = f"/casbTenant?page1&pagesize=100"
+        response = self.hp_http.get_call(
+            url=url,
+            headers=self.headers,
+            cookies={
+                "JSESSIONID": self.j_session_id,
+                "ZS_SESSION_CODE": self.zs_session_code,
+            },
+        )
+
+        return response.json()
```

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/talker.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zia/talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/portal_talker.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zpa/portal_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/talker.py` & `zscaler_api_talkers-5.0.1/zscaler_api_talkers/zpa/talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-5.0.0/PKG-INFO` & `zscaler_api_talkers-5.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-api-talkers
-Version: 5.0.0
+Version: 5.0.1
 Summary: Unofficial Zscaler API python SDK for ZIA, ZPA, ZDX, and Zscaler Client Connector
 Author: Sergio Pereira
 Author-email: sergitopereira@hotmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,23 +18,17 @@
 # Unofficial Zscaler API talkers
 
 ## API Talkers
 
 ### ZIA API Talker
 Python classes to leverage [Zscaler Internet Access API](https://help.zscaler.com/zia/api)
 
-The ZIA API talker is divided into two Class objects: **ZiaTalker** and **ZiaPortalTalker**.  ZiaTalker interacts with 
-ZIA via the published APIs; whereas ZiaPortalTalker interacts with ZIA via the URLs presented in the Portal (aka, the ZIA configuration website).
-
 ### ZPA API Talker
 Python classes to leverage [Zscaler Private Access API](https://help.zscaler.com/zpa/api-reference)
 
-The ZPA API talker is divided into two Class objects: **ZpaTalker** and **ZpaPortalTalker**.  ZpaTalker interacts with 
-ZPA via the published APIs; whereas ZpaPortalTalker interacts with ZPA via the URLs presented in the Portal (aka, the ZPA configuration website).
-
 ### Client Connector API Talker
 A Python class to leverage Zscaler Client Connector API. (Currently in Beta status.)
 
 The Client Connector API talker is accessed via the Class object named: **ClientConnectorTalker**
 
 ### ZDX API Talker
 A Python class to leverage Zscaler Digital Experience API. (Currently in development.)
```

