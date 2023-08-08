# Comparing `tmp/delvewheel-1.4.0.tar.gz` & `tmp/delvewheel-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delvewheel-1.4.0.tar", last modified: Thu Jul 20 19:25:02 2023, max compression
+gzip compressed data, was "delvewheel-1.5.0.tar", last modified: Tue Aug  8 15:05:23 2023, max compression
```

## Comparing `delvewheel-1.4.0.tar` & `delvewheel-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:25:02.743006 delvewheel-1.4.0/
--rw-rw-rw-   0        0        0     1073 2023-07-20 19:24:28.000000 delvewheel-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    10937 2023-07-20 19:25:02.743006 delvewheel-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     9817 2023-07-20 19:24:28.000000 delvewheel-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 19:25:02.727445 delvewheel-1.4.0/delvewheel/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/__init__.py
--rw-rw-rw-   0        0        0     5825 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/__main__.py
--rw-rw-rw-   0        0        0   139059 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_dll_list.py
--rw-rw-rw-   0        0        0    33153 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_dll_utils.py
--rw-rw-rw-   0        0        0       23 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_version.py
--rw-rw-rw-   0        0        0    48135 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_wheel_repair.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:25:02.743006 delvewheel-1.4.0/delvewheel.egg-info/
--rw-rw-rw-   0        0        0    10937 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-07-20 19:24:28.000000 delvewheel-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1214 2023-07-20 19:25:02.743006 delvewheel-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 15:05:23.371661 delvewheel-1.5.0/
+-rw-rw-rw-   0        0        0     1073 2023-08-08 15:04:54.000000 delvewheel-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    11152 2023-08-08 15:05:23.371661 delvewheel-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10032 2023-08-08 15:04:54.000000 delvewheel-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 15:05:23.356037 delvewheel-1.5.0/delvewheel/
+-rw-rw-rw-   0        0        0        0 2023-08-08 15:04:54.000000 delvewheel-1.5.0/delvewheel/__init__.py
+-rw-rw-rw-   0        0        0     5974 2023-08-08 15:04:54.000000 delvewheel-1.5.0/delvewheel/__main__.py
+-rw-rw-rw-   0        0        0   139064 2023-08-08 15:04:54.000000 delvewheel-1.5.0/delvewheel/_dll_list.py
+-rw-rw-rw-   0        0        0    34404 2023-08-08 15:04:54.000000 delvewheel-1.5.0/delvewheel/_dll_utils.py
+-rw-rw-rw-   0        0        0       23 2023-08-08 15:04:54.000000 delvewheel-1.5.0/delvewheel/_version.py
+-rw-rw-rw-   0        0        0    49529 2023-08-08 15:04:54.000000 delvewheel-1.5.0/delvewheel/_wheel_repair.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:05:23.371661 delvewheel-1.5.0/delvewheel.egg-info/
+-rw-rw-rw-   0        0        0    11152 2023-08-08 15:05:23.000000 delvewheel-1.5.0/delvewheel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-08-08 15:05:23.000000 delvewheel-1.5.0/delvewheel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 15:05:23.000000 delvewheel-1.5.0/delvewheel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-08-08 15:05:23.000000 delvewheel-1.5.0/delvewheel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 15:05:23.000000 delvewheel-1.5.0/delvewheel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 15:05:23.000000 delvewheel-1.5.0/delvewheel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-08-08 15:04:54.000000 delvewheel-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1214 2023-08-08 15:05:23.371661 delvewheel-1.5.0/setup.cfg
```

### Comparing `delvewheel-1.4.0/LICENSE` & `delvewheel-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delvewheel-1.4.0/PKG-INFO` & `delvewheel-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.4.0
+Version: 1.5.0
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -85,21 +85,22 @@
 - `-v`: verbosity
   - `-v`: level 1, some diagnostic information
   - `-vv`: level 2, include warnings from `pefile`
 - `--extract-dir`: directory to store extracted contents of wheel for debug use (default is a temp directory)
 - `-w`,`--wheel-dir`: directory to write the repaired wheel (default is `wheelhouse` relative to current working directory)
 - `--no-mangle`: name(s) of DLL(s) not to mangle, path-separator-delimited
 - `--no-mangle-all`: don't mangle any DLL names
-- `--strip`: strip DLLs that contain trailing data when name-mangling. The GNU `strip` utility must be present in `PATH`.
+- `--strip`: strip DLLs that contain an overlay when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
 - `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
   - `--namespace-pkg package1` declares `package1` as a namespace package.
   - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
+- `--include-symbols`: include `.pdb` symbol files with the vendored DLLs. To be included, a symbol file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.pdb`.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
-- To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
+- To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain an overlay at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, the overlay consists of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the overlay, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the overlay and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.4.0/README.md` & `delvewheel-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,21 +57,22 @@
 - `-v`: verbosity
   - `-v`: level 1, some diagnostic information
   - `-vv`: level 2, include warnings from `pefile`
 - `--extract-dir`: directory to store extracted contents of wheel for debug use (default is a temp directory)
 - `-w`,`--wheel-dir`: directory to write the repaired wheel (default is `wheelhouse` relative to current working directory)
 - `--no-mangle`: name(s) of DLL(s) not to mangle, path-separator-delimited
 - `--no-mangle-all`: don't mangle any DLL names
-- `--strip`: strip DLLs that contain trailing data when name-mangling. The GNU `strip` utility must be present in `PATH`.
+- `--strip`: strip DLLs that contain an overlay when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
 - `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
   - `--namespace-pkg package1` declares `package1` as a namespace package.
   - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
+- `--include-symbols`: include `.pdb` symbol files with the vendored DLLs. To be included, a symbol file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.pdb`.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
-- To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
+- To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain an overlay at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, the overlay consists of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the overlay, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the overlay and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.4.0/delvewheel/__main__.py` & `delvewheel-1.5.0/delvewheel/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     parser_repair.add_argument('-w', '--wheel-dir', dest='target', default='wheelhouse', help='directory to write repaired wheel')
     parser_repair.add_argument('--no-mangle', default='', metavar='DLLS', type=_dll_names, help=f'DLL names(s) not to mangle, {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-mangle-all', action='store_true', help="don't mangle any DLL names")
     parser_repair.add_argument('--strip', action='store_true', help='strip DLLs that contain trailing data when name-mangling')
     parser_repair.add_argument('-L', '--lib-sdir', default='.libs', type=_subdir_suffix, help='directory suffix in package to store vendored DLLs (default .libs)')
     parser_repair.add_argument('--namespace-pkg', default='', metavar='PKGS', type=_namespace_pkgs, help=f'namespace package(s), {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-diagnostic', action='store_true', help=argparse.SUPPRESS)  # don't write diagnostic information to DELVEWHEEL metadata file
+    parser_repair.add_argument('--include-symbols', action='store_true', help='include .pdb symbol files with vendored DLLs')
     parser_needed.add_argument('file', help='path to a DLL or PYD file')
     parser_needed.add_argument('-v', action='count', default=0, help='verbosity')
     args = parser.parse_args()
 
     # handle command
     if args.command in ('show', 'repair'):
         add_paths = dict.fromkeys(os.path.abspath(path) for path in args.add_path.split(os.pathsep) if path)
@@ -76,15 +77,15 @@
         for wheel in args.wheel:
             wr = WheelRepair(wheel, args.extract_dir, add_dlls, no_dlls, args.ignore_in_wheel, args.v, args.test.split(','))
             if args.command == 'show':
                 wr.show()
             else:  # args.command == 'repair'
                 no_mangles = set(dll_name.lower() for dll_name in args.no_mangle.split(os.pathsep) if dll_name)
                 namespace_pkgs = set(tuple(namespace_pkg.split('.')) for namespace_pkg in args.namespace_pkg.split(os.pathsep) if namespace_pkg)
-                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, args.no_diagnostic, namespace_pkgs)
+                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, args.no_diagnostic, namespace_pkgs, args.include_symbols)
     else:  # args.command == 'needed'
         for dll_name in sorted(_dll_utils.get_direct_needed(args.file, args.v), key=str.lower):
             print(dll_name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `delvewheel-1.4.0/delvewheel/_dll_list.py` & `delvewheel-1.5.0/delvewheel/_dll_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if tag == 'win_arm64':
             return cls.ARM64
         return None
 
 
 # set of regular expressions for additional DLLs to ignore
 ignore_regexes = {
-    re.compile(r'python[0-9]+\.dll'),  # included in CPython distribution
+    re.compile(r'python[0-9]+(_d)?\.dll'),  # included in CPython distribution
     re.compile(r'libpypy([0-9]+\.)*[0-9]+-c\.dll'),  # included in PyPy distribution
     re.compile('api-.*'),  # let Windows handle API sets
 }
 
 # DLLs to ignore based on ABI tag and platform tag. For CPython, these are
 # included in their respective Python distributions. For PyPy, these are
 # prerequisites for PyPy to run in the first place. Strictly speaking,
```

### Comparing `delvewheel-1.4.0/delvewheel/_dll_utils.py` & `delvewheel-1.5.0/delvewheel/_dll_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,48 +205,69 @@
         return lambda directory, arch: translate_system32_to_syswow64(directory) if arch is MachineType.I386 else directory
     return null_translator
 
 
 _translate_directory = _translate_directory()
 
 
-def find_library(name: str, wheel_dirs: typing.Optional[typing.Iterable], arch: MachineType) -> typing.Optional[str]:
-    """Given the name of a DLL, return the path to the DLL, or None if the DLL
-    cannot be found. DLL names are searched in a case-insensitive fashion. The
-    search goes in the following order and considers only the DLLs with the
-    given architecture.
+def find_library(name: str, wheel_dirs: typing.Optional[typing.Iterable], arch: MachineType, include_symbols: bool) -> typing.Optional[typing.Tuple[str, typing.Optional[str]]]:
+    """Given the name of a DLL, return a tuple where
+    - the 1st element is the path to the DLL
+    - the 2nd element is
+      - if include_symbols is False, then None
+      - if include_symbols is True, then the path to the .pdb symbol file next
+        to the DLL if it exists, None otherwise. Excluding the file extension,
+        the name of the symbol file is assumed to be the same as the name of
+        the DLL.
+    If the DLL cannot be found, then return None. DLL and symbol file names are
+    searched in a case-insensitive fashion. The search goes in the following
+    order and considers only the DLLs with the architecture arch.
 
-    1. If not None, the directories in wheel_dirs.
+    1. If not None, the directories in wheel_dirs. We never search for symbol
+       files in wheel_dirs.
     2. The PATH environment variable, with any applicable adjustments due to
-       the Windows file system redirector. (If we are on a case-sensitive file
+       the Windows file system redirector. If we are on a case-sensitive file
        system and a directory contains more than one DLL with the correct
-       architecture that differs by case only, then choose one arbitrarily.)"""
+       architecture that differs by case only, then choose one arbitrarily."""
     name = name.lower()
     if wheel_dirs is not None:
         for wheel_dir in wheel_dirs:
             try:
                 contents = os.listdir(wheel_dir)
             except FileNotFoundError:
                 continue
             for item in contents:
                 if name == item.lower():
                     path = os.path.join(wheel_dir, item)
                     if os.path.isfile(path) and get_arch(path) == arch:
-                        return path
+                        return path, None
     for directory in os.environ['PATH'].split(os.pathsep):
         directory = _translate_directory(directory, arch)
         try:
             contents = os.listdir(directory)
         except FileNotFoundError:
             continue
+        dll_path = None
         for item in contents:
             if name == item.lower():
                 path = os.path.join(directory, item)
                 if os.path.isfile(path) and get_arch(path) == arch:
-                    return path
+                    dll_path = path
+                    break
+        symbol_path = None
+        if dll_path and include_symbols:
+            symbol_name = os.path.splitext(name)[0] + '.pdb'
+            for item in contents:
+                if symbol_name == item.lower():
+                    path = os.path.join(directory, item)
+                    if os.path.isfile(path):
+                        symbol_path = path
+                        break
+        if dll_path:
+            return dll_path, symbol_path
     return None
 
 
 def get_direct_needed(lib_path: str, verbose: int) -> set:
     """Given the path to a shared library, return a set containing the DLL
     names of all its direct dependencies. Regular and delay-load dependencies
     are included. The DLL names are in the original case."""
@@ -296,36 +317,41 @@
     return needed
 
 
 def get_all_needed(lib_path: str,
                    no_dlls: set,
                    wheel_dirs: typing.Optional[typing.Iterable],
                    on_error: str,
-                   verbose: int) -> typing.Tuple[typing.Set[str], typing.Set[str], typing.Set[str]]:
-    """Given the path to a shared library, return a 3-tuple of sets
-    (discovered, ignored, not_found).
-
-    discovered contains the original-case DLL paths of all direct and indirect
-    dependencies of that shared library that should be bundled into the wheel.
-    ignored contains the lowercased DLL names of all direct and indirect
-    dependencies of that shared library that will not be bundled into the wheel
-    because they are assumed to be on the target system.
-
-    If on_error is 'raise', FileNotFoundError is raised if a dependent library
-    cannot be found. If on_error is 'ignore', not_found contains the lowercased
-    DLL names of all dependent DLLs that cannot be found.
+                   include_symbols: bool,
+                   verbose: int) -> typing.Tuple[typing.Set[str], typing.Set[str], typing.Set[str], typing.Set[str]]:
+    """Given the path to a shared library, return a 4-tuple of sets
+    (discovered, symbols, ignored, not_found).
+    - discovered contains the original-case DLL paths of all direct and
+      indirect dependencies of that shared library that should be bundled into
+      the wheel.
+    - symbols contains the original-case paths of any .pdb symbol files
+      corresponding to the DLLs in discovered.
+    - ignored contains the lowercased DLL names of all direct and indirect
+      dependencies of that shared library that will not be bundled into the
+      wheel because they are assumed to be on the target system.
+    - If on_error is 'raise', FileNotFoundError is raised if a dependent
+      library cannot be found. If on_error is 'ignore', not_found contains the
+      lowercased DLL names of all dependent DLLs that cannot be found.
 
     no_dlls is a set of DLL names to force exclusion from the wheel. We do not
     search for dependencies of these DLLs.
 
     If wheel_dirs is not None, it is an iterable of directories in the wheel
-    where dependencies are searched first."""
+    where dependencies are searched first.
+
+    include_symbols specifies whether to search for .pdb symbol files"""
     first_lib_path = lib_path.lower()
     stack = [first_lib_path]
     discovered = set()
+    symbols = set()
     ignored = set()
     not_found = set()
     while stack:
         lib_path = stack.pop()
         if lib_path not in discovered:
             discovered.add(lib_path)
             with PEContext(lib_path, None, True, verbose) as pe:
@@ -340,25 +366,27 @@
                 lib_name_lower = os.path.basename(lib_path).lower()
                 for entry in imports:
                     dll_name = entry.dll.decode('utf-8').lower()
                     if dll_name not in ignore_names and \
                             not any(r.fullmatch(dll_name) for r in _dll_list.ignore_regexes) and \
                             dll_name not in no_dlls and \
                             (lib_name_lower not in _dll_list.ignore_dependency or dll_name not in _dll_list.ignore_dependency[lib_name_lower]):
-                        dll_path = find_library(dll_name, wheel_dirs, lib_arch)
-                        if dll_path:
-                            stack.append(dll_path)
+                        dll_info = find_library(dll_name, wheel_dirs, lib_arch, include_symbols)
+                        if dll_info:
+                            stack.append(dll_info[0])
+                            if dll_info[1]:
+                                symbols.add(dll_info[1])
                         elif on_error == 'raise':
                             raise FileNotFoundError(f'Unable to find library: {dll_name}')
                         else:
                             not_found.add(dll_name)
                     else:
                         ignored.add(dll_name)
     discovered.remove(first_lib_path)
-    return discovered, ignored, not_found
+    return discovered, symbols, ignored, not_found
 
 
 def _round_to_next(size: int, alignment: int) -> int:
     """Return smallest n such that n % alignment == 0 and n >= size."""
     if size % alignment == 0:
         return size
     else:
@@ -374,16 +402,16 @@
             not section.IMAGE_SCN_LNK_NRELOC_OVFL and
             not section.IMAGE_SCN_MEM_DISCARDABLE and
             not section.IMAGE_SCN_MEM_EXECUTE and
             section.IMAGE_SCN_MEM_READ)
 
 
 def _get_pe_size_and_enough_padding(pe: pefile.PE, new_dlls: typing.Iterable[bytes]) -> typing.Tuple[int, bool]:
-    """Determine the size of a PE file (excluding any trailing data) and
-    whether the file has enough padding for writing the elements of new_dlls.
+    """Determine the size of a PE file (excluding any overlay) and whether the
+    file has enough padding for writing the elements of new_dlls.
 
     Determining whether the file has enough padding is an instance of the NP-
     complete bin packing problem, so we use the Next Fit approximation
     algorithm. new_dlls must be in a deterministic order in order for the Next
     Fit algorithm to return a deterministic result.
 
     Side effect: pe.sections is sorted by VirtualAddress. In most cases this
@@ -409,96 +437,94 @@
 
 def replace_needed(lib_path: str, old_deps: typing.List[str], name_map: typing.Dict[str, str], strip: bool, verbose: int, test: typing.List[str]) -> None:
     """For the DLL at lib_path, replace its declared dependencies on old_deps
     with those in name_map.
     old_deps: a subset of the dependencies that lib_path has, in list form
     name_map: a dict that maps an old dependency name to a new name, must
         contain at least all the keys in old_deps
-    strip: whether to try to strip DLLs that contain trailing data if not
-        enough internal padding exists
+    strip: whether to try to strip DLLs that contain overlays if not enough
+        internal padding exists
     verbose: verbosity level, 0 to 2
     test: testing options for internal use"""
     if not old_deps:
         # no dependency names to change
         return
     name_map = {dep.lower().encode('utf-8'): name_map[dep].encode('utf-8') for dep in old_deps}
         # keep only the DLLs that will be mangled
 
-    # If an attribute certificate table exists and is the only trailing data,
-    # remove the table. In this case, we end up removing all trailing data
-    # without needing to run strip.
+    # If an attribute certificate table exists and is the only thing in the
+    # overlay, remove the table. In this case, we end up removing the entire
+    # overlay without needing to run strip.
     with PEContext(lib_path, None, False, verbose) as pe:
         pe_size = max(section.PointerToRawData + section.SizeOfRawData for section in pe.sections)
         cert_table = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']]
         truncate = cert_table.VirtualAddress == _round_to_next(pe_size, _ATTRIBUTE_CERTIFICATE_TABLE_ALIGNMENT) and cert_table.VirtualAddress + cert_table.Size == os.path.getsize(lib_path)
     if truncate:
         with open(lib_path, 'rb+') as f:
             f.truncate(pe_size)
 
     # New dependency names are longer than the old ones, so we cannot simply
     # overwrite the bytes of the old dependency names. Determine whether the PE
     # file has enough usable internal padding to use to write the new
     # dependency names. If so, overwrite the padding. Otherwise, as long as the
-    # PE file contains no trailing data or the trailing data can be stripped,
-    # append a new PE section to store the new names. Determining whether
-    # enough internal padding exists is an instance of the bin packing problem
-    # in which the new dependency names are items and the contiguous padding
-    # runs are bins. The bin packing problem is NP-hard, so for simplicity, we
-    # use the Next Fit algorithm.
+    # PE file contains no overlay or the overlay can be stripped, append a new
+    # PE section to store the new names. Determining whether enough internal
+    # padding exists is an instance of the bin packing problem in which the new
+    # dependency names are items and the contiguous padding runs are bins. The
+    # bin packing problem is NP-hard, so for simplicity, we use the Next Fit
+    # algorithm.
     with PEContext(lib_path, None, False, verbose) as pe:
         pe_size, enough_padding = _get_pe_size_and_enough_padding(pe, name_map.values())
     if 'not_enough_padding' in test:
         enough_padding = False
     if not enough_padding and pe_size < os.path.getsize(lib_path) and strip:
-        # try to strip the trailing data
+        # try to strip the overlay
         try:
             subprocess.check_call(['strip', '-s', lib_path])
         except FileNotFoundError:
             raise FileNotFoundError('GNU strip not found in PATH') from None
         with PEContext(lib_path, None, False, verbose) as pe:
             pe_size, enough_padding = _get_pe_size_and_enough_padding(pe, name_map.values())
 
     lib_name = os.path.basename(lib_path)
     if not enough_padding and pe_size < os.path.getsize(lib_path):
-        # cannot rename dependencies due to trailing data
+        # cannot rename dependencies due to overlay
         if strip:
             raise RuntimeError(textwrap.fill(
                 f'Unable to rename the dependencies of {lib_name} because '
                 'this DLL does not contain enough internal padding to fit the '
-                'new dependency names, and it contains trailing data after '
-                'the point where the DLL file specification ends. The GNU '
+                'new dependency names, and it contains an overlay. The GNU '
                 'strip utility was run automatically in attempt to remove the '
-                'trailing data but failed to remove all of it. Unless you '
-                'have knowledge to the contrary, you should assume that the '
-                'trailing data exist for an important reason and are not safe '
-                f'to remove. Include {os.pathsep.join(old_deps)} in the '
+                'overlay but failed to remove all of it. Unless you have '
+                'knowledge to the contrary, you should assume that the '
+                'overlay exists for an important reason and is not safe to '
+                f'remove. Include {os.pathsep.join(old_deps)} in the '
                 '--no-mangle flag to fix this error.',
                 initial_indent=' ' * len('RuntimeError: ')).lstrip())
         else:
             error_text = [
                 textwrap.fill(
                     f'Unable to rename the dependencies of {lib_name} because '
                     'this DLL does not contain enough internal padding to fit '
-                    'the new dependency names, and it contains trailing data '
-                    'after the point where the DLL file specification ends. '
-                    'Commonly, the trailing data consist of symbols that can '
-                    'be safely removed, although there exist situations where '
+                    'the new dependency names, and it contains an overlay. '
+                    'Commonly, the overlay consists of symbols that can be '
+                    'safely removed, although there exist situations where '
                     'the data must be present for the DLL to function '
                     'properly. Here are your options.',
                     initial_indent=' ' * len('RuntimeError: ')).lstrip(),
                 '\n',
                 textwrap.fill(
-                    '- Try to remove the trailing data using the GNU strip '
+                    '- Try to remove the overlay using the GNU strip '
                     f"utility with the command `strip -s {lib_name}'.",
                     subsequent_indent='  '
                 ),
                 '\n',
                 textwrap.fill(
                     '- Use the --strip flag to ask delvewheel to execute '
-                    'strip automatically when trailing data are detected.',
+                    'strip automatically when an overlay is detected.',
                     subsequent_indent='  '
                 ),
                 '\n',
                 textwrap.fill(
                     f'- Include {os.pathsep.join(old_deps)} in the '
                     '--no-mangle flag.',
                     subsequent_indent='  '
```

### Comparing `delvewheel-1.4.0/delvewheel/_wheel_repair.py` & `delvewheel-1.5.0/delvewheel/_wheel_repair.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,22 +30,21 @@
 # We also preload the DLLs for Anaconda Python < 3.10, which has a bug where
 # os.add_dll_directory() does not always take effect.
 #
 # The template must produce Python code that is compatible with Python 2.6, the
 # oldest supported target Python version.
 #
 # To use the template, call str.format(), passing in
-# 0. '""""""' if the patch would be at the start of the file else ''
+# 0. '"""""" ' if the patch would be at the start of the file else ''
 # 1. an identifying string such as the delvewheel version
 # 2. a number of repeats of 'os.pardir, ' corresponding to the path depth of
 #    the file in site-packages upon wheel installation
 # 3. the name of the directory containing the vendored DLLs
 # 4. the name of the file containing the DLL load order.
-_patch_py_template = """
-
+_patch_py_template = """\
 {0}# start delvewheel patch
 def _delvewheel_patch_{1}():
     import ctypes
     import os
     import platform
     import sys
     libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), {2}{3!r}))
@@ -63,43 +62,40 @@
                 if os.path.isfile(lib_path) and not ctypes.windll.kernel32.LoadLibraryExW(ctypes.c_wchar_p(lib_path), None, 0x00000008):
                     raise OSError('Error loading {{}}; {{}}'.format(lib, ctypes.FormatError()))
 
 
 _delvewheel_patch_{1}()
 del _delvewheel_patch_{1}
 # end delvewheel patch
-
 """
 
 # Template for patching a .py file for Python 3.10 and above. For these Python
 # versions, os.add_dll_directory() is used as the exclusive strategy.
 #
 # The template must produce Python code that is compatible with Python 2.6, the
 # oldest supported target Python version.
 #
 # To use the template, call str.format(), passing in
-# 0. '""""""' if the patch would be at the start of the file else ''
+# 0. '"""""" ' if the patch would be at the start of the file else ''
 # 1. an identifying string such as the delvewheel version
 # 2. a number of repeats of 'os.pardir, ' corresponding to the path depth of
 #    the file in site-packages upon wheel installation
 # 3. the name of the directory containing the vendored DLLs
-_patch_py_template_v2 = """
-
+_patch_py_template_v2 = """\
 {0}# start delvewheel patch
 def _delvewheel_patch_{1}():
     import os
     libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), {2}{3!r}))
     if os.path.isdir(libs_dir):
         os.add_dll_directory(libs_dir)
 
 
 _delvewheel_patch_{1}()
 del _delvewheel_patch_{1}
 # end delvewheel patch
-
 """
 
 pp = pprint.PrettyPrinter(indent=4)
 
 
 class WheelRepair:
     """An instance represents a wheel that can be repaired."""
@@ -221,15 +217,17 @@
         else:
             self._wheel_dirs = None
         self._ignore_in_wheel = ignore_in_wheel
 
         # determine the CPU architecture of the wheel
         self._arch = _dll_list.MachineType.platform_tag_to_type(platform_tag)
         if not self._arch:
-            for root, _, filenames in os.walk(self._extract_dir):
+            for root, dirnames, filenames in os.walk(self._extract_dir):
+                if root == self._data_dir:
+                    dirnames[:] = set(dirnames) & {'platlib', 'purelib'}
                 for filename in filenames:
                     if filename.lower().endswith('.pyd'):
                         arch = _dll_utils.get_arch(os.path.join(root, filename))
                         if not arch:
                             raise NotImplementedError('Wheels for architectures other than x86, x64, and arm64 are not supported')
                         elif self._arch and self._arch is not arch:
                             raise NotImplementedError('Wheels targeting multiple CPU architectures are not supported')
@@ -279,17 +277,17 @@
             file is not used
         depth is the number of parent directories to traverse to reach the
             site-packages directory at runtime starting from the directory
             containing the .py file"""
         if self._min_supported_python is None or self._min_supported_python < (3, 10):
             if load_order_filename is None:
                 raise ValueError('load_order_filename cannot be None')
-            return _patch_py_template.format('""""""' if at_start else '', _version.__version__.replace('.', '_'), 'os.pardir, ' * depth, libs_dir, load_order_filename)
+            return _patch_py_template.format('"""""" ' if at_start else '', _version.__version__.replace('.', '_'), 'os.pardir, ' * depth, libs_dir, load_order_filename)
         else:
-            return _patch_py_template_v2.format('""""""' if at_start else '', _version.__version__.replace('.', '_'), 'os.pardir, ' * depth, libs_dir)
+            return _patch_py_template_v2.format('"""""" ' if at_start else '', _version.__version__.replace('.', '_'), 'os.pardir, ' * depth, libs_dir)
 
     def _patch_py_file(self, py_path: str, libs_dir: str, load_order_filename: typing.Optional[str], depth: int) -> None:
         """Given the path to a .py file, create or patch the file so that
         vendored DLLs can be loaded at runtime. The patch is placed at the
         topmost location after the docstring (if any) and any
         "from __future__ import" statements.
 
@@ -325,47 +323,55 @@
             future_import_lineno = 0  # no "from __future__ import" statement found
 
         if future_import_lineno > 0:
             # insert patch after the last __future__ import
             patch_py_contents = self._patch_py_contents(False, libs_dir, load_order_filename, depth)
             py_contents_split = py_contents.splitlines(True)
             with open(py_path, 'w', newline=newline) as file:
-                file.write(''.join(py_contents_split[:future_import_lineno]))
-                file.write('\n')
+                file.write(''.join(py_contents_split[:future_import_lineno]).rstrip())
+                file.write('\n\n\n')
                 file.write(patch_py_contents)
-                file.write(''.join(py_contents_split[future_import_lineno:]))
+                remainder = ''.join(py_contents_split[future_import_lineno:]).lstrip()
+                if remainder:
+                    file.write('\n')
+                    file.write(remainder)
         elif docstring is None:
             # prepend patch
             patch_py_contents = self._patch_py_contents(True, libs_dir, load_order_filename, depth)
             with open(py_path, 'w', newline=newline) as file:
                 file.write(patch_py_contents)
-                file.write(py_contents)
+                remainder = py_contents.lstrip()
+                if remainder:
+                    file.write('\n')
+                    file.write(remainder)
         else:
             # place patch just after docstring
             patch_py_contents = self._patch_py_contents(False, libs_dir, load_order_filename, depth)
             if len(children) == 0 or not isinstance(children[0], ast.Expr) or ast.literal_eval(children[0].value) != docstring:
                 # verify that the first child node is the docstring
                 raise ValueError(f'Error parsing {py_name}: docstring exists but is not the first element of the parse tree')
             if len(children) == 1:
                 # append patch
-                with open(py_path, 'a') as file:
+                with open(py_path, 'w', newline=newline) as file:
+                    file.write(py_contents.rstrip())
+                    file.write('\n\n\n')
                     file.write(patch_py_contents)
             else:
                 # insert patch after docstring
                 py_contents = '\n'.join(py_contents.splitlines())  # normalize line endings
                 docstring_search_start_index = 0
                 for line in py_contents.splitlines(True):
                     if line.lstrip().startswith('#'):
                         # ignore comments at start of file
                         docstring_search_start_index += len(line)
                     else:
                         break
                 double_quotes_index = py_contents.find('"""', docstring_search_start_index)
                 single_quotes_index = py_contents.find("'''", docstring_search_start_index)
-                if double_quotes_index == -1 and single_quotes_index == -1:
+                if double_quotes_index == single_quotes_index == -1:
                     raise ValueError(f'Error parsing {py_name}: docstring exists but does not start with triple quotes')
                 elif double_quotes_index == -1 or single_quotes_index != -1 and single_quotes_index < double_quotes_index:
                     docstring_start_index = single_quotes_index
                     quotes = "'''"
                 else:
                     docstring_start_index = double_quotes_index
                     quotes = '"""'
@@ -376,18 +382,19 @@
                 docstring_end_line = py_contents.find('\n', docstring_end_index)
                 if docstring_end_line == -1:
                     docstring_end_line = len(py_contents)
                 extra_text = py_contents[docstring_end_index: docstring_end_line]
                 if extra_text and not extra_text.isspace():
                     raise ValueError(f'Error parsing {py_name}: extra text {extra_text!r} is on the line where the docstring ends. Move the extra text to a new line and try again.')
                 with open(py_path, 'w', newline=newline) as file:
-                    file.write(py_contents[:docstring_end_index])
-                    file.write('\n')
+                    file.write(py_contents[:docstring_end_index].rstrip())
+                    file.write('\n\n\n')
                     file.write(patch_py_contents)
-                    file.write(py_contents[docstring_end_index:])
+                    file.write('\n')
+                    file.write(py_contents[docstring_end_index:].lstrip())
 
         # verify that the file can be parsed properly
         with open(py_path) as file:
             try:
                 ast.parse(file.read())
             except SyntaxError:
                 raise ValueError(f'Error parsing {py_name}: Patch failed. This might occur if a node is split across multiple lines.')
@@ -544,30 +551,32 @@
             return
 
         # find dependencies
         dependency_paths = set()
         ignored_dll_names = set()
         not_found_dll_names = set()
         extension_module_paths = []
-        for root, _, filenames in os.walk(self._extract_dir):
+        for root, dirnames, filenames in os.walk(self._extract_dir):
+            if root == self._data_dir:
+                dirnames[:] = set(dirnames) & {'platlib', 'purelib'}
             for filename in filenames:
                 if filename.lower().endswith('.pyd'):
                     extension_module_path = os.path.join(root, filename)
                     extension_module_paths.append(extension_module_path)
-                    discovered, ignored, not_found = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'ignore', self._verbose)
+                    discovered, _, ignored, not_found = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'ignore', False, self._verbose)
                     dependency_paths |= discovered
                     ignored_dll_names |= ignored
                     not_found_dll_names |= not_found
 
         # find extra dependencies specified with --add-dll
         extra_dependency_paths = set()
         for dll_name in self._add_dlls:
-            path = _dll_utils.find_library(dll_name, None, self._arch)
-            if path:
-                extra_dependency_paths.add(path)
+            dll_info = _dll_utils.find_library(dll_name, None, self._arch, False)
+            if dll_info:
+                extra_dependency_paths.add(dll_info[0])
             else:
                 not_found_dll_names.add(dll_name)
 
         if self._ignore_in_wheel:
             dependency_paths_in_wheel, dependency_paths_outside_wheel = self._split_dependency_paths(dependency_paths)
             for path in dependency_paths_in_wheel.copy():
                 if os.path.basename(path).lower() in self._add_dlls:
@@ -606,57 +615,63 @@
             for ignored_dll_name in ignored_dll_names:
                 print(f'    {ignored_dll_name}')
         else:
             print('    None')
         if not_found_dll_names:
             print('\nWarning: At least one dependent DLL needs to be copied into the wheel but was not found.')
 
-    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str, no_diagnostic: bool, namespace_pkgs: typing.Set[typing.Tuple[str]]) -> None:
+    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str, no_diagnostic: bool, namespace_pkgs: typing.Set[typing.Tuple[str]], include_symbols: bool) -> None:
         """Repair the wheel in a manner similar to auditwheel.
         target is the target directory for storing the repaired wheel
         no_mangles is a set of lowercase DLL names that will not be mangled
         no_mangle_all is True if no DLL name mangling should happen at all
         strip is True if we should strip DLLs that contain trailing data when
             name-mangling
         lib_sdir is the suffix for the directory to store the DLLs
         no_diagnostic is True if no diagnostic information is written to the
             DELVEWHEEL metadata file
         namespace_pkgs is a set of paths, relative to the wheel root,
             corresponding to the namespace packages. Each path is represented
-            as a tuple of path components"""
+            as a tuple of path components
+        include_symbols is True if .pdb symbol files should be included with
+            the vendored DLLs"""
         print(f'repairing {self._whl_path}')
 
         # check whether wheel has already been repaired
         repair_version = self._get_repair_version()
         if repair_version:
             print(f'Delvewheel {repair_version} has already repaired this wheel.')
             return
 
         # find dependencies
         print('finding DLL dependencies')
         dependency_paths = set()
+        symbol_paths = set()
         ignored_dll_names = set()
         extension_module_paths = []
         has_top_level_ext_module = False
-        for root, _, filenames in os.walk(self._extract_dir):
+        for root, dirnames, filenames in os.walk(self._extract_dir):
+            if root == self._data_dir:
+                dirnames[:] = set(dirnames) & {'platlib', 'purelib'}
             for filename in filenames:
                 if filename.lower().endswith('.pyd'):
                     extension_module_path = os.path.join(root, filename)
                     dll_arch = _dll_utils.get_arch(extension_module_path)
                     if dll_arch != self._arch:
                         raise RuntimeError(f'{os.path.relpath(extension_module_path, self._extract_dir)} has a CPU architecture that is not compatible with this wheel')
                     if self._get_site_packages_relpath(root) == os.curdir:
                         if self._verbose >= 1:
                             print(f'analyzing top-level extension module {os.path.relpath(extension_module_path, self._extract_dir)}')
                         has_top_level_ext_module = True
                     elif self._verbose >= 1:
                         print(f'analyzing package-level extension module {os.path.relpath(extension_module_path, self._extract_dir)}')
                     extension_module_paths.append(extension_module_path)
-                    discovered, ignored = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'raise', self._verbose)[:2]
+                    discovered, symbols, ignored = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'raise', include_symbols, self._verbose)[:3]
                     dependency_paths |= discovered
+                    symbol_paths |= symbols
                     ignored_dll_names |= ignored
 
         # if --ignore-in-wheel is specified, ignore DLLs that were found inside
         # the wheel unless they are specified with --add-dll
         if self._ignore_in_wheel:
             dependency_paths_in_wheel, dependency_paths_outside_wheel = self._split_dependency_paths(dependency_paths)
             for p in dependency_paths_in_wheel:
@@ -671,17 +686,19 @@
         # been found
         dependency_names = {os.path.basename(p) for p in dependency_paths}  # this is NOT lowercased
         dependency_names_lower = {name.lower() for name in dependency_names}
         extra_dependency_paths = set()
         for dll_name in self._add_dlls:
             if dll_name in dependency_names_lower:
                 continue
-            path = _dll_utils.find_library(dll_name, None, self._arch)
-            if path:
-                extra_dependency_paths.add(path)
+            dll_info = _dll_utils.find_library(dll_name, None, self._arch, include_symbols)
+            if dll_info:
+                extra_dependency_paths.add(dll_info[0])
+                if dll_info[1]:
+                    symbol_paths.add(dll_info[1])
             else:
                 raise FileNotFoundError(f'{dll_name} not found')
         if not dependency_paths and not extra_dependency_paths:
             print('no external dependencies are needed')
             return
 
         # Warn if namespace package does not exist
@@ -715,14 +732,18 @@
             libs_dir = os.path.join(self._extract_dir, libs_dir_name)
         os.makedirs(libs_dir, exist_ok=True)
         print(f'copying DLLs into {os.path.relpath(libs_dir, self._extract_dir)}')
         for dependency_path in dependency_paths | extra_dependency_paths:
             if self._verbose >= 1:
                 print(f'copying {dependency_path} -> {os.path.join(libs_dir, os.path.basename(dependency_path))}')
             shutil.copy2(dependency_path, libs_dir)
+        for symbol_path in symbol_paths:
+            if self._verbose >= 1:
+                print(f'copying {symbol_path} -> {os.path.join(libs_dir, os.path.basename(symbol_path))}')
+            shutil.copy2(symbol_path, libs_dir)
 
         # mangle library names
         name_mangler = {}  # dict from lowercased old name to new name
         if no_mangle_all:
             print('skip mangling DLL names')
         else:
             print('mangling DLL names')
@@ -810,19 +831,19 @@
                 'modules into regular (non-namespace) packages.', UserWarning)
             dirnames = list(set(map(os.path.dirname, namespace_root_ext_modules)))
             dirnames.sort(key=self._namespace_pkg_sortkey)
             seen_relative = set()
             for dirname in dirnames:
                 dirname_relative = self._get_site_packages_relpath(dirname)
                 if dirname_relative not in seen_relative:
-                    for lib_name in os.listdir(libs_dir):
-                        lib_path = os.path.join(libs_dir, lib_name)
+                    for filename in os.listdir(libs_dir):
+                        filepath = os.path.join(libs_dir, filename)
                         if self._verbose >= 1:
-                            print(f'copying {lib_path} -> {os.path.join(dirname, lib_name)}')
-                        shutil.copy2(lib_path, dirname)
+                            print(f'copying {filepath} -> {os.path.join(dirname, filename)}')
+                        shutil.copy2(filepath, dirname)
                     seen_relative.add(dirname_relative)
 
         if load_order_filename is not None:
             # Create .load-order file containing list of DLLs to load during
             # import. Contrary to what the filename suggests, the DLLs are not
             # listed in any particular order. In an older version of
             # delvewheel, the DLLs needed to be listed in a particular order,
```

### Comparing `delvewheel-1.4.0/delvewheel.egg-info/PKG-INFO` & `delvewheel-1.5.0/delvewheel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.4.0
+Version: 1.5.0
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -85,21 +85,22 @@
 - `-v`: verbosity
   - `-v`: level 1, some diagnostic information
   - `-vv`: level 2, include warnings from `pefile`
 - `--extract-dir`: directory to store extracted contents of wheel for debug use (default is a temp directory)
 - `-w`,`--wheel-dir`: directory to write the repaired wheel (default is `wheelhouse` relative to current working directory)
 - `--no-mangle`: name(s) of DLL(s) not to mangle, path-separator-delimited
 - `--no-mangle-all`: don't mangle any DLL names
-- `--strip`: strip DLLs that contain trailing data when name-mangling. The GNU `strip` utility must be present in `PATH`.
+- `--strip`: strip DLLs that contain an overlay when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
 - `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
   - `--namespace-pkg package1` declares `package1` as a namespace package.
   - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
+- `--include-symbols`: include `.pdb` symbol files with the vendored DLLs. To be included, a symbol file must be in the same directory as the DLL and have the same filename before the extension, e.g. `example.dll` and `example.pdb`.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
-- To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
+- To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain an overlay at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, the overlay consists of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the overlay, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the overlay and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.4.0/setup.cfg` & `delvewheel-1.5.0/setup.cfg`

 * *Files identical despite different names*

