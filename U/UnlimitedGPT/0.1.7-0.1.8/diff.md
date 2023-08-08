# Comparing `tmp/UnlimitedGPT-0.1.7.tar.gz` & `tmp/UnlimitedGPT-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.7.tar", last modified: Sun Jun 25 22:41:35 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.8.tar", last modified: Tue Aug  8 11:35:28 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.7.tar` & `UnlimitedGPT-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.220149 UnlimitedGPT-0.1.7/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    40614 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      271 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2268 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1274 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      116 2023-06-12 15:20:24.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13290 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-25 22:41:35.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       59 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-08-08 11:35:28.876752 UnlimitedGPT-0.1.8/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    35149 2023-05-26 09:35:45.000000 UnlimitedGPT-0.1.8/LICENSE
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4461 2023-08-08 11:35:28.876752 UnlimitedGPT-0.1.8/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3281 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.8/README.md
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-08-08 11:35:28.872751 UnlimitedGPT-0.1.8/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    41065 2023-08-08 11:30:30.000000 UnlimitedGPT-0.1.8/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-07-14 14:30:36.000000 UnlimitedGPT-0.1.8/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-08-08 11:35:28.876752 UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4461 2023-08-08 11:35:28.000000 UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      259 2023-08-08 11:35:28.000000 UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-08-08 11:35:28.000000 UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       89 2023-08-08 11:35:28.000000 UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       13 2023-08-08 11:35:28.000000 UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-08-08 11:35:28.876752 UnlimitedGPT-0.1.8/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1921 2023-08-08 11:18:29.000000 UnlimitedGPT-0.1.8/setup.py
```

### Comparing `UnlimitedGPT-0.1.7/PKG-INFO` & `UnlimitedGPT-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.7
+Version: 0.1.8
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -19,14 +19,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # UnlimitedGPT
 
 [![Downloads](https://static.pepy.tech/badge/unlimitedgpt)](https://pepy.tech/project/unlimitedgpt)
 [![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Sxvxgeness.svg?style=social)](https://twitter.com/Sxvxgeness)
```

### Comparing `UnlimitedGPT-0.1.7/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.8/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 from undetected_chromedriver import ChromeOptions
 
-from .internal.chatgpt_data import ChatGPTVariables as CGPTV
+from .internal.selectors import ChatGPTVariables as CGPTV
 from .internal.driver import ChatGPTDriver
 from .internal.exceptions import InvalidConversationID
-from .internal.objects import ChatGPTResponse, Conversations, SessionData, SharedConversations, User, Accounts
+from .internal.objects import ChatGPTResponse, Conversations, DefaultAccount, SessionData, SharedConversations, User
 
 class ChatGPT:
     """
     A class for interacting with ChatGPT.
 
     Args:
     ----------
         session_token (str): The session token for authentication.
         conversation_id (str, optional): The conversation ID. Defaults to ''.
         proxy (Optional[str], optional): The proxy server URL. Defaults to None.
         disable_moderation (bool, optional): Whether to disable moderation. Defaults to True.
         verbose (bool, optional): Whether to enable verbose logging. Defaults to False.
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
-        chrome_args (list, optional): Additional arguments for the Chrome browser. Defaults to [].
+        chrome_args (list): Additional arguments for the Chrome browser. Defaults to [].
 
     Raises:
     ----------
         InvalidConversationID: If the conversation ID is invalid.
         ValueError: If the session token is not provided.
         ValueError: If the proxy is invalid.
     """
@@ -58,15 +58,15 @@
         chrome_args: list = [],
     ) -> None:
         self._session_token = session_token
         self._conversation_id = conversation_id
         self._proxy = proxy
         self._disable_moderation = disable_moderation
         self._headless = headless
-        self._chrome_args = chrome_args
+        self._chrome_args = chrome_args or []
         self._clicked_buttons = False
         self._history_and_training_enabled = True
         self._init_logger(verbose)
 
         if self._proxy and not re.findall(
             r"(https?|socks(4|5)?):\/\/.+:\d{1,5}", self._proxy  # type: ignore
         ):
@@ -207,15 +207,15 @@
                     'window.localStorage.setItem("nextauth.message", arguments[0])',
                     payload,
                 )
             except Exception as e:
                 self.logger.debug(f"Failed to update session: {str(e)}")
             sleep(60)
 
-    def _check_blocking_elements(self) -> None:
+    def _check_blocking_elements(self, ignore_conversation_alert: bool = False) -> None:
         """
         Check for blocking elements and dismiss them.
         """
         self.logger.debug("Looking for blocking elements...")
         try:
             intro = WebDriverWait(self.driver, 5).until(
                 EC.presence_of_element_located(CGPTV.intro)
@@ -223,21 +223,22 @@
             self.logger.debug("Dismissing intro...")
             self.driver.execute_script("arguments[0].remove()", intro)
         except TimeoutException:  # type: ignore
             pass
 
         alerts = self.driver.find_elements(*CGPTV.alert)
         if alerts:
-            if "unable to load conversation" in alerts[0].text.lower():
+            if "unable to load conversation" in alerts[0].text.lower() and ignore_conversation_alert is False:
                 raise InvalidConversationID(alerts[0].text)
             self.logger.debug("Dismissing alert...")
             self.driver.execute_script("arguments[0].remove()", alerts[0])
 
         if not self._clicked_buttons:
             for button in CGPTV.info_buttons:
+                self.logger.debug(f"Clicking {button[1]} button")
                 self.driver.safe_click(button, timeout=60)
             self._clicked_buttons = True
 
     def _ensure_cf(self, retry: int = 3) -> None:
         """
         Ensure Cloudflare cookies are set.
 
@@ -292,15 +293,15 @@
         ----------
             timeout (int): Time to wait for the message to continue regenerating before timing out.
 
         Returns:
         ----------
             Optional[str]: The newly generated response.
         """
-        self.logger.debug("Continuing generating...")
+        self.logger.debug("Continuing generation...")
         # Click "Continue generating" button
         continue_response_clicked = self.driver.safe_click(
             CGPTV.continue_regenerating, timeout=5
         )
         if not continue_response_clicked:
             self.logger.debug("Could not click continue regenerating button")
             return None
@@ -408,15 +409,15 @@
 
             self.logger.debug("Clicked shared links manage button")
         except:
             self.logger.debug("Could not open shared conversations popup")
 
         return self._get_out_of_menu()
 
-    def get_user_data(self) -> Optional[Accounts]:
+    def get_user_data(self) -> Optional[DefaultAccount]:
         """
         Gets the user data.
 
         Returns
         ---------
             Optional[Accounts]: a list of the accounts.
         """
@@ -440,15 +441,15 @@
             self.logger.debug("Could not find user data")
             return None
 
         ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": data})
 
         response_data = loads(ret["body"])
 
-        return Accounts(response_data)
+        return DefaultAccount(**response_data["accounts"]['default'])
 
     def get_conversations(self) -> Conversations:
         """
         Get a list of conversations.
 
         Returns:
         ----------
@@ -483,15 +484,15 @@
             response_data["items"],
             response_data["has_missing_conversations"],
             response_data["limit"],
             response_data["offset"],
             response_data["total"]
         )
 
-    def get_shared_conversations(self, timeout: float = 5) -> SharedConversations:
+    def get_shared_conversations(self, timeout: float = 5) -> Optional[SharedConversations]:
         """
         Get a list of shared conversations.
 
         Args:
         ----------
             timeout (float, optional): Time to wait for the message to continue regenerating before timing out.
 
@@ -636,15 +637,15 @@
             continuation = self._continue_generating(timeout=timeout)
             if continuation:
                 content = continuation
 
         self.logger.debug(f"Message sent")
 
         if not self._conversation_id:
-            self.logger.debug(f"New conversation, cathing the id.")
+            self.logger.debug(f"New conversation, catching the ID.")
             self._get_conversation_id()
 
         return ChatGPTResponse(content, self._conversation_id)
 
     def regenerate_response(
         self,
         message_timeout: int = 240,
@@ -743,34 +744,38 @@
         try:
             menu_button_clicked = self.driver.safe_click(CGPTV.menu_button, timeout=60)
             if not menu_button_clicked:
                 self.logger.debug("Could not click menu button")
                 return self._get_out_of_menu()
             self.logger.debug("Clicked menu button")
 
-            clear_conversations_button_clicked = self.driver.safe_click(
-                CGPTV.menu_clear_conversations, timeout=60
-            )
-            if not clear_conversations_button_clicked:
-                self.logger.debug("Could not click clear conversations button")
+            settings_button_clicked = self.driver.safe_click(CGPTV.menu_settings)
+            if not settings_button_clicked:
+                self.logger.debug("Could not click settings button")
                 return self._get_out_of_menu()
-            self.logger.debug("Clicked clear conversations button")
+            self.logger.debug("Clicked settings button")
+
+            clear_button_clicked = self.driver.safe_click(CGPTV.menu_clear_conversations)
+            if not clear_button_clicked:
+                self.logger.debug("Could not click menu clear button")
+                return self._get_out_of_menu()
+            self.logger.debug("Clicked menu clear button")
 
             confirm_clear_button_clicked = self.driver.safe_click(
                 CGPTV.menu_confirm_clear_conversations, timeout=60
             )
             if not confirm_clear_button_clicked:
                 self.logger.debug("Could not click confirm clear conversations button")
                 return self._get_out_of_menu()
             self.logger.debug("Clicked confirm clear conversations button")
 
             self.logger.debug("Cleared all conversations")
             self._get_out_of_menu()
-        except NoSuchElementException: # type: ignore
-            self.logger.debug("Could not find menu buttons")
+        except NoSuchElementException as e: # type: ignore
+            self.logger.debug(f"Could not find menu buttons, exc: {e}")
             return self._get_out_of_menu()
 
     def switch_theme(
         self, theme: Literal["LIGHT", "DARK", "OPPOSITE", "SYSTEM"]
     ) -> None:
         """
         Switch the theme.
@@ -925,15 +930,15 @@
             response["authProvider"],
         )
         self.logger.debug("Authorization is valid")
 
         self.logger.debug("Opening chat page...")
         self.driver.get(f"{CGPTV.chat_url}/{self._conversation_id}")
         self.logger.debug("Opened chat page")
-        self._check_blocking_elements()
+        self._check_blocking_elements(ignore_conversation_alert=True)
         self.logger.debug("Switched account")
         return session_data
 
     def get_session_data(self) -> SessionData:
         """
         Get the session data.
```

### Comparing `UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.8/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.7
+Version: 0.1.8
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -19,14 +19,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # UnlimitedGPT
 
 [![Downloads](https://static.pepy.tech/badge/unlimitedgpt)](https://pepy.tech/project/unlimitedgpt)
 [![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Sxvxgeness.svg?style=social)](https://twitter.com/Sxvxgeness)
```

### Comparing `UnlimitedGPT-0.1.7/setup.py` & `UnlimitedGPT-0.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import os
 
 from setuptools import find_packages, setup
 
 base_path = os.path.abspath(os.path.dirname(__file__))
 
+# requirements = []
+# with open(os.path.join(os.path.dirname(base_path), "requirements.txt")) as f:
+#     requirements = f.read().splitlines()
+
+# readme = ""
+# with open(os.path.join(os.path.dirname(base_path), "README.md")) as f:
+#     readme = f.read()
+
 requirements = []
-with open(os.path.join(os.path.dirname(base_path), "requirements.txt")) as f:
+with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 readme = ""
-with open(os.path.join(os.path.dirname(base_path), "README.md")) as f:
+with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="UnlimitedGPT",
     author="Sxvxge",
     url="https://github.com/Sxvxgee/UnlimitedGPT",
     project_urls={
         "Documentation": "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md",
         "Issue tracker": "https://github.com/Sxvxgee/UnlimitedGPT/issues",
         "Changelog": "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md",
     },
-    version="0.1.7",
-    packages=["UnlimitedGPT", "UnlimitedGPT/internal"],
-    py_modules=["UnlimitedGPT"],
+    version="0.1.8",
+    packages=find_packages(),
+    # py_modules=["UnlimitedGPT"],
     license="GPL-3.0 license",
     description="An unofficial Python wrapper for OpenAI's ChatGPT API",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=requirements,
     python_requires=">=3.8.0",
```

