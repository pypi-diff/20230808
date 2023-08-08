# Comparing `tmp/srsgui-0.4.2.tar.gz` & `tmp/srsgui-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-avc40r37\srsgui-0.4.2.tar", last modified: Fri Jul 14 20:48:18 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-wr6qzki4\srsgui-0.4.3.tar", last modified: Tue Aug  8 21:41:58 2023, max compression
```

## Comparing `srsgui-0.4.2.tar` & `srsgui-0.4.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.791865 srsgui-0.4.2/
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.705507 srsgui-0.4.2/.github/
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.715501 srsgui-0.4.2/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-07-14 19:39:01.000000 srsgui-0.4.2/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-07-14 19:39:01.000000 srsgui-0.4.2/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-07-14 19:39:01.000000 srsgui-0.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4626 2023-07-14 20:48:18.791865 srsgui-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3595 2023-07-14 19:39:01.000000 srsgui-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.725496 srsgui-0.4.2/docs/
--rw-rw-rw-   0        0        0      654 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    88057 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/dock_widget_floating.png
--rw-rw-rw-   0        0        0    97266 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/dock_widgets_expanded.png
--rw-rw-rw-   0        0        0    71070 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    52123 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/lockin-capture.png
--rw-rw-rw-   0        0        0    29667 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    38581 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/task_selection.png
--rw-rw-rw-   0        0        0    39412 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     8703 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/application.rst
--rw-rw-rw-   0        0        0      840 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/changelog.rst
--rw-rw-rw-   0        0        0     1921 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/conf.py
--rw-rw-rw-   0        0        0     6270 2023-07-14 20:36:38.000000 srsgui-0.4.2/docs/create-project.rst
--rw-rw-rw-   0        0        0     7546 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/create-task.rst
--rw-rw-rw-   0        0        0     6547 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    16790 2023-07-14 20:42:29.000000 srsgui-0.4.2/docs/example.rst
--rw-rw-rw-   0        0        0     3837 2023-07-14 20:26:07.000000 srsgui-0.4.2/docs/index.rst
--rw-rw-rw-   0        0        0     4539 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      930 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1101 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1539 2023-07-14 19:39:01.000000 srsgui-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-07-14 19:39:01.000000 srsgui-0.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 20:48:18.791865 srsgui-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-07-14 19:39:01.000000 srsgui-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.705507 srsgui-0.4.2/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1829 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3147 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1998 2023-07-14 19:58:54.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.755479 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     4101 2023-07-14 20:06:32.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/captured_fft.py
--rw-rw-rw-   0        0        0     1662 2023-07-14 20:06:33.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/identify.py
--rw-rw-rw-   0        0        0     2585 2023-07-14 20:06:33.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/plot_example.py
--rw-rw-rw-   0        0        0     1946 2023-07-14 20:46:40.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/scope_capture.py
--rw-rw-rw-   0        0        0     2549 2023-07-14 20:31:28.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/simulated_fft.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.755479 srsgui-0.4.2/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9908 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.765474 srsgui-0.4.2/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8309 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1277 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8775 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11334 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    19292 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      845 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10411 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9991 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.765474 srsgui-0.4.2/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6990 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5858 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6939 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    25860 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4226 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.785463 srsgui-0.4.2/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3895 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6881 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.791865 srsgui-0.4.2/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1604 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12606 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8670 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5110 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3453 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4853 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9797 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3976 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15881 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    14951 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.791865 srsgui-0.4.2/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      800 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      678 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      778 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1286 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2718 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1006 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    26551 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui.egg-info/
--rw-rw-rw-   0        0        0     4626 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3201 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.723148 srsgui-0.4.3/
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.590935 srsgui-0.4.3/.github/
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.600903 srsgui-0.4.3/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-07-14 19:39:01.000000 srsgui-0.4.3/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-07-14 19:39:01.000000 srsgui-0.4.3/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-07-14 19:39:01.000000 srsgui-0.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4626 2023-08-08 21:41:58.723148 srsgui-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3595 2023-07-14 20:50:24.000000 srsgui-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.628717 srsgui-0.4.3/docs/
+-rw-rw-rw-   0        0        0      654 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8703 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/application.rst
+-rw-rw-rw-   0        0        0      840 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1921 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/conf.py
+-rw-rw-rw-   0        0        0     6270 2023-07-14 20:50:24.000000 srsgui-0.4.3/docs/create-project.rst
+-rw-rw-rw-   0        0        0     7546 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6547 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    16790 2023-07-14 20:50:24.000000 srsgui-0.4.3/docs/example.rst
+-rw-rw-rw-   0        0        0     3837 2023-07-14 20:50:24.000000 srsgui-0.4.3/docs/index.rst
+-rw-rw-rw-   0        0        0     4539 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1101 2023-07-14 19:39:01.000000 srsgui-0.4.3/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1539 2023-07-14 20:50:24.000000 srsgui-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-07-14 19:39:01.000000 srsgui-0.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 21:41:58.733143 srsgui-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-07-14 19:39:01.000000 srsgui-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/srsgui/
+-rw-rw-rw-   0        0        0     1552 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.590935 srsgui-0.4.3/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.658701 srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1829 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3147 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1998 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.658701 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     4101 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/captured_fft.py
+-rw-rw-rw-   0        0        0     1662 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/identify.py
+-rw-rw-rw-   0        0        0     2585 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/plot_example.py
+-rw-rw-rw-   0        0        0     1946 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/scope_capture.py
+-rw-rw-rw-   0        0        0     2549 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/simulated_fft.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.670172 srsgui-0.4.3/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9908 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.680169 srsgui-0.4.3/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8309 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1277 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8775 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11334 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    19292 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      845 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10411 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9992 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.690163 srsgui-0.4.3/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0     1313 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6990 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5858 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6939 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    25314 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4226 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.713154 srsgui-0.4.3/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3895 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6881 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.723148 srsgui-0.4.3/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1604 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12606 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8670 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5697 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3453 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4853 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9797 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3976 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15881 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    15296 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.723148 srsgui-0.4.3/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      800 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      678 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      778 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1372 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2769 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1006 2023-07-14 20:50:24.000000 srsgui-0.4.3/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    26324 2023-08-08 21:25:52.000000 srsgui-0.4.3/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-07-14 19:39:01.000000 srsgui-0.4.3/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:41:58.648707 srsgui-0.4.3/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     4626 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3201 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 21:41:58.000000 srsgui-0.4.3/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.4.2/.gitignore` & `srsgui-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/LICENSE.txt` & `srsgui-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/PKG-INFO` & `srsgui-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.2
+Version: 0.4.3
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
```

### Comparing `srsgui-0.4.2/README.md` & `srsgui-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/Makefile` & `srsgui-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.4.3/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.4.3/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.4.3/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/dock_widget_floating.png` & `srsgui-0.4.3/docs/_static/dock_widget_floating.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/dock_widgets_expanded.png` & `srsgui-0.4.3/docs/_static/dock_widgets_expanded.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/example-screen-capture-1.png` & `srsgui-0.4.3/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/example-screen-capture-2.png` & `srsgui-0.4.3/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/initial-screen-capture.png` & `srsgui-0.4.3/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/lockin-capture.png` & `srsgui-0.4.3/docs/_static/lockin-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.4.3/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/second-task-screen-capture.png` & `srsgui-0.4.3/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/task_selection.png` & `srsgui-0.4.3/docs/_static/task_selection.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/terminal-with-example-2.png` & `srsgui-0.4.3/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/_static/terminal-with-example.png` & `srsgui-0.4.3/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/application.rst` & `srsgui-0.4.3/docs/application.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/changelog.rst` & `srsgui-0.4.3/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/conf.py` & `srsgui-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/create-project.rst` & `srsgui-0.4.3/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/create-task.rst` & `srsgui-0.4.3/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/define-instrument.rst` & `srsgui-0.4.3/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/example.rst` & `srsgui-0.4.3/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/index.rst` & `srsgui-0.4.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/installation.rst` & `srsgui-0.4.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/make.bat` & `srsgui-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/srsgui.inst.communications.rst` & `srsgui-0.4.3/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/srsgui.inst.rst` & `srsgui-0.4.3/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/srsgui.task.rst` & `srsgui-0.4.3/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/srsgui.ui.commandtree.rst` & `srsgui-0.4.3/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/srsgui.ui.qt.rst` & `srsgui-0.4.3/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/srsgui.ui.rst` & `srsgui-0.4.3/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/docs/troubleshooting.rst` & `srsgui-0.4.3/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/pyproject.toml` & `srsgui-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/__init__.py` & `srsgui-0.4.3/srsgui/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,12 +18,12 @@
                                       FloatIndexCommand, FloatIndexGetCommand, \
                                       DictIndexCommand
 
 from srsgui.inst.exceptions import InstException, InstCommunicationError, \
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
-from srsgui.inst import Interface, SerialInterface, TcpipInterface
+from srsgui.inst.communications import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.4.2"  # Global version number
+__version__ = "0.4.3"  # Global version number
```

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/captured_fft.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/captured_fft.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/identify.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/identify.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/plot_example.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/plot_example.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/scope_capture.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/scope_capture.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/simulated_fft.py` & `srsgui-0.4.3/srsgui/examples/oscilloscope example/tasks/simulated_fft.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/__init__.py` & `srsgui-0.4.3/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/commands.py` & `srsgui-0.4.3/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/communications/interface.py` & `srsgui-0.4.3/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/communications/serial_ports.py` & `srsgui-0.4.3/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/communications/serialinterface.py` & `srsgui-0.4.3/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.4.3/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/component.py` & `srsgui-0.4.3/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/exceptions.py` & `srsgui-0.4.3/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/indexcommands.py` & `srsgui-0.4.3/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/inst/instrument.py` & `srsgui-0.4.3/srsgui/inst/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         return d
 
     def get_info(self):
         """
         Get the instrument information
 
         default return value is a dictionalry containing model name, serial number,
-        firmware version. A subclass can add more informaton into the dictionary
+        firmware version. A subclass can add more information into the dictionary
         as needed.
 
         :rtype: dict
         """
         d = self.comm.get_info()
         if type(d) is dict:
             d['model_name'] = self._model_name
```

### Comparing `srsgui-0.4.2/srsgui/task/callbacks.py` & `srsgui-0.4.3/srsgui/task/callbacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 ##! 
 ##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
-from matplotlib.figure import Figure
+
+
+class DummyFigure:
+    pass
+
+
+try:
+    from matplotlib.figure import Figure
+except (ImportError, ModuleNotFoundError):
+    Figure = DummyFigure
+
 
 logger = logging.getLogger(__file__)
 
 
 class Callbacks:
     """
     Base callbacks used by :class:`Task <srsgui.task.task.Task>` class.
```

### Comparing `srsgui-0.4.2/srsgui/task/config.py` & `srsgui-0.4.3/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/task/inputs.py` & `srsgui-0.4.3/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/task/sessionhandler.py` & `srsgui-0.4.3/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/task/task.py` & `srsgui-0.4.3/srsgui/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,26 @@
 ##! 
 
 import sys
 import traceback
 import logging
 import time
 
-try:
-    from matplotlib.figure import Figure
-except (ImportError, ModuleNotFoundError):
-    msg = "\n\nPython package 'Matplotlib' is required to use Task class." \
-          "\nTry again after installing 'Matplotlib' with" \
-          "\n\npip install matplotlib" \
-          "\n\nOr your system may have a different way to install it."
-    raise ModuleNotFoundError(msg)
-
 from .inputs import FloatInput, StringInput
 from .taskresult import TaskResult, ResultLogHandler
-from .callbacks import Callbacks
+from .callbacks import Callbacks, DummyFigure
 
 from srsgui.inst.instrument import Instrument
 
 try:
+    from matplotlib.figure import Figure
+except (ImportError, ModuleNotFoundError):
+    Figure = DummyFigure
+
+try:
     from srsgui.ui.qt.QtCore import QThread
     thread_class = QThread
 except (ImportError, ModuleNotFoundError):
     from threading import Thread
     thread_class = Thread
 
 # HTML formatter for QTextBrowser
@@ -56,16 +52,14 @@
     class TaskSetupFailed(TaskException): pass
     class TaskRunFailed(TaskException): pass
 
     # Escape strings used in stdout redirection to GUI
     EscapeForResult = '@RESULT@'
     EscapeForDevice = '@DEVICE@'
     EscapeForStatus = '@STATUS@'
-    EscapeForStart = '@START@'
-    EscapeForStop = '@STOP@'
 
     input_parameters = {
         # Example float parameter
             "Define parameters": FloatInput(10.0, " Hz", 1.0, 1000.0, 1.0),
             "before use!! ":     StringInput(" or empty input_parameters.")
     }
     """
@@ -101,15 +95,15 @@
         self.name = 'Base Task'
         self.logger_prefix = ''  # used for logger name for multi-threaded tasks
         self.logger = None
 
         self.result = None
         self.result_log_handler = None
         self.session_handler = None
-        self.callbacks = None
+        self.callbacks = Callbacks()
 
         # inst_dict holds all the instrument to use in task
         self.inst_dict = {}
         self.data_dict = {}
 
         # figure is expected to be Matplotlib figure object.
         self.figure_dict = {}
@@ -157,22 +151,20 @@
 
     def basic_setup(self):
         """
         basic_setup() runs before task-specific setup()
         """
 
         self.logger = self.get_logger(__name__)
-        if self.figure is None or not hasattr(self.figure, 'canvas'):
+        if self.figure is not None and not hasattr(self.figure, 'canvas'):
             raise AttributeError('Invalid figure')
 
         if not self._check_dict_items(self.inst_dict, Instrument):
             raise AttributeError('Invalid inst_dict detected during basic setup')
 
-        self.callbacks.started()
-
         # We want Exception to be handled in run()
         Task._is_running = True
         self._keep_running = True
         self._error_raised = False
 
         self.result = TaskResult(self.__class__.__name__)
         self.result.set_start_time_now()
@@ -186,26 +178,25 @@
         self.logger.addHandler(self.result_log_handler)
 
         msg = '{} STARTED'.format(self.name)
         self.display_result(msg)
         self.update_status(msg)
         self.logger.info(GreenBold.format(msg))
 
-        self._notify_start()
         self.clear_figures()
 
     def basic_cleanup(self):
         """
         basic_cleanup runs after task-specific cleanup()
         """
 
         try:
             Task._is_running = False
             self._keep_running = False
-            self._notify_finish()
+
             self.result.set_stop_time_now()
             if self._aborted:
                 msg = '{} ABORTED'.format(self.name)
                 self.display_result(msg)
                 self.update_status(msg)
                 msg = '<font color="red"><b>' + msg + '</b></font>'
                 self.logger.info(msg)
@@ -232,14 +223,15 @@
             self.logger.removeHandler(self.result_log_handler)
 
     def run(self):
         """
         Overrides Thread run() method. task-specific test() runs inside this method.
         """
         try:
+            self.callbacks.started()
             self.basic_setup()
             if self._keep_running:
                 self.logger.debug("{} run started".format(self.name))
             try:
                 self.setup()  # setup from the subclass
                 try:
                     self.logger.debug("{} task started".format(self.name))
@@ -296,14 +288,17 @@
         """
         Parent should set a callback handler to handle events from Task.
         """
         self.callbacks = callback_handler
 
     @staticmethod
     def _check_dict_items(item_dict, item_class):
+        """
+        Check if all the items in item_dict are instances of item_class.
+        """
         if type(item_dict) is not dict:
             return False
         for value in item_dict.values():
             if not issubclass(type(value), item_class):
                 return False
         return True
 
@@ -520,22 +515,14 @@
     def display_result(self, message, clear=False):
         """ output to the Result panel
         """
         if clear:
             self.write_text('{}cls'.format(self.EscapeForResult))
         self.write_text('{}{}'.format(self.EscapeForResult, message))
 
-    def _notify_start(self):
-        self.write_text(self.EscapeForStart + self.name)
-        self.update_status(self.name + ' running')
-
-    def _notify_finish(self):
-        self.write_text(self.EscapeForStop + self.name)
-        self.update_status(self.name + ' stopped')
-
     def write_text(self, text):
         """
         Base method to send output text to UI
         """
         self.callbacks.text_available(str(text))
 
     def get_input_parameter(self, name):
```

### Comparing `srsgui-0.4.2/srsgui/task/taskresult.py` & `srsgui-0.4.3/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandhandler.py` & `srsgui-0.4.3/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandterminal.py` & `srsgui-0.4.3/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.minimum_step = 0.1
         self.significant_figures = 4
         self.precision = 3
         self.decis = 3
+        self.setDecimals(10)
 
     def set_minimum_step(self, value):
         self.minimum_step = value
         step = self.minimum_step if self.minimum_step > 1e-12 else 1e-12
         self.decis = math.ceil(-math.log10(step))
 
     def set_significant_figures(self, value):
@@ -76,60 +77,76 @@
 
             else:
                 value = float(text)
             if value < self.minimum():
                 value = self.minimum()
             elif value > self.maximum():
                 value = self.maximum()
-
         except ValueError:
             print('valueFromText ValueError', text, self.suffix())
             value = self.minimum()
         return value
 
     def textFromValue(self, value):
         prec = self.decis
         try:
-            if value == 0:
+            if abs(value) < self.minimum_step:
                 return '0.0'
 
             digits = math.ceil(math.log10(abs(value)))
             """
             if digits == self.significant_figures:
                 step = 1
             else:
                 step = 10 ** (digits - self.significant_figures)
             value = round(value / step) * step
             """
-            prec = self.significant_figures - digits
-            prec = self.decis if prec > self.decis else prec
-            prec = 0 if prec < 0 else prec
-            self.precision = prec
-            format_string = '{:.' + str(prec) + 'f}'
+            if digits > -3:
+                prec = self.significant_figures - digits
+                prec = self.decis if prec > self.decis else prec
+                prec = 0 if prec < 0 else prec
+                self.precision = prec
+                format_string = '{:.' + str(prec) + 'f}'
+            else:
+                format_string = '{:.' + str(self.significant_figures - 1) + 'e}'
+
             text = format_string.format(value)
         except Exception as e:
             print('Error in textFromValue: {}'.format(e))
             return ''
         return text
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
         suffix_len = len(self.suffix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
-        text = self.lineEdit().text()
+        text = self.lineEdit().text().lower()
         cur_pos = self.lineEdit().cursorPosition()
+        max_pos = len(text) - suffix_len
+
+        if cur_pos < min_pos or cur_pos > max_pos:
+            return
+
+        e_pos = text.find('e')
+        if e_pos > 0 and e_pos < cur_pos:  # cursor is on the right side of 'E'
+            return
+
+        exponent = 0
+        if 0 < e_pos < max_pos:
+            try:
+                exponent = int(text[e_pos + 1: max_pos])
+            except:
+                return
+
         sep_pos = text.find('.')
         if sep_pos < 0:
             sep_pos = len(text) - suffix_len
 
-        if cur_pos < min_pos:
-            return
-
-        exponent = sep_pos - cur_pos
+        exponent += sep_pos - cur_pos
         if exponent == -1:
             cur_pos += 1
 
         if exponent < -1:
             exponent += 1
 
         single_step = 10 ** exponent
```

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.4.3/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.4.3/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/connectdlg.py` & `srsgui-0.4.3/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/deviceinfohandler.py` & `srsgui-0.4.3/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/dockhandler.py` & `srsgui-0.4.3/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/inputpanel.py` & `srsgui-0.4.3/srsgui/ui/inputpanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 ##! 
 ##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import math
 from .qt.QtCore import Qt
-from .qt.QtWidgets import QWidget, QDoubleSpinBox, QSpinBox, QComboBox, \
+from .qt.QtWidgets import QWidget, QComboBox, \
                           QLineEdit, QLabel, QGridLayout, QPushButton, QScrollArea
 
 from srsgui.inst.commands import Command, IntCommand, FloatCommand, DictCommand
 from srsgui.inst.indexcommands import IndexCommand, IntIndexCommand, FloatIndexCommand, DictIndexCommand
 
 from srsgui.task.task import Task
 from srsgui.task.inputs import IntegerInput, FloatInput, StringInput, \
                                ListInput, InstrumentInput, CommandInput
 
+from srsgui.ui.commandtree.commandspinbox import IntegerSpinBox, FloatSpinBox
+
 import logging
 logger = logging.getLogger(__name__)
 
 
 class InputPanel(QScrollArea):
     """
     To build the input panel in an instance of :class:`TaskMain <srsgui.ui.taskmain.TaskMain>` class
@@ -95,29 +97,30 @@
                     if not self.inst_dict[self.inst_name].is_connected:
                         raise ValueError('{} is not connected'.format(self.inst_name))
 
                     p.set_inst_name(self.inst_name)
                     p.cmd_instance = self.get_cmd_instance(p)
                     if issubclass(p.cmd_instance.__class__, IntCommand) or \
                        issubclass(p.cmd_instance.__class__, IntIndexCommand):
-                        widget = QSpinBox()
+                        widget = IntegerSpinBox()
                         widget.setSuffix(' ' + p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
                         widget.setSingleStep(p.cmd_instance.step)
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, FloatCommand) or \
                          issubclass(p.cmd_instance.__class__, FloatIndexCommand):
-                        widget = QDoubleSpinBox()
+                        widget = FloatSpinBox()
                         widget.setSuffix(' ' + p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
-                        widget.setSingleStep(p.cmd_instance.step)
-                        widget.setDecimals(math.ceil(math.log10(1.0 / p.cmd_instance.step)))
+                        widget.set_minimum_step(p.cmd_instance.step)
+                        # widget.setSingleStep(p.cmd_instance.step)
+                        #widget.setDecimals(math.ceil(math.log10(1.0 / p.cmd_instance.step)))
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, DictCommand) or \
                          issubclass(p.cmd_instance.__class__, DictIndexCommand):
                         widget = QComboBox()
                         item_list = map(str, p.cmd_instance.set_dict.keys())
                         widget.addItems(item_list)
@@ -137,34 +140,39 @@
                     label = QLabel(name)
                     layout.addWidget(label, row, self.FirstColumn)
                     layout.addWidget(widget, row, self.SecondColumn)
                     row += 1
                     continue
 
                 elif param_type == FloatInput:
-                    widget = QDoubleSpinBox()
+                    widget = FloatSpinBox()
                     setattr(self, name, widget)
-                    widget.setDecimals(4)
+                    widget.set_minimum_step(p.single_step)
+
+                    # widget.setDecimals(4)
                     widget.setAlignment(Qt.AlignRight)
                 elif param_type == IntegerInput:
-                    widget = QSpinBox()
+                    widget = IntegerSpinBox()
                     setattr(self, name, widget)
                     widget.setAlignment(Qt.AlignRight)
                 else:
                     raise TypeError('Unknown input type: {}'.format(param_type))
 
                 if p.value < p.minimum or p.value > p.maximum:
                     widget.setMinimum(p.value)
                     widget.setMaximum(p.value)
                     widget.setEnabled(False)
                 else:
                     widget.setMinimum(p.minimum)
                     widget.setMaximum(p.maximum)
                     widget.setEnabled(True)
-                widget.setSingleStep(p.single_step)
+                if param_type == FloatInput:
+                    widget.set_minimum_step(p.single_step)
+                else:
+                    widget.setSingleStep(p.single_step)
                 widget.setSuffix(' ' + p.suffix)
                 widget.setValue(p.value)
 
                 label = QLabel(name.capitalize())
                 layout.addWidget(label, row, self.FirstColumn)
                 layout.addWidget(widget, row, self.SecondColumn)
                 row += 1
@@ -222,20 +230,20 @@
                         p = params[name]
                         p.cmd_instance = self.get_cmd_instance(p)
                         if hasattr(p.cmd_instance, 'key_type') and \
                            getattr(p.cmd_instance, 'key_type') == 'int':
                             cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
                         else:
                             cmd = '{} = "{}"'.format(params[name].cmd, params[name].text)
-                elif type(widget) == QSpinBox and type(params[name].default_value) == int:
+                elif type(widget) == IntegerSpinBox and type(params[name].default_value) == int:
                     params[name].value = params[name].default_value
                     widget.setValue(params[name].default_value)
                     if type(params[name]) == CommandInput:
                         cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
-                elif type(widget) == QDoubleSpinBox and type(params[name].default_value) == float:
+                elif type(widget) == FloatSpinBox and type(params[name].default_value) == float:
                     params[name].value = params[name].default_value
                     widget.setValue(params[name].default_value)
                     if type(params[name]) == CommandInput:
                         cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
                 else:
                     logger.error('error to reset "{}" to default, {}'.
                                  format(name, params[name].default_value))
@@ -265,33 +273,33 @@
                         if hasattr(p.cmd_instance, 'key_type') and \
                            getattr(p.cmd_instance, 'key_type') is str:
                             fmt = '{} = "{}"'
                         else:
                             fmt = '{} = {}'
                         cmd = fmt.format(params[name].cmd, widget.currentText())
 
-                elif type(widget) in (QSpinBox, QDoubleSpinBox):
+                elif type(widget) in (IntegerSpinBox, FloatSpinBox):
                     params[name].value = widget.value()
                     if type(params[name]) == CommandInput:
                         cmd = '{} = {}'.format(params[name].cmd, widget.value())
 
                 if cmd:
                     self.command_handler.process_command(cmd, '')
 
             logger.debug("{} apply parameters from panel".format(self.__class__.__name__))
         except Exception as e:
             logger.error(e)
 
     def handle_reply(self, cmd, reply):
         try:
             if cmd in self.command_dict:
-                if type(self.command_dict[cmd]) == QSpinBox:
+                if type(self.command_dict[cmd]) == IntegerSpinBox:
                     self.command_dict[cmd].setValue(int(reply))
 
-                elif type(self.command_dict[cmd]) == QDoubleSpinBox:
+                elif type(self.command_dict[cmd]) == FloatSpinBox:
                     self.command_dict[cmd].setValue(float(reply))
 
                 elif type(self.command_dict[cmd]) == QComboBox:
                     index = self.command_dict[cmd].findText(reply)
                     self.command_dict[cmd].setCurrentIndex(index)
 
                 elif type(self.command_dict[cmd]) == QLineEdit:
```

### Comparing `srsgui-0.4.2/srsgui/ui/qt/QtCore.py` & `srsgui-0.4.3/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/qt/QtGui.py` & `srsgui-0.4.3/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.4.3/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/qt/__init__.py` & `srsgui-0.4.3/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/qtloghandler.py` & `srsgui-0.4.3/srsgui/ui/qtloghandler.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ##! 
 
 from logging import getLogger, Handler
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
 
+RedError = '<font color="red"><b>-ERROR-</b></font>'
 logger = getLogger(__name__)
 
 
 class QtLogHandler(Handler):
     """
     Subclass logging.Handler to be used with QTextBrowser widget.
     """
@@ -34,11 +35,11 @@
         message = self.format(record)
         # print(type(message), 'Format:::: {}'.format(message))
         if message:
             self.sig.new_message.emit(message)
             # self.append(message)
 
     def append(self, message):
-        self.text_browser.append(message)
+        self.text_browser.append(message.replace('-ERROR-', RedError, 1))
         sb = self.text_browser.verticalScrollBar()
         sb.setValue(sb.maximum())
```

### Comparing `srsgui-0.4.2/srsgui/ui/resource_rc.py` & `srsgui-0.4.3/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/signalhandler.py` & `srsgui-0.4.3/srsgui/ui/signalhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,24 @@
         sig_text_available,
         sig_parameter_changed,
         sig_figure_update_requested,
         sig_data_available,
         sig_new_question,
     ]
 
-    def __init__(self, parent=None):
+    def __init__(self, parent):
         super().__init__(parent)
 
         # Connect signals from the main widget
         self.sig_text_available.connect(parent.print_redirect)
         self.sig_data_available.connect(parent.task.update)
         self.sig_figure_update_requested.connect(parent.update_figure)
         self.sig_parameter_changed.connect(parent.taskParameter.update)
         self.sig_new_question.connect(parent.display_question)
+        self.sig_started.connect(parent.onTaskStarted)
         self.sig_finished.connect(parent.onTaskFinished)
 
     def started(self):
         self.sig_started.emit()
 
     def finished(self):
         self.sig_finished.emit()
```

### Comparing `srsgui-0.4.2/srsgui/ui/srslogo.jpg` & `srsgui-0.4.3/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/stdout.py` & `srsgui-0.4.3/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/taskmain.py` & `srsgui-0.4.3/srsgui/ui/taskmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,36 +173,38 @@
                         instr.disconnect()
             except Exception as e:
                 logger.error(e)
 
             # Check if argument is given in the command line
             if self.initial_load and len(sys.argv) == 2 and sys.argv[1].split('.')[-1].lower() == 'taskconfig':
                 self.default_config_file = sys.argv[1]
-                self.initial_load = False
-            else:
+            elif not self.initial_load:
                 popped_path = sys.path.pop(0)
                 logger.debug('"{}" removed from sys.path'.format(popped_path))
 
             current_dir = str(Path(self.default_config_file).parent)
             sys.path.insert(0, current_dir)
             os.chdir(current_dir)
+            self.initial_load = False
+
             logger.debug('Set the current directory to "{}"'.format(current_dir))
             self.config.load(self.default_config_file)
             logger.debug('TaskConfig file: "{}"  loading done'.format(self.default_config_file))
 
             for instr in prev_inst_dict:
                 del instr
             self.inst_dict = self.config.inst_dict
             self.task_dict = self.config.task_dict
             self.docs_dict = self.config.docs_dict
 
             self.dock_handler.reset_inst_docks()
 
             self.inst_info_handler.update_tabs()
             for inst_name in self.inst_dict:
+                self.inst_dict[inst_name].check_id()
                 self.inst_info_handler.update_info(inst_name)
 
             self.setWindowTitle(self.config.task_dict_name)
             self.dock_handler.display_image(self.get_logo_file())
 
             self.session_handler = SessionHandler(True, False, False)
             self.session_handler.set_data_directory(self.config.base_data_dir, self.config.task_dict_name)
@@ -317,23 +319,16 @@
                 elif inst_name and message == 'update':
                     self.inst_info_handler.update_info(inst_name)
                 else:
                     self.deviceInfo.append(message)
 
             elif text.startswith(Task.EscapeForStatus):
                 self.statusbar.showMessage(msg[2])
-            elif text.startswith(Task.EscapeForStart):
-                # self.taskInfo.append(text)
-                pass
-            elif text.startswith(Task.EscapeForStop):
-                # self.taskInfo.append(text)
-                # self.clear_busy()
-                pass
             else:
-                raise ValueError("Invalid escape string")
+                raise ValueError("Invalid escape string: {}".format(text))
         except Exception as e:
             logger.error(e)
 
     def onTaskStarted(self):
         # setup toolbar buttons
         self.actionRun.setEnabled(False)
         self.actionStop.setEnabled(True)
@@ -451,15 +446,14 @@
             self.setWindowTitle("{}  -  {}".format(self.config.task_dict_name, self.task.name))
             self.task.set_figure_dict(self.dock_handler.get_figure_dict())
             self.task.set_inst_dict(self.inst_dict)
             self.task.set_data_dict(self.data_dict)
             self.task.set_session_handler(self.session_handler)
             signal_handler = SignalHandler(self)
             self.task.set_callback_handler(signal_handler)
-            self.onTaskStarted()
             self.task.start()
         except Exception as e:
             logger.error(e)
 
     def onStop(self):
         if self.task is not None:
             logger.info('{} stopping'.format(self.task.name))
```

### Comparing `srsgui-0.4.2/srsgui/ui/taskmain.ui` & `srsgui-0.4.3/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui/ui/ui_taskmain.py` & `srsgui-0.4.3/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.2/srsgui.egg-info/PKG-INFO` & `srsgui-0.4.3/srsgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.2
+Version: 0.4.3
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
```

### Comparing `srsgui-0.4.2/srsgui.egg-info/SOURCES.txt` & `srsgui-0.4.3/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

