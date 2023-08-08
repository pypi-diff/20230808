# Comparing `tmp/tkintertools-2.6.9.dev0.tar.gz` & `tmp/tkintertools-2.6.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.9.dev0.tar", last modified: Sun Aug  6 09:09:21 2023, max compression
+gzip compressed data, was "tkintertools-2.6.9.dev1.tar", last modified: Tue Aug  8 12:13:25 2023, max compression
```

## Comparing `tkintertools-2.6.9.dev0.tar` & `tkintertools-2.6.9.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 09:09:21.951249 tkintertools-2.6.9.dev0/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.9.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0     7658 2023-08-06 09:09:21.950250 tkintertools-2.6.9.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     7024 2023-08-06 09:04:42.000000 tkintertools-2.6.9.dev0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 09:09:21.951249 tkintertools-2.6.9.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-08-06 08:46:47.000000 tkintertools-2.6.9.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:09:21.920421 tkintertools-2.6.9.dev0/tkintertools/
--rw-rw-rw-   0        0        0     2285 2023-08-06 08:46:12.000000 tkintertools-2.6.9.dev0/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    72017 2023-08-06 09:08:04.000000 tkintertools-2.6.9.dev0/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2937 2023-08-06 08:44:14.000000 tkintertools-2.6.9.dev0/tkintertools/constants.py
--rw-rw-rw-   0        0        0    24186 2023-08-04 04:36:12.000000 tkintertools-2.6.9.dev0/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:09:21.947270 tkintertools-2.6.9.dev0/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     7658 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-06 09:09:21.000000 tkintertools-2.6.9.dev0/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 12:13:25.989439 tkintertools-2.6.9.dev1/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.9.dev1/LICENSE.txt
+-rw-rw-rw-   0        0        0     8374 2023-08-08 12:13:25.988438 tkintertools-2.6.9.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     7740 2023-08-08 12:03:46.000000 tkintertools-2.6.9.dev1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 12:13:25.990482 tkintertools-2.6.9.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-08-08 11:58:13.000000 tkintertools-2.6.9.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:13:25.961832 tkintertools-2.6.9.dev1/tkintertools/
+-rw-rw-rw-   0        0        0     2304 2023-08-08 11:57:30.000000 tkintertools-2.6.9.dev1/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    75263 2023-08-08 12:11:32.000000 tkintertools-2.6.9.dev1/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     3373 2023-08-08 11:38:35.000000 tkintertools-2.6.9.dev1/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    24186 2023-08-04 04:36:12.000000 tkintertools-2.6.9.dev1/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:13:25.986970 tkintertools-2.6.9.dev1/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     8374 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.9.dev0/LICENSE.txt` & `tkintertools-2.6.9.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.9.dev0/PKG-INFO` & `tkintertools-2.6.9.dev1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: tkintertools
-Version: 2.6.9.dev0
-Summary: An auxiliary module of the tkinter module.
-Home-page: https://github.com/Xiaokang2022/tkintertools
-Author: Xiaokang2022
-Author-email: 2951256653@qq.com
-Maintainer: Xiaokang2022
-Maintainer-email: 2951256653@qq.com
-License: MulanPSL-2.0
-Keywords: tkinter,tkintertools,GUI
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <div align="center">
 
 # 🚀tkintertools🚀
 
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/06-orange)](CHANGELOG.md)
-[![ToDo](https://img.shields.io/badge/ToDo-15-yellow)](TODO.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/08-orange)](CHANGELOG.md)
+[![ToDo](https://img.shields.io/badge/ToDo-14-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
@@ -54,23 +36,23 @@
 
 ```
 pip install tkintertools==2.6.8
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.9.dev0` (第 1 个预发布版本)
-* Release/发布日期 : 2023/08/06 (UTC+08)
+* Version/最新版本 : `2.6.9.dev1` (第 2 个预发布版本)
+* Release/发布日期 : 2023/08/08 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.9.dev0
+pip install tkintertools==2.6.9.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -91,45 +73,52 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.9.dev0`**
+**最新版本: `tkintertools-v2.6.9.dev1`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev0`）的更新内容条目：
+下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev1`）的更新内容条目：
 
+- [X] Added new widget switch (`Switch`)  
+新增控件开关（`Switch`）
 - [X] Added widget Tip (`ToolTip`) and all virtual widgets added the parameter `tooltip`  
 新增控件提示框（`ToolTip`），且所有虚拟控件新增参数 `tooltip`
-- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` and `TOOLTIP_HIGNLIGHT_BACKGROUND`  
-新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` 和 `TOOLTIP_HIGNLIGHT_BACKGROUND`
+- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS`、`TOOLTIP_HIGNLIGHT_BACKGROUND`、`COLOR_SWITCH_ON`、`COLOR_SWITCH_OFF`、`SWITCH_WIDTH`、`SWITCH_HEIGHT`、`SWITCH_RADIUS` and `SWITCH_ANIMATION_MS`  
+新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS`、`TOOLTIP_HIGNLIGHT_BACKGROUND`、`COLOR_SWITCH_ON`、`COLOR_SWITCH_OFF`、`SWITCH_WIDTH`、`SWITCH_HEIGHT`、`SWITCH_RADIUS` 和 `SWITCH_ANIMATION_MS`
 - [X] Fixed an issue where the text class widget called method `clear` was invalid  
 修复了文本类控件调用方法 `clear` 无效的问题
+- [X] Fixed an issue where the class `Animation` automatically determined the parent widget of the widget to be moved  
+修复了类 `Animation` 自动确定待移动控件的父控件时出现错误的问题
+- [X] The positional parameter `length` of class `CheckButton` was renamed `height`  
+类 `CheckButton` 的位置参数 `length` 更名为 `height`
 - [X] Optimized the method `wm_geometry` of class `Tk` to accommodate some specially formatted parameters  
 优化了类 `Tk` 的方法 `wm_geometry` 以适应某些特殊格式的参数
 
 ### Template Demo/模板演示
 
-下面是一个主要新功能的示例程序，当按照示例代码方式给虚拟控件传入一个名为 `tooltip` 的参数之后，便可以让这个控件拥有提示框
+下面是一个主要新功能的示例程序，即新增控件：开关！这个控件可以调整长宽、颜色、以及圆角的大小！
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
 ![news](news.png)
 
 <details><summary><b>CODE/源代码</b></summary>
 
 ```python
 # 此处只展示核心代码
 
-tip = tkt.ToolTip('模块介绍\nToolTip 测试')
-tkt.Button(canvas, 10, 660, 200, 50, text='Doc', tooltip=tip)
+tkt.Switch(canvas, 540, 420)  # 默认样式
+tkt.Switch(canvas, 610, 420, radius=4, default=True)  # 圆角半径 4 像素，默认开
+tkt.Switch(canvas, 680, 420, radius=0)  # 无圆角
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.9.dev0/README.md` & `tkintertools-2.6.9.dev1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: tkintertools
+Version: 2.6.9.dev1
+Summary: An auxiliary module of the tkinter module.
+Home-page: https://github.com/Xiaokang2022/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+Maintainer: Xiaokang2022
+Maintainer-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Keywords: tkinter,tkintertools,GUI
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <div align="center">
 
 # 🚀tkintertools🚀
 
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/06-orange)](CHANGELOG.md)
-[![ToDo](https://img.shields.io/badge/ToDo-15-yellow)](TODO.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/08-orange)](CHANGELOG.md)
+[![ToDo](https://img.shields.io/badge/ToDo-14-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
@@ -36,23 +54,23 @@
 
 ```
 pip install tkintertools==2.6.8
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.9.dev0` (第 1 个预发布版本)
-* Release/发布日期 : 2023/08/06 (UTC+08)
+* Version/最新版本 : `2.6.9.dev1` (第 2 个预发布版本)
+* Release/发布日期 : 2023/08/08 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.9.dev0
+pip install tkintertools==2.6.9.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -73,45 +91,52 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.9.dev0`**
+**最新版本: `tkintertools-v2.6.9.dev1`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev0`）的更新内容条目：
+下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev1`）的更新内容条目：
 
+- [X] Added new widget switch (`Switch`)  
+新增控件开关（`Switch`）
 - [X] Added widget Tip (`ToolTip`) and all virtual widgets added the parameter `tooltip`  
 新增控件提示框（`ToolTip`），且所有虚拟控件新增参数 `tooltip`
-- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` and `TOOLTIP_HIGNLIGHT_BACKGROUND`  
-新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` 和 `TOOLTIP_HIGNLIGHT_BACKGROUND`
+- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS`、`TOOLTIP_HIGNLIGHT_BACKGROUND`、`COLOR_SWITCH_ON`、`COLOR_SWITCH_OFF`、`SWITCH_WIDTH`、`SWITCH_HEIGHT`、`SWITCH_RADIUS` and `SWITCH_ANIMATION_MS`  
+新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS`、`TOOLTIP_HIGNLIGHT_BACKGROUND`、`COLOR_SWITCH_ON`、`COLOR_SWITCH_OFF`、`SWITCH_WIDTH`、`SWITCH_HEIGHT`、`SWITCH_RADIUS` 和 `SWITCH_ANIMATION_MS`
 - [X] Fixed an issue where the text class widget called method `clear` was invalid  
 修复了文本类控件调用方法 `clear` 无效的问题
+- [X] Fixed an issue where the class `Animation` automatically determined the parent widget of the widget to be moved  
+修复了类 `Animation` 自动确定待移动控件的父控件时出现错误的问题
+- [X] The positional parameter `length` of class `CheckButton` was renamed `height`  
+类 `CheckButton` 的位置参数 `length` 更名为 `height`
 - [X] Optimized the method `wm_geometry` of class `Tk` to accommodate some specially formatted parameters  
 优化了类 `Tk` 的方法 `wm_geometry` 以适应某些特殊格式的参数
 
 ### Template Demo/模板演示
 
-下面是一个主要新功能的示例程序，当按照示例代码方式给虚拟控件传入一个名为 `tooltip` 的参数之后，便可以让这个控件拥有提示框
+下面是一个主要新功能的示例程序，即新增控件：开关！这个控件可以调整长宽、颜色、以及圆角的大小！
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
 ![news](news.png)
 
 <details><summary><b>CODE/源代码</b></summary>
 
 ```python
 # 此处只展示核心代码
 
-tip = tkt.ToolTip('模块介绍\nToolTip 测试')
-tkt.Button(canvas, 10, 660, 200, 50, text='Doc', tooltip=tip)
+tkt.Switch(canvas, 540, 420)  # 默认样式
+tkt.Switch(canvas, 610, 420, radius=4, default=True)  # 圆角半径 4 像素，默认开
+tkt.Switch(canvas, 680, 420, radius=0)  # 无圆角
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.9.dev0/setup.py` & `tkintertools-2.6.9.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 9. 删除多余文件
 """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.9.dev0',
+    version='2.6.9.dev1',
     description='An auxiliary module of the tkinter module.',
     long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
     author_email='2951256653@qq.com',
     maintainer='Xiaokang2022',
     maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
```

### Comparing `tkintertools-2.6.9.dev0/tkintertools/__init__.py` & `tkintertools-2.6.9.dev1/tkintertools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 * Text with controllable length and alignment
 * Convenient, inheritable singleton pattern class
 * 3D drawing
 
 Contents
 --------
 * Container Widgets: `Tk`, `Toplevel`, `Canvas`
-* Virtual Canvas Widgets: `Label`, `Button`, `CheckButton`, `Entry`, `Text`, `Progressbar`
-* Tool Classes: `PhotoImage`, `ToolTip`, `Singleton`, `Animation`
+* Virtual Canvas Widgets: `Label`, `Button`, `CheckButton`, `Entry`, `Text`, `Progressbar`,`ToolTip`, `Switch`
 * Tool Functions: `move`, `text`, `color`, `askfont`, `SetProcessDpiAwareness`
+* Tool Classes: `PhotoImage`, `Singleton`, `Animation`
 * Tool Submodules: `tool_3d`
 
 More
 ----
 [GitHub](https://github.com/Xiaokang2022/tkintertools) ·
 [License](https://github.com/Xiaokang2022/tkintertools/blob/master/LICENSE.txt) ·
 [ChangeLog](https://github.com/Xiaokang2022/tkintertools/blob/master/CHANGELOG.md) ·
@@ -44,18 +44,18 @@
 if sys.version_info < (3, 8):  # Version Check
     raise RuntimeError('Python version is too low (>=3.8)')
 
 from .__main__ import *
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.9.dev0'
+__version__ = '2.6.9.dev1'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
-    'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
+    'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar', 'ToolTip', 'Switch',
     # Tool Classes
-    'PhotoImage', 'ToolTip', 'Singleton', 'Animation',
+    'PhotoImage', 'Singleton', 'Animation',
     # Tool Functions
     'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness',
 ] + all_constants
```

### Comparing `tkintertools-2.6.9.dev0/tkintertools/__main__.py` & `tkintertools-2.6.9.dev1/tkintertools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,23 @@
         """
         tkinter.Toplevel.__init__(self, master, **kw)
         Tk.__init__(self, title, width, height, x, y, shutdown=shutdown, alpha=alpha,
                     toolwindow=toolwindow, topmost=topmost, transparentcolor=transparentcolor, **kw)
         self.focus_set()  # 把焦点转移到该子窗口上来
 
 
+class CombinedItem(list):
+    """ 画布元素组合体 """
+
+    def __init__(self, *args):  # type: (int) -> None
+        if not all(map(lambda _: isinstance(_, int), args)):
+            raise TypeError('Not all elements are of type _CanvasItemId')
+        list.__init__(self, args)
+
+
 class Canvas(tkinter.Canvas):
     """ 画布容器类 """
 
     def __init__(
         self,
         master,  # type: Tk | Toplevel
         width,  # type: int
@@ -983,36 +992,36 @@
     """ 虚拟复选框控件 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
-        length,  # type: int
+        height,  # type: int
         *,
         radius=RADIUS,  # type: float
         text='',  # type: str
         value=False,  # type: bool
         borderwidth=BORDERWIDTH,  # type: int
         justify='right',  # type: Literal['right', 'left']
         image=None,  # type: PhotoImage | None
         tooltip=None,  # type: ToolTip | None
         color_text=COLOR_TEXT,  # type: tuple[str, str, str]
         color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
         color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
     ):  # type: (...) -> None
         Button.__init__(
-            self, canvas, x, y, length, length, radius=radius, borderwidth=borderwidth, image=image,
+            self, canvas, x, y, height, height, radius=radius, borderwidth=borderwidth, image=image,
             tooltip=tooltip, color_text=color_text, color_fill=color_fill, color_outline=color_outline)
         if justify == 'right':
             self._text = canvas.create_text(
-                x+1.25*length, y+length/2, text=text, anchor='w')
+                x+1.25*height, y+height/2, text=text, anchor='w')
         else:
             self._text = canvas.create_text(
-                x-0.25*length, y+length/2, text=text, anchor='e')
+                x-0.25*height, y+height/2, text=text, anchor='e')
         self.command = lambda: self.set(not bool(self.value))
         if value:
             self.command()
 
     def get(self):  # type: () -> bool
         """ 获取复选框状态 """
         return bool(self.value)
@@ -1307,14 +1316,93 @@
         """
         percentage = 0 if percentage < 0 else 1 if percentage > 1 else percentage
         x2 = self.x1 + self.width * percentage * self.master.rx
         self.master.coords(self.bar, self.x1, self.y1, x2, self.y2)
         self.configure(text='%.2f%%' % (percentage * 100))
 
 
+class Switch:
+    """ 开关 """
+
+    def __init__(
+        self,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width=SWITCH_WIDTH,  # type: int
+        height=SWITCH_HEIGHT,  # type: int
+        *,
+        radius=SWITCH_RADIUS,  # type: float
+        borderwidth=BORDERWIDTH,  # type: int
+        tooltip=None,  # type: ToolTip | None
+        color_fill=COLOR_SWITCH_OFF,  # type: tuple[str, str, str]
+        color_outline=COLOR_BUTTON_OUTLINE,  # type: tuple[str, str, str]
+        default=False,  # type: bool
+        on=None,  # type: Callable | None
+        off=None,  # type: Callable | None
+    ):  # type: (...) -> None
+        """
+        `canvas`: 父画布控件 \ 
+        `x`: 横坐标 \ 
+        `y`: 纵坐标 \ 
+        `width`: 宽度 \ 
+        `height`: 高度 \ 
+        `radius`: 圆角半径 \ 
+        `borderwidth`: 边框宽度 \ 
+        `tooltip`: 提示框 \ 
+        `color_fill`: 内部颜色 \ 
+        `color_outline`: 边框颜色 \ 
+        `default`: 默认值 \ 
+        `on`: 转换到开时触发的回调函数 \ 
+        `off`: 转换到关时触发的回调函数 
+        """
+        self.value = default
+        self.width = height * 2 if width < height * 2 else width
+        self.height = height
+        self.on = on
+        self.off = off
+        self.outside = Button(
+            canvas, x, y, self.width, height, radius=radius, borderwidth=borderwidth,
+            tooltip=tooltip, color_fill=color_fill, color_outline=color_outline,
+            command=lambda self=self: self.set(not self.value))
+        spcaing = height * 2 / 15
+        self.inside = Label(
+            canvas, x+spcaing, y+spcaing, height-spcaing*2, height-spcaing*2, radius=radius,
+            borderwidth=borderwidth, color_outline=('#333',)*3, color_fill=('black',)*3)
+        if self.value is True:
+            self._animate(0)
+
+    def _animate(self, ms=SWITCH_ANIMATION_MS):  # type: (int) -> None
+        """ 移动动画 """
+        if self.value:
+            key = 1
+            self.outside.configure(
+                color_fill=COLOR_SWITCH_ON, color_outline=COLOR_SWITCH_ON)
+        else:
+            key = -1
+            self.outside.configure(
+                color_fill=COLOR_SWITCH_OFF, color_outline=COLOR_BUTTON_OUTLINE)
+        self.outside.state()
+        Animation(self.inside, ms, fps=90, control=(math.sin, 0, math.pi),
+                  translation=(key*(self.width-self.height)*self.inside.master.rx, 0)).run()
+
+    def get(self):  # type: () -> bool
+        """ 返回状态 """
+        return self.value
+
+    def set(self, value):  # type: (bool) -> None
+        """ 设定状态 """
+        self.value = value
+        if self.value and self.on is not None:
+            self.on()
+        if not self.value and self.off is not None:
+            self.off()
+        self._animate()
+
+
 class ToolTip:
     """ 提示框 """
 
     def __init__(
         self,
         text,  # type: str
         *,
@@ -1524,16 +1612,16 @@
         `step`: 动画每一帧结束后执行的函数（包括开始和结束）\ 
         `stop`: 动画结束后执行的函数 \ 
         `callback`: 回调函数，每一帧调用一次，传入参数为单帧占比 \ 
         `canvas`: 当 widget 是画布中的绘制对象时，应指定 canvas \ 
         `loop`: 是否循环播放动画，默认不循环，循环时参数 stop 失效
         """
         self.widget = widget
-        self.master = canvas if isinstance(widget, int) else widget.master if isinstance(
-            widget, tkinter.Widget) else widget
+        self.master = canvas if isinstance(widget, int) else widget if isinstance(
+            widget, tkinter.Widget) else widget.master
         self.start = start
         self.step = step
         self.stop = stop
         self.loop = loop
         self.translation = translation
         self.color = color
         self.sec = 1000 // fps  # 单帧间隔时间
```

### Comparing `tkintertools-2.6.9.dev0/tkintertools/constants.py` & `tkintertools-2.6.9.dev1/tkintertools/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
 COLOR_NONE = '', '', '', ''
 """ Default transparent color tuple """
 
 COLOR_BAR = '#E1E1E1', '#06b025'
 """ Default progress bar color """
 
+COLOR_SWITCH_ON = '#288CDB', '#3E98DF', '#4884B4', '#E0E0E0'
+""" Default color when `Switch` is on """
+
+COLOR_SWITCH_OFF = COLOR_BUTTON_FILL
+""" Default color when `Switch` is off """
+
 
 ### Other constants ###
 
 
 BORDERWIDTH = 1
 """ Default widget borderwidth """
 
@@ -79,14 +85,26 @@
 
 TOOLTIP_HIGNLIGHT_THICKNESS = 1
 """ Default ToolTip highlightthickness """
 
 TOOLTIP_HIGNLIGHT_BACKGROUND = 'black'
 """ Default ToolTip highlightbackground """
 
+SWITCH_WIDTH = 0
+""" Default Switch width """
+
+SWITCH_HEIGHT = 30
+""" Default Switch height """
+
+SWITCH_RADIUS = float('inf')
+""" Default Switch radius """
+
+SWITCH_ANIMATION_MS = 250
+""" Default animation duration of the Switch """
+
 
 ### 3D constants ###
 
 
 COLOR_POINT_FILL = '#000000'
 """ Default point fill color """
```

### Comparing `tkintertools-2.6.9.dev0/tkintertools/tools_3d.py` & `tkintertools-2.6.9.dev1/tkintertools/tools_3d.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.9.dev0/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.9.dev1/tkintertools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.9.dev0
+Version: 2.6.9.dev1
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,16 +23,16 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/06-orange)](CHANGELOG.md)
-[![ToDo](https://img.shields.io/badge/ToDo-15-yellow)](TODO.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/08/08-orange)](CHANGELOG.md)
+[![ToDo](https://img.shields.io/badge/ToDo-14-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
@@ -54,23 +54,23 @@
 
 ```
 pip install tkintertools==2.6.8
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.9.dev0` (第 1 个预发布版本)
-* Release/发布日期 : 2023/08/06 (UTC+08)
+* Version/最新版本 : `2.6.9.dev1` (第 2 个预发布版本)
+* Release/发布日期 : 2023/08/08 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.9.dev0
+pip install tkintertools==2.6.9.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -91,45 +91,52 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.9.dev0`**
+**最新版本: `tkintertools-v2.6.9.dev1`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev0`）的更新内容条目：
+下面是本次开发版本（`v2.6.8` -> `v2.6.9.dev1`）的更新内容条目：
 
+- [X] Added new widget switch (`Switch`)  
+新增控件开关（`Switch`）
 - [X] Added widget Tip (`ToolTip`) and all virtual widgets added the parameter `tooltip`  
 新增控件提示框（`ToolTip`），且所有虚拟控件新增参数 `tooltip`
-- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` and `TOOLTIP_HIGNLIGHT_BACKGROUND`  
-新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS` 和 `TOOLTIP_HIGNLIGHT_BACKGROUND`
+- [X] Added constants `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS`、`TOOLTIP_HIGNLIGHT_BACKGROUND`、`COLOR_SWITCH_ON`、`COLOR_SWITCH_OFF`、`SWITCH_WIDTH`、`SWITCH_HEIGHT`、`SWITCH_RADIUS` and `SWITCH_ANIMATION_MS`  
+新增常量 `DURATION`、`TOOLTIP_FG`、`TOOLTIP_BG`、`TOOLTIP_HIGNLIGHT_THICKNESS`、`TOOLTIP_HIGNLIGHT_BACKGROUND`、`COLOR_SWITCH_ON`、`COLOR_SWITCH_OFF`、`SWITCH_WIDTH`、`SWITCH_HEIGHT`、`SWITCH_RADIUS` 和 `SWITCH_ANIMATION_MS`
 - [X] Fixed an issue where the text class widget called method `clear` was invalid  
 修复了文本类控件调用方法 `clear` 无效的问题
+- [X] Fixed an issue where the class `Animation` automatically determined the parent widget of the widget to be moved  
+修复了类 `Animation` 自动确定待移动控件的父控件时出现错误的问题
+- [X] The positional parameter `length` of class `CheckButton` was renamed `height`  
+类 `CheckButton` 的位置参数 `length` 更名为 `height`
 - [X] Optimized the method `wm_geometry` of class `Tk` to accommodate some specially formatted parameters  
 优化了类 `Tk` 的方法 `wm_geometry` 以适应某些特殊格式的参数
 
 ### Template Demo/模板演示
 
-下面是一个主要新功能的示例程序，当按照示例代码方式给虚拟控件传入一个名为 `tooltip` 的参数之后，便可以让这个控件拥有提示框
+下面是一个主要新功能的示例程序，即新增控件：开关！这个控件可以调整长宽、颜色、以及圆角的大小！
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
 ![news](news.png)
 
 <details><summary><b>CODE/源代码</b></summary>
 
 ```python
 # 此处只展示核心代码
 
-tip = tkt.ToolTip('模块介绍\nToolTip 测试')
-tkt.Button(canvas, 10, 660, 200, 50, text='Doc', tooltip=tip)
+tkt.Switch(canvas, 540, 420)  # 默认样式
+tkt.Switch(canvas, 610, 420, radius=4, default=True)  # 圆角半径 4 像素，默认开
+tkt.Switch(canvas, 680, 420, radius=0)  # 无圆角
 ```
 
 </details>
 
 More/更多👇
 -----------
```

