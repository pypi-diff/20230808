# Comparing `tmp/amazon_kclpy-2.1.2.tar.gz` & `tmp/amazon_kclpy-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_kclpy-2.1.2.tar", last modified: Thu Jun 29 22:14:58 2023, max compression
+gzip compressed data, was "amazon_kclpy-2.1.3.tar", last modified: Tue Aug  8 21:09:00 2023, max compression
```

## Comparing `amazon_kclpy-2.1.2.tar` & `amazon_kclpy-2.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)    10142 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/LICENSE.txt
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)       72 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/MANIFEST.in
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      114 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/NOTICE.txt
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      351 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/PKG-INFO
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)    17303 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/README.md
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      827 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/__init__.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      781 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/checkpoint_error.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     1839 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/dispatch.py
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/jars/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/jars/__init__.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)    12498 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/kcl.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)    13819 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/messages.py
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/v2/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      820 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v2/__init__.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     5308 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v2/processor.py
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/v3/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      820 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v3/__init__.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     5583 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v3/processor.py
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      351 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/PKG-INFO
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      776 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/SOURCES.txt
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)        1 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/dependency_links.txt
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)        1 2023-06-29 21:55:36.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/not-zip-safe
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)       14 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/requires.txt
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)       53 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/top_level.txt
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)    14075 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/pom.xml
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/samples/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     2741 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/__init__.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     7176 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/amazon_kclpy_helper.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     4573 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/sample.properties
--rwxr-xr-x   0 rmpelaez (23627871) amazon     (100)     6915 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/sample_kclpy_app.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     5706 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/sample_kinesis_wordputter.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)      104 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/setup.cfg
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     8728 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/setup.py
-drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/test/
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     3791 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/test/test_amazon_kclpy.py
--rw-r--r--   0 rmpelaez (23627871) amazon     (100)     3925 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/test/test_amazon_kclpy_input_output_integration.py
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)    10142 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/LICENSE.txt
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)       72 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/MANIFEST.in
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      114 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/NOTICE.txt
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      351 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/PKG-INFO
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)    17612 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/README.md
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.746161 amazon_kclpy-2.1.3/amazon_kclpy/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      827 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/__init__.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      781 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/checkpoint_error.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     1839 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/dispatch.py
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy/jars/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/jars/__init__.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)    12498 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/kcl.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)    13819 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/messages.py
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy/v2/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      820 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v2/__init__.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     5308 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v2/processor.py
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy/v3/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      820 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v3/__init__.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     5583 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v3/processor.py
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      351 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/PKG-INFO
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      776 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/SOURCES.txt
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)        1 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/dependency_links.txt
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)        1 2023-08-08 20:54:13.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/not-zip-safe
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)       14 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/requires.txt
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)       53 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/top_level.txt
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)    14135 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/pom.xml
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/samples/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     2741 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/__init__.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     7176 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/amazon_kclpy_helper.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     4755 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/sample.properties
+-rwxr-xr-x   0 brenplyn (23167224) amazon     (100)     6915 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/sample_kclpy_app.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     5706 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/sample_kinesis_wordputter.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)      104 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/setup.cfg
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     8728 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/setup.py
+drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/test/
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     3791 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/test/test_amazon_kclpy.py
+-rw-r--r--   0 brenplyn (23167224) amazon     (100)     3925 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/test/test_amazon_kclpy_input_output_integration.py
```

### Comparing `amazon_kclpy-2.1.2/LICENSE.txt` & `amazon_kclpy-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/README.md` & `amazon_kclpy-2.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,18 @@
 * The [Amazon KCL for Java][kinesis-github]
 * The [Amazon KCL for Ruby][amazon-kinesis-ruby-github]
 * The [Amazon Kinesis Documentation][amazon-kinesis-docs]
 * The [Amazon Kinesis Forum][kinesis-forum]
 
 ## Release Notes
 
+### Release 2.1.3 (August 8, 2023)
+* Added the ability to specify STS endpoint and region [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/230)
+* Upgraded KCL and KCL-Multilang Dependencies from 2.5.1 to 2.5.2 [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/230)
+
 ### Release 2.1.2 (June 29, 2023)
 * Added the ability to pass in streamArn to multilang Daemon [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/221)
 * Upgraded KCL and KCL-Multilang Dependencies from 2.4.4 to 2.5.1 [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/221)
 * Upgraded Google Guava dependency from 31.0.1-jre to 32.0.0-jre [PR #223](https://github.com/awslabs/amazon-kinesis-client-python/pull/223)
 * Added aws-java-sdk-sts dependency [PR #212](https://github.com/awslabs/amazon-kinesis-client-python/pull/212)
 
 ### Release 2.1.1 (January 17, 2023)
```

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/__init__.py` & `amazon_kclpy-2.1.3/amazon_kclpy/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/checkpoint_error.py` & `amazon_kclpy-2.1.3/amazon_kclpy/checkpoint_error.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/dispatch.py` & `amazon_kclpy-2.1.3/amazon_kclpy/dispatch.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/kcl.py` & `amazon_kclpy-2.1.3/amazon_kclpy/kcl.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/messages.py` & `amazon_kclpy-2.1.3/amazon_kclpy/messages.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/v2/__init__.py` & `amazon_kclpy-2.1.3/amazon_kclpy/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/v2/processor.py` & `amazon_kclpy-2.1.3/amazon_kclpy/v2/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/v3/__init__.py` & `amazon_kclpy-2.1.3/amazon_kclpy/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy/v3/processor.py` & `amazon_kclpy-2.1.3/amazon_kclpy/v3/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/amazon_kclpy.egg-info/SOURCES.txt` & `amazon_kclpy-2.1.3/amazon_kclpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/pom.xml` & `amazon_kclpy-2.1.3/pom.xml`

 * *Files 0% similar despite different names*

#### Comparing `amazon_kclpy-2.1.2/pom.xml` & `amazon_kclpy-2.1.3/pom.xml`

```diff
@@ -1,28 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <properties>
     <awssdk.version>2.19.2</awssdk.version>
     <aws-java-sdk.version>1.12.370</aws-java-sdk.version>
+    <kcl.version>2.5.2</kcl.version>
     <netty.version>4.1.86.Final</netty.version>
     <netty-reactive.version>2.0.6</netty-reactive.version>
     <fasterxml-jackson.version>2.13.4</fasterxml-jackson.version>
     <logback.version>1.3.0</logback.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>software.amazon.kinesis</groupId>
       <artifactId>amazon-kinesis-client-multilang</artifactId>
-      <version>2.5.1</version>
+      <version>${kcl.version}</version>
     </dependency>
     <dependency>
       <groupId>software.amazon.kinesis</groupId>
       <artifactId>amazon-kinesis-client</artifactId>
-      <version>2.5.1</version>
+      <version>${kcl.version}</version>
     </dependency>
     <dependency>
       <groupId>software.amazon.awssdk</groupId>
       <artifactId>kinesis</artifactId>
       <version>${awssdk.version}</version>
     </dependency>
     <dependency>
```

### Comparing `amazon_kclpy-2.1.2/samples/__init__.py` & `amazon_kclpy-2.1.3/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/samples/amazon_kclpy_helper.py` & `amazon_kclpy-2.1.3/samples/amazon_kclpy_helper.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/samples/sample.properties` & `amazon_kclpy-2.1.3/samples/sample.properties`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 # information for workers with this application name
 applicationName = PythonKCLSample
 
 # Users can change the credentials provider the KCL will use to retrieve credentials.
 # The DefaultAWSCredentialsProviderChain checks several other providers, which is
 # described here:
 # http://docs.aws.amazon.com/AWSJavaSDK/latest/javadoc/com/amazonaws/auth/DefaultAWSCredentialsProviderChain.html
+#
+# For additional configuration, including nested properties, see:
+# https://github.com/awslabs/amazon-kinesis-client/blob/master/docs/multilang/configuring-credential-providers.md
 AWSCredentialsProvider = DefaultAWSCredentialsProviderChain
 
 # Appended to the user agent of the KCL. Does not impact the functionality of the
 # KCL in any other way.
 processingLanguage = python/3.8
 
 # Valid options at TRIM_HORIZON or LATEST.
```

### Comparing `amazon_kclpy-2.1.2/samples/sample_kclpy_app.py` & `amazon_kclpy-2.1.3/samples/sample_kclpy_app.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/samples/sample_kinesis_wordputter.py` & `amazon_kclpy-2.1.3/samples/sample_kinesis_wordputter.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/setup.py` & `amazon_kclpy-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #
 # Will retrieve the configured jars from maven and then advise the user
 # to rerun the install command.
 #
 
 PACKAGE_NAME = 'amazon_kclpy'
 JAR_DIRECTORY = os.path.join(PACKAGE_NAME, 'jars')
-PACKAGE_VERSION = '2.1.2'
+PACKAGE_VERSION = '2.1.3'
 PYTHON_REQUIREMENTS = [
     'boto',
     # argparse is part of python2.7 but must be declared for python2.6
     'argparse',
 ]
 REMOTE_MAVEN_PACKAGES_FILE = 'pom.xml'
```

### Comparing `amazon_kclpy-2.1.2/test/test_amazon_kclpy.py` & `amazon_kclpy-2.1.3/test/test_amazon_kclpy.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.2/test/test_amazon_kclpy_input_output_integration.py` & `amazon_kclpy-2.1.3/test/test_amazon_kclpy_input_output_integration.py`

 * *Files identical despite different names*

