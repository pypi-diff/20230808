# Comparing `tmp/soagen-0.4.0.tar.gz` & `tmp/soagen-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.4.0.tar", last modified: Sun Aug  6 15:06:20 2023, max compression
+gzip compressed data, was "soagen-0.5.0.tar", last modified: Tue Aug  8 19:04:02 2023, max compression
```

## Comparing `soagen-0.4.0.tar` & `soagen-0.5.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.058867 soagen-0.4.0/
--rw-rw-rw-   0        0        0     1154 2023-08-06 15:05:21.000000 soagen-0.4.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2499 2023-08-06 15:06:20.058867 soagen-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.4.0/README.md
--rw-rw-rw-   0        0        0     1893 2023-08-03 12:48:33.000000 soagen-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 15:06:20.059866 soagen-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.010866 soagen-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.034867 soagen-0.4.0/src/soagen/
--rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.4.0/src/soagen/column.py
--rw-rw-rw-   0        0        0     5264 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/config.py
--rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/configurable.py
--rw-rw-rw-   0        0        0    19094 2023-08-05 12:32:31.000000 soagen-0.4.0/src/soagen/cpp.py
--rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/errors.py
--rw-rw-rw-   0        0        0    11685 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.053869 soagen-0.4.0/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5693 2023-08-06 15:03:06.000000 soagen-0.4.0/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0    11199 2023-08-06 12:21:38.000000 soagen-0.4.0/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    36529 2023-08-06 09:59:43.000000 soagen-0.4.0/src/soagen/hpp/column_traits.hpp
--rw-rw-rw-   0        0        0    27306 2023-08-06 12:56:25.000000 soagen-0.4.0/src/soagen/hpp/core.hpp
--rw-rw-rw-   0        0        0     1680 2023-08-06 09:10:24.000000 soagen-0.4.0/src/soagen/hpp/emplacer.hpp
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.056869 soagen-0.4.0/src/soagen/hpp/generated/
--rw-rw-rw-   0        0        0     9858 2023-08-06 15:03:06.000000 soagen-0.4.0/src/soagen/hpp/generated/compressed_pair.hpp
--rw-rw-rw-   0        0        0     3859 2023-08-06 15:03:06.000000 soagen-0.4.0/src/soagen/hpp/generated/functions.hpp
--rw-rw-rw-   0        0        0    42666 2023-08-06 15:03:08.000000 soagen-0.4.0/src/soagen/hpp/generated/preprocessor.hpp
--rw-rw-rw-   0        0        0      420 2023-08-05 21:19:05.000000 soagen-0.4.0/src/soagen/hpp/generated/version.hpp
--rw-rw-rw-   0        0        0      868 2023-08-05 10:16:57.000000 soagen-0.4.0/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0     1073 2023-08-05 13:12:06.000000 soagen-0.4.0/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0     3250 2023-08-06 09:18:47.000000 soagen-0.4.0/src/soagen/hpp/invoke.hpp
--rw-rw-rw-   0        0        0    12689 2023-08-06 12:17:28.000000 soagen-0.4.0/src/soagen/hpp/iterator.hpp
--rw-rw-rw-   0        0        0     5481 2023-08-06 09:45:57.000000 soagen-0.4.0/src/soagen/hpp/mixins.hpp
--rw-rw-rw-   0        0        0    12609 2023-08-06 12:56:31.000000 soagen-0.4.0/src/soagen/hpp/row.hpp
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.057867 soagen-0.4.0/src/soagen/hpp/single/
--rw-rw-rw-   0        0        0   234028 2023-08-06 15:05:21.000000 soagen-0.4.0/src/soagen/hpp/single/soagen.hpp
--rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    56937 2023-08-06 09:40:50.000000 soagen-0.4.0/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    34687 2023-08-06 09:19:24.000000 soagen-0.4.0/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0     3680 2023-08-06 15:05:21.000000 soagen-0.4.0/src/soagen/hpp/tuples.hpp
--rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.4.0/src/soagen/includes.py
--rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.4.0/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/log.py
--rw-rw-rw-   0        0        0    22644 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/main.py
--rw-rw-rw-   0        0        0     3529 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     6453 2023-08-04 15:13:48.000000 soagen-0.4.0/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/paths.py
--rw-rw-rw-   0        0        0     6808 2023-08-05 11:46:44.000000 soagen-0.4.0/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.4.0/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    70014 2023-08-05 21:07:07.000000 soagen-0.4.0/src/soagen/struct.py
--rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     1657 2023-08-03 12:36:06.000000 soagen-0.4.0/src/soagen/utils.py
--rw-rw-rw-   0        0        0     3544 2023-08-05 12:31:21.000000 soagen-0.4.0/src/soagen/variable.py
--rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.4.0/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-08-05 21:19:05.000000 soagen-0.4.0/src/soagen/version.txt
--rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.4.0/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-08-06 15:06:20.040866 soagen-0.4.0/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     2499 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1433 2023-08-06 15:06:20.000000 soagen-0.4.0/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-06 15:06:19.000000 soagen-0.4.0/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.4.0/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.738071 soagen-0.5.0/
+-rw-rw-rw-   0        0        0     1284 2023-08-08 18:41:22.000000 soagen-0.5.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2635 2023-08-08 19:04:02.737071 soagen-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.5.0/README.md
+-rw-rw-rw-   0        0        0     1893 2023-08-03 12:48:33.000000 soagen-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 19:04:02.738071 soagen-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.687071 soagen-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.714071 soagen-0.5.0/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.5.0/src/soagen/column.py
+-rw-rw-rw-   0        0        0     5264 2023-08-04 15:13:48.000000 soagen-0.5.0/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19094 2023-08-05 12:32:31.000000 soagen-0.5.0/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    11382 2023-08-08 17:03:42.000000 soagen-0.5.0/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.732071 soagen-0.5.0/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5693 2023-08-08 18:51:46.000000 soagen-0.5.0/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11199 2023-08-06 12:21:38.000000 soagen-0.5.0/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    36875 2023-08-08 18:11:52.000000 soagen-0.5.0/src/soagen/hpp/column_traits.hpp
+-rw-rw-rw-   0        0        0    29658 2023-08-08 18:37:58.000000 soagen-0.5.0/src/soagen/hpp/core.hpp
+-rw-rw-rw-   0        0        0     1556 2023-08-08 18:01:12.000000 soagen-0.5.0/src/soagen/hpp/emplacer.hpp
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.735073 soagen-0.5.0/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9858 2023-08-08 18:51:46.000000 soagen-0.5.0/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     3859 2023-08-08 18:51:47.000000 soagen-0.5.0/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    43134 2023-08-08 18:51:49.000000 soagen-0.5.0/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      420 2023-08-08 16:35:14.000000 soagen-0.5.0/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      868 2023-08-05 10:16:57.000000 soagen-0.5.0/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0      985 2023-08-08 09:00:27.000000 soagen-0.5.0/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0     3250 2023-08-06 09:18:47.000000 soagen-0.5.0/src/soagen/hpp/invoke.hpp
+-rw-rw-rw-   0        0        0    13240 2023-08-08 18:01:22.000000 soagen-0.5.0/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0     5481 2023-08-06 09:45:57.000000 soagen-0.5.0/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0    12274 2023-08-08 18:01:17.000000 soagen-0.5.0/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.736071 soagen-0.5.0/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   245690 2023-08-08 18:51:49.000000 soagen-0.5.0/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    70025 2023-08-08 16:27:05.000000 soagen-0.5.0/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    34795 2023-08-08 18:30:03.000000 soagen-0.5.0/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     3694 2023-08-08 09:00:27.000000 soagen-0.5.0/src/soagen/hpp/tuples.hpp
+-rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.5.0/src/soagen/includes.py
+-rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.5.0/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/log.py
+-rw-rw-rw-   0        0        0    22555 2023-08-08 15:39:04.000000 soagen-0.5.0/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3529 2023-08-04 15:13:48.000000 soagen-0.5.0/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     6453 2023-08-04 15:13:48.000000 soagen-0.5.0/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     6808 2023-08-05 11:46:44.000000 soagen-0.5.0/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.5.0/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    69964 2023-08-08 17:03:30.000000 soagen-0.5.0/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     1657 2023-08-03 12:36:06.000000 soagen-0.5.0/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3544 2023-08-05 12:31:21.000000 soagen-0.5.0/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.5.0/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-08-08 16:35:14.000000 soagen-0.5.0/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.5.0/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:04:02.720071 soagen-0.5.0/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     2635 2023-08-08 19:04:02.000000 soagen-0.5.0/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1433 2023-08-08 19:04:02.000000 soagen-0.5.0/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 19:04:02.000000 soagen-0.5.0/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-08 19:04:02.000000 soagen-0.5.0/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-08 19:04:02.000000 soagen-0.5.0/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 19:04:02.000000 soagen-0.5.0/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.5.0/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.4.0/CHANGELOG.md` & `soagen-0.5.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v0.5.0
+
+-   Added rows to `soagen::table`
+-   Added iterators to `soagen::table`
+-   Added `soagen::table::for_each_column()`
+
 ## v0.4.0
 
 -   Fixed `soagen::is_table<>`
 -   Added support for emplace-constructing column values by unpacking all `std::tuple`-like types (not just the `emplacer`)
 -   Added support for taking `std::integral_constants` in `for_each_column()`
 -   Added `soagen::same_table_type<>`
 -   Added conversions between `soagen::row<>` specializations
```

### Comparing `soagen-0.4.0/LICENSE.txt` & `soagen-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/PKG-INFO` & `soagen-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.4.0
+Version: 0.5.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,20 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.5.0
+
+-   Added rows to `soagen::table`
+-   Added iterators to `soagen::table`
+-   Added `soagen::table::for_each_column()`
+
 ## v0.4.0
 
 -   Fixed `soagen::is_table<>`
 -   Added support for emplace-constructing column values by unpacking all `std::tuple`-like types (not just the `emplacer`)
 -   Added support for taking `std::integral_constants` in `for_each_column()`
 -   Added `soagen::same_table_type<>`
 -   Added conversions between `soagen::row<>` specializations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.4.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.5.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,22 +13,24 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.4.0 - Fixed `soagen::is_table<>` - Added
-support for emplace-constructing column values by unpacking all `std::tuple`-
-like types (not just the `emplacer`) - Added support for taking `std::
-integral_constants` in `for_each_column()` - Added `soagen::same_table_type<>`
-- Added conversions between `soagen::row<>` specializations - Optimized
-instantiation overhead for most type-traits ## v0.3.0 - Added `hpp.combined` -
-Added `std::integral_constant` to the overload set used by `for_each_column()`
-- Added support for constructing rows from all `std::tuple`-like types -
-Optimized bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
+sponsors/marzer # Changelog ## v0.5.0 - Added rows to `soagen::table` - Added
+iterators to `soagen::table` - Added `soagen::table::for_each_column()` ##
+v0.4.0 - Fixed `soagen::is_table<>` - Added support for emplace-constructing
+column values by unpacking all `std::tuple`-like types (not just the
+`emplacer`) - Added support for taking `std::integral_constants` in
+`for_each_column()` - Added `soagen::same_table_type<>` - Added conversions
+between `soagen::row<>` specializations - Optimized instantiation overhead for
+most type-traits ## v0.3.0 - Added `hpp.combined` - Added `std::
+integral_constant` to the overload set used by `for_each_column()` - Added
+support for constructing rows from all `std::tuple`-like types - Optimized
+bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
 `structs.attributes` - Added `auto` option for `structs.default_constructible`
 - Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
 iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
 Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
 columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
 First public release ð&#xFE0F;
```

### Comparing `soagen-0.4.0/pyproject.toml` & `soagen-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/column.py` & `soagen-0.5.0/src/soagen/column.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/config.py` & `soagen-0.5.0/src/soagen/config.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/configurable.py` & `soagen-0.5.0/src/soagen/configurable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/cpp.py` & `soagen-0.5.0/src/soagen/cpp.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/errors.py` & `soagen-0.5.0/src/soagen/errors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/header_file.py` & `soagen-0.5.0/src/soagen/header_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,17 +129,14 @@
             o('\n\n// __SOAGEN_EXTERNAL_HEADERS\n\n')
 
             # misc preprocessor boilerplate
             o(
                 rf'''
             SOAGEN_PUSH_WARNINGS;
             SOAGEN_DISABLE_SPAM_WARNINGS;
-            #if SOAGEN_CLANG >= 16
-                #pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-            #endif
             #if SOAGEN_MSVC
                 #pragma inline_recursion(on)
             #endif
             #if SOAGEN_MSVC_LIKE
                 #pragma push_macro("min")
                 #pragma push_macro("max")
                 #undef min
@@ -237,18 +234,14 @@
             '''
             )
             with HiddenFromDoxygen(o), ClangFormatOff(o):
                 with Namespace(o, self.config.namespace):
                     for struct in self.structs:
                         struct.write_forward_declarations(o)
                 o()
-                with Namespace(o, 'soagen'):
-                    for struct in self.structs:
-                        struct.write_soagen_specializations(o)
-                o()
                 with Namespace(o, 'soagen::detail'):
                     names = set()
                     for struct in self.structs:
                         for col in struct.columns:
                             names.add(col.name)
                     names = sorted(list(names))
                     for name in names:
```

### Comparing `soagen-0.4.0/src/soagen/hpp/.clang-format` & `soagen-0.5.0/src/soagen/hpp/.clang-format`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/allocator.hpp` & `soagen-0.5.0/src/soagen/hpp/allocator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/column_traits.hpp` & `soagen-0.5.0/src/soagen/hpp/column_traits.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -942,46 +942,65 @@
 		/// @brief	The type used when forwarding #rvalue_type to the backing container (e.g. `table.emplace_back()`)
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		/// @brief	The default type for `emplace()` and `emplace_back()` for columns that have a `default` value.
 		using default_emplace_type = make_cref<rvalue_type>;
 	};
 
-	/// @brief True if `T` is an instance of #soagen::column_traits.
-	template <typename T>
-	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	/// @cond
-	template <typename ValueType, size_t Align, typename ParamType>
-	inline constexpr bool is_column_traits<column_traits<ValueType, Align, ParamType>> = true;
-	template <typename StorageType>
-	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
-	template <typename T>
-	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
-	template <typename T>
-	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
-	template <typename T>
-	inline constexpr bool is_column_traits<const volatile T> = is_column_traits<T>;
+	namespace detail
+	{
+		template <typename>
+		struct is_column_traits_ : std::false_type
+		{};
+		template <typename ValueType, size_t Align, typename ParamType>
+		struct is_column_traits_<column_traits<ValueType, Align, ParamType>> : std::true_type
+		{};
+		template <typename StorageType>
+		struct is_column_traits_<detail::column_traits_base<StorageType>> : std::true_type
+		{};
+	}
 	/// @endcond
+	/// @brief True if `T` is a #soagen::column_traits.
+	template <typename T>
+	inline constexpr bool is_column_traits =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_column_traits_<std::remove_cv_t<T>>::value);
 }
 
 /// @cond
 namespace soagen::detail
 {
 	template <typename T>
 	struct to_base_traits_;
-
 	template <typename ValueType, size_t Align, typename ParamType>
 	struct to_base_traits_<column_traits<ValueType, Align, ParamType>>
 	{
 		using type = column_traits_base<storage_type<ValueType>>;
 
 		static_assert(std::is_base_of_v<type, column_traits<ValueType, Align, ParamType>>);
 	};
-
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
+
+	template <typename T>
+	struct as_column_
+	{
+		using type = column_traits<T>;
+	};
+	template <typename ValueType, size_t Align, typename ParamType>
+	struct as_column_<column_traits<ValueType, Align, ParamType>>
+	{
+		using type = column_traits<ValueType, Align, ParamType>;
+	};
+	template <typename StorageType>
+	struct as_column_<detail::column_traits_base<StorageType>>
+	{
+		using type = detail::column_traits_base<StorageType>;
+	};
+	template <typename T>
+	using as_column = typename as_column_<T>::type;
 }
 /// @endcond
 
 #undef soagen_aligned_storage
 
 #include "header_end.hpp"
```

### Comparing `soagen-0.4.0/src/soagen/hpp/core.hpp` & `soagen-0.5.0/src/soagen/hpp/core.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
 #include <iterator>
+#if SOAGEN_HAS_EXCEPTIONS
+	#include <stdexcept>
+#endif
 
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
 	#if SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
@@ -49,90 +52,95 @@
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
                                                                                                                        \
-		template <typename T, template <typename> typename Transformation = soagen::identity_type>                     \
-		struct named_member_##Name                                                                                     \
+		template <typename T>                                                                                          \
+		struct named_ref_##Name                                                                                        \
 		{                                                                                                              \
-			Transformation<T> Name;                                                                                    \
+			T Name;                                                                                                    \
                                                                                                                        \
 		  protected:                                                                                                   \
 			SOAGEN_PURE_INLINE_GETTER                                                                                  \
-			constexpr decltype(auto) get_named_member() const noexcept                                                 \
+			constexpr decltype(auto) get_ref() const noexcept                                                          \
 			{                                                                                                          \
-				if constexpr (std::is_reference_v<Transformation<T>>)                                                  \
-					return static_cast<Transformation<T>>(Name);                                                       \
+				if constexpr (std::is_reference_v<T>)                                                                  \
+					return static_cast<T>(Name);                                                                       \
 				else                                                                                                   \
 					return Name;                                                                                       \
 			}                                                                                                          \
 		}
 #endif
 
 #ifndef SOAGEN_MAKE_COLUMN
 	#define SOAGEN_MAKE_COLUMN(Table, Column, Name)                                                                    \
 		template <>                                                                                                    \
 		struct column_name<Table, Column> : name_constant_##Name                                                       \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct column_ref<Table&, Column>                                                                              \
-			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
+		struct column_ref<Table, Column>                                                                               \
+			: named_ref_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>    \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct column_ref<Table&&, Column>                                                                             \
-			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
+			: named_ref_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>    \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct column_ref<const Table&, Column>                                                                        \
-			: named_member_##Name<std::add_lvalue_reference_t<                                                         \
+		struct column_ref<const Table, Column>                                                                         \
+			: named_ref_##Name<std::add_lvalue_reference_t<                                                            \
 				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct column_ref<const Table&&, Column>                                                                       \
-			: named_member_##Name<std::add_rvalue_reference_t<                                                         \
+			: named_ref_##Name<std::add_rvalue_reference_t<                                                            \
 				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{}
 #endif
 
 /// @brief The root namespace for the library.
 namespace soagen
 {
 	using std::size_t;
 	using std::ptrdiff_t;
 	using std::intptr_t;
 	using std::uintptr_t;
 	using std::nullptr_t;
 
+	/// @cond
+	// forward declarations
+	template <typename... Args>
+	struct emplacer;
+	template <typename, size_t...>
+	struct row;
+	template <typename Table, size_t... Columns>
+	class iterator;
+	template <typename... Columns>
+	struct table_traits;
+	template <typename Traits, typename Allocator>
+	class table;
+	/// @endcond
+
 	/// @brief	Equivalent to C+20's std::remove_cvref_t.
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
 
 	/// @brief	Transforms `T` &rarr; `const T&`.
 	template <typename T>
 	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
 
 	/// @brief	Makes `T` into `T&` if `T` was not already a reference.
 	template <typename T>
 	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
 
-	/// @brief	The identity type transformation.
-	template <typename T>
-	using identity_type = T;
-
-	/// @brief	The 'identity' base for CRTP scenarios (adds nothing to the interface).
-	template <typename Derived>
-	struct SOAGEN_EMPTY_BASES identity_base
-	{};
-
 	/// @brief	True if `T` is `const` or `volatile` qualified.
 	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	/// @brief	True if `T` is (or is a reference to something that is) `const` or `volatile` qualified.
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
@@ -153,41 +161,116 @@
 	template <typename T, typename... U>
 	inline constexpr bool any_same = (false || ... || std::is_same_v<T, U>);
 
 	/// @brief	True if `Value` is in the list `Values`.
 	template <auto Value, auto... Values>
 	inline constexpr bool any_same_value = ((Value == Values) || ...);
 
-	/// @brief	True if `T` is a soagen-generated SoA table type.
-	template <typename T>
-	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(false); // specialized in generated code
 	/// @cond
+	namespace detail
+	{
+		template <typename>
+		struct is_table_ : std::false_type
+		{};
+		template <typename... Args>
+		struct is_table_<table<Args...>> : std::true_type
+		{};
+	}
+	/// @endcond
+	/// @brief True if `T` is a #soagen::table.
 	template <typename T>
-	inline constexpr bool is_soa<const T> = is_soa<T>;
-	template <typename T>
-	inline constexpr bool is_soa<volatile T> = is_soa<T>;
+	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(detail::is_table_<std::remove_cv_t<T>>::value);
+
+	/// @cond
+	namespace detail
+	{
+		template <typename T>
+		struct is_soa_ : is_table_<T> // specialized in the generated code
+		{};
+	}
+	/// @endcond
+	/// @brief	True if `T` is a #soagen::table or a soagen-generated SoA class.
 	template <typename T>
-	inline constexpr bool is_soa<const volatile T> = is_soa<T>;
+	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(detail::is_soa_<std::remove_cv_t<T>>::value);
 
+	/// @brief	Conditionally adds `const` to a type.
+	template <typename T, bool Cond>
+	using conditionally_add_const = std::conditional_t<Cond, std::add_const_t<T>, T>;
+
+	/// @brief	Conditionally adds `volatile` to a type.
+	template <typename T, bool Cond>
+	using conditionally_add_volatile = std::conditional_t<Cond, std::add_volatile_t<T>, T>;
+
+	/// @cond
 	namespace detail
 	{
 		template <typename T>
 		using is_implicit_lifetime_type_ = std::disjunction<std::is_scalar<T>,
 															std::is_array<T>,
 															std::conjunction<std::is_aggregate<T>,
 																			 std::is_trivially_constructible<T>,
 																			 std::is_trivially_destructible<T>>>;
+
+		template <typename T, typename>
+		struct copy_cvref_
+		{
+			using type = T;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, CopyFrom&>
+		{
+			using type = std::add_lvalue_reference_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, CopyFrom&&>
+		{
+			using type = std::add_rvalue_reference_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, const CopyFrom>
+		{
+			using type = std::add_const_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, volatile CopyFrom>
+		{
+			using type = std::add_volatile_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, const volatile CopyFrom>
+		{
+			using type = std::add_cv_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+
+		template <typename T>
+		struct remove_lvalue_ref_
+		{
+			using type = T;
+		};
+		template <typename T>
+		struct remove_lvalue_ref_<T&>
+		{
+			using type = T;
+		};
 	}
 	/// @endcond
 
 	/// @brief  True if `T` meets the `ImplicitLifetimeType` named requirement.
 	template <typename T>
 	inline constexpr bool is_implicit_lifetime_type =
 		POXY_IMPLEMENTATION_DETAIL(detail::is_implicit_lifetime_type_<T>::value);
 
+	/// @brief  Copies the cvref-qualifiers from one type onto another, replacing the existing ones.
+	template <typename T, typename CopyFrom>
+	using copy_cvref = POXY_IMPLEMENTATION_DETAIL(typename detail::copy_cvref_<remove_cvref<T>, CopyFrom>::type);
+
+	/// @brief	Removes lvalue reference qualifiers. Rvalues references are preserved as-is.
+	template <typename T>
+	using remove_lvalue_ref = POXY_IMPLEMENTATION_DETAIL(typename detail::remove_lvalue_ref_<T>::type);
+
 	/// @brief  Alias for `std::integral_constant<std::size_t, Value>`
 	template <auto Value>
 	using index_constant = std::integral_constant<size_t, static_cast<size_t>(Value)>;
 
 	/// @brief  The type that would result from `std::forward<T>()`.
 	template <typename T>
 	using forward_type = POXY_IMPLEMENTATION_DETAIL(
@@ -456,15 +539,15 @@
 			using type = typename T::table_type;
 		};
 	}
 	/// @endcond
 
 	/// @brief Gets the underlying #soagen::table of an SoA type.
 	template <typename T>
-	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<std::remove_cv_t<T>>::type);
+	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<remove_cvref<T>>::type);
 
 	/// @brief True if two types have the same underlying #soagen::table type.
 	template <typename A, typename B>
 	inline constexpr bool same_table_type =
 		POXY_IMPLEMENTATION_DETAIL(std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>);
 
 	/// @cond
@@ -476,36 +559,35 @@
 			using type = typename T::table_traits;
 		};
 	}
 	/// @endcond
 
 	/// @brief Gets the #soagen::table_traits for the underlying #soagen::table of an SoA type.
 	template <typename T>
-	using table_traits_type =
-		POXY_IMPLEMENTATION_DETAIL(typename detail::table_traits_type_<std::remove_cv_t<T>>::type);
+	using table_traits_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_traits_type_<remove_cvref<T>>::type);
 
 	/// @cond
 	namespace detail
 	{
 		template <typename T>
 		struct allocator_type_
 		{
 			using type = typename T::allocator_type;
 		};
 	}
 	/// @endcond
 
 	/// @brief Gets the allocator being used by the #soagen::table of an SoA type.
 	template <typename T>
-	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<std::remove_cv_t<T>>::type);
+	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<remove_cvref<T>>::type);
 
 	/// @brief Gets the #soagen::column_traits::value_type for the selected column of an SoA type.
 	template <typename T, auto Column>
 	using value_type = POXY_IMPLEMENTATION_DETAIL(
-		typename table_traits_type<T>::template column<static_cast<size_t>(Column)>::value_type);
+		typename table_traits_type<remove_cvref<T>>::template column<static_cast<size_t>(Column)>::value_type);
 
 	/// @cond
 	namespace detail
 	{
 		template <typename ValueType>
 		struct storage_type_
 		{
```

### Comparing `soagen-0.4.0/src/soagen/hpp/emplacer.hpp` & `soagen-0.5.0/src/soagen/hpp/emplacer.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -31,28 +31,28 @@
 	struct emplacer<>
 	{};
 
 	template <typename... Args>
 	emplacer(Args&&...) -> emplacer<Args&&...>;
 	/// @endcond
 
-	/// @brief True if `T` is an instance of #soagen::emplacer.
-	template <typename T>
-	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
-
 	/// @cond
-	template <typename... T>
-	inline constexpr bool is_emplacer<emplacer<T...>> = true;
-	template <typename T>
-	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
+	namespace detail
+	{
+		template <typename>
+		struct is_emplacer_ : std::false_type
+		{};
+		template <typename... Args>
+		struct is_emplacer_<emplacer<Args...>> : std::true_type
+		{};
+	}
 	/// @endcond
+	template <typename T>
+	/// @brief True if `T` is an instance of #soagen::emplacer.
+	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(detail::is_emplacer_<std::remove_cv_t<T>>::value);
 }
 
 /// @cond
 namespace std
 {
 	template <typename... Args>
 	struct tuple_size<soagen::emplacer<Args...>> //
```

### Comparing `soagen-0.4.0/src/soagen/hpp/generated/compressed_pair.hpp` & `soagen-0.5.0/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/generated/functions.hpp` & `soagen-0.5.0/src/soagen/hpp/generated/functions.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/generated/preprocessor.hpp` & `soagen-0.5.0/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -644,14 +644,21 @@
 		#if SOAGEN_CLANG >= 13
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13                                                              \
 				_Pragma("clang diagnostic ignored \"-Wc++20-compat\"")                                                 \
 				static_assert(true)
 		#else
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13 static_assert(true)
 		#endif
+		#if SOAGEN_CLANG >= 16
+			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_16                                                              \
+				_Pragma("clang diagnostic ignored \"-Wunsafe-buffer-usage\"")                                          \
+				static_assert(true)
+		#else
+			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_16 static_assert(true)
+		#endif
 		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
 			_Pragma("clang diagnostic ignored \"-Wc++98-compat-pedantic\"")                                            \
 			_Pragma("clang diagnostic ignored \"-Wc++98-compat\"")                                                     \
 			_Pragma("clang diagnostic ignored \"-Wweak-vtables\"")                                                     \
 			_Pragma("clang diagnostic ignored \"-Wdouble-promotion\"")                                                 \
 			_Pragma("clang diagnostic ignored \"-Wweak-template-vtables\"")                                            \
 			_Pragma("clang diagnostic ignored \"-Wpadded\"")                                                           \
@@ -662,19 +669,20 @@
 			_Pragma("clang diagnostic ignored \"-Wdisabled-macro-expansion\"")                                         \
 			_Pragma("clang diagnostic ignored \"-Wused-but-marked-unused\"")                                           \
 			_Pragma("clang diagnostic ignored \"-Wcovered-switch-default\"")                                           \
 			_Pragma("clang diagnostic ignored \"-Wtautological-pointer-compare\"")                                     \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_8;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_9;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13;                                                                     \
+			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_16;                                                                     \
 			static_assert(true)
 	#elif SOAGEN_MSVC
 		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
-			__pragma(warning(disable : 4127))  /* conditional expr is constant */                                      \
-			__pragma(warning(disable : 4324))  /* structure was padded due to alignment specifier */                   \
+			__pragma(warning(disable : 4127)) /* conditional expr is constant */                                       \
+			__pragma(warning(disable : 4324)) /* structure was padded due to alignment specifier */                    \
 			__pragma(warning(disable : 4348))                                                                          \
 			__pragma(warning(disable : 4464))  /* relative include path contains '..' */                               \
 			__pragma(warning(disable : 4505))  /* unreferenced local function removed */                               \
 			__pragma(warning(disable : 4514))  /* unreferenced inline function has been removed */                     \
 			__pragma(warning(disable : 4582))  /* constructor is not implicitly called */                              \
 			__pragma(warning(disable : 4619))  /* there is no warning number 'XXXX' */                                 \
 			__pragma(warning(disable : 4623))  /* default constructor was implicitly defined as deleted */             \
```

### Comparing `soagen-0.4.0/src/soagen/hpp/header_end.hpp` & `soagen-0.5.0/src/soagen/hpp/header_end.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/header_start.hpp` & `soagen-0.5.0/src/soagen/hpp/header_start.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 #include "generated/preprocessor.hpp"
 
 // __SOAGEN_HEADER_START{{
 
 //# push the current warning state
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
 
 //# disable windows.h min/max macro crimes
 #if SOAGEN_MSVC_LIKE
 	#pragma push_macro("min")
 	#pragma push_macro("max")
 	#undef min
 	#undef max
```

### Comparing `soagen-0.4.0/src/soagen/hpp/invoke.hpp` & `soagen-0.5.0/src/soagen/hpp/invoke.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/iterator.hpp` & `soagen-0.5.0/src/soagen/hpp/iterator.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -23,54 +23,52 @@
 				return &value;
 			}
 		};
 
 		template <typename Table>
 		struct iterator_storage
 		{
-			std::add_const_t<remove_cvref<Table>>* table;
+			remove_cvref<Table>* table;
 			typename remove_cvref<Table>::difference_type offset;
 		};
 	}
 	/// @endcond
 
 	/// @brief		Base class for soagen::iterator.
 	/// @details	Specialize this to add functionality to all iterators of a particular type via CRTP.
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES iterator_base
 	{};
 
-	/// @brief RandomAccessIterator for soagen-generated table types.
+	/// @brief RandomAccessIterator for table types.
 	template <typename Table, size_t... Columns>
 	class SOAGEN_EMPTY_BASES iterator ///
-		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>,
-						   public iterator_base<iterator<Table, Columns...>>)
+		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<soagen::table_type<remove_cvref<Table>>>,
+						   public iterator_base<iterator<remove_lvalue_ref<Table>, Columns...>>)
 	{
-		static_assert(std::is_empty_v<iterator_base<iterator<Table, Columns...>>>,
+		static_assert(std::is_empty_v<iterator_base<iterator<remove_lvalue_ref<Table>, Columns...>>>,
 					  "iterator_base specializations may not have data members");
-		static_assert(std::is_trivial_v<iterator_base<iterator<Table, Columns...>>>,
+		static_assert(std::is_trivial_v<iterator_base<iterator<remove_lvalue_ref<Table>, Columns...>>>,
 					  "iterator_base specializations must be trivial");
 
 	  public:
-		/// @brief Base SoA table type for this iterator.
-		using table_type = remove_cvref<Table>;
-		static_assert(is_soa<table_type>, "soagen iterators are for use with soagen-generated SoA table types.");
+		/// @brief Base soagen::table type for this iterator.
+		using table_type = soagen::table_type<remove_cvref<Table>>;
+		static_assert(is_table<table_type>, "soagen iterators are for use with soagen SoA types.");
 
 		/// @brief Cvref-qualified version of #table_type.
-		using table_ref = Table;
-		static_assert(std::is_reference_v<table_ref>,
-					  "Table must be a reference so row members can derive their reference category");
+		using table_ref = coerce_ref<copy_cvref<table_type, Table>>;
 
 		using size_type = typename table_type::size_type;
 
 		/// @brief Signed integer type returned by difference operations.
 		using difference_type = typename table_type::difference_type;
 
 		/// @brief The row type dereferenced by this iterator.
-		using row_type = row<Table, Columns...>;
+		using row_type = soagen::row_type<remove_lvalue_ref<Table>, Columns...>;
 
 		/// @brief Alias for #row_type.
 		using value_type = row_type;
 
 		/// @brief Alias for #row_type.
 		using reference = row_type;
 
@@ -80,16 +78,15 @@
 #if SOAGEN_CPP <= 17
 		using pointer = void;
 #endif
 
 	  private:
 		/// @cond
 
-		using base		= detail::iterator_storage<remove_cvref<Table>>;
-		using table_ptr = std::add_pointer_t<std::remove_reference_t<Table>>;
+		using base = detail::iterator_storage<soagen::table_type<remove_cvref<Table>>>;
 
 		template <typename, size_t...>
 		friend class soagen::iterator;
 
 		SOAGEN_NODISCARD_CTOR
 		constexpr iterator(base b) noexcept //
 			: base{ b }
@@ -101,15 +98,15 @@
 		/// @brief Default constructor.
 		SOAGEN_NODISCARD_CTOR
 		constexpr iterator() noexcept = default;
 
 		/// @brief Constructs an iterator to some part of a table.
 		SOAGEN_NODISCARD_CTOR
 		constexpr iterator(table_ref tbl, difference_type pos) noexcept //
-			: base{ &tbl, pos }
+			: base{ const_cast<table_type*>(&tbl), pos }
 		{}
 
 		/// @name Incrementing
 		/// @{
 
 		/// @brief Increments the iterator by one row (pre-fix).
 		friend constexpr iterator& operator++(iterator& it) noexcept // pre
@@ -189,23 +186,38 @@
 		}
 
 		/// @}
 
 		/// @name Dereferencing
 		/// @{
 
+	  private:
+		/// @cond
+		template <size_t Column>
+		using cv_value_type =
+			conditionally_add_volatile<conditionally_add_const<soagen::value_type<remove_cvref<Table>, Column>,
+															   std::is_const_v<std::remove_reference_t<Table>>>,
+									   std::is_volatile_v<std::remove_reference_t<Table>>>;
+
+		template <size_t Column>
+		using cv_value_ref = std::conditional_t<std::is_rvalue_reference_v<Table>,
+												std::add_rvalue_reference_t<cv_value_type<Column>>,
+												std::add_lvalue_reference_t<cv_value_type<Column>>>;
+		/// @endcond
+
+	  public:
 		/// @brief Returns the row the iterator refers to.
 		SOAGEN_PURE_GETTER
 		constexpr reference operator*() const noexcept
 		{
 			SOAGEN_ASSUME(!!base::table);
 			SOAGEN_ASSUME(base::offset >= 0);
 
-			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
-				.template row<Columns...>(static_cast<size_type>(base::offset));
+			return row_type{ { static_cast<cv_value_ref<Columns>>(
+				base::table->template column<Columns>()[base::offset]) }... };
 		}
 
 		/// @brief Returns the row the iterator refers to.
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr detail::arrow_proxy<row_type> operator->() const noexcept
 		{
 			return { *(*this) };
@@ -214,16 +226,16 @@
 		/// @brief Returns the row at some arbitrary offset from the one the iterator refers to.
 		SOAGEN_PURE_GETTER
 		constexpr reference operator[](difference_type offset) const noexcept
 		{
 			SOAGEN_ASSUME(!!base::table);
 			SOAGEN_ASSUME(base::offset + offset >= 0);
 
-			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
-				.template row<Columns...>(static_cast<size_type>(base::offset + offset));
+			return row_type{ { static_cast<cv_value_ref<Columns>>(
+				base::table->template column<Columns>()[base::offset + offset]) }... };
 		}
 
 		/// @}
 
 		/// @name Equality
 		/// @{
 
@@ -300,28 +312,28 @@
 		/// </table>
 		///
 		///	@note	Any of these conversions can also change the columns viewed by the iterator - iterators to a table
 		///			share the same underlying data structure regardless of the columns they are viewing.
 		///
 		/// @attention 	There are no conversions provided which offer the equivalent of a `const_cast`-by-proxy.
 		///				This is by design.
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::implicit_conversion_ok<Table, T>
-									 && !detail::explicit_conversion_ok<Table, T>),
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::implicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>
+									 && !detail::explicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>),
 									typename T,
 									size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr operator iterator<T, Cols...>() const noexcept
 		{
 			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
 		}
 
 		/// @cond
 
-		SOAGEN_CONSTRAINED_TEMPLATE((!detail::implicit_conversion_ok<Table, T>
-									 && detail::explicit_conversion_ok<Table, T>),
+		SOAGEN_CONSTRAINED_TEMPLATE((!detail::implicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>
+									 && detail::explicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>),
 									typename T,
 									size_t... Cols)
 		SOAGEN_PURE_INLINE_GETTER
 		explicit constexpr operator iterator<T, Cols...>() const noexcept
 		{
 			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
 		}
@@ -350,28 +362,14 @@
 	SOAGEN_PURE_INLINE_GETTER
 	constexpr iterator<Table, Columns...> operator+(typename iterator<Table, Columns...>::difference_type n,
 													const iterator<Table, Columns...>& it) noexcept
 	{
 		return it + n;
 	}
 
-	/// @brief True if `T` is an instance of #soagen::iterator.
-	template <typename T>
-	inline constexpr bool is_iterator = POXY_IMPLEMENTATION_DETAIL(false);
-	/// @cond
-	template <typename Table, size_t... Columns>
-	inline constexpr bool is_iterator<iterator<Table, Columns...>> = true;
-	template <typename T>
-	inline constexpr bool is_iterator<const T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_iterator<volatile T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_iterator<const volatile T> = is_row<T>;
-	/// @endcond
-
 	/// @cond
 	namespace detail
 	{
 		template <typename Table, size_t... Columns>
 		struct table_type_<iterator<Table, Columns...>>
 		{
 			using type = remove_cvref<Table>;
@@ -383,23 +381,40 @@
 		};
 
 		template <typename Table, typename IndexSequence>
 		struct iterator_type_;
 		template <typename Table, size_t... Columns>
 		struct iterator_type_<Table, std::index_sequence<Columns...>>
 		{
-			using type = iterator<Table, Columns...>;
+			using type = iterator<remove_lvalue_ref<Table>, Columns...>;
 		};
 		template <typename Table>
 		struct iterator_type_<Table, std::index_sequence<>>
-			: iterator_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
+			: iterator_type_<remove_lvalue_ref<Table>,
+							 std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
 	/// @endcond
 
 	/// @brief		The #soagen::iterator for a given SoA type and (some subset of) its columns.
-	template <typename Table, size_t... Columns>
+	template <typename Table, auto... Columns>
 	using iterator_type = POXY_IMPLEMENTATION_DETAIL(
-		typename detail::iterator_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
+		typename detail::iterator_type_<remove_lvalue_ref<Table>,
+										std::index_sequence<static_cast<size_t>(Columns)...>>::type);
+
+	/// @cond
+	namespace detail
+	{
+		template <typename>
+		struct is_iterator_ : std::false_type
+		{};
+		template <typename Table, size_t... Columns>
+		struct is_iterator_<iterator<Table, Columns...>> : std::true_type
+		{};
+	}
+	/// @endcond
+	/// @brief True if `T` is a #soagen::iterator.
+	template <typename T>
+	inline constexpr bool is_iterator = POXY_IMPLEMENTATION_DETAIL(detail::is_iterator_<std::remove_cv_t<T>>::value);
 }
 
 #include "header_end.hpp"
```

### Comparing `soagen-0.4.0/src/soagen/hpp/mixins.hpp` & `soagen-0.5.0/src/soagen/hpp/mixins.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/row.hpp` & `soagen-0.5.0/src/soagen/hpp/row.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 #include "core.hpp"
 #include "header_start.hpp"
 
 namespace soagen
 {
 	/// @cond
-	template <typename, size_t...>
-	struct row;
-
 	namespace detail
 	{
 		// general rules for allowing implicit conversions:
 		// - losing rvalue (T&& -> T&), (const T&& -> const T&)
 		// - gaining const (T& -> const T&, T&& -> const T&&)
 		// - both
 
@@ -66,93 +63,91 @@
 
 		template <typename From, typename To>
 		inline constexpr bool row_implicit_conversion_ok = false;
 
 		template <typename TableA, size_t... ColumnsA, typename TableB, size_t... ColumnsB>
 		inline constexpr bool row_implicit_conversion_ok<row<TableA, ColumnsA...>, //
 														 row<TableB, ColumnsB...>> =
-			implicit_conversion_ok<TableA, TableB>
+			implicit_conversion_ok<coerce_ref<TableA>, coerce_ref<TableB>>
 			&& column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>>;
 
 		// row explicit conversions:
 
 		template <typename From, typename To>
 		inline constexpr bool row_explicit_conversion_ok = false;
 
 		template <typename TableA, size_t... ColumnsA, typename TableB, size_t... ColumnsB>
 		inline constexpr bool row_explicit_conversion_ok<row<TableA, ColumnsA...>, //
 														 row<TableB, ColumnsB...>> =
-			explicit_conversion_ok<TableA, TableB>
+			explicit_conversion_ok<coerce_ref<TableA>, coerce_ref<TableB>>
 			&& column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>>;
 	}
 	/// @endcond
 
 	/// @brief		Base class for soagen::row.
 	/// @details	Specialize this to add functionality to all rows of a particular type via CRTP.
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES row_base
 	{};
 
 	/// @brief A proxy type for treating (some subset of) an SoA row as if it were a regular AoS struct.
 	template <typename Table, size_t... Columns>
 	struct SOAGEN_EMPTY_BASES row //
-	SOAGEN_HIDDEN_BASE(public detail::column_ref<Table, Columns>..., public row_base<row<Table, Columns...>>)
+	SOAGEN_HIDDEN_BASE(public detail::column_ref<remove_lvalue_ref<Table>, Columns>...,
+					   public row_base<row<remove_lvalue_ref<Table>, Columns...>>)
 	{
-		static_assert(std::is_reference_v<Table>,
-					  "Table must be a reference so row members can derive their reference category");
-		static_assert(std::is_empty_v<row_base<row<Table, Columns...>>>,
+		static_assert(std::is_empty_v<row_base<row<remove_lvalue_ref<Table>, Columns...>>>,
 					  "row_base specializations may not have data members");
-		static_assert(std::is_trivial_v<row_base<row<Table, Columns...>>>, "row_base specializations must be trivial");
+		static_assert(std::is_trivial_v<row_base<row<remove_lvalue_ref<Table>, Columns...>>>,
+					  "row_base specializations must be trivial");
 
 		// columns:
 
 		template <auto Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
-			static_assert(static_cast<size_t>(Column) < table_traits_type<remove_cvref<Table>>::column_count,
+			static_assert(static_cast<size_t>(Column) < table_traits_type<Table>::column_count,
 						  "column index out of range");
 
-			return detail::column_ref<Table, static_cast<size_t>(Column)>::get_named_member();
+			return detail::column_ref<remove_lvalue_ref<Table>, static_cast<size_t>(Column)>::get_ref();
 		}
 
 		// tuple protocol:
 
 		template <auto Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
-			return type_at_index<Member, detail::column_ref<Table, Columns>...>::get_named_member();
+			return type_at_index<Member, detail::column_ref<remove_lvalue_ref<Table>, Columns>...>::get_ref();
 		}
 
 		/// @name Equality
 		/// @availability These operators are only available when all the column types are equality-comparable.
 		/// @{
 
 		/// @brief Returns true if all of the elements in two rows are equal.
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator==(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_equality_comparable)
 		{
 			return ((lhs.template column<Columns>() == rhs.template column<Columns>()) && ...);
 		}
 
 		/// @brief Returns true if not all of the elements in two rows are equal.
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		SOAGEN_ALWAYS_INLINE
 		friend constexpr bool operator!=(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_equality_comparable)
 		{
 			return !(lhs == rhs);
 		}
 
 		/// @}
 
 		/// @name Comparison
@@ -160,15 +155,15 @@
 		/// @{
 
 	  private:
 		/// @cond
 		template <size_t Member, typename T>
 		SOAGEN_NODISCARD
 		static constexpr int row_compare_impl(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			if (lhs.template get<Member>() < rhs.template get<Member>())
 				return -1;
 
 			if (rhs.template get<Member>() < lhs.template get<Member>())
 				return 1;
 
@@ -177,53 +172,49 @@
 			else
 				return row_compare_impl<Member + 1u>(lhs, rhs);
 		}
 		/// @endcond
 
 	  public:
 		/// @brief Returns true if the RHS row is ordered lexicographically less-than the RHS row.
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator<(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) < 0;
 		}
 
 		/// @brief Returns true if the RHS row is ordered lexicographically less-than-or-equal-to the RHS row.
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator<=(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) <= 0;
 		}
 
 		/// @brief Returns true if the RHS row is ordered lexicographically greater-than the RHS row.
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator>(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) > 0;
 		}
 
 		/// @brief Returns true if the RHS row is ordered lexicographically greater-than-or-equal-to the RHS row.
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator>=(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) >= 0;
 		}
 
 		/// @}
 
 		/// @name Conversion
@@ -272,28 +263,14 @@
 		}
 
 		/// @endcond
 
 		/// @}
 	};
 
-	/// @brief True if `T` is an instance of #soagen::row.
-	template <typename T>
-	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(false);
-	/// @cond
-	template <typename Table, size_t... Columns>
-	inline constexpr bool is_row<row<Table, Columns...>> = true;
-	template <typename T>
-	inline constexpr bool is_row<const T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_row<volatile T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_row<const volatile T> = is_row<T>;
-	/// @endcond
-
 	/// @cond
 	namespace detail
 	{
 		template <typename Table, size_t... Columns>
 		struct table_type_<row<Table, Columns...>>
 		{
 			using type = remove_cvref<Table>;
@@ -305,27 +282,44 @@
 		};
 
 		template <typename Table, typename IndexSequence>
 		struct row_type_;
 		template <typename Table, size_t... Columns>
 		struct row_type_<Table, std::index_sequence<Columns...>>
 		{
-			using type = row<Table, Columns...>;
+			using type = row<remove_lvalue_ref<Table>, Columns...>;
 		};
 		template <typename Table>
 		struct row_type_<Table, std::index_sequence<>>
-			: row_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
+			: row_type_<remove_lvalue_ref<Table>,
+						std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
 	/// @endcond
 
 	/// @brief		The #soagen::row for a given SoA type and (some subset of) its columns.
 	template <typename Table, auto... Columns>
 	using row_type = POXY_IMPLEMENTATION_DETAIL(
-		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<static_cast<size_t>(Columns)...>>::type);
+		typename detail::row_type_<remove_lvalue_ref<Table>,
+								   std::index_sequence<static_cast<size_t>(Columns)...>>::type);
+
+	/// @cond
+	namespace detail
+	{
+		template <typename>
+		struct is_row_ : std::false_type
+		{};
+		template <typename Table, size_t... Columns>
+		struct is_row_<row<Table, Columns...>> : std::true_type
+		{};
+	}
+	/// @endcond
+	/// @brief True if `T` is a #soagen::row.
+	template <typename T>
+	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(detail::is_row_<std::remove_cv_t<T>>::value);
 }
 
 /// @cond
 namespace std
 {
 	template <typename Table, size_t... Columns>
 	struct tuple_size<soagen::row<Table, Columns...>> //
```

### Comparing `soagen-0.4.0/src/soagen/hpp/single/soagen.hpp` & `soagen-0.5.0/src/soagen/hpp/single/soagen.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp v0.4.0
+// soagen.hpp v0.5.0
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
@@ -28,17 +28,17 @@
 //----------------------------------------------------------------------------------------------------------------------
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
 //********  generated/version.hpp  *************************************************************************************
 
 #define SOAGEN_VERSION_MAJOR 0
-#define SOAGEN_VERSION_MINOR 4
+#define SOAGEN_VERSION_MINOR 5
 #define SOAGEN_VERSION_PATCH 0
-#define SOAGEN_VERSION_STRING "0.4.0"
+#define SOAGEN_VERSION_STRING "0.5.0"
 
 //********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
@@ -678,14 +678,21 @@
 		#if SOAGEN_CLANG >= 13
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13                                                              \
 				_Pragma("clang diagnostic ignored \"-Wc++20-compat\"")                                                 \
 				static_assert(true)
 		#else
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13 static_assert(true)
 		#endif
+		#if SOAGEN_CLANG >= 16
+			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_16                                                              \
+				_Pragma("clang diagnostic ignored \"-Wunsafe-buffer-usage\"")                                          \
+				static_assert(true)
+		#else
+			#define SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_16 static_assert(true)
+		#endif
 		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
 			_Pragma("clang diagnostic ignored \"-Wc++98-compat-pedantic\"")                                            \
 			_Pragma("clang diagnostic ignored \"-Wc++98-compat\"")                                                     \
 			_Pragma("clang diagnostic ignored \"-Wweak-vtables\"")                                                     \
 			_Pragma("clang diagnostic ignored \"-Wdouble-promotion\"")                                                 \
 			_Pragma("clang diagnostic ignored \"-Wweak-template-vtables\"")                                            \
 			_Pragma("clang diagnostic ignored \"-Wpadded\"")                                                           \
@@ -696,19 +703,20 @@
 			_Pragma("clang diagnostic ignored \"-Wdisabled-macro-expansion\"")                                         \
 			_Pragma("clang diagnostic ignored \"-Wused-but-marked-unused\"")                                           \
 			_Pragma("clang diagnostic ignored \"-Wcovered-switch-default\"")                                           \
 			_Pragma("clang diagnostic ignored \"-Wtautological-pointer-compare\"")                                     \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_8;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_9;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13;                                                                     \
+			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_16;                                                                     \
 			static_assert(true)
 	#elif SOAGEN_MSVC
 		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
-			__pragma(warning(disable : 4127))  /* conditional expr is constant */                                      \
-			__pragma(warning(disable : 4324))  /* structure was padded due to alignment specifier */                   \
+			__pragma(warning(disable : 4127)) /* conditional expr is constant */                                       \
+			__pragma(warning(disable : 4324)) /* structure was padded due to alignment specifier */                    \
 			__pragma(warning(disable : 4348))                                                                          \
 			__pragma(warning(disable : 4464))  /* relative include path contains '..' */                               \
 			__pragma(warning(disable : 4505))  /* unreferenced local function removed */                               \
 			__pragma(warning(disable : 4514))  /* unreferenced inline function has been removed */                     \
 			__pragma(warning(disable : 4582))  /* constructor is not implicitly called */                              \
 			__pragma(warning(disable : 4619))  /* there is no warning number 'XXXX' */                                 \
 			__pragma(warning(disable : 4623))  /* default constructor was implicitly defined as deleted */             \
@@ -1025,14 +1033,17 @@
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
 #include <iterator>
+#if SOAGEN_HAS_EXCEPTIONS
+	#include <stdexcept>
+#endif
 
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
 	#if SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
@@ -1053,17 +1064,14 @@
 	#define SOAGEN_OPTIONAL_TYPE std::optional
 #endif
 
 SOAGEN_ENABLE_WARNINGS;
 
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
-#if SOAGEN_CLANG >= 16
-	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
-#endif
 
 #if SOAGEN_MSVC_LIKE
 	#pragma push_macro("min")
 	#pragma push_macro("max")
 	#undef min
 	#undef max
 #endif
@@ -1084,85 +1092,90 @@
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
                                                                                                                        \
-		template <typename T, template <typename> typename Transformation = soagen::identity_type>                     \
-		struct named_member_##Name                                                                                     \
+		template <typename T>                                                                                          \
+		struct named_ref_##Name                                                                                        \
 		{                                                                                                              \
-			Transformation<T> Name;                                                                                    \
+			T Name;                                                                                                    \
                                                                                                                        \
 		  protected:                                                                                                   \
 			SOAGEN_PURE_INLINE_GETTER                                                                                  \
-			constexpr decltype(auto) get_named_member() const noexcept                                                 \
+			constexpr decltype(auto) get_ref() const noexcept                                                          \
 			{                                                                                                          \
-				if constexpr (std::is_reference_v<Transformation<T>>)                                                  \
-					return static_cast<Transformation<T>>(Name);                                                       \
+				if constexpr (std::is_reference_v<T>)                                                                  \
+					return static_cast<T>(Name);                                                                       \
 				else                                                                                                   \
 					return Name;                                                                                       \
 			}                                                                                                          \
 		}
 #endif
 
 #ifndef SOAGEN_MAKE_COLUMN
 	#define SOAGEN_MAKE_COLUMN(Table, Column, Name)                                                                    \
 		template <>                                                                                                    \
 		struct column_name<Table, Column> : name_constant_##Name                                                       \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct column_ref<Table&, Column>                                                                              \
-			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
+		struct column_ref<Table, Column>                                                                               \
+			: named_ref_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>    \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct column_ref<Table&&, Column>                                                                             \
-			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
+			: named_ref_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>    \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct column_ref<const Table&, Column>                                                                        \
-			: named_member_##Name<std::add_lvalue_reference_t<                                                         \
+		struct column_ref<const Table, Column>                                                                         \
+			: named_ref_##Name<std::add_lvalue_reference_t<                                                            \
 				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct column_ref<const Table&&, Column>                                                                       \
-			: named_member_##Name<std::add_rvalue_reference_t<                                                         \
+			: named_ref_##Name<std::add_rvalue_reference_t<                                                            \
 				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{}
 #endif
 
 namespace soagen
 {
 	using std::size_t;
 	using std::ptrdiff_t;
 	using std::intptr_t;
 	using std::uintptr_t;
 	using std::nullptr_t;
 
+	// forward declarations
+	template <typename... Args>
+	struct emplacer;
+	template <typename, size_t...>
+	struct row;
+	template <typename Table, size_t... Columns>
+	class iterator;
+	template <typename... Columns>
+	struct table_traits;
+	template <typename Traits, typename Allocator>
+	class table;
+
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
 
 	template <typename T>
 	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
 
 	template <typename T>
 	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
 
 	template <typename T>
-	using identity_type = T;
-
-	template <typename Derived>
-	struct SOAGEN_EMPTY_BASES identity_base
-	{};
-
-	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_integer = std::is_integral_v<T> && !std::is_same_v<T, bool>;
@@ -1175,38 +1188,105 @@
 
 	template <typename T, typename... U>
 	inline constexpr bool any_same = (false || ... || std::is_same_v<T, U>);
 
 	template <auto Value, auto... Values>
 	inline constexpr bool any_same_value = ((Value == Values) || ...);
 
-	template <typename T>
-	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(false); // specialized in generated code
+	namespace detail
+	{
+		template <typename>
+		struct is_table_ : std::false_type
+		{};
+		template <typename... Args>
+		struct is_table_<table<Args...>> : std::true_type
+		{};
+	}
 
 	template <typename T>
-	inline constexpr bool is_soa<const T> = is_soa<T>;
-	template <typename T>
-	inline constexpr bool is_soa<volatile T> = is_soa<T>;
+	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(detail::is_table_<std::remove_cv_t<T>>::value);
+
+	namespace detail
+	{
+		template <typename T>
+		struct is_soa_ : is_table_<T> // specialized in the generated code
+		{};
+	}
+
 	template <typename T>
-	inline constexpr bool is_soa<const volatile T> = is_soa<T>;
+	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(detail::is_soa_<std::remove_cv_t<T>>::value);
+
+	template <typename T, bool Cond>
+	using conditionally_add_const = std::conditional_t<Cond, std::add_const_t<T>, T>;
+
+	template <typename T, bool Cond>
+	using conditionally_add_volatile = std::conditional_t<Cond, std::add_volatile_t<T>, T>;
 
 	namespace detail
 	{
 		template <typename T>
 		using is_implicit_lifetime_type_ = std::disjunction<std::is_scalar<T>,
 															std::is_array<T>,
 															std::conjunction<std::is_aggregate<T>,
 																			 std::is_trivially_constructible<T>,
 																			 std::is_trivially_destructible<T>>>;
+
+		template <typename T, typename>
+		struct copy_cvref_
+		{
+			using type = T;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, CopyFrom&>
+		{
+			using type = std::add_lvalue_reference_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, CopyFrom&&>
+		{
+			using type = std::add_rvalue_reference_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, const CopyFrom>
+		{
+			using type = std::add_const_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, volatile CopyFrom>
+		{
+			using type = std::add_volatile_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+		template <typename T, typename CopyFrom>
+		struct copy_cvref_<T, const volatile CopyFrom>
+		{
+			using type = std::add_cv_t<typename copy_cvref_<T, CopyFrom>::type>;
+		};
+
+		template <typename T>
+		struct remove_lvalue_ref_
+		{
+			using type = T;
+		};
+		template <typename T>
+		struct remove_lvalue_ref_<T&>
+		{
+			using type = T;
+		};
 	}
 
 	template <typename T>
 	inline constexpr bool is_implicit_lifetime_type =
 		POXY_IMPLEMENTATION_DETAIL(detail::is_implicit_lifetime_type_<T>::value);
 
+	template <typename T, typename CopyFrom>
+	using copy_cvref = POXY_IMPLEMENTATION_DETAIL(typename detail::copy_cvref_<remove_cvref<T>, CopyFrom>::type);
+
+	template <typename T>
+	using remove_lvalue_ref = POXY_IMPLEMENTATION_DETAIL(typename detail::remove_lvalue_ref_<T>::type);
+
 	template <auto Value>
 	using index_constant = std::integral_constant<size_t, static_cast<size_t>(Value)>;
 
 	template <typename T>
 	using forward_type = POXY_IMPLEMENTATION_DETAIL(
 		std::conditional_t<std::is_lvalue_reference_v<T>, T, std::add_rvalue_reference_t<T>>);
 
@@ -1435,15 +1515,15 @@
 		struct table_type_
 		{
 			using type = typename T::table_type;
 		};
 	}
 
 	template <typename T>
-	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<std::remove_cv_t<T>>::type);
+	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<remove_cvref<T>>::type);
 
 	template <typename A, typename B>
 	inline constexpr bool same_table_type =
 		POXY_IMPLEMENTATION_DETAIL(std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>);
 
 	namespace detail
 	{
@@ -1451,32 +1531,31 @@
 		struct table_traits_type_
 		{
 			using type = typename T::table_traits;
 		};
 	}
 
 	template <typename T>
-	using table_traits_type =
-		POXY_IMPLEMENTATION_DETAIL(typename detail::table_traits_type_<std::remove_cv_t<T>>::type);
+	using table_traits_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_traits_type_<remove_cvref<T>>::type);
 
 	namespace detail
 	{
 		template <typename T>
 		struct allocator_type_
 		{
 			using type = typename T::allocator_type;
 		};
 	}
 
 	template <typename T>
-	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<std::remove_cv_t<T>>::type);
+	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<remove_cvref<T>>::type);
 
 	template <typename T, auto Column>
 	using value_type = POXY_IMPLEMENTATION_DETAIL(
-		typename table_traits_type<T>::template column<static_cast<size_t>(Column)>::value_type);
+		typename table_traits_type<remove_cvref<T>>::template column<static_cast<size_t>(Column)>::value_type);
 
 	namespace detail
 	{
 		template <typename ValueType>
 		struct storage_type_
 		{
 			using type = ValueType;
@@ -1622,17 +1701,14 @@
 	}
 }
 
 //********  row.hpp  ***************************************************************************************************
 
 namespace soagen
 {
-	template <typename, size_t...>
-	struct row;
-
 	namespace detail
 	{
 		// general rules for allowing implicit conversions:
 		// - losing rvalue (T&& -> T&), (const T&& -> const T&)
 		// - gaining const (T& -> const T&, T&& -> const T&&)
 		// - both
 
@@ -1679,139 +1755,133 @@
 		// row implicit conversions:
 		template <typename From, typename To>
 		inline constexpr bool row_implicit_conversion_ok = false;
 
 		template <typename TableA, size_t... ColumnsA, typename TableB, size_t... ColumnsB>
 		inline constexpr bool row_implicit_conversion_ok<row<TableA, ColumnsA...>, //
 														 row<TableB, ColumnsB...>> =
-			implicit_conversion_ok<TableA, TableB>
+			implicit_conversion_ok<coerce_ref<TableA>, coerce_ref<TableB>>
 			&& column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>>;
 
 		// row explicit conversions:
 		template <typename From, typename To>
 		inline constexpr bool row_explicit_conversion_ok = false;
 
 		template <typename TableA, size_t... ColumnsA, typename TableB, size_t... ColumnsB>
 		inline constexpr bool row_explicit_conversion_ok<row<TableA, ColumnsA...>, //
 														 row<TableB, ColumnsB...>> =
-			explicit_conversion_ok<TableA, TableB>
+			explicit_conversion_ok<coerce_ref<TableA>, coerce_ref<TableB>>
 			&& column_conversion_ok<std::index_sequence<ColumnsA...>, std::index_sequence<ColumnsB...>>;
 	}
 
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES row_base
 	{};
 
 	template <typename Table, size_t... Columns>
 	struct SOAGEN_EMPTY_BASES row //
-	SOAGEN_HIDDEN_BASE(public detail::column_ref<Table, Columns>..., public row_base<row<Table, Columns...>>)
+	SOAGEN_HIDDEN_BASE(public detail::column_ref<remove_lvalue_ref<Table>, Columns>...,
+					   public row_base<row<remove_lvalue_ref<Table>, Columns...>>)
 	{
-		static_assert(std::is_reference_v<Table>,
-					  "Table must be a reference so row members can derive their reference category");
-		static_assert(std::is_empty_v<row_base<row<Table, Columns...>>>,
+		static_assert(std::is_empty_v<row_base<row<remove_lvalue_ref<Table>, Columns...>>>,
 					  "row_base specializations may not have data members");
-		static_assert(std::is_trivial_v<row_base<row<Table, Columns...>>>, "row_base specializations must be trivial");
+		static_assert(std::is_trivial_v<row_base<row<remove_lvalue_ref<Table>, Columns...>>>,
+					  "row_base specializations must be trivial");
 
 		// columns:
 		template <auto Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
-			static_assert(static_cast<size_t>(Column) < table_traits_type<remove_cvref<Table>>::column_count,
+			static_assert(static_cast<size_t>(Column) < table_traits_type<Table>::column_count,
 						  "column index out of range");
 
-			return detail::column_ref<Table, static_cast<size_t>(Column)>::get_named_member();
+			return detail::column_ref<remove_lvalue_ref<Table>, static_cast<size_t>(Column)>::get_ref();
 		}
 
 		// tuple protocol:
 		template <auto Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
-			return type_at_index<Member, detail::column_ref<Table, Columns>...>::get_named_member();
+			return type_at_index<Member, detail::column_ref<remove_lvalue_ref<Table>, Columns>...>::get_ref();
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator==(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_equality_comparable)
 		{
 			return ((lhs.template column<Columns>() == rhs.template column<Columns>()) && ...);
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		SOAGEN_ALWAYS_INLINE
 		friend constexpr bool operator!=(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_equality_comparable)
 		{
 			return !(lhs == rhs);
 		}
 
 	  private:
 		template <size_t Member, typename T>
 		SOAGEN_NODISCARD
 		static constexpr int row_compare_impl(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			if (lhs.template get<Member>() < rhs.template get<Member>())
 				return -1;
 
 			if (rhs.template get<Member>() < lhs.template get<Member>())
 				return 1;
 
 			if constexpr (Member + 1u == sizeof...(Columns))
 				return 0;
 			else
 				return row_compare_impl<Member + 1u>(lhs, rhs);
 		}
 
 	  public:
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator<(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) < 0;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator<=(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) <= 0;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator>(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) > 0;
 		}
 
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>
-									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T> && table_traits_type<Table>::all_less_than_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator>=(const row& lhs, const row<T, Columns...>& rhs) //
-			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+			noexcept(table_traits_type<Table>::all_nothrow_less_than_comparable)
 		{
 			return row_compare_impl<0>(lhs, rhs) >= 0;
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE((detail::row_implicit_conversion_ok<row, row<T, Cols...>>
 									 && !detail::row_explicit_conversion_ok<row, row<T, Cols...>>),
 									typename T,
@@ -1831,26 +1901,14 @@
 		explicit constexpr operator row<T, Cols...>() const noexcept
 		{
 			return row<T, Cols...>{ { static_cast<decltype(std::declval<row<T, Cols...>>().template column<Cols>())>(
 				this->template column<Cols>()) }... };
 		}
 	};
 
-	template <typename T>
-	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(false);
-
-	template <typename Table, size_t... Columns>
-	inline constexpr bool is_row<row<Table, Columns...>> = true;
-	template <typename T>
-	inline constexpr bool is_row<const T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_row<volatile T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_row<const volatile T> = is_row<T>;
-
 	namespace detail
 	{
 		template <typename Table, size_t... Columns>
 		struct table_type_<row<Table, Columns...>>
 		{
 			using type = remove_cvref<Table>;
 		};
@@ -1861,25 +1919,40 @@
 		};
 
 		template <typename Table, typename IndexSequence>
 		struct row_type_;
 		template <typename Table, size_t... Columns>
 		struct row_type_<Table, std::index_sequence<Columns...>>
 		{
-			using type = row<Table, Columns...>;
+			using type = row<remove_lvalue_ref<Table>, Columns...>;
 		};
 		template <typename Table>
 		struct row_type_<Table, std::index_sequence<>>
-			: row_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
+			: row_type_<remove_lvalue_ref<Table>,
+						std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
 
 	template <typename Table, auto... Columns>
 	using row_type = POXY_IMPLEMENTATION_DETAIL(
-		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<static_cast<size_t>(Columns)...>>::type);
+		typename detail::row_type_<remove_lvalue_ref<Table>,
+								   std::index_sequence<static_cast<size_t>(Columns)...>>::type);
+
+	namespace detail
+	{
+		template <typename>
+		struct is_row_ : std::false_type
+		{};
+		template <typename Table, size_t... Columns>
+		struct is_row_<row<Table, Columns...>> : std::true_type
+		{};
+	}
+
+	template <typename T>
+	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(detail::is_row_<std::remove_cv_t<T>>::value);
 }
 
 namespace std
 {
 	template <typename Table, size_t... Columns>
 	struct tuple_size<soagen::row<Table, Columns...>> //
 		: std::integral_constant<size_t, sizeof...(Columns)>
@@ -2548,25 +2621,27 @@
 	template <>
 	struct emplacer<>
 	{};
 
 	template <typename... Args>
 	emplacer(Args&&...) -> emplacer<Args&&...>;
 
-	template <typename T>
-	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
+	namespace detail
+	{
+		template <typename>
+		struct is_emplacer_ : std::false_type
+		{};
+		template <typename... Args>
+		struct is_emplacer_<emplacer<Args...>> : std::true_type
+		{};
+	}
 
-	template <typename... T>
-	inline constexpr bool is_emplacer<emplacer<T...>> = true;
-	template <typename T>
-	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
-	template <typename T>
-	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
 	template <typename T>
-	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
+
+	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(detail::is_emplacer_<std::remove_cv_t<T>>::value);
 }
 
 namespace std
 {
 	template <typename... Args>
 	struct tuple_size<soagen::emplacer<Args...>> //
 		: std::integral_constant<size_t, sizeof...(Args)>
@@ -2616,15 +2691,15 @@
 	{
 		if constexpr (detail::has_tuple_get_member_<T&&>::value)
 		{
 			return static_cast<T&&>(tuple).template get<I>();
 		}
 		else if constexpr (detail::has_tuple_get_adl_<T&&>::value)
 		{
-			using std::get;
+			using detail::adl_dummy::get;
 			return get<I>(static_cast<T&&>(tuple));
 		}
 	}
 
 	namespace detail
 	{
 		template <typename...>
@@ -3568,44 +3643,63 @@
 		static_assert(base_traits::template is_constructible<rvalue_type>);
 
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		using default_emplace_type = make_cref<rvalue_type>;
 	};
 
-	template <typename T>
-	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
+	namespace detail
+	{
+		template <typename>
+		struct is_column_traits_ : std::false_type
+		{};
+		template <typename ValueType, size_t Align, typename ParamType>
+		struct is_column_traits_<column_traits<ValueType, Align, ParamType>> : std::true_type
+		{};
+		template <typename StorageType>
+		struct is_column_traits_<detail::column_traits_base<StorageType>> : std::true_type
+		{};
+	}
 
-	template <typename ValueType, size_t Align, typename ParamType>
-	inline constexpr bool is_column_traits<column_traits<ValueType, Align, ParamType>> = true;
-	template <typename StorageType>
-	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
-	template <typename T>
-	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
-	template <typename T>
-	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
 	template <typename T>
-	inline constexpr bool is_column_traits<const volatile T> = is_column_traits<T>;
+	inline constexpr bool is_column_traits =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_column_traits_<std::remove_cv_t<T>>::value);
 }
 
 namespace soagen::detail
 {
 	template <typename T>
 	struct to_base_traits_;
-
 	template <typename ValueType, size_t Align, typename ParamType>
 	struct to_base_traits_<column_traits<ValueType, Align, ParamType>>
 	{
 		using type = column_traits_base<storage_type<ValueType>>;
 
 		static_assert(std::is_base_of_v<type, column_traits<ValueType, Align, ParamType>>);
 	};
-
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
+
+	template <typename T>
+	struct as_column_
+	{
+		using type = column_traits<T>;
+	};
+	template <typename ValueType, size_t Align, typename ParamType>
+	struct as_column_<column_traits<ValueType, Align, ParamType>>
+	{
+		using type = column_traits<ValueType, Align, ParamType>;
+	};
+	template <typename StorageType>
+	struct as_column_<detail::column_traits_base<StorageType>>
+	{
+		using type = detail::column_traits_base<StorageType>;
+	};
+	template <typename T>
+	using as_column = typename as_column_<T>::type;
 }
 
 #undef soagen_aligned_storage
 
 //********  invoke.hpp  ************************************************************************************************
 
 namespace soagen
@@ -3690,14 +3784,16 @@
 	// (to minimize template instantiation explosion)
 	template <typename...>
 	struct table_traits_base;
 
 	template <size_t... I, typename... Columns>
 	struct table_traits_base<std::index_sequence<I...>, Columns...>
 	{
+		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
+
 		static_assert(std::is_same_v<std::index_sequence<I...>, std::make_index_sequence<sizeof...(Columns)>>,
 					  "index sequence must match columns");
 
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
@@ -4423,30 +4519,32 @@
 			noexcept(all_nothrow_swappable)
 		{
 			(column<I>::swap(lhs[I], lhs_index, rhs[I], rhs_index), ...);
 		}
 
 		//--- swap columns ---------------------------------------------------------------------------------------------
 
-		template <size_t A, size_t B>
+		template <auto A, auto B>
 		static constexpr bool can_swap_columns =
-			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
+			static_cast<size_t>(A) == static_cast<size_t>(B)
+			|| (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
 
-		template <size_t A, size_t B>
+		template <auto A, auto B>
 		static constexpr bool can_nothrow_swap_columns =
-			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_nothrow_swappable);
+			static_cast<size_t>(A) == static_cast<size_t>(B)
+			|| (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_nothrow_swappable);
 
-		SOAGEN_HIDDEN_CONSTRAINT((can_swap_columns<A, B>), size_t A, size_t B)
+		SOAGEN_HIDDEN_CONSTRAINT((can_swap_columns<A, B>), auto A, auto B)
 		SOAGEN_CPP20_CONSTEXPR
 		static void swap_columns([[maybe_unused]] column_pointers& columns,
 								 [[maybe_unused]] size_t start,
 								 [[maybe_unused]] size_t count) //
 			noexcept(can_nothrow_swap_columns<A, B>)
 		{
-			if constexpr (A != B)
+			if constexpr (static_cast<size_t>(A) != static_cast<size_t>(B))
 			{
 				static_assert(std::is_same_v<storage_type<A>, storage_type<B>>);
 				static_assert(column<A>::is_swappable);
 				static_assert(column<B>::is_swappable);
 
 				column<A>::swap(columns[A], start, columns[B], start, count);
 			}
@@ -4499,14 +4597,16 @@
 	template <typename...>
 	struct table_traits_base_specialized;
 
 	template <size_t... I, typename... Columns>
 	struct table_traits_base_specialized<std::index_sequence<I...>, Columns...> //
 		: public table_traits_base<std::index_sequence<I...>, to_base_traits<Columns>...>
 	{
+		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
+
 		template <typename Func, bool Const = false>
 		static constexpr bool for_each_column_invocable =
 			(is_invocable_with_optional_index<I,
 											  Func,
 											  std::conditional_t<Const,
 																 std::add_const_t<typename Columns::value_type>,
 																 typename Columns::value_type>*>
@@ -4523,103 +4623,417 @@
 	};
 }
 
 namespace soagen
 {
 	template <typename... Columns>
 	struct SOAGEN_EMPTY_BASES table_traits //
-		SOAGEN_HIDDEN_BASE(
-			public detail::table_traits_base_specialized<std::make_index_sequence<sizeof...(Columns)>, Columns...>)
+		SOAGEN_HIDDEN_BASE(public detail::table_traits_base_specialized<std::make_index_sequence<sizeof...(Columns)>,
+																		detail::as_column<Columns>...>)
 	{
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
-		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
-		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, Columns::aligned_stride...);
+		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, detail::as_column<Columns>::aligned_stride...);
 
 		// columns
 		// (note that these hide the base class typedefs - this is intentional)
 
 		template <auto Index>
-		using column = type_at_index<static_cast<size_t>(Index), Columns...>;
+		using column = type_at_index<static_cast<size_t>(Index), detail::as_column<Columns>...>;
 
 		template <typename IndexConstant>
-		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), Columns...>;
+		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), detail::as_column<Columns>...>;
 
-		static constexpr size_t column_alignments[column_count] = { Columns::alignment... };
+		static constexpr size_t column_alignments[column_count] = { detail::as_column<Columns>::alignment... };
 
-		static constexpr size_t largest_alignment = max(size_t{ 1 }, Columns::alignment...);
+		static constexpr size_t largest_alignment = max(size_t{ 1 }, detail::as_column<Columns>::alignment...);
 
-		static constexpr bool rvalue_type_list_is_distinct = POXY_IMPLEMENTATION_DETAIL(
-			!(std::is_same_v<typename Columns::param_type, typename Columns::rvalue_type> && ...));
+		static constexpr bool rvalue_type_list_is_distinct =
+			POXY_IMPLEMENTATION_DETAIL(!(std::is_same_v<typename detail::as_column<Columns>::param_type,
+														typename detail::as_column<Columns>::rvalue_type>
+										 && ...));
 
 		template <typename BackingTable, typename... Args>
 		static constexpr bool emplace_back_is_nothrow =
 			noexcept(std::declval<BackingTable>().emplace_back(std::declval<Args>()...));
 
 		template <typename BackingTable>
 		static constexpr bool push_back_is_nothrow =
-			emplace_back_is_nothrow<BackingTable, typename Columns::param_forward_type...>;
+			emplace_back_is_nothrow<BackingTable, typename detail::as_column<Columns>::param_forward_type...>;
 
 		template <typename BackingTable>
 		static constexpr bool rvalue_push_back_is_nothrow =
-			emplace_back_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
+			emplace_back_is_nothrow<BackingTable, typename detail::as_column<Columns>::rvalue_forward_type...>;
 
 		template <typename BackingTable, typename Row>
 		static constexpr bool row_push_back_is_nothrow = emplace_back_is_nothrow<BackingTable, Row>;
 
 		template <typename BackingTable, typename... Args>
 		static constexpr bool emplace_is_nothrow =
 			noexcept(std::declval<BackingTable>().emplace(typename remove_cvref<BackingTable>::size_type{},
 														  std::declval<Args>()...));
 
 		template <typename BackingTable>
 		static constexpr bool insert_is_nothrow =
-			emplace_is_nothrow<BackingTable, typename Columns::param_forward_type...>;
+			emplace_is_nothrow<BackingTable, typename detail::as_column<Columns>::param_forward_type...>;
 
 		template <typename BackingTable>
 		static constexpr bool rvalue_insert_is_nothrow =
-			emplace_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
+			emplace_is_nothrow<BackingTable, typename detail::as_column<Columns>::rvalue_forward_type...>;
 
 		template <typename BackingTable, typename Row>
 		static constexpr bool row_insert_is_nothrow = emplace_is_nothrow<BackingTable, Row>;
 	};
 
-	template <typename T>
-	inline constexpr bool is_table_traits = POXY_IMPLEMENTATION_DETAIL(false);
+	namespace detail
+	{
+		template <typename>
+		struct is_table_traits_ : std::false_type
+		{};
+		template <typename... Columns>
+		struct is_table_traits_<table_traits<Columns...>> : std::true_type
+		{};
+		template <typename... Columns>
+		struct is_table_traits_<detail::table_traits_base<Columns...>> : std::true_type
+		{};
+	}
 
-	template <typename... Columns>
-	inline constexpr bool is_table_traits<table_traits<Columns...>> = true;
-	template <typename... Columns>
-	inline constexpr bool is_table_traits<detail::table_traits_base<Columns...>> = true;
-	template <typename T>
-	inline constexpr bool is_table_traits<const T> = is_table_traits<T>;
 	template <typename T>
-	inline constexpr bool is_table_traits<volatile T> = is_table_traits<T>;
-	template <typename T>
-	inline constexpr bool is_table_traits<const volatile T> = is_table_traits<T>;
+	inline constexpr bool is_table_traits =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_table_traits_<std::remove_cv_t<T>>::value);
 }
 
 namespace soagen::detail
 {
 	template <typename... Columns>
 	struct to_base_traits_<table_traits<Columns...>>
 	{
-		using type = table_traits_base<to_base_traits<Columns>...>;
+		using type = table_traits_base<to_base_traits<as_column<Columns>>...>;
 
 		static_assert(std::is_base_of_v<type, table_traits<Columns...>>);
 	};
 
 	template <typename... Columns>
 	struct table_traits_type_<table_traits<Columns...>>
 	{
 		using type = table_traits<Columns...>;
 	};
 }
 
+//********  iterator.hpp  **********************************************************************************************
+
+namespace soagen
+{
+	namespace detail
+	{
+		template <typename T>
+		struct arrow_proxy
+		{
+			mutable T value;
+
+			SOAGEN_PURE_INLINE_GETTER
+			constexpr T* operator->() const noexcept
+			{
+				return &value;
+			}
+		};
+
+		template <typename Table>
+		struct iterator_storage
+		{
+			remove_cvref<Table>* table;
+			typename remove_cvref<Table>::difference_type offset;
+		};
+	}
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES iterator_base
+	{};
+
+	template <typename Table, size_t... Columns>
+	class SOAGEN_EMPTY_BASES iterator
+		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<soagen::table_type<remove_cvref<Table>>>,
+						   public iterator_base<iterator<remove_lvalue_ref<Table>, Columns...>>)
+	{
+		static_assert(std::is_empty_v<iterator_base<iterator<remove_lvalue_ref<Table>, Columns...>>>,
+					  "iterator_base specializations may not have data members");
+		static_assert(std::is_trivial_v<iterator_base<iterator<remove_lvalue_ref<Table>, Columns...>>>,
+					  "iterator_base specializations must be trivial");
+
+	  public:
+		using table_type = soagen::table_type<remove_cvref<Table>>;
+		static_assert(is_table<table_type>, "soagen iterators are for use with soagen SoA types.");
+
+		using table_ref = coerce_ref<copy_cvref<table_type, Table>>;
+
+		using size_type = typename table_type::size_type;
+
+		using difference_type = typename table_type::difference_type;
+
+		using row_type = soagen::row_type<remove_lvalue_ref<Table>, Columns...>;
+
+		using value_type = row_type;
+
+		using reference = row_type;
+
+		using iterator_category = std::random_access_iterator_tag;
+
+#if SOAGEN_CPP <= 17
+		using pointer = void;
+#endif
+
+	  private:
+		using base = detail::iterator_storage<soagen::table_type<remove_cvref<Table>>>;
+
+		template <typename, size_t...>
+		friend class soagen::iterator;
+
+		SOAGEN_NODISCARD_CTOR
+		constexpr iterator(base b) noexcept //
+			: base{ b }
+		{}
+
+	  public:
+		SOAGEN_NODISCARD_CTOR
+		constexpr iterator() noexcept = default;
+
+		SOAGEN_NODISCARD_CTOR
+		constexpr iterator(table_ref tbl, difference_type pos) noexcept //
+			: base{ const_cast<table_type*>(&tbl), pos }
+		{}
+
+		friend constexpr iterator& operator++(iterator& it) noexcept // pre
+		{
+			++it.offset;
+			return it;
+		}
+
+		friend constexpr iterator operator++(iterator& it, int) noexcept // post
+		{
+			iterator pre = it;
+			++it.offset;
+			return pre;
+		}
+
+		friend constexpr iterator& operator+=(iterator& it, difference_type n) noexcept
+		{
+			it.offset += n;
+			return it;
+		}
+
+		SOAGEN_PURE_GETTER
+		friend constexpr iterator operator+(const iterator& it, difference_type n) noexcept
+		{
+			auto it2 = it;
+			it2 += n;
+			return it2;
+		}
+
+		friend constexpr iterator& operator--(iterator& it) noexcept // pre
+		{
+			--it.offset;
+			return it;
+		}
+
+		friend constexpr iterator operator--(iterator& it, int) noexcept // post
+		{
+			iterator pre = it;
+			--it.offset;
+			return pre;
+		}
+
+		friend constexpr iterator& operator-=(iterator& it, difference_type n) noexcept
+		{
+			return it += (-n);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		friend constexpr iterator operator-(const iterator& it, difference_type n) noexcept
+		{
+			return it + (-n);
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_GETTER
+		constexpr difference_type operator-(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset - rhs.offset;
+		}
+
+	  private:
+		template <size_t Column>
+		using cv_value_type =
+			conditionally_add_volatile<conditionally_add_const<soagen::value_type<remove_cvref<Table>, Column>,
+															   std::is_const_v<std::remove_reference_t<Table>>>,
+									   std::is_volatile_v<std::remove_reference_t<Table>>>;
+
+		template <size_t Column>
+		using cv_value_ref = std::conditional_t<std::is_rvalue_reference_v<Table>,
+												std::add_rvalue_reference_t<cv_value_type<Column>>,
+												std::add_lvalue_reference_t<cv_value_type<Column>>>;
+
+	  public:
+		SOAGEN_PURE_GETTER
+		constexpr reference operator*() const noexcept
+		{
+			SOAGEN_ASSUME(!!base::table);
+			SOAGEN_ASSUME(base::offset >= 0);
+
+			return row_type{ { static_cast<cv_value_ref<Columns>>(
+				base::table->template column<Columns>()[base::offset]) }... };
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr detail::arrow_proxy<row_type> operator->() const noexcept
+		{
+			return { *(*this) };
+		}
+
+		SOAGEN_PURE_GETTER
+		constexpr reference operator[](difference_type offset) const noexcept
+		{
+			SOAGEN_ASSUME(!!base::table);
+			SOAGEN_ASSUME(base::offset + offset >= 0);
+
+			return row_type{ { static_cast<cv_value_ref<Columns>>(
+				base::table->template column<Columns>()[base::offset + offset]) }... };
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_GETTER
+		constexpr bool operator==(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::table == rhs.table && base::offset == rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		friend constexpr bool operator!=(const iterator& lhs, const iterator<T, Cols...>& rhs) noexcept
+		{
+			return !(lhs == rhs);
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator<(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset < rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator<=(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset <= rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator>(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset > rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator>=(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset >= rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::implicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>
+									 && !detail::explicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>),
+									typename T,
+									size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr operator iterator<T, Cols...>() const noexcept
+		{
+			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((!detail::implicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>
+									 && detail::explicit_conversion_ok<coerce_ref<Table>, coerce_ref<T>>),
+									typename T,
+									size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator iterator<T, Cols...>() const noexcept
+		{
+			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator difference_type() const noexcept
+		{
+			return base::offset;
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator size_type() const noexcept
+		{
+			SOAGEN_ASSUME(base::offset >= 0);
+
+			return static_cast<size_type>(base::offset);
+		}
+	};
+
+	template <typename Table, size_t... Columns>
+	SOAGEN_PURE_INLINE_GETTER
+	constexpr iterator<Table, Columns...> operator+(typename iterator<Table, Columns...>::difference_type n,
+													const iterator<Table, Columns...>& it) noexcept
+	{
+		return it + n;
+	}
+
+	namespace detail
+	{
+		template <typename Table, size_t... Columns>
+		struct table_type_<iterator<Table, Columns...>>
+		{
+			using type = remove_cvref<Table>;
+		};
+		template <typename Table, size_t... Columns>
+		struct table_traits_type_<iterator<Table, Columns...>>
+		{
+			using type = table_traits_type<remove_cvref<Table>>;
+		};
+
+		template <typename Table, typename IndexSequence>
+		struct iterator_type_;
+		template <typename Table, size_t... Columns>
+		struct iterator_type_<Table, std::index_sequence<Columns...>>
+		{
+			using type = iterator<remove_lvalue_ref<Table>, Columns...>;
+		};
+		template <typename Table>
+		struct iterator_type_<Table, std::index_sequence<>>
+			: iterator_type_<remove_lvalue_ref<Table>,
+							 std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
+		{};
+	}
+
+	template <typename Table, auto... Columns>
+	using iterator_type = POXY_IMPLEMENTATION_DETAIL(
+		typename detail::iterator_type_<remove_lvalue_ref<Table>,
+										std::index_sequence<static_cast<size_t>(Columns)...>>::type);
+
+	namespace detail
+	{
+		template <typename>
+		struct is_iterator_ : std::false_type
+		{};
+		template <typename Table, size_t... Columns>
+		struct is_iterator_<iterator<Table, Columns...>> : std::true_type
+		{};
+	}
+
+	template <typename T>
+	inline constexpr bool is_iterator = POXY_IMPLEMENTATION_DETAIL(detail::is_iterator_<std::remove_cv_t<T>>::value);
+}
+
 //********  table.hpp  *************************************************************************************************
 
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
 	SOAGEN_NODISCARD
 	constexpr bool add_without_overflowing(T lhs, T rhs, T& result) noexcept
@@ -5402,38 +5816,40 @@
 		template <size_t A, size_t B>
 		static constexpr bool can_nothrow_swap_columns =
 			Traits::template can_nothrow_swap_columns<A, B>
 			|| (std::is_same_v<typename Traits::template storage_type<A>, typename Traits::template storage_type<B>>
 				&& actual_column_alignment<Traits, Allocator, A> == actual_column_alignment<Traits, Allocator, B>);
 
 	  public:
-		template <size_t A, size_t B>
+		template <auto A, auto B>
 		SOAGEN_CPP20_CONSTEXPR
 		void swap_columns() //
-			noexcept(can_nothrow_swap_columns<A, B>)
+			noexcept(can_nothrow_swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>)
 		{
-			static_assert(can_swap_columns<A, B>);
+			static_assert(can_swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>);
 
-			if constexpr (A != B)
+			if constexpr (static_cast<size_t>(A) != static_cast<size_t>(B))
 			{
 				using storage_a = typename Traits::template storage_type<A>;
 				using storage_b = typename Traits::template storage_type<B>;
 				static_assert(std::is_same_v<storage_a, storage_b>);
 
 				// if they have the same base alignment, we can just swap the two pointers
 				// rather than having to do an element-wise swap
-				if constexpr (actual_column_alignment<Traits, Allocator, A>
-							  == actual_column_alignment<Traits, Allocator, B>)
+				if constexpr (actual_column_alignment<Traits, Allocator, static_cast<size_t>(A)>
+							  == actual_column_alignment<Traits, Allocator, static_cast<size_t>(B)>)
 				{
-					std::swap(base::alloc_.columns[A], base::alloc_.columns[B]);
+					std::swap(base::alloc_.columns[static_cast<size_t>(A)],
+							  base::alloc_.columns[static_cast<size_t>(B)]);
 				}
-
 				else
 				{
-					Traits::template swap_columns<A, B>(base::alloc_.columns, {}, base::count_);
+					Traits::template swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>(base::alloc_.columns,
+																								  {},
+																								  base::count_);
 				}
 			}
 		}
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructible column types
@@ -6013,67 +6429,308 @@
 		: public SOAGEN_BASE_TYPE
 	{
 	  public:
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_data_ptr);
 	};
-}
+
+	//------------------------------------------------------------------------------------------------------------------
+	// specialization: functions that require the column indices
+	//------------------------------------------------------------------------------------------------------------------
 
 #undef SOAGEN_BASE_NAME
 #define SOAGEN_BASE_NAME table_data_ptr
+
+	template <typename Traits, typename Allocator, typename>
+	class table_row_and_column_funcs;
+
+	template <typename Traits, typename Allocator, size_t... Columns>
+	class table_row_and_column_funcs<Traits, Allocator, std::index_sequence<Columns...>> //
+		: public SOAGEN_BASE_TYPE
+	{
+		static_assert(std::is_same_v<std::index_sequence<Columns...>, std::make_index_sequence<Traits::column_count>>);
+
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_row_and_column_funcs);
+
+		using size_type		  = std::size_t;
+		using difference_type = std::ptrdiff_t;
+		using allocator_type  = Allocator;
+
+		using table_type   = table<Traits, Allocator>;
+		using table_traits = Traits;
+		template <auto Column>
+		using column_traits = typename table_traits::template column<static_cast<size_t>(Column)>;
+		template <auto Column>
+		using column_type = typename column_traits<static_cast<size_t>(Column)>::value_type;
+
+		using iterator		  = soagen::iterator_type<table_type>;
+		using const_iterator  = soagen::iterator_type<const table_type>;
+		using rvalue_iterator = soagen::iterator_type<table_type&&>;
+
+		using row_type		  = soagen::row_type<table_type>;
+		using const_row_type  = soagen::row_type<const table_type>;
+		using rvalue_row_type = soagen::row_type<table_type&&>;
+
+		template <auto Column>
+		SOAGEN_ALIGNED_COLUMN(Column)
+		constexpr column_type<Column>* column() noexcept
+		{
+			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
+
+			using column	   = column_traits<static_cast<size_t>(Column)>;
+			using storage_type = typename column::storage_type;
+			using value_type   = typename column::value_type;
+
+			SOAGEN_CPP23_STATIC_CONSTEXPR size_t align =
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>;
+
+			if constexpr (std::is_pointer_v<storage_type>)
+			{
+				static_assert(std::is_same_v<storage_type, void*>);
+
+				return soagen::assume_aligned<align>(
+					SOAGEN_LAUNDER(reinterpret_cast<value_type*>(base::alloc_.columns[static_cast<size_t>(Column)])));
+			}
+			else
+			{
+				static_assert(std::is_same_v<storage_type, std::remove_cv_t<value_type>>);
+
+				return soagen::assume_aligned<align>(column::ptr(base::alloc_.columns[static_cast<size_t>(Column)]));
+			}
+		}
+
+		template <auto Column>
+		SOAGEN_ALIGNED_COLUMN(Column)
+		constexpr std::add_const_t<column_type<Column>>* column() const noexcept
+		{
+			return const_cast<table_row_and_column_funcs&>(*this).template column<static_cast<size_t>(Column)>();
+		}
+
+		template <auto... Cols>
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		soagen::row_type<table_type, Cols...> row(size_type index) & noexcept
+		{
+			if constexpr (sizeof...(Cols))
+			{
+				return { { this->template column<static_cast<size_type>(Cols)>()[index] }... };
+			}
+			else
+			{
+				return { { this->template column<static_cast<size_type>(Columns)>()[index] }... };
+			}
+		}
+
+		template <auto... Cols>
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		soagen::row_type<table_type&&, Cols...> row(size_type index) && noexcept
+		{
+			if constexpr (sizeof...(Cols))
+			{
+				return { { std::move(this->template column<static_cast<size_type>(Cols)>()[index]) }... };
+			}
+			else
+			{
+				return { { std::move(this->template column<static_cast<size_type>(Columns)>()[index]) }... };
+			}
+		}
+
+		template <auto... Cols>
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		soagen::row_type<const table_type, Cols...> row(size_type index) const& noexcept
+		{
+			if constexpr (sizeof...(Cols))
+			{
+				return { { this->template column<static_cast<size_type>(Cols)>()[index] }... };
+			}
+			else
+			{
+				return { { this->template column<static_cast<size_type>(Columns)>()[index] }... };
+			}
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type operator[](size_type index) & noexcept
+		{
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type operator[](size_type index) && noexcept
+		{
+			return std::move(*this).row(index);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type operator[](size_type index) const& noexcept
+		{
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type at(size_type index) &
+		{
+#if SOAGEN_HAS_EXCEPTIONS
+			if (index >= base::size())
+				throw std::out_of_range{ "bad element access" };
+#endif
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type at(size_type index) &&
+		{
+#if SOAGEN_HAS_EXCEPTIONS
+			if (index >= base::size())
+				throw std::out_of_range{ "bad element access" };
+#endif
+			return std::move(*this).row(index);
+		}
+
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type at(size_type index) const&
+		{
+#if SOAGEN_HAS_EXCEPTIONS
+			if (index >= base::size())
+				throw std::out_of_range{ "bad element access" };
+#endif
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type front() & noexcept
+		{
+			return (*this).row(0u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type back() & noexcept
+		{
+			return (*this).row(base::size() - 1u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type front() && noexcept
+		{
+			return std::move(*this).row(0u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type back() && noexcept
+		{
+			return std::move(*this).row(base::size() - 1u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type front() const& noexcept
+		{
+			return (*this).row(0u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type back() const& noexcept
+		{
+			return (*this).row(base::size() - 1u);
+		}
+
+		template <typename Func>
+		constexpr void for_each_column(Func&& func) //
+			noexcept(table_traits::template for_each_column_nothrow_invocable<Func&&>)
+		{
+			(invoke_with_optional_index<Columns>(static_cast<Func&&>(func), this->template column<Columns>()), ...);
+		}
+
+		template <typename Func>
+		constexpr void for_each_column(Func&& func) const //
+			noexcept(table_traits::template for_each_column_nothrow_invocable<Func&&, true>)
+		{
+			(invoke_with_optional_index<Columns>(static_cast<Func&&>(func), this->template column<Columns>()), ...);
+		}
+	};
+}
+
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_row_and_column_funcs
 #undef SOAGEN_BASE_TYPE
-#define SOAGEN_BASE_TYPE detail::SOAGEN_BASE_NAME<Traits, Allocator>
+#define SOAGEN_BASE_TYPE                                                                                               \
+	detail::SOAGEN_BASE_NAME<Traits, Allocator, std::make_index_sequence<remove_cvref<Traits>::column_count>>
 
 namespace soagen
 {
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES table_base
 	{};
 
 	template <typename Traits,
-			  typename Allocator				= soagen::allocator,
-			  template <typename> typename Base = soagen::identity_base>
+			  typename Allocator = soagen::allocator>
 	class SOAGEN_EMPTY_BASES table //
-		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE,
-						   public table_base<table<Traits, Allocator, Base>>,
-						   public Base<table<Traits, Allocator, Base>>)
+		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE, public table_base<table<Traits, Allocator>>)
 	{
 		static_assert(is_table_traits<Traits>, "Traits must be an instance of soagen::table_traits");
 		static_assert(!is_cvref<Traits>, "table traits may not be cvref-qualified");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
-		static_assert(!std::is_same_v<table_base<table<Traits, Allocator, Base>>, Base<table<Traits, Allocator, Base>>>,
-					  "table_base and Base may not be the same type");
-
-		static_assert(std::is_empty_v<table_base<table<Traits, Allocator, Base>>>,
+		static_assert(std::is_empty_v<table_base<table<Traits, Allocator>>>,
 					  "table_base specializations may not have data members");
-		static_assert(std::is_trivial_v<table_base<table<Traits, Allocator, Base>>>,
+		static_assert(std::is_trivial_v<table_base<table<Traits, Allocator>>>,
 					  "table_base specializations must be trivial");
 
-		static_assert(std::is_empty_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases may not have data members");
-		static_assert(std::is_trivial_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases must be trivial");
-
 	  private:
 		using base = SOAGEN_BASE_TYPE;
 
 	  public:
-		using size_type		  = size_t;
-		using difference_type = ptrdiff_t;
+		using size_type = std::size_t;
 
-		using table_traits = Traits;
+		using difference_type = std::ptrdiff_t;
 
 		using allocator_type = Allocator;
 
+		using table_traits = Traits;
+
+		static constexpr size_type column_count = table_traits::column_count;
+
 		template <auto Column>
 		using column_traits = typename table_traits::template column<static_cast<size_t>(Column)>;
 
 		template <auto Column>
 		using column_type = typename column_traits<static_cast<size_t>(Column)>::value_type;
 
+		using iterator = soagen::iterator_type<table>;
+
+		using const_iterator = soagen::iterator_type<const table>;
+
+		using rvalue_iterator = soagen::iterator_type<table&&>;
+
+		using row_type = soagen::row_type<table>;
+
+		using const_row_type = soagen::row_type<const table>;
+
+		using rvalue_row_type = soagen::row_type<table&&>;
+
 		static constexpr size_t aligned_stride = Traits::aligned_stride;
 
 		SOAGEN_NODISCARD_CTOR
 		table() = default;
 
 		SOAGEN_NODISCARD_CTOR
 		table(table&&) = default;
@@ -6085,79 +6742,146 @@
 
 		table& operator=(const table&) = default;
 
 		~table() = default;
 
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
-		template <auto Column>
-		SOAGEN_ALIGNED_COLUMN(Column)
-		constexpr column_type<Column>* column() noexcept
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table, Columns...> begin() & noexcept
 		{
-			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
-
-			using column	   = column_traits<static_cast<size_t>(Column)>;
-			using storage_type = typename column::storage_type;
-			using value_type   = typename column::value_type;
+			return { *this, 0 };
+		}
 
-			SOAGEN_CPP23_STATIC_CONSTEXPR size_t align =
-				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>;
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table, Columns...> end() & noexcept
+		{
+			return { *this, static_cast<difference_type>(base::size()) };
+		}
 
-			if constexpr (std::is_pointer_v<storage_type>)
-			{
-				static_assert(std::is_same_v<storage_type, void*>);
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table&&, Columns...> begin() && noexcept
+		{
+			return { static_cast<table&&>(*this), 0 };
+		}
 
-				return soagen::assume_aligned<align>(
-					SOAGEN_LAUNDER(reinterpret_cast<value_type*>(base::alloc_.columns[static_cast<size_t>(Column)])));
-			}
-			else
-			{
-				static_assert(std::is_same_v<storage_type, std::remove_cv_t<value_type>>);
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table&&, Columns...> end() && noexcept
+		{
+			return { static_cast<table&&>(*this), static_cast<difference_type>(base::size()) };
+		}
 
-				return soagen::assume_aligned<align>(column::ptr(base::alloc_.columns[static_cast<size_t>(Column)]));
-			}
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> begin() const& noexcept
+		{
+			return { *this, 0 };
 		}
 
-		template <auto Column>
-		SOAGEN_ALIGNED_COLUMN(Column)
-		constexpr std::add_const_t<column_type<Column>>* column() const noexcept
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> end() const& noexcept
 		{
-			return const_cast<table&>(*this).template column<static_cast<size_t>(Column)>();
+			return { *this, static_cast<difference_type>(base::size()) };
 		}
-	};
 
-	template <typename>
-	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> cbegin() const noexcept
+		{
+			return { *this, 0 };
+		}
 
-	template <typename Traits, typename Allocator, template <typename> typename Base>
-	inline constexpr bool is_table<table<Traits, Allocator, Base>> = true;
-	template <typename T>
-	inline constexpr bool is_table<const T> = is_table<T>;
-	template <typename T>
-	inline constexpr bool is_table<volatile T> = is_table<T>;
-	template <typename T>
-	inline constexpr bool is_table<const volatile T> = is_table<T>;
-	namespace detail
-	{
-		template <typename... Args>
-		struct table_type_<table<Args...>>
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> cend() const noexcept
 		{
-			using type = table<Args...>;
-		};
-	}
+			return { *this, static_cast<difference_type>(base::size()) };
+		}
+	};
 
 	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Args...>>), typename... Args)
 	SOAGEN_ALWAYS_INLINE
 	constexpr void swap(table<Args...>& lhs, table<Args...>& rhs) //
 		noexcept(soagen::has_nothrow_swap_member<table<Args...>>)
 	{
 		lhs.swap(rhs);
 	}
 }
 
+namespace soagen::detail
+{
+	template <typename... Args>
+	struct table_type_<table<Args...>>
+	{
+		using type = table<Args...>;
+	};
+
+	template <typename Traits, typename... Args>
+	struct table_traits_type_<table<Traits, Args...>>
+	{
+		using type = Traits;
+	};
+
+	template <typename Traits, typename Allocator>
+	struct allocator_type_<table<Traits, Allocator>>
+	{
+		using type = Allocator;
+	};
+
+	template <typename T>
+	struct unnamed_ref
+	{
+	  protected:
+		T val_;
+
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr decltype(auto) get_ref() const noexcept
+		{
+			if constexpr (std::is_reference_v<T>)
+				return static_cast<T>(val_);
+			else
+				return val_;
+		}
+
+	  public:
+		template <typename Val>
+		SOAGEN_NODISCARD_CTOR
+		constexpr unnamed_ref(Val&& val) noexcept //
+			: val_{ static_cast<Val&&>(val) }
+		{}
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(unnamed_ref);
+	};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<table<Args...>, Column>
+		: unnamed_ref<std::add_lvalue_reference_t<soagen::value_type<table<Args...>, Column>>>
+	{};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<table<Args...>&&, Column>
+		: unnamed_ref<std::add_rvalue_reference_t<soagen::value_type<table<Args...>, Column>>>
+	{};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<const table<Args...>, Column>
+		: unnamed_ref<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<table<Args...>, Column>>>>
+	{};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<const table<Args...>&&, Column>
+		: unnamed_ref<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<table<Args...>, Column>>>>
+	{};
+}
+
 #undef SOAGEN_BASE_NAME
 #undef SOAGEN_BASE_TYPE
 
 //********  mixins.hpp  ************************************************************************************************
 
 namespace soagen::mixins
 {
@@ -6316,311 +7040,14 @@
 	};
 
 	template <typename Derived>
 	struct SOAGEN_EMPTY_BASES const_data_ptr<Derived, false>
 	{};
 }
 
-//********  iterator.hpp  **********************************************************************************************
-
-namespace soagen
-{
-	namespace detail
-	{
-		template <typename T>
-		struct arrow_proxy
-		{
-			mutable T value;
-
-			SOAGEN_PURE_INLINE_GETTER
-			constexpr T* operator->() const noexcept
-			{
-				return &value;
-			}
-		};
-
-		template <typename Table>
-		struct iterator_storage
-		{
-			std::add_const_t<remove_cvref<Table>>* table;
-			typename remove_cvref<Table>::difference_type offset;
-		};
-	}
-
-	template <typename Derived>
-	struct SOAGEN_EMPTY_BASES iterator_base
-	{};
-
-	template <typename Table, size_t... Columns>
-	class SOAGEN_EMPTY_BASES iterator
-		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>,
-						   public iterator_base<iterator<Table, Columns...>>)
-	{
-		static_assert(std::is_empty_v<iterator_base<iterator<Table, Columns...>>>,
-					  "iterator_base specializations may not have data members");
-		static_assert(std::is_trivial_v<iterator_base<iterator<Table, Columns...>>>,
-					  "iterator_base specializations must be trivial");
-
-	  public:
-		using table_type = remove_cvref<Table>;
-		static_assert(is_soa<table_type>, "soagen iterators are for use with soagen-generated SoA table types.");
-
-		using table_ref = Table;
-		static_assert(std::is_reference_v<table_ref>,
-					  "Table must be a reference so row members can derive their reference category");
-
-		using size_type = typename table_type::size_type;
-
-		using difference_type = typename table_type::difference_type;
-
-		using row_type = row<Table, Columns...>;
-
-		using value_type = row_type;
-
-		using reference = row_type;
-
-		using iterator_category = std::random_access_iterator_tag;
-
-#if SOAGEN_CPP <= 17
-		using pointer = void;
-#endif
-
-	  private:
-		using base		= detail::iterator_storage<remove_cvref<Table>>;
-		using table_ptr = std::add_pointer_t<std::remove_reference_t<Table>>;
-
-		template <typename, size_t...>
-		friend class soagen::iterator;
-
-		SOAGEN_NODISCARD_CTOR
-		constexpr iterator(base b) noexcept //
-			: base{ b }
-		{}
-
-	  public:
-		SOAGEN_NODISCARD_CTOR
-		constexpr iterator() noexcept = default;
-
-		SOAGEN_NODISCARD_CTOR
-		constexpr iterator(table_ref tbl, difference_type pos) noexcept //
-			: base{ &tbl, pos }
-		{}
-
-		friend constexpr iterator& operator++(iterator& it) noexcept // pre
-		{
-			++it.offset;
-			return it;
-		}
-
-		friend constexpr iterator operator++(iterator& it, int) noexcept // post
-		{
-			iterator pre = it;
-			++it.offset;
-			return pre;
-		}
-
-		friend constexpr iterator& operator+=(iterator& it, difference_type n) noexcept
-		{
-			it.offset += n;
-			return it;
-		}
-
-		SOAGEN_PURE_GETTER
-		friend constexpr iterator operator+(const iterator& it, difference_type n) noexcept
-		{
-			auto it2 = it;
-			it2 += n;
-			return it2;
-		}
-
-		friend constexpr iterator& operator--(iterator& it) noexcept // pre
-		{
-			--it.offset;
-			return it;
-		}
-
-		friend constexpr iterator operator--(iterator& it, int) noexcept // post
-		{
-			iterator pre = it;
-			--it.offset;
-			return pre;
-		}
-
-		friend constexpr iterator& operator-=(iterator& it, difference_type n) noexcept
-		{
-			return it += (-n);
-		}
-
-		SOAGEN_PURE_INLINE_GETTER
-		friend constexpr iterator operator-(const iterator& it, difference_type n) noexcept
-		{
-			return it + (-n);
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_GETTER
-		constexpr difference_type operator-(const iterator<T, Cols...>& rhs) const noexcept
-		{
-			return base::offset - rhs.offset;
-		}
-
-		SOAGEN_PURE_GETTER
-		constexpr reference operator*() const noexcept
-		{
-			SOAGEN_ASSUME(!!base::table);
-			SOAGEN_ASSUME(base::offset >= 0);
-
-			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
-				.template row<Columns...>(static_cast<size_type>(base::offset));
-		}
-
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr detail::arrow_proxy<row_type> operator->() const noexcept
-		{
-			return { *(*this) };
-		}
-
-		SOAGEN_PURE_GETTER
-		constexpr reference operator[](difference_type offset) const noexcept
-		{
-			SOAGEN_ASSUME(!!base::table);
-			SOAGEN_ASSUME(base::offset + offset >= 0);
-
-			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
-				.template row<Columns...>(static_cast<size_type>(base::offset + offset));
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_GETTER
-		constexpr bool operator==(const iterator<T, Cols...>& rhs) const noexcept
-		{
-			return base::table == rhs.table && base::offset == rhs.offset;
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		friend constexpr bool operator!=(const iterator& lhs, const iterator<T, Cols...>& rhs) noexcept
-		{
-			return !(lhs == rhs);
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr bool operator<(const iterator<T, Cols...>& rhs) const noexcept
-		{
-			return base::offset < rhs.offset;
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr bool operator<=(const iterator<T, Cols...>& rhs) const noexcept
-		{
-			return base::offset <= rhs.offset;
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr bool operator>(const iterator<T, Cols...>& rhs) const noexcept
-		{
-			return base::offset > rhs.offset;
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((same_table_type<Table, T>), typename T, size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr bool operator>=(const iterator<T, Cols...>& rhs) const noexcept
-		{
-			return base::offset >= rhs.offset;
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((detail::implicit_conversion_ok<Table, T>
-									 && !detail::explicit_conversion_ok<Table, T>),
-									typename T,
-									size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr operator iterator<T, Cols...>() const noexcept
-		{
-			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
-		}
-
-		SOAGEN_CONSTRAINED_TEMPLATE((!detail::implicit_conversion_ok<Table, T>
-									 && detail::explicit_conversion_ok<Table, T>),
-									typename T,
-									size_t... Cols)
-		SOAGEN_PURE_INLINE_GETTER
-		explicit constexpr operator iterator<T, Cols...>() const noexcept
-		{
-			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
-		}
-
-		SOAGEN_PURE_INLINE_GETTER
-		explicit constexpr operator difference_type() const noexcept
-		{
-			return base::offset;
-		}
-
-		SOAGEN_PURE_INLINE_GETTER
-		explicit constexpr operator size_type() const noexcept
-		{
-			SOAGEN_ASSUME(base::offset >= 0);
-
-			return static_cast<size_type>(base::offset);
-		}
-	};
-
-	template <typename Table, size_t... Columns>
-	SOAGEN_PURE_INLINE_GETTER
-	constexpr iterator<Table, Columns...> operator+(typename iterator<Table, Columns...>::difference_type n,
-													const iterator<Table, Columns...>& it) noexcept
-	{
-		return it + n;
-	}
-
-	template <typename T>
-	inline constexpr bool is_iterator = POXY_IMPLEMENTATION_DETAIL(false);
-
-	template <typename Table, size_t... Columns>
-	inline constexpr bool is_iterator<iterator<Table, Columns...>> = true;
-	template <typename T>
-	inline constexpr bool is_iterator<const T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_iterator<volatile T> = is_row<T>;
-	template <typename T>
-	inline constexpr bool is_iterator<const volatile T> = is_row<T>;
-
-	namespace detail
-	{
-		template <typename Table, size_t... Columns>
-		struct table_type_<iterator<Table, Columns...>>
-		{
-			using type = remove_cvref<Table>;
-		};
-		template <typename Table, size_t... Columns>
-		struct table_traits_type_<iterator<Table, Columns...>>
-		{
-			using type = table_traits_type<remove_cvref<Table>>;
-		};
-
-		template <typename Table, typename IndexSequence>
-		struct iterator_type_;
-		template <typename Table, size_t... Columns>
-		struct iterator_type_<Table, std::index_sequence<Columns...>>
-		{
-			using type = iterator<Table, Columns...>;
-		};
-		template <typename Table>
-		struct iterator_type_<Table, std::index_sequence<>>
-			: iterator_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
-		{};
-	}
-
-	template <typename Table, size_t... Columns>
-	using iterator_type = POXY_IMPLEMENTATION_DETAIL(
-		typename detail::iterator_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
-}
-
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
 		#pragma inline_recursion(off)
 	#elif SOAGEN_GCC
```

### Comparing `soagen-0.4.0/src/soagen/hpp/soagen.hpp` & `soagen-0.5.0/src/soagen/hpp/soagen.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/hpp/table.hpp` & `soagen-0.5.0/src/soagen/hpp/table.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
 #include "generated/compressed_pair.hpp"
 #include "allocator.hpp"
 #include "table_traits.hpp"
+#include "row.hpp"
+#include "iterator.hpp"
 #include "header_start.hpp"
 
 /// @cond
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
 	SOAGEN_NODISCARD
@@ -794,38 +796,40 @@
 		template <size_t A, size_t B>
 		static constexpr bool can_nothrow_swap_columns =
 			Traits::template can_nothrow_swap_columns<A, B>
 			|| (std::is_same_v<typename Traits::template storage_type<A>, typename Traits::template storage_type<B>>
 				&& actual_column_alignment<Traits, Allocator, A> == actual_column_alignment<Traits, Allocator, B>);
 
 	  public:
-		template <size_t A, size_t B>
+		template <auto A, auto B>
 		SOAGEN_CPP20_CONSTEXPR
 		void swap_columns() //
-			noexcept(can_nothrow_swap_columns<A, B>)
+			noexcept(can_nothrow_swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>)
 		{
-			static_assert(can_swap_columns<A, B>);
+			static_assert(can_swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>);
 
-			if constexpr (A != B)
+			if constexpr (static_cast<size_t>(A) != static_cast<size_t>(B))
 			{
 				using storage_a = typename Traits::template storage_type<A>;
 				using storage_b = typename Traits::template storage_type<B>;
 				static_assert(std::is_same_v<storage_a, storage_b>);
 
 				// if they have the same base alignment, we can just swap the two pointers
 				// rather than having to do an element-wise swap
-				if constexpr (actual_column_alignment<Traits, Allocator, A>
-							  == actual_column_alignment<Traits, Allocator, B>)
+				if constexpr (actual_column_alignment<Traits, Allocator, static_cast<size_t>(A)>
+							  == actual_column_alignment<Traits, Allocator, static_cast<size_t>(B)>)
 				{
-					std::swap(base::alloc_.columns[A], base::alloc_.columns[B]);
+					std::swap(base::alloc_.columns[static_cast<size_t>(A)],
+							  base::alloc_.columns[static_cast<size_t>(B)]);
 				}
-
 				else
 				{
-					Traits::template swap_columns<A, B>(base::alloc_.columns, {}, base::count_);
+					Traits::template swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>(base::alloc_.columns,
+																								  {},
+																								  base::count_);
 				}
 			}
 		}
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructible column types
@@ -1405,20 +1409,256 @@
 		: public SOAGEN_BASE_TYPE
 	{
 	  public:
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_data_ptr);
 	};
-}
+
+	//------------------------------------------------------------------------------------------------------------------
+	// specialization: functions that require the column indices
+	//------------------------------------------------------------------------------------------------------------------
 
 #undef SOAGEN_BASE_NAME
 #define SOAGEN_BASE_NAME table_data_ptr
+
+	template <typename Traits, typename Allocator, typename>
+	class table_row_and_column_funcs;
+
+	template <typename Traits, typename Allocator, size_t... Columns>
+	class table_row_and_column_funcs<Traits, Allocator, std::index_sequence<Columns...>> //
+		: public SOAGEN_BASE_TYPE
+	{
+		static_assert(std::is_same_v<std::index_sequence<Columns...>, std::make_index_sequence<Traits::column_count>>);
+
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_row_and_column_funcs);
+
+		using size_type		  = std::size_t;
+		using difference_type = std::ptrdiff_t;
+		using allocator_type  = Allocator;
+
+		using table_type   = table<Traits, Allocator>;
+		using table_traits = Traits;
+		template <auto Column>
+		using column_traits = typename table_traits::template column<static_cast<size_t>(Column)>;
+		template <auto Column>
+		using column_type = typename column_traits<static_cast<size_t>(Column)>::value_type;
+
+		using iterator		  = soagen::iterator_type<table_type>;
+		using const_iterator  = soagen::iterator_type<const table_type>;
+		using rvalue_iterator = soagen::iterator_type<table_type&&>;
+
+		using row_type		  = soagen::row_type<table_type>;
+		using const_row_type  = soagen::row_type<const table_type>;
+		using rvalue_row_type = soagen::row_type<table_type&&>;
+
+		template <auto Column>
+		SOAGEN_ALIGNED_COLUMN(Column)
+		constexpr column_type<Column>* column() noexcept
+		{
+			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
+
+			using column	   = column_traits<static_cast<size_t>(Column)>;
+			using storage_type = typename column::storage_type;
+			using value_type   = typename column::value_type;
+
+			SOAGEN_CPP23_STATIC_CONSTEXPR size_t align =
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>;
+
+			if constexpr (std::is_pointer_v<storage_type>)
+			{
+				static_assert(std::is_same_v<storage_type, void*>);
+
+				return soagen::assume_aligned<align>(
+					SOAGEN_LAUNDER(reinterpret_cast<value_type*>(base::alloc_.columns[static_cast<size_t>(Column)])));
+			}
+			else
+			{
+				static_assert(std::is_same_v<storage_type, std::remove_cv_t<value_type>>);
+
+				return soagen::assume_aligned<align>(column::ptr(base::alloc_.columns[static_cast<size_t>(Column)]));
+			}
+		}
+
+		template <auto Column>
+		SOAGEN_ALIGNED_COLUMN(Column)
+		constexpr std::add_const_t<column_type<Column>>* column() const noexcept
+		{
+			return const_cast<table_row_and_column_funcs&>(*this).template column<static_cast<size_t>(Column)>();
+		}
+
+		template <auto... Cols>
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		soagen::row_type<table_type, Cols...> row(size_type index) & noexcept
+		{
+			if constexpr (sizeof...(Cols))
+			{
+				return { { this->template column<static_cast<size_type>(Cols)>()[index] }... };
+			}
+			else
+			{
+				return { { this->template column<static_cast<size_type>(Columns)>()[index] }... };
+			}
+		}
+
+		template <auto... Cols>
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		soagen::row_type<table_type&&, Cols...> row(size_type index) && noexcept
+		{
+			if constexpr (sizeof...(Cols))
+			{
+				return { { std::move(this->template column<static_cast<size_type>(Cols)>()[index]) }... };
+			}
+			else
+			{
+				return { { std::move(this->template column<static_cast<size_type>(Columns)>()[index]) }... };
+			}
+		}
+
+		template <auto... Cols>
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		soagen::row_type<const table_type, Cols...> row(size_type index) const& noexcept
+		{
+			if constexpr (sizeof...(Cols))
+			{
+				return { { this->template column<static_cast<size_type>(Cols)>()[index] }... };
+			}
+			else
+			{
+				return { { this->template column<static_cast<size_type>(Columns)>()[index] }... };
+			}
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type operator[](size_type index) & noexcept
+		{
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type operator[](size_type index) && noexcept
+		{
+			return std::move(*this).row(index);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type operator[](size_type index) const& noexcept
+		{
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type at(size_type index) &
+		{
+#if SOAGEN_HAS_EXCEPTIONS
+			if (index >= base::size())
+				throw std::out_of_range{ "bad element access" };
+#endif
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type at(size_type index) &&
+		{
+#if SOAGEN_HAS_EXCEPTIONS
+			if (index >= base::size())
+				throw std::out_of_range{ "bad element access" };
+#endif
+			return std::move(*this).row(index);
+		}
+
+		SOAGEN_PURE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type at(size_type index) const&
+		{
+#if SOAGEN_HAS_EXCEPTIONS
+			if (index >= base::size())
+				throw std::out_of_range{ "bad element access" };
+#endif
+			return (*this).row(index);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type front() & noexcept
+		{
+			return (*this).row(0u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		row_type back() & noexcept
+		{
+			return (*this).row(base::size() - 1u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type front() && noexcept
+		{
+			return std::move(*this).row(0u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		rvalue_row_type back() && noexcept
+		{
+			return std::move(*this).row(base::size() - 1u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type front() const& noexcept
+		{
+			return (*this).row(0u);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		SOAGEN_CPP20_CONSTEXPR
+		const_row_type back() const& noexcept
+		{
+			return (*this).row(base::size() - 1u);
+		}
+
+		template <typename Func>
+		constexpr void for_each_column(Func&& func) //
+			noexcept(table_traits::template for_each_column_nothrow_invocable<Func&&>)
+		{
+			(invoke_with_optional_index<Columns>(static_cast<Func&&>(func), this->template column<Columns>()), ...);
+		}
+
+		template <typename Func>
+		constexpr void for_each_column(Func&& func) const //
+			noexcept(table_traits::template for_each_column_nothrow_invocable<Func&&, true>)
+		{
+			(invoke_with_optional_index<Columns>(static_cast<Func&&>(func), this->template column<Columns>()), ...);
+		}
+	};
+
+}
+
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_row_and_column_funcs
 #undef SOAGEN_BASE_TYPE
-#define SOAGEN_BASE_TYPE detail::SOAGEN_BASE_NAME<Traits, Allocator>
+#define SOAGEN_BASE_TYPE                                                                                               \
+	detail::SOAGEN_BASE_NAME<Traits, Allocator, std::make_index_sequence<remove_cvref<Traits>::column_count>>
 
 /// @endcond
 
 namespace soagen
 {
 	/// @brief		Base class for soagen::table.
 	/// @details	Specialize this to add functionality to all tables of a particular type via CRTP.
@@ -1426,65 +1666,79 @@
 	struct SOAGEN_EMPTY_BASES table_base
 	{};
 
 	/// @brief		A table.
 	/// @details	Effectively a multi-column std::vector.
 	/// @tparam		Traits		The #soagen::table_traits for the table.
 	/// @tparam		Allocator	The allocator used by the table.
-	/// @tparam		Base		Base class hook allowing you to add more functionality to the table via CRTP.
 	///
 	///	@attention	This class is the backing data structure for the soagen-generated Structure-of-arrays classes.
 	///				You don't need to know anything about it unless you are implementing your own SoA machinery
 	///				without using the soagen generator.
 	template <typename Traits,
-			  typename Allocator				= soagen::allocator,
-			  template <typename> typename Base = soagen::identity_base>
+			  typename Allocator = soagen::allocator>
 	class SOAGEN_EMPTY_BASES table //
-		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE,
-						   public table_base<table<Traits, Allocator, Base>>,
-						   public Base<table<Traits, Allocator, Base>>)
+		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE, public table_base<table<Traits, Allocator>>)
 	{
 		static_assert(is_table_traits<Traits>, "Traits must be an instance of soagen::table_traits");
 		static_assert(!is_cvref<Traits>, "table traits may not be cvref-qualified");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
-		static_assert(!std::is_same_v<table_base<table<Traits, Allocator, Base>>, Base<table<Traits, Allocator, Base>>>,
-					  "table_base and Base may not be the same type");
-
-		static_assert(std::is_empty_v<table_base<table<Traits, Allocator, Base>>>,
+		static_assert(std::is_empty_v<table_base<table<Traits, Allocator>>>,
 					  "table_base specializations may not have data members");
-		static_assert(std::is_trivial_v<table_base<table<Traits, Allocator, Base>>>,
+		static_assert(std::is_trivial_v<table_base<table<Traits, Allocator>>>,
 					  "table_base specializations must be trivial");
 
-		static_assert(std::is_empty_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases may not have data members");
-		static_assert(std::is_trivial_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases must be trivial");
-
 	  private:
 		/// @cond
 		using base = SOAGEN_BASE_TYPE;
 		/// @endcond
 
 	  public:
-		using size_type		  = size_t;
-		using difference_type = ptrdiff_t;
+		/// @brief The unsigned integer size type used by tables.
+		using size_type = std::size_t;
 
-		/// @brief	The #soagen::table_traits for the the table.
-		using table_traits = Traits;
+		/// @brief The signed integer difference type used by tables.
+		using difference_type = std::ptrdiff_t;
 
 		/// @brief	The allocator used by the table.
 		using allocator_type = Allocator;
 
+		/// @brief	The #soagen::table_traits for the the table.
+		using table_traits = Traits;
+
+		/// @brief The number of columns in the table.
+		static constexpr size_type column_count = table_traits::column_count;
+
 		/// @brief	Returns the #soagen::column_traits for the column at the specified index.
 		template <auto Column>
 		using column_traits = typename table_traits::template column<static_cast<size_t>(Column)>;
 
 		/// @brief	Returns the `value_type` for the column at the specified index.
 		template <auto Column>
 		using column_type = typename column_traits<static_cast<size_t>(Column)>::value_type;
 
+		/// @brief Row iterators returned by iterator functions.
+		using iterator = soagen::iterator_type<table>;
+
+		/// @brief Row iterators returned by const-qualified iterator functions.
+		using const_iterator = soagen::iterator_type<const table>;
+
+		/// @brief Row iterators returned by rvalue-qualified iterator functions.
+		using rvalue_iterator = soagen::iterator_type<table&&>;
+
+		/// @brief Regular (lvalue-qualified) row type used by tables.
+		using row_type = soagen::row_type<table>;
+
+		/// @brief Const row type used by tables.
+		using const_row_type = soagen::row_type<const table>;
+
+		/// @brief Rvalue row type used by tables.
+		using rvalue_row_type = soagen::row_type<table&&>;
+
 		/// @copydoc	table_traits::aligned_stride
 		static constexpr size_t aligned_stride = Traits::aligned_stride;
 
 		/// @brief Default constructor.
 		SOAGEN_NODISCARD_CTOR
 		table() = default;
 
@@ -1564,35 +1818,46 @@
 		/// you can use the return value to update your data accordingly.
 		///
 		/// @returns	The index of the row that was moved into the erased row's position, if any.
 		///
 		/// @availability This method is only available when all the column types are move-assignable.
 		soagen::optional<size_type> unordered_erase(size_type pos) noexcept(...);
 
-		/// @brief Constructs a new row in-place at the end of the table.
-		template <typename... Args>
-		void emplace_back(Args&&... args) noexcept(...);
-
-		/// @brief Constructs a new row in-place at an arbitrary position in the table.
-		template <typename... Args>
-		void emplace(size_type index, Args&&... args) noexcept(...);
-
 		/// @brief Removes the last row(s) from the table.
 		void pop_back(size_type num = 1) noexcept(...);
 
 		/// @brief Resizes the table to the given number of rows.
 		///
 		/// @availability This method is only available when all the column types are default-constructible.
 		void resize(size_type new_size) noexcept(...);
 
 		/// @brief Swaps the contents of the table with another.
 		///
 		/// @availability This method is only available when #allocator_type is swappable or non-propagating.
 		constexpr void swap(table& other) noexcept(...);
 
+		/// @brief Swaps two columns.
+		///
+		/// @availability The two columns must have the same underlying value_type.
+		template <auto A, auto B>
+		void swap_columns() noexcept(...);
+
+		/// @}
+
+		/// @name Adding rows
+		/// @{
+
+		/// @brief Constructs a new row in-place at the end of the table.
+		template <typename... Args>
+		void emplace_back(Args&&... args) noexcept(...);
+
+		/// @brief Constructs a new row in-place at an arbitrary position in the table.
+		template <typename... Args>
+		void emplace(size_type index, Args&&... args) noexcept(...);
+
 		/// @}
 
 		/// @name Equality
 		/// @availability These operators are only available when all the column types are equality-comparable.
 		/// @{
 
 		/// @brief Returns true if all of the elements in two tables are equal.
@@ -1620,101 +1885,280 @@
 		friend constexpr bool operator>=(const table& lhs, const table& rhs) noexcept(...);
 
 		/// @}
 
 		/// @brief Returns the allocator being used by the table.
 		constexpr allocator_type get_allocator() const noexcept;
 
-#endif
-
 		/// @name Column access
 		/// @{
 
-#if SOAGEN_DOXYGEN
 		/// @brief Returns a pointer to the raw byte backing array.
 		///
 		/// @availability This method is only available when all the column types are trivially-copyable.
 		constexpr std::byte* data() noexcept;
 
 		/// @brief Returns a const pointer to the raw byte backing array.
 		///
 		/// @availability This method is only available when all the column types are trivially-copyable.
 		constexpr const std::byte* data() const noexcept;
-#endif
 
 		/// @brief Returns a pointer to the elements of a specific column.
 		template <auto Column>
-		SOAGEN_ALIGNED_COLUMN(Column)
-		constexpr column_type<Column>* column() noexcept
+		constexpr column_type<Column>* column() noexcept;
+
+		/// @brief Returns a pointer to the elements of a specific column.
+		template <auto Column>
+		constexpr std::add_const_t<column_type<Column>>* column() const noexcept;
+
+		/// @brief Invokes a function once for each column data pointer.
+		///
+		/// @tparam Func A callable type compatible with one of the following signatures:<ul>
+		/// <li> `void(auto*, std::integral_constant<size_type, N>)`
+		/// <li> `void(auto*, size_type)`
+		/// <li> `void(std::integral_constant<size_type, N>, auto*)`
+		/// <li> `void(size_type, auto*)`
+		/// <li> `void(auto*)`
+		/// </ul>
+		/// Overload resolution is performed in the order listed above.
+		///
+		/// @param func The callable to invoke.
+		template <typename Func>
+		constexpr void for_each_column(Func&& func) noexcept(...);
+
+		/// @brief Invokes a function once for each column data pointer (const overload).
+		///
+		/// @tparam Func A callable type compatible with one of the following signatures:<ul>
+		/// <li> `void(auto*, std::integral_constant<size_type, N>)`
+		/// <li> `void(auto*, size_type)`
+		/// <li> `void(std::integral_constant<size_type, N>, auto*)`
+		/// <li> `void(size_type, auto*)`
+		/// <li> `void(auto*)`
+		/// </ul>
+		/// Overload resolution is performed in the order listed above.
+		///
+		/// @param func The callable to invoke.
+		template <typename Func>
+		constexpr void for_each_column(Func&& func) const noexcept(...);
+
+		/// @}
+
+		/// @name Row access
+		/// @{
+
+		/// @brief Returns the row at the given index.
+		///
+		/// @tparam Columns Indices of the columns to include in the row. Leave the list empty for all columns.
+		template <auto... Columns>
+		soagen::row_type<boxes, Columns...> row(size_type index) & noexcept;
+
+		/// @brief Returns the row at the given index.
+		row_type operator[](size_type index) & noexcept;
+
+		/// @brief Returns the row at the given index.
+		///
+		/// @throws std::out_of_range
+		row_type at(size_type index) &;
+
+		/// @brief Returns the very first row in the table.
+		row_type front() & noexcept;
+
+		/// @brief Returns the very last row in the table.
+		row_type back() & noexcept;
+
+		/// @brief Returns the row at the given index.
+		///
+		/// @tparam Columns Indices of the columns to include in the row. Leave the list empty for all columns.
+		template <auto... Columns>
+		soagen::row_type<boxes&&, Columns...> row(size_type index) && noexcept;
+
+		/// @brief Returns the row at the given index.
+		rvalue_row_type operator[](size_type index) && noexcept;
+
+		/// @brief Returns the row at the given index.
+		///
+		/// @throws std::out_of_range
+		rvalue_row_type at(size_type index) &&;
+
+		/// @brief Returns the very first row in the table.
+		rvalue_row_type front() && noexcept;
+
+		/// @brief Returns the very last row in the table.
+		rvalue_row_type back() && noexcept;
+
+		/// @brief Returns the row at the given index.
+		///
+		/// @tparam Columns Indices of the columns to include in the row. Leave the list empty for all columns.
+		template <auto... Columns>
+		soagen::row_type<const boxes, Columns...> row(size_type index) const& noexcept;
+
+		/// @brief Returns the row at the given index.
+		const_row_type operator[](size_type index) const& noexcept;
+
+		/// @brief Returns the row at the given index.
+		///
+		/// @throws std::out_of_range
+		const_row_type at(size_type index) const&;
+
+		/// @brief Returns the very first row in the table.
+		const_row_type front() const& noexcept;
+
+		/// @brief Returns the very last row in the table.
+		const_row_type back() const& noexcept;
+
+		/// @}
+
+#endif
+
+		/// @name Iterators
+		/// @{
+
+		/// @brief Returns an iterator to the first row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table, Columns...> begin() & noexcept
 		{
-			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
+			return { *this, 0 };
+		}
 
-			using column	   = column_traits<static_cast<size_t>(Column)>;
-			using storage_type = typename column::storage_type;
-			using value_type   = typename column::value_type;
+		/// @brief Returns an iterator to one-past-the-last row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table, Columns...> end() & noexcept
+		{
+			return { *this, static_cast<difference_type>(base::size()) };
+		}
 
-			SOAGEN_CPP23_STATIC_CONSTEXPR size_t align =
-				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>;
+		/// @brief Returns an iterator to the first row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table&&, Columns...> begin() && noexcept
+		{
+			return { static_cast<table&&>(*this), 0 };
+		}
 
-			if constexpr (std::is_pointer_v<storage_type>)
-			{
-				static_assert(std::is_same_v<storage_type, void*>);
+		/// @brief Returns an iterator to one-past-the-last row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<table&&, Columns...> end() && noexcept
+		{
+			return { static_cast<table&&>(*this), static_cast<difference_type>(base::size()) };
+		}
 
-				return soagen::assume_aligned<align>(
-					SOAGEN_LAUNDER(reinterpret_cast<value_type*>(base::alloc_.columns[static_cast<size_t>(Column)])));
-			}
-			else
-			{
-				static_assert(std::is_same_v<storage_type, std::remove_cv_t<value_type>>);
+		/// @brief Returns an iterator to the first row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> begin() const& noexcept
+		{
+			return { *this, 0 };
+		}
 
-				return soagen::assume_aligned<align>(column::ptr(base::alloc_.columns[static_cast<size_t>(Column)]));
-			}
+		/// @brief Returns an iterator to one-past-the-last row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> end() const& noexcept
+		{
+			return { *this, static_cast<difference_type>(base::size()) };
 		}
 
-		/// @brief Returns a pointer to the elements of a specific column.
-		template <auto Column>
-		SOAGEN_ALIGNED_COLUMN(Column)
-		constexpr std::add_const_t<column_type<Column>>* column() const noexcept
+		/// @brief Returns an iterator to the first row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> cbegin() const noexcept
+		{
+			return { *this, 0 };
+		}
+
+		/// @brief Returns an iterator to one-past-the-last row in the table.
+		template <auto... Columns>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr soagen::iterator_type<const table, Columns...> cend() const noexcept
 		{
-			return const_cast<table&>(*this).template column<static_cast<size_t>(Column)>();
+			return { *this, static_cast<difference_type>(base::size()) };
 		}
 
 		/// @}
 	};
 
-	/// @brief True if `T` is an instance of #soagen::table.
-	template <typename>
-	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
-	/// @cond
-	template <typename Traits, typename Allocator, template <typename> typename Base>
-	inline constexpr bool is_table<table<Traits, Allocator, Base>> = true;
-	template <typename T>
-	inline constexpr bool is_table<const T> = is_table<T>;
-	template <typename T>
-	inline constexpr bool is_table<volatile T> = is_table<T>;
-	template <typename T>
-	inline constexpr bool is_table<const volatile T> = is_table<T>;
-	namespace detail
-	{
-		template <typename... Args>
-		struct table_type_<table<Args...>>
-		{
-			using type = table<Args...>;
-		};
-	}
-	/// @endcond
-
 	/// @brief Swaps the contents of two tables.
 	///
 	/// @availability This method is only available when the table's `allocator_type` is swappable or non-propagating.
 	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Args...>>), typename... Args)
 	SOAGEN_ALWAYS_INLINE
 	constexpr void swap(table<Args...>& lhs, table<Args...>& rhs) //
 		noexcept(soagen::has_nothrow_swap_member<table<Args...>>)
 	{
 		lhs.swap(rhs);
 	}
 }
 
+/// @cond
+namespace soagen::detail
+{
+	template <typename... Args>
+	struct table_type_<table<Args...>>
+	{
+		using type = table<Args...>;
+	};
+
+	template <typename Traits, typename... Args>
+	struct table_traits_type_<table<Traits, Args...>>
+	{
+		using type = Traits;
+	};
+
+	template <typename Traits, typename Allocator>
+	struct allocator_type_<table<Traits, Allocator>>
+	{
+		using type = Allocator;
+	};
+
+	template <typename T>
+	struct unnamed_ref
+	{
+	  protected:
+		T val_;
+
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr decltype(auto) get_ref() const noexcept
+		{
+			if constexpr (std::is_reference_v<T>)
+				return static_cast<T>(val_);
+			else
+				return val_;
+		}
+
+	  public:
+		template <typename Val>
+		SOAGEN_NODISCARD_CTOR
+		constexpr unnamed_ref(Val&& val) noexcept //
+			: val_{ static_cast<Val&&>(val) }
+		{}
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(unnamed_ref);
+	};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<table<Args...>, Column>
+		: unnamed_ref<std::add_lvalue_reference_t<soagen::value_type<table<Args...>, Column>>>
+	{};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<table<Args...>&&, Column>
+		: unnamed_ref<std::add_rvalue_reference_t<soagen::value_type<table<Args...>, Column>>>
+	{};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<const table<Args...>, Column>
+		: unnamed_ref<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<table<Args...>, Column>>>>
+	{};
+
+	template <size_t Column, typename... Args>
+	struct column_ref<const table<Args...>&&, Column>
+		: unnamed_ref<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<table<Args...>, Column>>>>
+	{};
+}
+/// @endcond
+
 #undef SOAGEN_BASE_NAME
 #undef SOAGEN_BASE_TYPE
 #include "header_end.hpp"
```

### Comparing `soagen-0.4.0/src/soagen/hpp/table_traits.hpp` & `soagen-0.5.0/src/soagen/hpp/table_traits.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 	// (to minimize template instantiation explosion)
 	template <typename...>
 	struct table_traits_base;
 
 	template <size_t... I, typename... Columns>
 	struct table_traits_base<std::index_sequence<I...>, Columns...>
 	{
+		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
+
 		static_assert(std::is_same_v<std::index_sequence<I...>, std::make_index_sequence<sizeof...(Columns)>>,
 					  "index sequence must match columns");
 
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
@@ -750,30 +752,32 @@
 			noexcept(all_nothrow_swappable)
 		{
 			(column<I>::swap(lhs[I], lhs_index, rhs[I], rhs_index), ...);
 		}
 
 		//--- swap columns ---------------------------------------------------------------------------------------------
 
-		template <size_t A, size_t B>
+		template <auto A, auto B>
 		static constexpr bool can_swap_columns =
-			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
+			static_cast<size_t>(A) == static_cast<size_t>(B)
+			|| (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
 
-		template <size_t A, size_t B>
+		template <auto A, auto B>
 		static constexpr bool can_nothrow_swap_columns =
-			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_nothrow_swappable);
+			static_cast<size_t>(A) == static_cast<size_t>(B)
+			|| (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_nothrow_swappable);
 
-		SOAGEN_HIDDEN_CONSTRAINT((can_swap_columns<A, B>), size_t A, size_t B)
+		SOAGEN_HIDDEN_CONSTRAINT((can_swap_columns<A, B>), auto A, auto B)
 		SOAGEN_CPP20_CONSTEXPR
 		static void swap_columns([[maybe_unused]] column_pointers& columns,
 								 [[maybe_unused]] size_t start,
 								 [[maybe_unused]] size_t count) //
 			noexcept(can_nothrow_swap_columns<A, B>)
 		{
-			if constexpr (A != B)
+			if constexpr (static_cast<size_t>(A) != static_cast<size_t>(B))
 			{
 				static_assert(std::is_same_v<storage_type<A>, storage_type<B>>);
 				static_assert(column<A>::is_swappable);
 				static_assert(column<B>::is_swappable);
 
 				column<A>::swap(columns[A], start, columns[B], start, count);
 			}
@@ -826,14 +830,16 @@
 	template <typename...>
 	struct table_traits_base_specialized;
 
 	template <size_t... I, typename... Columns>
 	struct table_traits_base_specialized<std::index_sequence<I...>, Columns...> //
 		: public table_traits_base<std::index_sequence<I...>, to_base_traits<Columns>...>
 	{
+		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
+
 		template <typename Func, bool Const = false>
 		static constexpr bool for_each_column_invocable =
 			(is_invocable_with_optional_index<I,
 											  Func,
 											  std::conditional_t<Const,
 																 std::add_const_t<typename Columns::value_type>,
 																 typename Columns::value_type>*>
@@ -850,79 +856,76 @@
 	};
 }
 /// @endcond
 
 namespace soagen
 {
 	/// @brief	Traits for a table.
-	/// @tparam	Columns		The #soagen::column_traits for the columns of the table.
-	///
-	///	@attention	This class is an implementation detail for the soagen-generated Structure-of-arrays classes.
-	///				You don't need to know anything about it unless you are implementing your own SoA machinery
-	///				without using the soagen generator.
+	/// @tparam	Columns		The types and/or #soagen::column_traits for the columns of the table.
 	template <typename... Columns>
 	struct SOAGEN_EMPTY_BASES table_traits //
-		SOAGEN_HIDDEN_BASE(
-			public detail::table_traits_base_specialized<std::make_index_sequence<sizeof...(Columns)>, Columns...>)
+		SOAGEN_HIDDEN_BASE(public detail::table_traits_base_specialized<std::make_index_sequence<sizeof...(Columns)>,
+																		detail::as_column<Columns>...>)
 	{
 		/// @brief The number of columns in the table.
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
-		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		/// @brief	The number of rows to advance to maintain the requested `alignment` for every column.
 		///
 		/// @details	The stride size you need to use when iterating through rows of this table such that
 		///				the starting element for each batch in each column would have the same memory alignment as the
 		///				value specified for the column-specific `alignment`.
 		///
 		/// @note		Typically you can ignore this; column elements are always aligned correctly according to their
 		///				type. This is for over-alignment scenarios where you need to do things in batches (e.g. SIMD).
-		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, Columns::aligned_stride...);
+		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, detail::as_column<Columns>::aligned_stride...);
 
 		// columns
 		// (note that these hide the base class typedefs - this is intentional)
 
 		/// @brief	Returns the #soagen::column_traits for the column at the specified index.
 		template <auto Index>
-		using column = type_at_index<static_cast<size_t>(Index), Columns...>;
+		using column = type_at_index<static_cast<size_t>(Index), detail::as_column<Columns>...>;
 
 		/// @brief	Same as #column but takes an #index_constant.
 		template <typename IndexConstant>
-		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), Columns...>;
+		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), detail::as_column<Columns>...>;
 
 		/// @brief Array containing the `alignment` for each column.
-		static constexpr size_t column_alignments[column_count] = { Columns::alignment... };
+		static constexpr size_t column_alignments[column_count] = { detail::as_column<Columns>::alignment... };
 
 		/// @brief The max `alignment` of all columns in the table.
-		static constexpr size_t largest_alignment = max(size_t{ 1 }, Columns::alignment...);
+		static constexpr size_t largest_alignment = max(size_t{ 1 }, detail::as_column<Columns>::alignment...);
 
 		/// @brief True if the arguments passed to the rvalue overloads of `push_back()`
 		/// and `insert()` would be distinct from the regular const lvalue  overload.
-		static constexpr bool rvalue_type_list_is_distinct = POXY_IMPLEMENTATION_DETAIL(
-			!(std::is_same_v<typename Columns::param_type, typename Columns::rvalue_type> && ...));
+		static constexpr bool rvalue_type_list_is_distinct =
+			POXY_IMPLEMENTATION_DETAIL(!(std::is_same_v<typename detail::as_column<Columns>::param_type,
+														typename detail::as_column<Columns>::rvalue_type>
+										 && ...));
 
 		/// @brief True if a generated class's `emplace_back()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		/// @tparam Args The args being passed to #soagen::table::emplace_back().
 		template <typename BackingTable, typename... Args>
 		static constexpr bool emplace_back_is_nothrow =
 			noexcept(std::declval<BackingTable>().emplace_back(std::declval<Args>()...));
 
 		/// @brief True if a generated class's lvalue `push_back()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		template <typename BackingTable>
 		static constexpr bool push_back_is_nothrow =
-			emplace_back_is_nothrow<BackingTable, typename Columns::param_forward_type...>;
+			emplace_back_is_nothrow<BackingTable, typename detail::as_column<Columns>::param_forward_type...>;
 
 		/// @brief True if a generated class's rvalue `push_back()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		template <typename BackingTable>
 		static constexpr bool rvalue_push_back_is_nothrow =
-			emplace_back_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
+			emplace_back_is_nothrow<BackingTable, typename detail::as_column<Columns>::rvalue_forward_type...>;
 
 		/// @brief True if a generated class's row `push_back()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		/// @tparam Row The row type.
 		template <typename BackingTable, typename Row>
 		static constexpr bool row_push_back_is_nothrow = emplace_back_is_nothrow<BackingTable, Row>;
 
@@ -934,21 +937,21 @@
 			noexcept(std::declval<BackingTable>().emplace(typename remove_cvref<BackingTable>::size_type{},
 														  std::declval<Args>()...));
 
 		/// @brief True if a generated class's lvalue `insert()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		template <typename BackingTable>
 		static constexpr bool insert_is_nothrow =
-			emplace_is_nothrow<BackingTable, typename Columns::param_forward_type...>;
+			emplace_is_nothrow<BackingTable, typename detail::as_column<Columns>::param_forward_type...>;
 
 		/// @brief True if a generated class's rvalue `insert()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		template <typename BackingTable>
 		static constexpr bool rvalue_insert_is_nothrow =
-			emplace_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
+			emplace_is_nothrow<BackingTable, typename detail::as_column<Columns>::rvalue_forward_type...>;
 
 		/// @brief True if a generated class's row `insert()` would be nothrow.
 		/// @tparam BackingTable The backing #soagen::table type.
 		/// @tparam Row The row type.
 		template <typename BackingTable, typename Row>
 		static constexpr bool row_insert_is_nothrow = emplace_is_nothrow<BackingTable, Row>;
 
@@ -965,38 +968,41 @@
 		/// @tparam Const True for `const` column data pointers.
 		template <typename Func, bool Const = false>
 		static constexpr bool for_each_column_nothrow_invocable = POXY_IMPLEMENTATION_DETAIL(void);
 
 #endif
 	};
 
-	/// @brief True if `T` is an instance of #soagen::table_traits.
-	template <typename T>
-	inline constexpr bool is_table_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	/// @cond
-	template <typename... Columns>
-	inline constexpr bool is_table_traits<table_traits<Columns...>> = true;
-	template <typename... Columns>
-	inline constexpr bool is_table_traits<detail::table_traits_base<Columns...>> = true;
-	template <typename T>
-	inline constexpr bool is_table_traits<const T> = is_table_traits<T>;
-	template <typename T>
-	inline constexpr bool is_table_traits<volatile T> = is_table_traits<T>;
-	template <typename T>
-	inline constexpr bool is_table_traits<const volatile T> = is_table_traits<T>;
+	namespace detail
+	{
+		template <typename>
+		struct is_table_traits_ : std::false_type
+		{};
+		template <typename... Columns>
+		struct is_table_traits_<table_traits<Columns...>> : std::true_type
+		{};
+		template <typename... Columns>
+		struct is_table_traits_<detail::table_traits_base<Columns...>> : std::true_type
+		{};
+	}
 	/// @endcond
+	/// @brief True if `T` is a #soagen::table_traits.
+	template <typename T>
+	inline constexpr bool is_table_traits =
+		POXY_IMPLEMENTATION_DETAIL(detail::is_table_traits_<std::remove_cv_t<T>>::value);
 }
 
 /// @cond
 namespace soagen::detail
 {
 	template <typename... Columns>
 	struct to_base_traits_<table_traits<Columns...>>
 	{
-		using type = table_traits_base<to_base_traits<Columns>...>;
+		using type = table_traits_base<to_base_traits<as_column<Columns>>...>;
 
 		static_assert(std::is_base_of_v<type, table_traits<Columns...>>);
 	};
 
 	template <typename... Columns>
 	struct table_traits_type_<table_traits<Columns...>>
 	{
```

### Comparing `soagen-0.4.0/src/soagen/hpp/tuples.hpp` & `soagen-0.5.0/src/soagen/hpp/tuples.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 	{
 		if constexpr (detail::has_tuple_get_member_<T&&>::value)
 		{
 			return static_cast<T&&>(tuple).template get<I>();
 		}
 		else if constexpr (detail::has_tuple_get_adl_<T&&>::value)
 		{
-			using std::get;
+			using detail::adl_dummy::get;
 			return get<I>(static_cast<T&&>(tuple));
 		}
 	}
 
 	/// @cond
 	namespace detail
 	{
```

### Comparing `soagen-0.4.0/src/soagen/includes.py` & `soagen-0.5.0/src/soagen/includes.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/injectors.py` & `soagen-0.5.0/src/soagen/injectors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/log.py` & `soagen-0.5.0/src/soagen/log.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/main.py` & `soagen-0.5.0/src/soagen/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,15 +451,14 @@
                     # sub in external headers
                     includes = sorted(set(src.includes.external + cpp.detect_includes(s)))
                     includes = cpp.remove_implicit_includes(includes)
                     EXTERNAL_HEADERS = r'\n[ \t]*//[ \t]*__SOAGEN_EXTERNAL_HEADERS[ \t]*\n'
                     rep = '\nSOAGEN_DISABLE_WARNINGS;'
                     for inc in includes:
                         rep += f'\n#include <{inc}>'
-                    rep += '\n#if SOAGEN_HAS_EXCEPTIONS\n\t#include <stdexcept>\n#endif'
                     rep += '\nSOAGEN_ENABLE_WARNINGS;\n'
                     s = re.sub(EXTERNAL_HEADERS, rep, s)
                     # strip doxygen stuff if we have that disabled
                     if not o.doxygen:
                         s = re.sub(
                             r'\n[ \t]*#[ \t]*if[ \t]*SOAGEN_DOXYGEN[ \t]*\n.+?\n[ \t]*#[ \t]*endif[ \t]*\n',
                             '\n',
```

### Comparing `soagen-0.4.0/src/soagen/metavars.py` & `soagen-0.5.0/src/soagen/metavars.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/natvis_file.py` & `soagen-0.5.0/src/soagen/natvis_file.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/paths.py` & `soagen-0.5.0/src/soagen/paths.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/preprocessor.py` & `soagen-0.5.0/src/soagen/preprocessor.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/schemas.py` & `soagen-0.5.0/src/soagen/schemas.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/struct.py` & `soagen-0.5.0/src/soagen/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,23 +189,14 @@
         self.meta.push('index', index)
         self.meta.push('struct::index', index)
 
     def write_forward_declarations(self, o: Writer):
         with MetaScope(self):
             o(rf'class {self.type};')
 
-    def write_soagen_specializations(self, o: Writer):
-        with MetaScope(self):
-            o(
-                rf'''
-            template <>
-            inline constexpr bool is_soa<{self.qualified_name}> = true;
-            '''
-            )
-
     def write_soagen_detail_specializations(self, o: Writer):
         with MetaScope(self):
             max_length = 0
             for col in self.columns:
                 max_length = max(len(col.name), max_length)
             with StringIO() as buf:
                 buf.write('table_traits<\n')
@@ -231,14 +222,18 @@
                 }};
 
                 template <>
                 struct allocator_type_<{self.qualified_name}>
                 {{
                     using type = {self.allocator};
                 }};
+
+                template <>
+                struct is_soa_<{self.qualified_name}> : std::true_type
+                {{}};
                 '''
                 )
 
                 for col in self.columns:
                     o(rf'SOAGEN_MAKE_COLUMN({self.qualified_name}, {col.index}, {col.name});')
 
             o(
@@ -322,15 +317,15 @@
                     {doxygen(r"@brief This class's underlying soagen::table type.")}
                     using table_type = soagen::table_type<{self.name}>;
 
                     {doxygen(r"@brief The soagen::table_traits for the underlying table.")}
                     using table_traits = soagen::table_traits_type<{self.name}>;
 
                     {doxygen(r"@brief The number of columns in the table.")}
-                    static constexpr size_type column_count = soagen::table_traits_type<{self.name}>::column_count;
+                    static constexpr size_type column_count = table_traits::column_count;
 
                     {doxygen(r"@brief Gets the soagen::column_traits for a specific column of the table.")}
                     template <auto Column>
                     using column_traits = typename table_traits::template column<static_cast<size_type>(Column)>;
 
                     {doxygen(r"@brief Gets the type of a specific column in the table.")}
                     template <auto Column>
@@ -339,18 +334,18 @@
                     '''
                     )
 
                     if self.iterators:
                         o(
                             rf'''
                             {doxygen(r"@brief Row iterators returned by iterator functions.")}
-                            using iterator = soagen::iterator_type<{self.name}&>;
+                            using iterator = soagen::iterator_type<{self.name}>;
 
                             {doxygen(r"@brief Row iterators returned by const-qualified iterator functions.")}
-                            using const_iterator = soagen::iterator_type<const {self.name}&>;
+                            using const_iterator = soagen::iterator_type<const {self.name}>;
                             '''
                         )
 
                         if self.rvalue_iterators:
                             o(
                                 rf'''
                                 {doxygen(r"@brief Row iterators returned by rvalue-qualified iterator functions.")}
@@ -377,18 +372,18 @@
                                 using rvalue_reverse_iterator = std::reverse_iterator<rvalue_iterator>;
                                 '''
                             )
 
                     o(
                         rf'''
                     {doxygen(r"@brief Regular (lvalue-qualified) row type used by this class.")}
-                    using row_type = soagen::row_type<{self.name}&>;
+                    using row_type = soagen::row_type<{self.name}>;
 
                     {doxygen(r"@brief Const row type used by this class.")}
-                    using const_row_type = soagen::row_type<const {self.name}&>;
+                    using const_row_type = soagen::row_type<const {self.name}>;
 
                     {doxygen(r"@brief Rvalue row type used by this class.")}
                     using rvalue_row_type = soagen::row_type<{self.name}&&>;
 
                     {doxygen(r"""
                     @brief   The number of rows to advance to maintain the requested `alignment` for every column.
 
@@ -679,15 +674,15 @@
                                     SOAGEN_HIDDEN(template <bool sfinae = soagen::has_unordered_erase_member<table_type>>)
                                     SOAGEN_ALWAYS_INLINE
                                     SOAGEN_CPP20_CONSTEXPR
                                     SOAGEN_ENABLE_IF_T(soagen::optional<{const}iterator>, sfinae) unordered_erase({const}iterator pos) //
                                         noexcept(soagen::has_nothrow_unordered_erase_member<table_type>)
                                     {{
                                         if (auto moved_pos = table_.unordered_erase(static_cast<size_type>(pos)); moved_pos)
-                                            return {const}iterator{{ *this, static_cast<difference_type>(*moved_pos) }};
+                                            return {const}iterator{{ table_, static_cast<difference_type>(*moved_pos) }};
                                         return {{}};
                                     }}
 
 
 
                                 '''
                                 )
@@ -709,17 +704,17 @@
                         @brief Swaps two columns.
 
                         @availability The two columns must have the same underlying value_type.""")}
                         template <auto A, auto B>
                         SOAGEN_ALWAYS_INLINE
                         SOAGEN_CPP20_CONSTEXPR
                         {self.name}& swap_columns() //
-                            noexcept(noexcept(std::declval<table_type&>().template swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>()))
+                            noexcept(noexcept(std::declval<table_type&>().template swap_columns<static_cast<size_type>(A), static_cast<size_type>(B)>()))
                         {{
-                            table_.template swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>();
+                            table_.template swap_columns<static_cast<size_type>(A), static_cast<size_type>(B)>();
                             return *this;
                         }}
 
                         #if SOAGEN_DOXYGEN
 
                         {doxygen(r"""
                         @brief Resizes the table to the given number of rows.
@@ -1184,15 +1179,15 @@
                                 {doxygen(r"""
                                 @brief Returns the row at the given index.
 
                                 @tparam Columns Indices of the columns to include in the row. Leave the list empty for all columns.""")}
                                 template <auto... Columns>
                                 SOAGEN_PURE_GETTER
                                 SOAGEN_CPP20_CONSTEXPR
-                                soagen::row_type<{const}{self.name}{ref}, Columns...> row(size_type index) {const}{ref} noexcept
+                                soagen::row_type<{const}{self.name}{'&&' if ref == '&&' else ''}, Columns...> row(size_type index) {const}{ref} noexcept
                                 {{
                                     if constexpr (sizeof...(Columns))
                                     {{
                                         return {{ {{ {move_l}this->template column<static_cast<size_type>(Columns)>()[index]{move_r} }}... }};
                                     }}
                                     else
                                     {{
@@ -1254,42 +1249,43 @@
                                         if 'c' in func and (not const or ref == '&&'):
                                             continue
                                         if ref == '&&' and not self.rvalue_iterators:
                                             continue
 
                                         move_l = 'std::move(' if ref == '&&' else ''
                                         move_r = ')' if ref == '&&' else ''
-                                        begin = rf'{func}end()' if reverse else rf'{move_l}*this{move_r}, 0'
+                                        begin = rf'{func}end()' if reverse else rf'{move_l}table_{move_r}, 0'
                                         end = (
                                             rf'{func}begin()'
                                             if reverse
-                                            else rf'{move_l}*this{move_r}, static_cast<difference_type>(size())'
+                                            else rf'{move_l}table_{move_r}, static_cast<difference_type>(size())'
                                         )
+                                        func_ref = ref if (self.rvalue_iterators and 'c' not in func) else ''
 
                                         an = 'a reverse' if reverse else 'an'
                                         past = 'before' if reverse else 'past'
                                         first = 'last' if reverse else 'first'
                                         last = 'first' if reverse else 'last'
-                                        iterator = rf'soagen::iterator_type<{const}{self.name}{ref}, Columns...>'
+                                        iterator = rf'soagen::iterator_type<{const}{self.name}{"&&" if ref == "&&" else ""}, Columns...>'
 
                                         o(
                                             rf'''
 
                                         {doxygen(rf"""@brief Returns {an} iterator to the {first} row in the table.""")}
-                                        template <size_type... Columns>
+                                        template <auto... Columns>
                                         SOAGEN_PURE_INLINE_GETTER
-                                        constexpr {iterator} {func}begin() {const}{ref if self.rvalue_iterators else ''} noexcept
+                                        constexpr {iterator} {func}begin() {const}{func_ref} noexcept
                                         {{
                                             return {{ {begin} }};
                                         }}
 
                                         {doxygen(rf"""@brief Returns {an} iterator to one-{past}-the-{last} row in the table.""")}
-                                        template <size_type... Columns>
+                                        template <auto... Columns>
                                         SOAGEN_PURE_INLINE_GETTER
-                                        constexpr {iterator} {func}end() {const}{ref if self.rvalue_iterators else ''} noexcept
+                                        constexpr {iterator} {func}end() {const}{func_ref} noexcept
                                         {{
                                             return {{ {end} }};
                                         }}
                                         '''
                                         )
 
                 o(
```

### Comparing `soagen-0.4.0/src/soagen/type_list.py` & `soagen-0.5.0/src/soagen/type_list.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/utils.py` & `soagen-0.5.0/src/soagen/utils.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/variable.py` & `soagen-0.5.0/src/soagen/variable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/version.py` & `soagen-0.5.0/src/soagen/version.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen/writer.py` & `soagen-0.5.0/src/soagen/writer.py`

 * *Files identical despite different names*

### Comparing `soagen-0.4.0/src/soagen.egg-info/PKG-INFO` & `soagen-0.5.0/src/soagen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.4.0
+Version: 0.5.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,20 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.5.0
+
+-   Added rows to `soagen::table`
+-   Added iterators to `soagen::table`
+-   Added `soagen::table::for_each_column()`
+
 ## v0.4.0
 
 -   Fixed `soagen::is_table<>`
 -   Added support for emplace-constructing column values by unpacking all `std::tuple`-like types (not just the `emplacer`)
 -   Added support for taking `std::integral_constants` in `for_each_column()`
 -   Added `soagen::same_table_type<>`
 -   Added conversions between `soagen::row<>` specializations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.4.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.5.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,22 +13,24 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.4.0 - Fixed `soagen::is_table<>` - Added
-support for emplace-constructing column values by unpacking all `std::tuple`-
-like types (not just the `emplacer`) - Added support for taking `std::
-integral_constants` in `for_each_column()` - Added `soagen::same_table_type<>`
-- Added conversions between `soagen::row<>` specializations - Optimized
-instantiation overhead for most type-traits ## v0.3.0 - Added `hpp.combined` -
-Added `std::integral_constant` to the overload set used by `for_each_column()`
-- Added support for constructing rows from all `std::tuple`-like types -
-Optimized bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
+sponsors/marzer # Changelog ## v0.5.0 - Added rows to `soagen::table` - Added
+iterators to `soagen::table` - Added `soagen::table::for_each_column()` ##
+v0.4.0 - Fixed `soagen::is_table<>` - Added support for emplace-constructing
+column values by unpacking all `std::tuple`-like types (not just the
+`emplacer`) - Added support for taking `std::integral_constants` in
+`for_each_column()` - Added `soagen::same_table_type<>` - Added conversions
+between `soagen::row<>` specializations - Optimized instantiation overhead for
+most type-traits ## v0.3.0 - Added `hpp.combined` - Added `std::
+integral_constant` to the overload set used by `for_each_column()` - Added
+support for constructing rows from all `std::tuple`-like types - Optimized
+bulk-swap operations ## v0.2.0 - Added `structs.annotations` - Added
 `structs.attributes` - Added `auto` option for `structs.default_constructible`
 - Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
 iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
 Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
 columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
 First public release ð&#xFE0F;
```

### Comparing `soagen-0.4.0/src/soagen.egg-info/SOURCES.txt` & `soagen-0.5.0/src/soagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

