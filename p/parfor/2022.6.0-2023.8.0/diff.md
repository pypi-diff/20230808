# Comparing `tmp/parfor-2022.6.0.tar.gz` & `tmp/parfor-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parfor-2022.6.0.tar", last modified: Tue Jun 28 09:09:18 2022, max compression
+gzip compressed data, was "parfor-2023.8.0.tar", max compression
```

## Comparing `parfor-2022.6.0.tar` & `parfor-2023.8.0.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-06-28 09:09:18.318216 parfor-2022.6.0/
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)    35128 2021-03-19 08:42:10.000000 parfor-2022.6.0/LICENSE
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     5850 2022-06-28 09:09:18.318216 parfor-2022.6.0/PKG-INFO
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     5380 2022-05-03 13:56:13.000000 parfor-2022.6.0/README.md
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-06-28 09:09:18.318216 parfor-2022.6.0/parfor/
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)    23173 2022-06-28 08:56:45.000000 parfor-2022.6.0/parfor/__init__.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     3681 2022-05-03 12:47:13.000000 parfor-2022.6.0/parfor/pickler.py
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-06-28 09:09:18.318216 parfor-2022.6.0/parfor.egg-info/
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     5850 2022-06-28 09:09:17.000000 parfor-2022.6.0/parfor.egg-info/PKG-INFO
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      212 2022-06-28 09:09:18.000000 parfor-2022.6.0/parfor.egg-info/SOURCES.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)        1 2022-06-28 09:09:17.000000 parfor-2022.6.0/parfor.egg-info/dependency_links.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)       32 2022-06-28 09:09:18.000000 parfor-2022.6.0/parfor.egg-info/requires.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)        7 2022-06-28 09:09:18.000000 parfor-2022.6.0/parfor.egg-info/top_level.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)       38 2022-06-28 09:09:18.318216 parfor-2022.6.0/setup.cfg
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      750 2022-06-28 09:01:22.000000 parfor-2022.6.0/setup.py
+-rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2023.8.0/LICENSE
+-rw-r--r--   0        0        0     5380 2022-05-03 13:56:13.252950 parfor-2023.8.0/README.md
+-rw-r--r--   0        0        0    23167 2023-08-08 12:13:01.704434 parfor-2023.8.0/parfor/__init__.py
+-rw-r--r--   0        0        0     3681 2022-05-03 12:47:13.994545 parfor-2023.8.0/parfor/pickler.py
+-rw-r--r--   0        0        0      604 2023-08-08 12:59:59.173918 parfor-2023.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 parfor-2023.8.0/PKG-INFO
```

### Comparing `parfor-2022.6.0/LICENSE` & `parfor-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parfor-2022.6.0/PKG-INFO` & `parfor-2023.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: parfor
-Version: 2022.6.0
-Summary: A package to mimic the use of parfor as done in Matlab.
-Home-page: https://github.com/wimpomp/parfor
-Author: Wim Pomp
-Author-email: wimpomp@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Parfor
 Used to parallelize for-loops using parfor in Matlab? This package allows you to do the same in python.
 Take any normal serial but parallelizable for-loop and execute it in parallel using easy syntax.
 Don't worry about the technical details of using the multiprocessing module, race conditions, queues,
 parfor handles all that. 
 
 Tested on linux on python 2.7 and 3.8 and on Windows and OSX on python 3.8.
```

### Comparing `parfor-2022.6.0/README.md` & `parfor-2023.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: parfor
+Version: 2023.8.0
+Summary: A package to mimic the use of parfor as done in Matlab.
+Home-page: https://gitlab.rhpc.nki.nl/LenstraLab/LiveCellAnalysis
+License: GPLv3
+Keywords: parfor,concurrency,multiprocessing,parallel
+Author: Wim Pomp
+Author-email: wimpomp@gmail.com
+Requires-Python: >=3.5,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: test
+Requires-Dist: dill (>=0.3.0)
+Requires-Dist: psutil
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: tqdm (>=4.50.0)
+Project-URL: Repository, https://gitlab.rhpc.nki.nl/LenstraLab/LiveCellAnalysis
+Description-Content-Type: text/markdown
+
 # Parfor
 Used to parallelize for-loops using parfor in Matlab? This package allows you to do the same in python.
 Take any normal serial but parallelizable for-loop and execute it in parallel using easy syntax.
 Don't worry about the technical details of using the multiprocessing module, race conditions, queues,
 parfor handles all that. 
 
 Tested on linux on python 2.7 and 3.8 and on Windows and OSX on python 3.8.
@@ -160,7 +187,8 @@
 ## Parpool
 More low-level accessibility to parallel execution. Submit tasks and request the result at any time,
 (although necessarily submit first, then request a specific task), use different functions and function
 arguments for different tasks.
 
 ## TqdmMeter
 Meter bar, inherited from tqdm, used for displaying buffers.
+
```

### Comparing `parfor-2022.6.0/parfor/__init__.py` & `parfor-2023.8.0/parfor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import multiprocessing
 from os import getpid
 from tqdm.auto import tqdm
 from traceback import format_exc
 from psutil import Process
 from collections import OrderedDict
 from warnings import warn
+from functools import wraps
 from .pickler import Pickler, dumps, loads
 
 
 try:
     from javabridge import kill_vm
 except ImportError:
     kill_vm = lambda: None
@@ -19,64 +20,60 @@
 
 class Chunks:
     """ Yield successive chunks from lists.
         Usage: chunks(list0, list1, ...)
                chunks(list0, list1, ..., size=s)
                chunks(list0, list1, ..., number=n)
                chunks(list0, list1, ..., ratio=r)
-        size:   size of chunks, might change to optimize devision between chunks
+        size:   size of chunks, might change to optimize division between chunks
         number: number of chunks, coerced to 1 <= n <= len(list0)
         ratio:  number of chunks / number of cpus, coerced to 1 <= n <= len(list0)
         both size and number or ratio are given: use number or ratio, unless the chunk size would be bigger than size
         both ratio and number are given: use ratio
     """
 
-    def __init__(self, *args, size=None, number=None, ratio=None, length=None, s=None, n=None, r=None):
+    def __init__(self, *iterators, size=None, number=None, ratio=None, length=None, s=None, n=None, r=None):
         # s, r and n are deprecated
         if s is not None:
+            warn('parfor: use of \'s\' is deprecated, use \'size\' instead', DeprecationWarning, stacklevel=2)
             size = s
         if n is not None:
+            warn('parfor: use of \'n\' is deprecated, use \'number\' instead', DeprecationWarning, stacklevel=2)
             number = n
         if r is not None:
+            warn('parfor: use of \'r\' is deprecated, use \'ratio\' instead', DeprecationWarning, stacklevel=2)
             ratio = r
         if length is None:
             try:
-                length = min(*[len(a) for a in args]) if len(args) > 1 else len(args[0])
+                length = min(*[len(iterator) for iterator in iterators]) if len(iterators) > 1 else len(iterators[0])
             except TypeError:
-                raise TypeError('Cannot determine the length of the argument so the length must be provided as an'
+                raise TypeError('Cannot determine the length of the iterator(s), so the length must be provided as an'
                                 ' argument.')
         if size is not None and (number is not None or ratio is not None):
             if number is None:
                 number = int(cpu_count * ratio)
             if length >= size * number:
                 number = round(length / size)
         elif size is not None:  # size of chunks
             number = round(length / size)
         elif ratio is not None:  # number of chunks
             number = int(cpu_count * ratio)
-        self.args = args
+        self.iterators = [iter(arg) for arg in iterators]
         self.number_of_items = length
         self.length = max(1, min(length, number))
         self.lengths = [((i + 1) * self.number_of_items // self.length) - (i * self.number_of_items // self.length)
                         for i in range(self.length)]
 
     def __iter__(self):
         for i in range(self.length):
             p, q = (i * self.number_of_items // self.length), ((i + 1) * self.number_of_items // self.length)
-            if len(self.args) == 1:
-                yield self._yielder(self.args[0], p, q)
+            if len(self.iterators) == 1:
+                yield [next(self.iterators[0]) for _ in range(q - p)]
             else:
-                yield [self._yielder(arg, p, q) for arg in self.args]
-
-    @staticmethod
-    def _yielder(arg, p, q):
-        try:
-            return arg[p:q]
-        except TypeError:
-            return [next(arg) for _ in range(q-p)]
+                yield [[next(iterator) for _ in range(q-p)] for iterator in self.iterators]
 
     def __len__(self):
         return self.length
 
 
 class ExternalBar:
     def __init__(self, iterable=None, callback=None, total=0):
@@ -144,100 +141,14 @@
 
     def __exit__(self, exc_type=None, exc_value=None, traceback=None):
         if not self.leave:
             self.n = self.total
         super().__exit__(exc_type, exc_value, traceback)
 
 
-def parfor(*args, **kwargs):
-    """ @parfor(iterator=None, args=(), kwargs={}, length=None, desc=None, bar=True, qbar=True, rP=1/3, serial=4):
-        decorator to parallize for-loops
-
-        required arguments:
-            fun:    function taking arguments: iteration from  iterable, other arguments defined in args & kwargs
-            iterable: iterable from which an item is given to fun as a first argument
-
-        optional arguments:
-            args:   tuple with other unnamed arguments to fun
-            kwargs: dict with other named arguments to fun
-            length: give the length of the iterator in cases where len(iterator) results in an error
-            desc:   string with description of the progress bar
-            bar:    bool enable progress bar, or a function taking the number of passed iterations as an argument
-            pbar:   bool enable buffer indicator bar, or a function taking the queue size as an argument
-            rP:     ratio workers to cpu cores, default: 1
-            nP:     number of workers, default: None, overrides rP if not None
-                number of workers will always be at least 2
-            serial: execute in series instead of parallel if True, None (default): let parfor decide
-
-        output:       list with results from applying the decorated function to each iteration of the iterator
-                      specified as the first argument to the function
-
-        examples:
-            << from time import sleep
-
-            <<
-            @parfor(range(10), (3,))
-            def fun(i, a):
-                sleep(1)
-                return a*i**2
-            fun
-
-            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
-
-            <<
-            @parfor(range(10), (3,), bar=False)
-            def fun(i, a):
-                sleep(1)
-                return a*i**2
-            fun
-
-            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
-
-            <<
-            def fun(i, a):
-                sleep(1)
-                return a*i**2
-            pmap(fun, range(10), (3,))
-
-            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
-
-            equivalent to using the deco module:
-            <<
-            @concurrent
-            def fun(i, a):
-                time.sleep(1)
-                return a*i**2
-
-            @synchronized
-            def run(iterator, a):
-                res = []
-                for i in iterator:
-                    res.append(fun(i, a))
-                return res
-
-            run(range(10), 3)
-
-            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
-
-            all equivalent to the serial for-loop:
-            <<
-            a = 3
-            fun = []
-            for i in range(10):
-                sleep(1)
-                fun.append(a*i**2)
-            fun
-
-            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
-        """
-    def decfun(fun):
-        return pmap(fun, *args, **kwargs)
-    return decfun
-
-
 class Hasher:
     def __init__(self, obj, hsh=None):
         if hsh is not None:
             self.obj, self.str, self.hash = None, obj, hsh
         elif isinstance(obj, Hasher):
             self.obj, self.str, self.hash = obj.obj, obj.str, obj.hash
         else:
@@ -384,15 +295,15 @@
                 if task.pid is not None and task.pid not in [child.pid for child in Process().children()]:
                     self.queue_in.put(task)
                     warn('Task {} was restarted because process {} was probably killed.'.format(task.handle, task.pid))
             return False
 
     def error(self, error):
         self.close()
-        raise Exception('Error occured in worker: {}'.format(error))
+        raise Exception('Error occurred in worker: {}'.format(error))
 
     def task_error(self, handle, error):
         if handle in self:
             task = self.tasks[handle]
             print('Error from process working on iteration {}:\n'.format(handle))
             print(error)
             self.close()
@@ -561,62 +472,142 @@
             kill_vm()
             if terminator is not None:
                 terminator()
             with self.n_tasks.get_lock():
                 self.n_tasks.value -= 1
 
 
-def pmap(fun, iterable=None, args=None, kwargs=None, length=None, desc=None, bar=True, qbar=False, terminator=None,
-         rP=1, nP=None, serial=None, qsize=None):
+def pmap(fun, iterable=None, args=None, kwargs=None, total=None, desc=None, bar=True, qbar=False, terminator=None,
+         rP=1, nP=None, serial=None, qsize=None, length=None, **bar_kwargs):
     """ map a function fun to each iteration in iterable
-            best use: iterable is a generator and length is given to this function
+        use as a function: pmap
+        use as a decorator: parfor
+        best use: iterable is a generator and length is given to this function as 'total'
+
+        required:
+            fun:    function taking arguments: iteration from  iterable, other arguments defined in args & kwargs
+            iterable: iterable or iterator from which an item is given to fun as a first argument
+        optional:
+            args:   tuple with other unnamed arguments to fun
+            kwargs: dict with other named arguments to fun
+            total:  give the length of the iterator in cases where len(iterator) results in an error
+            desc:   string with description of the progress bar
+            bar:    bool enable progress bar,
+                        or a callback function taking the number of passed iterations as an argument
+            pbar:   bool enable buffer indicator bar, or a callback function taking the queue size as an argument
+            terminator: function which is executed in each worker after all the work is done
+            rP:     ratio workers to cpu cores, default: 1
+            nP:     number of workers, default, None, overrides rP if not None
+            serial: execute in series instead of parallel if True, None (default): let pmap decide
+            qsize:  maximum size of the task queue
+            length: deprecated alias for total
+            **bar_kwargs: keywords arguments for tqdm.tqdm
+
+        output:
+            list with results from applying the function \'fun\' to each iteration of the iterable / iterator
 
-        fun:    function taking arguments: iteration from  iterable, other arguments defined in args & kwargs
-        iterable: iterable from which an item is given to fun as a first argument
-        args:   tuple with other unnamed arguments to fun
-        kwargs: dict with other named arguments to fun
-        length: give the length of the iterator in cases where len(iterator) results in an error
-        desc:   string with description of the progress bar
-        bar:    bool enable progress bar, or a callback function taking the number of passed iterations as an argument
-        pbar:   bool enable buffer indicator bar, or a callback function taking the queue size as an argument
-        terminator: function which is executed in each worker after all the work is done
-        rP:     ratio workers to cpu cores, default: 1
-        nP:     number of workers, default, None, overrides rP if not None
-        serial: execute in series instead of parallel if True, None (default): let pmap decide
+        examples:
+            << from time import sleep
+            <<
+            @parfor(range(10), (3,))
+            def fun(i, a):
+                sleep(1)
+                return a * i ** 2
+            fun
+            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
+
+            <<
+            def fun(i, a):
+                sleep(1)
+                return a * i ** 2
+            pmap(fun, range(10), (3,))
+            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
+
+            equivalent to using the deco module:
+            <<
+            @concurrent
+            def fun(i, a):
+                time.sleep(1)
+                return a * i ** 2
+
+            @synchronized
+            def run(iterator, a):
+                res = []
+                for i in iterator:
+                    res.append(fun(i, a))
+                return res
+            run(range(10), 3)
+            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
+
+            all equivalent to the serial for-loop:
+            <<
+            a = 3
+            fun = []
+            for i in range(10):
+                sleep(1)
+                fun.append(a * i ** 2)
+            fun
+            >> [0, 3, 12, 27, 48, 75, 108, 147, 192, 243]
     """
+    if total is None and length is not None:
+        total = length
+        warn('parfor: use of \'length\' is deprecated, use \'total\' instead', DeprecationWarning, stacklevel=2)
     is_chunked = isinstance(iterable, Chunks)
     if is_chunked:
         chunk_fun = fun
     else:
-        iterable = Chunks(iterable, ratio=5, length=length)
+        iterable = Chunks(iterable, ratio=5, length=total)
+
         def chunk_fun(iterator, *args, **kwargs):
             return [fun(i, *args, **kwargs) for i in iterator]
 
     args = args or ()
     kwargs = kwargs or {}
 
-    length = sum(iterable.lengths)
+    if 'total' not in bar_kwargs:
+        bar_kwargs['total'] = sum(iterable.lengths)
+    if 'desc' not in bar_kwargs:
+        bar_kwargs['desc'] = desc
+    if 'disable' not in bar_kwargs:
+        bar_kwargs['disable'] = not bar
     if serial is True or (serial is None and len(iterable) < min(cpu_count, 4)):  # serial case
         if callable(bar):
             return sum([chunk_fun(c, *args, **kwargs) for c in ExternalBar(iterable, bar)], [])
         else:
-            return sum([chunk_fun(c, *args, **kwargs)
-                        for c in tqdm(iterable, total=len(iterable), desc=desc, disable=not bar)], [])
-    else:                           # parallel case
+            return sum([chunk_fun(c, *args, **kwargs) for c in tqdm(iterable, **bar_kwargs)], [])
+    else:   # parallel case
         with ExternalBar(callback=qbar) if callable(qbar) \
                 else TqdmMeter(total=0, desc='Task buffer', disable=not qbar, leave=False) as qbar, \
-             ExternalBar(callback=bar) if callable(bar) else tqdm(total=length, desc=desc, disable=not bar) as bar:
+             ExternalBar(callback=bar) if callable(bar) else tqdm(**bar_kwargs) as bar:
             with Parpool(chunk_fun, args, kwargs, rP, nP, bar, qbar, terminator, qsize) as p:
                 for i, (j, l) in enumerate(zip(iterable, iterable.lengths)):  # add work to the queue
                     p(j, handle=i, barlength=iterable.lengths[i])
                     if bar.total is None or bar.total < i+1:
                         bar.total = i+1
                 if is_chunked:
                     return [p[i] for i in range(len(iterable))]
                 else:
                     return sum([p[i] for i in range(len(iterable))], [])  # collect the results
 
 
+@wraps(pmap)
+def parfor(*args, **kwargs):
+    def decfun(fun):
+        return pmap(fun, *args, **kwargs)
+    return decfun
+
+
+def deprecated(cls, name):
+    """ This is a decorator which can be used to mark functions and classes as deprecated. It will result in a warning
+        being emitted when the function or class is used."""
+    @wraps(cls)
+    def wrapper(*args, **kwargs):
+        warn(f'parfor: use of \'{name}\' is deprecated, use \'{cls.__name__}\' instead',
+             category=DeprecationWarning, stacklevel=2)
+        return cls(*args, **kwargs)
+    return wrapper
+
+
 # backwards compatibility
-parpool = Parpool
-tqdmm = TqdmMeter
-chunks = Chunks
+parpool = deprecated(Parpool, 'parpool')
+tqdmm = deprecated(TqdmMeter, 'tqdmm')
+chunks = deprecated(Chunks, 'chunks')
```

### Comparing `parfor-2022.6.0/parfor/pickler.py` & `parfor-2023.8.0/parfor/pickler.py`

 * *Files identical despite different names*

