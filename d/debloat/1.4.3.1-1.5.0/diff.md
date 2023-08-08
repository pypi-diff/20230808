# Comparing `tmp/debloat-1.4.3.1.tar.gz` & `tmp/debloat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.4.3.1.tar", last modified: Tue Jul 11 18:54:17 2023, max compression
+gzip compressed data, was "debloat-1.5.0.tar", last modified: Tue Aug  8 18:24:56 2023, max compression
```

## Comparing `debloat-1.4.3.1.tar` & `debloat-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.142985 debloat-1.4.3.1/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.3.1/LICENSE
--rw-rw-rw-   0        0        0     7907 2023-07-11 18:54:17.142985 debloat-1.4.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7353 2023-07-11 18:34:10.000000 debloat-1.4.3.1/README.md
--rw-rw-rw-   0        0        0      790 2023-07-11 18:53:39.000000 debloat-1.4.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-07-11 18:54:17.144985 debloat-1.4.3.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.092549 debloat-1.4.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.108479 debloat-1.4.3.1/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.3.1/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.3.1/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     3987 2023-07-11 18:51:55.000000 debloat-1.4.3.1/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1702 2023-07-11 18:51:55.000000 debloat-1.4.3.1/src/debloat/main.py
--rw-rw-rw-   0        0        0    24524 2023-07-11 18:52:22.000000 debloat-1.4.3.1/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.138985 debloat-1.4.3.1/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.3.1/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0      579 2023-07-11 18:51:55.000000 debloat-1.4.3.1/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.141485 debloat-1.4.3.1/src/debloat/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-04 17:05:39.000000 debloat-1.4.3.1/src/debloat/utilities/__init__.py
--rw-rw-rw-   0        0        0      746 2023-07-11 18:18:14.000000 debloat-1.4.3.1/src/debloat/utilities/rsrc.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.136484 debloat-1.4.3.1/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7907 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 18:24:56.080533 debloat-1.5.0/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     8321 2023-08-08 18:24:56.081032 debloat-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7769 2023-08-08 22:21:26.000000 debloat-1.5.0/README.md
+-rw-rw-rw-   0        0        0      790 2023-08-08 14:28:36.000000 debloat-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-08-08 18:24:56.082532 debloat-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:24:56.009478 debloat-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 18:24:56.035544 debloat-1.5.0/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.0/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-07-11 19:08:33.000000 debloat-1.5.0/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3984 2023-08-08 22:21:26.000000 debloat-1.5.0/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1725 2023-08-08 22:21:26.000000 debloat-1.5.0/src/debloat/main.py
+-rw-rw-rw-   0        0        0    26248 2023-08-08 22:21:26.000000 debloat-1.5.0/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:24:56.069753 debloat-1.5.0/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.0/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0      561 2023-07-11 19:08:33.000000 debloat-1.5.0/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:24:56.079532 debloat-1.5.0/src/debloat/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.0/src/debloat/utilities/__init__.py
+-rw-rw-rw-   0        0        0    50696 2023-08-08 14:47:25.000000 debloat-1.5.0/src/debloat/utilities/nsisParser.py
+-rw-rw-rw-   0        0        0    20576 2023-08-08 14:47:32.000000 debloat-1.5.0/src/debloat/utilities/readers.py
+-rw-rw-rw-   0        0        0      746 2023-07-11 19:08:33.000000 debloat-1.5.0/src/debloat/utilities/rsrc.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:24:56.062101 debloat-1.5.0/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     8321 2023-08-08 18:24:55.000000 debloat-1.5.0/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-08-08 18:24:56.000000 debloat-1.5.0/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:24:55.000000 debloat-1.5.0/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-08-08 18:24:55.000000 debloat-1.5.0/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-08-08 18:24:55.000000 debloat-1.5.0/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-08 18:24:55.000000 debloat-1.5.0/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.4.3.1/LICENSE` & `debloat-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.4.3.1/PKG-INFO` & `debloat-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.3.1
+Version: 1.5.0
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
-By excess garbage, I mean 300 - 800MB of junk bytes added to a binary to keep it from going into a sandbox.
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox.
 
 Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
 The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
@@ -29,29 +29,29 @@
 
 ## How to use the GUI?
 The GUI of Debloat intends to be as intuitive as possible.
 When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
 Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
 Sound easy? It is!
 
-Running the program should debloat the binary in 30-40 second on average.
+Processing files will take a few seconds.<br>
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
 
-<img width="602" alt="Screenshot 2023-01-29 at 2 52 13 PM" src="https://user-images.githubusercontent.com/77356206/215352245-b37091ce-4d58-415c-a7ba-44a9c45bd6f1.png">
 
 ## How to use the CLI?
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
 My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
 
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch-effort" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
@@ -63,17 +63,22 @@
 In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
 ![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
 
 - [X] Cases where bloat is added inside a PE Section.<br>
 In the image below, the bloat has been included in a PE section named [0]. <br>
 ![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
 
+- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
+These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
+In the image below, Malcat has identified the executable as a NSIS installer.
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
+
 # Partial Support
 
-- [X] Some packer detection for instances where the binary simply cannot be debloated. For example, NullSoft installers. These can be unpacked with UniExtract2 and do not need debloated.
+- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
 
 ### Other use cases
 There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
 
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
@@ -92,16 +97,18 @@
 MacOS<br>
 `pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
 Windows<br>
 `pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
 
 Linux<br> 
-`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." gui.py`
-- I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
+`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
+
+## Credits
+Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
 
 ## Where is this project going next?
 Batch processing: process all files in a directory and produce a report.
 
 Better support for using processing methods outside of debloat.
 
 Support for debloating without unzipping.
```

### Comparing `debloat-1.4.3.1/README.md` & `debloat-1.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
-By excess garbage, I mean 300 - 800MB of junk bytes added to a binary to keep it from going into a sandbox.
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox.
 
 Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
 The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
@@ -15,29 +15,29 @@
 
 ## How to use the GUI?
 The GUI of Debloat intends to be as intuitive as possible.
 When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
 Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
 Sound easy? It is!
 
-Running the program should debloat the binary in 30-40 second on average.
+Processing files will take a few seconds.<br>
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
 
-<img width="602" alt="Screenshot 2023-01-29 at 2 52 13 PM" src="https://user-images.githubusercontent.com/77356206/215352245-b37091ce-4d58-415c-a7ba-44a9c45bd6f1.png">
 
 ## How to use the CLI?
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
 My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
 
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch-effort" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
@@ -49,17 +49,22 @@
 In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
 ![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
 
 - [X] Cases where bloat is added inside a PE Section.<br>
 In the image below, the bloat has been included in a PE section named [0]. <br>
 ![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
 
+- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
+These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
+In the image below, Malcat has identified the executable as a NSIS installer.
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
+
 # Partial Support
 
-- [X] Some packer detection for instances where the binary simply cannot be debloated. For example, NullSoft installers. These can be unpacked with UniExtract2 and do not need debloated.
+- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
 
 ### Other use cases
 There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
 
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
@@ -78,16 +83,18 @@
 MacOS<br>
 `pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
 Windows<br>
 `pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
 
 Linux<br> 
-`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." gui.py`
-- I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
+`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
+
+## Credits
+Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
 
 ## Where is this project going next?
 Batch processing: process all files in a directory and produce a report.
 
 Better support for using processing methods outside of debloat.
 
 Support for debloating without unzipping.
```

### Comparing `debloat-1.4.3.1/pyproject.toml` & `debloat-1.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.4.3.1"
+version = "1.5.0"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
@@ -24,8 +24,8 @@
 [project.urls]
 "Homepage" = "https://github.com/Squiblydoo/debloat"
 "Bug Tracker" = "https://github.com/Squiblydoo/debloat/issues"
 
 
 [project.scripts]
 debloat = "debloat.main:main"
-debloat-gui = "debloat.gui:main"
+debloat-gui = "debloat.gui:main"
```

### Comparing `debloat-1.4.3.1/src/debloat/gui.py` & `debloat-1.5.0/src/debloat/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             self.clear_pathbox()
             return
         out_path = file_path.parent \
             / f"{file_path.stem}_patched{file_path.suffix}"
 
         debloat.processor.process_pe(pe,  out_path, self.unsafe_processing.get(), 
                    log_message=self.output_scrollbox_handler)
-        self.output_scrollbox_handler("-----Processessing took %s seconds ---\n" \
+        self.output_scrollbox_handler("-----Processing took %s seconds ---\n" \
                                     % round((time.time() - start_time), 2))
         self.clear_pathbox()
 
 def main() -> None:
     root = MainWindow()
     root.mainloop()
```

### Comparing `debloat-1.4.3.1/src/debloat/main.py` & `debloat-1.5.0/src/debloat/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     parser.add_argument("executable", 
                         help="Path to the executable to be debloated",
                         type=Path)
     parser.add_argument("--output", 
                         help="Output location", 
                         type=Path,
                         required=False)
-    parser.add_argument("-u", "--last-ditch-effort", dest="unsafe",
+    parser.add_argument("-yolo", "--last-ditch", dest="last_ditch_processing",
                         help="""
-    Run last-ditch-effort processing. In this mode Debloat may remove the
+    Run last-ditch processing. In this mode Debloat may remove the
     whole PE Overlay as a last resort if no smarter method works.
                             """,
                         action='store_true', default=False)
     args = parser.parse_args()
 
     file_path = args.executable
     out_path = args.output
@@ -38,14 +38,14 @@
         print('''
 Provided file is not an executable! Please try again with an executable. 
 Maybe it needs unzipped?'''
               )
         return 1
 
     debloat.processor.process_pe(pe, 
-                        out_path=str(out_path), unsafe_processing=args.unsafe,
+                        out_path=str(out_path), last_ditch_processing=args.last_ditch_processing,
                         log_message=print
                         )
     return 0
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `debloat-1.4.3.1/src/debloat/processor.py` & `debloat-1.5.0/src/debloat/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 Copyright 2019 Jesko Hüttenhain under the 3-Clause BSD License 
 The methods are:
 refinery_strip()
 adjust_offsets()
 refinery_trim_resources()
 The RSRC Class is also from refinery.
 """
+from pathlib import Path
 import re
 from typing import Tuple, Optional, Any, Callable
 import pefile
 import binascii
 import zlib
 from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
 from typing import Generator, Iterable, Optional
 
+import debloat.utilities.nsisParser as nsisParser
 import debloat.utilities.rsrc as rsrc
 
 _KB = 1000
 _MB = _KB * _KB
 
 PACKER = {
     1 : "Nullsoft"
@@ -34,14 +36,36 @@
     elif value < 1024 * 1024:
         return '%.1f KB' % (float(value) / 1024.0)
     elif value < 1024 * 1024 * 1024:
         return '%.1f MB' % (float(value) / 1024.0 / 1024.0)
     else:
         return '%.1f GB' % (float(value) / 1024.0 / 1024.0 / 1024.0)
 
+def write_multiple_files(out_path: str,
+                         files: list, log_message: Callable[[str], None]) -> Tuple[int, str]:
+    '''
+    Writes multiple files to disk when applicable.
+    '''
+    log_message("Installer unpacked!\n")
+    log_message(f"The files are being written to {out_path}")
+    for file in files:
+        out_file_path = Path(out_path) / Path(file.path.replace("\\", "/"))
+        out_dir_path = out_file_path.parent
+        out_dir_path.mkdir(parents=True, exist_ok=True)
+        with open(out_file_path, "wb") as f:
+            f.write(file.data)
+            log_message("File: " + str(Path(file.path.replace("\\", "/"))))
+    log_message("")
+    log_message("The user will need to determine which file is malicious if any.")
+    log_message("If a file is bloated: resubmit it through the tool to debloat it.")
+    log_message(f"Consider reviewing the 'setup.nsis' from the installer to determine how the files were meant to be used.")
+
+    return
+
+
 def write_patched_file(out_path: str,
                         pe: pefile.PE) -> Tuple[int, str]:
     '''Writes the patched file to disk.
     
     Keyword Arguments:
     out_path -- the path and file name to write
     pe -- the pefile that is being processed
@@ -62,30 +86,37 @@
         signature_address = beginning_file_size
     # Check to see if there is data after the signature; if so, it is
     #  junk data
     if beginning_file_size > (signature_address + signature_size):
         return True
     return False
 
-def check_for_packer(pe: pefile.PE) -> int:
+def check_and_extract_NSIS(possible_header: bytearray, data: bytearray) -> list:
+    '''Check if the PE is an NSIS installer.'''
+    extractor = nsisParser.extractNSIS()
+    guess = extractor._find_archive_offset(possible_header)
+    if guess is not None:
+        files = extractor.unpack(data)
+        return files
+
+def check_for_packer(possible_header: bytearray) -> int:
     '''Check overlay bytes for known packers.'''
-    packer_header = pe.write()[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
     # TODO: Evalute any other packers that need special processing.
 
     # NullSoft is not a packer, but an installer. We will detect this. It cannot be processed at this time
     NULLSOFT_MAGICS = [
         # https://nsis.sourceforge.io/Can_I_decompile_an_existing_installer
         B'\xEF\xBE\xAD\xDE' B'Null' B'soft' B'Inst',   # v1.6
         B'\xEF\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.3
         B'\xED\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.1
         B'\xEF\xBE\xAD\xDE' B'nsis' B'inst' B'all\0',  # v1.0
     ]
 
     for magic in range(len(NULLSOFT_MAGICS)):
-        packer_header_match = re.search(NULLSOFT_MAGICS[magic], packer_header)
+        packer_header_match = re.search(NULLSOFT_MAGICS[magic], possible_header)
         if packer_header_match:
              # Future: Handle NSIS installers
             return 1 # Nullsoft
     return 0
 
 def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]:
     '''Iterate through PE sections to identify the last one.'''
@@ -442,15 +473,15 @@
     # The returned size must account for the file alignment.
     # We will make sure it is aligned by adding bytes.
     not_aligned = delta_last_non_junk % alignment
     delta_last_non_junk = delta_last_non_junk - not_aligned
 
     return delta_last_non_junk  
 
-def process_pe(pe: pefile.PE, out_path: str, unsafe_processing: bool,
+def process_pe(pe: pefile.PE, out_path: str, last_ditch_processing: bool,
                log_message: Callable[[str], None]) -> None:
     '''Prepare PE, perform checks, remote junk, write patched binary.'''
     beginning_file_size = len(pe.write())
     # We are using the variable "end_of_real_data" and are reassigning 
     # the value based on our analysis.We are assigning it now in case 
     # we are unable to reduce the binary size for any reason.
     end_of_real_data = beginning_file_size
@@ -464,30 +495,34 @@
     if signature_abnormality:
         log_message('''
 We detected data after the signature. This is abnormal. Removing signature and extra data...''')
         end_of_real_data = signature_address
         pe_data = pe_data[:end_of_real_data]
     # Handle Overlays: this includes packers and overlays which are completely junk
     elif pe.get_overlay_data_start_offset() and signature_size < len(pe.get_overlay()):
+        possible_header = pe.write()[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
+        # Check first to see if the file is NSIS
+        nsis_extracted = check_and_extract_NSIS(possible_header, pe_data)
+        if nsis_extracted:
+            write_multiple_files(out_path, nsis_extracted, log_message)
+            return 0
         log_message("An overlay was detected. Checking for known packer.")
-        packer_idenfitied = check_for_packer(pe)
+        packer_idenfitied = check_for_packer(possible_header)
         if packer_idenfitied:
             log_message("Packer identified: " + PACKER[packer_idenfitied])
             if PACKER[1]:
-                log_message('''
-The original file cannot be debloated. It must be unpacked with a tool such as UniExtract2.
-                ''')
+                log_message("Nullsoft Installer, but unable to extract.")
         else:
             log_message("Packer not identified. Attempting dynamic trim...")
             last_section = find_last_section(pe)
             overlay = pe_data[last_section.PointerToRawData + last_section.SizeOfRawData:]
             end_of_real_data = trim_junk(pe, overlay, end_of_real_data)
             pe_data = pe_data[:end_of_real_data]
-            if end_of_real_data == beginning_file_size:
-                if unsafe_processing is True:
+            if end_of_real_data > (beginning_file_size * 0.9) or end_of_real_data == beginning_file_size :
+                if last_ditch_processing is True:
                     log_message("""
 "Last ditch" switch detected. Running last ditch debloat technique:\n
 This is the last resort that removes the whole overlay: this works in cases where the overlay lacks a pattern.
 However, if the file does not run after this, it is in indicator that this method removed critical data.
                     """)
                     last_section = find_last_section(pe)
                     end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
@@ -503,15 +538,15 @@
         # In order to solve some use cases, we will find the biggest section 
         # within the binary.
         end_of_real_data, result = check_section_compression(pe, pe_data,
                                                              end_of_real_data, 
                                                              log_message=log_message)
         log_message(result)
     # All processing is done. Report results.
-    if end_of_real_data == beginning_file_size:
+    if end_of_real_data > (beginning_file_size * 0.9) or end_of_real_data == beginning_file_size:
         log_message("""No automated method for reducing the size worked. Please consider sharing the
 sample for additional analysis.
 Email: Squiblydoo@pm.me
 Twitter: @SquiblydooBlog.
                     """)
     else:
         pe.__data__ = pe_data
```

### Comparing `debloat-1.4.3.1/src/debloat/tests/debloat_test.py` & `debloat-1.5.0/src/debloat/tests/debloat_test.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import pytest
-import debloat.processor as processor 
-import pefile
-
-
-# Can we print sizes?
-def test_readable_size():
-    assert processor.readable_size(10) == "10 bytes"
-
-
-
-def test_signture_abnormality():
-    # Is there information after the signature?
-    # Signature is at 10 with a size of 5, total file is 15
-    assert processor.handle_signature_abnormality(10, 5, 15) == False
-    # Is there information after the signature?
-    # Signature is at 10 with a size of 5, total file is 20
-    assert processor.handle_signature_abnormality(10, 5, 20) == True
+import pytest
+import debloat.processor as processor 
+import pefile
+
+
+# Can we print sizes?
+def test_readable_size():
+    assert processor.readable_size(10) == "10 bytes"
+
+
+
+def test_signture_abnormality():
+    # Is there information after the signature?
+    # Signature is at 10 with a size of 5, total file is 15
+    assert processor.handle_signature_abnormality(10, 5, 15) == False
+    # Is there information after the signature?
+    # Signature is at 10 with a size of 5, total file is 20
+    assert processor.handle_signature_abnormality(10, 5, 20) == True
```

### Comparing `debloat-1.4.3.1/src/debloat/utilities/rsrc.py` & `debloat-1.5.0/src/debloat/utilities/rsrc.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.3.1/src/debloat.egg-info/PKG-INFO` & `debloat-1.5.0/src/debloat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.3.1
+Version: 1.5.0
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 ![debloat](https://user-images.githubusercontent.com/77356206/215351855-9f89c298-36b4-4234-89b5-dc3f26d1f8b0.png)
 
 # Debloat
 Debloat is a GUI and CLI tool to remove excess garbage from bloated executables.
 
-By excess garbage, I mean 300 - 800MB of junk bytes added to a binary to keep it from going into a sandbox.
+By excess garbage, I mean 100 - 800 MB of junk bytes added to a binary to keep it from going into a sandbox.
 
 Being built with Python, the code and logic is easily accessible for others to take the concepts and apply them to their own tools. The program can be compiled for Windows, MacOS, Linux. The GUI removes any need for remembering commandline options and reading through CLI manuals: it is intended to be as simple as possible. The logic within the program handles the different use cases automatically.
 
 Compiled binaries have already been included in the [Releases](https://github.com/Squiblydoo/debloat/releases/).
 
 The debloat can installed using `pip install debloat`. Use `debloat` to launch the CLI and `debloat-gui` to launch the GUI.
 
@@ -29,29 +29,29 @@
 
 ## How to use the GUI?
 The GUI of Debloat intends to be as intuitive as possible.
 When launched, you can drag and drop bloated file onto the text bar and press the "Process file" button.
 Some technical information will be printed to the scrolling textbox and the file without bloat will be written to the directory the file was pulled from.
 Sound easy? It is!
 
-Running the program should debloat the binary in 30-40 second on average.
+Processing files will take a few seconds.<br>
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/3d2756cd-bc83-44e8-b223-edd8ed464369)
 
-<img width="602" alt="Screenshot 2023-01-29 at 2 52 13 PM" src="https://user-images.githubusercontent.com/77356206/215352245-b37091ce-4d58-415c-a7ba-44a9c45bd6f1.png">
 
 ## How to use the CLI?
 After installing using `pip install debloat` use the command `debloat`.<br>
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
 My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
 
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch-effort" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
@@ -63,17 +63,22 @@
 In the image below, the bloat is identified as in the .rsrc section and is removed from the PE.<br>
 ![Screenshot 2023-02-11 at 3 35 21 PM](https://user-images.githubusercontent.com/77356206/218280086-7cd548f8-e16b-4290-9283-a8a848de1419.png)
 
 - [X] Cases where bloat is added inside a PE Section.<br>
 In the image below, the bloat has been included in a PE section named [0]. <br>
 ![Screenshot 2023-02-11 at 3 26 52 PM](https://user-images.githubusercontent.com/77356206/218279753-ed2c9102-482a-4639-aeb1-df8efc9c4e2e.png)
 
+- [X] Cases where the executable is a Nullsoft Scriptable Installer System executable (NSIS aka Nullsoft)
+These exe are installers that may contain one or more files. The files contained may or may not be malicious. (Sometimes actors will add files simply for increasing the file size.) All files within the installer are extracted to a new directory. The directory also contains the script for the installer which can be consulted to determine which files may be malicious.
+In the image below, Malcat has identified the executable as a NSIS installer.
+![image](https://github.com/Squiblydoo/debloat/assets/77356206/86780abc-da4b-4808-bccb-733d97fa80d8)
+
 # Partial Support
 
-- [X] Some packer detection for instances where the binary simply cannot be debloated. For example, NullSoft installers. These can be unpacked with UniExtract2 and do not need debloated.
+- [X] Cases where the junk is too random and the entropy is too high. In these cases, a switch/option called "--last-ditch" 
 
 ### Other use cases
 There are use cases where the tool does not work. However, I plan to solve for them before publishing too much about them.
 
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
@@ -92,16 +97,18 @@
 MacOS<br>
 `pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
 Windows<br>
 `pyinstaller --onefile  --noconsole  --additional-hooks-dir=./hook --icon=debloat.ico gui.py`
 
 Linux<br> 
-`~/.local/bin/pyinstaller --onefile --noconsole --icon=debloat.ico --additional-hooks-dir=./hook --add-binary "/home/redacted/.local/lib/python3.10/site-packages/:." gui.py`
-- I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
+`pyinstaller --onefile --noconsole --icon=debloat.ico --collect-all tkinterdnd2 gui.py`
+
+## Credits
+Big shoutout to Jesko Hüttenhain creator of [Binary Refinery](https://github.com/binref/refinery). The NSIS extraction is based on his reverse engineering of the NSIS file format. Check out Binary Refinery if you have not.
 
 ## Where is this project going next?
 Batch processing: process all files in a directory and produce a report.
 
 Better support for using processing methods outside of debloat.
 
 Support for debloating without unzipping.
```

