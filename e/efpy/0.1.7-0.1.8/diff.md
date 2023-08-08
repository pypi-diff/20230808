# Comparing `tmp/efpy-0.1.7.tar.gz` & `tmp/efpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efpy-0.1.7.tar", last modified: Thu Aug  3 14:06:54 2023, max compression
+gzip compressed data, was "efpy-0.1.8.tar", last modified: Tue Aug  8 05:40:45 2023, max compression
```

## Comparing `efpy-0.1.7.tar` & `efpy-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 14:06:54.763632 efpy-0.1.7/
--rw-rw-rw-   0        0        0      255 2023-08-03 14:06:54.763632 efpy-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 14:06:54.754687 efpy-0.1.7/efpy/
--rw-rw-rw-   0        0        0      868 2023-07-28 04:22:45.000000 efpy-0.1.7/efpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.7/efpy/env.py
--rw-rw-rw-   0        0        0     5068 2023-08-03 14:05:43.000000 efpy-0.1.7/efpy/expHelper.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:06:54.761638 efpy-0.1.7/efpy.egg-info/
--rw-rw-rw-   0        0        0      255 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 14:06:54.763632 efpy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-08-03 14:06:48.000000 efpy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 05:40:45.603865 efpy-0.1.8/
+-rw-rw-rw-   0        0        0      255 2023-08-08 05:40:45.603865 efpy-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-08 05:40:45.588211 efpy-0.1.8/efpy/
+-rw-rw-rw-   0        0        0      868 2023-07-28 04:22:45.000000 efpy-0.1.8/efpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.8/efpy/env.py
+-rw-rw-rw-   0        0        0     7185 2023-08-08 05:40:07.000000 efpy-0.1.8/efpy/expHelper.py
+drwxrwxrwx   0        0        0        0 2023-08-08 05:40:45.588211 efpy-0.1.8/efpy.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-08-08 05:40:45.000000 efpy-0.1.8/efpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-08-08 05:40:45.000000 efpy-0.1.8/efpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 05:40:45.000000 efpy-0.1.8/efpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 05:40:45.000000 efpy-0.1.8/efpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-08 05:40:45.000000 efpy-0.1.8/efpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 05:40:45.603865 efpy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-08-08 05:40:14.000000 efpy-0.1.8/setup.py
```

### Comparing `efpy-0.1.7/efpy/__init__.py` & `efpy-0.1.8/efpy/__init__.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.7/efpy/env.py` & `efpy-0.1.8/efpy/env.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.7/efpy/expHelper.py` & `efpy-0.1.8/efpy/expHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import yaml
 import re
 import copy
 import warnings
 
+
 def getYamlConfName(pyFileName):
     return pyFileName.split(".")[0] + ".config.yaml";
 
 
 def getSubExpId(pyFileName):
     pattern = r'^p\d+\.py$'
     if re.match(pattern, pyFileName):
@@ -70,41 +71,99 @@
     if activeDynamicYamlId < 0 or activeDynamicYamlId >= len(dyConfig):
         raise RuntimeError(
             f'activeBackgroundYamlId的范围错误，activeBackgroundYamlId = {activeDynamicYamlId}, 应该在[0, {len(dyConfig)}) 内')
         return None;
     dyConfig = dyConfig[activeDynamicYamlId]
     dictConv(theConfig, dyConfig)
     if isOptionParse:
-        theConfig=optionParse(theConfig)
+        theConfig = optionParse(theConfig)
     dictConv(theConfig, varSettings)
     return theConfig, varSettings
 
+
+def parseConfigRef(config):
+    config = copy.deepcopy(config)
+    while True:
+        isRef = {}
+        _buildRefAllowed(config, isRef, '');
+        (config, nSuc, nFail) = _configRefParse(config, config, '', isRef);
+        if nSuc == 0 and nFail == 0:
+            return config
+        if nSuc == 0 and nFail > 0:
+            raise SyntaxError(f'存在{nFail}个引用路径无法解析，请检查配置文件是否存在循环引用等问题！')
+    return config
+
+
+def _buildRefAllowed(config, isRef, path):
+    res = True
+    if isinstance(config, dict):
+        for key in config:
+            r1 = _buildRefAllowed(config[key], isRef, (path + '.' if path != "" else "") + key)
+            res = res and r1
+    elif isinstance(config, str) and config.startswith('?'):
+        res = False
+    isRef[path] = res
+    return res
+
+
+def _configRefParse(config, orgConfig, path, isRef):
+    nSuc = 0
+    nFail = 0
+    if isinstance(config, str) and config.startswith('?'):
+        refPath = config[1:]
+        if refPath in isRef:
+            if isRef[refPath]:
+                keys = refPath.split('.');
+                tmpConfig = orgConfig
+                for ks in keys:
+                    tmpConfig = tmpConfig[ks]
+                nSuc += 1
+                config = tmpConfig;
+            else:
+                nFail += 1
+        else:
+            raise SyntaxError(f'配置路径{path}不存在被引用路径{refPath}，引用无效！')
+        return (config, nSuc, nFail)
+    elif isinstance(config, dict):
+        for key in config:
+            (res, nSuc0, nFail0) = _configRefParse(config[key], orgConfig, (path + '.' if path != "" else "") + key,
+                                                   isRef)
+            config[key] = res
+            nSuc += nSuc0
+            nFail += nFail0
+    return (config, nSuc, nFail)
+
+
 def optionParse(config):
-    config=copy.deepcopy(config)
+    config = copy.deepcopy(config)
     while True:
-        (config,nSuc,nFail)=_optionParse(config, config,'');
-        if nSuc==0 and nFail==0:
+        (config, nSuc, nFail) = _optionParse(config, config, '');
+        if nSuc == 0 and nFail == 0:
             return config
-        if nSuc==0 and nFail>0:
+        if nSuc == 0 and nFail > 0:
             raise SyntaxError(f'存在{nFail}个引用路径为非字符串类型！')
     return config
 
+
 def _optionParse(config, orgConfig, path):
-    nSuc=0
-    nFail=0
+    nSuc = 0
+    nFail = 0
     if isinstance(config, dict):
         if '$' in config:
-            refPath=config['$']
+            if config['$'].startswith('?'):
+                refPath = config['$'][1:]
+            else:
+                raise SyntaxError(f'配置路径{path}下的属性$为"{config["$"]}"。它必须是一个引用（以?开头）！')
             keys = refPath.split('.');
-            tmpConfig=orgConfig
+            tmpConfig = orgConfig
             for ks in keys:
-                tmpConfig=tmpConfig[ks]
-            if not isinstance(tmpConfig,str):
-                nFail=1
-                return (config,nSuc,nFail)
+                tmpConfig = tmpConfig[ks]
+            if not isinstance(tmpConfig, str):
+                nFail = 1
+                return (config, nSuc, nFail)
 
             if tmpConfig in config:
                 nSuc = 1
                 return (config[tmpConfig], nSuc, nFail)
             else:
                 for key in config:
                     if re.match(key, tmpConfig):
@@ -114,22 +173,20 @@
                 if 'default' in config:
                     warnings.warn(f"配置路径{path}不存在关键词{tmpConfig}，但使用了default标签的内容！")
                     nSuc = 1
                     return (config['default'], nSuc, nFail)
                 raise SyntaxError(f'配置路径{path}不存在关键词{tmpConfig}，请检查{refPath}的值！')
 
         else:
-            nSuc=0
-            nFail=0
             for key in config:
-                (res,nSuc0,nFail0)=_optionParse(config[key],orgConfig, (path+'.' if path!="" else "")+key)
-                config[key]=res
-                nSuc+=nSuc0
-                nFail+=nFail0
-    return (config,nSuc,nFail)
+                (res, nSuc0, nFail0) = _optionParse(config[key], orgConfig, (path + '.' if path != "" else "") + key)
+                config[key] = res
+                nSuc += nSuc0
+                nFail += nFail0
+    return (config, nSuc, nFail)
 
 
 def loadSettingFromYamlSimple(backgroundYamlFile, varSettings={}):
     with open(backgroundYamlFile, 'r', encoding='utf-8') as c:
         defConfigs = list(yaml.load_all(c, Loader=yaml.FullLoader))
         theConfig = defConfigs[0]
     dictConv(theConfig, varSettings)
```

### Comparing `efpy-0.1.7/setup.py` & `efpy-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2023-4-29 07:13:42
 #############################################
 
 
 from setuptools import setup, find_packages
 #主要变量
 name="efpy"
-version = "0.1.7"
+version = "0.1.8"
 install_requires = ['PyYAML']
 
 setup(
     name = name,
     version = version,
     keywords = ("experience","environment"),
     description = "experience",
```

