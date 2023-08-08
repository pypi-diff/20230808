# Comparing `tmp/mydb_tsm-1.0.tar.gz` & `tmp/mydb_tsm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mydb_tsm-1.0.tar", last modified: Mon Aug  7 16:04:01 2023, max compression
+gzip compressed data, was "mydb_tsm-1.0.1.tar", last modified: Tue Aug  8 12:54:09 2023, max compression
```

## Comparing `mydb_tsm-1.0.tar` & `mydb_tsm-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 16:04:01.758561 mydb_tsm-1.0/
--rw-rw-rw-   0        0        0     1398 2023-08-07 16:04:01.758561 mydb_tsm-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2023-08-07 14:11:52.000000 mydb_tsm-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 16:04:01.748068 mydb_tsm-1.0/mydb_tsm/
--rw-rw-rw-   0        0        0        0 2023-08-07 13:45:30.000000 mydb_tsm-1.0/mydb_tsm/__init__.py
--rw-rw-rw-   0        0        0     6248 2023-08-07 13:57:48.000000 mydb_tsm-1.0/mydb_tsm/mydb_tsm.py
--rw-rw-rw-   0        0        0     7522 2023-08-07 13:28:05.000000 mydb_tsm-1.0/mydb_tsm/test.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:04:01.755754 mydb_tsm-1.0/mydb_tsm.egg-info/
--rw-rw-rw-   0        0        0     1398 2023-08-07 16:04:01.000000 mydb_tsm-1.0/mydb_tsm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-08-07 16:04:01.000000 mydb_tsm-1.0/mydb_tsm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 16:04:01.000000 mydb_tsm-1.0/mydb_tsm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 16:04:01.000000 mydb_tsm-1.0/mydb_tsm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 16:04:01.759839 mydb_tsm-1.0/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-08-07 15:49:06.000000 mydb_tsm-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:54:09.757519 mydb_tsm-1.0.1/
+-rw-rw-rw-   0        0        0     1400 2023-08-08 12:54:09.757519 mydb_tsm-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2023-08-07 14:11:52.000000 mydb_tsm-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 12:54:09.747044 mydb_tsm-1.0.1/mydb_tsm/
+-rw-rw-rw-   0        0        0        0 2023-08-07 13:45:30.000000 mydb_tsm-1.0.1/mydb_tsm/__init__.py
+-rw-rw-rw-   0        0        0     6305 2023-08-08 12:52:24.000000 mydb_tsm-1.0.1/mydb_tsm/mydb_tsm.py
+-rw-rw-rw-   0        0        0     7522 2023-08-07 13:28:05.000000 mydb_tsm-1.0.1/mydb_tsm/test.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:54:09.755271 mydb_tsm-1.0.1/mydb_tsm.egg-info/
+-rw-rw-rw-   0        0        0     1400 2023-08-08 12:54:09.000000 mydb_tsm-1.0.1/mydb_tsm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-08-08 12:54:09.000000 mydb_tsm-1.0.1/mydb_tsm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 12:54:09.000000 mydb_tsm-1.0.1/mydb_tsm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 12:54:09.000000 mydb_tsm-1.0.1/mydb_tsm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 12:54:09.757519 mydb_tsm-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-08-08 12:29:51.000000 mydb_tsm-1.0.1/setup.py
```

### Comparing `mydb_tsm-1.0/PKG-INFO` & `mydb_tsm-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mydb_tsm
-Version: 1.0
+Version: 1.0.1
 Author: Tomboy
 Author-email: Tomboy1996@163.com
 Description-Content-Type: text/markdown
 
 ## description
     这是第一个对外发布的模块，基于pymysql1.1.0进行的封装。
     功能：报错后自动关闭sql连接，py编写sql更友好。
```

### Comparing `mydb_tsm-1.0/README.md` & `mydb_tsm-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mydb_tsm-1.0/mydb_tsm/mydb_tsm.py` & `mydb_tsm-1.0.1/mydb_tsm/mydb_tsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,18 @@
     def close(self) -> None:
         """
         关闭数据库资源
         :return: None
         """
         if self.cur:
             self.cur.close()
+            self.cur = None
         if self.conn:
             self.conn.close()
+            self.conn = None
 
     @commit
     def create_db(self, db_name: str, character="utf8mb4", collate="utf8mb4_unicode_ci") -> None:
         """
         创建数据库
         :param db_name: 数据库名称
         :param character: 字符集
@@ -183,8 +185,8 @@
         'host': '192.168.93.131',
         'port': 3306,
         'user': 'root',
         'password': 'Tomboy_test',
     }
 
     db = DBUtil(config)
-    db.create_db('mydb_tsm')
+    db.create_db('db_tsm')
```

### Comparing `mydb_tsm-1.0/mydb_tsm/test.py` & `mydb_tsm-1.0.1/mydb_tsm/test.py`

 * *Files identical despite different names*

### Comparing `mydb_tsm-1.0/mydb_tsm.egg-info/PKG-INFO` & `mydb_tsm-1.0.1/mydb_tsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mydb-tsm
-Version: 1.0
+Version: 1.0.1
 Author: Tomboy
 Author-email: Tomboy1996@163.com
 Description-Content-Type: text/markdown
 
 ## description
     这是第一个对外发布的模块，基于pymysql1.1.0进行的封装。
     功能：报错后自动关闭sql连接，py编写sql更友好。
```

### Comparing `mydb_tsm-1.0/setup.py` & `mydb_tsm-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='mydb_tsm',  # 对外我们模块的名字
-    version='1.0',  # 版本号
+    version='1.0.1',  # 版本号
     long_description=long_description,  # 包的描述
     long_description_content_type='text/markdown',  # 包描述的类型
     author='Tomboy',  # 作者
     author_email='Tomboy1996@163.com',  # 作者邮箱
     py_modules=['mydb_tsm.mydb_tsm', 'mydb_tsm.test'],  # 要发布的模块
 )
```

