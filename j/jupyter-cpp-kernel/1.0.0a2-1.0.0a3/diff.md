# Comparing `tmp/jupyter_cpp_kernel-1.0.0a2.tar.gz` & `tmp/jupyter_cpp_kernel-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_cpp_kernel-1.0.0a2.tar", last modified: Sat Jul 15 03:31:05 2023, max compression
+gzip compressed data, was "jupyter_cpp_kernel-1.0.0a3.tar", last modified: Tue Aug  8 17:13:48 2023, max compression
```

## Comparing `jupyter_cpp_kernel-1.0.0a2.tar` & `jupyter_cpp_kernel-1.0.0a3.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-15 03:31:05.681646 jupyter_cpp_kernel-1.0.0a2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2023-07-14 12:37:56.000000 jupyter_cpp_kernel-1.0.0a2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       78 2023-07-14 12:37:56.000000 jupyter_cpp_kernel-1.0.0a2/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5261 2023-07-15 03:31:05.681646 jupyter_cpp_kernel-1.0.0a2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4693 2023-07-14 12:37:56.000000 jupyter_cpp_kernel-1.0.0a2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-15 03:31:05.673646 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-14 12:38:47.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      126 2023-07-14 12:37:56.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2029 2023-07-14 15:06:07.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/install_cpp_kernel
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10269 2023-07-15 03:21:38.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/kernel.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-15 03:31:05.677646 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/resources/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      921 2023-07-14 15:09:07.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel/resources/master.cpp
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-15 03:31:05.677646 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5261 2023-07-15 03:31:05.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      400 2023-07-15 03:31:05.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-15 03:31:05.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2023-07-15 03:31:05.000000 jupyter_cpp_kernel-1.0.0a2/jupyter_cpp_kernel.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-07-14 12:37:56.000000 jupyter_cpp_kernel-1.0.0a2/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      764 2023-07-15 03:31:05.685646 jupyter_cpp_kernel-1.0.0a2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      657 2023-07-14 15:02:37.000000 jupyter_cpp_kernel-1.0.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:13:48.597483 jupyter_cpp_kernel-1.0.0a3/
+-rw-rw-rw-   0        0        0     1090 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5130 2023-08-08 17:13:48.597483 jupyter_cpp_kernel-1.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     4331 2023-08-08 16:39:05.000000 jupyter_cpp_kernel-1.0.0a3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 17:13:48.584851 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/
+-rw-rw-rw-   0        0        0        0 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/__main__.py
+-rw-rw-rw-   0        0        0    10762 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/kernel.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:13:48.591170 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/resources/
+-rw-rw-rw-   0        0        0     3320 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/resources/dlfcn.h
+-rw-rw-rw-   0        0        0     1203 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel/resources/master.cpp
+drwxrwxrwx   0        0        0        0 2023-08-08 17:13:48.589163 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel.egg-info/
+-rw-rw-rw-   0        0        0     5130 2023-08-08 17:13:48.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-08-08 17:13:48.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 17:13:48.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-08 17:13:48.000000 jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 17:13:48.596484 jupyter_cpp_kernel-1.0.0a3/kernel_spec/
+-rw-rw-rw-   0        0        0      191 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/kernel_spec/kernel.json
+-rw-rw-rw-   0        0        0     5218 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/kernel_spec/logo-32x32.png
+-rw-rw-rw-   0        0        0    19133 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/kernel_spec/logo-64x64.png
+-rw-rw-rw-   0        0        0     1919 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/kernel_spec/logo-svg.svg
+-rw-rw-rw-   0        0        0      111 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0      791 2023-08-08 17:13:48.598483 jupyter_cpp_kernel-1.0.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-08-08 16:37:24.000000 jupyter_cpp_kernel-1.0.0a3/setup.py
```

### Comparing `jupyter_cpp_kernel-1.0.0a2/LICENSE` & `jupyter_cpp_kernel-1.0.0a3/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 @takinekotfs
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 @takinekotfs
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `jupyter_cpp_kernel-1.0.0a2/PKG-INFO` & `jupyter_cpp_kernel-1.0.0a3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,215 +1,211 @@
-Metadata-Version: 2.1
-Name: jupyter_cpp_kernel
-Version: 1.0.0a2
-Summary: C++ 14 kernel for Jupyter
-Home-page: https://github.com/takinekotfs/jupyter-cpp-kernel
-Download-URL: https://github.com/takinekotfs/jupyter-cpp-kernel
-Author: Tsuki Takineko
-Author-email: systakineko.tfs@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/takinekotfs/jupyter-cpp-kernel/issues
-Keywords: jupyter,cpp,cpp14,jupyter-kernels,pip
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-```markdown
-This repo is originally created by Brendan Rius - `C Kernel for Jupyter`
-
-You can see the original project at https://github.com/brendan-rius/jupyter-c-kernel
-
-Plus, this C++ kernel only uses C++ 14. The others are being developed
-(or not, who knows 😅)
-```
-
-[![CodeQL](https://github.com/takinekotfs/jupyter-cpp-kernel/actions/workflows/codeql.yml/badge.svg)](https://github.com/takinekotfs/jupyter-cpp-kernel/actions/workflows/codeql.yml)
-
-# C++ 14 kernel for Jupyter
-
-## Installation
-
-> :warning:
->
-> This kernel only works on Linux and macOS.
-> If you want to use it on Windows, please consider using [WSL](https://aka.ms/wsl), [Docker](https://docker.com), or using a virtual machine.
-
-Normally, your target machine must meet these requirement packages before installing and using `jupyter-cpp-kernel`.
-
-* `g++`
-* `python3`, `python3-pip`
-* `jupyter` (recommend `jupyterlab`)
-
-### Install from PyPI
-
-#### Installing on macOS
-
-> :warning:
->
-> You must all requirements above before doing anything else
-> I don't use macOS too regularly, so I don't know how macOS get these packages
-> But you can follow installation instructions on the Internet
-> After that, you can copy this script and install the kernel
-
-```shell
-pip install jupyter-cpp-kernel
-install_cpp_kernel --user
-```
-
-#### Installing on Debian/Ubuntu
-
-```shell
-sudo apt update && sudo apt full-upgrade -y 
-sudo apt install -y g++
-sudo apt install -y python3 python3-pip
-sudo pip install --upgrade pip
-sudo pip install jupyter # Or jupyterlab. Using `sudo` to install to the main packge
-sudo pip install jupyter-cpp-kernel # Can be `sudo`, but using it with caution. Only for large deployment Jupyter server
-install_cpp_kernel --user # Can be `sudo`, but using it with caution. Only for large deployment Jupyter server
-```
-
-### Install from GitHub repo
-
-#### Installing on macOS
-
-> :warning:
->
-> You must all requirements above before doing anything else
-> I don't use macOS too regularly, so I don't know how macOS get these packages
-> But you can follow installation instructions on the Internet
-> After that, you can copy this script and install the kernel
-
-```shell
-pip install git+https://github.com/takinekotfs/jupyter-cpp-kernel.git
-install_cpp_kernel --user
-```
-
-#### Installing on Debian/Ubuntu
-
-```shell
-sudo apt update && sudo apt full-upgrade -y 
-sudo apt install -y g++
-sudo apt install -y python3 python3-pip
-sudo pip install --upgrade pip
-sudo pip install jupyter # Or jupyterlab. Using `sudo` to install to the main packge
-sudo pip install git+https://github.com/takinekotfs/jupyter-cpp-kernel.git 
-install_cpp_kernel --user # Can be `sudo`, but using it with caution. Only for large deployment Jupyter server
-```
-
-## Contributing
-
-You can clone, create a fork or import this repo whenever you want.
-
-Please follow the GitHub standards and the license
-
-## Sample codes
-
-> :warning:
->
-> - Raw input into program is still not completed yet. You may `cannot` using `cin` or any user input parameter.
->
-> - For the best practices, you shouldn't write `using namespace std;` because of the conflicts between the `namespace`. This problem doesn't come from the interpreter, it's actually the problem of `g++` globally
-
-### Hello world
-
-```cpp
-#include <iostream>
-
-int main() {
-    std::cout << "Hello World" << std::endl;
-    return 0;
-}
-```
-
-### Declare variable (`int`) and take a math of them
-
-```cpp
-#include <iostream>
-#include <cmath>
-
-int main() {
-    int x = 3, y = 6;
-    std::cout << "Sum of x and y is " << x + y << std::endl;
-    std::cout << "Subtract of x and y is " << x - y << std::endl;
-    return 0;
-}
-```
-
-### Condition
-
-#### With `If...else...`
-
-```cpp
-#include <iostream>
-
-int main() {
-    bool isMale = false;
-    if (isMale) {
-        std::cout << "Male" << std::endl;
-    }
-    else {
-        std::cout << "Is not Male" << std::endl;
-    }
-    return 0;
-}
-```
-
-#### With `switch...case...`
-
-```cpp
-#include <iostream>
-
-int main() {
-    int number = 1;
-    switch (number) {
-        case 1:
-            std::cout << "1" << std::endl;
-        case 2:
-            std::cout << "2" << std::endl;
-        default:
-            std::cout << "Not defined" << std::endl;
-    }
-    return 0;
-}
-```
-
-### Loop
-
-#### For float condition
-
-```cpp
-#include <iostream>
-
-int main() {
-    int lim = 10;
-    for (int i = 0; i < lim; i++) {
-        std::cout << i << std::endl;
-    }
-    return 0;
-}
-```
-
-#### For fixed condition
-
-```cpp
-#include <iostream>
-
-int main() {
-    int lim = 0;
-    while (lim < 10) {
-        std::cout << lim << std::endl;
-        lim++;
-    }
-    return 0;
-}
-```
-
-### Exception handler
-
-```cpp
-#include <iostream>
-
-int main() {
-    std::cerr << "Exception happened";
-}
-```
+Metadata-Version: 2.1
+Name: jupyter_cpp_kernel
+Version: 1.0.0a3
+Summary: C++ 14 kernel for Jupyter
+Home-page: https://github.com/takinekotfs/jupyter-cpp-kernel
+Download-URL: https://github.com/takinekotfs/jupyter-cpp-kernel
+Author: Tsuki Takineko
+Author-email: systakineko.tfs@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/takinekotfs/jupyter-cpp-kernel/issues
+Keywords: jupyter,cpp,cpp14,jupyter-kernels,pip
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C++
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+```markdown
+This repo is originally created by Brendan Rius - `C Kernel for Jupyter`
+
+You can see the original project at https://github.com/brendan-rius/jupyter-c-kernel
+
+Plus, this C++ kernel only uses C++ 14. The others are being developed
+(or not, who knows 😅)
+```
+
+[![CodeQL](https://github.com/takinekotfs/jupyter-cpp-kernel/actions/workflows/codeql.yml/badge.svg)](https://github.com/takinekotfs/jupyter-cpp-kernel/actions/workflows/codeql.yml)
+
+# C++ 14 kernel for Jupyter
+
+## Installation
+
+> :warning:
+>
+> If you want to use it on Windows, please installing the [GNU Compiler Collection for Windows](https://github.com/takinekotfs/jupyter-cpp-kernel/releases/tag/gcc-13.2.0)
+
+Normally, your target machine must meet these requirement packages before installing and using `jupyter-cpp-kernel`.
+
+* `g++`
+* `python3`, `python3-pip`
+* `jupyter` (recommend `jupyterlab`)
+
+### Install from PyPI
+
+#### Installing on macOS and Windows
+
+> :warning:
+>
+> You must all requirements above before doing anything else.
+> After that, you can copy this script and install the kernel
+
+```shell
+pip install jupyter-cpp-kernel
+```
+
+#### Installing on Debian/Ubuntu
+
+```shell
+sudo apt update && sudo apt full-upgrade -y 
+sudo apt install -y g++
+sudo apt install -y python3 python3-pip
+sudo pip install --upgrade pip
+sudo pip install jupyter # Or jupyterlab. Using `sudo` to install to the main packge
+sudo pip install jupyter-cpp-kernel # Can be `sudo`, but using it with caution. Only for large deployment Jupyter server
+```
+
+### Install from GitHub repo
+
+#### Installing on macOS and Windows
+
+> :warning:
+>
+> You must all requirements above before doing anything else.\
+> After that, you can copy this script and install the kernel
+
+```shell
+pip install git+https://github.com/takinekotfs/jupyter-cpp-kernel.git
+```
+
+#### Installing on Debian/Ubuntu
+
+```shell
+sudo apt update && sudo apt full-upgrade -y 
+sudo apt install -y g++
+sudo apt install -y python3 python3-pip
+sudo pip install --upgrade pip
+sudo pip install jupyter # Or jupyterlab. Using `sudo` to install to the main packge
+sudo pip install git+https://github.com/takinekotfs/jupyter-cpp-kernel.git 
+```
+
+## Contributing
+
+You can clone, create a fork or import this repo whenever you want.
+
+Please follow the GitHub standards and the license
+
+## Sample codes
+
+> :warning:
+>
+> - Raw input into program is still not completed yet. You may cannot using `cin` or any user input parameter.
+>
+> - For the best practices, you shouldn't write `using namespace std;` because of the conflicts between the `namespace`. This problem doesn't come from the interpreter, it's actually the problem of `g++` globally
+
+### Hello world
+
+```cpp
+#include <iostream>
+
+int main() {
+    std::cout << "Hello World" << std::endl;
+    return 0;
+}
+```
+
+### Declare variable (`int`) and take a math of them
+
+```cpp
+#include <iostream>
+#include <cmath>
+
+int main() {
+    int x = 3, y = 6;
+    std::cout << "Sum of x and y is " << x + y << std::endl;
+    std::cout << "Subtract of x and y is " << x - y << std::endl;
+    return 0;
+}
+```
+
+### Condition
+
+#### With `If...else...`
+
+```cpp
+#include <iostream>
+
+int main() {
+    bool isMale = false;
+    if (isMale) {
+        std::cout << "Male" << std::endl;
+    }
+    else {
+        std::cout << "Is not Male" << std::endl;
+    }
+    return 0;
+}
+```
+
+#### With `switch...case...`
+
+```cpp
+#include <iostream>
+
+int main() {
+    int number = 1;
+    switch (number) {
+        case 1:
+            std::cout << "1" << std::endl;
+        case 2:
+            std::cout << "2" << std::endl;
+        default:
+            std::cout << "Not defined" << std::endl;
+    }
+    return 0;
+}
+```
+
+### Loop
+
+#### For float condition
+
+```cpp
+#include <iostream>
+
+int main() {
+    int lim = 10;
+    for (int i = 0; i < lim; i++) {
+        std::cout << i << std::endl;
+    }
+    return 0;
+}
+```
+
+#### For fixed condition
+
+```cpp
+#include <iostream>
+
+int main() {
+    int lim = 0;
+    while (lim < 10) {
+        std::cout << lim << std::endl;
+        lim++;
+    }
+    return 0;
+}
+```
+
+### Exception handler
+
+```cpp
+#include <iostream>
+
+int main() {
+    std::cerr << "Exception happened";
+}
+```
```

### Comparing `jupyter_cpp_kernel-1.0.0a2/README.md` & `jupyter_cpp_kernel-1.0.0a3/jupyter_cpp_kernel.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,294 +1,321 @@
-00000000: 6060 606d 6172 6b64 6f77 6e0a 5468 6973  ```markdown.This
-00000010: 2072 6570 6f20 6973 206f 7269 6769 6e61   repo is origina
-00000020: 6c6c 7920 6372 6561 7465 6420 6279 2042  lly created by B
-00000030: 7265 6e64 616e 2052 6975 7320 2d20 6043  rendan Rius - `C
-00000040: 204b 6572 6e65 6c20 666f 7220 4a75 7079   Kernel for Jupy
-00000050: 7465 7260 0a0a 596f 7520 6361 6e20 7365  ter`..You can se
-00000060: 6520 7468 6520 6f72 6967 696e 616c 2070  e the original p
-00000070: 726f 6a65 6374 2061 7420 6874 7470 733a  roject at https:
-00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f62 7265  //github.com/bre
-00000090: 6e64 616e 2d72 6975 732f 6a75 7079 7465  ndan-rius/jupyte
-000000a0: 722d 632d 6b65 726e 656c 0a0a 506c 7573  r-c-kernel..Plus
-000000b0: 2c20 7468 6973 2043 2b2b 206b 6572 6e65  , this C++ kerne
-000000c0: 6c20 6f6e 6c79 2075 7365 7320 432b 2b20  l only uses C++ 
-000000d0: 3134 2e20 5468 6520 6f74 6865 7273 2061  14. The others a
-000000e0: 7265 2062 6569 6e67 2064 6576 656c 6f70  re being develop
-000000f0: 6564 0a28 6f72 206e 6f74 2c20 7768 6f20  ed.(or not, who 
-00000100: 6b6e 6f77 7320 f09f 9885 290a 6060 600a  knows ....).```.
-00000110: 0a5b 215b 436f 6465 514c 5d28 6874 7470  .[![CodeQL](http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000130: 616b 696e 656b 6f74 6673 2f6a 7570 7974  akinekotfs/jupyt
-00000140: 6572 2d63 7070 2d6b 6572 6e65 6c2f 6163  er-cpp-kernel/ac
-00000150: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000160: 636f 6465 716c 2e79 6d6c 2f62 6164 6765  codeql.yml/badge
-00000170: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000180: 6974 6875 622e 636f 6d2f 7461 6b69 6e65  ithub.com/takine
-00000190: 6b6f 7466 732f 6a75 7079 7465 722d 6370  kotfs/jupyter-cp
-000001a0: 702d 6b65 726e 656c 2f61 6374 696f 6e73  p-kernel/actions
-000001b0: 2f77 6f72 6b66 6c6f 7773 2f63 6f64 6571  /workflows/codeq
-000001c0: 6c2e 796d 6c29 0a0a 2320 432b 2b20 3134  l.yml)..# C++ 14
-000001d0: 206b 6572 6e65 6c20 666f 7220 4a75 7079   kernel for Jupy
-000001e0: 7465 720a 0a23 2320 496e 7374 616c 6c61  ter..## Installa
-000001f0: 7469 6f6e 0a0a 3e20 3a77 6172 6e69 6e67  tion..> :warning
-00000200: 3a0a 3e0a 3e20 5468 6973 206b 6572 6e65  :.>.> This kerne
-00000210: 6c20 6f6e 6c79 2077 6f72 6b73 206f 6e20  l only works on 
-00000220: 4c69 6e75 7820 616e 6420 6d61 634f 532e  Linux and macOS.
-00000230: 0a3e 2049 6620 796f 7520 7761 6e74 2074  .> If you want t
-00000240: 6f20 7573 6520 6974 206f 6e20 5769 6e64  o use it on Wind
-00000250: 6f77 732c 2070 6c65 6173 6520 636f 6e73  ows, please cons
-00000260: 6964 6572 2075 7369 6e67 205b 5753 4c5d  ider using [WSL]
-00000270: 2868 7474 7073 3a2f 2f61 6b61 2e6d 732f  (https://aka.ms/
-00000280: 7773 6c29 2c20 5b44 6f63 6b65 725d 2868  wsl), [Docker](h
-00000290: 7474 7073 3a2f 2f64 6f63 6b65 722e 636f  ttps://docker.co
-000002a0: 6d29 2c20 6f72 2075 7369 6e67 2061 2076  m), or using a v
-000002b0: 6972 7475 616c 206d 6163 6869 6e65 2e0a  irtual machine..
-000002c0: 0a4e 6f72 6d61 6c6c 792c 2079 6f75 7220  .Normally, your 
-000002d0: 7461 7267 6574 206d 6163 6869 6e65 206d  target machine m
-000002e0: 7573 7420 6d65 6574 2074 6865 7365 2072  ust meet these r
-000002f0: 6571 7569 7265 6d65 6e74 2070 6163 6b61  equirement packa
-00000300: 6765 7320 6265 666f 7265 2069 6e73 7461  ges before insta
-00000310: 6c6c 696e 6720 616e 6420 7573 696e 6720  lling and using 
-00000320: 606a 7570 7974 6572 2d63 7070 2d6b 6572  `jupyter-cpp-ker
-00000330: 6e65 6c60 2e0a 0a2a 2060 672b 2b60 0a2a  nel`...* `g++`.*
-00000340: 2060 7079 7468 6f6e 3360 2c20 6070 7974   `python3`, `pyt
-00000350: 686f 6e33 2d70 6970 600a 2a20 606a 7570  hon3-pip`.* `jup
-00000360: 7974 6572 6020 2872 6563 6f6d 6d65 6e64  yter` (recommend
-00000370: 2060 6a75 7079 7465 726c 6162 6029 0a0a   `jupyterlab`)..
-00000380: 2323 2320 496e 7374 616c 6c20 6672 6f6d  ### Install from
-00000390: 2050 7950 490a 0a23 2323 2320 496e 7374   PyPI..#### Inst
-000003a0: 616c 6c69 6e67 206f 6e20 6d61 634f 530a  alling on macOS.
-000003b0: 0a3e 203a 7761 726e 696e 673a 0a3e 0a3e  .> :warning:.>.>
-000003c0: 2059 6f75 206d 7573 7420 616c 6c20 7265   You must all re
-000003d0: 7175 6972 656d 656e 7473 2061 626f 7665  quirements above
-000003e0: 2062 6566 6f72 6520 646f 696e 6720 616e   before doing an
-000003f0: 7974 6869 6e67 2065 6c73 650a 3e20 4920  ything else.> I 
-00000400: 646f 6e27 7420 7573 6520 6d61 634f 5320  don't use macOS 
-00000410: 746f 6f20 7265 6775 6c61 726c 792c 2073  too regularly, s
-00000420: 6f20 4920 646f 6e27 7420 6b6e 6f77 2068  o I don't know h
-00000430: 6f77 206d 6163 4f53 2067 6574 2074 6865  ow macOS get the
-00000440: 7365 2070 6163 6b61 6765 730a 3e20 4275  se packages.> Bu
-00000450: 7420 796f 7520 6361 6e20 666f 6c6c 6f77  t you can follow
-00000460: 2069 6e73 7461 6c6c 6174 696f 6e20 696e   installation in
-00000470: 7374 7275 6374 696f 6e73 206f 6e20 7468  structions on th
-00000480: 6520 496e 7465 726e 6574 0a3e 2041 6674  e Internet.> Aft
-00000490: 6572 2074 6861 742c 2079 6f75 2063 616e  er that, you can
-000004a0: 2063 6f70 7920 7468 6973 2073 6372 6970   copy this scrip
-000004b0: 7420 616e 6420 696e 7374 616c 6c20 7468  t and install th
-000004c0: 6520 6b65 726e 656c 0a0a 6060 6073 6865  e kernel..```she
-000004d0: 6c6c 0a70 6970 2069 6e73 7461 6c6c 206a  ll.pip install j
-000004e0: 7570 7974 6572 2d63 7070 2d6b 6572 6e65  upyter-cpp-kerne
-000004f0: 6c0a 696e 7374 616c 6c5f 6370 705f 6b65  l.install_cpp_ke
-00000500: 726e 656c 202d 2d75 7365 720a 6060 600a  rnel --user.```.
-00000510: 0a23 2323 2320 496e 7374 616c 6c69 6e67  .#### Installing
-00000520: 206f 6e20 4465 6269 616e 2f55 6275 6e74   on Debian/Ubunt
-00000530: 750a 0a60 6060 7368 656c 6c0a 7375 646f  u..```shell.sudo
-00000540: 2061 7074 2075 7064 6174 6520 2626 2073   apt update && s
-00000550: 7564 6f20 6170 7420 6675 6c6c 2d75 7067  udo apt full-upg
-00000560: 7261 6465 202d 7920 0a73 7564 6f20 6170  rade -y .sudo ap
-00000570: 7420 696e 7374 616c 6c20 2d79 2067 2b2b  t install -y g++
-00000580: 0a73 7564 6f20 6170 7420 696e 7374 616c  .sudo apt instal
-00000590: 6c20 2d79 2070 7974 686f 6e33 2070 7974  l -y python3 pyt
-000005a0: 686f 6e33 2d70 6970 0a73 7564 6f20 7069  hon3-pip.sudo pi
-000005b0: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
-000005c0: 6164 6520 7069 700a 7375 646f 2070 6970  ade pip.sudo pip
-000005d0: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
-000005e0: 2023 204f 7220 6a75 7079 7465 726c 6162   # Or jupyterlab
-000005f0: 2e20 5573 696e 6720 6073 7564 6f60 2074  . Using `sudo` t
-00000600: 6f20 696e 7374 616c 6c20 746f 2074 6865  o install to the
-00000610: 206d 6169 6e20 7061 636b 6765 0a73 7564   main packge.sud
-00000620: 6f20 7069 7020 696e 7374 616c 6c20 6a75  o pip install ju
-00000630: 7079 7465 722d 6370 702d 6b65 726e 656c  pyter-cpp-kernel
-00000640: 2023 2043 616e 2062 6520 6073 7564 6f60   # Can be `sudo`
-00000650: 2c20 6275 7420 7573 696e 6720 6974 2077  , but using it w
-00000660: 6974 6820 6361 7574 696f 6e2e 204f 6e6c  ith caution. Onl
-00000670: 7920 666f 7220 6c61 7267 6520 6465 706c  y for large depl
-00000680: 6f79 6d65 6e74 204a 7570 7974 6572 2073  oyment Jupyter s
-00000690: 6572 7665 720a 696e 7374 616c 6c5f 6370  erver.install_cp
-000006a0: 705f 6b65 726e 656c 202d 2d75 7365 7220  p_kernel --user 
-000006b0: 2320 4361 6e20 6265 2060 7375 646f 602c  # Can be `sudo`,
-000006c0: 2062 7574 2075 7369 6e67 2069 7420 7769   but using it wi
-000006d0: 7468 2063 6175 7469 6f6e 2e20 4f6e 6c79  th caution. Only
-000006e0: 2066 6f72 206c 6172 6765 2064 6570 6c6f   for large deplo
-000006f0: 796d 656e 7420 4a75 7079 7465 7220 7365  yment Jupyter se
-00000700: 7276 6572 0a60 6060 0a0a 2323 2320 496e  rver.```..### In
-00000710: 7374 616c 6c20 6672 6f6d 2047 6974 4875  stall from GitHu
-00000720: 6220 7265 706f 0a0a 2323 2323 2049 6e73  b repo..#### Ins
-00000730: 7461 6c6c 696e 6720 6f6e 206d 6163 4f53  talling on macOS
-00000740: 0a0a 3e20 3a77 6172 6e69 6e67 3a0a 3e0a  ..> :warning:.>.
-00000750: 3e20 596f 7520 6d75 7374 2061 6c6c 2072  > You must all r
-00000760: 6571 7569 7265 6d65 6e74 7320 6162 6f76  equirements abov
-00000770: 6520 6265 666f 7265 2064 6f69 6e67 2061  e before doing a
-00000780: 6e79 7468 696e 6720 656c 7365 0a3e 2049  nything else.> I
-00000790: 2064 6f6e 2774 2075 7365 206d 6163 4f53   don't use macOS
-000007a0: 2074 6f6f 2072 6567 756c 6172 6c79 2c20   too regularly, 
-000007b0: 736f 2049 2064 6f6e 2774 206b 6e6f 7720  so I don't know 
-000007c0: 686f 7720 6d61 634f 5320 6765 7420 7468  how macOS get th
-000007d0: 6573 6520 7061 636b 6167 6573 0a3e 2042  ese packages.> B
-000007e0: 7574 2079 6f75 2063 616e 2066 6f6c 6c6f  ut you can follo
-000007f0: 7720 696e 7374 616c 6c61 7469 6f6e 2069  w installation i
-00000800: 6e73 7472 7563 7469 6f6e 7320 6f6e 2074  nstructions on t
-00000810: 6865 2049 6e74 6572 6e65 740a 3e20 4166  he Internet.> Af
-00000820: 7465 7220 7468 6174 2c20 796f 7520 6361  ter that, you ca
-00000830: 6e20 636f 7079 2074 6869 7320 7363 7269  n copy this scri
-00000840: 7074 2061 6e64 2069 6e73 7461 6c6c 2074  pt and install t
-00000850: 6865 206b 6572 6e65 6c0a 0a60 6060 7368  he kernel..```sh
-00000860: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
-00000870: 6769 742b 6874 7470 733a 2f2f 6769 7468  git+https://gith
-00000880: 7562 2e63 6f6d 2f74 616b 696e 656b 6f74  ub.com/takinekot
-00000890: 6673 2f6a 7570 7974 6572 2d63 7070 2d6b  fs/jupyter-cpp-k
-000008a0: 6572 6e65 6c2e 6769 740a 696e 7374 616c  ernel.git.instal
-000008b0: 6c5f 6370 705f 6b65 726e 656c 202d 2d75  l_cpp_kernel --u
-000008c0: 7365 720a 6060 600a 0a23 2323 2320 496e  ser.```..#### In
-000008d0: 7374 616c 6c69 6e67 206f 6e20 4465 6269  stalling on Debi
-000008e0: 616e 2f55 6275 6e74 750a 0a60 6060 7368  an/Ubuntu..```sh
-000008f0: 656c 6c0a 7375 646f 2061 7074 2075 7064  ell.sudo apt upd
-00000900: 6174 6520 2626 2073 7564 6f20 6170 7420  ate && sudo apt 
-00000910: 6675 6c6c 2d75 7067 7261 6465 202d 7920  full-upgrade -y 
-00000920: 0a73 7564 6f20 6170 7420 696e 7374 616c  .sudo apt instal
-00000930: 6c20 2d79 2067 2b2b 0a73 7564 6f20 6170  l -y g++.sudo ap
-00000940: 7420 696e 7374 616c 6c20 2d79 2070 7974  t install -y pyt
-00000950: 686f 6e33 2070 7974 686f 6e33 2d70 6970  hon3 python3-pip
-00000960: 0a73 7564 6f20 7069 7020 696e 7374 616c  .sudo pip instal
-00000970: 6c20 2d2d 7570 6772 6164 6520 7069 700a  l --upgrade pip.
-00000980: 7375 646f 2070 6970 2069 6e73 7461 6c6c  sudo pip install
-00000990: 206a 7570 7974 6572 2023 204f 7220 6a75   jupyter # Or ju
-000009a0: 7079 7465 726c 6162 2e20 5573 696e 6720  pyterlab. Using 
-000009b0: 6073 7564 6f60 2074 6f20 696e 7374 616c  `sudo` to instal
-000009c0: 6c20 746f 2074 6865 206d 6169 6e20 7061  l to the main pa
-000009d0: 636b 6765 0a73 7564 6f20 7069 7020 696e  ckge.sudo pip in
-000009e0: 7374 616c 6c20 6769 742b 6874 7470 733a  stall git+https:
-000009f0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 616b  //github.com/tak
-00000a00: 696e 656b 6f74 6673 2f6a 7570 7974 6572  inekotfs/jupyter
-00000a10: 2d63 7070 2d6b 6572 6e65 6c2e 6769 7420  -cpp-kernel.git 
-00000a20: 0a69 6e73 7461 6c6c 5f63 7070 5f6b 6572  .install_cpp_ker
-00000a30: 6e65 6c20 2d2d 7573 6572 2023 2043 616e  nel --user # Can
-00000a40: 2062 6520 6073 7564 6f60 2c20 6275 7420   be `sudo`, but 
-00000a50: 7573 696e 6720 6974 2077 6974 6820 6361  using it with ca
-00000a60: 7574 696f 6e2e 204f 6e6c 7920 666f 7220  ution. Only for 
-00000a70: 6c61 7267 6520 6465 706c 6f79 6d65 6e74  large deployment
-00000a80: 204a 7570 7974 6572 2073 6572 7665 720a   Jupyter server.
-00000a90: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
-00000aa0: 7469 6e67 0a0a 596f 7520 6361 6e20 636c  ting..You can cl
-00000ab0: 6f6e 652c 2063 7265 6174 6520 6120 666f  one, create a fo
-00000ac0: 726b 206f 7220 696d 706f 7274 2074 6869  rk or import thi
-00000ad0: 7320 7265 706f 2077 6865 6e65 7665 7220  s repo whenever 
-00000ae0: 796f 7520 7761 6e74 2e0a 0a50 6c65 6173  you want...Pleas
-00000af0: 6520 666f 6c6c 6f77 2074 6865 2047 6974  e follow the Git
-00000b00: 4875 6220 7374 616e 6461 7264 7320 616e  Hub standards an
-00000b10: 6420 7468 6520 6c69 6365 6e73 650a 0a23  d the license..#
-00000b20: 2320 5361 6d70 6c65 2063 6f64 6573 0a0a  # Sample codes..
-00000b30: 3e20 3a77 6172 6e69 6e67 3a0a 3e0a 3e20  > :warning:.>.> 
-00000b40: 2d20 5261 7720 696e 7075 7420 696e 746f  - Raw input into
-00000b50: 2070 726f 6772 616d 2069 7320 7374 696c   program is stil
-00000b60: 6c20 6e6f 7420 636f 6d70 6c65 7465 6420  l not completed 
-00000b70: 7965 742e 2059 6f75 206d 6179 2060 6361  yet. You may `ca
-00000b80: 6e6e 6f74 6020 7573 696e 6720 6063 696e  nnot` using `cin
-00000b90: 6020 6f72 2061 6e79 2075 7365 7220 696e  ` or any user in
-00000ba0: 7075 7420 7061 7261 6d65 7465 722e 0a3e  put parameter..>
-00000bb0: 0a3e 202d 2046 6f72 2074 6865 2062 6573  .> - For the bes
-00000bc0: 7420 7072 6163 7469 6365 732c 2079 6f75  t practices, you
-00000bd0: 2073 686f 756c 646e 2774 2077 7269 7465   shouldn't write
-00000be0: 2060 7573 696e 6720 6e61 6d65 7370 6163   `using namespac
-00000bf0: 6520 7374 643b 6020 6265 6361 7573 6520  e std;` because 
-00000c00: 6f66 2074 6865 2063 6f6e 666c 6963 7473  of the conflicts
-00000c10: 2062 6574 7765 656e 2074 6865 2060 6e61   between the `na
-00000c20: 6d65 7370 6163 6560 2e20 5468 6973 2070  mespace`. This p
-00000c30: 726f 626c 656d 2064 6f65 736e 2774 2063  roblem doesn't c
-00000c40: 6f6d 6520 6672 6f6d 2074 6865 2069 6e74  ome from the int
-00000c50: 6572 7072 6574 6572 2c20 6974 2773 2061  erpreter, it's a
-00000c60: 6374 7561 6c6c 7920 7468 6520 7072 6f62  ctually the prob
-00000c70: 6c65 6d20 6f66 2060 672b 2b60 2067 6c6f  lem of `g++` glo
-00000c80: 6261 6c6c 790a 0a23 2323 2048 656c 6c6f  bally..### Hello
-00000c90: 2077 6f72 6c64 0a0a 6060 6063 7070 0a23   world..```cpp.#
-00000ca0: 696e 636c 7564 6520 3c69 6f73 7472 6561  include <iostrea
-00000cb0: 6d3e 0a0a 696e 7420 6d61 696e 2829 207b  m>..int main() {
-00000cc0: 0a20 2020 2073 7464 3a3a 636f 7574 203c  .    std::cout <
-00000cd0: 3c20 2248 656c 6c6f 2057 6f72 6c64 2220  < "Hello World" 
-00000ce0: 3c3c 2073 7464 3a3a 656e 646c 3b0a 2020  << std::endl;.  
-00000cf0: 2020 7265 7475 726e 2030 3b0a 7d0a 6060    return 0;.}.``
-00000d00: 600a 0a23 2323 2044 6563 6c61 7265 2076  `..### Declare v
-00000d10: 6172 6961 626c 6520 2860 696e 7460 2920  ariable (`int`) 
-00000d20: 616e 6420 7461 6b65 2061 206d 6174 6820  and take a math 
-00000d30: 6f66 2074 6865 6d0a 0a60 6060 6370 700a  of them..```cpp.
-00000d40: 2369 6e63 6c75 6465 203c 696f 7374 7265  #include <iostre
-00000d50: 616d 3e0a 2369 6e63 6c75 6465 203c 636d  am>.#include <cm
-00000d60: 6174 683e 0a0a 696e 7420 6d61 696e 2829  ath>..int main()
-00000d70: 207b 0a20 2020 2069 6e74 2078 203d 2033   {.    int x = 3
-00000d80: 2c20 7920 3d20 363b 0a20 2020 2073 7464  , y = 6;.    std
-00000d90: 3a3a 636f 7574 203c 3c20 2253 756d 206f  ::cout << "Sum o
-00000da0: 6620 7820 616e 6420 7920 6973 2022 203c  f x and y is " <
-00000db0: 3c20 7820 2b20 7920 3c3c 2073 7464 3a3a  < x + y << std::
-00000dc0: 656e 646c 3b0a 2020 2020 7374 643a 3a63  endl;.    std::c
-00000dd0: 6f75 7420 3c3c 2022 5375 6274 7261 6374  out << "Subtract
-00000de0: 206f 6620 7820 616e 6420 7920 6973 2022   of x and y is "
-00000df0: 203c 3c20 7820 2d20 7920 3c3c 2073 7464   << x - y << std
-00000e00: 3a3a 656e 646c 3b0a 2020 2020 7265 7475  ::endl;.    retu
-00000e10: 726e 2030 3b0a 7d0a 6060 600a 0a23 2323  rn 0;.}.```..###
-00000e20: 2043 6f6e 6469 7469 6f6e 0a0a 2323 2323   Condition..####
-00000e30: 2057 6974 6820 6049 662e 2e2e 656c 7365   With `If...else
-00000e40: 2e2e 2e60 0a0a 6060 6063 7070 0a23 696e  ...`..```cpp.#in
-00000e50: 636c 7564 6520 3c69 6f73 7472 6561 6d3e  clude <iostream>
-00000e60: 0a0a 696e 7420 6d61 696e 2829 207b 0a20  ..int main() {. 
-00000e70: 2020 2062 6f6f 6c20 6973 4d61 6c65 203d     bool isMale =
-00000e80: 2066 616c 7365 3b0a 2020 2020 6966 2028   false;.    if (
-00000e90: 6973 4d61 6c65 2920 7b0a 2020 2020 2020  isMale) {.      
-00000ea0: 2020 7374 643a 3a63 6f75 7420 3c3c 2022    std::cout << "
-00000eb0: 4d61 6c65 2220 3c3c 2073 7464 3a3a 656e  Male" << std::en
-00000ec0: 646c 3b0a 2020 2020 7d0a 2020 2020 656c  dl;.    }.    el
-00000ed0: 7365 207b 0a20 2020 2020 2020 2073 7464  se {.        std
-00000ee0: 3a3a 636f 7574 203c 3c20 2249 7320 6e6f  ::cout << "Is no
-00000ef0: 7420 4d61 6c65 2220 3c3c 2073 7464 3a3a  t Male" << std::
-00000f00: 656e 646c 3b0a 2020 2020 7d0a 2020 2020  endl;.    }.    
-00000f10: 7265 7475 726e 2030 3b0a 7d0a 6060 600a  return 0;.}.```.
-00000f20: 0a23 2323 2320 5769 7468 2060 7377 6974  .#### With `swit
-00000f30: 6368 2e2e 2e63 6173 652e 2e2e 600a 0a60  ch...case...`..`
-00000f40: 6060 6370 700a 2369 6e63 6c75 6465 203c  ``cpp.#include <
-00000f50: 696f 7374 7265 616d 3e0a 0a69 6e74 206d  iostream>..int m
-00000f60: 6169 6e28 2920 7b0a 2020 2020 696e 7420  ain() {.    int 
-00000f70: 6e75 6d62 6572 203d 2031 3b0a 2020 2020  number = 1;.    
-00000f80: 7377 6974 6368 2028 6e75 6d62 6572 2920  switch (number) 
-00000f90: 7b0a 2020 2020 2020 2020 6361 7365 2031  {.        case 1
-00000fa0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
-00000fb0: 643a 3a63 6f75 7420 3c3c 2022 3122 203c  d::cout << "1" <
-00000fc0: 3c20 7374 643a 3a65 6e64 6c3b 0a20 2020  < std::endl;.   
-00000fd0: 2020 2020 2063 6173 6520 323a 0a20 2020       case 2:.   
-00000fe0: 2020 2020 2020 2020 2073 7464 3a3a 636f           std::co
-00000ff0: 7574 203c 3c20 2232 2220 3c3c 2073 7464  ut << "2" << std
-00001000: 3a3a 656e 646c 3b0a 2020 2020 2020 2020  ::endl;.        
-00001010: 6465 6661 756c 743a 0a20 2020 2020 2020  default:.       
-00001020: 2020 2020 2073 7464 3a3a 636f 7574 203c       std::cout <
-00001030: 3c20 224e 6f74 2064 6566 696e 6564 2220  < "Not defined" 
-00001040: 3c3c 2073 7464 3a3a 656e 646c 3b0a 2020  << std::endl;.  
-00001050: 2020 7d0a 2020 2020 7265 7475 726e 2030    }.    return 0
-00001060: 3b0a 7d0a 6060 600a 0a23 2323 204c 6f6f  ;.}.```..### Loo
-00001070: 700a 0a23 2323 2320 466f 7220 666c 6f61  p..#### For floa
-00001080: 7420 636f 6e64 6974 696f 6e0a 0a60 6060  t condition..```
-00001090: 6370 700a 2369 6e63 6c75 6465 203c 696f  cpp.#include <io
-000010a0: 7374 7265 616d 3e0a 0a69 6e74 206d 6169  stream>..int mai
-000010b0: 6e28 2920 7b0a 2020 2020 696e 7420 6c69  n() {.    int li
-000010c0: 6d20 3d20 3130 3b0a 2020 2020 666f 7220  m = 10;.    for 
-000010d0: 2869 6e74 2069 203d 2030 3b20 6920 3c20  (int i = 0; i < 
-000010e0: 6c69 6d3b 2069 2b2b 2920 7b0a 2020 2020  lim; i++) {.    
-000010f0: 2020 2020 7374 643a 3a63 6f75 7420 3c3c      std::cout <<
-00001100: 2069 203c 3c20 7374 643a 3a65 6e64 6c3b   i << std::endl;
-00001110: 0a20 2020 207d 0a20 2020 2072 6574 7572  .    }.    retur
-00001120: 6e20 303b 0a7d 0a60 6060 0a0a 2323 2323  n 0;.}.```..####
-00001130: 2046 6f72 2066 6978 6564 2063 6f6e 6469   For fixed condi
-00001140: 7469 6f6e 0a0a 6060 6063 7070 0a23 696e  tion..```cpp.#in
-00001150: 636c 7564 6520 3c69 6f73 7472 6561 6d3e  clude <iostream>
-00001160: 0a0a 696e 7420 6d61 696e 2829 207b 0a20  ..int main() {. 
-00001170: 2020 2069 6e74 206c 696d 203d 2030 3b0a     int lim = 0;.
-00001180: 2020 2020 7768 696c 6520 286c 696d 203c      while (lim <
-00001190: 2031 3029 207b 0a20 2020 2020 2020 2073   10) {.        s
-000011a0: 7464 3a3a 636f 7574 203c 3c20 6c69 6d20  td::cout << lim 
-000011b0: 3c3c 2073 7464 3a3a 656e 646c 3b0a 2020  << std::endl;.  
-000011c0: 2020 2020 2020 6c69 6d2b 2b3b 0a20 2020        lim++;.   
-000011d0: 207d 0a20 2020 2072 6574 7572 6e20 303b   }.    return 0;
-000011e0: 0a7d 0a60 6060 0a0a 2323 2320 4578 6365  .}.```..### Exce
-000011f0: 7074 696f 6e20 6861 6e64 6c65 720a 0a60  ption handler..`
-00001200: 6060 6370 700a 2369 6e63 6c75 6465 203c  ``cpp.#include <
-00001210: 696f 7374 7265 616d 3e0a 0a69 6e74 206d  iostream>..int m
-00001220: 6169 6e28 2920 7b0a 2020 2020 7374 643a  ain() {.    std:
-00001230: 3a63 6572 7220 3c3c 2022 4578 6365 7074  :cerr << "Except
-00001240: 696f 6e20 6861 7070 656e 6564 223b 0a7d  ion happened";.}
-00001250: 0a60 6060 0a                             .```.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 206a 7570  : 2.1..Name: jup
+00000020: 7974 6572 2d63 7070 2d6b 6572 6e65 6c0d  yter-cpp-kernel.
+00000030: 0a56 6572 7369 6f6e 3a20 312e 302e 3061  .Version: 1.0.0a
+00000040: 330d 0a53 756d 6d61 7279 3a20 432b 2b20  3..Summary: C++ 
+00000050: 3134 206b 6572 6e65 6c20 666f 7220 4a75  14 kernel for Ju
+00000060: 7079 7465 720d 0a48 6f6d 652d 7061 6765  pyter..Home-page
+00000070: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000080: 2e63 6f6d 2f74 616b 696e 656b 6f74 6673  .com/takinekotfs
+00000090: 2f6a 7570 7974 6572 2d63 7070 2d6b 6572  /jupyter-cpp-ker
+000000a0: 6e65 6c0d 0a44 6f77 6e6c 6f61 642d 5552  nel..Download-UR
+000000b0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
+000000c0: 622e 636f 6d2f 7461 6b69 6e65 6b6f 7466  b.com/takinekotf
+000000d0: 732f 6a75 7079 7465 722d 6370 702d 6b65  s/jupyter-cpp-ke
+000000e0: 726e 656c 0d0a 4175 7468 6f72 3a20 5473  rnel..Author: Ts
+000000f0: 756b 6920 5461 6b69 6e65 6b6f 0d0a 4175  uki Takineko..Au
+00000100: 7468 6f72 2d65 6d61 696c 3a20 7379 7374  thor-email: syst
+00000110: 616b 696e 656b 6f2e 7466 7340 676d 6169  akineko.tfs@gmai
+00000120: 6c2e 636f 6d0d 0a4c 6963 656e 7365 3a20  l.com..License: 
+00000130: 4d49 540d 0a50 726f 6a65 6374 2d55 524c  MIT..Project-URL
+00000140: 3a20 4275 6720 5472 6163 6b65 722c 2068  : Bug Tracker, h
+00000150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000160: 6d2f 7461 6b69 6e65 6b6f 7466 732f 6a75  m/takinekotfs/ju
+00000170: 7079 7465 722d 6370 702d 6b65 726e 656c  pyter-cpp-kernel
+00000180: 2f69 7373 7565 730d 0a4b 6579 776f 7264  /issues..Keyword
+00000190: 733a 206a 7570 7974 6572 2c63 7070 2c63  s: jupyter,cpp,c
+000001a0: 7070 3134 2c6a 7570 7974 6572 2d6b 6572  pp14,jupyter-ker
+000001b0: 6e65 6c73 2c70 6970 0d0a 436c 6173 7369  nels,pip..Classi
+000001c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000001d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001e0: 7468 6f6e 203a 3a20 330d 0a43 6c61 7373  thon :: 3..Class
+000001f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2043  ng Language :: C
+00000210: 2b2b 0d0a 436c 6173 7369 6669 6572 3a20  ++..Classifier: 
+00000220: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000230: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000240: 6963 656e 7365 0d0a 436c 6173 7369 6669  icense..Classifi
+00000250: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00000260: 7374 656d 203a 3a20 556e 6978 0d0a 436c  stem :: Unix..Cl
+00000270: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000280: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+00000290: 634f 530d 0a43 6c61 7373 6966 6965 723a  cOS..Classifier:
+000002a0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+000002b0: 6d20 3a3a 2050 4f53 4958 203a 3a20 4c69  m :: POSIX :: Li
+000002c0: 6e75 780d 0a52 6571 7569 7265 732d 5079  nux..Requires-Py
+000002d0: 7468 6f6e 3a20 3e3d 332e 380d 0a44 6573  thon: >=3.8..Des
+000002e0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000002f0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000300: 646f 776e 0d0a 4c69 6365 6e73 652d 4669  down..License-Fi
+00000310: 6c65 3a20 4c49 4345 4e53 450d 0a0d 0a60  le: LICENSE....`
+00000320: 6060 6d61 726b 646f 776e 0d0a 5468 6973  ``markdown..This
+00000330: 2072 6570 6f20 6973 206f 7269 6769 6e61   repo is origina
+00000340: 6c6c 7920 6372 6561 7465 6420 6279 2042  lly created by B
+00000350: 7265 6e64 616e 2052 6975 7320 2d20 6043  rendan Rius - `C
+00000360: 204b 6572 6e65 6c20 666f 7220 4a75 7079   Kernel for Jupy
+00000370: 7465 7260 0d0a 0d0a 596f 7520 6361 6e20  ter`....You can 
+00000380: 7365 6520 7468 6520 6f72 6967 696e 616c  see the original
+00000390: 2070 726f 6a65 6374 2061 7420 6874 7470   project at http
+000003a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+000003b0: 7265 6e64 616e 2d72 6975 732f 6a75 7079  rendan-rius/jupy
+000003c0: 7465 722d 632d 6b65 726e 656c 0d0a 0d0a  ter-c-kernel....
+000003d0: 506c 7573 2c20 7468 6973 2043 2b2b 206b  Plus, this C++ k
+000003e0: 6572 6e65 6c20 6f6e 6c79 2075 7365 7320  ernel only uses 
+000003f0: 432b 2b20 3134 2e20 5468 6520 6f74 6865  C++ 14. The othe
+00000400: 7273 2061 7265 2062 6569 6e67 2064 6576  rs are being dev
+00000410: 656c 6f70 6564 0d0a 286f 7220 6e6f 742c  eloped..(or not,
+00000420: 2077 686f 206b 6e6f 7773 20f0 9f98 8529   who knows ....)
+00000430: 0d0a 6060 600d 0a0d 0a5b 215b 436f 6465  ..```....[![Code
+00000440: 514c 5d28 6874 7470 733a 2f2f 6769 7468  QL](https://gith
+00000450: 7562 2e63 6f6d 2f74 616b 696e 656b 6f74  ub.com/takinekot
+00000460: 6673 2f6a 7570 7974 6572 2d63 7070 2d6b  fs/jupyter-cpp-k
+00000470: 6572 6e65 6c2f 6163 7469 6f6e 732f 776f  ernel/actions/wo
+00000480: 726b 666c 6f77 732f 636f 6465 716c 2e79  rkflows/codeql.y
+00000490: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+000004a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004b0: 6d2f 7461 6b69 6e65 6b6f 7466 732f 6a75  m/takinekotfs/ju
+000004c0: 7079 7465 722d 6370 702d 6b65 726e 656c  pyter-cpp-kernel
+000004d0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+000004e0: 7773 2f63 6f64 6571 6c2e 796d 6c29 0d0a  ws/codeql.yml)..
+000004f0: 0d0a 2320 432b 2b20 3134 206b 6572 6e65  ..# C++ 14 kerne
+00000500: 6c20 666f 7220 4a75 7079 7465 720d 0a0d  l for Jupyter...
+00000510: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000520: 0d0a 0d0a 3e20 3a77 6172 6e69 6e67 3a0d  ....> :warning:.
+00000530: 0a3e 0d0a 3e20 4966 2079 6f75 2077 616e  .>..> If you wan
+00000540: 7420 746f 2075 7365 2069 7420 6f6e 2057  t to use it on W
+00000550: 696e 646f 7773 2c20 706c 6561 7365 2069  indows, please i
+00000560: 6e73 7461 6c6c 696e 6720 7468 6520 5b47  nstalling the [G
+00000570: 4e55 2043 6f6d 7069 6c65 7220 436f 6c6c  NU Compiler Coll
+00000580: 6563 7469 6f6e 2066 6f72 2057 696e 646f  ection for Windo
+00000590: 7773 5d28 6874 7470 733a 2f2f 6769 7468  ws](https://gith
+000005a0: 7562 2e63 6f6d 2f74 616b 696e 656b 6f74  ub.com/takinekot
+000005b0: 6673 2f6a 7570 7974 6572 2d63 7070 2d6b  fs/jupyter-cpp-k
+000005c0: 6572 6e65 6c2f 7265 6c65 6173 6573 2f74  ernel/releases/t
+000005d0: 6167 2f67 6363 2d31 332e 322e 3029 0d0a  ag/gcc-13.2.0)..
+000005e0: 0d0a 4e6f 726d 616c 6c79 2c20 796f 7572  ..Normally, your
+000005f0: 2074 6172 6765 7420 6d61 6368 696e 6520   target machine 
+00000600: 6d75 7374 206d 6565 7420 7468 6573 6520  must meet these 
+00000610: 7265 7175 6972 656d 656e 7420 7061 636b  requirement pack
+00000620: 6167 6573 2062 6566 6f72 6520 696e 7374  ages before inst
+00000630: 616c 6c69 6e67 2061 6e64 2075 7369 6e67  alling and using
+00000640: 2060 6a75 7079 7465 722d 6370 702d 6b65   `jupyter-cpp-ke
+00000650: 726e 656c 602e 0d0a 0d0a 2a20 6067 2b2b  rnel`.....* `g++
+00000660: 600d 0a2a 2060 7079 7468 6f6e 3360 2c20  `..* `python3`, 
+00000670: 6070 7974 686f 6e33 2d70 6970 600d 0a2a  `python3-pip`..*
+00000680: 2060 6a75 7079 7465 7260 2028 7265 636f   `jupyter` (reco
+00000690: 6d6d 656e 6420 606a 7570 7974 6572 6c61  mmend `jupyterla
+000006a0: 6260 290d 0a0d 0a23 2323 2049 6e73 7461  b`)....### Insta
+000006b0: 6c6c 2066 726f 6d20 5079 5049 0d0a 0d0a  ll from PyPI....
+000006c0: 2323 2323 2049 6e73 7461 6c6c 696e 6720  #### Installing 
+000006d0: 6f6e 206d 6163 4f53 2061 6e64 2057 696e  on macOS and Win
+000006e0: 646f 7773 0d0a 0d0a 3e20 3a77 6172 6e69  dows....> :warni
+000006f0: 6e67 3a0d 0a3e 0d0a 3e20 596f 7520 6d75  ng:..>..> You mu
+00000700: 7374 2061 6c6c 2072 6571 7569 7265 6d65  st all requireme
+00000710: 6e74 7320 6162 6f76 6520 6265 666f 7265  nts above before
+00000720: 2064 6f69 6e67 2061 6e79 7468 696e 6720   doing anything 
+00000730: 656c 7365 2e0d 0a3e 2041 6674 6572 2074  else...> After t
+00000740: 6861 742c 2079 6f75 2063 616e 2063 6f70  hat, you can cop
+00000750: 7920 7468 6973 2073 6372 6970 7420 616e  y this script an
+00000760: 6420 696e 7374 616c 6c20 7468 6520 6b65  d install the ke
+00000770: 726e 656c 0d0a 0d0a 6060 6073 6865 6c6c  rnel....```shell
+00000780: 0d0a 7069 7020 696e 7374 616c 6c20 6a75  ..pip install ju
+00000790: 7079 7465 722d 6370 702d 6b65 726e 656c  pyter-cpp-kernel
+000007a0: 0d0a 6060 600d 0a0d 0a23 2323 2320 496e  ..```....#### In
+000007b0: 7374 616c 6c69 6e67 206f 6e20 4465 6269  stalling on Debi
+000007c0: 616e 2f55 6275 6e74 750d 0a0d 0a60 6060  an/Ubuntu....```
+000007d0: 7368 656c 6c0d 0a73 7564 6f20 6170 7420  shell..sudo apt 
+000007e0: 7570 6461 7465 2026 2620 7375 646f 2061  update && sudo a
+000007f0: 7074 2066 756c 6c2d 7570 6772 6164 6520  pt full-upgrade 
+00000800: 2d79 200d 0a73 7564 6f20 6170 7420 696e  -y ..sudo apt in
+00000810: 7374 616c 6c20 2d79 2067 2b2b 0d0a 7375  stall -y g++..su
+00000820: 646f 2061 7074 2069 6e73 7461 6c6c 202d  do apt install -
+00000830: 7920 7079 7468 6f6e 3320 7079 7468 6f6e  y python3 python
+00000840: 332d 7069 700d 0a73 7564 6f20 7069 7020  3-pip..sudo pip 
+00000850: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
+00000860: 6520 7069 700d 0a73 7564 6f20 7069 7020  e pip..sudo pip 
+00000870: 696e 7374 616c 6c20 6a75 7079 7465 7220  install jupyter 
+00000880: 2320 4f72 206a 7570 7974 6572 6c61 622e  # Or jupyterlab.
+00000890: 2055 7369 6e67 2060 7375 646f 6020 746f   Using `sudo` to
+000008a0: 2069 6e73 7461 6c6c 2074 6f20 7468 6520   install to the 
+000008b0: 6d61 696e 2070 6163 6b67 650d 0a73 7564  main packge..sud
+000008c0: 6f20 7069 7020 696e 7374 616c 6c20 6a75  o pip install ju
+000008d0: 7079 7465 722d 6370 702d 6b65 726e 656c  pyter-cpp-kernel
+000008e0: 2023 2043 616e 2062 6520 6073 7564 6f60   # Can be `sudo`
+000008f0: 2c20 6275 7420 7573 696e 6720 6974 2077  , but using it w
+00000900: 6974 6820 6361 7574 696f 6e2e 204f 6e6c  ith caution. Onl
+00000910: 7920 666f 7220 6c61 7267 6520 6465 706c  y for large depl
+00000920: 6f79 6d65 6e74 204a 7570 7974 6572 2073  oyment Jupyter s
+00000930: 6572 7665 720d 0a60 6060 0d0a 0d0a 2323  erver..```....##
+00000940: 2320 496e 7374 616c 6c20 6672 6f6d 2047  # Install from G
+00000950: 6974 4875 6220 7265 706f 0d0a 0d0a 2323  itHub repo....##
+00000960: 2323 2049 6e73 7461 6c6c 696e 6720 6f6e  ## Installing on
+00000970: 206d 6163 4f53 2061 6e64 2057 696e 646f   macOS and Windo
+00000980: 7773 0d0a 0d0a 3e20 3a77 6172 6e69 6e67  ws....> :warning
+00000990: 3a0d 0a3e 0d0a 3e20 596f 7520 6d75 7374  :..>..> You must
+000009a0: 2061 6c6c 2072 6571 7569 7265 6d65 6e74   all requirement
+000009b0: 7320 6162 6f76 6520 6265 666f 7265 2064  s above before d
+000009c0: 6f69 6e67 2061 6e79 7468 696e 6720 656c  oing anything el
+000009d0: 7365 2e5c 0d0a 3e20 4166 7465 7220 7468  se.\..> After th
+000009e0: 6174 2c20 796f 7520 6361 6e20 636f 7079  at, you can copy
+000009f0: 2074 6869 7320 7363 7269 7074 2061 6e64   this script and
+00000a00: 2069 6e73 7461 6c6c 2074 6865 206b 6572   install the ker
+00000a10: 6e65 6c0d 0a0d 0a60 6060 7368 656c 6c0d  nel....```shell.
+00000a20: 0a70 6970 2069 6e73 7461 6c6c 2067 6974  .pip install git
+00000a30: 2b68 7474 7073 3a2f 2f67 6974 6875 622e  +https://github.
+00000a40: 636f 6d2f 7461 6b69 6e65 6b6f 7466 732f  com/takinekotfs/
+00000a50: 6a75 7079 7465 722d 6370 702d 6b65 726e  jupyter-cpp-kern
+00000a60: 656c 2e67 6974 0d0a 6060 600d 0a0d 0a23  el.git..```....#
+00000a70: 2323 2320 496e 7374 616c 6c69 6e67 206f  ### Installing o
+00000a80: 6e20 4465 6269 616e 2f55 6275 6e74 750d  n Debian/Ubuntu.
+00000a90: 0a0d 0a60 6060 7368 656c 6c0d 0a73 7564  ...```shell..sud
+00000aa0: 6f20 6170 7420 7570 6461 7465 2026 2620  o apt update && 
+00000ab0: 7375 646f 2061 7074 2066 756c 6c2d 7570  sudo apt full-up
+00000ac0: 6772 6164 6520 2d79 200d 0a73 7564 6f20  grade -y ..sudo 
+00000ad0: 6170 7420 696e 7374 616c 6c20 2d79 2067  apt install -y g
+00000ae0: 2b2b 0d0a 7375 646f 2061 7074 2069 6e73  ++..sudo apt ins
+00000af0: 7461 6c6c 202d 7920 7079 7468 6f6e 3320  tall -y python3 
+00000b00: 7079 7468 6f6e 332d 7069 700d 0a73 7564  python3-pip..sud
+00000b10: 6f20 7069 7020 696e 7374 616c 6c20 2d2d  o pip install --
+00000b20: 7570 6772 6164 6520 7069 700d 0a73 7564  upgrade pip..sud
+00000b30: 6f20 7069 7020 696e 7374 616c 6c20 6a75  o pip install ju
+00000b40: 7079 7465 7220 2320 4f72 206a 7570 7974  pyter # Or jupyt
+00000b50: 6572 6c61 622e 2055 7369 6e67 2060 7375  erlab. Using `su
+00000b60: 646f 6020 746f 2069 6e73 7461 6c6c 2074  do` to install t
+00000b70: 6f20 7468 6520 6d61 696e 2070 6163 6b67  o the main packg
+00000b80: 650d 0a73 7564 6f20 7069 7020 696e 7374  e..sudo pip inst
+00000b90: 616c 6c20 6769 742b 6874 7470 733a 2f2f  all git+https://
+00000ba0: 6769 7468 7562 2e63 6f6d 2f74 616b 696e  github.com/takin
+00000bb0: 656b 6f74 6673 2f6a 7570 7974 6572 2d63  ekotfs/jupyter-c
+00000bc0: 7070 2d6b 6572 6e65 6c2e 6769 7420 0d0a  pp-kernel.git ..
+00000bd0: 6060 600d 0a0d 0a23 2320 436f 6e74 7269  ```....## Contri
+00000be0: 6275 7469 6e67 0d0a 0d0a 596f 7520 6361  buting....You ca
+00000bf0: 6e20 636c 6f6e 652c 2063 7265 6174 6520  n clone, create 
+00000c00: 6120 666f 726b 206f 7220 696d 706f 7274  a fork or import
+00000c10: 2074 6869 7320 7265 706f 2077 6865 6e65   this repo whene
+00000c20: 7665 7220 796f 7520 7761 6e74 2e0d 0a0d  ver you want....
+00000c30: 0a50 6c65 6173 6520 666f 6c6c 6f77 2074  .Please follow t
+00000c40: 6865 2047 6974 4875 6220 7374 616e 6461  he GitHub standa
+00000c50: 7264 7320 616e 6420 7468 6520 6c69 6365  rds and the lice
+00000c60: 6e73 650d 0a0d 0a23 2320 5361 6d70 6c65  nse....## Sample
+00000c70: 2063 6f64 6573 0d0a 0d0a 3e20 3a77 6172   codes....> :war
+00000c80: 6e69 6e67 3a0d 0a3e 0d0a 3e20 2d20 5261  ning:..>..> - Ra
+00000c90: 7720 696e 7075 7420 696e 746f 2070 726f  w input into pro
+00000ca0: 6772 616d 2069 7320 7374 696c 6c20 6e6f  gram is still no
+00000cb0: 7420 636f 6d70 6c65 7465 6420 7965 742e  t completed yet.
+00000cc0: 2059 6f75 206d 6179 2063 616e 6e6f 7420   You may cannot 
+00000cd0: 7573 696e 6720 6063 696e 6020 6f72 2061  using `cin` or a
+00000ce0: 6e79 2075 7365 7220 696e 7075 7420 7061  ny user input pa
+00000cf0: 7261 6d65 7465 722e 0d0a 3e0d 0a3e 202d  rameter...>..> -
+00000d00: 2046 6f72 2074 6865 2062 6573 7420 7072   For the best pr
+00000d10: 6163 7469 6365 732c 2079 6f75 2073 686f  actices, you sho
+00000d20: 756c 646e 2774 2077 7269 7465 2060 7573  uldn't write `us
+00000d30: 696e 6720 6e61 6d65 7370 6163 6520 7374  ing namespace st
+00000d40: 643b 6020 6265 6361 7573 6520 6f66 2074  d;` because of t
+00000d50: 6865 2063 6f6e 666c 6963 7473 2062 6574  he conflicts bet
+00000d60: 7765 656e 2074 6865 2060 6e61 6d65 7370  ween the `namesp
+00000d70: 6163 6560 2e20 5468 6973 2070 726f 626c  ace`. This probl
+00000d80: 656d 2064 6f65 736e 2774 2063 6f6d 6520  em doesn't come 
+00000d90: 6672 6f6d 2074 6865 2069 6e74 6572 7072  from the interpr
+00000da0: 6574 6572 2c20 6974 2773 2061 6374 7561  eter, it's actua
+00000db0: 6c6c 7920 7468 6520 7072 6f62 6c65 6d20  lly the problem 
+00000dc0: 6f66 2060 672b 2b60 2067 6c6f 6261 6c6c  of `g++` globall
+00000dd0: 790d 0a0d 0a23 2323 2048 656c 6c6f 2077  y....### Hello w
+00000de0: 6f72 6c64 0d0a 0d0a 6060 6063 7070 0d0a  orld....```cpp..
+00000df0: 2369 6e63 6c75 6465 203c 696f 7374 7265  #include <iostre
+00000e00: 616d 3e0d 0a0d 0a69 6e74 206d 6169 6e28  am>....int main(
+00000e10: 2920 7b0d 0a20 2020 2073 7464 3a3a 636f  ) {..    std::co
+00000e20: 7574 203c 3c20 2248 656c 6c6f 2057 6f72  ut << "Hello Wor
+00000e30: 6c64 2220 3c3c 2073 7464 3a3a 656e 646c  ld" << std::endl
+00000e40: 3b0d 0a20 2020 2072 6574 7572 6e20 303b  ;..    return 0;
+00000e50: 0d0a 7d0d 0a60 6060 0d0a 0d0a 2323 2320  ..}..```....### 
+00000e60: 4465 636c 6172 6520 7661 7269 6162 6c65  Declare variable
+00000e70: 2028 6069 6e74 6029 2061 6e64 2074 616b   (`int`) and tak
+00000e80: 6520 6120 6d61 7468 206f 6620 7468 656d  e a math of them
+00000e90: 0d0a 0d0a 6060 6063 7070 0d0a 2369 6e63  ....```cpp..#inc
+00000ea0: 6c75 6465 203c 696f 7374 7265 616d 3e0d  lude <iostream>.
+00000eb0: 0a23 696e 636c 7564 6520 3c63 6d61 7468  .#include <cmath
+00000ec0: 3e0d 0a0d 0a69 6e74 206d 6169 6e28 2920  >....int main() 
+00000ed0: 7b0d 0a20 2020 2069 6e74 2078 203d 2033  {..    int x = 3
+00000ee0: 2c20 7920 3d20 363b 0d0a 2020 2020 7374  , y = 6;..    st
+00000ef0: 643a 3a63 6f75 7420 3c3c 2022 5375 6d20  d::cout << "Sum 
+00000f00: 6f66 2078 2061 6e64 2079 2069 7320 2220  of x and y is " 
+00000f10: 3c3c 2078 202b 2079 203c 3c20 7374 643a  << x + y << std:
+00000f20: 3a65 6e64 6c3b 0d0a 2020 2020 7374 643a  :endl;..    std:
+00000f30: 3a63 6f75 7420 3c3c 2022 5375 6274 7261  :cout << "Subtra
+00000f40: 6374 206f 6620 7820 616e 6420 7920 6973  ct of x and y is
+00000f50: 2022 203c 3c20 7820 2d20 7920 3c3c 2073   " << x - y << s
+00000f60: 7464 3a3a 656e 646c 3b0d 0a20 2020 2072  td::endl;..    r
+00000f70: 6574 7572 6e20 303b 0d0a 7d0d 0a60 6060  eturn 0;..}..```
+00000f80: 0d0a 0d0a 2323 2320 436f 6e64 6974 696f  ....### Conditio
+00000f90: 6e0d 0a0d 0a23 2323 2320 5769 7468 2060  n....#### With `
+00000fa0: 4966 2e2e 2e65 6c73 652e 2e2e 600d 0a0d  If...else...`...
+00000fb0: 0a60 6060 6370 700d 0a23 696e 636c 7564  .```cpp..#includ
+00000fc0: 6520 3c69 6f73 7472 6561 6d3e 0d0a 0d0a  e <iostream>....
+00000fd0: 696e 7420 6d61 696e 2829 207b 0d0a 2020  int main() {..  
+00000fe0: 2020 626f 6f6c 2069 734d 616c 6520 3d20    bool isMale = 
+00000ff0: 6661 6c73 653b 0d0a 2020 2020 6966 2028  false;..    if (
+00001000: 6973 4d61 6c65 2920 7b0d 0a20 2020 2020  isMale) {..     
+00001010: 2020 2073 7464 3a3a 636f 7574 203c 3c20     std::cout << 
+00001020: 224d 616c 6522 203c 3c20 7374 643a 3a65  "Male" << std::e
+00001030: 6e64 6c3b 0d0a 2020 2020 7d0d 0a20 2020  ndl;..    }..   
+00001040: 2065 6c73 6520 7b0d 0a20 2020 2020 2020   else {..       
+00001050: 2073 7464 3a3a 636f 7574 203c 3c20 2249   std::cout << "I
+00001060: 7320 6e6f 7420 4d61 6c65 2220 3c3c 2073  s not Male" << s
+00001070: 7464 3a3a 656e 646c 3b0d 0a20 2020 207d  td::endl;..    }
+00001080: 0d0a 2020 2020 7265 7475 726e 2030 3b0d  ..    return 0;.
+00001090: 0a7d 0d0a 6060 600d 0a0d 0a23 2323 2320  .}..```....#### 
+000010a0: 5769 7468 2060 7377 6974 6368 2e2e 2e63  With `switch...c
+000010b0: 6173 652e 2e2e 600d 0a0d 0a60 6060 6370  ase...`....```cp
+000010c0: 700d 0a23 696e 636c 7564 6520 3c69 6f73  p..#include <ios
+000010d0: 7472 6561 6d3e 0d0a 0d0a 696e 7420 6d61  tream>....int ma
+000010e0: 696e 2829 207b 0d0a 2020 2020 696e 7420  in() {..    int 
+000010f0: 6e75 6d62 6572 203d 2031 3b0d 0a20 2020  number = 1;..   
+00001100: 2073 7769 7463 6820 286e 756d 6265 7229   switch (number)
+00001110: 207b 0d0a 2020 2020 2020 2020 6361 7365   {..        case
+00001120: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00001130: 2073 7464 3a3a 636f 7574 203c 3c20 2231   std::cout << "1
+00001140: 2220 3c3c 2073 7464 3a3a 656e 646c 3b0d  " << std::endl;.
+00001150: 0a20 2020 2020 2020 2063 6173 6520 323a  .        case 2:
+00001160: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00001170: 643a 3a63 6f75 7420 3c3c 2022 3222 203c  d::cout << "2" <
+00001180: 3c20 7374 643a 3a65 6e64 6c3b 0d0a 2020  < std::endl;..  
+00001190: 2020 2020 2020 6465 6661 756c 743a 0d0a        default:..
+000011a0: 2020 2020 2020 2020 2020 2020 7374 643a              std:
+000011b0: 3a63 6f75 7420 3c3c 2022 4e6f 7420 6465  :cout << "Not de
+000011c0: 6669 6e65 6422 203c 3c20 7374 643a 3a65  fined" << std::e
+000011d0: 6e64 6c3b 0d0a 2020 2020 7d0d 0a20 2020  ndl;..    }..   
+000011e0: 2072 6574 7572 6e20 303b 0d0a 7d0d 0a60   return 0;..}..`
+000011f0: 6060 0d0a 0d0a 2323 2320 4c6f 6f70 0d0a  ``....### Loop..
+00001200: 0d0a 2323 2323 2046 6f72 2066 6c6f 6174  ..#### For float
+00001210: 2063 6f6e 6469 7469 6f6e 0d0a 0d0a 6060   condition....``
+00001220: 6063 7070 0d0a 2369 6e63 6c75 6465 203c  `cpp..#include <
+00001230: 696f 7374 7265 616d 3e0d 0a0d 0a69 6e74  iostream>....int
+00001240: 206d 6169 6e28 2920 7b0d 0a20 2020 2069   main() {..    i
+00001250: 6e74 206c 696d 203d 2031 303b 0d0a 2020  nt lim = 10;..  
+00001260: 2020 666f 7220 2869 6e74 2069 203d 2030    for (int i = 0
+00001270: 3b20 6920 3c20 6c69 6d3b 2069 2b2b 2920  ; i < lim; i++) 
+00001280: 7b0d 0a20 2020 2020 2020 2073 7464 3a3a  {..        std::
+00001290: 636f 7574 203c 3c20 6920 3c3c 2073 7464  cout << i << std
+000012a0: 3a3a 656e 646c 3b0d 0a20 2020 207d 0d0a  ::endl;..    }..
+000012b0: 2020 2020 7265 7475 726e 2030 3b0d 0a7d      return 0;..}
+000012c0: 0d0a 6060 600d 0a0d 0a23 2323 2320 466f  ..```....#### Fo
+000012d0: 7220 6669 7865 6420 636f 6e64 6974 696f  r fixed conditio
+000012e0: 6e0d 0a0d 0a60 6060 6370 700d 0a23 696e  n....```cpp..#in
+000012f0: 636c 7564 6520 3c69 6f73 7472 6561 6d3e  clude <iostream>
+00001300: 0d0a 0d0a 696e 7420 6d61 696e 2829 207b  ....int main() {
+00001310: 0d0a 2020 2020 696e 7420 6c69 6d20 3d20  ..    int lim = 
+00001320: 303b 0d0a 2020 2020 7768 696c 6520 286c  0;..    while (l
+00001330: 696d 203c 2031 3029 207b 0d0a 2020 2020  im < 10) {..    
+00001340: 2020 2020 7374 643a 3a63 6f75 7420 3c3c      std::cout <<
+00001350: 206c 696d 203c 3c20 7374 643a 3a65 6e64   lim << std::end
+00001360: 6c3b 0d0a 2020 2020 2020 2020 6c69 6d2b  l;..        lim+
+00001370: 2b3b 0d0a 2020 2020 7d0d 0a20 2020 2072  +;..    }..    r
+00001380: 6574 7572 6e20 303b 0d0a 7d0d 0a60 6060  eturn 0;..}..```
+00001390: 0d0a 0d0a 2323 2320 4578 6365 7074 696f  ....### Exceptio
+000013a0: 6e20 6861 6e64 6c65 720d 0a0d 0a60 6060  n handler....```
+000013b0: 6370 700d 0a23 696e 636c 7564 6520 3c69  cpp..#include <i
+000013c0: 6f73 7472 6561 6d3e 0d0a 0d0a 696e 7420  ostream>....int 
+000013d0: 6d61 696e 2829 207b 0d0a 2020 2020 7374  main() {..    st
+000013e0: 643a 3a63 6572 7220 3c3c 2022 4578 6365  d::cerr << "Exce
+000013f0: 7074 696f 6e20 6861 7070 656e 6564 223b  ption happened";
+00001400: 0d0a 7d0d 0a60 6060 0d0a                 ..}..```..
```

### Comparing `jupyter_cpp_kernel-1.0.0a2/setup.cfg` & `jupyter_cpp_kernel-1.0.0a3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-00000000: 5b6d 6574 6164 6174 615d 0a64 6573 6372  [metadata].descr
-00000010: 6970 7469 6f6e 2d66 696c 6520 3d20 5245  iption-file = RE
-00000020: 4144 4d45 2e6d 640a 6e61 6d65 203d 206a  ADME.md.name = j
-00000030: 7570 7974 6572 2d63 7070 2d6b 6572 6e65  upyter-cpp-kerne
-00000040: 6c0a 7665 7273 696f 6e20 3d20 312e 302e  l.version = 1.0.
-00000050: 3061 320a 6175 7468 6f72 203d 2054 7375  0a2.author = Tsu
-00000060: 6b69 2054 616b 696e 656b 6f20 2866 742e  ki Takineko (ft.
-00000070: 2042 7265 6e64 616e 2052 6975 7329 0a61   Brendan Rius).a
-00000080: 7574 686f 725f 656d 6169 6c20 3d20 7379  uthor_email = sy
-00000090: 7374 616b 696e 656b 6f2e 7466 7340 676d  stakineko.tfs@gm
-000000a0: 6169 6c2e 636f 6d0a 6465 7363 7269 7074  ail.com.descript
-000000b0: 696f 6e20 3d20 432b 2b20 6b65 726e 656c  ion = C++ kernel
-000000c0: 2066 6f72 204a 7570 7974 6572 2e20 4561   for Jupyter. Ea
-000000d0: 7369 6c79 2061 646f 7074 2061 6e64 2064  sily adopt and d
-000000e0: 6570 6c6f 7920 666f 7220 7465 7374 696e  eploy for testin
-000000f0: 6720 656e 7669 726f 6e6d 656e 742e 0a6c  g environment..l
-00000100: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000110: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000120: 640a 6c6f 6e67 5f64 6573 6372 6970 7469  d.long_descripti
-00000130: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-00000140: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0a  = text/markdown.
-00000150: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000160: 7468 7562 2e63 6f6d 2f74 616b 696e 656b  thub.com/takinek
-00000170: 6f74 6673 2f6a 7570 7974 6572 2d63 7070  otfs/jupyter-cpp
-00000180: 2d6b 6572 6e65 6c0a 7072 6f6a 6563 745f  -kernel.project_
-00000190: 7572 6c73 203d 200a 0942 7567 2054 7261  urls = ..Bug Tra
-000001a0: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-000001b0: 6974 6875 622e 636f 6d2f 7461 6b69 6e65  ithub.com/takine
-000001c0: 6b6f 7466 732f 6a75 7079 7465 722d 6370  kotfs/jupyter-cp
-000001d0: 702d 6b65 726e 656c 2f69 7373 7565 730a  p-kernel/issues.
-000001e0: 636c 6173 7369 6669 6572 7320 3d20 0a09  classifiers = ..
-000001f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000200: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000210: 3a20 330a 0950 726f 6772 616d 6d69 6e67  : 3..Programming
-00000220: 204c 616e 6775 6167 6520 3a3a 2043 2b2b   Language :: C++
-00000230: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000240: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000250: 204c 6963 656e 7365 0a09 4f70 6572 6174   License..Operat
-00000260: 696e 6720 5379 7374 656d 203a 3a20 556e  ing System :: Un
-00000270: 6978 0a09 4f70 6572 6174 696e 6720 5379  ix..Operating Sy
-00000280: 7374 656d 203a 3a20 4d61 634f 530a 094f  stem :: MacOS..O
-00000290: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000002a0: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
-000002b0: 780a 0a5b 6f70 7469 6f6e 735d 0a70 7974  x..[options].pyt
-000002c0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002d0: 3d33 2e36 0a0a 5b65 6767 5f69 6e66 6f5d  =3.6..[egg_info]
-000002e0: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
-000002f0: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6465 7363  [metadata]..desc
+00000010: 7269 7074 696f 6e2d 6669 6c65 203d 2052  ription-file = R
+00000020: 4541 444d 452e 6d64 0d0a 6e61 6d65 203d  EADME.md..name =
+00000030: 206a 7570 7974 6572 2d63 7070 2d6b 6572   jupyter-cpp-ker
+00000040: 6e65 6c0d 0a76 6572 7369 6f6e 203d 2031  nel..version = 1
+00000050: 2e30 2e30 6133 0d0a 6175 7468 6f72 203d  .0.0a3..author =
+00000060: 2054 7375 6b69 2054 616b 696e 656b 6f20   Tsuki Takineko 
+00000070: 2866 742e 2042 7265 6e64 616e 2052 6975  (ft. Brendan Riu
+00000080: 7329 0d0a 6175 7468 6f72 5f65 6d61 696c  s)..author_email
+00000090: 203d 2073 7973 7461 6b69 6e65 6b6f 2e74   = systakineko.t
+000000a0: 6673 4067 6d61 696c 2e63 6f6d 0d0a 6465  fs@gmail.com..de
+000000b0: 7363 7269 7074 696f 6e20 3d20 432b 2b20  scription = C++ 
+000000c0: 6b65 726e 656c 2066 6f72 204a 7570 7974  kernel for Jupyt
+000000d0: 6572 2e20 4561 7369 6c79 2061 646f 7074  er. Easily adopt
+000000e0: 2061 6e64 2064 6570 6c6f 7920 666f 7220   and deploy for 
+000000f0: 7465 7374 696e 6720 656e 7669 726f 6e6d  testing environm
+00000100: 656e 742e 0d0a 6c6f 6e67 5f64 6573 6372  ent...long_descr
+00000110: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+00000120: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+00000130: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000140: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000150: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000160: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000170: 6d2f 7461 6b69 6e65 6b6f 7466 732f 6a75  m/takinekotfs/ju
+00000180: 7079 7465 722d 6370 702d 6b65 726e 656c  pyter-cpp-kernel
+00000190: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+000001a0: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+000001b0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001c0: 2e63 6f6d 2f74 616b 696e 656b 6f74 6673  .com/takinekotfs
+000001d0: 2f6a 7570 7974 6572 2d63 7070 2d6b 6572  /jupyter-cpp-ker
+000001e0: 6e65 6c2f 6973 7375 6573 0d0a 636c 6173  nel/issues..clas
+000001f0: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000220: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000230: 616e 6775 6167 6520 3a3a 2043 2b2b 0d0a  anguage :: C++..
+00000240: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000250: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000260: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000270: 696e 6720 5379 7374 656d 203a 3a20 556e  ing System :: Un
+00000280: 6978 0d0a 094f 7065 7261 7469 6e67 2053  ix...Operating S
+00000290: 7973 7465 6d20 3a3a 204d 6163 4f53 0d0a  ystem :: MacOS..
+000002a0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000002b0: 6d20 3a3a 2050 4f53 4958 203a 3a20 4c69  m :: POSIX :: Li
+000002c0: 6e75 780d 0a0d 0a5b 6f70 7469 6f6e 735d  nux....[options]
+000002d0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+000002e0: 7320 3d20 3e3d 332e 380d 0a0d 0a5b 6567  s = >=3.8....[eg
+000002f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000300: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000310: 3d20 300d 0a0d 0a                        = 0....
```

