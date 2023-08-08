# Comparing `tmp/teneva_opti-0.3.6.tar.gz` & `tmp/teneva_opti-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_opti-0.3.6.tar", last modified: Mon Aug  7 08:36:35 2023, max compression
+gzip compressed data, was "teneva_opti-0.3.7.tar", last modified: Tue Aug  8 15:41:57 2023, max compression
```

## Comparing `teneva_opti-0.3.6.tar` & `teneva_opti-0.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-07 08:36:35.543649 teneva_opti-0.3.6/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.6/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.6/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3443 2023-08-07 08:36:35.543874 teneva_opti-0.3.6/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2168 2023-08-07 08:35:18.000000 teneva_opti-0.3.6/README.md
--rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-04 12:11:01.000000 teneva_opti-0.3.6/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      111 2023-08-07 08:33:40.000000 teneva_opti-0.3.6/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-07 08:36:35.544799 teneva_opti-0.3.6/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.6/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-07 08:36:35.532332 teneva_opti-0.3.6/teneva_opti/
--rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-07 08:35:12.000000 teneva_opti-0.3.6/teneva_opti/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     9976 2023-08-06 21:19:38.000000 teneva_opti-0.3.6/teneva_opti/bm_view.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-07 08:36:35.535166 teneva_opti-0.3.6/teneva_opti/func/
--rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.6/teneva_opti/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6846 2023-08-06 13:11:44.000000 teneva_opti-0.3.6/teneva_opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      171 2023-08-04 11:59:34.000000 teneva_opti-0.3.6/teneva_opti/opti_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     9169 2023-08-06 20:34:51.000000 teneva_opti-0.3.6/teneva_opti/opti_manager.py
--rw-r--r--   0 andrei     (501) staff       (20)     2359 2023-08-06 13:12:12.000000 teneva_opti-0.3.6/teneva_opti/opti_tens.py
--rw-r--r--   0 andrei     (501) staff       (20)     2282 2023-08-06 19:48:49.000000 teneva_opti-0.3.6/teneva_opti/plot.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-07 08:36:35.542857 teneva_opti-0.3.6/teneva_opti/tens/
--rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.6/teneva_opti/tens/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)     2393 2023-08-04 13:57:19.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1586 2023-08-04 13:43:52.000000 teneva_opti-0.3.6/teneva_opti/tens/opti_tens_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.6/teneva_opti/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-07 08:36:35.534834 teneva_opti-0.3.6/teneva_opti.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3443 2023-08-07 08:36:35.000000 teneva_opti-0.3.6/teneva_opti.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      783 2023-08-07 08:36:35.000000 teneva_opti-0.3.6/teneva_opti.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-07 08:36:35.000000 teneva_opti-0.3.6/teneva_opti.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      111 2023-08-07 08:36:35.000000 teneva_opti-0.3.6/teneva_opti.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-07 08:36:35.000000 teneva_opti-0.3.6/teneva_opti.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-08 15:41:57.292124 teneva_opti-0.3.7/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.7/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.7/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3443 2023-08-08 15:41:57.292428 teneva_opti-0.3.7/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2168 2023-08-08 15:36:23.000000 teneva_opti-0.3.7/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-04 12:11:01.000000 teneva_opti-0.3.7/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      111 2023-08-07 08:33:40.000000 teneva_opti-0.3.7/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-08 15:41:57.293340 teneva_opti-0.3.7/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.7/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-08 15:41:57.278659 teneva_opti-0.3.7/teneva_opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-08 15:36:34.000000 teneva_opti-0.3.7/teneva_opti/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)    10397 2023-08-08 10:30:07.000000 teneva_opti-0.3.7/teneva_opti/bm_view.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-08 15:41:57.282808 teneva_opti-0.3.7/teneva_opti/func/
+-rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.7/teneva_opti/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6846 2023-08-06 13:11:44.000000 teneva_opti-0.3.7/teneva_opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      171 2023-08-04 11:59:34.000000 teneva_opti-0.3.7/teneva_opti/opti_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     9422 2023-08-08 10:30:28.000000 teneva_opti-0.3.7/teneva_opti/opti_manager.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2359 2023-08-06 13:12:12.000000 teneva_opti-0.3.7/teneva_opti/opti_tens.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2356 2023-08-08 10:21:52.000000 teneva_opti-0.3.7/teneva_opti/plot.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-08 15:41:57.291250 teneva_opti-0.3.7/teneva_opti/tens/
+-rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.7/teneva_opti/tens/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2393 2023-08-04 13:57:19.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1586 2023-08-04 13:43:52.000000 teneva_opti-0.3.7/teneva_opti/tens/opti_tens_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.7/teneva_opti/utils.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-08 15:41:57.282241 teneva_opti-0.3.7/teneva_opti.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3443 2023-08-08 15:41:57.000000 teneva_opti-0.3.7/teneva_opti.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      783 2023-08-08 15:41:57.000000 teneva_opti-0.3.7/teneva_opti.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-08 15:41:57.000000 teneva_opti-0.3.7/teneva_opti.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      111 2023-08-08 15:41:57.000000 teneva_opti-0.3.7/teneva_opti.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-08 15:41:57.000000 teneva_opti-0.3.7/teneva_opti.egg-info/top_level.txt
```

### Comparing `teneva_opti-0.3.6/LICENSE.txt` & `teneva_opti-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/PKG-INFO` & `teneva_opti-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_opti
-Version: 0.3.6
+Version: 0.3.7
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -32,15 +32,15 @@
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_opti==0.3.6
+    pip install teneva_opti==0.3.7
     ```
     > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
 
 2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
     ```bash
     wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
     ```
```

### Comparing `teneva_opti-0.3.6/README.md` & `teneva_opti-0.3.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_opti==0.3.6
+    pip install teneva_opti==0.3.7
     ```
     > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
 
 2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
     ```bash
     wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
     ```
```

### Comparing `teneva_opti-0.3.6/demo.py` & `teneva_opti-0.3.7/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/setup.py` & `teneva_opti-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti/bm_view.py` & `teneva_opti-0.3.7/teneva_opti/bm_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         self.is_fail = True if self.op_history['err'] else False
 
         self.is_init = True
 
     def info_table(self, prec=2, value_best=None, kind='mean', is_time=False,
                    prefix='        & ', fail='FAIL', best_cmd='fat',
                    postfix='', prefix_comment_inner='%       > ',
-                   with_comment=True):
+                   with_comment=False):
         form = '{:-10.' + str(prec) + 'e}'
 
         if self.is_fail:
             v = fail
         else:
             v = self.get(kind, is_time)
             v = form.format(v).strip()
@@ -188,48 +188,59 @@
         if v == value_best and best_cmd:
             text += '\\' + best_cmd + '{'+ v + '}'
         else:
             text += v
 
         return text + postfix
 
-    def info_text(self, len_max=21):
+    def info_text(self, prec=5, prec_time=1, len_max=21):
         text = ''
         text += '\n' + self.info_text_bm(len_max)
         text += '\n' + self.info_text_op(len_max)
 
         task = 'max' if self.is_max else 'min'
 
+        form = '{:-14.' + str(prec) + 'e}'
+        form_time = '{:-.' + str(prec_time) + 'e}'
+
         if self.is_group:
             if self.is_fail:
                 text += '\n          ***FAIL***'
             else:
                 text += '\n'
                 text += '  > BEST >> '
-                text += f'{task}: {self.y_opt_best:-14.5e}   '
-                text += f'[time: {self.t_best:-8.1e}]'
+                v = form.format(self.y_opt_best)
+                text += f'{task}: {v}   '
+                v = form_time.format(self.t_best)
+                text += f'[time: {v}]'
 
                 text += '\n'
                 text += '  > MEAN >> '
-                text += f'{task}: {self.y_opt_mean:-14.5e}   '
-                text += f'[time: {self.t_mean:-8.1e}]'
+                v = form.format(self.y_opt_mean)
+                text += f'{task}: {v}   '
+                v = form_time.format(self.t_mean)
+                text += f'[time: {v}]'
 
                 text += '\n'
                 text += '  > WRST >> '
-                text += f'{task}: {self.y_opt_wrst:-14.5e}   '
-                text += f'[time: {self.t_wrst:-8.1e}]'
+                v = form.format(self.y_opt_wrst)
+                text += f'{task}: {v}   '
+                v = form_time.format(self.t_wrst)
+                text += f'[time: {v}]'
 
         else:
             text += '\n'
             text += '  >>>>>> '
             if self.is_fail:
                 text += ' ***FAIL***'
             else:
-                text += f'{task}: {self.y_opt:-14.5e}   '
-                text += f'[time: {self.t:-8.1e}]'
+                v = form.format(self.y_opt)
+                text += f'{task}: {v}   '
+                v = form_time.format(self.t)
+                text += f'[time: {v}]'
 
         return text
 
     def info_text_bm(self, len_max=21, with_prefix=True):
         text = ''
         name = self.bm_name[:(len_max-1)]
         if with_prefix:
@@ -310,16 +321,17 @@
             if bm1.op_opts[id] != bm2.op_opts[id]:
                 return False
 
         return True
 
     def values_to_one(self, y_lists, kind='mean'):
         res = []
-        lens = [len(y_list) for y_list in y_lists]
-        for k in range(max(lens)):
+        # lens = [len(y_list) for y_list in y_lists]
+        # for k in range(max(lens)):
+        for k in range(self.bm_config['budget_m']):
             vals = []
             for y_list in y_lists:
                 l = len(y_list)
                 vals.append(y_list[k] if l > k else y_list[l-1])
             if kind == 'best':
                 res.append(np.max(vals))
             elif kind == 'mean':
```

### Comparing `teneva_opti-0.3.6/teneva_opti/opti.py` & `teneva_opti-0.3.7/teneva_opti/opti.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti/opti_manager.py` & `teneva_opti-0.3.7/teneva_opti/opti_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.tasks = tasks
         self.fold = fold
         self.machine = machine
         self.is_show = is_show
 
         fname = 'log_manager_show' if self.is_show else 'log_manager'
         fpath = os.path.join(self.fold, fname)
-        self.log = Log(fpath)
+        self.log = Log(fpath, is_file_add=is_show)
 
         self.bms = []
 
     def build_args(self, args, bm):
         args['bm'] = args.get('bm', bm)
         args['fold'] = args.get('fold', self.fold)
         args['log'] = args.get('log', False)
@@ -152,15 +152,15 @@
                     raise ValueError('Invalid data')
                 if v != data['config'][id]:
                     raise ValueError('Invalid data')
 
         fold1 = self.fold
         for bm_name in os.listdir(fold1):
             fold2 = os.path.join(fold1, bm_name)
-            if os.path.isfile(fold2):
+            if  bm_name[0] == '_' or os.path.isfile(fold2):
                 continue
             fold3 = os.path.join(fold2, 'data')
             for bm_opts_str in os.listdir(fold3):
                 fold4 = os.path.join(fold3, bm_opts_str)
                 if os.path.isfile(fold4):
                     continue
                 for op_opts_str in os.listdir(fold4):
@@ -177,35 +177,14 @@
                         data['bm_opts'] = opts_str_to_dict(bm_opts_str)
                         data['op_opts'] = opts_str_to_dict(op_opts_str)
                         data['bm_name'] = bm_name
                         data['op_name'] = op_name
                         check(data)
                         self.bms.append(BmView(data))
 
-    def plot(self, fpath=None, name_map=None, name_spec=None, colors=None):
-        self.check_table()
-
-        if colors is None:
-            colors = [
-                '#000099', '#003300', '#FFF800', '#FFB300', '#CE0071',
-                '#333300', '#66ffcc', '#ff9999', '#cc0000', '#6699ff',
-                '#804000', '#cc6699', '#00B454', '#ff66ff', '#558000']
-
-        data = {}
-        for bm in self.bms:
-            name = name_map[bm.op_name] if name_map else bm.op_name
-            #print(name, len(bm.y_all_mean))
-            data[name] = {
-                'best': bm.y_all_best,
-                'mean': bm.y_all_mean,
-                'wrst': bm.y_all_wrst,
-                'skip': bm.is_fail}
-
-        plot_deps(data, colors, path(fpath, 'png'), name_spec)
-
     def run(self):
         for task in self.tasks:
             # Create Bm class instance:
             Bm = task['bm']
             args = task.get('bm_args', {})
             bm = Bm(**args)
             if 'bm_opts' in task:
@@ -229,33 +208,57 @@
 
             # Save the results:
             opti.save()
             if not opti.is_fail:
                 opti.render(with_wrn=False)
                 opti.show(with_wrn=False)
 
+    def show_plot(self, fpath=None, name_map=None, name_spec=None, colors=None,
+                  scale=1., lim_x=None, lim_y=None):
+        """This is draft!!!"""
+        self.check_table()
+
+        if colors is None:
+            colors = [
+                '#000099', '#FFB300', '#00B454', '#cc0000', '#cc6699',
+                '#804000', '#ff66ff', '#333300',
+                '#003300', '#FFF800', '#CE0071', '#333300', '#66ffcc',
+                '#ff9999', '#6699ff', '#804000', '#558000']
+
+        data = {}
+        for bm in self.bms:
+            name = name_map[bm.op_name] if name_map else bm.op_name
+            data[name] = {
+                'best': np.array(bm.y_all_best) / scale,
+                'mean': np.array(bm.y_all_mean) / scale,
+                'wrst': np.array(bm.y_all_wrst) / scale,
+                'skip': bm.is_fail}
+
+        plot_deps(data, colors, path(fpath, 'png'), name_spec,
+            lim_x=lim_x, lim_y=lim_y)
+
     def show_table(self, prefix='', postfix='', prec=2, kind='mean',
                    is_time=False, prefix_inner='        & ', fail='FAIL',
                    best_cmd='fat', postfix_inner='',
-                   prefix_comment_inner='%       > ', with_comment=True):
+                   prefix_comment_inner='%       > ', with_comment=False):
         self.check_table()
         value_best = self.get_best(kind, is_time)
 
         if prefix:
             self.log(prefix)
         for bm in self.bms:
             self.log(bm.info_table(prec, value_best, kind, is_time,
                 prefix_inner, fail, best_cmd, postfix_inner,
                 prefix_comment_inner, with_comment))
         if postfix:
             self.log(postfix)
 
-    def show_text(self):
+    def show_text(self, prec=5, prec_time=1):
         for bm in self.bms:
-            self.log(bm.info_text())
+            self.log(bm.info_text(prec, prec_time))
 
     def sort(self, arg='name', values=None, is_op=False):
         def sort(bm):
             config = getattr(bm, 'op_config' if is_op else 'bm_config', {})
             value = config.get(arg)
             if values is None:
                 return value
```

### Comparing `teneva_opti-0.3.6/teneva_opti/opti_tens.py` & `teneva_opti-0.3.7/teneva_opti/opti_tens.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti/plot.py` & `teneva_opti-0.3.7/teneva_opti/plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 sns.set_context('paper', font_scale=2.5)
 sns.set_style('white')
 sns.mpl.rcParams['legend.frameon'] = 'False'
 
 
 def plot_deps(data, colors, fpath=None, name_spec=None,
-              xlabel='Number of requests', ylabel=None, title=None):
+              xlabel='Number of requests', ylabel=None, title=None,
+              lim_x=None, lim_y=None):
+    """This is draft!!!"""
     fig, ax = plt.subplots(1, 1, figsize=(8, 8))
     plt.subplots_adjust(wspace=0.)
 
     if xlabel:
         ax.set_xlabel(xlabel)
     if ylabel:
         ax.set_ylabel(ylabel)
@@ -39,23 +41,25 @@
         if item.get('skip') == True:
             continue
 
         y = item['mean']
         y_best = np.array(item['best'])
         y_wrst = np.array(item['wrst'])
         x = np.arange(len(y))
-        linewidth = 3 if name_spec == name else 2
+        linewidth = 1 if name_spec == name else 1
         ax.plot(x, y, label=name, color=colors[i],
-            marker='o', markersize=4, linewidth=linewidth)
+            marker='o', markersize=0, linewidth=linewidth)
 
-        ax.fill_between(x, y_wrst, y_best, alpha=0.5, color=colors[i])
+        ax.fill_between(x, y_wrst, y_best, alpha=0.4, color=colors[i])
 
     _prep_ax(ax, xlog=True, ylog=False, leg=True)
-    # ax.set_xlim(m_min, 2.E+4)
-    # ax.set_ylim(plot_opts[bm]['y_min'], plot_opts[bm]['y_max'])
+    if lim_x is not None:
+        ax.set_xlim(*lim_x)
+    if lim_y is not None:
+        ax.set_ylim(*lim_y)
 
     #yticks = [1.8E+3, 2.0E+3, 2.2E+3, 2.4E+3, 2.6E+3, 2.8E+3, 3.0E+3, 3.2E+3]
     #ax.set(yticks=yticks, yticklabels=[int(])
     #ax.get_yaxis().get_major_formatter().labelOnlyBase = False
 
     if fpath:
         plt.savefig(fpath, bbox_inches='tight')
@@ -67,15 +71,15 @@
     if xlog:
         ax.semilogx()
     if ylog:
         ax.semilogy()
         ax.set_yscale('symlog')
 
     if leg:
-        ax.legend(loc='upper right', frameon=True)
+        ax.legend(loc='upper left', frameon=True)
 
     ax.grid(ls=":")
 
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
 
     ax.get_xaxis().tick_bottom()
```

### Comparing `teneva_opti-0.3.6/teneva_opti/tens/opti_tens_optimatt.py` & `teneva_opti-0.3.7/teneva_opti/tens/opti_tens_optimatt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti/tens/opti_tens_protes.py` & `teneva_opti-0.3.7/teneva_opti/tens/opti_tens_protes.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti/tens/opti_tens_ttopt.py` & `teneva_opti-0.3.7/teneva_opti/tens/opti_tens_ttopt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti/utils.py` & `teneva_opti-0.3.7/teneva_opti/utils.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.6/teneva_opti.egg-info/PKG-INFO` & `teneva_opti-0.3.7/teneva_opti.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-opti
-Version: 0.3.6
+Version: 0.3.7
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -32,15 +32,15 @@
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_opti==0.3.6
+    pip install teneva_opti==0.3.7
     ```
     > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
 
 2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
     ```bash
     wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
     ```
```

### Comparing `teneva_opti-0.3.6/teneva_opti.egg-info/SOURCES.txt` & `teneva_opti-0.3.7/teneva_opti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

