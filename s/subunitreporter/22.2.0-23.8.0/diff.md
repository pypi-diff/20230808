# Comparing `tmp/subunitreporter-22.2.0.tar.gz` & `tmp/subunitreporter-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subunitreporter-22.2.0.tar", last modified: Mon Feb 14 20:13:09 2022, max compression
+gzip compressed data, was "subunitreporter-23.8.0.tar", last modified: Tue Aug  8 14:13:51 2023, max compression
```

## Comparing `subunitreporter-22.2.0.tar` & `subunitreporter-23.8.0.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2022-02-14 20:13:09.826798 subunitreporter-22.2.0/
--rw-r--r--   0 exarkun   (1000) users      (100)     1091 2022-02-14 16:57:42.000000 subunitreporter-22.2.0/LICENSE
--rw-r--r--   0 exarkun   (1000) users      (100)       45 2022-02-14 16:57:42.000000 subunitreporter-22.2.0/MANIFEST.in
--rw-r--r--   0 exarkun   (1000) users      (100)     2438 2022-02-14 20:13:09.826798 subunitreporter-22.2.0/PKG-INFO
--rw-r--r--   0 exarkun   (1000) users      (100)     1709 2022-02-14 16:57:42.000000 subunitreporter-22.2.0/README.rst
--rw-r--r--   0 exarkun   (1000) users      (100)       61 2022-02-14 20:13:09.826798 subunitreporter-22.2.0/setup.cfg
--rw-r--r--   0 exarkun   (1000) users      (100)      901 2022-02-14 19:59:46.000000 subunitreporter-22.2.0/setup.py
-drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2022-02-14 20:13:09.823799 subunitreporter-22.2.0/src/
-drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2022-02-14 20:13:09.825798 subunitreporter-22.2.0/src/subunitreporter/
--rw-r--r--   0 exarkun   (1000) users      (100)     7100 2022-02-14 20:11:13.000000 subunitreporter-22.2.0/src/subunitreporter/__init__.py
--rw-r--r--   0 exarkun   (1000) users      (100)      248 2022-02-14 20:11:47.000000 subunitreporter-22.2.0/src/subunitreporter/_metadata.py
-drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2022-02-14 20:13:09.826798 subunitreporter-22.2.0/src/subunitreporter.egg-info/
--rw-r--r--   0 exarkun   (1000) users      (100)     2438 2022-02-14 20:13:09.000000 subunitreporter-22.2.0/src/subunitreporter.egg-info/PKG-INFO
--rw-r--r--   0 exarkun   (1000) users      (100)      409 2022-02-14 20:13:09.000000 subunitreporter-22.2.0/src/subunitreporter.egg-info/SOURCES.txt
--rw-r--r--   0 exarkun   (1000) users      (100)        1 2022-02-14 20:13:09.000000 subunitreporter-22.2.0/src/subunitreporter.egg-info/dependency_links.txt
--rw-r--r--   0 exarkun   (1000) users      (100)        1 2022-02-14 20:13:09.000000 subunitreporter-22.2.0/src/subunitreporter.egg-info/not-zip-safe
--rw-r--r--   0 exarkun   (1000) users      (100)       54 2022-02-14 20:13:09.000000 subunitreporter-22.2.0/src/subunitreporter.egg-info/requires.txt
--rw-r--r--   0 exarkun   (1000) users      (100)       24 2022-02-14 20:13:09.000000 subunitreporter-22.2.0/src/subunitreporter.egg-info/top_level.txt
-drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2022-02-14 20:13:09.823799 subunitreporter-22.2.0/src/twisted/
-drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2022-02-14 20:13:09.826798 subunitreporter-22.2.0/src/twisted/plugins/
--rw-r--r--   0 exarkun   (1000) users      (100)     1251 2022-02-14 16:57:42.000000 subunitreporter-22.2.0/src/twisted/plugins/subunitreporter.py
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.413360 subunitreporter-23.8.0/
+-rw-r--r--   0 exarkun   (1000) users      (100)     1091 2022-02-14 16:57:42.000000 subunitreporter-23.8.0/LICENSE
+-rw-r--r--   0 exarkun   (1000) users      (100)       45 2022-02-14 16:57:42.000000 subunitreporter-23.8.0/MANIFEST.in
+-rw-r--r--   0 exarkun   (1000) users      (100)     1967 2023-08-08 14:13:51.413360 subunitreporter-23.8.0/PKG-INFO
+-rw-r--r--   0 exarkun   (1000) users      (100)     1709 2022-02-14 16:57:42.000000 subunitreporter-23.8.0/README.rst
+-rw-r--r--   0 exarkun   (1000) users      (100)       61 2023-08-08 14:13:51.413360 subunitreporter-23.8.0/setup.cfg
+-rw-r--r--   0 exarkun   (1000) users      (100)      901 2022-02-14 19:59:46.000000 subunitreporter-23.8.0/setup.py
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.411360 subunitreporter-23.8.0/src/
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.412360 subunitreporter-23.8.0/src/subunitreporter/
+-rw-r--r--   0 exarkun   (1000) users      (100)     7712 2023-08-08 14:01:01.000000 subunitreporter-23.8.0/src/subunitreporter/__init__.py
+-rw-r--r--   0 exarkun   (1000) users      (100)      248 2023-08-08 14:01:50.000000 subunitreporter-23.8.0/src/subunitreporter/_metadata.py
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.413360 subunitreporter-23.8.0/src/subunitreporter/test/
+-rw-r--r--   0 exarkun   (1000) users      (100)       39 2022-04-28 20:11:31.000000 subunitreporter-23.8.0/src/subunitreporter/test/__init__.py
+-rw-r--r--   0 exarkun   (1000) users      (100)      124 2022-04-28 20:11:31.000000 subunitreporter-23.8.0/src/subunitreporter/test/cases.py
+-rw-r--r--   0 exarkun   (1000) users      (100)     2496 2022-04-28 20:11:31.000000 subunitreporter-23.8.0/src/subunitreporter/test/test_distreporter_integration.py
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.412360 subunitreporter-23.8.0/src/subunitreporter.egg-info/
+-rw-r--r--   0 exarkun   (1000) users      (100)     1967 2023-08-08 14:13:51.000000 subunitreporter-23.8.0/src/subunitreporter.egg-info/PKG-INFO
+-rw-r--r--   0 exarkun   (1000) users      (100)      568 2023-08-08 14:13:51.000000 subunitreporter-23.8.0/src/subunitreporter.egg-info/SOURCES.txt
+-rw-r--r--   0 exarkun   (1000) users      (100)        1 2023-08-08 14:13:51.000000 subunitreporter-23.8.0/src/subunitreporter.egg-info/dependency_links.txt
+-rw-r--r--   0 exarkun   (1000) users      (100)        1 2022-02-14 20:13:09.000000 subunitreporter-23.8.0/src/subunitreporter.egg-info/not-zip-safe
+-rw-r--r--   0 exarkun   (1000) users      (100)       54 2023-08-08 14:13:51.000000 subunitreporter-23.8.0/src/subunitreporter.egg-info/requires.txt
+-rw-r--r--   0 exarkun   (1000) users      (100)       24 2023-08-08 14:13:51.000000 subunitreporter-23.8.0/src/subunitreporter.egg-info/top_level.txt
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.411360 subunitreporter-23.8.0/src/twisted/
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.413360 subunitreporter-23.8.0/src/twisted/plugins/
+-rw-r--r--   0 exarkun   (1000) users      (100)     1251 2022-02-14 16:57:42.000000 subunitreporter-23.8.0/src/twisted/plugins/subunitreporter.py
+drwxr-xr-x   0 exarkun   (1000) users      (100)        0 2023-08-08 14:13:51.413360 subunitreporter-23.8.0/tests/
+-rw-r--r--   0 exarkun   (1000) users      (100)      511 2022-02-14 20:11:13.000000 subunitreporter-23.8.0/tests/test_subunitreporter.py
```

### Comparing `subunitreporter-22.2.0/LICENSE` & `subunitreporter-23.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subunitreporter-22.2.0/PKG-INFO` & `subunitreporter-23.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: subunitreporter
-Version: 22.2.0
+Version: 23.8.0
 Summary: A Twisted Trial reporter which emits Subunit v2 streams.
 Home-page: https://github.com/LeastAuthority/subunitreporter
 Author: subunitreporter Developers
-Author-email: UNKNOWN
 License: MIT
-Description: subunitreporter
-        ===============
-        
-        .. image:: http://img.shields.io/pypi/v/subunitreporter.svg
-           :target: https://pypi.python.org/pypi/subunitreporter
-           :alt: PyPI Package
-        
-        What is this?
-        -------------
-        
-        subunitreporter is a plugin for Twisted Trial which adds two new reporters.
-        The ``subunitv2`` reporter emits subunit v2 result streams with timing information.
-        The ``subunitv2-b64`` reporter emits the same information, base64-encoded.
-        The ``subunitv2-file`` reporter emits the same information,
-        written directly to a file instead of the normal trial output stream.
-        The ``subunitv2-file`` reporter can also emit progress information to the normal reporting stream
-        (usually stdout)
-        to avoid falling prey to hang-detection based on amount of time with no output.
-        
-        Usage Sample
-        ------------
-        
-        Use this with your trial command-lines.
-        For example::
-        
-          $ trial --reporter=subunitv2 ... | subunit-stats
-          $ trial --reporter=subunitv2-b64 ... | base64 -d | subunit-stats
-          $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --reporter=subunitv2-file ...
-          $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --rterrors --reporter=subunitv2-file ...
-        
-        Installing
-        ----------
-        
-        To install the latest version of subunitreporter using pip::
-        
-          $ pip install subunitreporter
-        
-        For additional development dependencies, install the ``dev`` extra::
-        
-          $ pip install subunitreporter[dev]
-        
-        Testing
-        -------
-        
-        subunitreporter uses pyunit-style tests.
-        After installing the development dependencies, you can run the test suite with trial::
-        
-          $ pip install subunitreporter[dev]
-          $ trial subunitreporter
-        
-        License
-        -------
-        
-        subunitreporter is open source software released under the MIT License.
-        See the LICENSE file for more details.
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+subunitreporter
+===============
+
+.. image:: http://img.shields.io/pypi/v/subunitreporter.svg
+   :target: https://pypi.python.org/pypi/subunitreporter
+   :alt: PyPI Package
+
+What is this?
+-------------
+
+subunitreporter is a plugin for Twisted Trial which adds two new reporters.
+The ``subunitv2`` reporter emits subunit v2 result streams with timing information.
+The ``subunitv2-b64`` reporter emits the same information, base64-encoded.
+The ``subunitv2-file`` reporter emits the same information,
+written directly to a file instead of the normal trial output stream.
+The ``subunitv2-file`` reporter can also emit progress information to the normal reporting stream
+(usually stdout)
+to avoid falling prey to hang-detection based on amount of time with no output.
+
+Usage Sample
+------------
+
+Use this with your trial command-lines.
+For example::
+
+  $ trial --reporter=subunitv2 ... | subunit-stats
+  $ trial --reporter=subunitv2-b64 ... | base64 -d | subunit-stats
+  $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --reporter=subunitv2-file ...
+  $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --rterrors --reporter=subunitv2-file ...
+
+Installing
+----------
+
+To install the latest version of subunitreporter using pip::
+
+  $ pip install subunitreporter
+
+For additional development dependencies, install the ``dev`` extra::
+
+  $ pip install subunitreporter[dev]
+
+Testing
+-------
+
+subunitreporter uses pyunit-style tests.
+After installing the development dependencies, you can run the test suite with trial::
+
+  $ pip install subunitreporter[dev]
+  $ trial subunitreporter
+
+License
+-------
+
+subunitreporter is open source software released under the MIT License.
+See the LICENSE file for more details.
```

### Comparing `subunitreporter-22.2.0/README.rst` & `subunitreporter-23.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `subunitreporter-22.2.0/setup.py` & `subunitreporter-23.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `subunitreporter-22.2.0/src/subunitreporter/__init__.py` & `subunitreporter-23.8.0/src/subunitreporter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,20 +28,29 @@
         ExtendedToStreamDecorator(
             StreamResultToBytes(
                 reporter.stream,
             ),
         ),
     )
 
+def _open_output(name):
+    """
+    Open a file with a configuration suitable for use as our output
+    stream.
+    """
+    return open(name, "wt", encoding="utf-8")
+
 def _default_progress_stream():
-    return open(devnull, "wt")
+    return _open_output(devnull)
 
 def _progress_stream(v):
     if v is None:
-        return _default_progress_stream()
+        v = _default_progress_stream()
+        return v
+    v.reconfigure(encoding="utf-8")
     return v
 
 @attr.s
 @implementer(IReporter)
 class _SubunitReporter(object):
     """
     Reports test output using the subunit v2 protocol.
@@ -137,38 +146,39 @@
         self._subunit.addSkip(test, reason)
 
     def addError(self, test, err):
         """
         Record that ``test`` failed with an unexpected error ``err``.
         """
         self.progress_stream.write(self._ERROR_MARK)
-        return self._subunit.addError(
-            test,
-            excInfoOrFailureToExcInfo(err),
-        )
+        exc_type, exc_value, exc_tb = excInfoOrFailureToExcInfo(err)
+        if isinstance(exc_value, str):
+            # work around twisted#10333
+            exc_value = Exception(exc_value)
+        return self._subunit.addError(test, (exc_type, exc_value, exc_tb))
 
     def addFailure(self, test, err):
         """
         Record that ``test`` failed an assertion with the error ``err``.
         """
         self.progress_stream.write(self._FAIL_MARK)
-        return self._subunit.addFailure(
-            test,
-            excInfoOrFailureToExcInfo(err),
-        )
+        exc_type, exc_value, exc_tb = excInfoOrFailureToExcInfo(err)
+        if isinstance(exc_value, str):
+            exc_value = Exception(exc_value)
+        return self._subunit.addFailure(test, (exc_type, exc_value, exc_tb))
 
     def addExpectedFailure(self, test, failure, todo):
         """
         Record an expected failure from a test.
         """
         self.progress_stream.write(self._XFAIL_MARK)
-        self._subunit.addExpectedFailure(
-            test,
-            excInfoOrFailureToExcInfo(failure),
-        )
+        exc_type, exc_value, exc_tb = excInfoOrFailureToExcInfo(failure)
+        if isinstance(exc_value, str):
+            exc_value = Exception(exc_value)
+        self._subunit.addExpectedFailure(test, (exc_type, exc_value, exc_tb))
 
     def addUnexpectedSuccess(self, test, todo=None):
         """
         Record an unexpected success.
 
         Since subunit has no way of expressing this concept, we record a
         success on the subunit stream.
@@ -223,15 +233,15 @@
         to mean something somewhat different than the intent, here, but it's
         an easy way to a boolean argument in as configuration.
     """
     if realtime:
         progress_stream = stream
     else:
         progress_stream = None
-    stream = open(environ["SUBUNITREPORTER_OUTPUT_PATH"], "wb")
+    stream = _open_output(environ["SUBUNITREPORTER_OUTPUT_PATH"])
     return _SubunitReporter(stream=stream, progress_stream=progress_stream)
 
 
 @attr.s
 class _Base64Bytes(object):
     stream = attr.ib()
```

### Comparing `subunitreporter-22.2.0/src/subunitreporter.egg-info/PKG-INFO` & `subunitreporter-23.8.0/src/subunitreporter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: subunitreporter
-Version: 22.2.0
+Version: 23.8.0
 Summary: A Twisted Trial reporter which emits Subunit v2 streams.
 Home-page: https://github.com/LeastAuthority/subunitreporter
 Author: subunitreporter Developers
-Author-email: UNKNOWN
 License: MIT
-Description: subunitreporter
-        ===============
-        
-        .. image:: http://img.shields.io/pypi/v/subunitreporter.svg
-           :target: https://pypi.python.org/pypi/subunitreporter
-           :alt: PyPI Package
-        
-        What is this?
-        -------------
-        
-        subunitreporter is a plugin for Twisted Trial which adds two new reporters.
-        The ``subunitv2`` reporter emits subunit v2 result streams with timing information.
-        The ``subunitv2-b64`` reporter emits the same information, base64-encoded.
-        The ``subunitv2-file`` reporter emits the same information,
-        written directly to a file instead of the normal trial output stream.
-        The ``subunitv2-file`` reporter can also emit progress information to the normal reporting stream
-        (usually stdout)
-        to avoid falling prey to hang-detection based on amount of time with no output.
-        
-        Usage Sample
-        ------------
-        
-        Use this with your trial command-lines.
-        For example::
-        
-          $ trial --reporter=subunitv2 ... | subunit-stats
-          $ trial --reporter=subunitv2-b64 ... | base64 -d | subunit-stats
-          $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --reporter=subunitv2-file ...
-          $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --rterrors --reporter=subunitv2-file ...
-        
-        Installing
-        ----------
-        
-        To install the latest version of subunitreporter using pip::
-        
-          $ pip install subunitreporter
-        
-        For additional development dependencies, install the ``dev`` extra::
-        
-          $ pip install subunitreporter[dev]
-        
-        Testing
-        -------
-        
-        subunitreporter uses pyunit-style tests.
-        After installing the development dependencies, you can run the test suite with trial::
-        
-          $ pip install subunitreporter[dev]
-          $ trial subunitreporter
-        
-        License
-        -------
-        
-        subunitreporter is open source software released under the MIT License.
-        See the LICENSE file for more details.
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+subunitreporter
+===============
+
+.. image:: http://img.shields.io/pypi/v/subunitreporter.svg
+   :target: https://pypi.python.org/pypi/subunitreporter
+   :alt: PyPI Package
+
+What is this?
+-------------
+
+subunitreporter is a plugin for Twisted Trial which adds two new reporters.
+The ``subunitv2`` reporter emits subunit v2 result streams with timing information.
+The ``subunitv2-b64`` reporter emits the same information, base64-encoded.
+The ``subunitv2-file`` reporter emits the same information,
+written directly to a file instead of the normal trial output stream.
+The ``subunitv2-file`` reporter can also emit progress information to the normal reporting stream
+(usually stdout)
+to avoid falling prey to hang-detection based on amount of time with no output.
+
+Usage Sample
+------------
+
+Use this with your trial command-lines.
+For example::
+
+  $ trial --reporter=subunitv2 ... | subunit-stats
+  $ trial --reporter=subunitv2-b64 ... | base64 -d | subunit-stats
+  $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --reporter=subunitv2-file ...
+  $ SUBUNITREPORTER_OUTPUT_PATH=results.subunit2 trial --rterrors --reporter=subunitv2-file ...
+
+Installing
+----------
+
+To install the latest version of subunitreporter using pip::
+
+  $ pip install subunitreporter
+
+For additional development dependencies, install the ``dev`` extra::
+
+  $ pip install subunitreporter[dev]
+
+Testing
+-------
+
+subunitreporter uses pyunit-style tests.
+After installing the development dependencies, you can run the test suite with trial::
+
+  $ pip install subunitreporter[dev]
+  $ trial subunitreporter
+
+License
+-------
+
+subunitreporter is open source software released under the MIT License.
+See the LICENSE file for more details.
```

### Comparing `subunitreporter-22.2.0/src/twisted/plugins/subunitreporter.py` & `subunitreporter-23.8.0/src/twisted/plugins/subunitreporter.py`

 * *Files identical despite different names*

