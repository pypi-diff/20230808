# Comparing `tmp/cmn-1.9.0.tar.gz` & `tmp/cmn-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmn-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cmn-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cmn-1.9.0.tar` & `cmn-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0       88 2023-08-07 19:14:41.930601 cmn-1.9.0/.gitignore
--rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.9.0/LICENSE
--rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.9.0/README.md
--rw-r--r--   0        0        0      540 2023-08-07 20:24:40.906103 cmn-1.9.0/pyproject.toml
--rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.9.0/requirements.txt
--rw-r--r--   0        0        0     4726 2023-08-07 19:02:33.161717 cmn-1.9.0/src/ChangeMediaName/ChangeMediaName.py
--rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.9.0/src/ColoredLogger/ColoredLogger.py
--rw-r--r--   0        0        0     2818 2023-08-07 20:22:09.175027 cmn-1.9.0/src/OutputFormatter/OutputFormatter.py
--rw-r--r--   0        0        0     2333 2023-08-07 20:22:09.159388 cmn-1.9.0/src/OutputFormatter/test_OutputFormatter.py
--rw-r--r--   0        0        0     4099 2023-08-07 20:22:09.159388 cmn-1.9.0/src/cmn/__init__.py
--rw-r--r--   0        0        0     3071 2023-08-07 20:00:09.458595 cmn-1.9.0/src/cmn/__main__.py
--rw-r--r--   0        0        0     7213 2023-08-07 20:23:05.915432 cmn-1.9.0/src/test_main.py
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 cmn-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      532 2023-08-07 23:32:47.399899 cmn-2.0.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1186 2023-08-07 23:32:47.399899 cmn-2.0.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      662 2023-08-07 23:32:47.399899 cmn-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       81 2023-08-07 23:32:47.403900 cmn-2.0.0/.gitignore
+-rw-r--r--   0        0        0     9161 2023-08-07 23:32:47.403900 cmn-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2622 2023-08-07 23:32:47.403900 cmn-2.0.0/README.md
+-rw-r--r--   0        0        0     4039 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/__init__.py
+-rw-r--r--   0        0        0     3314 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/__main__.py
+-rw-r--r--   0        0        0     4686 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/change_media_name/change_media_name.py
+-rw-r--r--   0        0        0     1059 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/colored_logger/colored_logger.py
+-rw-r--r--   0        0        0     2737 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/output_formatter/output_formatter.py
+-rw-r--r--   0        0        0     2253 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/output_formatter/test_output_formatter.py
+-rw-r--r--   0        0        0     7675 2023-08-07 23:32:47.403900 cmn-2.0.0/cmn/test_main.py
+-rw-r--r--   0        0        0      519 2023-08-07 23:32:47.403900 cmn-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-08-07 23:32:47.403900 cmn-2.0.0/requirements.txt
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 cmn-2.0.0/PKG-INFO
```

### Comparing `cmn-1.9.0/LICENSE` & `cmn-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-Apache License
-Version 2.0, January 2004
-http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-2. Grant of Copyright License.
-
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License.
-
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-4. Redistribution.
-
-You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-    You must give any other recipients of the Work or Derivative Works a copy of this License; and
-    You must cause any modified files to carry prominent notices stating that You changed the files; and
-    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-5. Submission of Contributions.
-
-Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-6. Trademarks.
-
-This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty.
-
-Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability.
-
-In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability.
-
-While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
-
-END OF TERMS AND CONDITIONS
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+
+"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+
+"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+
+"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+
+"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+
+"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+
+"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+
+2. Grant of Copyright License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+
+4. Redistribution.
+
+You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+
+    You must give any other recipients of the Work or Derivative Works a copy of this License; and
+    You must cause any modified files to carry prominent notices stating that You changed the files; and
+    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+
+You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+
+5. Submission of Contributions.
+
+Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+
+6. Trademarks.
+
+This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty.
+
+Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability.
+
+In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability.
+
+While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
```

### Comparing `cmn-1.9.0/README.md` & `cmn-2.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-# ChangeMediaName
-Tool that changes media files to its creation date.
-
-## Usage
-```
-python3 ChangeMediaName.py -i <paths>
-```
-
-## Options
-
-| Option 1 | Option 2              | Description                                                           |
-|----------|-----------------------|-----------------------------------------------------------------------|
-| h        | help                  | Show this help message and exit                                       |
-| i        | input-files           | **Required**. File(s) or folder(s) to scan                            |
-| v        | verbose               | Default: `False`. Verbose mode                                        |
-| r        | recursive             | Default: `False`. Scan folders recursively                            |
-| ni       | ignored-paths         | Default: `None`. Files or folders to be ignored                       |
-| nr       | not-ignore-subfolders | Default: `True`. Choose to not ignore subfolders of the ignored paths |
-| t        | file-types            | Default: `None`. List of file types to consider                       |
-| nt       | not-file-types        | Default: `None`. List of file types to ignore                         |
-| of       | only-images           | Default: `False`. Consider only images                                |
-| ov       | only-videos           | Default: `False`. Consider only videos                                |
-| cf       | create-new-folders    | Default: `False`. Create new folders according to the new image names |
-| fn       | name-format           | Default:`%Y%m%d_%H%M%S` Format of the new names                       |
-| ff       | name-folder-format    | Default:`%Y - %m - %d`. Format of the new folder names                |
-
-
-## Supported file types
-| Type  | Extension | Name                                         |
-|-------|-----------|----------------------------------------------|
-| Image | HEIC      | High Efficiency Image File Format            |
-| Image | JPEG      | Joint Photographic Experts Group File Format |
-| Image | JPG       | Joint Photographic Group File Format         |
-| Image | PNG       | Portable Network Graphics File Format        |
-| Image | WEBP      | WebP Image File Format                       |
-| Video | AVI       | Audio Video Interleave                       |
-| Video | AVI       | Audio Video Interleave                       |
-| Video | MP4       | MPEG-4 Part 14                               |
-
-## Requirements
-- Install `exiftool` command from https://exiftool.org/. Credits to Phil Harvey.
-
-## Made by me :)
+# ChangeMediaName
+Tool that changes media files to its creation date.
+
+## Installation
+```
+pip install cmn
+```
+
+## Usage
+```
+cmn -i <input-files> [options]
+```
+
+## Options
+
+| Option 1 | Option 2              | Description                                                           |
+|----------|-----------------------|-----------------------------------------------------------------------|
+| h        | help                  | Show this help message and exit                                       |
+| i        | input-files           | **Required**. File(s) or folder(s) to scan                            |
+| v        | verbose               | Default: `False`. Verbose mode                                        |
+| r        | recursive             | Default: `False`. Scan folders recursively                            |
+| ni       | ignored-paths         | Default: `None`. Files or folders to be ignored                       |
+| nr       | not-ignore-subfolders | Default: `True`. Choose to not ignore subfolders of the ignored paths |
+| t        | file-types            | Default: `None`. List of file types to consider                       |
+| nt       | not-file-types        | Default: `None`. List of file types to ignore                         |
+| of       | only-images           | Default: `False`. Consider only images                                |
+| ov       | only-videos           | Default: `False`. Consider only videos                                |
+| cf       | create-new-folders    | Default: `False`. Create new folders according to the new image names |
+| fn       | name-format           | Default: `%Y%m%d_%H%M%S`. Format of the new names                     |
+| ff       | name-folder-format    | Default: `%Y - %m - %d`. Format of the new folder names               |
+
+
+## Supported file types
+| Type  | Extension | Name                                         |
+|-------|-----------|----------------------------------------------|
+| Image | HEIC      | High Efficiency Image File Format            |
+| Image | JPEG      | Joint Photographic Experts Group File Format |
+| Image | JPG       | Joint Photographic Group File Format         |
+| Image | PNG       | Portable Network Graphics File Format        |
+| Image | WEBP      | WebP Image File Format                       |
+| Video | AVI       | Audio Video Interleave                       |
+| Video | AVI       | Audio Video Interleave                       |
+| Video | MP4       | MPEG-4 Part 14                               |
+
+## Requirements
+- Install `exiftool` command from https://exiftool.org/. Credits to Phil Harvey.
```

### Comparing `cmn-1.9.0/src/ChangeMediaName/ChangeMediaName.py` & `cmn-2.0.0/cmn/change_media_name/change_media_name.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,160 @@
-"""
-CMN - Common functions
-"""
-__version__ = "1.0.1"
-import os
-import subprocess
-from datetime import datetime
-from shutil import which
-
-from src import ColoredLogger
-from src.OutputFormatter.OutputFormatter import ImageRegularformatter, VideoRegularformatter, AVIformatter
-
-NewNameFile = '{year}{month}{day}_{hour}{minute}{second}{filetype}'
-NewNameFolder = '{year}-{month}-{day}'
-
-nChanged = 0
-nErrors = 0
-completed = 0.0
-
-logger: ColoredLogger
-
-formatters = {
-    ".jpg": ImageRegularformatter,
-    ".jpeg": ImageRegularformatter,
-    ".png": ImageRegularformatter,
-    ".mp4": VideoRegularformatter,
-    ".avi": AVIformatter,
-    ".mov": VideoRegularformatter,
-    ".heic": ImageRegularformatter,
-    ".webp": ImageRegularformatter,
-}
-
-
-def checkExiftool() -> bool:
-    return which('exiftool') is not None
-
-
-def getDateTime(file: str) -> tuple:
-    global logger
-    try:
-        output = subprocess.check_output(["exiftool", file], shell=True, text=True, stderr=subprocess.STDOUT)
-        output = output.strip()
-        return formatters[os.path.splitext(file)[1].lower()](output).getGroups()
-    except (Exception,):
-        logger.error(f"{completed:.2f}% - Error getting datetime for {file}")
-
-    return ()
-
-
-def createFolder(folderFormat: str, date: tuple[str]) -> str:
-    global logger
-    if len(date) == 7:
-        datestr = datetime.strptime("".join(date), "%Y%m%d%H%M%S%f")
-    else:
-        datestr = datetime.strptime("".join(date), "%Y%m%d%H%M%S")
-
-    folder = datestr.strftime(folderFormat)
-    if not os.path.exists(folder):
-        os.mkdir(folder)
-        logger.info(f"{completed:.2f}% - Created folder {folder}")
-    return folder
-
-
-def changeFileName(oldPath: str, newPath: str, oldFile: str, nameFormat: str, date_tuple: tuple[str]):
-    global nChanged, nErrors, logger
-
-    date_str = "".join(date_tuple)
-    if len(date_tuple) == 7:
-        date = datetime.strptime(date_str, "%Y%m%d%H%M%S%f")
-    else:
-        date = datetime.strptime(date_str, "%Y%m%d%H%M%S")
-
-    new = date.strftime(nameFormat)
-    new += os.path.splitext(oldFile)[1]
-
-    counter = 1
-
-    if new == oldFile:
-        logger.warning(f"{completed:.2f}% - File {oldFile} already has the correct name.")
-        return
-
-    # Need to check if path exists AND if the file is the same. If it is the same, we don't need to change the name.
-    while os.path.exists(os.path.join(newPath, new)):
-        counter += 1
-
-        new = date.strftime(nameFormat)
-        new += '(' + str(counter) + ')'
-        new += os.path.splitext(oldFile)[1]
-
-    try:
-        os.rename(os.path.join(oldPath, oldFile), os.path.join(newPath, new))
-        logger.success(f"{completed:.2f}% - Changed {oldFile} to {new}")
-        nChanged += 1
-    except (Exception,) as e:
-        logger.error(f"{completed:.2f}% - Error while changing name of {oldFile}: {e}")
-        nErrors += 1
-
-
-def cmn(coloredLog: ColoredLogger, files: list[str], newFolder: bool, nameFormat: str, folderFormat: str) -> \
-        (int, int, int):
-    global logger, nErrors, completed
-    logger = coloredLog
-    command = checkExiftool()
-    percentage = 100 / (2*(len(files)))
-    completed = 0.00
-    if not command:
-        logger.critical("Exiftool program/Command missing. Please install it: https://exiftool.org/install.html")
-        return 0, 0, 1
-
-    for file in files:
-        completed += percentage
-        logger.info(f"{completed:.2f}% - Processing {file}")
-        completed += percentage
-        try:
-            date = getDateTime(file)
-        except (Exception,):
-            logger.error(f"{completed:.2f}% - Error while getting date from {file}.")
-            continue
-
-        if date == ():
-            logger.warning(f"{completed:.2f}% - Couldn't get date from {file}.")
-            continue
-
-        folder = ""
-        if newFolder:
-            try:
-                folder = createFolder(folderFormat, date)
-            except (Exception,):
-                logger.error(f"{completed:.2f}% - Error while creating folder for {file}.")
-                continue
-
-        try:
-            oldpath = os.path.dirname(file)
-            oldfile = os.path.basename(file)
-            if folder:
-                newpath = os.path.join(os.getcwd(), folder)
-            else:
-                newpath = oldpath
-            changeFileName(oldpath, newpath, oldfile, nameFormat, date)
-        except (Exception,):
-            logger.error(f"{completed:.2f}% - Error getting new path of {file}.")
-            nErrors += 1
-            continue
-
-    return nChanged, nErrors
-
-if __name__ == "__main__":
-    print("dont")
+"""
+CMN - Common functions
+"""
+__version__ = "2.0.0"
+
+import os
+import subprocess
+from datetime import datetime
+from shutil import which
+
+from cmn.colored_logger.colored_logger import ColoredLogger
+from cmn.output_formatter.output_formatter import (
+    ImageRegularformatter,
+    VideoRegularformatter,
+    AVIformatter
+)
+
+NewNameFile = '{year}{month}{day}_{hour}{minute}{second}{filetype}'
+NewNameFolder = '{year}-{month}-{day}'
+
+n_changed = 0
+n_errors = 0
+completed = 0.0
+
+logger: ColoredLogger
+
+formatters = {
+    ".jpg": ImageRegularformatter,
+    ".jpeg": ImageRegularformatter,
+    ".png": ImageRegularformatter,
+    ".mp4": VideoRegularformatter,
+    ".avi": AVIformatter,
+    ".mov": VideoRegularformatter,
+    ".heic": ImageRegularformatter,
+    ".webp": ImageRegularformatter,
+}
+
+
+def checkExiftool() -> bool:
+    return which('exiftool') is not None
+
+
+def getDateTime(file: str) -> tuple:
+    global logger
+    try:
+        output = subprocess.check_output(
+            ["exiftool", file],
+            shell=True, text=True, stderr=subprocess.STDOUT
+        )
+        output = output.strip()
+        return formatters[os.path.splitext(file)[1].lower()](output).getGroups()
+    except (Exception,):
+        logger.error(f"{completed:.2f}% - Error getting datetime for {file}")
+
+    return ()
+
+
+def createFolder(folderFormat: str, date: tuple[str]) -> str:
+    global logger
+    if len(date) == 7:
+        datestr = datetime.strptime("".join(date), "%Y%m%d%H%M%S%f")
+    else:
+        datestr = datetime.strptime("".join(date), "%Y%m%d%H%M%S")
+
+    folder = datestr.strftime(folderFormat)
+    if not os.path.exists(folder):
+        os.mkdir(folder)
+        logger.info(f"{completed:.2f}% - Created folder {folder}")
+    return folder
+
+
+def changeFileName(
+        oldPath: str, newPath: str, oldFile: str,
+        nameFormat: str, date_tuple: tuple[str]
+):
+    global n_changed, n_errors, logger
+
+    date_str = "".join(date_tuple)
+    if len(date_tuple) == 7:
+        date = datetime.strptime(date_str, "%Y%m%d%H%M%S%f")
+    else:
+        date = datetime.strptime(date_str, "%Y%m%d%H%M%S")
+
+    new = date.strftime(nameFormat)
+    new += os.path.splitext(oldFile)[1]
+
+    counter = 1
+
+    if new == oldFile:
+        logger.warning(f"{completed:.2f}% - File {oldFile} already has the correct name.")
+        return
+
+    # Need to check if path exists AND if the file is the same. If it is the same, we don't need to change the name.
+    while os.path.exists(os.path.join(newPath, new)):
+        counter += 1
+
+        new = date.strftime(nameFormat)
+        new += '(' + str(counter) + ')'
+        new += os.path.splitext(oldFile)[1]
+
+    try:
+        os.rename(os.path.join(oldPath, oldFile), os.path.join(newPath, new))
+        logger.success(f"{completed:.2f}% - Changed {oldFile} to {new}")
+        n_changed += 1
+    except (Exception,) as e:
+        logger.error(f"{completed:.2f}% - Error while changing name of {oldFile}: {e}")
+        n_errors += 1
+
+
+def cmn(coloredLog: ColoredLogger, files: list[str], newFolder: bool, nameFormat: str, folderFormat: str) -> \
+        (int, int):
+    global logger, n_errors, completed
+    logger = coloredLog
+    command = checkExiftool()
+    percentage = 100 / (2 * (len(files)))
+    completed = 0.00
+    if not command:
+        logger.critical("Exiftool program/Command missing. Please install it: https://exiftool.org/install.html")
+        return 0, 1
+
+    for file in files:
+        completed += percentage
+        logger.info(f"{completed:.2f}% - Processing {file}")
+        completed += percentage
+        try:
+            date = getDateTime(file)
+        except (Exception,):
+            logger.error(f"{completed:.2f}% - Error while getting date from {file}.")
+            continue
+
+        if date == ():
+            logger.warning(f"{completed:.2f}% - Couldn't get date from {file}.")
+            continue
+
+        folder = ""
+        if newFolder:
+            try:
+                folder = createFolder(folderFormat, date)
+            except (Exception,):
+                logger.error(f"{completed:.2f}% - Error while creating folder for {file}.")
+                continue
+
+        try:
+            oldpath = os.path.dirname(file)
+            oldfile = os.path.basename(file)
+            if folder:
+                newpath = os.path.join(os.getcwd(), folder)
+            else:
+                newpath = oldpath
+            changeFileName(oldpath, newpath, oldfile, nameFormat, date)
+        except (Exception,):
+            logger.error(f"{completed:.2f}% - Error getting new path of {file}.")
+            n_errors += 1
+            continue
+
+    return n_changed, n_errors
+
+
+if __name__ == "__main__":
+    print("dont")
```

### Comparing `cmn-1.9.0/src/OutputFormatter/OutputFormatter.py` & `cmn-2.0.0/cmn/output_formatter/output_formatter.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import re
-
-months = {
-    "Jan": "01",
-    "Feb": "02",
-    "Mar": "03",
-    "Apr": "04",
-    "May": "05",
-    "Jun": "06",
-    "Jul": "07",
-    "Aug": "08",
-    "Sep": "09",
-    "Oct": "10",
-    "Nov": "11",
-    "Dec": "12"
-}
-
-
-class OutputFormatter:
-    def __init__(self, output: str, expressions: list[str]):
-        self.output = output
-        self.expressions = expressions
-
-    def format(self) -> tuple:
-        for expression in self.expressions:
-            match = re.search(expression, self.output)
-            if match:
-                groups = match.groups()
-                if (1957 <= int(groups[0]) and 1 <= int(groups[1]) <= 12 and 1 <= int(groups[2]) <= 31 and
-                        0 <= int(groups[3]) <= 23 and 0 <= int(groups[4]) <= 59 and 0 <= int(groups[5]) <= 59):
-                    return groups
-        return ()
-
-    def refactor(self, groups: tuple) -> tuple:
-        return groups
-
-    def getGroups(self):
-        return self.refactor(self.format())
-
-
-class AVIformatter(OutputFormatter):
-    def __init__(self, output: str):
-        super().__init__(output, [
-            r"Date\s*Time\s*\d\s*:\s*\w{3}\s*(\w{3})\s*(\d{1,2})\s*(\d{2}):(\d{2}):(\d{2})\s*(\d{4})",
-        ])
-
-    def format(self) -> tuple:
-        for expression in self.expressions:
-            match = re.search(expression, self.output)
-            if match:
-                groups = match.groups()
-                if groups[0] in months.keys() and 1 <= int(groups[1]) <= 31 and 0 <= int(groups[2]) <= 23 and \
-                        0 <= int(groups[3]) <= 59 and 0 <= int(groups[4]) <= 59 and 1957 <= int(groups[5]):
-                    return groups
-        return ()
-
-    def refactor(self, groups: tuple) -> tuple:
-        if groups:
-            return groups[5], months[groups[0]], groups[1], groups[2], groups[3], groups[4]
-        return ()
-
-    def getGroups(self):
-        return self.refactor(self.format())
-
-
-class ImageRegularformatter(OutputFormatter):
-    def __init__(self, output: str):
-        super().__init__(output, [
-            r"Date/Time Original\s*:\s*(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})\.(\d{3})",
-            r"Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})\.(\d{3})",
-            r"Date/Time Original\s*:\s*(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})",
-            r"Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})"
-        ])
-
-
-class VideoRegularformatter(OutputFormatter):
-    def __init__(self, output: str):
-        super().__init__(output, [
-            r"Media Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})\.(\d{3})",
-            r"Media Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})"
-        ])
+import re
+
+months = {
+    "Jan": "01",
+    "Feb": "02",
+    "Mar": "03",
+    "Apr": "04",
+    "May": "05",
+    "Jun": "06",
+    "Jul": "07",
+    "Aug": "08",
+    "Sep": "09",
+    "Oct": "10",
+    "Nov": "11",
+    "Dec": "12"
+}
+
+
+class OutputFormatter:
+    def __init__(self, output: str, expressions: list[str]):
+        self.output = output
+        self.expressions = expressions
+
+    def format(self) -> tuple:
+        for expression in self.expressions:
+            match = re.search(expression, self.output)
+            if match:
+                groups = match.groups()
+                if (1957 <= int(groups[0]) and 1 <= int(groups[1]) <= 12 and 1 <= int(groups[2]) <= 31 and
+                        0 <= int(groups[3]) <= 23 and 0 <= int(groups[4]) <= 59 and 0 <= int(groups[5]) <= 59):
+                    return groups
+        return ()
+
+    def refactor(self, groups: tuple) -> tuple:
+        return groups
+
+    def getGroups(self):
+        return self.refactor(self.format())
+
+
+class AVIformatter(OutputFormatter):
+    def __init__(self, output: str):
+        super().__init__(output, [
+            r"Date\s*Time\s*\d\s*:\s*\w{3}\s*(\w{3})\s*(\d{1,2})\s*(\d{2}):(\d{2}):(\d{2})\s*(\d{4})",
+        ])
+
+    def format(self) -> tuple:
+        for expression in self.expressions:
+            match = re.search(expression, self.output)
+            if match:
+                groups = match.groups()
+                if groups[0] in months.keys() and 1 <= int(groups[1]) <= 31 and 0 <= int(groups[2]) <= 23 and \
+                        0 <= int(groups[3]) <= 59 and 0 <= int(groups[4]) <= 59 and 1957 <= int(groups[5]):
+                    return groups
+        return ()
+
+    def refactor(self, groups: tuple) -> tuple:
+        if groups:
+            return groups[5], months[groups[0]], groups[1], groups[2], groups[3], groups[4]
+        return ()
+
+    def getGroups(self):
+        return self.refactor(self.format())
+
+
+class ImageRegularformatter(OutputFormatter):
+    def __init__(self, output: str):
+        super().__init__(output, [
+            r"Date/Time Original\s*:\s*(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})\.(\d{3})",
+            r"Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})\.(\d{3})",
+            r"Date/Time Original\s*:\s*(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})",
+            r"Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})"
+        ])
+
+
+class VideoRegularformatter(OutputFormatter):
+    def __init__(self, output: str):
+        super().__init__(output, [
+            r"Media Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})\.(\d{3})",
+            r"Media Create Date\s+:\s(\d{4}):(\d{2}):(\d{2})\s*(\d{2}):(\d{2}):(\d{2})"
+        ])
```

### Comparing `cmn-1.9.0/src/OutputFormatter/test_OutputFormatter.py` & `cmn-2.0.0/cmn/output_formatter/test_output_formatter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import unittest
-
-from src.OutputFormatter.OutputFormatter import ImageRegularformatter, VideoRegularformatter, AVIformatter
-
-
-class OutputFormatterTest(unittest.TestCase):
-    def test_getDateTime(self):
-        samples = [
-            {
-                "output": "Track Create Date               : 0000:00:00 00:00:00",
-                "formatter": VideoRegularformatter,
-                "expected": ()
-            },
-            {
-                "output": "Track Create Date               : 0000:00:00 00:00:00",
-                "formatter": AVIformatter,
-                "expected": ()
-            },
-            {
-                "output": "Track Create Date               : 0000:00:00 00:00:00",
-                "formatter": ImageRegularformatter,
-                "expected": ()
-            },
-            {
-                "output": "Track Create Date               : 0000:00:00 00:00:00",
-                "formatter": VideoRegularformatter,
-                "expected": ()
-            },
-            {
-                "output": "Track Create Date               : 0000:00:00 00:00:00",
-                "formatter": AVIformatter,
-                "expected": ()
-            },
-            {
-                "output": "Track Create Date               : 0000:00:00 00:00:00",
-                "formatter": ImageRegularformatter,
-                "expected": ()
-            },
-            {
-                "output": "Date/Time Original                    : 2023:07:16 17:13:57",
-                "formatter": VideoRegularformatter,
-                "expected": ()
-            },
-            {
-                "output": "Date/Time Original                    : 2023:07:16 17:13:57",
-                "formatter": AVIformatter,
-                "expected": ()
-            },
-            {
-                "output": "Date/Time Original                    : 2023:07:16 17:13:57",
-                "formatter": ImageRegularformatter,
-                "expected": ("2023", "07", "16", "17", "13", "57")
-            },
-        ]
-        for i in range(0, len(samples)):
-            actual = samples[i]["formatter"](samples[i]["output"]).getGroups()
-            self.assertEqual(actual, samples[i]["expected"], f"Error in {samples[i]}")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from output_formatter import ImageRegularformatter, VideoRegularformatter, AVIformatter
+
+
+class OutputFormatterTest(unittest.TestCase):
+    def test_getDateTime(self):
+        samples = [
+            {
+                "output": "Track Create Date               : 0000:00:00 00:00:00",
+                "formatter": VideoRegularformatter,
+                "expected": ()
+            },
+            {
+                "output": "Track Create Date               : 0000:00:00 00:00:00",
+                "formatter": AVIformatter,
+                "expected": ()
+            },
+            {
+                "output": "Track Create Date               : 0000:00:00 00:00:00",
+                "formatter": ImageRegularformatter,
+                "expected": ()
+            },
+            {
+                "output": "Track Create Date               : 0000:00:00 00:00:00",
+                "formatter": VideoRegularformatter,
+                "expected": ()
+            },
+            {
+                "output": "Track Create Date               : 0000:00:00 00:00:00",
+                "formatter": AVIformatter,
+                "expected": ()
+            },
+            {
+                "output": "Track Create Date               : 0000:00:00 00:00:00",
+                "formatter": ImageRegularformatter,
+                "expected": ()
+            },
+            {
+                "output": "Date/Time Original                    : 2023:07:16 17:13:57",
+                "formatter": VideoRegularformatter,
+                "expected": ()
+            },
+            {
+                "output": "Date/Time Original                    : 2023:07:16 17:13:57",
+                "formatter": AVIformatter,
+                "expected": ()
+            },
+            {
+                "output": "Date/Time Original                    : 2023:07:16 17:13:57",
+                "formatter": ImageRegularformatter,
+                "expected": ("2023", "07", "16", "17", "13", "57")
+            },
+        ]
+        for i in range(0, len(samples)):
+            actual = samples[i]["formatter"](samples[i]["output"]).getGroups()
+            self.assertEqual(actual, samples[i]["expected"], f"Error in {samples[i]}")
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `cmn-1.9.0/src/cmn/__main__.py` & `cmn-2.0.0/cmn/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,75 @@
-"""
-Main - Module responsible for the main program. Parses the arguments and calls the other modules.
-"""
-__version__ = "1.9.0"
-
-import argparse
-from datetime import datetime
-
-from src.ColoredLogger.ColoredLogger import ColoredLogger
-from src.ChangeMediaName import ChangeMediaName
-from src.cmn import getFiletypes, getScanFiles, nameFormatter
-
-logger = ColoredLogger()
-
-
-def main():
-    global logger
-    parser = argparse.ArgumentParser(
-        description="Program to scan multimedia files and rename them to their creation date.")
-    parser.add_argument("-i", "--input-files", nargs="+", required=True, help="File(s) or folder(s) to scan")
-    parser.add_argument("-v", "--verbose", action="store_true", default=False, help="Verbose mode")
-    parser.add_argument("-r", "--recursive", action="store_true", help="Scan folders recursively", default=False)
-    parser.add_argument("-ni", "--ignored-paths", nargs="*", help="Files or folders to be ignored", default=[])
-    parser.add_argument("-nr", "--not-ignore-subfolders", action="store_false", default=True,
-                        help="Choose to not ignore subfolders of the ignored paths")
-    parser.add_argument("-t", "--file-types", nargs="*", default=[], help="List of file types to consider")
-    parser.add_argument("-nt", "--not-file-types", nargs="*", default=[], help="List of file types to ignore")
-    parser.add_argument("-oi", "--only-images", action="store_true", help="Consider only images", default=False)
-    parser.add_argument("-ov", "--only-videos", action="store_true", help="Consider only videos", default=False)
-    parser.add_argument("-cf", "--create-new-folders", action="store_true", default=False,
-                        help="Create new folders according to the new image names")
-    parser.add_argument("-fn", "--name-format", default="%Y%m%d_%H%M%S", help="Format of the new names")
-    parser.add_argument("-ff", "--name-folder-format", default="%Y - %m - %d", help="Format of the new folder names")
-
-    args = parser.parse_args()
-
-    logger = ColoredLogger(args.verbose)
-    initialTimer = datetime.now()
-    logger.debug("Program started.")
-
-    if not nameFormatter(args.name_format, "") or not nameFormatter(args.name_folder_format, "folder "):
-        return
-
-    filetypes = getFiletypes(args.file_types, args.only_images, args.only_videos, args.not_file_types)
-    files = getScanFiles(args.input_files, args.recursive, args.ignored_paths, args.not_ignore_subfolders, filetypes)
-
-    nChanged, nErrors = ChangeMediaName.cmn(logger, files, args.create_new_folders, args.name_format,
-                                            args.name_folder_format)
-    nProcessed = len(files)
-    endTimer = datetime.now()
-    logger.info(f"Processed {nProcessed} file{'s' if nProcessed != 1 else ''} in {endTimer - initialTimer}.")
-    logger.info(f"Changed {nChanged} file{'s' if nChanged != 1 else ''}.")
-    logger.info(f"Errors: {nErrors}.")
-    logger.info("Program finished.")
-
-
-if __name__ == "__main__":
-    main()
+"""
+Main - Module responsible for the main program. Parses the arguments and calls the other modules.
+"""
+__version__ = "2.0.0"
+
+import argparse
+from datetime import datetime
+
+from cmn.colored_logger.colored_logger import ColoredLogger
+from cmn.change_media_name.change_media_name import cmn
+from cmn import get_filetypes, get_scan_files, name_formatter
+
+
+def main():
+    """Main function of the program"""
+    logger = ColoredLogger()
+    parser = argparse.ArgumentParser(
+        description="Program to scan multimedia files and rename them to their creation date.")
+    parser.add_argument("-i", "--input-files", nargs="+", required=True,
+                        help="File(s) or folder(s) to scan")
+    parser.add_argument("-v", "--verbose", action="store_true", default=False, help="Verbose mode")
+    parser.add_argument("-r", "--recursive", action="store_true", default=False,
+                        help="Scan folders recursively")
+    parser.add_argument("-ni", "--ignored-paths", nargs="*", default=[],
+                        help="Files or folders to be ignored")
+    parser.add_argument("-nr", "--not-ignore-subfolders", action="store_false", default=True,
+                        help="Choose to not ignore subfolders of the ignored paths")
+    parser.add_argument("-t", "--file-types", nargs="*", default=[],
+                        help="List of file types to consider")
+    parser.add_argument("-nt", "--not-file-types", nargs="*", default=[],
+                        help="List of file types to ignore")
+    parser.add_argument("-oi", "--only-images", action="store_true",
+                        help="Consider only images", default=False)
+    parser.add_argument("-ov", "--only-videos", action="store_true",
+                        help="Consider only videos", default=False)
+    parser.add_argument("-cf", "--create-new-folders", action="store_true", default=False,
+                        help="Create new folders according to the new image names")
+    parser.add_argument("-fn", "--name-format", default="%Y%m%d_%H%M%S",
+                        help="Format of the new names")
+    parser.add_argument("-ff", "--name-folder-format", default="%Y - %m - %d",
+                        help="Format of the new folder names")
+
+    args = parser.parse_args()
+
+    logger = ColoredLogger(args.verbose)
+    initial_timer = datetime.now()
+    logger.debug("Program started.")
+
+    if (
+            not name_formatter(args.name_format, "") or
+            not name_formatter(args.name_folder_format, "folder ")
+    ):
+        return
+
+    filetypes = get_filetypes(
+        args.file_types, args.only_images, args.only_videos, args.not_file_types
+    )
+    files = get_scan_files(
+        args.input_files, args.recursive, args.ignored_paths, args.not_ignore_subfolders, filetypes
+    )
+
+    n_changed, n_errors = cmn(
+        logger, files, args.create_new_folders, args.name_format, args.name_folder_format
+    )
+    n_processed = len(files)
+    end_timer = datetime.now()
+    logger.info(f"Processed {n_processed} file"
+                f"{'s' if n_processed != 1 else ''} in {end_timer - initial_timer}.")
+    logger.info(f"Changed {n_changed} file{'s' if n_changed != 1 else ''}.")
+    logger.info(f"Errors: {n_errors}.")
+    logger.info("Program finished.")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `cmn-1.9.0/PKG-INFO` & `cmn-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: cmn
-Version: 1.9.0
+Version: 2.0.0
 Summary: Main - Module responsible for the main program. Parses the arguments and calls the other modules.
 Author-email: Henrique Alvelos <henriquealvelos@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: colorama >= 0.4.6
 Project-URL: Home, https://github.com/Henrique-190/CMN
 
 # ChangeMediaName
 Tool that changes media files to its creation date.
 
+## Installation
+```
+pip install cmn
+```
+
 ## Usage
 ```
-python3 ChangeMediaName.py -i <paths>
+cmn -i <input-files> [options]
 ```
 
 ## Options
 
 | Option 1 | Option 2              | Description                                                           |
 |----------|-----------------------|-----------------------------------------------------------------------|
 | h        | help                  | Show this help message and exit                                       |
@@ -28,16 +33,16 @@
 | ni       | ignored-paths         | Default: `None`. Files or folders to be ignored                       |
 | nr       | not-ignore-subfolders | Default: `True`. Choose to not ignore subfolders of the ignored paths |
 | t        | file-types            | Default: `None`. List of file types to consider                       |
 | nt       | not-file-types        | Default: `None`. List of file types to ignore                         |
 | of       | only-images           | Default: `False`. Consider only images                                |
 | ov       | only-videos           | Default: `False`. Consider only videos                                |
 | cf       | create-new-folders    | Default: `False`. Create new folders according to the new image names |
-| fn       | name-format           | Default:`%Y%m%d_%H%M%S` Format of the new names                       |
-| ff       | name-folder-format    | Default:`%Y - %m - %d`. Format of the new folder names                |
+| fn       | name-format           | Default: `%Y%m%d_%H%M%S`. Format of the new names                     |
+| ff       | name-folder-format    | Default: `%Y - %m - %d`. Format of the new folder names               |
 
 
 ## Supported file types
 | Type  | Extension | Name                                         |
 |-------|-----------|----------------------------------------------|
 | Image | HEIC      | High Efficiency Image File Format            |
 | Image | JPEG      | Joint Photographic Experts Group File Format |
@@ -47,9 +52,7 @@
 | Video | AVI       | Audio Video Interleave                       |
 | Video | AVI       | Audio Video Interleave                       |
 | Video | MP4       | MPEG-4 Part 14                               |
 
 ## Requirements
 - Install `exiftool` command from https://exiftool.org/. Credits to Phil Harvey.
 
-## Made by me :)
-
```

