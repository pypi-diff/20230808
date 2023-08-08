# Comparing `tmp/scPANTHEON-0.3.9.3.tar.gz` & `tmp/scPANTHEON-0.3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scPANTHEON-0.3.9.3.tar", last modified: Fri Aug  4 13:22:06 2023, max compression
+gzip compressed data, was "dist\scPANTHEON-0.3.9.4.tar", last modified: Tue Aug  8 06:28:33 2023, max compression
```

## Comparing `scPANTHEON-0.3.9.3.tar` & `scPANTHEON-0.3.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      290 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.3/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.3/scpantheon/app/__init__.py
--rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.3/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/scpantheon/front_end/
--rw-rw-rw-   0        0        0     6887 2023-08-04 12:24:07.000000 scPANTHEON-0.3.9.3/scpantheon/front_end/R_data_qt.py
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.3/scpantheon/front_end/__init__.py
--rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.3/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.3/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1363 2023-08-04 11:26:27.000000 scPANTHEON-0.3.9.3/scpantheon/main.py
--rw-rw-rw-   0        0        0    66286 2023-08-04 12:36:11.000000 scPANTHEON-0.3.9.3/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2023-08-04 13:22:06.000000 scPANTHEON-0.3.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-08-04 13:21:47.000000 scPANTHEON-0.3.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.4/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.4/scpantheon/app/__init__.py
+-rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.4/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/scpantheon/front_end/
+-rw-rw-rw-   0        0        0     6920 2023-08-08 06:23:48.000000 scPANTHEON-0.3.9.4/scpantheon/front_end/R_data_qt.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.4/scpantheon/front_end/__init__.py
+-rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.4/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.4/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1363 2023-08-04 11:26:27.000000 scPANTHEON-0.3.9.4/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66286 2023-08-04 12:36:11.000000 scPANTHEON-0.3.9.4/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 06:28:33.000000 scPANTHEON-0.3.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-08-08 06:28:30.000000 scPANTHEON-0.3.9.4/setup.py
```

### Comparing `scPANTHEON-0.3.9.3/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.3.9.4/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.3/scpantheon/front_end/R_data_qt.py` & `scPANTHEON-0.3.9.4/scpantheon/front_end/R_data_qt.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,47 +37,47 @@
         self.btn_RNA_folder.clicked.connect(self.slot_RNA_folder)
         self.btn_RNA_folder.setFont(font)
         self.btn_RNA_folder.setMinimumSize(750, 100)
         # self.btn_Extensions.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         # file1
         self.btn_ADT_file = QPushButton("ADT_file",self)  
-        self.btn_ADT_file.setObjectName("btn_Data")  
+        self.btn_ADT_file.setObjectName("btn_ADT_file")  
         self.btn_ADT_file.clicked.connect(self.slot_ADT_file)
         self.btn_ADT_file.setFont(font)
         self.btn_ADT_file.setMinimumSize(750, 100)
         # self.btn_Data.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         # file2
         self.btn_Droplet_file = QPushButton("Droplet_file",self)  
-        self.btn_Droplet_file.setObjectName("btn_Data")  
+        self.btn_Droplet_file.setObjectName("btn_Droplet_file")  
         self.btn_Droplet_file.clicked.connect(self.slot_Droplet_file)
         self.btn_Droplet_file.setFont(font)
         self.btn_Droplet_file.setMinimumSize(750, 100)
 
-        # Start scpantheon
-        self.btn_Start = QPushButton("Start",self)
-        self.btn_Start.setObjectName("btn_Start")
-        self.btn_Start.clicked.connect(lambda : self.rejected(Dialog))
-        self.btn_Start.setFont(font)
-        self.btn_Start.setMinimumSize(750, 100)
+        # folder
+        self.btn_RNA_folder = QPushButton("RNA_folder",self)
+        self.btn_RNA_folder.setObjectName("btn_RNA_folder")
+        self.btn_RNA_folder.clicked.connect(self.slot_RNA_folder)
+        self.btn_RNA_folder.setFont(font)
+        self.btn_RNA_folder.setMinimumSize(750, 100)
         # self.btn_Start.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         self.layout1 = QVBoxLayout()
         self.layout2 = QVBoxLayout(Dialog)
         self.layout2.setObjectName("Layout2")    
         self.layout2.addWidget(self.text_brow)             
 
         self.buttonBox = QDialogButtonBox(Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
         self.buttonBox.setObjectName("buttonBox")
         self.layout2.addWidget(self.buttonBox)
 
-        self.layout2.addWidget(self.btn_Extensions)
-        self.layout2.addWidget(self.btn_Data)
+        self.layout2.addWidget(self.btn_ADT_file)
+        self.layout2.addWidget(self.btn_Droplet_file)
         self.layout2.addWidget(self.btn_Start)
 
         # self.retranslateUi(Dialog) 
         # self.buttonBox.accepted.connect(self.accepted)
         self.buttonBox.rejected.connect(self.rejected)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
```

### Comparing `scPANTHEON-0.3.9.3/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.3.9.4/scpantheon/front_end/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.3/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.3.9.4/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.3/scpantheon/main.py` & `scPANTHEON-0.3.9.4/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.3/scpantheon/source.py` & `scPANTHEON-0.3.9.4/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.3/setup.py` & `scPANTHEON-0.3.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.9.3',#版本
+    version='0.3.9.4',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs','rpy2'], # 依赖包,如果没有,可以不要
```

