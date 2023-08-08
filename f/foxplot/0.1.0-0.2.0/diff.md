# Comparing `tmp/foxplot-0.1.0.tar.gz` & `tmp/foxplot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxplot-0.1.0.tar", last modified: Tue May 23 17:58:24 2023, max compression
+gzip compressed data, was "foxplot-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `foxplot-0.1.0.tar` & `foxplot-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
--rw-r--r--   0        0        0     2700 2023-05-03 10:05:19.625704 foxplot-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1268 2023-05-03 10:16:36.797927 foxplot-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0       62 2023-05-03 10:05:19.625704 foxplot-0.1.0/.gitignore
--rw-r--r--   0        0        0      728 2023-05-23 17:57:57.262019 foxplot-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-01-26 08:59:41.542467 foxplot-0.1.0/LICENSE
--rw-r--r--   0        0        0       30 2023-01-26 08:59:41.542467 foxplot-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     2248 2023-05-23 17:57:22.370680 foxplot-0.1.0/README.md
--rw-r--r--   0        0        0       51 2023-05-03 10:05:19.625704 foxplot-0.1.0/docs/api.rst
--rw-r--r--   0        0        0     9358 2023-05-03 10:05:19.625704 foxplot-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      204 2023-05-03 10:05:19.625704 foxplot-0.1.0/docs/environment.yml
--rw-r--r--   0        0        0      253 2023-05-03 10:05:19.629704 foxplot-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      202 2023-05-03 10:05:19.629704 foxplot-0.1.0/docs/installation.rst
--rw-r--r--   0        0        0      983 2023-05-16 17:17:17.695690 foxplot-0.1.0/docs/usage.rst
--rw-r--r--   0        0        0     1073 2023-04-25 14:58:06.539529 foxplot-0.1.0/examples/plot_robot_data.py
--rw-r--r--   0        0        0   128378 2023-04-25 14:37:52.909959 foxplot-0.1.0/examples/robot_data.json
--rw-r--r--   0        0        0      747 2023-05-23 17:58:03.477903 foxplot-0.1.0/foxplot/__init__.py
--rw-r--r--   0        0        0     3682 2023-05-23 17:57:22.374680 foxplot-0.1.0/foxplot/cli.py
--rw-r--r--   0        0        0     1442 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/color_picker.py
--rw-r--r--   0        0        0      777 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/decoders/__init__.py
--rw-r--r--   0        0        0     1469 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/decoders/json.py
--rw-r--r--   0        0        0     1302 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/decoders/msgpack.py
--rw-r--r--   0        0        0      736 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/exceptions.py
--rw-r--r--   0        0        0     6137 2023-05-23 17:57:22.374680 foxplot-0.1.0/foxplot/fox.py
--rw-r--r--   0        0        0     8177 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/generate_html.py
--rw-r--r--   0        0        0     1597 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/indexed_series.py
--rw-r--r--   0        0        0     3231 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/node.py
--rw-r--r--   0        0        0   120184 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/uPlot/uPlot.iife.js
--rw-r--r--   0        0        0     1839 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/uPlot/uPlot.min.css
--rw-r--r--   0        0        0     4543 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/uPlot/uPlot.mousewheel.js
--rw-r--r--   0        0        0     1217 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/write_tmpfile.py
--rw-r--r--   0        0        0     1544 2023-05-16 17:17:17.695690 foxplot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-01-26 08:59:41.542467 foxplot-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-04 12:24:42.147920 foxplot-0.1.0/tests/test_color_picker.py
--rw-r--r--   0        0        0     1739 2023-05-03 09:37:04.510756 foxplot-0.1.0/tests/test_decoders.py
--rw-r--r--   0        0        0     6603 2023-04-24 12:24:53.005389 foxplot-0.1.0/tests/test_fox.py
--rw-r--r--   0        0        0     1074 2023-04-24 11:57:18.540637 foxplot-0.1.0/tests/test_generate_html.py
--rw-r--r--   0        0        0      739 2023-05-03 09:37:04.510756 foxplot-0.1.0/tox.ini
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 foxplot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      690 2023-07-27 13:12:41.050629 foxplot-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      565 2023-07-27 13:12:41.050629 foxplot-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2700 2023-05-23 18:05:24.471113 foxplot-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1268 2023-05-23 18:05:24.471113 foxplot-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       62 2023-05-23 18:05:24.471113 foxplot-0.2.0/.gitignore
+-rw-r--r--   0        0        0      995 2023-08-08 09:44:07.133459 foxplot-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-23 18:05:24.471113 foxplot-0.2.0/LICENSE
+-rw-r--r--   0        0        0       30 2023-05-23 18:05:24.471113 foxplot-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     2494 2023-08-08 09:57:33.908961 foxplot-0.2.0/README.md
+-rw-r--r--   0        0        0       51 2023-05-23 18:05:24.471113 foxplot-0.2.0/docs/api.rst
+-rw-r--r--   0        0        0     9358 2023-05-23 18:05:24.471113 foxplot-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      204 2023-05-23 18:05:24.471113 foxplot-0.2.0/docs/environment.yml
+-rw-r--r--   0        0        0      253 2023-05-23 18:05:24.471113 foxplot-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      202 2023-05-23 18:05:24.471113 foxplot-0.2.0/docs/installation.rst
+-rw-r--r--   0        0        0      983 2023-05-23 18:05:24.471113 foxplot-0.2.0/docs/usage.rst
+-rw-r--r--   0        0        0     1073 2023-05-23 18:05:24.471113 foxplot-0.2.0/examples/plot_robot_data.py
+-rw-r--r--   0        0        0   128378 2023-05-23 18:05:24.471113 foxplot-0.2.0/examples/robot_data.json
+-rw-r--r--   0        0        0      747 2023-08-08 09:43:57.349563 foxplot-0.2.0/foxplot/__init__.py
+-rw-r--r--   0        0        0     3682 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/cli.py
+-rw-r--r--   0        0        0     1442 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/color_picker.py
+-rw-r--r--   0        0        0      777 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/decoders/__init__.py
+-rw-r--r--   0        0        0     1469 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/decoders/json.py
+-rw-r--r--   0        0        0     1302 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/decoders/msgpack.py
+-rw-r--r--   0        0        0      736 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/exceptions.py
+-rw-r--r--   0        0        0     6137 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/fox.py
+-rw-r--r--   0        0        0     8216 2023-07-27 13:12:41.054629 foxplot-0.2.0/foxplot/generate_html.py
+-rw-r--r--   0        0        0     1597 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/indexed_series.py
+-rw-r--r--   0        0        0     3231 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/node.py
+-rw-r--r--   0        0        0   120184 2023-05-23 18:05:24.471113 foxplot-0.2.0/foxplot/uPlot/uPlot.iife.js
+-rw-r--r--   0        0        0     1839 2023-05-23 18:05:24.475113 foxplot-0.2.0/foxplot/uPlot/uPlot.min.css
+-rw-r--r--   0        0        0     4543 2023-05-23 18:05:24.475113 foxplot-0.2.0/foxplot/uPlot/uPlot.mousewheel.js
+-rw-r--r--   0        0        0     1217 2023-05-23 18:05:24.475113 foxplot-0.2.0/foxplot/write_tmpfile.py
+-rw-r--r--   0        0        0     1579 2023-08-08 09:43:40.749737 foxplot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-05-23 18:05:24.475113 foxplot-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-05-23 18:05:24.475113 foxplot-0.2.0/tests/test_color_picker.py
+-rw-r--r--   0        0        0     1739 2023-05-23 18:05:24.475113 foxplot-0.2.0/tests/test_decoders.py
+-rw-r--r--   0        0        0     6603 2023-05-23 18:05:24.475113 foxplot-0.2.0/tests/test_fox.py
+-rw-r--r--   0        0        0     1074 2023-05-23 18:05:24.475113 foxplot-0.2.0/tests/test_generate_html.py
+-rw-r--r--   0        0        0      781 2023-07-27 13:12:41.054629 foxplot-0.2.0/tox.ini
+-rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 foxplot-0.2.0/PKG-INFO
```

### Comparing `foxplot-0.1.0/.github/workflows/CI.yml` & `foxplot-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/.github/workflows/docs.yml` & `foxplot-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/LICENSE` & `foxplot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/README.md` & `foxplot-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # foxplot
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/CI.yml?branch=main)](https://github.com/stephane-caron/foxplot/actions)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/foxplot/)
+[![Coverage](https://coveralls.io/repos/github/stephane-caron/foxplot/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/foxplot?branch=main)
 
 Plot time-series data from [newline-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Newline-delimited-JSON).
 
-Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case (robotic control loops). Dictionaries are the observation format used in [Vulp](https://github.com/tasts-robots/vulp). Plots are plots :wink:
+Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case with robot control loops, while dictionaries are a common weakly-typed self-describing format (used *e.g.* in the [GitHub REST API](https://docs.github.com/en/rest/), [robot logging](https://github.com/tasts-robots/mpacklog), ...).
 
 ## Installation
 
 ```console
-$ pip install foxplot
+pip install foxplot
 ```
 
 ## Usage
 
 ### Interactive mode
 
 In interactive mode, you can explore the data in ``data`` (tab completion works) and plot it using the ``fox.plot`` function:
```

### Comparing `foxplot-0.1.0/docs/conf.py` & `foxplot-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/docs/usage.rst` & `foxplot-0.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/examples/plot_robot_data.py` & `foxplot-0.2.0/examples/plot_robot_data.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/examples/robot_data.json` & `foxplot-0.2.0/examples/robot_data.json`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/__init__.py` & `foxplot-0.2.0/foxplot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Plot time-series data from line-delimited JSON."""
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 from .fox import Fox
 
 __all__ = ["Fox"]
```

### Comparing `foxplot-0.1.0/foxplot/cli.py` & `foxplot-0.2.0/foxplot/cli.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/color_picker.py` & `foxplot-0.2.0/foxplot/color_picker.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/decoders/__init__.py` & `foxplot-0.2.0/foxplot/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/decoders/json.py` & `foxplot-0.2.0/foxplot/decoders/json.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/decoders/msgpack.py` & `foxplot-0.2.0/foxplot/decoders/msgpack.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/exceptions.py` & `foxplot-0.2.0/foxplot/exceptions.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/fox.py` & `foxplot-0.2.0/foxplot/fox.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/generate_html.py` & `foxplot-0.2.0/foxplot/generate_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     uplot_min_css = resource_filename("foxplot", "uPlot/uPlot.min.css")
     uplot_iife_js = resource_filename("foxplot", "uPlot/uPlot.iife.js")
     uplot_mwheel_js = resource_filename("foxplot", "uPlot/uPlot.mousewheel.js")
 
     color_picker = ColorPicker()
     left_axis_label = f" {left_axis_unit}" if left_axis_unit else ""
     right_axis_label = f" {right_axis_unit}" if right_axis_unit else ""
-    left_labels = set(left_axis.keys())
-    right_labels = set(right_axis.keys())
-    labels = left_labels | right_labels
+    left_labels = list(left_axis.keys())
+    right_labels = list(right_axis.keys())
+    labels = left_labels + [r for r in right_labels if r not in left_labels]
     series_from_label = {}
     series_from_label.update(left_axis)
     series_from_label.update(right_axis)
     if None in times:
         raise ValueError("time index cannot contain None values")
     html = f"""<!DOCTYPE html>
 <html lang="en">
@@ -175,15 +175,15 @@
                         time: {"true" if timestamped else "false"},
                     }},
                 }},
                 series: ["""
     html += f"""
                     {{
                         value: (self, rawValue) => Number.parseFloat(rawValue -
-                        {times[0]}).toPrecision(3),
+                        {times[0]}).toPrecision(4),
                     }},"""
     for label in labels:
         html += f"""
                     {{
                         // initial toggled state (optional)
                         show: true,
                         spanGaps: false,
```

### Comparing `foxplot-0.1.0/foxplot/indexed_series.py` & `foxplot-0.2.0/foxplot/indexed_series.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/node.py` & `foxplot-0.2.0/foxplot/node.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/uPlot/uPlot.iife.js` & `foxplot-0.2.0/foxplot/uPlot/uPlot.iife.js`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/uPlot/uPlot.min.css` & `foxplot-0.2.0/foxplot/uPlot/uPlot.min.css`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/uPlot/uPlot.mousewheel.js` & `foxplot-0.2.0/foxplot/uPlot/uPlot.mousewheel.js`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/foxplot/write_tmpfile.py` & `foxplot-0.2.0/foxplot/write_tmpfile.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/pyproject.toml` & `foxplot-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 maintainers = [
     {name = "Stéphane Caron", email = "stephane.caron@normalesup.org"},
 ]
 dynamic = ['version', 'description']
 requires-python = ">=3.7"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -37,14 +37,17 @@
 Source = "https://github.com/stephane-caron/foxplot"
 Tracker = "https://github.com/stephane-caron/foxplot/issues"
 Changelog = "https://github.com/stephane-caron/foxplot/blob/master/CHANGELOG.md"
 
 [tool.black]
 line-length = 79
 
+[tool.pytype]
+inputs = ['foxplot']
+
 [tool.ruff]
 line-length = 79
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E",
```

### Comparing `foxplot-0.1.0/tests/test_color_picker.py` & `foxplot-0.2.0/tests/test_color_picker.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/tests/test_decoders.py` & `foxplot-0.2.0/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/tests/test_fox.py` & `foxplot-0.2.0/tests/test_fox.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/tests/test_generate_html.py` & `foxplot-0.2.0/tests/test_generate_html.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.1.0/tox.ini` & `foxplot-0.2.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     coverage report --include="foxplot/**"
 
 [testenv:lint]
 deps =
     black >=22.10.0
     mypy >=0.812
     pylint >=2.8.2
+    pytype >=2023.5.24
     ruff >=0.0.220
     types-setuptools >=65.6.0.2
 commands =
     black --check --diff foxplot
-    ruff foxplot
-    pylint foxplot --exit-zero --rcfile={toxinidir}/tox.ini
     mypy foxplot --ignore-missing-imports
+    pylint foxplot --exit-zero --rcfile={toxinidir}/tox.ini
+    pytype foxplot
+    ruff foxplot
```

### Comparing `foxplot-0.1.0/PKG-INFO` & `foxplot-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: foxplot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Plot time-series data from line-delimited JSON.
 Keywords: json,time,series,plot
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,23 +22,24 @@
 Project-URL: Source, https://github.com/stephane-caron/foxplot
 Project-URL: Tracker, https://github.com/stephane-caron/foxplot/issues
 
 # foxplot
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/CI.yml?branch=main)](https://github.com/stephane-caron/foxplot/actions)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/foxplot/)
+[![Coverage](https://coveralls.io/repos/github/stephane-caron/foxplot/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/foxplot?branch=main)
 
 Plot time-series data from [newline-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Newline-delimited-JSON).
 
-Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case (robotic control loops). Dictionaries are the observation format used in [Vulp](https://github.com/tasts-robots/vulp). Plots are plots :wink:
+Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case with robot control loops, while dictionaries are a common weakly-typed self-describing format (used *e.g.* in the [GitHub REST API](https://docs.github.com/en/rest/), [robot logging](https://github.com/tasts-robots/mpacklog), ...).
 
 ## Installation
 
 ```console
-$ pip install foxplot
+pip install foxplot
 ```
 
 ## Usage
 
 ### Interactive mode
 
 In interactive mode, you can explore the data in ``data`` (tab completion works) and plot it using the ``fox.plot`` function:
```

