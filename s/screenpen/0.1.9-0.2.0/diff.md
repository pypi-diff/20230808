# Comparing `tmp/screenpen-0.1.9.tar.gz` & `tmp/screenpen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/screenpen-0.1.9.tar", last modified: Tue Aug  3 12:52:04 2021, max compression
+gzip compressed data, was "screenpen-0.2.0.tar", last modified: Tue Aug  8 21:24:20 2023, max compression
```

## Comparing `screenpen-0.1.9.tar` & `screenpen-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 ok        (1000) ok        (1000)        0 2021-08-03 12:52:04.000000 screenpen-0.1.9/
--rw-rw-r--   0 ok        (1000) ok        (1000)    35149 2021-05-13 13:55:50.000000 screenpen-0.1.9/LICENSE
--rw-rw-r--   0 ok        (1000) ok        (1000)    35148 2021-05-09 22:11:14.000000 screenpen-0.1.9/LICENSE.txt
--rw-rw-r--   0 ok        (1000) ok        (1000)     3102 2021-08-03 12:52:04.000000 screenpen-0.1.9/PKG-INFO
--rw-rw-r--   0 ok        (1000) ok        (1000)     1679 2021-08-03 12:50:39.000000 screenpen-0.1.9/README.md
-drwxrwxr-x   0 ok        (1000) ok        (1000)        0 2021-08-03 12:52:04.000000 screenpen-0.1.9/screenpen/
--rw-rw-r--   0 ok        (1000) ok        (1000)        0 2021-05-13 19:31:11.000000 screenpen-0.1.9/screenpen/__init__.py
--rw-rw-r--   0 ok        (1000) ok        (1000)       76 2021-05-13 19:38:09.000000 screenpen-0.1.9/screenpen/__main__.py
--rw-rw-r--   0 ok        (1000) ok        (1000)    29050 2021-05-13 21:59:09.000000 screenpen-0.1.9/screenpen/screenpen.py
-drwxrwxr-x   0 ok        (1000) ok        (1000)        0 2021-08-03 12:52:04.000000 screenpen-0.1.9/screenpen/utils/
--rw-rw-r--   0 ok        (1000) ok        (1000)    41586 2021-05-13 13:55:50.000000 screenpen-0.1.9/screenpen/utils/resources.xml
--rw-rw-r--   0 ok        (1000) ok        (1000)     6260 2021-05-13 13:55:50.000000 screenpen-0.1.9/screenpen/utils/syntax.py
--rw-rw-r--   0 ok        (1000) ok        (1000)       22 2021-08-03 12:51:13.000000 screenpen-0.1.9/screenpen/version.py
-drwxrwxr-x   0 ok        (1000) ok        (1000)        0 2021-08-03 12:52:04.000000 screenpen-0.1.9/screenpen.egg-info/
--rw-rw-r--   0 ok        (1000) ok        (1000)     3102 2021-08-03 12:52:03.000000 screenpen-0.1.9/screenpen.egg-info/PKG-INFO
--rw-rw-r--   0 ok        (1000) ok        (1000)      394 2021-08-03 12:52:03.000000 screenpen-0.1.9/screenpen.egg-info/SOURCES.txt
--rw-rw-r--   0 ok        (1000) ok        (1000)        1 2021-08-03 12:52:03.000000 screenpen-0.1.9/screenpen.egg-info/dependency_links.txt
--rw-rw-r--   0 ok        (1000) ok        (1000)       42 2021-08-03 12:52:03.000000 screenpen-0.1.9/screenpen.egg-info/entry_points.txt
--rw-rw-r--   0 ok        (1000) ok        (1000)       33 2021-08-03 12:52:03.000000 screenpen-0.1.9/screenpen.egg-info/requires.txt
--rw-rw-r--   0 ok        (1000) ok        (1000)       10 2021-08-03 12:52:03.000000 screenpen-0.1.9/screenpen.egg-info/top_level.txt
--rw-rw-r--   0 ok        (1000) ok        (1000)       38 2021-08-03 12:52:04.000000 screenpen-0.1.9/setup.cfg
--rw-rw-r--   0 ok        (1000) ok        (1000)     1877 2021-05-13 13:55:50.000000 screenpen-0.1.9/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-08-08 21:24:20.183892 screenpen-0.2.0/
+-rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-01-03 18:20:34.000000 screenpen-0.2.0/LICENSE
+-rw-r--r--   0 ok        (1000) ok        (1000)    35148 2023-01-03 18:20:34.000000 screenpen-0.2.0/LICENSE.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)     3987 2023-08-08 21:24:20.182892 screenpen-0.2.0/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)     2955 2023-08-08 21:17:04.000000 screenpen-0.2.0/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-08-08 21:24:20.170892 screenpen-0.2.0/screenpen/
+-rw-r--r--   0 ok        (1000) ok        (1000)       74 2023-01-03 18:20:34.000000 screenpen-0.2.0/screenpen/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)       76 2023-01-03 18:20:34.000000 screenpen-0.2.0/screenpen/__main__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)    39930 2023-08-08 21:17:04.000000 screenpen-0.2.0/screenpen/screenpen.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-08-08 21:24:20.174892 screenpen-0.2.0/screenpen/utils/
+-rw-r--r--   0 ok        (1000) ok        (1000)        0 2023-08-05 08:20:16.000000 screenpen-0.2.0/screenpen/utils/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)    41586 2023-01-03 18:20:34.000000 screenpen-0.2.0/screenpen/utils/resources.xml
+-rw-r--r--   0 ok        (1000) ok        (1000)    12954 2023-08-08 21:17:04.000000 screenpen-0.2.0/screenpen/utils/syntax.py
+-rw-r--r--   0 ok        (1000) ok        (1000)       22 2023-08-08 21:17:04.000000 screenpen-0.2.0/screenpen/version.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-08-08 21:24:20.182892 screenpen-0.2.0/screenpen.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3987 2023-08-08 21:24:19.000000 screenpen-0.2.0/screenpen.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      424 2023-08-08 21:24:20.000000 screenpen-0.2.0/screenpen.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-08-08 21:24:19.000000 screenpen-0.2.0/screenpen.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       41 2023-08-08 21:24:19.000000 screenpen-0.2.0/screenpen.egg-info/entry_points.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       33 2023-08-08 21:24:19.000000 screenpen-0.2.0/screenpen.egg-info/requires.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       10 2023-08-08 21:24:19.000000 screenpen-0.2.0/screenpen.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-08-08 21:24:20.183892 screenpen-0.2.0/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     2438 2023-01-19 10:04:29.000000 screenpen-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `screenpen-0.1.9/LICENSE` & `screenpen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpen-0.1.9/LICENSE.txt` & `screenpen-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `screenpen-0.1.9/PKG-INFO` & `screenpen-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,84 @@
-Metadata-Version: 2.1
-Name: screenpen
-Version: 0.1.9
-Summary: Screen annotation software which allows drawing directly on the screen.
-Home-page: https://rsusik.github.io/screenpen/
-Author: Robert Susik
-Author-email: robert.susik@gmail.com
-License: GPLv3
-Description: <p align="center">
-            <img src="https://github.com/rsusik/screenpen/raw/master/screenpen.png" alt="ScreenPen" />
-        </p>
-        <p align="center">
-            <em>Multiplatform screen annotation software that allows drawing directly on the screen.</em>
-        </p>
-        <p align="center">
-        <a href="https://pypi.org/project/screenpen" target="_blank">
-            <img src="https://img.shields.io/pypi/v/screenpen?color=%2334D058&label=pypi%20package" alt="Package version">
-        </a>
-        <a href="https://github.com/rsusik/screenpen/blob/master/LICENSE" target="_blank">
-            <img src="https://img.shields.io/github/license/rsusik/screenpen" alt="Package version">
-        </a>
-        </p>
-        
-        ## Description
-        
-        Screen annotation software which allows drawing directly on the screen. It is a free and multiplatform (all systems that support Python) alternative for tools such as Epic Pen. Supported shapes:
-        * line,
-        * rectangle,
-        * chart (using matplotlib).
-        
-        The behavior of the program depends on the OS you use:
-        * For Linux transparent background is used (you can see a video playing in the background).
-        * For Windows, the screenshot is taken, and the user draws on the captured image (you see a static image of the screen).
-        
-        ### Controls
-        * Left mouse button - drawing.
-        * Right mouse button - quit.
-        * Keyboard shortcuts:
-            * `Ctrl+Z` - undo,
-            * `Ctrl+Y` - redo,
-            * hold `Shift` - change mouse cursor icon to arrrow.
-        
-        ### Demo (video)
-        
-        https://user-images.githubusercontent.com/19404835/116938635-5e63a980-ac6b-11eb-818d-7723967e1d94.mp4?s=100
-        
-        
-        *Note: The app is created ad-hoc only for my use case. It may contain bugs, and the code definitely is not clean.*
-        
-        
-        ## Usage
-        
-        Tu run the program:
-        
-        ```bash
-        pip install screenpen
-        screenpen
-        ```
-        
-        
-Platform: UNKNOWN
-Classifier: Environment :: X11 Applications :: Qt
-Classifier: Framework :: Matplotlib
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Communications :: Conferencing
-Classifier: Topic :: Education
-Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
-Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+<p align="center">
+    <img src="https://github.com/rsusik/screenpen/raw/master/screenpen.png" alt="ScreenPen" />
+</p>
+<p align="center">
+    <em>Multiplatform screen annotation software that allows drawing directly on the screen.</em>
+</p>
+<p align="center">
+<a href="https://pypi.org/project/screenpen" target="_blank">
+    <img src="https://img.shields.io/pypi/v/screenpen?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://github.com/rsusik/screenpen/blob/master/LICENSE" target="_blank">
+    <img src="https://img.shields.io/github/license/rsusik/screenpen" alt="License">
+</a>
+<a href="https://pepy.tech/project/screenpen" target="_blank">
+    <img src="https://static.pepy.tech/personalized-badge/screenpen?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Number of downloads">
+</a>
+<a href="https://pepy.tech/project/screenpen" target="_blank">
+    <img src="https://static.pepy.tech/personalized-badge/screenpen?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/month">
+</a>
+</p>
+
+## Description
+
+Screen annotation software which allows drawing directly on the screen. 
+It is an open source and multiplatform 
+(all systems that support Python) 
+alternative to tools such as Epic Pen. 
+Supported shapes:
+* line,
+* rectangle,
+* chart (using matplotlib).
+
+The behavior of the program depends on the Window System you use:
+* if the system supports "live transparency then a transparent background is used (you can see a video playing in the background),
+* if not then the screenshot is taken, and the user draws on the captured image (you see a static image of the screen),
+* sometimes your WM may be detected as not supporting "live transparency". In that case try running with `-t` parameter to force it._
+
+
+### Demo (video)
+
+https://user-images.githubusercontent.com/19404835/130215780-705e4eb9-330b-4a91-bd1f-b9ec3843556e.mp4
+
+
+*Note: The app is created ad-hoc only for my use case. It may contain bugs...*
+
+
+## Usage
+
+### Installation and execution
+
+Tu run the program you need to have Python installed and execute following:
+
+```bash
+pip install screenpen
+screenpen                # or python -m screenpen
+```
+
+**NOTE: Your WM may be detected as not supporting "live transparency". In that case try running with `-t` parameter:**
+
+```bash
+screenpen -t
+```
+
+### Controls
+* Left mouse button - drawing.
+* Right mouse button - quit.
+* Keyboard shortcuts:
+    * `Ctrl+Z` - undo,
+    * `Ctrl+Y` - redo,
+    * hold `Shift` - change mouse cursor icon to arrrow.
+
+### TODO
+
+- [ ] Better Matplotlib charts support.
+
+### Compatilibity notes
+
+Screenpen (from 0.2 version) is compatible with PyQt5 and PyQt6, nevertheless the PyQt5 is currently in the requirements and recommended.
+It is possible to run it using PyQt6 by running:
+```
+pip install screenpen --no-deps
+pip install matplotlib>=3.2 numpy>=1.8 PyQt6
+```
+
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: screenpen Version: 0.1.9 Summary: Screen annotation
-software which allows drawing directly on the screen. Home-page: https://
-rsusik.github.io/screenpen/ Author: Robert Susik Author-email:
-robert.susik@gmail.com License: GPLv3 Description:
                                   [ScreenPen]
  Multiplatform screen annotation software that allows drawing directly on the
                                     screen.
-                      [Package_version] [Package_version]
+ [Package_version] [License] [Number_of_downloads] [https://static.pepy.tech/
+                              personalized-badge/
+screenpen?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/
+                                    month]
 ## Description Screen annotation software which allows drawing directly on the
-screen. It is a free and multiplatform (all systems that support Python)
-alternative for tools such as Epic Pen. Supported shapes: * line, * rectangle,
-* chart (using matplotlib). The behavior of the program depends on the OS you
-use: * For Linux transparent background is used (you can see a video playing in
-the background). * For Windows, the screenshot is taken, and the user draws on
-the captured image (you see a static image of the screen). ### Controls * Left
-mouse button - drawing. * Right mouse button - quit. * Keyboard shortcuts: *
-`Ctrl+Z` - undo, * `Ctrl+Y` - redo, * hold `Shift` - change mouse cursor icon
-to arrrow. ### Demo (video) https://user-images.githubusercontent.com/19404835/
-116938635-5e63a980-ac6b-11eb-818d-7723967e1d94.mp4?s=100 *Note: The app is
-created ad-hoc only for my use case. It may contain bugs, and the code
-definitely is not clean.* ## Usage Tu run the program: ```bash pip install
-screenpen screenpen ``` Platform: UNKNOWN Classifier: Environment :: X11
-Applications :: Qt Classifier: Framework :: Matplotlib Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
-Communications :: Conferencing Classifier: Topic :: Education Classifier: Topic
-:: Multimedia :: Graphics :: Capture :: Screen Capture Classifier: Topic ::
-Multimedia :: Graphics :: Presentation Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+screen. It is an open source and multiplatform (all systems that support
+Python) alternative to tools such as Epic Pen. Supported shapes: * line, *
+rectangle, * chart (using matplotlib). The behavior of the program depends on
+the Window System you use: * if the system supports "live transparency then a
+transparent background is used (you can see a video playing in the background),
+* if not then the screenshot is taken, and the user draws on the captured image
+(you see a static image of the screen), * sometimes your WM may be detected as
+not supporting "live transparency". In that case try running with `-t`
+parameter to force it._ ### Demo (video) https://user-
+images.githubusercontent.com/19404835/130215780-705e4eb9-330b-4a91-bd1f-
+b9ec3843556e.mp4 *Note: The app is created ad-hoc only for my use case. It may
+contain bugs...* ## Usage ### Installation and execution Tu run the program you
+need to have Python installed and execute following: ```bash pip install
+screenpen screenpen # or python -m screenpen ``` **NOTE: Your WM may be
+detected as not supporting "live transparency". In that case try running with
+`-t` parameter:** ```bash screenpen -t ``` ### Controls * Left mouse button -
+drawing. * Right mouse button - quit. * Keyboard shortcuts: * `Ctrl+Z` - undo,
+* `Ctrl+Y` - redo, * hold `Shift` - change mouse cursor icon to arrrow. ###
+TODO - [ ] Better Matplotlib charts support. ### Compatilibity notes Screenpen
+(from 0.2 version) is compatible with PyQt5 and PyQt6, nevertheless the PyQt5
+is currently in the requirements and recommended. It is possible to run it
+using PyQt6 by running: ``` pip install screenpen --no-deps pip install
+matplotlib>=3.2 numpy>=1.8 PyQt6 ```
```

### Comparing `screenpen-0.1.9/screenpen/screenpen.py` & `screenpen-0.2.0/screenpen/screenpen.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,353 @@
 # ----------------------------------------------------------------------------
 # Author:       Robert Susik
 # Email:        robert.susik@gmail.com
 # ----------------------------------------------------------------------------
 
 #from .version import __version__  # noqa: F401,E402
 
+import pkg_resources
+
+try:
+    import PyQt5
+    print("PyQt5 is installed.")
+    pyqt_version = 5
+except ImportError:
+    try:
+        import PyQt6
+        print("PyQt6 is installed.")
+        pyqt_version = 6
+    except ImportError:
+        print("PyQt5 nor PyQt6 is installed.")
+        print("Please install PyQt5 or PyQt6 by running:")
+        print("pip install PyQt5")
+        print("or")
+        print("pip install PyQt6")
+        print("Exiting...")
+        exit(1)
+
+
+try:
+    pkg_resources.get_distribution("PySide6")
+    print('\033[41m', end='')
+    print('=========================> WARNING <===========================')
+    print('>       PySide6 is installed but PyQt5 only is expected.      <')
+    print('>          Errors may appear. Please remove PySide6.          <')
+    print('===============================================================\033[0m')
+except pkg_resources.DistributionNotFound:
+    pass
+
+import subprocess
 import sys
 from datetime import datetime
-from matplotlib.backends.backend_qt5 import ToolbarQt
-from PyQt5 import QtGui
-from PyQt5 import QtWidgets
-from PyQt5 import QtCore
-from PyQt5.QtWidgets import QMainWindow, QApplication, QDesktopWidget
-from PyQt5.QtCore import QPoint, Qt, QSize
-from PyQt5.QtWidgets import QToolBar, QAction, QDialog, QToolButton, QMenu, QColorDialog
-from PyQt5.QtGui import (
-    QIcon, QScreen, QPalette, QColor, QCursor,
-    QSyntaxHighlighter, QPixmap, QKeySequence
-)
-
-
-from PyQt5.QtWidgets import (
-    QApplication, QDialog, QDialogButtonBox, QLabel, QMainWindow,
-    QPushButton, QVBoxLayout, QListWidget, QListWidgetItem, QFormLayout,
-    QHBoxLayout, QGridLayout,
-    QLineEdit, QPlainTextEdit,
-    QShortcut
-)
+
+if pyqt_version == 5:
+    from PyQt5 import QtGui
+    from PyQt5 import QtWidgets
+    from PyQt5 import QtCore
+    from PyQt5.QtWidgets import QMainWindow, QApplication, QDesktopWidget
+    from PyQt5.QtCore import QPoint, Qt, QSize
+    from PyQt5.QtWidgets import QToolBar, QAction, QDialog, QToolButton, QMenu, QColorDialog
+    from PyQt5.QtGui import (
+        QIcon, QScreen, QPalette, QColor, QCursor,
+        QSyntaxHighlighter, QPixmap, QKeySequence
+    )
+
+    from PyQt5.QtWidgets import (
+        QApplication, QDialog, QDialogButtonBox, QLabel, QMainWindow,
+        QPushButton, QVBoxLayout, QListWidget, QListWidgetItem, QFormLayout,
+        QHBoxLayout, QGridLayout,
+        QLineEdit, QPlainTextEdit,
+        QShortcut
+    )
+
+    def _create_palette():
+        return QPalette()
+    
+    PALETTE_PROPS = {
+        'window': QPalette.Window,
+        'windowText': QPalette.WindowText,
+        'base': QPalette.Base,
+        'alternateBase': QPalette.AlternateBase,
+        'toolTipBase': QPalette.ToolTipBase,
+        'toolTipText': QPalette.ToolTipText,
+        'text': QPalette.Text,
+        'button': QPalette.Button,
+        'buttonText': QPalette.ButtonText,
+        'brightText': QPalette.BrightText,
+        'link': QPalette.Link,
+        'highlight': QPalette.Highlight,
+        'highlightedText': QPalette.HighlightedText,
+    }
+
+    def _get_color_from_RGB(r, g, b):
+        return QColor(r, g, b)
+
+    def _set_palette_color(palette, property, value):
+        return palette.setColor(property, value)
+    
+    # _set_palette_color(_create_palette(), PALETTE_PROPS['window'], _get_color_from_RGB(53, 53, 53))
+    
+    ALIGNMENT = {
+        'center': QtCore.Qt.AlignCenter,
+        'left': QtCore.Qt.AlignLeft,
+        'right': QtCore.Qt.AlignRight,
+    }
+
+    COLORS = {
+        'black': Qt.black,
+        'white': Qt.white,
+        'red': Qt.red,
+        'green': Qt.green,
+        'blue': Qt.blue,
+        'cyan': Qt.cyan,
+        'magenta': Qt.magenta,
+        'yellow': Qt.yellow,
+        'gray': Qt.gray,
+        'darkGray': Qt.darkGray,
+        'lightGray': Qt.lightGray,
+        'transparent': Qt.transparent,
+        'darkRed': Qt.darkRed,
+        'darkGreen': Qt.darkGreen,
+        'darkBlue': Qt.darkBlue,
+        'darkCyan': Qt.darkCyan,
+        'darkMagenta': Qt.darkMagenta,
+        'darkYellow': Qt.darkYellow,
+    }
+
+    def _execute_dialog(dlg):
+        return dlg.exec_()
+    
+    WINDOW_ATTRS = {
+        'translucentBackground': QtCore.Qt.WA_TranslucentBackground,
+    }
+
+    IMAGE_FORMATS = {
+        'ARGB32': QtGui.QImage.Format_ARGB32,
+    }
+
+    PEN_STYLES = {
+        'solidLine': Qt.SolidLine,
+        'dashLine': Qt.DashLine,
+        'dotLine': Qt.DotLine,
+        'dashDotLine': Qt.DashDotLine,
+        'roundCap': Qt.RoundCap,
+        'squareCap': Qt.SquareCap,
+        'flatCap': Qt.FlatCap,
+        'roundJoin': Qt.RoundJoin,
+    }
+
+    TOOLBAR_AREAS = {
+        'leftToolBarArea': Qt.LeftToolBarArea,
+        'rightToolBarArea': Qt.RightToolBarArea,
+        'topToolBarArea': Qt.TopToolBarArea,
+        'bottomToolBarArea': Qt.BottomToolBarArea,
+    }
+
+    TOOL_BUTTON_STYLE = {
+        'toolButtonIconOnly': Qt.ToolButtonIconOnly,
+    }
+
+    POPUP_MODE = {
+        'instantPopup': QToolButton.InstantPopup
+    }
+
+    COMPOSITION_MODE = {
+        'source': QtGui.QPainter.CompositionMode_Source,
+        'source_over': QtGui.QPainter.CompositionMode_SourceOver,
+    }
+
+    BUTTONS = {
+        'left': Qt.LeftButton,
+        'right': Qt.RightButton,
+        'middle': Qt.MiddleButton,
+    }
+
+    BRUSHES = {
+        'no_brush': Qt.NoBrush,
+    }
+
+    CURSORS = {
+        'arrow_cursor': Qt.ArrowCursor,
+    }
+
+    KEYS = {
+        'escape': Qt.Key_Escape,
+        'enter': Qt.Key_Enter,
+        'return': Qt.Key_Return,
+        'shift': Qt.Key_Shift,
+    }
+
+    def _path_move_to(path, point):
+        return path.moveTo(point)
+    
+    def _path_cubic_to(path, point1, point2, point3):
+        return path.cubicTo(point1, point2, point3)
+    
+    DIALOG_BUTTONS = {
+        'ok': QDialogButtonBox.Ok,
+        'cancel': QDialogButtonBox.Cancel,
+    }
+
+
+elif pyqt_version == 6:
+    from PyQt6 import QtGui
+    from PyQt6 import QtWidgets
+    from PyQt6 import QtCore
+    from PyQt6.QtWidgets import QMainWindow, QApplication #, QDesktopWidget
+    from PyQt6.QtCore import QPoint, Qt, QSize
+    from PyQt6.QtWidgets import QToolBar, QDialog, QToolButton, QMenu, QColorDialog
+    from PyQt6.QtGui import (
+        QGuiApplication,
+        QIcon, QScreen, QPalette, QColor, QCursor,
+        QSyntaxHighlighter, QPixmap, QKeySequence,
+        QAction, QShortcut
+    )
+
+    from PyQt6.QtWidgets import (
+        QApplication, QDialog, QDialogButtonBox, QLabel, QMainWindow,
+        QPushButton, QVBoxLayout, QListWidget, QListWidgetItem, QFormLayout,
+        QHBoxLayout, QGridLayout,
+        QLineEdit, QPlainTextEdit,
+        #QShortcut
+    )
+
+    def _create_palette():
+        return QPalette()
+
+    PALETTE_PROPS = {
+        'window': 'window',
+        'windowText': 'windowText',
+        'base': 'base',
+        'alternateBase': 'alternateBase',
+        'toolTipBase': 'toolTipBase',
+        'toolTipText': 'toolTipText',
+        'text': 'text',
+        'button': 'button',
+        'buttonText': 'buttonText',
+        'brightText': 'brightText',
+        'link': 'link',
+        'highlight': 'highlight',
+        'highlightedText': 'highlightedText',
+    }
+
+
+    def _get_color_from_RGB(r, g, b):
+        return QColor(r, g, b)
+
+    def _set_palette_color(palette, property, value):
+        return getattr(palette, property)().setColor(value)
+
+    # _set_palette_color(_create_palette(), PALETTE_PROPS['window'], _get_color_from_RGB(53, 53, 53))
+
+    ALIGNMENT = {
+        'center': Qt.AlignmentFlag.AlignCenter,
+        'left': Qt.AlignmentFlag.AlignLeft,
+        'right': Qt.AlignmentFlag.AlignRight,
+    }
+
+    COLORS = {
+        'black': QtGui.QColorConstants.Black,
+        'white': QtGui.QColorConstants.White,
+        'red': QtGui.QColorConstants.Red,
+        'green': QtGui.QColorConstants.Green,
+        'blue': QtGui.QColorConstants.Blue,
+        'cyan': QtGui.QColorConstants.Cyan,
+        'magenta': QtGui.QColorConstants.Magenta,
+        'yellow': QtGui.QColorConstants.Yellow,
+        'gray': QtGui.QColorConstants.Gray,
+        'darkGray': QtGui.QColorConstants.DarkGray,
+        'lightGray': QtGui.QColorConstants.LightGray,
+        'transparent': QtGui.QColorConstants.Transparent,
+        'darkRed': QtGui.QColorConstants.DarkRed,
+        'darkGreen': QtGui.QColorConstants.DarkGreen,
+        'darkBlue': QtGui.QColorConstants.DarkBlue,
+        'darkCyan': QtGui.QColorConstants.DarkCyan,
+        'darkMagenta': QtGui.QColorConstants.DarkMagenta,
+        'darkYellow': QtGui.QColorConstants.DarkYellow,
+    }
+
+    def _execute_dialog(dlg):
+        return dlg.exec()
+    
+    WINDOW_ATTRS = {
+        'translucentBackground': QtCore.Qt.WidgetAttribute.WA_TranslucentBackground,
+    }
+    
+    IMAGE_FORMATS = {
+        'ARGB32': QtGui.QImage.Format.Format_ARGB32,
+    }
+
+    PEN_STYLES = {
+        'solidLine': QtCore.Qt.PenStyle.SolidLine,
+        'dashLine': QtCore.Qt.PenStyle.DashLine,
+        'dotLine': QtCore.Qt.PenStyle.DotLine,
+        'dashDotLine': QtCore.Qt.PenStyle.DashDotLine,
+        'roundCap': QtCore.Qt.PenCapStyle.RoundCap,
+        'squareCap': QtCore.Qt.PenCapStyle.SquareCap,
+        'flatCap': QtCore.Qt.PenCapStyle.FlatCap,
+        'roundJoin': QtCore.Qt.PenJoinStyle.RoundJoin,
+    }
+
+    TOOLBAR_AREAS = {
+        'leftToolBarArea': Qt.ToolBarArea.LeftToolBarArea,
+        'rightToolBarArea': Qt.ToolBarArea.RightToolBarArea,
+        'topToolBarArea': Qt.ToolBarArea.TopToolBarArea,
+        'bottomToolBarArea': Qt.ToolBarArea.BottomToolBarArea,
+    }
+
+    TOOL_BUTTON_STYLE = {
+        'toolButtonIconOnly': QtCore.Qt.ToolButtonStyle.ToolButtonIconOnly,
+    }
+
+    POPUP_MODE = {
+        'instantPopup': QtWidgets.QToolButton.ToolButtonPopupMode.InstantPopup
+    }
+
+    COMPOSITION_MODE = {
+        'source': QtGui.QPainter.CompositionMode.CompositionMode_Source,
+        'source_over': QtGui.QPainter.CompositionMode.CompositionMode_SourceOver,
+    }
+
+    BUTTONS = {
+        'left': QtCore.Qt.MouseButton.LeftButton,
+        'right': QtCore.Qt.MouseButton.RightButton,
+        'middle': QtCore.Qt.MouseButton.MiddleButton,
+    }
+
+    BRUSHES = {
+        'no_brush': QtCore.Qt.BrushStyle.NoBrush,
+    }
+
+    CURSORS = {
+        'arrow_cursor': QtCore.Qt.CursorShape.ArrowCursor,
+    }
+
+    KEYS = {
+        'escape': QtCore.Qt.Key.Key_Escape,
+        'enter': QtCore.Qt.Key.Key_Enter,
+        'return': QtCore.Qt.Key.Key_Return,
+        'shift': QtCore.Qt.Key.Key_Shift,
+    }
+
+    def _path_move_to(path, point):
+        path.moveTo(point.x(), point.y())
+
+    def _path_cubic_to(path, point1, point2, point3):
+        return path.cubicTo(
+            point1.x(), point1.y(), 
+            point2.x(), point2.y(), 
+            point3.x(), point3.y(), 
+        )
+    
+    DIALOG_BUTTONS = {
+        'ok': QDialogButtonBox.StandardButton.Ok,
+        'cancel': QDialogButtonBox.StandardButton.Cancel,
+    }
+    
 
 import numpy as np
 import platform
 from datetime import datetime
 from xml.dom import minidom
 import os
 from types import SimpleNamespace
@@ -43,54 +360,49 @@
     from matplotlib.backends.backend_qt5agg import (
         FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
 else:
     from matplotlib.backends.backend_qt4agg import (
         FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
 from matplotlib.figure import Figure
 
-#from pkg_resources import resource_filename, Requirement
+from screenpen.version import __version__
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 syntax_py_path = f'{dir_path}/utils/syntax.py'
 spec = importlib.util.spec_from_file_location('syntax', syntax_py_path)
 syntax = importlib.util.module_from_spec(spec)
 sys.modules['syntax'] = syntax
 spec.loader.exec_module(syntax)
 
 class ScreenPenWindow(QMainWindow):
-    def __init__(self, screen, screen_geom, pixmap: QtGui.QPixmap = None): # app: QApplication
+    def __init__(self, screen, screen_geom, pixmap: QtGui.QPixmap = None, transparent_background = True): # app: QApplication
         super().__init__()
 
         # PATHS
         try:
             prefix = sys._MEIPASS
             resources_xml_path = os.path.join(prefix, 'utils/resources.xml')
         except Exception:
-            prefix = '' #os.path.abspath(".")
-            #utils_path = resource_filename(Requirement.parse('screenpen'), "utils")
+            prefix = ''
             dir_path = os.path.dirname(os.path.realpath(__file__))
             resources_xml_path = f'{dir_path}/utils/resources.xml'
-        #resources_xml_path = f'{utils_path}/resources.xml'
-        # resources_xml_path = f'./utils/resources.xml'
-        # print(__file__)
-        # print(Requirement.parse('screenpen'))
-        # print(resource_filename(Requirement.parse('screenpen'), "utils"))
 
         
 
         self.files = SimpleNamespace(
             resources_xml = resources_xml_path
         )
         
         self.screen = screen
         self.screen_pixmap = pixmap
         self.screen_geom = screen_geom
+        self.transparent_background = transparent_background
 
-        if platform.system() == 'Linux':
-            self.setAttribute(Qt.WA_TranslucentBackground)
+        if self.transparent_background:
+            self.setAttribute(WINDOW_ATTRS['translucentBackground'])
         self.move(screen_geom.topLeft())
         self.setGeometry(screen_geom)
         self.activateWindow()
         self.showFullScreen()
         self._createCanvas()
         self._clearCanvas()
         
@@ -99,18 +411,18 @@
 
         self.begin = QtCore.QPoint()
         self.end = QtCore.QPoint()
         self.lastPoint = QtCore.QPoint()
 
         self.drawing = False
         self.curr_method = 'drawPath'
-        self.curr_color = Qt.red
-        self.curr_style = Qt.SolidLine
-        self.curr_capstyle = Qt.RoundCap
-        self.curr_joinstyle = Qt.RoundJoin
+        self.curr_color = COLORS['red']
+        self.curr_style = PEN_STYLES['solidLine']
+        self.curr_capstyle = PEN_STYLES['roundCap']
+        self.curr_joinstyle = PEN_STYLES['roundJoin']
         self.curr_width = 3
         self.curr_br = QtGui.QBrush(self.curr_color)
         self.curr_pen = QtGui.QPen()
         self._setupTools()
         self._setupIcons()
         self._setupCodes()
         self._createToolBars()
@@ -124,32 +436,32 @@
         if hotx is None:
             hotx = 2
         if hoty is None:
             hoty = 2
         if type(cursor) == str:
             pixm = QtGui.QPixmap.fromImage(QtGui.QImage.fromData(bytes(self._applySvgConfig(self._icons[cursor], None), encoding='utf-8')))
             pixm = pixm.scaled(QSize(32, 32))
-            self.setCursor(QCursor(pixm, hotx, hoty))
+            self.setCursor(QCursor(pixm, int(hotx), int(hoty)))
         elif type(cursor) == Qt.CursorShape:
             self.setCursor(QCursor(cursor))
         elif type(cursor) == QPixmap:
-            self.setCursor(QCursor(cursor, hotx, hoty))
+            self.setCursor(QCursor(cursor, int(hotx), int(hoty)))
 
     def keyPressEvent(self, event):
         if event.isAutoRepeat():
             return
         k = event.key()
-        if (k==Qt.Key_Shift):
+        if (k==KEYS['shift']):
             self._setCursor('arrow2')
 
     def keyReleaseEvent(self, event):
         if event.isAutoRepeat():
             return
         k = event.key()
-        if (k==Qt.Key_Shift):
+        if (k==KEYS['shift']):
             self._setCursor(Qt.ArrowCursor)
 
     def _setupIcons(self):
         self._icons = {}
         try:
             DOMTree = minidom.parse(self.files.resources_xml)
             icons = DOMTree.getElementsByTagName('icon')
@@ -196,38 +508,38 @@
             parsed = parsed.replace(f'{{{el}}}', colors_dict[el])
         return parsed
 
     def _getIcon(self, name, custom_colors_dict=None):
         return QIcon(QtGui.QPixmap.fromImage(QtGui.QImage.fromData(bytes(self._applySvgConfig(self._icons[name], custom_colors_dict), encoding='utf-8'))))
 
     def _createCanvas(self):
-        self.background = QtGui.QImage(self.size(), QtGui.QImage.Format_ARGB32)
-        self.imageDraw = QtGui.QImage(self.size(), QtGui.QImage.Format_ARGB32)
-        self.imageDraw_bck = QtGui.QImage(self.size(), QtGui.QImage.Format_ARGB32)
+        self.background = QtGui.QImage(self.size(), IMAGE_FORMATS['ARGB32'])
+        self.imageDraw = QtGui.QImage(self.size(), IMAGE_FORMATS['ARGB32'])
+        self.imageDraw_bck = QtGui.QImage(self.size(), IMAGE_FORMATS['ARGB32'])
         self._clearBackground()
         
     def _clearBackground(self): # make background transparent
-        if platform.system() == 'Linux':
-            self.background.fill(QtCore.Qt.transparent)
+        if self.transparent_background:
+            self.background.fill(COLORS['transparent'])
         else:
             qp2 = QtGui.QPainter(self.background)
             qp2.drawPixmap(self.background.rect(), self.screen_pixmap, self.screen_pixmap.rect())
             qp2.end()
         self.update()
 
     def _clearCanvas(self):
-        self.imageDraw.fill(QtCore.Qt.transparent)
-        self.imageDraw_bck.fill(QtCore.Qt.transparent)
+        self.imageDraw.fill(COLORS['transparent'])
+        self.imageDraw_bck.fill(COLORS['transparent'])
         self.update()
 
     def drawMatplotlib(self, qp:QtGui.QPainter, canvas:FigureCanvas, p1:QtCore.QPoint):
         size = canvas.size()
         width, height = size.width(), size.height()
-        im = QtGui.QImage(canvas.buffer_rgba(), width, height, QtGui.QImage.Format_ARGB32).rgbSwapped()
-        p2 = QtCore.QPoint(p1.x()+width, p1.y()+height) 
+        im = QtGui.QImage(canvas.buffer_rgba(), width, height, IMAGE_FORMATS['ARGB32']).rgbSwapped()
+        p2 = QtCore.QPoint(int(p1.x()+width), int(p1.y()+height))
         qp.drawImage(QtCore.QRect(
             p1, 
             p2
         ), im, im.rect())
         
 
     def _setupTools(self):
@@ -240,36 +552,36 @@
 
     def setColor(self, color):
         def _setColor():
             self.curr_color = color
             self._setupTools()
         return _setColor
 
-    def _getEraserPen(self, color=Qt.transparent, size=30):
+    def _getEraserPen(self, color=COLORS['transparent'], size=30):
         pen = QtGui.QPen()
         pen.setBrush(QtGui.QBrush(color))
-        pen.setStyle(Qt.SolidLine) ; pen.setCapStyle(Qt.RoundCap) 
-        pen.setJoinStyle(Qt.RoundJoin) ; pen.setWidth(size)
+        pen.setStyle(PEN_STYLES['solidLine']) ; pen.setCapStyle(PEN_STYLES['roundCap']) 
+        pen.setJoinStyle(PEN_STYLES['roundJoin']) ; pen.setWidth(size)
         return pen
 
     def setEraser(self):
         def _setEraser():
             pix = QPixmap()
-            img = QtGui.QImage(QSize(32, 32), QtGui.QImage.Format_ARGB32)
-            img.fill(Qt.transparent)
+            img = QtGui.QImage(QSize(32, 32), IMAGE_FORMATS['ARGB32'])
+            img.fill(COLORS['transparent'])
             qp = QtGui.QPainter(img)
             qp.setPen(self._getEraserPen(QColor('#7acfe6'), 30))
             path = QtGui.QPainterPath()
-            path.moveTo(QPoint(16, 16))
-            path.cubicTo(QPoint(16, 17), QPoint(16, 16), QPoint(16, 16))
+            _path_move_to(path, QPoint(16, 16))
+            _path_cubic_to(path, QPoint(16, 17), QPoint(16, 16), QPoint(16, 16))
             qp.drawPath(path)
             qp.setPen(self._getEraserPen(QColor('#eccdec'), 26))
             path = QtGui.QPainterPath()
-            path.moveTo(QPoint(16, 16))
-            path.cubicTo(QPoint(16, 17), QPoint(16, 16), QPoint(16, 16))
+            _path_move_to(path, QPoint(16, 16))
+            _path_cubic_to(path, QPoint(16, 17), QPoint(16, 16), QPoint(16, 16))
             qp.drawPath(path)
             qp.end()
             pix = pix.fromImage(img)
             self.setAction('drawEraser')()
             self._setCursor(pix, 16, 16)
             self._setupTools()
         return _setEraser
@@ -286,15 +598,15 @@
             self._setupTools()
         return _setWidth
 
     def setAction(self, action, cursor=None):
         def _setAction():
             self.curr_method = action
             if cursor is None:
-                self._setCursor(Qt.ArrowCursor)
+                self._setCursor(CURSORS['arrow_cursor'])
         return _setAction
 
     class ChartDialog(QDialog):
         def ok_success(self, *args):
             sourcecode = '\n'.join(list(map(lambda x: f'    {x}', self.code.toPlainText().replace('\t', '').replace(' ', '').splitlines())))
             self.code = f'''
 def drawChart(qp:QtGui.QPainter, p1:QtCore.QPoint):
@@ -313,15 +625,17 @@
             self.accept()
 
         def __init__(self, parent):
             super().__init__(parent=parent)
             self.parent = parent
             self.setWindowTitle("Chart")
 
-            QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+
+
+            QBtn = DIALOG_BUTTONS['ok'] | DIALOG_BUTTONS['cancel']
 
             self.buttonBox = QDialogButtonBox(QBtn)
             self.buttonBox.accepted.connect(self.ok_success)
             self.buttonBox.rejected.connect(self.reject)
             
             self.resize(800, 600)
             self.code    = QPlainTextEdit()
@@ -350,17 +664,17 @@
             self.layout.addLayout(codelay)
             self.layout.addLayout(buttons)
 
             self.setLayout(self.layout)
 
     def showChart(self):
         def _showChart():
-            self._setCursor(Qt.ArrowCursor)
+            self._setCursor(CURSORS['arrow_cursor'])
             dlg = self.ChartDialog(self)
-            if dlg.exec_():
+            if _execute_dialog(dlg):
                 self.curr_method = 'drawChart'
             else:
                 pass
         
         return _showChart
 
     def removeDrawing(self):
@@ -380,14 +694,15 @@
         for tb in self.toolBars:
             tb.show()
         return img
 
     def saveDrawing(self):
         def _saveDrawing(n=0):
             filename = f'{datetime.now().strftime("%Y%m%d_%H%M%S")}.png'
+            print(f'Saving {filename}')
             self.captureScreen().save(f'{filename}')
         return _saveDrawing
 
     def colorPicker(self):
         def _colorPicker():
             color = QColorDialog.getColor()
 
@@ -407,27 +722,27 @@
         boardToolBar = QToolBar("Color", self)
         boardToolBar.setIconSize(QSize(50, 50))
         actionBar = QToolBar("Action", self)
         actionBar.setIconSize(QSize(50, 50))
         self.toolBars = [penToolBar, boardToolBar, actionBar]
         self.addToolBar(penToolBar)
         self.addToolBar(boardToolBar)
-        self.addToolBar(Qt.LeftToolBarArea, actionBar)
+        self.addToolBar(TOOLBAR_AREAS['leftToolBarArea'], actionBar)
         
         avail_colors = {
-            'red': Qt.red,
-            'green': Qt.green,
-            'blue': Qt.blue,
-            'cyan': Qt.cyan,
-            'magenta': Qt.magenta,
-            'yellow': Qt.yellow,
-            'black': Qt.black,
-            'white': Qt.white,
-            'orange': QColor('#ff8000'),
-            'gray': QColor('#808080'),
+            'red': COLORS['red'],
+            'green': COLORS['green'],
+            'blue': COLORS['blue'],
+            'cyan': COLORS['cyan'],
+            'magenta': COLORS['magenta'],
+            'yellow': COLORS['yellow'],
+            'black': COLORS['black'],
+            'white': COLORS['white'],
+            'orange': _get_color_from_RGB(255, 165, 0),
+            'gray': _get_color_from_RGB(128, 128, 128),
         }
 
         for acol in avail_colors:
             penToolBar.addAction(
                 self.addAction(f'{acol}', self._getIcon('rect_filled', {'FILL': acol, 'STROKE': 'none'}), self.setColor(avail_colors[acol]))
             )
         
@@ -439,77 +754,79 @@
         actionBar.addAction(self.addAction("Line", self._getIcon('line'), self.setAction('drawLine')))
         actionBar.addAction(self.addAction("Point", self._getIcon('dot'), self.setAction('drawDot')))
         actionBar.addAction(self.addAction("Matplotlib chart", self._getIcon('mpl'), self.showChart()))
         
         
 
         lineTypeMenu = QMenu()
-        lineTypeMenu.addAction(self.addAction('Solid', self._getIcon('line'), self.setStyle(Qt.SolidLine)))
-        lineTypeMenu.addAction(self.addAction('Dashed', self._getIcon('line_dashed'), self.setStyle(Qt.DashLine)))
+        lineTypeMenu.addAction(self.addAction('Solid', self._getIcon('line'), self.setStyle(PEN_STYLES['solidLine'])))
+        lineTypeMenu.addAction(self.addAction('Dashed', self._getIcon('line_dashed'), self.setStyle(PEN_STYLES['dashLine'])))
         lineTypeButton = QToolButton(self)
-        lineTypeButton.setToolButtonStyle(Qt.ToolButtonIconOnly)
+        lineTypeButton.setToolButtonStyle(TOOL_BUTTON_STYLE['toolButtonIconOnly'])
         lineTypeButton.setIcon(self._getIcon('line_type'))
-        lineTypeButton.setPopupMode(QToolButton.InstantPopup) # MenuButtonPopup
+        lineTypeButton.setPopupMode(POPUP_MODE['instantPopup']) # MenuButtonPopup
         lineTypeButton.setMenu(lineTypeMenu)
         lineTypeButton.setToolTip('Line type')
         actionBar.addWidget(lineTypeButton)
 
         lineWidthMenu = QMenu()
         lineWidthMenu.addAction(self.addAction('Thin', self._getIcon('line_thin'), self.setWidth(width=3)))
         lineWidthMenu.addAction(self.addAction('Medium', self._getIcon('line_medium'), self.setWidth(width=15)))
         lineWidthMenu.addAction(self.addAction('Thick', self._getIcon('line_thick'), self.setWidth(width=25)))
         lineWidthButton = QToolButton(self)
-        lineWidthButton.setToolButtonStyle(Qt.ToolButtonIconOnly)
+        lineWidthButton.setToolButtonStyle(TOOL_BUTTON_STYLE['toolButtonIconOnly'])
         lineWidthButton.setIcon(self._getIcon('line_width'))
-        lineWidthButton.setPopupMode(QToolButton.InstantPopup)
+        lineWidthButton.setPopupMode(POPUP_MODE['instantPopup'])
         lineWidthButton.setMenu(lineWidthMenu)
         lineWidthButton.setToolTip('Line width')
         actionBar.addWidget(lineWidthButton)
-        boardToolBar.addAction(self.addAction("Whiteboard", self._getIcon('board', custom_colors_dict={'FILL': 'white'}), self.setupBoard(Qt.white)))
-        boardToolBar.addAction(self.addAction("Blackboard", self._getIcon('board', custom_colors_dict={'FILL': 'black'}), self.setupBoard(Qt.black)))
+        boardToolBar.addAction(self.addAction("Whiteboard", self._getIcon('board', custom_colors_dict={'FILL': 'white'}), self.setupBoard(COLORS['white'])))
+        boardToolBar.addAction(self.addAction("Blackboard", self._getIcon('board', custom_colors_dict={'FILL': 'black'}), self.setupBoard(COLORS['black'])))
         boardToolBar.addAction(self.addAction("Transparent", self._getIcon('board_transparent', custom_colors_dict={'FILL': 'black'}), self._clearBackground))
         boardToolBar.addAction(self.addAction("Remove drawings", self._getIcon('remove'), self.removeDrawing()))
         
         actionBar.addAction(self.addAction("Save image", self._getIcon('save'), self.saveDrawing())) # self.style().standardIcon(QtWidgets.QStyle.SP_DialogSaveButton)
 
         
     def scaleCoords(self, coords):
         canvas_size = self.imageDraw.size()
         window_size = self.size()
         x_scale = canvas_size.width() / window_size.width()
         y_scale = canvas_size.height() / window_size.height()
-        return QtCore.QPoint(coords.x()*x_scale, coords.y()*y_scale)
+        return QtCore.QPoint(int(coords.x()*x_scale), int(coords.y()*y_scale))
 
     def paintEvent(self, event):
         self._setupTools()
 
         qp = QtGui.QPainter(self.imageDraw)
         canvasPainter = QtGui.QPainter(self)
 
-        qp.setCompositionMode (QtGui.QPainter.CompositionMode_Source)
-        canvasPainter.setCompositionMode (QtGui.QPainter.CompositionMode_SourceOver)
 
-        if Qt.LeftButton and self.drawing:
+
+        qp.setCompositionMode(COMPOSITION_MODE['source'])
+        canvasPainter.setCompositionMode(COMPOSITION_MODE['source_over'])
+
+        if BUTTONS['left'] and self.drawing:
             qp.setPen(self.curr_pen)
             qp.setBrush(self.curr_br)
             if self.curr_method in ['drawRect']:
-                qp.setBrush(Qt.NoBrush)
+                qp.setBrush(BRUSHES['no_brush'])
                 self.curr_args = [QtCore.QRect(self.begin, self.end)]
                 qp.drawImage(self.imageDraw.rect(), self.imageDraw_bck, self.imageDraw_bck.rect())
                 
                 getattr(qp, self.curr_method)(*self.curr_args)
                 qp.setBrush(self.curr_br)
             elif self.curr_method in ['drawDot']:
                 self.curr_args = [self.end, 10, 10]
                 qp.drawImage(self.imageDraw.rect(), self.imageDraw_bck, self.imageDraw_bck.rect())
                 
                 getattr(qp, 'drawEllipse')(*self.curr_args)
 
             elif self.curr_method in ['drawLine']:
-                qp.setBrush(Qt.NoBrush)
+                qp.setBrush(BRUSHES['no_brush'])
                 self.curr_args = [self.begin, self.end]
                 qp.drawImage(self.imageDraw.rect(), self.imageDraw_bck, self.imageDraw_bck.rect())
                 
                 getattr(qp, self.curr_method)(*self.curr_args)
                 qp.setBrush(self.curr_br)
 
             elif self.curr_method in ['drawChart']:
@@ -526,62 +843,62 @@
                     self.curr_method = 'drawPath'
                     self.update()
                     return
 
 
             elif self.curr_method in ['drawPath']:
                 if self.lastPoint != self.end:
-                    qp.setBrush(Qt.NoBrush)
+                    qp.setBrush(BRUSHES['no_brush'])
                     qp.setPen(self.curr_pen)
-                    self.path.cubicTo(self.end, self.end, self.end)
+                    _path_cubic_to(self.path, self.end, self.end, self.end)
                     self.curr_args = [self.path]
                     getattr(qp, self.curr_method)(*self.curr_args)
                     self.lastPoint = self.end
                     self.update()
                     qp.setBrush(self.curr_br)
 
             elif self.curr_method in ['drawEraser']:
                 if self.lastPoint != self.end:
-                    qp.setBrush(Qt.NoBrush)
-                    qp.setPen(self._getEraserPen(Qt.transparent))
-                    self.path.cubicTo(self.end, self.end, self.end)
+                    qp.setBrush(BRUSHES['no_brush'])
+                    qp.setPen(self._getEraserPen(COLORS['transparent']))
+                    _path_cubic_to(self.path, self.end, self.end, self.end)
                     self.curr_args = [self.path]
                     getattr(qp, 'drawPath')(*self.curr_args)
                     self.lastPoint = self.end
                     self.update()
                     qp.setBrush(self.curr_br)
 
-        qp.setCompositionMode (QtGui.QPainter.CompositionMode_SourceOver)
+        qp.setCompositionMode(COMPOSITION_MODE['source_over'])
         qp.end()
         
         canvasPainter.drawImage(self.rect(), self.background, self.background.rect())
         canvasPainter.drawImage(self.rect(), self.imageDraw, self.imageDraw.rect())
-        canvasPainter.setCompositionMode (QtGui.QPainter.CompositionMode_SourceOver)
+        canvasPainter.setCompositionMode(COMPOSITION_MODE['source_over'])
         canvasPainter.end()
 
 
     def mousePressEvent(self, event):
-        if event.button() == Qt.RightButton:
+        if event.button() == BUTTONS['right']:
             sys.exit(0)
             
-        if event.button() == Qt.LeftButton and self.childAt(event.pos()) is None:
+        if event.button() == BUTTONS['left'] and self.childAt(event.pos()) is None:
             self.drawing = True
 
         if self.curr_method in ['drawRect', 'drawChart', 'drawLine', 'drawDot']:
             qp = QtGui.QPainter(self.imageDraw_bck)
             qp.drawImage(self.imageDraw_bck.rect(), self.imageDraw, self.imageDraw.rect())
             qp.end()
             self.begin = self.scaleCoords(event.pos())
             self.end = self.scaleCoords(event.pos())
             
         elif self.curr_method in ['drawPath', 'drawEraser']:
             self.path = QtGui.QPainterPath()
             self.begin = self.scaleCoords(event.pos())
             self.end = self.scaleCoords(event.pos())
-            self.path.moveTo(self.begin)
+            _path_move_to(self.path, self.begin)
             self.lastPoint = self.scaleCoords(event.pos())
         self.update()
 
     def mouseMoveEvent(self, event):
         self.end = self.scaleCoords(event.pos())
         self.update()
 
@@ -613,35 +930,35 @@
         def redo(self):
             if self.current + 1 < len(self):
                 self.current += 1
             return self[self.current]
             
     def drawPixmap(self, p):
         qp = QtGui.QPainter(self.imageDraw)
-        qp.setCompositionMode (QtGui.QPainter.CompositionMode_Source)
+        qp.setCompositionMode (COMPOSITION_MODE['source'])
         qp.drawPixmap(self.imageDraw.rect(), p, p.rect())
         qp.end()
 
         qp2 = QtGui.QPainter(self.imageDraw_bck)
-        qp2.setCompositionMode (QtGui.QPainter.CompositionMode_Source)
+        qp2.setCompositionMode (COMPOSITION_MODE['source'])
         qp2.drawPixmap(self.imageDraw_bck.rect(), p, p.rect())
         qp2.end()
 
     def undo(self):
         p = self.history.undo()
         self.drawPixmap(p)
         self.update()
 
     def redo(self):
         p = self.history.redo()
         self.drawPixmap(p)
         self.update()
 
     def mouseReleaseEvent(self, event):
-        if event.button() == Qt.LeftButton and self.drawing == True:
+        if event.button() == BUTTONS['left'] and self.drawing == True:
             self.drawing = False
             self.path = None
 
             self.begin = self.scaleCoords(event.pos())
             self.end = self.scaleCoords(event.pos())
 
             self.update()
@@ -654,20 +971,23 @@
         def _setupBoard():
             self.background.fill(color)
             self.update()
         return _setupBoard
 
 
 def _grab_screen(screen_idx, screen):
-    screen_geom = QDesktopWidget().screenGeometry(screen_idx)
+    if pyqt_version == 5:
+        screen_geom = QDesktopWidget().screenGeometry(screen_idx)
+    else:
+        screen_geom = QGuiApplication.screens()[screen_idx].geometry()
+
     return (
         screen_geom, 
-        QScreen.grabWindow(
-            screen, 
-            QApplication.desktop().winId(), 
+        screen.grabWindow(
+            0, 
             screen_geom.x(), 
             screen_geom.y(), 
             screen.size().width(), 
             screen.size().height()
         )
     )
     
@@ -675,80 +995,96 @@
 def _get_screens(app):
     screens = []
     for screen_idx, screen in enumerate(app.screens()):
         screen_geom, screen_pixmap = _grab_screen(screen_idx, screen)
         screens.append([screen, screen_geom, screen_pixmap])
     return screens
 
+
+def _is_transparency_supported():
+    warn = 'INFO: Your system may support transparency but we cannot detect it. You may try to use -t parameter to force it.'
+    try:
+        if platform.system() == 'Linux':
+            return '_NET_WM_WINDOW_OPACITY' in subprocess.run("xprop -root", shell=True, stdout=subprocess.PIPE).stdout.decode()
+        else:
+            print(warn)
+            return False
+    except:
+        print(warn)
+        return False
+
+
 def show_screen_selection(screens):
     number_of_screens = len(screens)
     def _getScreenButton(pixmap, label):
         btn = QPushButton()
         ico = QIcon(pixmap)
         btn.setIcon(ico)
-        btn.setIconSize(QSize(160, 160/(pixmap.rect().width()/pixmap.rect().height())))
+        btn.setIconSize(QSize(int(160), int(160//(pixmap.rect().width()/pixmap.rect().height()))))
 
         shad = QtWidgets.QGraphicsDropShadowEffect()
         shad.setOffset(-10, 10)
-        shad.setColor(Qt.black)
+        shad.setColor(COLORS['black'])
 
         lay = QVBoxLayout(btn)
         lbl = QtWidgets.QLabel()
         lbl.setContentsMargins(0, 0, 0, 0)
-        lbl.setStyleSheet("""color : white; font-weight:6000;""")
+        lbl.setStyleSheet("""color : white; font-weight:1000;""")
         lbl.setText(label)
         lbl.setGraphicsEffect(shad)
-        lay.addWidget(lbl, alignment=QtCore.Qt.AlignCenter)
+        lay.addWidget(lbl, alignment=ALIGNMENT['center'])
         return btn
 
     dlg = QDialog()
     dlg.layout = QGridLayout()
-    dlg.layout.addWidget(QLabel('Select the screen') , 0, 0, 1, number_of_screens, alignment=QtCore.Qt.AlignCenter)
+    dlg.layout.addWidget(QLabel('Select the screen') , 0, 0, 1, number_of_screens, alignment=ALIGNMENT['center'])
 
     def _getBtnAction(idx):
         def act():
             dlg.done(idx)
         return act
 
     for idx, scr in enumerate(screens):
         screen, screen_geom, screen_pixmap = scr
         label = f'Screen {idx+1}' if idx > 0 else f'Main screen'
         btn = _getScreenButton(screen_pixmap, label)
         btn.released.connect(_getBtnAction(idx+1))
         dlg.layout.addWidget(btn , 1, idx)
     dlg.setLayout(dlg.layout)
-    return dlg.exec_()
+    return _execute_dialog(dlg)
 
 def _setPalette(app):
-    palette = QPalette()
-    palette.setColor(QPalette.Window, QColor(53, 53, 53))
-    palette.setColor(QPalette.WindowText, Qt.white)
-    palette.setColor(QPalette.Base, QColor(25, 25, 25))
-    palette.setColor(QPalette.AlternateBase, QColor(53, 53, 53))
-    palette.setColor(QPalette.ToolTipBase, Qt.black)
-    palette.setColor(QPalette.ToolTipText, Qt.white)
-    
-    palette.setColor(QPalette.Text, Qt.white)
-    palette.setColor(QPalette.Button, QColor(53, 53, 53))
-    palette.setColor(QPalette.ButtonText, Qt.white)
-    palette.setColor(QPalette.BrightText, Qt.red)
-    palette.setColor(QPalette.Link, QColor(42, 130, 218))
-    palette.setColor(QPalette.Highlight, QColor(42, 130, 218))
-    palette.setColor(QPalette.HighlightedText, Qt.black)
+    palette = _create_palette()
+    _set_palette_color(palette, PALETTE_PROPS['window'], _get_color_from_RGB(53, 53, 53))
+    _set_palette_color(palette, PALETTE_PROPS['windowText'], COLORS['white'])
+    _set_palette_color(palette, PALETTE_PROPS['base'], _get_color_from_RGB(25, 25, 25))
+    _set_palette_color(palette, PALETTE_PROPS['alternateBase'], _get_color_from_RGB(53, 53, 53))
+    _set_palette_color(palette, PALETTE_PROPS['toolTipBase'], COLORS['black'])
+    _set_palette_color(palette, PALETTE_PROPS['toolTipText'], COLORS['white'])
+    _set_palette_color(palette, PALETTE_PROPS['text'], COLORS['white'])
+    _set_palette_color(palette, PALETTE_PROPS['button'], _get_color_from_RGB(53, 53, 53))
+    _set_palette_color(palette, PALETTE_PROPS['buttonText'], COLORS['white'])
+    _set_palette_color(palette, PALETTE_PROPS['brightText'], COLORS['red'])
+    _set_palette_color(palette, PALETTE_PROPS['link'], _get_color_from_RGB(42, 130, 218))
+    _set_palette_color(palette, PALETTE_PROPS['highlight'], _get_color_from_RGB(42, 130, 218))
+    _set_palette_color(palette, PALETTE_PROPS['highlightedText'], COLORS['black'])
+    
     app.setPalette(palette)
     app.setStyle("Fusion")
 
-#if __name__ == '__main__':
+
 def main():
     import argparse
 
     parser = argparse.ArgumentParser(description='Process some integers.')
+    parser.add_argument('-v', '--version', dest='version', action='version', version=f'Version: {__version__}')
     parser.add_argument('-1', nargs='?', type=int, dest='screen', const='0')
     parser.add_argument('-2', nargs='?', type=int, dest='screen', const='1')
     parser.add_argument('-3', nargs='?', type=int, dest='screen', const='2')
+    parser.add_argument('-t', '--transparent', dest='transparent', help='Force transparent background. If you are sure your WM support it.', action='store_true')
     args = parser.parse_args()
     
     app = QApplication(sys.argv)
     _setPalette(app)
 
     number_of_screens = len(app.screens())
 
@@ -760,14 +1096,19 @@
             print('No screen chosen, exiting.')
             sys.exit(0)
         else:
             args.screen -= 1
     elif args.screen is None:
         args.screen = 0
         
+    if args.screen >= len(screens):
+        raise Exception(f'Error: You don\'t have so many screens ({args.screen+1}). Try lower number.')
+    
     screen, screen_geom, pixmap = screens[args.screen]
     
-    window = ScreenPenWindow(screen, screen_geom, pixmap)
-    sys.exit(app.exec_())
+    use_transparency = args.transparent or _is_transparency_supported()
+    
+    window = ScreenPenWindow(screen, screen_geom, pixmap, use_transparency)
+    sys.exit(_execute_dialog(app))
 
 if __name__ == '__main__':
     main()
```

### Comparing `screenpen-0.1.9/screenpen/utils/resources.xml` & `screenpen-0.2.0/screenpen/utils/resources.xml`

 * *Files identical despite different names*

### Comparing `screenpen-0.1.9/setup.py` & `screenpen-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,8 +48,20 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.7",
         "Topic :: Communications :: Conferencing",
         "Topic :: Education",
         "Topic :: Multimedia :: Graphics :: Capture :: Screen Capture",
         "Topic :: Multimedia :: Graphics :: Presentation",
     ],
+    command_options={
+        'nuitka': {
+            # boolean option, e.g. if you cared for C commands
+            '--show-scons': ("setup.py", True),
+            # options without value, e.g. enforce using Clang
+            '--clang': ("setup.py", None),
+            # options with single values, e.g. enable a plugin of Nuitka
+            '--enable-plugin': ("setup.py", 'anti-bloat'),
+            # options with several values, e.g. avoiding including modules
+            '--nofollow-import-to' : ("setup.py", ["*.tests", "*.distutils"]),
+        }
+    },
 )
```

