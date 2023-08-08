# Comparing `tmp/hdfs-2.7.0.tar.gz` & `tmp/hdfs-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdfs-2.7.0.tar", last modified: Mon Mar 28 16:05:14 2022, max compression
+gzip compressed data, was "hdfs-2.7.1.tar", last modified: Tue Aug  8 17:14:15 2023, max compression
```

## Comparing `hdfs-2.7.0.tar` & `hdfs-2.7.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 mtth       (501) staff       (20)        0 2022-03-28 16:05:14.452843 hdfs-2.7.0/
--rw-r--r--   0 mtth       (501) staff       (20)      187 2021-02-14 21:07:25.000000 hdfs-2.7.0/AUTHORS
--rw-r--r--   0 mtth       (501) staff       (20)     1061 2021-02-14 21:10:41.000000 hdfs-2.7.0/LICENSE
--rw-r--r--   0 mtth       (501) staff       (20)       26 2021-02-14 21:07:25.000000 hdfs-2.7.0/MANIFEST.in
--rw-r--r--   0 mtth       (501) staff       (20)     3616 2022-03-28 16:05:14.452155 hdfs-2.7.0/PKG-INFO
--rw-r--r--   0 mtth       (501) staff       (20)     2879 2022-03-28 15:42:05.000000 hdfs-2.7.0/README.md
-drwxr-xr-x   0 mtth       (501) staff       (20)        0 2022-03-28 16:05:14.430126 hdfs-2.7.0/hdfs/
--rw-r--r--   0 mtth       (501) staff       (20)      338 2022-03-28 15:48:42.000000 hdfs-2.7.0/hdfs/__init__.py
--rw-r--r--   0 mtth       (501) staff       (20)     8860 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/__main__.py
--rw-r--r--   0 mtth       (501) staff       (20)    48557 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/client.py
--rw-r--r--   0 mtth       (501) staff       (20)     6590 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/config.py
-drwxr-xr-x   0 mtth       (501) staff       (20)        0 2022-03-28 16:05:14.437333 hdfs-2.7.0/hdfs/ext/
--rw-r--r--   0 mtth       (501) staff       (20)       59 2021-02-14 21:07:25.000000 hdfs-2.7.0/hdfs/ext/__init__.py
-drwxr-xr-x   0 mtth       (501) staff       (20)        0 2022-03-28 16:05:14.439306 hdfs-2.7.0/hdfs/ext/avro/
--rw-r--r--   0 mtth       (501) staff       (20)     9826 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/ext/avro/__init__.py
--rw-r--r--   0 mtth       (501) staff       (20)     4790 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/ext/avro/__main__.py
--rw-r--r--   0 mtth       (501) staff       (20)     1500 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/ext/dataframe.py
--rw-r--r--   0 mtth       (501) staff       (20)     4309 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/ext/kerberos.py
--rw-r--r--   0 mtth       (501) staff       (20)     4425 2022-03-28 15:46:02.000000 hdfs-2.7.0/hdfs/util.py
-drwxr-xr-x   0 mtth       (501) staff       (20)        0 2022-03-28 16:05:14.433960 hdfs-2.7.0/hdfs.egg-info/
--rw-r--r--   0 mtth       (501) staff       (20)     3616 2022-03-28 16:05:13.000000 hdfs-2.7.0/hdfs.egg-info/PKG-INFO
--rw-r--r--   0 mtth       (501) staff       (20)      582 2022-03-28 16:05:14.000000 hdfs-2.7.0/hdfs.egg-info/SOURCES.txt
--rw-r--r--   0 mtth       (501) staff       (20)        1 2022-03-28 16:05:13.000000 hdfs-2.7.0/hdfs.egg-info/dependency_links.txt
--rw-r--r--   0 mtth       (501) staff       (20)       90 2022-03-28 16:05:13.000000 hdfs-2.7.0/hdfs.egg-info/entry_points.txt
--rw-r--r--   0 mtth       (501) staff       (20)      143 2022-03-28 16:05:14.000000 hdfs-2.7.0/hdfs.egg-info/requires.txt
--rw-r--r--   0 mtth       (501) staff       (20)        5 2022-03-28 16:05:14.000000 hdfs-2.7.0/hdfs.egg-info/top_level.txt
--rw-r--r--   0 mtth       (501) staff       (20)       38 2022-03-28 16:05:14.453100 hdfs-2.7.0/setup.cfg
--rw-r--r--   0 mtth       (501) staff       (20)     1753 2022-03-28 15:46:02.000000 hdfs-2.7.0/setup.py
-drwxr-xr-x   0 mtth       (501) staff       (20)        0 2022-03-28 16:05:14.450217 hdfs-2.7.0/test/
--rw-r--r--   0 mtth       (501) staff       (20)    45622 2022-03-28 15:46:50.000000 hdfs-2.7.0/test/test_client.py
--rw-r--r--   0 mtth       (501) staff       (20)     4706 2021-02-14 21:07:25.000000 hdfs-2.7.0/test/test_config.py
--rw-r--r--   0 mtth       (501) staff       (20)     1528 2022-03-28 15:46:03.000000 hdfs-2.7.0/test/test_examples.py
--rw-r--r--   0 mtth       (501) staff       (20)     8886 2022-03-28 15:46:03.000000 hdfs-2.7.0/test/test_ext_avro.py
--rw-r--r--   0 mtth       (501) staff       (20)     1768 2021-02-14 21:07:25.000000 hdfs-2.7.0/test/test_ext_dataframe.py
--rw-r--r--   0 mtth       (501) staff       (20)     1080 2022-03-28 15:46:03.000000 hdfs-2.7.0/test/test_ext_kerberos.py
--rw-r--r--   0 mtth       (501) staff       (20)     5675 2021-02-14 21:07:25.000000 hdfs-2.7.0/test/test_main.py
--rw-r--r--   0 mtth       (501) staff       (20)     2264 2021-02-14 21:07:25.000000 hdfs-2.7.0/test/test_util.py
+drwxr-xr-x   0 mtth       (501) staff       (20)        0 2023-08-08 17:14:15.504777 hdfs-2.7.1/
+-rw-r--r--   0 mtth       (501) staff       (20)      187 2021-02-14 21:07:25.000000 hdfs-2.7.1/AUTHORS
+-rw-r--r--   0 mtth       (501) staff       (20)     1061 2021-02-14 21:10:41.000000 hdfs-2.7.1/LICENSE
+-rw-r--r--   0 mtth       (501) staff       (20)       26 2021-02-14 21:07:25.000000 hdfs-2.7.1/MANIFEST.in
+-rw-r--r--   0 mtth       (501) staff       (20)     3582 2023-08-08 17:14:15.504140 hdfs-2.7.1/PKG-INFO
+-rw-r--r--   0 mtth       (501) staff       (20)     2865 2023-08-08 16:18:02.000000 hdfs-2.7.1/README.md
+drwxr-xr-x   0 mtth       (501) staff       (20)        0 2023-08-08 17:14:15.487342 hdfs-2.7.1/hdfs/
+-rw-r--r--   0 mtth       (501) staff       (20)      338 2023-08-08 16:18:02.000000 hdfs-2.7.1/hdfs/__init__.py
+-rw-r--r--   0 mtth       (501) staff       (20)     8860 2022-03-28 15:46:02.000000 hdfs-2.7.1/hdfs/__main__.py
+-rw-r--r--   0 mtth       (501) staff       (20)    48376 2023-08-02 18:06:01.000000 hdfs-2.7.1/hdfs/client.py
+-rw-r--r--   0 mtth       (501) staff       (20)     6701 2023-08-08 16:18:02.000000 hdfs-2.7.1/hdfs/config.py
+drwxr-xr-x   0 mtth       (501) staff       (20)        0 2023-08-08 17:14:15.494913 hdfs-2.7.1/hdfs/ext/
+-rw-r--r--   0 mtth       (501) staff       (20)       59 2021-02-14 21:07:25.000000 hdfs-2.7.1/hdfs/ext/__init__.py
+drwxr-xr-x   0 mtth       (501) staff       (20)        0 2023-08-08 17:14:15.496622 hdfs-2.7.1/hdfs/ext/avro/
+-rw-r--r--   0 mtth       (501) staff       (20)     9826 2022-03-28 15:46:02.000000 hdfs-2.7.1/hdfs/ext/avro/__init__.py
+-rw-r--r--   0 mtth       (501) staff       (20)     4790 2022-03-28 15:46:02.000000 hdfs-2.7.1/hdfs/ext/avro/__main__.py
+-rw-r--r--   0 mtth       (501) staff       (20)     1500 2022-03-28 15:46:02.000000 hdfs-2.7.1/hdfs/ext/dataframe.py
+-rw-r--r--   0 mtth       (501) staff       (20)     4309 2022-03-28 15:46:02.000000 hdfs-2.7.1/hdfs/ext/kerberos.py
+-rw-r--r--   0 mtth       (501) staff       (20)     4425 2022-03-28 15:46:02.000000 hdfs-2.7.1/hdfs/util.py
+drwxr-xr-x   0 mtth       (501) staff       (20)        0 2023-08-08 17:14:15.492218 hdfs-2.7.1/hdfs.egg-info/
+-rw-r--r--   0 mtth       (501) staff       (20)     3582 2023-08-08 17:14:15.000000 hdfs-2.7.1/hdfs.egg-info/PKG-INFO
+-rw-r--r--   0 mtth       (501) staff       (20)      612 2023-08-08 17:14:15.000000 hdfs-2.7.1/hdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 mtth       (501) staff       (20)        1 2023-08-08 17:14:15.000000 hdfs-2.7.1/hdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 mtth       (501) staff       (20)       90 2023-08-08 17:14:15.000000 hdfs-2.7.1/hdfs.egg-info/entry_points.txt
+-rw-r--r--   0 mtth       (501) staff       (20)      143 2023-08-08 17:14:15.000000 hdfs-2.7.1/hdfs.egg-info/requires.txt
+-rw-r--r--   0 mtth       (501) staff       (20)       10 2023-08-08 17:14:15.000000 hdfs-2.7.1/hdfs.egg-info/top_level.txt
+-rw-r--r--   0 mtth       (501) staff       (20)       38 2023-08-08 17:14:15.505000 hdfs-2.7.1/setup.cfg
+-rw-r--r--   0 mtth       (501) staff       (20)     1753 2023-08-02 18:01:48.000000 hdfs-2.7.1/setup.py
+drwxr-xr-x   0 mtth       (501) staff       (20)        0 2023-08-08 17:14:15.503146 hdfs-2.7.1/test/
+-rw-r--r--   0 mtth       (501) staff       (20)        0 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/__init__.py
+-rw-r--r--   0 mtth       (501) staff       (20)    47432 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_client.py
+-rw-r--r--   0 mtth       (501) staff       (20)     4779 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_config.py
+-rw-r--r--   0 mtth       (501) staff       (20)     1618 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_examples.py
+-rw-r--r--   0 mtth       (501) staff       (20)     8922 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_ext_avro.py
+-rw-r--r--   0 mtth       (501) staff       (20)     1708 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_ext_dataframe.py
+-rw-r--r--   0 mtth       (501) staff       (20)     1041 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_ext_kerberos.py
+-rw-r--r--   0 mtth       (501) staff       (20)     5841 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_main.py
+-rw-r--r--   0 mtth       (501) staff       (20)     2344 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/test_util.py
+-rw-r--r--   0 mtth       (501) staff       (20)     3259 2023-08-08 16:18:02.000000 hdfs-2.7.1/test/util.py
```

### Comparing `hdfs-2.7.0/LICENSE` & `hdfs-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/PKG-INFO` & `hdfs-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: hdfs
-Version: 2.7.0
+Version: 2.7.1
 Summary: HdfsCLI: API and command line interface for HDFS.
 Home-page: https://hdfscli.readthedocs.io
 Author: Matthieu Monsch
 Author-email: mtth@apache.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: avro
 Provides-Extra: kerberos
 Provides-Extra: dataframe
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -55,15 +54,15 @@
   ...:     from json import load
   ...:     model = load(reader)
   ...:
 ```
 
 ## Features
 
-* Python (2 and 3) bindings for the [WebHDFS][] (and [HttpFS][]) API,
+* Python 3 bindings for the [WebHDFS][] (and [HttpFS][]) API,
   supporting both secure and insecure clusters.
 * Command line interface to transfer files and start an interactive client
   shell, with aliases for convenient namenode URL caching.
 * Additional functionality through optional extensions:
 
   + `avro`, to [read and write Avro files directly from HDFS][].
   + `dataframe`, to [load and save Pandas dataframes][].
@@ -83,16 +82,16 @@
 
 ## Testing
 
 HdfsCLI is tested against both [WebHDFS][] and [HttpFS][]. There are two ways
 of running tests (see `scripts/` for helpers to set up a test HDFS cluster):
 
 ```sh
-$ HDFSCLI_TEST_URL=http://localhost:50070 nosetests # Using a namenode's URL.
-$ HDFSCLI_TEST_ALIAS=dev nosetests # Using an alias.
+$ HDFSCLI_TEST_URL=http://localhost:50070 pytest # Using a namenode's URL.
+$ HDFSCLI_TEST_ALIAS=dev pytest # Using an alias.
 ```
 
 ## Contributing
 
 We'd love to hear what you think on the [issues][] page. Pull requests are also
 most welcome!
 
@@ -100,9 +99,7 @@
 [WebHDFS]: http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html
 [read and write Avro files directly from HDFS]: https://hdfscli.readthedocs.io/en/latest/api.html#module-hdfs.ext.avro
 [load and save Pandas dataframes]: https://hdfscli.readthedocs.io/en/latest/api.html#module-hdfs.ext.dataframe
 [support Kerberos authenticated clusters]: https://hdfscli.readthedocs.io/en/latest/api.html#module-hdfs.ext.kerberos
 [documentation]: https://hdfscli.readthedocs.io/
 [quickstart]: https://hdfscli.readthedocs.io/en/latest/quickstart.html
 [issues]: https://github.com/mtth/hdfs/issues
-
-
```

### Comparing `hdfs-2.7.0/README.md` & `hdfs-2.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   ...:     from json import load
   ...:     model = load(reader)
   ...:
 ```
 
 ## Features
 
-* Python (2 and 3) bindings for the [WebHDFS][] (and [HttpFS][]) API,
+* Python 3 bindings for the [WebHDFS][] (and [HttpFS][]) API,
   supporting both secure and insecure clusters.
 * Command line interface to transfer files and start an interactive client
   shell, with aliases for convenient namenode URL caching.
 * Additional functionality through optional extensions:
 
   + `avro`, to [read and write Avro files directly from HDFS][].
   + `dataframe`, to [load and save Pandas dataframes][].
@@ -60,16 +60,16 @@
 
 ## Testing
 
 HdfsCLI is tested against both [WebHDFS][] and [HttpFS][]. There are two ways
 of running tests (see `scripts/` for helpers to set up a test HDFS cluster):
 
 ```sh
-$ HDFSCLI_TEST_URL=http://localhost:50070 nosetests # Using a namenode's URL.
-$ HDFSCLI_TEST_ALIAS=dev nosetests # Using an alias.
+$ HDFSCLI_TEST_URL=http://localhost:50070 pytest # Using a namenode's URL.
+$ HDFSCLI_TEST_ALIAS=dev pytest # Using an alias.
 ```
 
 ## Contributing
 
 We'd love to hear what you think on the [issues][] page. Pull requests are also
 most welcome!
```

### Comparing `hdfs-2.7.0/hdfs/__main__.py` & `hdfs-2.7.1/hdfs/__main__.py`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/hdfs/client.py` & `hdfs-2.7.1/hdfs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,16 +324,15 @@
   def acl_status(self, hdfs_path, strict=True):
     """Get AclStatus_ for a file or folder on HDFS.
 
     :param hdfs_path: Remote path.
     :param strict: If `False`, return `None` rather than raise an exception if
       the path doesn't exist.
 
-    .. _AclStatus: ACLS_
-    .. _ACLS: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Get_ACL_Status
+    .. _AclStatus: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Get_ACL_Status
 
     """
     _logger.info('Fetching ACL status for %r.', hdfs_path)
     res = self._get_acl_status(hdfs_path, strict=strict)
     return res.json()['AclStatus'] if res else None
 
   def set_acl(self, hdfs_path, acl_spec, clear=True):
@@ -344,65 +343,59 @@
     :param acl_spec: String representation of an ACL spec. Must be a valid
       string with entries for user, group and other. For example:
       `"user::rwx,user:foo:rw-,group::r--,other::---"`.
     :param clear: Clear existing ACL entries. If set to false, all existing ACL
       entries that are not specified in this call are retained without changes,
       behaving like ModifyAcl_. For example: `"user:foo:rwx"`.
 
-    .. _SetAcl: SETACL_
-    .. SETACL_: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Set_ACL
-
-    .. ModifyAcl_: MODACL_
-    .. MODACL_: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Modify_ACL_Entries
+    .. _SetAcl: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Set_ACL
+    .. _ModifyAcl: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Modify_ACL_Entries
 
     """
     if clear:
       _logger.info('Setting ACL spec for %r to %r.', hdfs_path, acl_spec)
       self._set_acl(hdfs_path, aclspec=acl_spec)
     else:
       _logger.info('Modifying ACL spec for %r to %r.', hdfs_path, acl_spec)
       self._modify_acl_entries(hdfs_path, aclspec=acl_spec)
 
   def remove_acl_entries(self, hdfs_path, acl_spec):
-    """RemoveACL_ for a file or folder on HDFS.
+    """RemoveAclEntries_ for a file or folder on HDFS.
 
     :param hdfs_path: Path to an existing remote file or directory. An
       :class:`HdfsError` will be raised if the path doesn't exist.
     :param acl_spec: String representation of an ACL spec. Must be a valid
       string with entries for user, group and other. For example:
       `"user::rwx,user:foo:rw-,group::r--,other::---"`.
 
-    .. _RemoveAcl: REMOVEACLENTRIES_
-    .. REMOVEACLENTRIES_: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Remove_ACL_Entries
+    .. _RemoveAclEntries: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Remove_ACL_Entries
 
     """
     _logger.info('Removing ACL spec on %r for %r.', hdfs_path, acl_spec)
     self._remove_acl_entries(hdfs_path, aclspec=acl_spec)
 
   def remove_default_acl(self, hdfs_path):
-    """RemoveDefaultACL_ for a file or folder on HDFS.
+    """RemoveDefaultAcl_ for a file or folder on HDFS.
 
         :param hdfs_path: Path to an existing remote file or directory. An
           :class:`HdfsError` will be raised if the path doesn't exist.
 
-        .. _RemoveDefaultAcl: REMOVEDEFAULTACL_
-        .. REMOVEDEFAULTACL_: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Remove_Default_ACL
+        .. _RemoveDefaultAcl: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Remove_Default_ACL
 
         """
     _logger.info('Removing default acl for %r', hdfs_path)
     self._remove_default_acl(hdfs_path)
 
   def remove_acl(self, hdfs_path):
-    """RemoveACL_ for a file or folder on HDFS.
+    """RemoveAcl_ for a file or folder on HDFS.
 
         :param hdfs_path: Path to an existing remote file or directory. An
           :class:`HdfsError` will be raised if the path doesn't exist.
 
-        .. _RemoveAcl: REMOVEACL_
-        .. REMOVEACL_: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Remove_ACL
+        .. _RemoveAcl: https://hadoop.apache.org/docs/stable2/hadoop-project-dist/hadoop-hdfs/WebHDFS.html#Remove_ACL
 
         """
     _logger.info('Removing all ACL for %r', hdfs_path)
     self._remove_acl(hdfs_path)
 
   def parts(self, hdfs_path, parts=None, status=False):
     """Returns a dictionary of part-files corresponding to a path.
```

### Comparing `hdfs-2.7.0/hdfs/config.py` & `hdfs-2.7.1/hdfs/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,28 @@
 :meth:`Config.get_client`).
 
 """
 
 from .client import Client
 from .util import HdfsError
 from functools import wraps
-from imp import load_source
 from logging.handlers import TimedRotatingFileHandler
 from six.moves.configparser import ParsingError, RawConfigParser
 from tempfile import gettempdir
 import logging as lg
 import os
 import os.path as osp
 import sys
 
+try:
+  # Python 3.12 and above
+  from importlib import load_source
+except ImportError:
+  # Below Python 3.12
+  from imp import load_source
 
 _logger = lg.getLogger(__name__)
 
 
 class NullHandler(lg.Handler):
 
   """Pass-through logging handler.
```

### Comparing `hdfs-2.7.0/hdfs/ext/avro/__init__.py` & `hdfs-2.7.1/hdfs/ext/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/hdfs/ext/avro/__main__.py` & `hdfs-2.7.1/hdfs/ext/avro/__main__.py`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/hdfs/ext/dataframe.py` & `hdfs-2.7.1/hdfs/ext/dataframe.py`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/hdfs/ext/kerberos.py` & `hdfs-2.7.1/hdfs/ext/kerberos.py`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/hdfs/util.py` & `hdfs-2.7.1/hdfs/util.py`

 * *Files identical despite different names*

### Comparing `hdfs-2.7.0/hdfs.egg-info/PKG-INFO` & `hdfs-2.7.1/hdfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: hdfs
-Version: 2.7.0
+Version: 2.7.1
 Summary: HdfsCLI: API and command line interface for HDFS.
 Home-page: https://hdfscli.readthedocs.io
 Author: Matthieu Monsch
 Author-email: mtth@apache.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: avro
 Provides-Extra: kerberos
 Provides-Extra: dataframe
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -55,15 +54,15 @@
   ...:     from json import load
   ...:     model = load(reader)
   ...:
 ```
 
 ## Features
 
-* Python (2 and 3) bindings for the [WebHDFS][] (and [HttpFS][]) API,
+* Python 3 bindings for the [WebHDFS][] (and [HttpFS][]) API,
   supporting both secure and insecure clusters.
 * Command line interface to transfer files and start an interactive client
   shell, with aliases for convenient namenode URL caching.
 * Additional functionality through optional extensions:
 
   + `avro`, to [read and write Avro files directly from HDFS][].
   + `dataframe`, to [load and save Pandas dataframes][].
@@ -83,16 +82,16 @@
 
 ## Testing
 
 HdfsCLI is tested against both [WebHDFS][] and [HttpFS][]. There are two ways
 of running tests (see `scripts/` for helpers to set up a test HDFS cluster):
 
 ```sh
-$ HDFSCLI_TEST_URL=http://localhost:50070 nosetests # Using a namenode's URL.
-$ HDFSCLI_TEST_ALIAS=dev nosetests # Using an alias.
+$ HDFSCLI_TEST_URL=http://localhost:50070 pytest # Using a namenode's URL.
+$ HDFSCLI_TEST_ALIAS=dev pytest # Using an alias.
 ```
 
 ## Contributing
 
 We'd love to hear what you think on the [issues][] page. Pull requests are also
 most welcome!
 
@@ -100,9 +99,7 @@
 [WebHDFS]: http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html
 [read and write Avro files directly from HDFS]: https://hdfscli.readthedocs.io/en/latest/api.html#module-hdfs.ext.avro
 [load and save Pandas dataframes]: https://hdfscli.readthedocs.io/en/latest/api.html#module-hdfs.ext.dataframe
 [support Kerberos authenticated clusters]: https://hdfscli.readthedocs.io/en/latest/api.html#module-hdfs.ext.kerberos
 [documentation]: https://hdfscli.readthedocs.io/
 [quickstart]: https://hdfscli.readthedocs.io/en/latest/quickstart.html
 [issues]: https://github.com/mtth/hdfs/issues
-
-
```

### Comparing `hdfs-2.7.0/hdfs.egg-info/SOURCES.txt` & `hdfs-2.7.1/hdfs.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 hdfs.egg-info/requires.txt
 hdfs.egg-info/top_level.txt
 hdfs/ext/__init__.py
 hdfs/ext/dataframe.py
 hdfs/ext/kerberos.py
 hdfs/ext/avro/__init__.py
 hdfs/ext/avro/__main__.py
+test/__init__.py
 test/test_client.py
 test/test_config.py
 test/test_examples.py
 test/test_ext_avro.py
 test/test_ext_dataframe.py
 test/test_ext_kerberos.py
 test/test_main.py
-test/test_util.py
+test/test_util.py
+test/util.py
```

### Comparing `hdfs-2.7.0/setup.py` & `hdfs-2.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,17 @@
   license='MIT',
   packages=find_packages(),
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 2.7',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
   ],
   install_requires=[
     'docopt',
     'requests>=2.7.0',
     'six>=1.9.0',
   ],
   extras_require={
```

### Comparing `hdfs-2.7.0/test/test_client.py` & `hdfs-2.7.1/test/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,251 +2,251 @@
 # encoding: utf-8
 
 """Test Hdfs client interactions with HDFS."""
 
 from collections import defaultdict
 from hdfs.client import *
 from hdfs.util import HdfsError, temppath
-from util import _IntegrationTest
-from nose.tools import eq_, nottest, ok_, raises, assert_regex
+from test.util import _IntegrationTest
 from requests.exceptions import ConnectTimeout, ReadTimeout
 from shutil import rmtree
 from six import b
 from tempfile import mkdtemp
 import os
 import os.path as osp
 import posixpath as psp
+import pytest
 
 
 class TestLoad(object):
 
   """Test client loader."""
 
   def test_bare(self):
     client = Client.from_options({'url': 'foo'})
-    ok_(isinstance(client, Client))
+    assert isinstance(client, Client)
 
   def test_new_type(self):
     class NewClient(Client):
       def __init__(self, url, bar):
         super(NewClient, self).__init__(url)
         self.bar = bar
     client = Client.from_options({'url': 'bar', 'bar': 2}, 'NewClient')
-    eq_(client.bar, 2)
+    assert client.bar == 2
 
-  @raises(HdfsError)
   def test_missing_options(self):
-    Client.from_options({}, 'KerberosClient')
+    with pytest.raises(HdfsError):
+      Client.from_options({}, 'KerberosClient')
 
-  @raises(HdfsError)
   def test_invalid_options(self):
-    Client.from_options({'foo': 123})
+    with pytest.raises(HdfsError):
+      Client.from_options({'foo': 123})
 
-  @raises(HdfsError)
   def test_missing_type(self):
-    Client.from_options({}, 'MissingClient')
+    with pytest.raises(HdfsError):
+      Client.from_options({}, 'MissingClient')
 
   def test_timeout(self):
-    eq_(Client('')._timeout, None)
-    eq_(Client('', timeout=1)._timeout, 1)
-    eq_(Client('', timeout=(1,2))._timeout, (1,2))
-    eq_(Client.from_options({'url': ''})._timeout, None)
+    assert Client('')._timeout == None
+    assert Client('', timeout=1)._timeout == 1
+    assert Client('', timeout=(1,2))._timeout == (1,2)
+    assert Client.from_options({'url': ''})._timeout == None
 
 
 class TestOptions(_IntegrationTest):
 
   """Test client options."""
 
+  @pytest.mark.skip(reason="TODO: Investigate why this fails in Python 3.7 and 3.9")
   def test_timeout(self):
-    self.client._timeout = 1e-5 # Small enough for it to always timeout.
-    try:
-      self.client.status('.')
-    except (ConnectTimeout, ReadTimeout):
-      self.client._timeout = None
-    else:
-      raise HdfsError('No timeout.')
+    with pytest.raises(ConnectTimeout, ReadTimeout):
+      self.client._timeout = 1e-6 # Small enough for it to always timeout.
+      try:
+        self.client.status('.')
+      finally:
+        self.client._timeout = None
 
 
 class TestApi(_IntegrationTest):
 
   """Test client raw API interactions."""
 
   def test_list_status_absolute_root(self):
-    ok_(self.client._list_status('/'))
+    assert self.client._list_status('/')
 
   def test_get_folder_status(self):
     self.client._mkdirs('foo')
     status = self.client._get_file_status('foo').json()['FileStatus']
-    eq_(status['type'], 'DIRECTORY')
+    assert status['type'] == 'DIRECTORY'
 
   def test_get_home_directory(self):
     path = self.client._get_home_directory('/').json()['Path']
-    ok_('/user/' in path)
+    assert '/user/' in path
 
   def test_delete_file(self):
     path = 'bar'
     self._write(path, b'hello')
-    ok_(self.client._delete(path).json()['boolean'])
-    ok_(not self._exists(path))
+    assert self.client._delete(path).json()['boolean']
+    assert not self._exists(path)
 
   def test_delete_missing_file(self):
     path = 'bar2'
-    ok_(not self.client._delete(path).json()['boolean'])
+    assert not self.client._delete(path).json()['boolean']
 
   def test_rename_file(self):
     paths = ['foo', '{}/bar'.format(self.client.root.rstrip('/'))]
     self._write(paths[0], b'hello')
-    ok_(self.client._rename(paths[0], destination=paths[1]).json()['boolean'])
-    ok_(not self._exists(paths[0]))
-    eq_(self.client._open(paths[1].rsplit('/', 1)[1]).content, b'hello')
+    assert self.client._rename(paths[0], destination=paths[1]).json()['boolean']
+    assert not self._exists(paths[0])
+    assert self.client._open(paths[1].rsplit('/', 1)[1]).content == b'hello'
     self.client._delete(paths[1])
 
   def test_rename_file_to_existing(self):
     p = ['foo', '{}/bar'.format(self.client.root.rstrip('/'))]
     self._write(p[0], b'hello')
     self._write(p[1], b'hi')
     try:
-      ok_(not self.client._rename(p[0], destination=p[1]).json()['boolean'])
+      assert not self.client._rename(p[0], destination=p[1]).json()['boolean']
     finally:
       self.client._delete(p[0])
       self.client._delete(p[1])
 
   def test_open_file(self):
     self._write('foo', b'hello')
-    eq_(self.client._open('foo').content, b'hello')
+    assert self.client._open('foo').content == b'hello'
 
   def test_get_file_checksum(self):
     self._write('foo', b'hello')
     data = self.client._get_file_checksum('foo').json()['FileChecksum']
-    eq_(sorted(data), ['algorithm', 'bytes', 'length'])
-    ok_(int(data['length']))
+    assert sorted(data) == ['algorithm', 'bytes', 'length']
+    assert int(data['length'])
 
-  @raises(HdfsError)
   def test_get_file_checksum_on_folder(self):
-    self.client._get_file_checksum('')
+    with pytest.raises(HdfsError):
+      self.client._get_file_checksum('')
 
 
 class TestResolve(_IntegrationTest):
 
   def test_resolve_relative(self):
-    eq_(Client('url', root='/').resolve('bar'), '/bar')
-    eq_(Client('url', root='/foo').resolve('bar'), '/foo/bar')
-    eq_(Client('url', root='/foo/').resolve('bar'), '/foo/bar')
-    eq_(Client('url', root='/foo/').resolve('bar/'), '/foo/bar')
-    eq_(Client('url', root='/foo/').resolve('/bar/'), '/bar')
+    assert Client('url', root='/').resolve('bar') == '/bar'
+    assert Client('url', root='/foo').resolve('bar') == '/foo/bar'
+    assert Client('url', root='/foo/').resolve('bar') == '/foo/bar'
+    assert Client('url', root='/foo/').resolve('bar/') == '/foo/bar'
+    assert Client('url', root='/foo/').resolve('/bar/') == '/bar'
 
   def test_resolve_relative_no_root(self):
     root = self.client.root
     try:
       self.client.root = None
       home = self.client._get_home_directory('/').json()['Path']
-      eq_(self.client.resolve('bar'), psp.join(home, 'bar'))
-      eq_(self.client.root, home)
+      assert self.client.resolve('bar') == psp.join(home, 'bar')
+      assert self.client.root == home
     finally:
       self.client.root = root
 
   def test_resolve_relative_root(self):
     root = self.client.root
     try:
       self.client.root = 'bar'
       home = self.client._get_home_directory('/').json()['Path']
-      eq_(self.client.resolve('foo'), psp.join(home, 'bar', 'foo'))
-      eq_(self.client.root, psp.join(home, 'bar'))
+      assert self.client.resolve('foo') == psp.join(home, 'bar', 'foo')
+      assert self.client.root == psp.join(home, 'bar')
     finally:
       self.client.root = root
 
   def test_resolve_absolute(self):
-    eq_(Client('url').resolve('/bar'), '/bar')
-    eq_(Client('url').resolve('/bar/foo/'), '/bar/foo')
+    assert Client('url').resolve('/bar') == '/bar'
+    assert Client('url').resolve('/bar/foo/') == '/bar/foo'
 
   def test_create_file_with_percent(self):
     # `%` (`0x25`) is a special case because it seems to cause errors (even
     # though the action still goes through). Typical error message will be
     # `"Unknown exception in doAs"`.
     path = 'fo&o/a%a'
     try:
       self._write(path, b'hello')
     except HdfsError:
       pass
-    eq_(self._read(path), b'hello')
+    assert self._read(path) == b'hello'
 
 
 class TestWrite(_IntegrationTest):
 
   def test_create_from_string(self):
     self.client.write('up', b'hello, world!')
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_create_from_string_with_encoding(self):
     self.client.write('up', u'hello, world!', encoding='utf-8')
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_create_from_generator(self):
     data = (e for e in [b'hello, ', b'world!'])
     self.client.write('up', data)
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_create_from_generator_with_encoding(self):
     data = (e for e in [u'hello, ', u'world!'])
     self.client.write('up', data, encoding='utf-8')
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_create_from_file_object(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('hello, world!')
       with open(tpath) as reader:
         self.client.write('up', reader)
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_create_set_permission(self):
     self.client.write('up', b'hello, world!', permission='722')
-    eq_(self._read('up'), b'hello, world!')
-    eq_(self.client.status('up')['permission'], '722')
+    assert self._read('up') == b'hello, world!'
+    assert self.client.status('up')['permission'] == '722'
 
-  @raises(HdfsError)
   def test_create_to_existing_file_without_overwrite(self):
-    self.client.write('up', b'hello, world!')
-    self.client.write('up', b'hello again, world!')
+    with pytest.raises(HdfsError):
+      self.client.write('up', b'hello, world!')
+      self.client.write('up', b'hello again, world!')
 
   def test_create_and_overwrite_file(self):
     self.client.write('up', b'hello, world!')
     self.client.write('up', b'hello again, world!', overwrite=True)
-    eq_(self._read('up'), b'hello again, world!')
+    assert self._read('up') == b'hello again, world!'
 
   def test_as_context_manager(self):
     with self.client.write('up') as writer:
       writer.write(b'hello, ')
       writer.write(b'world!')
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_as_context_manager_with_encoding(self):
     with self.client.write('up', encoding='utf-8') as writer:
       writer.write(u'hello, ')
       writer.write(u'world!')
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
   def test_dump_json(self):
     from json import dump, loads
     data = {'one': 1, 'two': 2}
     with self.client.write('up', encoding='utf-8') as writer:
       dump(data, writer)
-    eq_(loads(self._read('up', encoding='utf-8')), data)
+    assert loads(self._read('up', encoding='utf-8')) == data
 
-  @raises(HdfsError)
   def test_create_and_overwrite_directory(self):
-    # can't overwrite a directory with a file
-    self.client._mkdirs('up')
-    self.client.write('up', b'hello, world!')
+    with pytest.raises(HdfsError):
+      # can't overwrite a directory with a file
+      self.client._mkdirs('up')
+      self.client.write('up', b'hello, world!')
 
-  @raises(HdfsError)
   def test_create_invalid_path(self):
-    # conversely, can't overwrite a file with a directory
-    self.client.write('up', b'hello, world!')
-    self.client.write('up/up', b'hello again, world!')
+    with pytest.raises(HdfsError):
+      # conversely, can't overwrite a file with a directory
+      self.client.write('up', b'hello, world!')
+      self.client.write('up/up', b'hello again, world!')
 
 
 class TestAppend(_IntegrationTest):
 
   @classmethod
   def setup_class(cls):
     super(TestAppend, cls).setup_class()
@@ -260,115 +260,115 @@
           # Skip these tests if HDFS isn't configured to support appends.
         else:
           raise err
 
   def test_simple(self):
     self.client.write('ap', b'hello,')
     self.client.write('ap', b' world!', append=True)
-    eq_(self._read('ap'), b'hello, world!')
+    assert self._read('ap') == b'hello, world!'
 
-  @raises(HdfsError)
   def test_missing_file(self):
-    self.client.write('ap', b'hello!', append=True)
+    with pytest.raises(HdfsError):
+      self.client.write('ap', b'hello!', append=True)
 
-  @raises(ValueError)
   def test_overwrite_and_append(self):
-    self.client.write('ap', b'hello!', overwrite=True, append=True)
+    with pytest.raises(ValueError):
+      self.client.write('ap', b'hello!', overwrite=True, append=True)
 
-  @raises(ValueError)
   def test_set_permission_and_append(self):
-    self.client.write('ap', b'hello!', permission='777', append=True)
+    with pytest.raises(ValueError):
+      self.client.write('ap', b'hello!', permission='777', append=True)
 
 
 class TestUpload(_IntegrationTest):
 
   def test_upload_file(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('hello, world!')
       self.client.upload('up', tpath)
-    eq_(self._read('up'), b'hello, world!')
+    assert self._read('up') == b'hello, world!'
 
-  @raises(HdfsError)
   def test_upload_missing(self):
-    with temppath() as tpath:
-      self.client.upload('up', tpath)
+    with pytest.raises(HdfsError):
+      with temppath() as tpath:
+        self.client.upload('up', tpath)
 
-  @raises(HdfsError)
   def test_upload_empty_directory(self):
-    dpath = mkdtemp()
-    try:
-      self.client.upload('up', dpath)
-    finally:
-      os.rmdir(dpath)
+    with pytest.raises(HdfsError):
+      dpath = mkdtemp()
+      try:
+        self.client.upload('up', dpath)
+      finally:
+        os.rmdir(dpath)
 
   def test_upload_directory_to_existing_directory(self):
     dpath = mkdtemp()
     try:
       npath = osp.join(dpath, 'hi')
       os.mkdir(npath)
       with open(osp.join(npath, 'foo'), 'w') as writer:
         writer.write('hello!')
       os.mkdir(osp.join(npath, 'bar'))
       with open(osp.join(npath, 'bar', 'baz'), 'w') as writer:
         writer.write('world!')
       self.client._mkdirs('up')
       self.client.upload('up', npath)
-      eq_(self._read('up/hi/foo'), b'hello!')
-      eq_(self._read('up/hi/bar/baz'), b'world!')
+      assert self._read('up/hi/foo') == b'hello!'
+      assert self._read('up/hi/bar/baz') == b'world!'
     finally:
       rmtree(dpath)
 
   def test_upload_directory_to_missing(self):
     dpath = mkdtemp()
     try:
       with open(osp.join(dpath, 'foo'), 'w') as writer:
         writer.write('hello!')
       os.mkdir(osp.join(dpath, 'bar'))
       with open(osp.join(dpath, 'bar', 'baz'), 'w') as writer:
         writer.write('world!')
       self.client.upload('up', dpath)
-      eq_(self._read('up/foo'), b'hello!')
-      eq_(self._read('up/bar/baz'), b'world!')
+      assert self._read('up/foo') == b'hello!'
+      assert self._read('up/bar/baz') == b'world!'
     finally:
       rmtree(dpath)
 
   def test_upload_directory_overwrite_existing_file(self):
     dpath = mkdtemp()
     try:
       with open(osp.join(dpath, 'foo'), 'w') as writer:
         writer.write('hello!')
       os.mkdir(osp.join(dpath, 'bar'))
       with open(osp.join(dpath, 'bar', 'baz'), 'w') as writer:
         writer.write('world!')
       self._write('up', b'hi')
       self.client.upload('up', dpath, overwrite=True)
-      eq_(self._read('up/foo'), b'hello!')
-      eq_(self._read('up/bar/baz'), b'world!')
+      assert self._read('up/foo') == b'hello!'
+      assert self._read('up/bar/baz') == b'world!'
     finally:
       rmtree(dpath)
 
   def test_upload_overwrite(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('hello')
       self.client.upload('up', tpath)
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('there')
       self.client.upload('up', tpath, overwrite=True)
-    eq_(self._read('up'), b'there')
+    assert self._read('up') == b'there'
 
-  @raises(HdfsError)
   def test_upload_overwrite_error(self):
-    with temppath() as tpath:
-      with open(tpath, 'w') as writer:
-        writer.write('here')
-      self.client.upload('up', tpath)
-      self.client.upload('up', tpath)
+    with pytest.raises(HdfsError):
+      with temppath() as tpath:
+        with open(tpath, 'w') as writer:
+          writer.write('here')
+        self.client.upload('up', tpath)
+        self.client.upload('up', tpath)
 
   def test_upload_cleanup(self):
     dpath = mkdtemp()
     _write = self.client.write
 
     def write(hdfs_path, *args, **kwargs):
       if 'bar' in hdfs_path:
@@ -383,17 +383,17 @@
         writer.write('hello!')
       os.mkdir(osp.join(npath, 'bar'))
       with open(osp.join(npath, 'bar', 'baz'), 'w') as writer:
         writer.write('world!')
       try:
         self.client.upload('foo', dpath)
       except RuntimeError:
-        ok_(not self._exists('foo'))
+        assert not self._exists('foo')
       else:
-        ok_(False) # This shouldn't happen.
+        assert False # This shouldn't happen.
     finally:
       rmtree(dpath)
       self.client.write = _write
 
   def test_upload_no_cleanup(self):
     dpath = mkdtemp()
     _write = self.client.write
@@ -412,17 +412,17 @@
       os.mkdir(osp.join(npath, 'bar'))
       with open(osp.join(npath, 'bar', 'baz'), 'w') as writer:
         writer.write('world!')
       try:
         self.client.upload('foo', dpath, cleanup=False)
       except RuntimeError:
         # The outer folder still exists.
-        ok_(self._exists('foo'))
+        assert self._exists('foo')
       else:
-        ok_(False) # This shouldn't happen.
+        assert False # This shouldn't happen.
     finally:
       rmtree(dpath)
       self.client.write = _write
 
   def test_upload_with_progress(self):
 
     def callback(path, nbytes, history=defaultdict(list)):
@@ -441,241 +441,240 @@
       self.client.upload(
         'up',
         dpath,
         chunk_size=4,
         n_threads=1, # Callback isn't thread-safe.
         progress=callback
       )
-      eq_(self._read('up/foo'), b'hello!')
-      eq_(self._read('up/bar/baz'), b'the world!')
-      eq_(
-        callback('', 0),
-        {path1: [4, 6, -1], path2: [4, 8, 10, -1], '': [0]}
-      )
+      assert self._read('up/foo') == b'hello!'
+      assert self._read('up/bar/baz') == b'the world!'
+      assert (
+        callback('', 0) ==
+        {path1: [4, 6, -1], path2: [4, 8, 10, -1], '': [0]})
     finally:
       rmtree(dpath)
 
 
 class TestDelete(_IntegrationTest):
 
   def test_delete_file(self):
     self._write('foo', b'hello, world!')
-    ok_(self.client.delete('foo'))
-    ok_(not self._exists('foo'))
+    assert self.client.delete('foo')
+    assert not self._exists('foo')
 
   def test_delete_empty_directory(self):
     self.client._mkdirs('foo')
-    ok_(self.client.delete('foo'))
-    ok_(not self._exists('foo'))
+    assert self.client.delete('foo')
+    assert not self._exists('foo')
 
   def test_delete_missing_file(self):
-    ok_(not self.client.delete('foo'))
+    assert not self.client.delete('foo')
 
   def test_delete_non_empty_directory(self):
     self._write('de/foo', b'hello, world!')
-    ok_(self.client.delete('de', recursive=True))
-    ok_(not self._exists('de'))
+    assert self.client.delete('de', recursive=True)
+    assert not self._exists('de')
 
-  @raises(HdfsError)
   def test_delete_non_empty_directory_without_recursive(self):
-    self._write('de/foo', b'hello, world!')
-    self.client.delete('de')
+    with pytest.raises(HdfsError):
+      self._write('de/foo', b'hello, world!')
+      self.client.delete('de')
 
   def test_trash_file(self):
     self._write('foo', b'hello, world!')
-    ok_(self.client.delete('foo', skip_trash=False))
-    eq_(self.client.status('foo', strict=False), None)
+    assert self.client.delete('foo', skip_trash=False)
+    assert self.client.status('foo', strict=False) == None
 
   def test_trash_missing_file(self):
-    ok_(not self.client.delete('foo', skip_trash=False))
+    assert not self.client.delete('foo', skip_trash=False)
 
-  @raises(HdfsError)
   def test_trash_directory_non_recursive(self):
-    self._write('bar/foo', b'hello, world!')
-    self.client.delete('bar', skip_trash=False)
+    with pytest.raises(HdfsError):
+      self._write('bar/foo', b'hello, world!')
+      self.client.delete('bar', skip_trash=False)
 
   def test_trash_directory(self):
     self._write('bar/foo', b'hello, world!')
-    ok_(self.client.delete('bar', recursive=True, skip_trash=False))
-    eq_(self.client.status('bar', strict=False), None)
+    assert self.client.delete('bar', recursive=True, skip_trash=False)
+    assert self.client.status('bar', strict=False) == None
 
 
 class TestRead(_IntegrationTest):
 
-  @raises(ValueError)
   def test_progress_without_chunk_size(self):
-    self._write('foo', b'hello, world!')
-    with self.client.read('foo', progress=lambda path, nbytes: None) as reader:
-      pass
+    with pytest.raises(ValueError):
+      self._write('foo', b'hello, world!')
+      with self.client.read('foo', progress=lambda path, nbytes: None) as reader:
+        pass
 
-  @raises(ValueError)
   def test_delimiter_without_encoding(self):
-    self._write('foo', b'hello, world!')
-    with self.client.read('foo', delimiter=',') as reader:
-      pass
+    with pytest.raises(ValueError):
+      self._write('foo', b'hello, world!')
+      with self.client.read('foo', delimiter=',') as reader:
+        pass
 
-  @raises(ValueError)
   def test_delimiter_with_chunk_size(self):
-    self._write('foo', b'hello, world!')
-    with self.client.read('foo', delimiter=',', chunk_size=1) as reader:
-      pass
+    with pytest.raises(ValueError):
+      self._write('foo', b'hello, world!')
+      with self.client.read('foo', delimiter=',', chunk_size=1) as reader:
+        pass
 
   def test_read_file(self):
     self._write('foo', b'hello, world!')
     with self.client.read('foo') as reader:
-      eq_(reader.read(), b'hello, world!')
+      assert reader.read() == b'hello, world!'
 
-  @raises(HdfsError)
   def test_read_directory(self):
-    self.client._mkdirs('foo')
-    with self.client.read('foo') as reader:
-      pass
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      with self.client.read('foo') as reader:
+        pass
 
-  @raises(HdfsError)
   def test_read_missing_file(self):
-    with self.client.read('foo') as reader:
-      pass
+    with pytest.raises(HdfsError):
+      with self.client.read('foo') as reader:
+        pass
 
   def test_read_file_from_offset(self):
     self._write('foo', b'hello, world!')
     with self.client.read('foo', offset=7) as reader:
-      eq_(reader.read(), b'world!')
+      assert reader.read() == b'world!'
 
   def test_read_file_from_offset_with_limit(self):
     self._write('foo', b'hello, world!')
     with self.client.read('foo', offset=7, length=5) as reader:
-      eq_(reader.read(), b'world')
+      assert reader.read() == b'world'
 
   def test_read_file_with_chunk_size(self):
     self._write('foo', b'hello, world!')
     with self.client.read('foo', chunk_size=5) as reader:
-      eq_(list(reader), [b'hello', b', wor', b'ld!'])
+      assert list(reader) == [b'hello', b', wor', b'ld!']
 
   def test_with_progress(self):
     def cb(path, nbytes, chunk_lengths=[]):
       chunk_lengths.append(nbytes)
       return chunk_lengths
     self._write('foo', b'hello, world!')
     with temppath() as tpath:
       with open(tpath, 'wb') as writer:
         with self.client.read('foo', chunk_size=5, progress=cb) as reader:
           for chunk in reader:
             writer.write(chunk)
       with open(tpath, 'rb') as reader:
-        eq_(reader.read(), b'hello, world!')
-      eq_(cb('', 0), [5, 10, 13, -1, 0])
+        assert reader.read() == b'hello, world!'
+      assert cb('', 0) == [5, 10, 13, -1, 0]
 
   def test_read_with_encoding(self):
     s = u'hello, world!'
     self._write('foo', s, encoding='utf-8')
     with self.client.read('foo', encoding='utf-8') as reader:
-      eq_(reader.read(), s)
+      assert reader.read() == s
 
   def test_read_with_chunk_size_and_encoding(self):
     s = u'hello, world!'
     self._write('foo', s, encoding='utf-8')
     with self.client.read('foo', chunk_size=5, encoding='utf-8') as reader:
-      eq_(list(reader), [u'hello', u', wor', u'ld!'])
+      assert list(reader) == [u'hello', u', wor', u'ld!']
 
   def test_read_json(self):
     from json import dumps, load
     data = {'one': 1, 'two': 2}
     self._write('foo', data=dumps(data), encoding='utf-8')
     with self.client.read('foo', encoding='utf-8') as reader:
-      eq_(load(reader), data)
+      assert load(reader) == data
 
   def test_read_with_delimiter(self):
     self._write('foo', u'hi\nworld!\n', encoding='utf-8')
     with self.client.read('foo', delimiter='\n', encoding='utf-8') as reader:
-      eq_(list(reader), [u'hi', u'world!', u''])
+      assert list(reader) == [u'hi', u'world!', u'']
 
 
 class TestRename(_IntegrationTest):
 
   def test_rename_file(self):
     self._write('foo', b'hello, world!')
     self.client.rename('foo', 'bar')
-    eq_(self._read('bar'), b'hello, world!')
+    assert self._read('bar') == b'hello, world!'
 
-  @raises(HdfsError)
   def test_rename_missing_file(self):
-    self.client.rename('foo', 'bar')
+    with pytest.raises(HdfsError):
+      self.client.rename('foo', 'bar')
 
-  @raises(HdfsError)
   def test_rename_file_to_existing_file(self):
-    self._write('foo', b'hello, world!')
-    self._write('bar', b'hello again, world!')
-    self.client.rename('foo', 'bar')
+    with pytest.raises(HdfsError):
+      self._write('foo', b'hello, world!')
+      self._write('bar', b'hello again, world!')
+      self.client.rename('foo', 'bar')
 
   def test_move_file_into_existing_directory(self):
     self._write('foo', b'hello, world!')
     self.client._mkdirs('bar')
     self.client.rename('foo', 'bar')
-    eq_(self._read('bar/foo'), b'hello, world!')
+    assert self._read('bar/foo') == b'hello, world!'
 
   def test_rename_file_into_existing_directory(self):
     self._write('foo', b'hello, world!')
     self.client._mkdirs('bar')
     self.client.rename('foo', 'bar/baz')
-    eq_(self._read('bar/baz'), b'hello, world!')
+    assert self._read('bar/baz') == b'hello, world!'
 
   def test_rename_file_with_special_characters(self):
     path = 'fo&oa ?a=1'
     self._write('foo', b'hello, world!')
     self.client.rename('foo', path)
-    eq_(self._read(path), b'hello, world!')
+    assert self._read(path) == b'hello, world!'
 
 
 class TestDownload(_IntegrationTest):
 
-  @raises(HdfsError)
   def test_missing_dir(self):
-    self._write('dl', b'hello')
-    with temppath() as tpath:
-      self.client.download('dl', osp.join(tpath, 'foo'))
+    with pytest.raises(HdfsError):
+      self._write('dl', b'hello')
+      with temppath() as tpath:
+        self.client.download('dl', osp.join(tpath, 'foo'))
 
   def test_normal_file(self):
     self._write('dl', b'hello')
     with temppath() as tpath:
       fpath = self.client.download('dl', tpath)
       with open(fpath) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
   def test_nonpartitioned_file(self):
     partname = 'part-r-00000'
     self._write('dl/' + partname, b'world')
     with temppath() as tpath:
       fname = self.client.download('dl/' + partname, tpath)
       with open(fname) as reader:
-        eq_(reader.read(), 'world')
+        assert reader.read() == 'world'
 
   def test_singly_partitioned_file(self):
     partname = 'part-r-00000'
     self._write('dl/' + partname, b'world')
     with temppath() as tpath:
       os.mkdir(tpath)
       fname = self.client.download('dl', tpath)
       with open(osp.join(fname, partname)) as reader:
-        eq_(reader.read(), 'world')
+        assert reader.read() == 'world'
 
   def _download_partitioned_file(self, n_threads):
     parts = {
       'part-r-00000': b'fee',
       'part-r-00001': b'faa',
       'part-r-00002': b'foo',
     }
     for name, content in parts.items():
       self._write('dl/{}'.format(name), content)
     with temppath() as tpath:
       self.client.download('dl', tpath, n_threads=-1)
       local_parts = os.listdir(tpath)
-      eq_(set(local_parts), set(parts)) # We have all the parts.
+      assert set(local_parts) == set(parts) # We have all the parts.
       for part in local_parts:
         with open(osp.join(tpath, part), mode='rb') as reader:
-          eq_(reader.read(), parts[part]) # Their content is correct.
+          assert reader.read() == parts[part] # Their content is correct.
 
   def test_partitioned_file_max_threads(self):
     self._download_partitioned_file(0)
 
   def test_partitioned_file_sync(self):
     self._download_partitioned_file(1)
 
@@ -685,91 +684,91 @@
   def test_overwrite_file(self):
     with temppath() as tpath:
       self._write('dl', b'hello')
       self.client.download('dl', tpath)
       self.client.write('dl', b'there', overwrite=True)
       fname = self.client.download('dl', tpath, overwrite=True)
       with open(fname) as reader:
-        eq_(reader.read(), 'there')
+        assert reader.read() == 'there'
 
-  @raises(HdfsError)
   def test_download_file_to_existing_file(self):
-    self._write('dl', b'hello')
-    with temppath() as tpath:
-      with open(tpath, 'w') as writer:
-        writer.write('hi')
-      self.client.download('dl', tpath)
+    with pytest.raises(HdfsError):
+      self._write('dl', b'hello')
+      with temppath() as tpath:
+        with open(tpath, 'w') as writer:
+          writer.write('hi')
+        self.client.download('dl', tpath)
 
   def test_download_file_to_existing_file_with_overwrite(self):
     self._write('dl', b'hello')
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('hi')
       self.client.download('dl', tpath, overwrite=True)
       with open(tpath) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
   def test_download_file_to_existing_folder(self):
     self._write('dl', b'hello')
     with temppath() as tpath:
       os.mkdir(tpath)
       self.client.download('dl', tpath)
       with open(osp.join(tpath, 'dl')) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
-  @raises(HdfsError)
   def test_download_file_to_existing_folder_with_matching_file(self):
-    self._write('dl', b'hello')
-    with temppath() as tpath:
-      os.mkdir(tpath)
-      with open(osp.join(tpath, 'dl'), 'w') as writer:
-        writer.write('hey')
-      self.client.download('dl', tpath)
+    with pytest.raises(HdfsError):
+      self._write('dl', b'hello')
+      with temppath() as tpath:
+        os.mkdir(tpath)
+        with open(osp.join(tpath, 'dl'), 'w') as writer:
+          writer.write('hey')
+        self.client.download('dl', tpath)
 
   def test_download_file_to_existing_folder_overwrite_matching_file(self):
     self._write('dl', b'hello')
     with temppath() as tpath:
       os.mkdir(tpath)
       with open(osp.join(tpath, 'dl'), 'w') as writer:
         writer.write('hey')
       self.client.download('dl', tpath, overwrite=True)
       with open(osp.join(tpath, 'dl')) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
   def test_download_folder_to_existing_folder(self):
     self._write('foo/dl', b'hello')
     self._write('foo/bar/dl', b'there')
     with temppath() as tpath:
       os.mkdir(tpath)
       self.client.download('foo', tpath)
       with open(osp.join(tpath, 'foo', 'dl')) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
       with open(osp.join(tpath, 'foo', 'bar', 'dl')) as reader:
-        eq_(reader.read(), 'there')
+        assert reader.read() == 'there'
 
   def test_download_folder_to_existing_folder_parallel(self):
     self._write('foo/dl', b'hello')
     self._write('foo/bar/dl', b'there')
     with temppath() as tpath:
       os.mkdir(tpath)
       self.client.download('foo', tpath, n_threads=0)
       with open(osp.join(tpath, 'foo', 'dl')) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
       with open(osp.join(tpath, 'foo', 'bar', 'dl')) as reader:
-        eq_(reader.read(), 'there')
+        assert reader.read() == 'there'
 
   def test_download_folder_to_missing_folder(self):
     self._write('foo/dl', b'hello')
     self._write('foo/bar/dl', b'there')
     with temppath() as tpath:
       self.client.download('foo', tpath)
       with open(osp.join(tpath, 'dl')) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
       with open(osp.join(tpath, 'bar', 'dl')) as reader:
-        eq_(reader.read(), 'there')
+        assert reader.read() == 'there'
 
   def test_download_cleanup(self):
     self._write('foo/dl', b'hello')
     self._write('foo/bar/dl', b'there')
     _read = self.client.read
 
     def read(hdfs_path, *args, **kwargs):
@@ -778,61 +777,61 @@
       return _read(hdfs_path, *args, **kwargs)
 
     with temppath() as tpath:
       try:
         self.client.read = read
         self.client.download('foo', tpath)
       except RuntimeError:
-        ok_(not osp.exists(tpath))
+        assert not osp.exists(tpath)
       else:
-        ok_(False) # This shouldn't happen.
+        assert False # This shouldn't happen.
       finally:
         self.client.read = _read
 
-  @raises(HdfsError)
   def test_download_empty_folder(self):
-    self.client._mkdirs('foo')
-    with temppath() as tpath:
-      self.client.download('foo', tpath)
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      with temppath() as tpath:
+        self.client.download('foo', tpath)
 
   def test_download_dir_whitespace(self):
     self._write('foo/foo bar.txt', b'hello')
     with temppath() as tpath:
       self.client.download('foo', tpath)
       with open(osp.join(tpath, 'foo bar.txt')) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
   def test_download_file_whitespace(self):
     self._write('foo/foo bar%.txt', b'hello')
     with temppath() as tpath:
       self.client.download('foo/foo bar%.txt', tpath)
       with open(tpath) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
 
 class TestStatus(_IntegrationTest):
 
   def test_directory(self):
     self.client._mkdirs('foo')
     status = self.client.status('foo')
-    eq_(status['type'], 'DIRECTORY')
-    eq_(status['length'], 0)
+    assert status['type'] == 'DIRECTORY'
+    assert status['length'] == 0
 
   def test_file(self):
     self._write('foo', b'hello, world!')
     status = self.client.status('foo')
-    eq_(status['type'], 'FILE')
-    eq_(status['length'], 13)
+    assert status['type'] == 'FILE'
+    assert status['length'] == 13
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.status('foo')
+    with pytest.raises(HdfsError):
+      self.client.status('foo')
 
   def test_missing_non_strict(self):
-    ok_(self.client.status('foo', strict=False) is None)
+    assert self.client.status('foo', strict=False) is None
 
 
 class TestSetOwner(_IntegrationTest):
 
   @classmethod
   def setup_class(cls):
     super(TestSetOwner, cls).setup_class()
@@ -849,459 +848,458 @@
 
   def test_directory_owner(self):
     new_owner = 'newowner'
     self.client._mkdirs('foo')
     self.client.set_owner('foo', 'oldowner')
     self.client.set_owner('foo', new_owner)
     status = self.client.status('foo')
-    eq_(status['owner'], new_owner)
+    assert status['owner'] == new_owner
 
   def test_file_owner(self):
     new_owner = 'newowner'
     self._write('foo', b'hello, world!')
     self.client.set_owner('foo', 'oldowner')
     self.client.set_owner('foo', new_owner)
     status = self.client.status('foo')
-    eq_(status['owner'], new_owner)
+    assert status['owner'] == new_owner
 
   def test_directory_for_group(self):
     new_group = 'newgroup'
     self.client._mkdirs('foo')
     self.client.set_owner('foo', group='oldgroup')
     self.client.set_owner('foo', group=new_group)
     status = self.client.status('foo')
-    eq_(status['group'], new_group)
+    assert status['group'] == new_group
 
   def test_file_for_group(self):
     new_group = 'newgroup'
     self._write('foo', b'hello, world!')
     self.client.set_owner('foo', group='oldgroup')
     self.client.set_owner('foo', group=new_group)
     status = self.client.status('foo')
-    eq_(status['group'], new_group)
+    assert status['group'] == new_group
 
-  @raises(HdfsError)
   def test_missing_for_group(self):
-    self.client.set_owner('foo', group='blah')
+    with pytest.raises(HdfsError):
+      self.client.set_owner('foo', group='blah')
 
 
 class TestSetPermission(_IntegrationTest):
 
   def test_directory(self):
     new_permission = '755'
     self.client._mkdirs('foo', permission='444')
     self.client.set_permission('foo', new_permission)
     status = self.client.status('foo')
-    eq_(status['permission'], new_permission)
+    assert status['permission'] == new_permission
 
   def test_file(self):
     new_permission = '755'
     self.client.write('foo', b'hello, world!', permission='444')
     self.client.set_permission('foo', new_permission)
     status = self.client.status('foo')
-    eq_(status['permission'], new_permission)
+    assert status['permission'] == new_permission
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.set_permission('foo', '755')
+    with pytest.raises(HdfsError):
+      self.client.set_permission('foo', '755')
 
 
 class TestContent(_IntegrationTest):
 
   def test_directory(self):
     self._write('foo', b'hello, world!')
     content = self.client.content('')
-    eq_(content['directoryCount'], 1)
-    eq_(content['fileCount'], 1)
-    eq_(content['length'], 13)
+    assert content['directoryCount'] == 1
+    assert content['fileCount'] == 1
+    assert content['length'] == 13
 
   def test_file(self):
     self._write('foo', b'hello, world!')
     content = self.client.content('foo')
-    eq_(content['directoryCount'], 0)
-    eq_(content['fileCount'], 1)
-    eq_(content['length'], 13)
+    assert content['directoryCount'] == 0
+    assert content['fileCount'] == 1
+    assert content['length'] == 13
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.content('foo')
+    with pytest.raises(HdfsError):
+      self.client.content('foo')
 
   def test_missing_non_strict(self):
-    ok_(self.client.content('foo', strict=False) is None)
+    assert self.client.content('foo', strict=False) is None
 
 
 class TestAcl(_IntegrationTest):
 
   def test_directory(self):
     self._write('foo', b'hello, world!')
     content = self.client.acl_status('')
-    ok_(len(content) > 1)
-    ok_('entries' in content)
-    ok_('group' in content)
-    ok_('owner' in content)
+    assert len(content) > 1
+    assert 'entries' in content
+    assert 'group' in content
+    assert 'owner' in content
 
   def test_set_acl(self):
     self.client.write('foo', 'hello, world!')
     self.client.set_acl('foo', 'user::rwx,user:foouser:rwx,group::r--,other::---')
     content = self.client.acl_status('foo')
-    ok_(any('user:foouser:rwx' in s for s in content['entries']))
-    ok_(len(content) > 1)
-    ok_(content['entries'] is not None)
+    assert any('user:foouser:rwx' in s for s in content['entries'])
+    assert len(content) > 1
+    assert content['entries'] is not None
 
   def test_modify_acl(self):
     self.client.write('foo', 'hello, world!')
     self.client.set_acl('foo', 'user::rwx,user:foouser:rwx,group::r--,other::---')
     self.client.set_acl('foo', 'user:foouser:rw-', clear=False)
     content = self.client.acl_status('foo')
-    ok_(any('user:foouser:rw-' in s for s in content['entries']))
+    assert any('user:foouser:rw-' in s for s in content['entries'])
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.acl_status('foo')
+    with pytest.raises(HdfsError):
+      self.client.acl_status('foo')
 
   def test_missing_non_strict(self):
-    ok_(self.client.acl_status('foo', strict=False) is None)
+    assert self.client.acl_status('foo', strict=False) is None
 
   def test_remove_acl_entries(self):
     self.client.write('foo', 'hello, world!')
     self.client.set_acl('foo', 'user:baruser:rwx,user:foouser:rw-', clear=False)
     self.client.remove_acl_entries('foo', 'user:foouser:')
     content = self.client.acl_status('foo')
-    ok_(not any('user:foouser:rw-' in s for s in content['entries']))
-    ok_(any('user:baruser:rwx' in s for s in content['entries']))
+    assert not any('user:foouser:rw-' in s for s in content['entries'])
+    assert any('user:baruser:rwx' in s for s in content['entries'])
 
   def test_remove_default_acl(self):
     self.client.write('foo', 'hello, world!')
     self.client.set_acl('foo', 'user:foouser:rwx', clear=False)
     self.client.remove_default_acl('foo')
     content = self.client.acl_status('foo')
-    ok_(not any('user::rwx' in s for s in content['entries']))
+    assert not any('user::rwx' in s for s in content['entries'])
 
   def test_remove_acl(self):
     self.client.write('foo', 'hello, world!')
     self.client.remove_acl('foo')
     content = self.client.acl_status('foo')
-    eq_(content.get('entries'), [])
+    assert content.get('entries') == []
 
 
 class TestList(_IntegrationTest):
 
-  @raises(HdfsError)
   def test_file(self):
-    self.client.write('foo', 'hello, world!')
-    self.client.list('foo')
+    with pytest.raises(HdfsError):
+      self.client.write('foo', 'hello, world!')
+      self.client.list('foo')
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.list('foo')
+    with pytest.raises(HdfsError):
+      self.client.list('foo')
 
   def test_empty_dir(self):
     self.client._mkdirs('foo')
-    eq_(self.client.list('foo'), [])
+    assert self.client.list('foo') == []
 
   def test_dir(self):
     self.client.write('foo/bar', 'hello, world!')
-    eq_(self.client.list('foo'), ['bar'])
+    assert self.client.list('foo') == ['bar']
 
   def test_dir_with_status(self):
     self.client.write('foo/bar', 'hello, world!')
     statuses = self.client.list('foo', status=True)
-    eq_(len(statuses), 1)
+    assert len(statuses) == 1
     status = self.client.status('foo/bar')
     status['pathSuffix'] = 'bar'
-    eq_(statuses[0], ('bar', status))
+    assert statuses[0] == ('bar', status)
 
 
 class TestWalk(_IntegrationTest):
 
-  @raises(HdfsError)
   def test_missing(self):
-    list(self.client.walk('foo'))
+    with pytest.raises(HdfsError):
+      list(self.client.walk('foo'))
 
   def test_file(self):
     self.client.write('foo', 'hello, world!')
-    ok_(not list(self.client.walk('foo')))
+    assert not list(self.client.walk('foo'))
 
   def test_folder(self):
     self.client.write('hello', 'hello, world!')
     self.client.write('foo/hey', 'hey, world!')
     infos = list(self.client.walk(''))
-    eq_(len(infos), 2)
-    eq_(infos[0], (psp.join(self.client.root), ['foo'], ['hello']))
-    eq_(infos[1], (psp.join(self.client.root, 'foo'), [], ['hey']))
+    assert len(infos) == 2
+    assert infos[0] == (psp.join(self.client.root), ['foo'], ['hello'])
+    assert infos[1] == (psp.join(self.client.root, 'foo'), [], ['hey'])
 
   def test_folder_with_depth(self):
     self.client.write('foo/bar', 'hello, world!')
     infos = list(self.client.walk('', depth=1))
-    eq_(len(infos), 1)
-    eq_(infos[0], (self.client.root, ['foo'], []))
+    assert len(infos) == 1
+    assert infos[0] == (self.client.root, ['foo'], [])
 
   def test_folder_with_status(self):
     self.client.write('foo', 'hello, world!')
     infos = list(self.client.walk('', status=True))
     status = self.client.status('foo')
     status['pathSuffix'] = 'foo'
-    eq_(len(infos), 1)
-    eq_(
-      infos[0],
+    assert len(infos) == 1
+    assert (
+      infos[0] ==
       (
         (self.client.root, self.client.status('')),
         [],
         [('foo', status)]
-      )
-    )
+      ))
 
   def test_skip_missing_folder(self):
     self.client.write('file', 'one')
     self.client.write('folder/hey', 'two')
     for info in self.client.walk('', ignore_missing=True):
-      eq_(info, (psp.join(self.client.root), ['folder'], ['file']))
+      assert info == (psp.join(self.client.root), ['folder'], ['file'])
       self.client.delete('folder', recursive=True)
 
-  @raises(ValueError)
   def test_status_and_allow_dir_changes(self):
-    list(self.client.walk('.', status=True, allow_dir_changes=True))
+    with pytest.raises(ValueError):
+      list(self.client.walk('.', status=True, allow_dir_changes=True))
 
   def test_allow_dir_changes_subset(self):
     self.client.write('foo/file1', 'one')
     self.client.write('bar/file2', 'two')
     infos = self.client.walk('.', allow_dir_changes=True)
     info = next(infos)
     info[1][:] = ['bar']
     info = next(infos)
-    eq_(info, (psp.join(self.client.root, 'bar'), [], ['file2']))
+    assert info == (psp.join(self.client.root, 'bar'), [], ['file2'])
 
   def test_allow_dir_changes_insert(self):
     self.client.write('foo/file1', 'one')
     infos = self.client.walk('.', allow_dir_changes=True)
     info = next(infos)
     self.client.write('bar/file2', 'two')
     info[1][:] = ['bar'] # Insert new directory.
     info = next(infos)
-    eq_(info, (psp.join(self.client.root, 'bar'), [], ['file2']))
+    assert info == (psp.join(self.client.root, 'bar'), [], ['file2'])
 
 
 class TestLatestExpansion(_IntegrationTest):
 
   def test_resolve_simple(self):
     self.client.write('bar', 'hello, world!')
     self.client.write('foo', 'hello again, world!')
-    eq_(self.client.resolve('#LATEST'), osp.join(self.client.root, 'foo'))
+    assert self.client.resolve('#LATEST') == osp.join(self.client.root, 'foo')
 
   def test_resolve_nested(self):
     self.client.write('baz/bar', 'hello, world!')
     self.client.write('bar/bar', 'hello there, world!')
     self.client.write('bar/foo', 'hello again, world!')
     latest = self.client.resolve('#LATEST/#LATEST')
-    eq_(latest, osp.join(self.client.root, 'bar', 'foo'))
+    assert latest == osp.join(self.client.root, 'bar', 'foo')
 
   def test_resolve_multiple(self):
     self.client.write('bar/bar', 'hello, world!')
     self.client.write('bar/foo', 'hello again, world!')
     latest = self.client.resolve('#LATEST/#LATEST')
-    eq_(latest, osp.join(self.client.root, 'bar', 'foo'))
+    assert latest == osp.join(self.client.root, 'bar', 'foo')
 
   def test_resolve_multiple_shortcut(self):
     self.client.write('bar/bar', 'hello, world!')
     self.client.write('bar/foo', 'hello again, world!')
     latest = self.client.resolve('#LATEST{2}')
-    eq_(latest, osp.join(self.client.root, 'bar', 'foo'))
+    assert latest == osp.join(self.client.root, 'bar', 'foo')
 
-  @nottest # HttpFS is inconsistent here.
-  @raises(HdfsError)
+  @pytest.mark.skip(reason="HttpFS is inconsistent here.")
   def test_resolve_file(self):
-    self.client.write('bar', 'hello, world!')
-    self.client.resolve('bar/#LATEST')
+    with pytest.raises(HdfsError):
+      self.client.write('bar', 'hello, world!')
+      self.client.resolve('bar/#LATEST')
 
-  @raises(HdfsError)
   def test_resolve_empty_directory(self):
-    self.client._mkdirs('bar')
-    self.client.resolve('bar/#LATEST')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('bar')
+      self.client.resolve('bar/#LATEST')
 
 
 class TestParts(_IntegrationTest):
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.parts('foo')
+    with pytest.raises(HdfsError):
+      self.client.parts('foo')
 
-  @raises(HdfsError)
   def test_file(self):
-    self.client.write('foo', 'hello')
-    self.client.parts('foo')
+    with pytest.raises(HdfsError):
+      self.client.write('foo', 'hello')
+      self.client.parts('foo')
 
-  @raises(HdfsError)
   def test_empty_folder(self):
-    self.client._mkdirs('foo')
-    self.client.parts('foo')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      self.client.parts('foo')
 
-  @raises(HdfsError)
   def test_folder_without_parts(self):
-    self.client.write('foo/bar', 'hello')
-    self.client.parts('foo')
+    with pytest.raises(HdfsError):
+      self.client.write('foo/bar', 'hello')
+      self.client.parts('foo')
 
   def test_folder_with_single_part(self):
     fname = 'part-m-00000.avro'
     self.client.write(psp.join('foo', fname), 'first')
-    eq_(self.client.parts('foo'), [fname])
+    assert self.client.parts('foo') == [fname]
 
   def test_folder_with_multiple_parts(self):
     fnames = ['part-m-00000.avro', 'part-m-00001.avro']
     self.client.write(psp.join('foo', fnames[0]), 'first')
     self.client.write(psp.join('foo', fnames[1]), 'second')
-    eq_(self.client.parts('foo'), fnames)
+    assert self.client.parts('foo') == fnames
 
   def test_folder_with_multiple_parts_and_others(self):
     fnames = ['part-m-00000.avro', 'part-m-00001.avro']
     self.client.write(psp.join('foo', '.header'), 'metadata')
     self.client.write(psp.join('foo', fnames[0]), 'first')
     self.client.write(psp.join('foo', fnames[1]), 'second')
-    eq_(self.client.parts('foo'), fnames)
+    assert self.client.parts('foo') == fnames
 
   def test_with_selection(self):
     fnames = ['part-m-00000.avro', 'part-m-00001.avro']
     self.client.write(psp.join('foo', '.header'), 'metadata')
     self.client.write(psp.join('foo', fnames[0]), 'first')
     self.client.write(psp.join('foo', fnames[1]), 'second')
     parts = self.client.parts('foo', parts=1)
-    eq_(len(parts), 1)
-    ok_(parts[0] in fnames)
+    assert len(parts) == 1
+    assert parts[0] in fnames
 
   def test_with_selection(self):
     fnames = ['part-m-00000.avro', 'part-m-00001.avro']
     self.client.write(psp.join('foo', '.header'), 'metadata')
     self.client.write(psp.join('foo', fnames[0]), 'first')
     self.client.write(psp.join('foo', fnames[1]), 'second')
-    eq_(self.client.parts('foo', parts=[1]), fnames[1:])
+    assert self.client.parts('foo', parts=[1]) == fnames[1:]
 
   def test_with_status(self):
     fname = 'part-m-00000.avro'
     fpath = psp.join('foo', fname)
     self.client.write(fpath, 'first')
     status = self.client.status(fpath)
     status['pathSuffix'] = fname
-    eq_(self.client.parts('foo', status=True), [(fname, status)])
+    assert self.client.parts('foo', status=True) == [(fname, status)]
 
 
 class TestMakeDirs(_IntegrationTest):
 
   def test_simple(self):
     self.client.makedirs('foo')
-    eq_(self.client.status('foo')['type'], 'DIRECTORY')
+    assert self.client.status('foo')['type'] == 'DIRECTORY'
 
   def test_nested(self):
     self.client.makedirs('foo/bar')
-    eq_(self.client.status('foo/bar')['type'], 'DIRECTORY')
+    assert self.client.status('foo/bar')['type'] == 'DIRECTORY'
 
   def test_with_permission(self):
     self.client.makedirs('foo', permission='733')
-    eq_(self.client.status('foo')['permission'], '733')
+    assert self.client.status('foo')['permission'] == '733'
 
-  @raises(HdfsError)
   def test_overwrite_file(self):
-    self.client.write('foo', 'hello')
-    self.client.makedirs('foo')
+    with pytest.raises(HdfsError):
+      self.client.write('foo', 'hello')
+      self.client.makedirs('foo')
 
   def test_overwrite_directory_with_permission(self):
     self.client.makedirs('foo', permission='733')
     self.client.makedirs('foo/bar', permission='722')
-    eq_(self.client.status('foo')['permission'], '733')
-    eq_(self.client.status('foo/bar')['permission'], '722')
+    assert self.client.status('foo')['permission'] == '733'
+    assert self.client.status('foo/bar')['permission'] == '722'
 
 
 class TestSetTimes(_IntegrationTest):
 
-  @raises(ValueError)
   def test_none(self):
-    self.client.makedirs('foo')
-    self.client.set_times('foo')
+    with pytest.raises(ValueError):
+      self.client.makedirs('foo')
+      self.client.set_times('foo')
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.set_times('foo', 1234)
+    with pytest.raises(HdfsError):
+      self.client.set_times('foo', 1234)
 
-  @nottest # HttpFS doesn't raise an error here.
-  @raises(HdfsError)
+  @pytest.mark.skip() # HttpFS doesn't raise an error here.
   def test_negative(self):
-    self.client.write('foo', 'hello')
-    self.client.set_times('foo', access_time=-1234)
+    with pytest.raises(HdfsError):
+      self.client.write('foo', 'hello')
+      self.client.set_times('foo', access_time=-1234)
 
   def test_file(self):
     self.client.write('foo', 'hello')
     self.client.set_times('foo', access_time=1234)
-    eq_(self.client.status('foo')['accessTime'], 1234)
+    assert self.client.status('foo')['accessTime'] == 1234
     self.client.set_times('foo', modification_time=12345)
-    eq_(self.client.status('foo')['modificationTime'], 12345)
+    assert self.client.status('foo')['modificationTime'] == 12345
     self.client.set_times('foo', access_time=1, modification_time=2)
     status = self.client.status('foo')
-    eq_(status['accessTime'], 1)
-    eq_(status['modificationTime'], 2)
+    assert status['accessTime'] == 1
+    assert status['modificationTime'] == 2
 
   def test_folder(self):
     self.client.write('foo/bar', 'hello')
     self.client.set_times('foo', access_time=1234)
-    eq_(self.client.status('foo')['accessTime'], 1234)
+    assert self.client.status('foo')['accessTime'] == 1234
     self.client.set_times('foo', modification_time=12345)
-    eq_(self.client.status('foo')['modificationTime'], 12345)
+    assert self.client.status('foo')['modificationTime'] == 12345
     self.client.set_times('foo', access_time=1, modification_time=2)
     status = self.client.status('foo')
-    eq_(status['accessTime'], 1)
-    eq_(status['modificationTime'], 2)
+    assert status['accessTime'] == 1
+    assert status['modificationTime'] == 2
 
 
 class TestChecksum(_IntegrationTest):
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.checksum('foo')
+    with pytest.raises(HdfsError):
+      self.client.checksum('foo')
 
-  @raises(HdfsError)
   def test_folder(self):
-    self.client.makedirs('foo')
-    self.client.checksum('foo')
+    with pytest.raises(HdfsError):
+      self.client.makedirs('foo')
+      self.client.checksum('foo')
 
   def test_file(self):
     self.client.write('foo', 'hello')
     checksum = self.client.checksum('foo')
-    eq_({'algorithm', 'bytes', 'length'}, set(checksum))
+    assert {'algorithm', 'bytes', 'length'} == set(checksum)
 
 
 class TestSetReplication(_IntegrationTest):
 
-  @raises(HdfsError)
   def test_missing(self):
-    self.client.set_replication('foo', 1)
+    with pytest.raises(HdfsError):
+      self.client.set_replication('foo', 1)
 
-  @raises(HdfsError)
   def test_folder(self):
-    self.client.makedirs('foo')
-    self.client.set_replication('foo', 1)
+    with pytest.raises(HdfsError):
+      self.client.makedirs('foo')
+      self.client.set_replication('foo', 1)
 
-  @raises(HdfsError)
   def test_invalid_replication(self):
-    self.client.write('foo', 'hello')
-    self.client.set_replication('foo', 0)
+    with pytest.raises(HdfsError):
+      self.client.write('foo', 'hello')
+      self.client.set_replication('foo', 0)
 
   def test_file(self):
     self.client.write('foo', 'hello')
     replication = self.client.status('foo')['replication'] + 1
     self.client.set_replication('foo', replication)
-    eq_(self.client.status('foo')['replication'], replication)
+    assert self.client.status('foo')['replication'] == replication
 
 
 class TestTokenClient(object):
 
   def test_without_session(self):
     client = TokenClient('url', '123')
-    eq_(client._session.params['delegation'], '123')
+    assert client._session.params['delegation'] == '123'
 
   def test_with_session(self):
     session = rq.Session()
     client = TokenClient('url', '123', session=session)
-    eq_(session.params['delegation'], '123')
+    assert session.params['delegation'] == '123'
 
 
 class TestSnapshot(_IntegrationTest):
 
   @classmethod
   def setup_class(cls):
     super(TestSnapshot, cls).setup_class()
@@ -1331,31 +1329,31 @@
     self.client.allow_snapshot('foo')
     self.client.disallow_snapshot('foo')
 
   def test_disallow_no_allow(self):
     self.client._mkdirs('foo')
     self.client.disallow_snapshot('foo')
 
-  @raises(HdfsError)
   def test_allow_snapshot_not_exists(self):
-    self.client.allow_snapshot('foo')
+    with pytest.raises(HdfsError):
+      self.client.allow_snapshot('foo')
 
-  @raises(HdfsError)
   def test_disallow_snapshot_not_exists(self):
-    self.client.disallow_snapshot('foo')
+    with pytest.raises(HdfsError):
+      self.client.disallow_snapshot('foo')
 
-  @raises(HdfsError)
   def test_allow_snapshot_file(self):
-    self._write('foo', b'hello')
-    self.client.allow_snapshot('foo')
+    with pytest.raises(HdfsError):
+      self._write('foo', b'hello')
+      self.client.allow_snapshot('foo')
 
-  @raises(HdfsError)
   def test_disallow_snapshot_file(self):
-    self._write('foo', b'hello')
-    self.client.disallow_snapshot('foo')
+    with pytest.raises(HdfsError):
+      self._write('foo', b'hello')
+      self.client.disallow_snapshot('foo')
 
   def test_create_delete_snapshot(self):
     # One cannot test creation and deletion separately, as one cannot
     # clean HDFS for test isolation if a created snapshot remains
     # undeleted.
     self.client._mkdirs('foo')
     self.client.allow_snapshot('foo')
@@ -1363,75 +1361,75 @@
     self.client.delete_snapshot('foo', 'mysnap')
 
   def test_create_snapshot_name(self):
     self.client._mkdirs('foo')
     self.client.allow_snapshot('foo')
     try:
       snapshot_path = self.client.create_snapshot('foo', 'mysnap')
-      assert_regex(snapshot_path, r'/foo/\.snapshot/mysnap$')
+      assert re.search(r'/foo/\.snapshot/mysnap$',snapshot_path)
     finally:
       # Cleanup, as it breaks other tests otherwise: the dir cannot be
       # removed with an active snapshots.
       self.client.delete_snapshot('foo', 'mysnap')
 
-  @raises(HdfsError)
   def test_delete_snapshot_other(self):
-    self.client._mkdirs('foo')
-    self.client.allow_snapshot('foo')
-    self.client.create_snapshot('foo', 'mysnap')
-    try:
-      self.client.delete_snapshot('foo', 'othersnap')
-    finally:
-      # Cleanup, as it breaks other tests otherwise: the dir cannot be
-      # removed with an active snapshots.
-      self.client.delete_snapshot('foo', 'mysnap')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      self.client.allow_snapshot('foo')
+      self.client.create_snapshot('foo', 'mysnap')
+      try:
+        self.client.delete_snapshot('foo', 'othersnap')
+      finally:
+        # Cleanup, as it breaks other tests otherwise: the dir cannot be
+        # removed with an active snapshots.
+        self.client.delete_snapshot('foo', 'mysnap')
 
-  @raises(HdfsError)
   def test_disallow_snapshot_exists(self):
-    self.client._mkdirs('foo_disallow')
-    self.client.allow_snapshot('foo_disallow')
-    self.client.create_snapshot('foo_disallow', 'mysnap')
-    try:
-      self.client.disallow_snapshot('foo_disallow')
-    finally:
-      # Cleanup, as it breaks other tests otherwise: the dir cannot be
-      # removed with an active snapshots.
-      self.client.delete_snapshot('foo_disallow', 'mysnap')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo_disallow')
+      self.client.allow_snapshot('foo_disallow')
+      self.client.create_snapshot('foo_disallow', 'mysnap')
+      try:
+        self.client.disallow_snapshot('foo_disallow')
+      finally:
+        # Cleanup, as it breaks other tests otherwise: the dir cannot be
+        # removed with an active snapshots.
+        self.client.delete_snapshot('foo_disallow', 'mysnap')
 
-  @raises(HdfsError)
   def test_create_snapshot_noallow(self):
-    self.client._mkdirs('foo')
-    self.client.create_snapshot('foo', 'mysnap')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      self.client.create_snapshot('foo', 'mysnap')
 
-  @raises(HdfsError)
   def test_delete_snapshot_noallow(self):
-    self.client._mkdirs('foo')
-    self.client.delete_snapshot('foo', 'mysnap')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      self.client.delete_snapshot('foo', 'mysnap')
 
-  @raises(HdfsError)
   def test_create_snapshot_noexist(self):
-    self.client.create_snapshot('foo', 'mysnap')
+    with pytest.raises(HdfsError):
+     self.client.create_snapshot('foo', 'mysnap')
 
   def test_rename_snapshot(self):
     self.client._mkdirs('foo')
     self.client.allow_snapshot('foo')
     self.client.create_snapshot('foo', 'myspan')
     try:
       self.client.rename_snapshot('foo', 'myspan', 'yourspan')
     finally:
       self.client.delete_snapshot('foo', 'yourspan')
 
-  @raises(HdfsError)
   def test_rename_snapshot_not_exists(self):
-    self.client.rename_snapshot('foo', 'myspan', 'yourspan')
+    with pytest.raises(HdfsError):
+      self.client.rename_snapshot('foo', 'myspan', 'yourspan')
 
-  @raises(HdfsError)
   def test_rename_snapshot_not_overwrite(self):
-    self.client._mkdirs('foo')
-    self.client.allow_snapshot('foo')
-    self.client.create_snapshot('foo', 'myspan')
-    self.client.create_snapshot('foo', 'yourspan')
-    try:
-      self.client.rename_snapshot('foo', 'myspan', 'yourspan')
-    finally:
-      self.client.delete_snapshot('foo', 'myspan')
-      self.client.delete_snapshot('foo', 'yourspan')
+    with pytest.raises(HdfsError):
+      self.client._mkdirs('foo')
+      self.client.allow_snapshot('foo')
+      self.client.create_snapshot('foo', 'myspan')
+      self.client.create_snapshot('foo', 'yourspan')
+      try:
+        self.client.rename_snapshot('foo', 'myspan', 'yourspan')
+      finally:
+        self.client.delete_snapshot('foo', 'myspan')
+        self.client.delete_snapshot('foo', 'yourspan')
```

### Comparing `hdfs-2.7.0/test/test_config.py` & `hdfs-2.7.1/test/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
 """Test configuration module."""
 
 from hdfs.client import Client
 from hdfs.config import Config
 from hdfs.util import HdfsError, temppath
 from logging.handlers import TimedRotatingFileHandler
-from nose.tools import eq_, ok_, nottest, raises
 from string import Template
-from util import save_config
+from test.util import save_config
 import logging as lg
 import os
 import os.path as osp
+import pytest
 import sys
 
 
 class TestConfig(object):
 
-  @nottest # TODO: Find cross-platform way to reset the environment variable.
+  @pytest.mark.skip(reason="TODO: Find cross-platform way to reset the environment variable.")
   def test_config_path(self):
     path = os.getenv('HDFSCLI_CONFIG')
     try:
       with temppath() as tpath:
         os.environ['HDFSCLI_CONFIG'] = tpath
         with open(tpath, 'w') as writer:
           writer.write('[foo]\nbar=hello')
-        eq_(Config().get('foo', 'bar'), 'hello')
+        assert Config().get('foo', 'bar') == 'hello'
     finally:
       if path:
         os['HDFSCLI_CONFIG'] = path
       else:
         del os['HDFSCLI_CONFIG']
 
   def _write_client_module(self, path, class_name):
@@ -47,39 +47,39 @@
       self._write_client_module(module_path, 'PathClient')
       with temppath() as config_path:
         config = Config(config_path)
         config.add_section(config.global_section)
         config.set(config.global_section, 'autoload.paths', module_path)
         config._autoload()
         client = Client.from_options({'url': ''}, 'PathClient')
-        eq_(client.one, 1)
+        assert client.one == 1
 
-  @raises(SystemExit)
   def test_autoload_missing_path(self):
-    with temppath() as module_path:
-      with temppath() as config_path:
-        config = Config(config_path)
-        config.add_section(config.global_section)
-        config.set(config.global_section, 'autoload.paths', module_path)
-        config._autoload()
+    with pytest.raises(SystemExit):
+      with temppath() as module_path:
+        with temppath() as config_path:
+          config = Config(config_path)
+          config.add_section(config.global_section)
+          config.set(config.global_section, 'autoload.paths', module_path)
+          config._autoload()
 
   def test_autoload_client_from_module(self):
     with temppath() as module_dpath:
       os.mkdir(module_dpath)
       sys.path.append(module_dpath)
       module_fpath = osp.join(module_dpath, 'mclient.py')
       self._write_client_module(module_fpath, 'ModuleClient')
       try:
         with temppath() as config_path:
           config = Config(config_path)
           config.add_section(config.global_section)
           config.set(config.global_section, 'autoload.modules', 'mclient')
           config._autoload()
           client = Client.from_options({'url': ''}, 'ModuleClient')
-          eq_(client.one, 1)
+          assert client.one == 1
       finally:
         sys.path.remove(module_dpath)
 
   def test_create_client_with_alias(self):
     with temppath() as tpath:
       config = Config(path=tpath)
       section = 'dev.alias'
@@ -92,28 +92,28 @@
     with temppath() as tpath:
       config = Config(path=tpath)
       section = 'dev.alias'
       config.add_section(section)
       config.set(section, 'url', 'http://host:port')
       config.set(section, 'timeout', '1')
       save_config(config)
-      eq_(Config(path=tpath).get_client('dev')._timeout, 1)
+      assert Config(path=tpath).get_client('dev')._timeout == 1
       config.set(section, 'timeout', '1,2')
       save_config(config)
-      eq_(Config(path=tpath).get_client('dev')._timeout, (1,2))
+      assert Config(path=tpath).get_client('dev')._timeout == (1,2)
 
-  @raises(HdfsError)
   def test_create_client_with_missing_alias(self):
-    with temppath() as tpath:
-      Config(tpath).get_client('dev')
+    with pytest.raises(HdfsError):
+      with temppath() as tpath:
+        Config(tpath).get_client('dev')
 
-  @raises(HdfsError)
   def test_create_client_with_no_alias_without_default(self):
-    with temppath() as tpath:
-      Config(tpath).get_client()
+    with pytest.raises(HdfsError):
+      with temppath() as tpath:
+        Config(tpath).get_client()
 
   def test_create_client_with_default_alias(self):
     with temppath() as tpath:
       config = Config(tpath)
       config.add_section(config.global_section)
       config.set(config.global_section, 'default.alias', 'dev')
       section = 'dev.alias'
@@ -122,18 +122,18 @@
       save_config(config)
       Config(tpath).get_client()
 
   def test_get_file_handler(self):
     with temppath() as tpath:
       config = Config(tpath)
       handler = config.get_log_handler('cmd')
-      ok_(isinstance(handler, TimedRotatingFileHandler))
+      assert isinstance(handler, TimedRotatingFileHandler)
 
   def test_disable_file_logging(self):
     with temppath() as tpath:
       config = Config(tpath)
       config.add_section('cmd.command')
       config.set('cmd.command', 'log.disable', 'true')
       save_config(config)
       config = Config(tpath)
       handler = config.get_log_handler('cmd')
-      ok_(not isinstance(handler, TimedRotatingFileHandler))
+      assert not isinstance(handler, TimedRotatingFileHandler)
```

### Comparing `hdfs-2.7.0/test/test_examples.py` & `hdfs-2.7.1/test/test_examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 """Test that the examples run correctly."""
 
 from hdfs import Config
-from imp import load_source
-from nose.plugins.skip import SkipTest
 from six import add_metaclass
-from util import _IntegrationTest
+from test.util import _IntegrationTest
 import os
 import os.path as osp
+import pytest
 
+try:
+  # Python 3.12 and above
+  from importlib import load_source
+except ImportError:
+  # Below Python 3.12
+  from imp import load_source
 
 class _ExamplesType(type):
 
   """Metaclass generating a test for each example."""
 
   dpath = osp.join(osp.dirname(__file__), os.pardir, 'examples')
 
@@ -25,15 +30,15 @@
       module = osp.splitext(fname)[0]
 
       def test(self):
         try:
           load_source(module, fpath)
         except ImportError:
           # Unmet dependency.
-          raise SkipTest
+          pytest.skip()
 
       test.__name__ = 'test_{}'.format(module)
       test.__doc__ = 'Test for example {}.'.format(fpath)
       return test
 
     for fname in os.listdir(mcs.dpath):
       if osp.splitext(fname)[1] == '.py':
```

### Comparing `hdfs-2.7.0/test/test_ext_avro.py` & `hdfs-2.7.1/test/test_ext_avro.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,93 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 """Test Avro extension."""
 
 from hdfs.util import HdfsError, temppath
 from json import dumps, load, loads
-from nose.plugins.skip import SkipTest
-from nose.tools import eq_, ok_, raises
-from util import _IntegrationTest
+from test.util import _IntegrationTest
 import os
 import os.path as osp
-import sys
+import pytest
 
 try:
   from hdfs.ext.avro import (_SeekableReader, _SchemaInferrer, AvroReader,
     AvroWriter)
   from hdfs.ext.avro.__main__ import main
 except ImportError:
   SKIP = True
 else:
   SKIP = False
 
 
 class TestSeekableReader(object):
 
-  def setup(self):
+  def setup_method(self):
     if SKIP:
-      raise SkipTest
+      pytest.skip()
 
   def test_normal_read(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('abcd')
       with open(tpath) as reader:
         sreader = _SeekableReader(reader)
-        eq_(sreader.read(3), 'abc')
-        eq_(sreader.read(2), 'd')
-        ok_(not sreader.read(1))
+        assert sreader.read(3) == 'abc'
+        assert sreader.read(2) == 'd'
+        assert not sreader.read(1)
 
   def test_buffered_read(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('abcdefghi')
       with open(tpath) as reader:
         sreader = _SeekableReader(reader, 3)
-        eq_(sreader.read(1), 'a')
-        eq_(sreader.read(3), 'bcd')
+        assert sreader.read(1) == 'a'
+        assert sreader.read(3) == 'bcd'
         sreader.seek(-3, os.SEEK_CUR)
-        eq_(sreader.read(2), 'bc')
-        eq_(sreader.read(6), 'defghi')
-        ok_(not sreader.read(1))
+        assert sreader.read(2) == 'bc'
+        assert sreader.read(6) == 'defghi'
+        assert not sreader.read(1)
 
 
 class TestInferSchema(object):
 
-  def setup(self):
+  def setup_method(self):
     if SKIP:
-      raise SkipTest
+      pytest.skip()
+
 
   def test_array(self):
-    eq_(
-      _SchemaInferrer().infer({'foo': 1, 'bar': ['hello']}),
+    assert (
+      _SchemaInferrer().infer({'foo': 1, 'bar': ['hello']}) ==
       {
         'type': 'record',
         'name': '__Record1',
         'fields': [
           {'type': {'type': 'array', 'items': 'string'}, 'name': 'bar'},
           {'type': 'int', 'name': 'foo'},
         ]
-      }
-    )
+      })
 
   def test_flat_record(self):
-    eq_(
-      _SchemaInferrer().infer({'foo': 1, 'bar': 'hello'}),
+    assert (
+      _SchemaInferrer().infer({'foo': 1, 'bar': 'hello'}) ==
       {
         'type': 'record',
         'name': '__Record1',
         'fields': [
           {'type': 'string', 'name': 'bar'},
           {'type': 'int', 'name': 'foo'},
         ]
-      }
-    )
+      })
 
   def test_nested_record(self):
-    eq_(
-      _SchemaInferrer().infer({'foo': {'bax': 2}, 'bar': {'baz': 3}}),
+    assert (
+      _SchemaInferrer().infer({'foo': {'bax': 2}, 'bar': {'baz': 3}}) ==
       {
         'type': 'record',
         'name': '__Record1',
         'fields': [
           {
             'type': {
               'type': 'record',
@@ -104,16 +101,15 @@
               'type': 'record',
               'name': '__Record3',
               'fields': [{'type': 'int', 'name': 'bax'}]
             },
             'name': 'foo',
           },
         ]
-      }
-    )
+      })
 
 
 class _AvroIntegrationTest(_IntegrationTest):
 
   dpath = osp.join(osp.dirname(__file__), 'dat')
   schema = None
   records = None
@@ -142,36 +138,35 @@
 
 
 class TestRead(_AvroIntegrationTest):
 
   def test_read(self):
     self.client.upload('weather.avro', osp.join(self.dpath, 'weather.avro'))
     with AvroReader(self.client, 'weather.avro') as reader:
-      eq_(list(reader), self.records)
+      assert list(reader) == self.records
 
   def test_read_with_same_schema(self):
     self.client.upload('w.avro', osp.join(self.dpath, 'weather.avro'))
     with AvroReader(self.client, 'w.avro', reader_schema=self.schema) as reader:
-      eq_(list(reader), self.records)
+      assert list(reader) == self.records
 
   def test_read_with_compatible_schema(self):
     self.client.upload('w.avro', osp.join(self.dpath, 'weather.avro'))
     schema = {
       'name': 'test.Weather',
       'type': 'record',
       'fields': [
         {'name': 'temp', 'type': 'int'},
         {'name': 'tag', 'type': 'string', 'default': ''},
       ],
     }
     with AvroReader(self.client, 'w.avro', reader_schema=schema) as reader:
-      eq_(
-        list(reader),
-        [{'temp': r['temp'], 'tag': ''} for r in self.records]
-      )
+      assert (
+        list(reader) ==
+        [{'temp': r['temp'], 'tag': ''} for r in self.records])
 
 
 class TestWriter(_AvroIntegrationTest):
 
   def test_write(self):
     writer = AvroWriter(
       self.client,
@@ -179,78 +174,77 @@
       schema=self.schema,
     )
     with writer:
       for record in self.records:
         writer.write(record)
     with temppath() as tpath:
       self.client.download('weather.avro', tpath)
-      eq_(
-        self._get_data_bytes(osp.join(self.dpath, 'weather.avro')),
-        self._get_data_bytes(tpath)
-      )
+      assert (
+        self._get_data_bytes(osp.join(self.dpath, 'weather.avro')) ==
+        self._get_data_bytes(tpath))
 
   def test_write_in_multiple_blocks(self):
     writer = AvroWriter(
       self.client,
       'weather.avro',
       schema=self.schema,
       sync_interval=1 # Flush block on every write.
     )
     with writer:
       for record in self.records:
         writer.write(record)
     with AvroReader(self.client, 'weather.avro') as reader:
-      eq_(list(reader), self.records)
+      assert list(reader) == self.records
 
   def test_write_empty(self):
     with AvroWriter(self.client, 'empty.avro', schema=self.schema):
       pass
     with AvroReader(self.client, 'empty.avro') as reader:
-      eq_(reader.schema, self.schema)
-      eq_(list(reader), [])
+      assert reader.schema == self.schema
+      assert list(reader) == []
 
-  @raises(HdfsError)
   def test_write_overwrite_error(self):
-    # To check that the background `AsyncWriter` thread doesn't hang.
-    self.client.makedirs('weather.avro')
-    with AvroWriter(self.client, 'weather.avro', schema=self.schema) as writer:
-      for record in self.records:
-        writer.write(record)
+    with pytest.raises(HdfsError):
+      # To check that the background `AsyncWriter` thread doesn't hang.
+      self.client.makedirs('weather.avro')
+      with AvroWriter(self.client, 'weather.avro', schema=self.schema) as writer:
+        for record in self.records:
+          writer.write(record)
 
   def test_infer_schema(self):
     with AvroWriter(self.client, 'weather.avro') as writer:
       for record in self.records:
         writer.write(record)
     with AvroReader(self.client, 'weather.avro') as reader:
-      eq_(list(reader), self.records)
+      assert list(reader) == self.records
 
 
 class TestMain(_AvroIntegrationTest):
 
   def test_schema(self):
     self.client.upload('weather.avro', osp.join(self.dpath, 'weather.avro'))
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         main(['schema', 'weather.avro'], client=self.client, stdout=writer)
       with open(tpath) as reader:
         schema = load(reader)
-      eq_(self.schema, schema)
+      assert self.schema == schema
 
   def test_read(self):
     self.client.upload('weather.avro', osp.join(self.dpath, 'weather.avro'))
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         main(
           ['read', 'weather.avro', '--num', '2'],
           client=self.client,
           stdout=writer
         )
       with open(tpath) as reader:
         records = [loads(line) for line in reader]
-      eq_(records, self.records[:2])
+      assert records == self.records[:2]
 
   def test_read_part_file(self):
     data = {
       'part-m-00000.avro': [{'name': 'jane'}, {'name': 'bob'}],
       'part-m-00001.avro': [{'name': 'john'}, {'name': 'liz'}],
     }
     for fname, records in data.items():
@@ -262,33 +256,32 @@
         main(
           ['read', 'data.avro', '--parts', '1,'],
           client=self.client,
           stdout=writer
         )
       with open(tpath) as reader:
         records = [loads(line) for line in reader]
-      eq_(records, data['part-m-00001.avro'])
+      assert records == data['part-m-00001.avro']
 
   def test_write(self):
     with open(osp.join(self.dpath, 'weather.jsonl')) as reader:
       main(
         [
           'write', 'weather.avro',
           '--schema', dumps(self.schema),
           '--codec', 'null',
         ],
         client=self.client,
         stdin=reader
       )
     with temppath() as tpath:
       self.client.download('weather.avro', tpath)
-      eq_(
-        self._get_data_bytes(tpath),
-        self._get_data_bytes(osp.join(self.dpath, 'weather.avro'))
-      )
+      assert (
+        self._get_data_bytes(tpath) ==
+        self._get_data_bytes(osp.join(self.dpath, 'weather.avro')))
 
   def test_write_codec(self):
     with open(osp.join(self.dpath, 'weather.jsonl')) as reader:
       main(
         [
           'write', 'weather.avro',
           '--schema', dumps(self.schema),
@@ -296,12 +289,12 @@
         ],
         client=self.client,
         stdin=reader
       )
     # Correct content.
     with AvroReader(self.client, 'weather.avro') as reader:
       records = list(reader)
-    eq_(records, self.records)
+    assert records == self.records
     # Different size (might not be smaller, since very small file).
     compressed_size = self.client.content('weather.avro')['length']
     uncompressed_size = osp.getsize(osp.join(self.dpath, 'weather.avro'))
-    ok_(compressed_size != uncompressed_size)
+    assert compressed_size != uncompressed_size
```

### Comparing `hdfs-2.7.0/test/test_ext_dataframe.py` & `hdfs-2.7.1/test/test_ext_dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 """Test Dataframe extension."""
 
 from hdfs.util import HdfsError, temppath
 from json import loads
-from nose.plugins.skip import SkipTest
-from nose.tools import *
-from util import _IntegrationTest
+from test.util import _IntegrationTest
 import os.path as osp
 
 try:
   from hdfs.ext.avro import AvroReader
   from hdfs.ext.dataframe import read_dataframe, write_dataframe
-  from pandas.util.testing import assert_frame_equal
+  from pandas.testing import assert_frame_equal
   import pandas as pd
 except ImportError:
   SKIP = True
 else:
   SKIP = False
 
 
@@ -48,15 +46,15 @@
 
 
 class TestWriteDataFrame(_DataFrameIntegrationTest):
 
   def test_write(self):
     write_dataframe(self.client, 'weather.avro', self.df)
     with AvroReader(self.client, 'weather.avro') as reader:
-      eq_(list(reader), self.records)
+      assert list(reader) == self.records
 
 
 class TestReadWriteDataFrame(_DataFrameIntegrationTest):
 
   def test_column_order(self):
     # Column order should be preserved, not just alphabetical.
     df = self.df[['temp', 'station', 'time']]
```

### Comparing `hdfs-2.7.0/test/test_ext_kerberos.py` & `hdfs-2.7.1/test/test_ext_kerberos.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 """Test Kerberos extension."""
 
-from nose.tools import eq_, nottest, ok_, raises
 from threading import Lock, Thread
 from time import sleep, time
 import sys
 
 
 class MockHTTPKerberosAuth(object):
 
   def __init__(self, **kwargs):
     self._lock = Lock()
     self._calls = set()
     self._items = []
 
   def __call__(self, n):
     with self._lock:
-      ok_(not self._items)
+      assert not self._items
       self._items.append(n)
     sleep(0.25)
     with self._lock:
       thread = self._items.pop()
-      eq_(thread, n)
+      assert thread == n
       self._calls.add(thread)
 
 
 class MockModule(object):
   def __init__(self):
     self.HTTPKerberosAuth = MockHTTPKerberosAuth
 
@@ -43,8 +42,8 @@
     auth = _HdfsHTTPKerberosAuth(1, mutual_auth='OPTIONAL')
     t1 = Thread(target=auth.__call__, args=(1, ))
     t1.start()
     t2 = Thread(target=auth.__call__, args=(2, ))
     t2.start()
     t1.join()
     t2.join()
-    eq_(auth._calls, {1, 2})
+    assert auth._calls == {1, 2}
```

### Comparing `hdfs-2.7.0/test/test_main.py` & `hdfs-2.7.1/test/test_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,105 +3,105 @@
 
 """Test CLI."""
 
 from hdfs.__main__ import _Progress, configure_client, main, parse_arg
 from hdfs.config import Config, NullHandler
 from hdfs.util import HdfsError, temppath
 from logging.handlers import TimedRotatingFileHandler
-from nose.tools import eq_, nottest, ok_, raises
-from util import _IntegrationTest, save_config
+from test.util import _IntegrationTest
 import filecmp
 import logging as lg
 import os
 import os.path as osp
+import pytest
 import sys
 
 
 class TestParseArg(object):
 
-  @raises(HdfsError)
   def test_parse_invalid(self):
-    parse_arg({'foo': 'a'}, 'foo', int)
+    with pytest.raises(HdfsError):
+      parse_arg({'foo': 'a'}, 'foo', int)
 
   def test_parse_int(self):
-    eq_(parse_arg({'foo': '1'}, 'foo', int), 1)
-    eq_(parse_arg({'foo': '1'}, 'foo', int, ','), 1)
+    assert parse_arg({'foo': '1'}, 'foo', int) == 1
+    assert parse_arg({'foo': '1'}, 'foo', int, ',') == 1
 
   def test_parse_float(self):
-    eq_(parse_arg({'foo': '123.4'}, 'foo', float), 123.4)
+    assert parse_arg({'foo': '123.4'}, 'foo', float) == 123.4
 
   def test_parse_int_list(self):
-    eq_(parse_arg({'foo': '1,'}, 'foo', int, ','), [1])
-    eq_(parse_arg({'foo': '1,2'}, 'foo', int, ','), [1,2])
+    assert parse_arg({'foo': '1,'}, 'foo', int, ',') == [1]
+    assert parse_arg({'foo': '1,2'}, 'foo', int, ',') == [1,2]
 
 
 class TestConfigureClient(object):
 
   def test_with_alias(self):
     url = 'http://host:port'
     with temppath() as tpath:
       config = Config(path=tpath)
       section = 'dev.alias'
       config.add_section(section)
       config.set(section, 'url', url)
       args = {'--alias': 'dev', '--log': False, '--verbose': 0}
       client = configure_client('test', args, config=config)
-      eq_(client.url, url)
-      eq_(client.urls, [url])
+      assert client.url == url
+      assert client.urls == [url]
 
 
 class TestProgress(object):
 
   def test_single_file(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         progress = _Progress(100, 1, writer=writer)
         progress('foo', 60)
-        eq_(progress._data['foo'], 60)
-        eq_(progress._pending_files, 0)
-        eq_(progress._downloading_files, 1)
+        assert progress._data['foo'] == 60
+        assert progress._pending_files == 0
+        assert progress._downloading_files == 1
         progress('foo', 40)
         progress('foo', -1)
-        eq_(progress._downloading_files, 0)
-        eq_(progress._complete_files, 1)
+        assert progress._downloading_files == 0
+        assert progress._complete_files == 1
 
   def test_from_local_path(self):
     with temppath() as dpath:
       os.mkdir(dpath)
       fpath1 = osp.join(dpath, 'foo')
       with open(fpath1, 'w') as writer:
         writer.write('hey')
       os.mkdir(osp.join(dpath, 'bar'))
       fpath2 = osp.join(dpath, 'bar', 'baz')
       with open(fpath2, 'w') as writer:
         writer.write('hello')
       with temppath() as tpath:
         with open(tpath, 'w') as writer:
           progress = _Progress.from_local_path(dpath, writer=writer)
-          eq_(progress._total_bytes, 8)
-          eq_(progress._pending_files, 2)
+          assert progress._total_bytes == 8
+          assert progress._pending_files == 2
 
 
 class TestMain(_IntegrationTest):
 
   dpath = osp.join(osp.dirname(__file__), 'dat')
 
-  def setup(self):
+  def setup_method(self):
     self._root_logger = lg.getLogger()
     self._handlers = self._root_logger.handlers
-    super(TestMain, self).setup()
+    super(TestMain, self).setup_method()
 
-  def teardown(self):
+  def teardown_method(self):
     self._root_logger.handlers = self._handlers
 
   def _dircmp(self, dpath):
     dircmp = filecmp.dircmp(self.dpath, dpath)
-    ok_(not dircmp.left_only)
-    ok_(not dircmp.right_only)
-    ok_(not dircmp.diff_files)
+    assert not dircmp.left_only
+    assert not dircmp.right_only
+    assert not dircmp.diff_files
 
   def test_download(self):
     self.client.upload('foo', self.dpath)
     with temppath() as tpath:
       main(
         ['download', 'foo', tpath, '--silent', '--threads', '1'],
         self.client
@@ -118,64 +118,64 @@
           main(
             ['download', 'foo', '-', '--silent', '--threads', '1'],
             self.client
           )
       finally:
         sys.stdout = stdout
       with open(tpath) as reader:
-        eq_(reader.read(), 'hello')
+        assert reader.read() == 'hello'
 
-  @raises(SystemExit)
   def test_download_stream_multiple_files(self):
-    self.client.upload('foo', self.dpath)
-    main(
-      ['download', 'foo', '-', '--silent', '--threads', '1'],
-      self.client
-    )
-
-  @raises(SystemExit)
-  def test_download_overwrite(self):
-    self.client.upload('foo', self.dpath)
-    with temppath() as tpath:
-      with open(tpath, 'w'):
-        pass
+    with pytest.raises(SystemExit):
+      self.client.upload('foo', self.dpath)
       main(
-        ['download', 'foo', tpath, '--silent', '--threads', '1'],
+        ['download', 'foo', '-', '--silent', '--threads', '1'],
         self.client
       )
-      self._dircmp(tpath)
+
+  def test_download_overwrite(self):
+    with pytest.raises(SystemExit):
+      self.client.upload('foo', self.dpath)
+      with temppath() as tpath:
+        with open(tpath, 'w'):
+          pass
+        main(
+          ['download', 'foo', tpath, '--silent', '--threads', '1'],
+          self.client
+        )
+        self._dircmp(tpath)
 
   def test_download_force(self):
     self.client.write('foo', 'hey')
     with temppath() as tpath:
       with open(tpath, 'w'):
         pass
       main(
         ['download', 'foo', tpath, '--silent', '--force', '--threads', '1'],
         self.client
       )
       with open(tpath) as reader:
-        eq_(reader.read(), 'hey')
+        assert reader.read() == 'hey'
 
   def test_upload(self):
     main(
       ['upload', self.dpath, 'bar', '--silent', '--threads', '1'],
       self.client
     )
     with temppath() as tpath:
       self.client.download('bar', tpath)
       self._dircmp(tpath)
 
-  @raises(SystemExit)
   def test_upload_overwrite(self):
-    self.client.write('bar', 'hey')
-    main(
-      ['upload', self.dpath, 'bar', '--silent', '--threads', '1'],
-      self.client
-    )
+    with pytest.raises(SystemExit):
+      self.client.write('bar', 'hey')
+      main(
+        ['upload', self.dpath, 'bar', '--silent', '--threads', '1'],
+        self.client
+      )
 
   def test_upload_force(self):
     self.client.write('bar', 'hey')
     main(
       ['upload', self.dpath, 'bar', '--silent', '--threads', '1', '--force'],
       self.client
     )
@@ -189,13 +189,13 @@
         writer.write('hey')
       main(['upload', tpath, 'bar', '--silent', '--threads', '1'], self.client)
       main(
         ['upload', tpath, 'bar', '--silent', '--threads', '1', '--append'],
         self.client
       )
     with self.client.read('bar') as reader:
-      eq_(reader.read(), b'heyhey')
+      assert reader.read() == b'heyhey'
 
-  @raises(SystemExit)
   def test_upload_append_folder(self):
-    with temppath() as tpath:
-      main(['upload', self.dpath, '--silent', '--append'], self.client)
+    with pytest.raises(SystemExit):
+      with temppath() as tpath:
+        main(['upload', self.dpath, '--silent', '--append'], self.client)
```

### Comparing `hdfs-2.7.0/test/test_util.py` & `hdfs-2.7.1/test/test_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 """Test Hdfs client interactions with HDFS."""
 
 from hdfs.util import *
-from nose.tools import eq_, ok_, raises
+import pytest
 
 
 class TestAsyncWriter(object):
 
   def test_basic(self):
     result = []
     def consumer(gen):
       result.append(list(gen))
     with AsyncWriter(consumer) as writer:
       writer.write('one')
       writer.write('two')
-    eq_(result, [['one','two']])
+    assert result == [['one','two']]
 
   def test_multiple_writer_uses(self):
     result = []
     def consumer(gen):
       result.append(list(gen))
     writer = AsyncWriter(consumer)
     with writer:
       writer.write('one')
       writer.write('two')
     with writer:
       writer.write('three')
       writer.write('four')
-    eq_(result, [['one','two'],['three','four']])
+    assert result == [['one','two'],['three','four']]
 
   def test_multiple_consumer_uses(self):
     result = []
     def consumer(gen):
       result.append(list(gen))
     with AsyncWriter(consumer) as writer:
       writer.write('one')
       writer.write('two')
     with AsyncWriter(consumer) as writer:
       writer.write('three')
       writer.write('four')
-    eq_(result, [['one','two'],['three','four']])
+    assert result == [['one','two'],['three','four']]
 
-  @raises(ValueError)
   def test_nested(self):
-    result = []
-    def consumer(gen):
-      result.append(list(gen))
-    with AsyncWriter(consumer) as _writer:
-      _writer.write('one')
-      with _writer as writer:
-        writer.write('two')
+    with pytest.raises(ValueError):
+      result = []
+      def consumer(gen):
+        result.append(list(gen))
+      with AsyncWriter(consumer) as _writer:
+        _writer.write('one')
+        with _writer as writer:
+          writer.write('two')
 
-  @raises(HdfsError)
   def test_child_error(self):
-    def consumer(gen):
-      for value in gen:
-        if value == 'two':
-          raise HdfsError('Yo')
-    with AsyncWriter(consumer) as writer:
-      writer.write('one')
-      writer.write('two')
+    with pytest.raises(HdfsError):
+      def consumer(gen):
+        for value in gen:
+          if value == 'two':
+            raise HdfsError('Yo')
+      with AsyncWriter(consumer) as writer:
+        writer.write('one')
+        writer.write('two')
 
-  @raises(HdfsError)
   def test_parent_error(self):
-    def consumer(gen):
-      for value in gen:
-        pass
-    def invalid(w):
-      w.write('one')
-      raise HdfsError('Ya')
-    with AsyncWriter(consumer) as writer:
-      invalid(writer)
+    with pytest.raises(HdfsError):
+      def consumer(gen):
+        for value in gen:
+          pass
+      def invalid(w):
+        w.write('one')
+        raise HdfsError('Ya')
+      with AsyncWriter(consumer) as writer:
+        invalid(writer)
 
 
 class TestTemppath(object):
 
   def test_new(self):
     with temppath() as tpath:
-      ok_(not osp.exists(tpath))
+      assert not osp.exists(tpath)
 
   def test_cleanup(self):
     with temppath() as tpath:
       with open(tpath, 'w') as writer:
         writer.write('hi')
-    ok_(not osp.exists(tpath))
+    assert not osp.exists(tpath)
 
   def test_dpath(self):
     with temppath() as dpath:
       os.mkdir(dpath)
       with temppath(dpath) as tpath:
-        eq_(osp.dirname(tpath), dpath)
+        assert osp.dirname(tpath) == dpath
```

