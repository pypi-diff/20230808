# Comparing `tmp/lsstream-1.2.1.tar.gz` & `tmp/lsstream-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.2.1.tar", last modified: Wed Aug  2 20:47:57 2023, max compression
+gzip compressed data, was "lsstream-1.3.0.tar", last modified: Tue Aug  8 19:14:45 2023, max compression
```

## Comparing `lsstream-1.2.1.tar` & `lsstream-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.234718 lsstream-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 20:47:47.000000 lsstream-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:47:57.234718 lsstream-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 20:47:47.000000 lsstream-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 20:47:47.000000 lsstream-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:47:57.234718 lsstream-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.230718 lsstream-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.234718 lsstream-1.2.1/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.234718 lsstream-1.2.1/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.878897 lsstream-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 19:14:35.000000 lsstream-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 19:14:45.878897 lsstream-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 19:14:35.000000 lsstream-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 19:14:35.000000 lsstream-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:14:45.878897 lsstream-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.874897 lsstream-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.874897 lsstream-1.3.0/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.878897 lsstream-1.3.0/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.2.1/LICENSE` & `lsstream-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.2.1/PKG-INFO` & `lsstream-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.2.1
+Version: 1.3.0
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,16 +55,15 @@
 ```
 
 Simply follow the on-screen prompts to streamline your streaming experience! :sparkles:
 
 ## 💡 Features
 
 - **Batch File Generation**: Generates multiple .txt files in a snap. Just input your media titles and links, and `lsstream` will use the correct template to create your files.
-- **Embed Code Testing**: Say goodbye to waiting! Test the embed code instantly and make sure everything works perfectly.
-- **Color-Coded Interface**: The output isn't just useful, it's also pretty. With cool colors enhancing readability, `lsstream` is truly a feast for your eyes!
+- **Embed Code Testing**: Say goodbye to waiting! Test the embed code almost instantaneously and make sure everything works perfectly. Codes are copied to your clipboards and
 
 ## 📝 License
 
 This project is licensed under the MIT License.
 
 ## ❗ Issues
```

### Comparing `lsstream-1.2.1/README.md` & `lsstream-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 ```
 
 Simply follow the on-screen prompts to streamline your streaming experience! :sparkles:
 
 ## 💡 Features
 
 - **Batch File Generation**: Generates multiple .txt files in a snap. Just input your media titles and links, and `lsstream` will use the correct template to create your files.
-- **Embed Code Testing**: Say goodbye to waiting! Test the embed code instantly and make sure everything works perfectly.
-- **Color-Coded Interface**: The output isn't just useful, it's also pretty. With cool colors enhancing readability, `lsstream` is truly a feast for your eyes!
+- **Embed Code Testing**: Say goodbye to waiting! Test the embed code almost instantaneously and make sure everything works perfectly. Codes are copied to your clipboards and
 
 ## 📝 License
 
 This project is licensed under the MIT License.
 
 ## ❗ Issues
```

### Comparing `lsstream-1.2.1/pyproject.toml` & `lsstream-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.2.1"
+version = "1.3.0"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `lsstream-1.2.1/src/lsstream/file_generation.py` & `lsstream-1.3.0/src/lsstream/file_generation.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .defaults import EMBED_TEMPLATE    
 from .style import color
 from .prompts import prompt_directory, prompt_details
 
 # Creates the files and returns its contents
 def create_file(movie_title, media_link, output_directory):
     output_file_path = os.path.join(output_directory, f'{movie_title}.txt')
-    file_content = EMBED_TEMPLATE.format(LINK=media_link, TITLE=movie_title)
+    file_content = EMBED_TEMPLATE.format(LINK=media_link)
 
     with open(output_file_path, 'w') as f:
         f.write(file_content)
     
     return output_file_path, file_content 
 
 # Loop for file and content generation
@@ -25,21 +25,21 @@
     output_directory = prompt_directory()
 
     while True:
         movie_title, media_link = prompt_details()
         movie_titles.append(f'"{movie_title}"')
         new_file, new_content = create_file(movie_title, media_link, output_directory)  
 
-        embed_content = EMBED_TEMPLATE.format(LINK = media_link, TITLE = movie_title)
+        embed_content = EMBED_TEMPLATE.format(LINK = media_link)
         embed_contents.append(embed_content) 
 
         new_files.append(new_file)
         new_contents.append(new_content)  
 
-        continue_prompt = input(color('\nContinue? (Y/N): ', 'white'))
-        if continue_prompt.lower() != 'y':
-            print('\n', color(f"✔ Embed code(s) for {', '.join(movie_titles)} successfully pasted to clipboard!", 'green'))
+        continue_prompt = input(color('\nWould you like to create another embed code file? (Y/N): '))
+        if continue_prompt.lower() != 'y' or continue_prompt.lower() == '':
+            print('\n', color(f"Embed code(s) for {', '.join(movie_titles)} successfully pasted to clipboard!", None))
             break
     
     pyperclip.copy('\n'.join(embed_contents))
     
     return new_files, new_contents
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lsstream-1.2.1/src/lsstream/prompts.py` & `lsstream-1.3.0/src/lsstream/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # If the config file exists, try to read the preferred directory
     if os.path.exists(CONFIG_FILE):
         config.read(CONFIG_FILE)
         if SECTION_NAME in config and KEY_NAME in config[SECTION_NAME]:
             return config[SECTION_NAME][KEY_NAME]
 
     # If we didn't return above, we need to ask the user for the directory
-    output_directory = input(color('\nWhere do you want the files stored?: ', 'white'))
+    output_directory = input(color('\nWhere do you want the files stored?: '))
     if not os.path.isdir(output_directory):
         print(color("Invalid directory, please enter a valid directory.", 'red'))
         return prompt_directory()
 
     # Save the preferred directory in the config file
     if SECTION_NAME not in config:
         config.add_section(SECTION_NAME)
@@ -31,22 +31,23 @@
 
     return output_directory
 
 
 # Prompt users for movie details
 def prompt_details():
     movie_title = input(color('\nEnter the Media Title: '))
-    media_link = input(color('\nEnter the Media Link: '))
+    media_link = input(color('\nEnter the Media Embed Code: '))
 
     return movie_title, media_link
 
 # Prompts users if they want to test the links
 def prompt_test_html():
-    test_prompt = input(color('\nDo you want to test the media(s)? (Y/N): ', 'cyan'))
-    if test_prompt.lower() == 'y':
+    test_prompt = input(color('\nWould you like to try out the embed code(s) on the test page? (Y/N): '))
+    if test_prompt.lower() == 'ez': return "secret"
+    if test_prompt.lower() == 'y' or test_prompt.lower() == '':
         return True
     
 def prompt_update_preferred_directory():
     config = configparser.ConfigParser()
 
     # Prompt the user for the new directory
     new_directory = input('\nEnter the new preferred directory: ')
@@ -59,11 +60,11 @@
         config.read(CONFIG_FILE)
         if SECTION_NAME not in config:
             config.add_section(SECTION_NAME)
         config[SECTION_NAME][KEY_NAME] = new_directory
         with open(CONFIG_FILE, 'w') as config_file:
             config.write(config_file)
 
-    print(color("Preferred directory updated successfully!", 'green'))
+    print(color("Preferred directory updated successfully!", None))
 
     return new_directory
```

### Comparing `lsstream-1.2.1/src/lsstream/run.py` & `lsstream-1.3.0/src/lsstream/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import os
-import webbrowser
+import configparser
 from .style import intro, color
 from .file_generation import create_content
 from .prompts import prompt_test_html
 from .test import test_html, open_canvas_test_page
+from .prompts import CONFIG_FILE, SECTION_NAME, KEY_NAME
+ 
 
 # Delete current batch of html files
 def end_session(new_files, new_contents):
-    end_prompt = input(color('\nAre you done with this session? (Y/N): ', 'white'))
-    if end_prompt.lower() == 'y':
+    end_prompt = input(color('\nAre you done with this session? (Y/N): '))
+    if end_prompt.lower() == 'y' or end_prompt.lower() == '':
         if os.path.exists('temp.html'):
             os.remove('temp.html')
 
-        print(color(f'\n✔ Done!', 'green'))
+        print(color(f'\nGreat work!', None))
 
-    else:
+    elif end_prompt.lower() == 'n':
         while True:
-            print(color('\nA: Start a new batch?', 'yellow'))
-            print(color('B: Test the media(s)?', 'cyan'))
-            print(color('C: Remove the newly created files and restart?', 'red'))
-            print(color('D: End session?', 'green'))
-            continue_prompt = input(color('What would you like to do? (', 'white') + color('A', 'yellow') + color('/', 'white') + color('B', 'cyan') + color('/', 'white') + color('C', 'red') + color('/', 'white') + color('D', 'green') + color('): ', 'white'))
+            print(color('\nA: Start a new batch', None))
+            print(color('B: Bring up test page', None))
+            print(color('C: Remove the newly created embed code file(s) and restart', None))
+            print(color('D: End session', None))
+            continue_prompt = input(color('What would you like to do? (A/B/C/D): '))
             
             if continue_prompt.lower() == 'a':
                 lsstream()
                 break
             elif continue_prompt.lower() == 'b':
-                webbrowser.open('file://' + os.path.realpath('temp.html'))
+                open_canvas_test_page()
                 end_session(new_files, new_contents)
                 break
             elif continue_prompt.lower() == 'c':
                 for file in new_files:
                     os.remove(file)
                 if os.path.exists('temp.html'):
                     os.remove('temp.html')
@@ -39,24 +41,39 @@
             elif continue_prompt.lower() == 'd':
                 if os.path.exists('temp.html'):
                     os.remove('temp.html')
                     
                 print(color(f'\n✔ Done!', 'green'))
                 break
             else:
-                print(color('\nInvalid option, please choose A, B, or C.', 'red'))
+                print(color('\nInvalid option, please choose A, B, C or D.', 'red'))
+                
 
 def lsstream():    
     new_files, new_contents = create_content()
 
-    # if prompt_test_html(new_contents): test_html(new_contents)
-    if prompt_test_html(): open_canvas_test_page()
+    result = prompt_test_html()
+    if result == "secret":
+        test_html(new_contents)
+    elif result == True:
+        open_canvas_test_page()
+
 
     end_session(new_files, new_contents) 
 
 
 def main():
-    print(color(intro.renderText('LSSTREAM'), 'green'))
+    print(color(intro.renderText('LSSTREAM')))
+
+    config = configparser.ConfigParser()
+
+    if os.path.exists(CONFIG_FILE):
+        config.read(CONFIG_FILE)
+        if SECTION_NAME in config and KEY_NAME in config[SECTION_NAME]:
+            directory_name = config[SECTION_NAME][KEY_NAME]
+            directory_name = color(directory_name, None, attrs=["underline"])
+            print(f"Your embed code files will be stored in {directory_name}")
+        
     lsstream() 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lsstream-1.2.1/src/lsstream.egg-info/PKG-INFO` & `lsstream-1.3.0/src/lsstream.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.2.1
+Version: 1.3.0
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,16 +55,15 @@
 ```
 
 Simply follow the on-screen prompts to streamline your streaming experience! :sparkles:
 
 ## 💡 Features
 
 - **Batch File Generation**: Generates multiple .txt files in a snap. Just input your media titles and links, and `lsstream` will use the correct template to create your files.
-- **Embed Code Testing**: Say goodbye to waiting! Test the embed code instantly and make sure everything works perfectly.
-- **Color-Coded Interface**: The output isn't just useful, it's also pretty. With cool colors enhancing readability, `lsstream` is truly a feast for your eyes!
+- **Embed Code Testing**: Say goodbye to waiting! Test the embed code almost instantaneously and make sure everything works perfectly. Codes are copied to your clipboards and
 
 ## 📝 License
 
 This project is licensed under the MIT License.
 
 ## ❗ Issues
```

