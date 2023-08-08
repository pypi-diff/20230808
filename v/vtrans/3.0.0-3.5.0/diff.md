# Comparing `tmp/vtrans-3.0.0.tar.gz` & `tmp/vtrans-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtrans-3.0.0.tar", last modified: Wed May 31 08:27:12 2023, max compression
+gzip compressed data, was "vtrans-3.5.0.tar", last modified: Tue Aug  8 18:41:39 2023, max compression
```

## Comparing `vtrans-3.0.0.tar` & `vtrans-3.5.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 08:27:12.075964 vtrans-3.0.0/
--rw-rw-rw-   0        0        0       70 2023-05-31 08:23:56.000000 vtrans-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9224 2023-05-31 08:27:12.078961 vtrans-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8194 2023-05-31 08:05:03.000000 vtrans-3.0.0/README.md
--rw-rw-rw-   0        0        0      114 2023-05-31 08:27:12.086972 vtrans-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1332 2023-05-31 08:21:47.000000 vtrans-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 08:27:11.950773 vtrans-3.0.0/vtrans/
--rw-rw-rw-   0        0        0     9521 2023-05-31 07:01:44.000000 vtrans-3.0.0/vtrans/__init__.py
--rw-rw-rw-   0        0        0       58 2023-05-27 07:48:30.000000 vtrans-3.0.0/vtrans/config.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 08:27:12.064943 vtrans-3.0.0/vtrans.egg-info/
--rw-rw-rw-   0        0        0     9224 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 18:41:39.502603 vtrans-3.5.0/
+-rw-rw-rw-   0        0        0       70 2023-05-31 08:23:56.000000 vtrans-3.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9189 2023-08-08 18:41:39.502603 vtrans-3.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8194 2023-05-31 08:05:03.000000 vtrans-3.5.0/README.md
+-rw-rw-rw-   0        0        0      114 2023-08-08 18:41:39.504598 vtrans-3.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1311 2023-08-08 18:37:48.000000 vtrans-3.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:41:39.477670 vtrans-3.5.0/vtrans/
+-rw-rw-rw-   0        0        0     9727 2023-08-08 18:20:54.000000 vtrans-3.5.0/vtrans/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:41:39.500608 vtrans-3.5.0/vtrans.egg-info/
+-rw-rw-rw-   0        0        0     9189 2023-08-08 18:41:39.000000 vtrans-3.5.0/vtrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-08-08 18:41:39.000000 vtrans-3.5.0/vtrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:41:39.000000 vtrans-3.5.0/vtrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-08-08 18:41:39.000000 vtrans-3.5.0/vtrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 18:41:39.000000 vtrans-3.5.0/vtrans.egg-info/top_level.txt
```

### Comparing `vtrans-3.0.0/PKG-INFO` & `vtrans-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: vtrans
-Version: 3.0.0
-Summary: This is a self-updating translator for free and unlimited usage with upto 130 langauges
+Version: 3.5.0
+Summary: This is a cross-platfrom self-updating translator for free and unlimited usage with upto 130 langauges
 Home-page: https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans
 Author: S.Vigneswaran
 Author-email: t896242@gmail.com
 License: MIT
 Keywords: translator,googletranslate,self-updating,googletrans,vtrans
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Freeware
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vtrans-3.0.0/README.md` & `vtrans-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `vtrans-3.0.0/setup.py` & `vtrans-3.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from setuptools import setup, find_packages
 
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
   'Intended Audience :: End Users/Desktop',
   'License :: Freeware',
-  'Operating System :: MacOS :: MacOS X',
   'Topic :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'Operating System :: Microsoft :: Windows :: Windows 8.1',
   'Operating System :: Microsoft :: Windows :: Windows 8',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3.8'
 ]
 
 setup(
   name='vtrans',
-  version='3.0.0',
-  description='This is a self-updating translator for free and unlimited usage with upto 130 langauges',
+  version='3.5.0',
+  description='This is a cross-platfrom self-updating translator for free and unlimited usage with upto 130 langauges',
   long_description=open('README.md',"r",encoding="utf-8").read(),
   long_description_content_type='text/markdown',
   url='https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans',  
   author='S.Vigneswaran',
   author_email='t896242@gmail.com',
   license='MIT',
   classifiers=classifiers,
   keywords=['translator', 'googletranslate', 'self-updating', 'googletrans','vtrans'],
   packages=find_packages(),
   package_data={
         'vtrans': ['config.txt'],
     },
-  install_requires=['googletrans==3.1.0a0', 'pandas', 'requests', 'beautifulsoup4', 'astor'] 
+  install_requires=['googletrans==3.1.0a0', 'pandas', 'requests', 'beautifulsoup4', 'astor','lxml'] 
 )
```

### Comparing `vtrans-3.0.0/vtrans/__init__.py` & `vtrans-3.5.0/vtrans/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,25 @@
 
 import os
 
 """ This function is helps to set optional settings of this translator 
        
     it helps to disable the autoupdating"""
 def config(auto_updating='True'):
+    
+    """ This function is helps to set optional settings of this translator 
+       
+    it helps to disable the autoupdating"""
+
     #Convert auto_updating value to string
     auto_updating = str(auto_updating)
 
     #Get the current working interpreter site-packages to find the config file path
-    site_path = get_sitePackages_path()
-    config_path = site_path + "vtrans\\config.txt"
+    site_path   = get_sitePackages_path()
+    config_path = os.path.join(site_path,"vtrans","config.txt")
 
     #Open the config file
     with open(config_path,"r") as configfile:
         #Read the config file and evaluate that
         config_data = eval(configfile.read())
     
     #get the values of autoupdate and langauge_num
@@ -47,48 +52,48 @@
             print("Auto updating is turn enabled")
         elif auto_updating == 'False':
             print("Auto updating is disabled")
 
 def remove_unwanted_printing():
     data =check_con()
     sitep = get_sitePackages_path()
-    sitep = sitep + "vtrans\\config.txt"
+    sitep = os.path.join(sitep,"vtrans","config.txt")
     num_lang = data['original_lang']
     print_stat = data['print']
     auto_up = data['autoupdate']
     pattern = {'print':'False','autoupdate':auto_up,'original_lang':num_lang}
     with open(sitep,"w") as file:
         file.write(str(pattern))
 
 def enable_printing():
     data =check_con()
     sitep = get_sitePackages_path()
-    sitep = sitep + "vtrans\\config.txt"
+    sitep = os.path.join(sitep,"vtrans","config.txt")
     num_lang = data['original_lang']
     print_stat = data['print']
     auto_up = data['autoupdate']
     pattern = {'print':'True','autoupdate':auto_up,'original_lang':num_lang}
     with open(sitep,"w") as file:
         file.write(str(pattern))
 
 """  This function hels to find config data """
 def check_con():
     site_path = get_sitePackages_path()
-    config_path = site_path + "vtrans\\config.txt"
+    config_path = os.path.join(site_path,"vtrans","config.txt")
     with open(config_path,"r") as read_con:
         con_data = eval(read_con.read())
         return con_data
     
 """ This function gets the current working interpreter path  """
 def get_sitePackages_path():
     #importing site library
     import site
 
     #Site uses to  get current working interpreter path
-    site_packages_path = site.getsitepackages()[0] + "\Lib\\site-packages\\"
+    site_packages_path = site.getsitepackages()[1]
 
     #Return the path
     return site_packages_path
 
 """ This function used for checking updates on Google Translator updates by  Wikipedia article """
 def update_chacker():
     print("Checking for updates(auto updating).auto-updating make it slower.If you want to stop auto-updating, use this code: '''vtrans.config(auto_updating=False)'''")
@@ -144,15 +149,15 @@
         language = str(dictio['Language']).lower() # extract Language from that
         langcode = str(dictio['ISO-639 code'])     #Extract langaugecode from that
 
         language = language.lower() # Make langauge in lower case
         orginal_lang[langcode] = language #Add new key and value
     
     site_path = get_sitePackages_path() #Get site packages path
-    config_path = site_path + "Vtrans\\config.txt" #and add confg file path
+    config_path = os.path.join(site_path,"vtrans","config.txt") #and add confg file path
 
     with open(config_path,"r") as configfile:  #OPEN CONFIG FILE
         config_data = eval(configfile.read()) #read config file and eval it
 
     autoup_config = config_data['autoupdate'] #get autoupdate value
     prin = config_data['print']
 
@@ -177,15 +182,15 @@
             for indlangcode in langcode: #use for loop to get langcode one by one
                 lang_with_langcode[indlangcode] = language #add new key and values
             
         else:
             lang_with_langcode[str(langcode[0])] = language #if the langcode have only language codes add langcode list first value as new key and set new value  
 
     constant_path = get_sitePackages_path() #get site-packages path
-    constant_path = constant_path + "googletrans\\constants.py" #add constant.py file path
+    constant_path = os.path.join(constant_path,"googletrans","constants.py") #add constant.py file path
 
     print(f"Total languages: {len(lang_with_langcode)}") #print how many langauges have updated version
     
     with open(constant_path, "r") as lang_config: #open constants.py 
         tree = ast.parse(lang_config.read()) #read file
     
     #Change LANGAUGES dictionary values with the new dictionary
@@ -205,15 +210,15 @@
     print("Update finished. Now you can use extra languages.")
 
 def ready(data):
     if data['print'] == 'True':
         print("ready to translate")
 
 confile_path = get_sitePackages_path()
-confile_path = confile_path + "vtrans\\config.txt"
+confile_path = os.path.join(confile_path,"vtrans","config.txt")
 if os.path.isfile(confile_path):
     file_vai = "ok"
 else:
     print("setup config file")
     pattern = {'print':'True','autoupdate':'True','original_lang':'107'}
     with open(confile_path,'w') as new_file:
         new_file.write(str(pattern))
```

### Comparing `vtrans-3.0.0/vtrans.egg-info/PKG-INFO` & `vtrans-3.5.0/vtrans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: vtrans
-Version: 3.0.0
-Summary: This is a self-updating translator for free and unlimited usage with upto 130 langauges
+Version: 3.5.0
+Summary: This is a cross-platfrom self-updating translator for free and unlimited usage with upto 130 langauges
 Home-page: https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans
 Author: S.Vigneswaran
 Author-email: t896242@gmail.com
 License: MIT
 Keywords: translator,googletranslate,self-updating,googletrans,vtrans
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Freeware
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

