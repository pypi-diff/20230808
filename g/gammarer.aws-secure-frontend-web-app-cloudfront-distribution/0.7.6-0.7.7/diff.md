# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6.tar", last modified: Sun Aug  6 18:26:16 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7.tar", last modified: Mon Aug  7 18:28:09 2023, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:26:02.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:26:16.174967 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-06 18:26:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-06 18:26:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:26:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-06 18:26:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 18:26:16.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:28:09.913810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-07 18:28:09.913810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 18:28:09.913810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:28:09.909810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:28:09.909810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:28:09.913810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:28:09.913810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:27:57.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:28:09.909810 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-07 18:28:09.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-07 18:28:09.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:28:09.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-07 18:28:09.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 18:28:09.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.7.6
+Version: 0.7.7
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/README.md` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "0.7.6",
+    "version": "0.7.7",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@0.7.6.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@0.7.7.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.6.jsii.tgz` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.7.jsii.tgz`

 * *Files 26% similar despite different names*

#### Comparing `aws-secure-frontend-web-app-cloudfront-distribution@0.7.6.jsii.tgz-content` & `aws-secure-frontend-web-app-cloudfront-distribution@0.7.7.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'rE/NKE5Y0DXKhs/Zax7BzIJvVkGPy26QkGoNNhjvXvM='", "'version'": "'0.7.7'"}*

```diff
@@ -3057,15 +3057,15 @@
             }
         }
     },
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "GEYdxcb+71oGZGBVxNVFXnT5pQlp1oqFCgeRyGSDtFE=",
+    "fingerprint": "rE/NKE5Y0DXKhs/Zax7BzIJvVkGPy26QkGoNNhjvXvM=",
     "homepage": "https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "jsiiVersion": "1.86.1 (build defb235)",
     "keywords": [
         "angular",
         "aws",
         "cdk",
         "cdn",
@@ -3253,9 +3253,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/index:SecureFrontendWebAppCloudFrontDistributionProps"
         }
     },
-    "version": "0.7.6"
+    "version": "0.7.7"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -87,10 +87,10 @@
         });
     }
 }
 exports.SecureFrontendWebAppCloudFrontDistribution = SecureFrontendWebAppCloudFrontDistribution;
 _a = JSII_RTTI_SYMBOL_1;
 SecureFrontendWebAppCloudFrontDistribution[_a] = {
     fqn: "@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistribution",
-    version: "0.7.6"
+    version: "0.7.7"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSxtQ0FBbUM7QUFFbkMseURBQXlEO0FBQ3pELDhEQUE4RDtBQWE5RCxNQUFhLDBDQUEyQyxTQUFRLFVBQVUsQ0FBQyxZQUFZO0lBRXJGLFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBc0Q7UUFDOUYsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUU7WUFDZixPQUFPLEVBQUUsSUFBSTtZQUNiLE9BQU8sRUFBRSxLQUFLLENBQUMsT0FBTztZQUN0QixpQkFBaUIsRUFBRSxZQUFZO1lBQy9CLFdBQVcsRUFBRSxLQUFLLENBQUMsV0FBVztZQUM5QixXQUFXLEVBQUUsQ0FBQyxLQUFLLENBQUMsVUFBVSxDQUFDO1lBQy9CLHNCQUFzQixFQUFFLFVBQVUsQ0FBQyxzQkFBc0IsQ0FBQyxhQUFhO1lBQ3ZFLGdCQUFnQixFQUFFLFVBQVUsQ0FBQyxTQUFTLENBQUMsR0FBRztZQUMxQyxXQUFXLEVBQUUsVUFBVSxDQUFDLFdBQVcsQ0FBQyxXQUFXO1lBQy9DLDRCQUE0QjtZQUM1QixTQUFTLEVBQUUsS0FBSyxDQUFDLGVBQWU7WUFDaEMsYUFBYSxFQUFFLEtBQUssQ0FBQyxlQUFlLENBQUMsQ0FBQyxDQUFDLEdBQUcsS0FBSyxDQUFDLFVBQVUsR0FBRyxDQUFDLENBQUMsQ0FBQyxTQUFTO1lBQ3pFLGVBQWUsRUFBRTtnQkFDZixjQUFjLEVBQUUsVUFBVSxDQUFDLGNBQWMsQ0FBQyxzQkFBc0I7Z0JBQ2hFLGFBQWEsRUFBRSxVQUFVLENBQUMsYUFBYSxDQUFDLHNCQUFzQjtnQkFDOUQsV0FBVyxFQUFFLFVBQVUsQ0FBQyxXQUFXLENBQUMsaUJBQWlCO2dCQUNyRCxRQUFRLEVBQUUsSUFBSTtnQkFDZCxvQkFBb0IsRUFBRSxVQUFVLENBQUMsb0JBQW9CLENBQUMsVUFBVTtnQkFDaEUsTUFBTSxFQUFFLElBQUksT0FBTyxDQUFDLFFBQVEsQ0FBQyxLQUFLLENBQUMsWUFBWSxFQUFFO29CQUMvQyxvQkFBb0IsRUFBRSxLQUFLLENBQUMsb0JBQW9CO2lCQUNqRCxDQUFDO2dCQUNGLHFCQUFxQixFQUFFLElBQUksVUFBVSxDQUFDLHFCQUFxQixDQUFDLEtBQUssRUFBRSx1QkFBdUIsRUFBRTtvQkFDMUYsOEJBQThCO29CQUM5QixPQUFPLEVBQUUsa0JBQWtCO29CQUMzQix1QkFBdUIsRUFBRTt3QkFDdkIsMEZBQTBGO3dCQUMxRixrQkFBa0IsRUFBRSxFQUFFLFFBQVEsRUFBRSxJQUFJLEVBQUU7d0JBQ3RDLFlBQVksRUFBRTs0QkFDWixXQUFXLEVBQUUsVUFBVSxDQUFDLGtCQUFrQixDQUFDLFVBQVU7NEJBQ3JELFFBQVEsRUFBRSxJQUFJO3lCQUNmO3dCQUNELGNBQWMsRUFBRTs0QkFDZCxjQUFjLEVBQUUsVUFBVSxDQUFDLHFCQUFxQixDQUFDLCtCQUErQjs0QkFDaEYsUUFBUSxFQUFFLElBQUk7eUJBQ2Y7d0JBQ0QsdUJBQXVCLEVBQUU7NEJBQ3ZCLG1CQUFtQixFQUFFLEdBQUcsQ0FBQyxRQUFRLENBQUMsT0FBTyxDQUFDLFFBQVEsQ0FBQzs0QkFDbkQsT0FBTyxFQUFFLElBQUk7NEJBQ2IsaUJBQWlCLEVBQUUsSUFBSTs0QkFDdkIsUUFBUSxFQUFFLElBQUk7eUJBQ2Y7d0JBQ0QsYUFBYSxFQUFFOzRCQUNiLFVBQVUsRUFBRSxJQUFJOzRCQUNoQixTQUFTLEVBQUUsSUFBSTs0QkFDZixRQUFRLEVBQUUsSUFBSTt5QkFDZjtxQkFDRjtvQkFDRCxxQkFBcUIsRUFBRTt3QkFDckIsYUFBYSxFQUFFOzRCQUNiO2dDQUNFLE1BQU0sRUFBRSxlQUFlO2dDQUN2QixLQUFLLEVBQUUsNkJBQTZCO2dDQUNwQyxRQUFRLEVBQUUsSUFBSTs2QkFDZjs0QkFDRDtnQ0FDRSxNQUFNLEVBQUUsUUFBUTtnQ0FDaEIsS0FBSyxFQUFFLFVBQVU7Z0NBQ2pCLFFBQVEsRUFBRSxJQUFJOzZCQUNmO3lCQUNGO3FCQUNGO2lCQUNGLENBQUM7YUFDSDtZQUNELGNBQWMsRUFBRTtnQkFDZDtvQkFDRSxHQUFHLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxPQUFPLENBQUMsR0FBRyxDQUFDO29CQUM5QixVQUFVLEVBQUUsR0FBRztvQkFDZixrQkFBa0IsRUFBRSxHQUFHO29CQUN2QixnQkFBZ0IsRUFBRSxhQUFhO2lCQUNoQztnQkFDRDtvQkFDRSxHQUFHLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxPQUFPLENBQUMsR0FBRyxDQUFDO29CQUM5QixVQUFVLEVBQUUsR0FBRztvQkFDZixrQkFBa0IsRUFBRSxHQUFHO29CQUN2QixnQkFBZ0IsRUFBRSxhQUFhO2lCQUNoQzthQUNGO1lBQ0QsVUFBVSxFQUFFLFVBQVUsQ0FBQyxVQUFVLENBQUMsZUFBZTtTQUNsRCxDQUFDLENBQUM7SUFDTCxDQUFDOztBQWxGSCxnR0FtRkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBjZGsgZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0ICogYXMgYWNtIGZyb20gJ2F3cy1jZGstbGliL2F3cy1jZXJ0aWZpY2F0ZW1hbmFnZXInO1xuaW1wb3J0ICogYXMgY2xvdWRmcm9udCBmcm9tICdhd3MtY2RrLWxpYi9hd3MtY2xvdWRmcm9udCc7XG5pbXBvcnQgKiBhcyBvcmlnaW5zIGZyb20gJ2F3cy1jZGstbGliL2F3cy1jbG91ZGZyb250LW9yaWdpbnMnO1xuaW1wb3J0ICogYXMgczMgZnJvbSAnYXdzLWNkay1saWIvYXdzLXMzJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuXG5leHBvcnQgaW50ZXJmYWNlIFNlY3VyZUZyb250ZW5kV2ViQXBwQ2xvdWRGcm9udERpc3RyaWJ1dGlvblByb3BzIHtcbiAgcmVhZG9ubHkgY29tbWVudD86IHN0cmluZztcbiAgcmVhZG9ubHkgZG9tYWluTmFtZTogc3RyaW5nO1xuICByZWFkb25seSBjZXJ0aWZpY2F0ZTogYWNtLklDZXJ0aWZpY2F0ZTtcbiAgcmVhZG9ubHkgb3JpZ2luQnVja2V0OiBzMy5JQnVja2V0O1xuICByZWFkb25seSBvcmlnaW5BY2Nlc3NJZGVudGl0eTogY2xvdWRmcm9udC5JT3JpZ2luQWNjZXNzSWRlbnRpdHk7XG4gIHJlYWRvbmx5IGFjY2Vzc0xvZ0J1Y2tldD86IHMzLklCdWNrZXQ7XG59XG5cbmV4cG9ydCBjbGFzcyBTZWN1cmVGcm9udGVuZFdlYkFwcENsb3VkRnJvbnREaXN0cmlidXRpb24gZXh0ZW5kcyBjbG91ZGZyb250LkRpc3RyaWJ1dGlvbiB7XG5cbiAgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM6IFNlY3VyZUZyb250ZW5kV2ViQXBwQ2xvdWRGcm9udERpc3RyaWJ1dGlvblByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkLCB7XG4gICAgICBlbmFibGVkOiB0cnVlLFxuICAgICAgY29tbWVudDogcHJvcHMuY29tbWVudCxcbiAgICAgIGRlZmF1bHRSb290T2JqZWN0OiAnaW5kZXguaHRtbCcsXG4gICAgICBjZXJ0aWZpY2F0ZTogcHJvcHMuY2VydGlmaWNhdGUsXG4gICAgICBkb21haW5OYW1lczogW3Byb3BzLmRvbWFpbk5hbWVdLFxuICAgICAgbWluaW11bVByb3RvY29sVmVyc2lvbjogY2xvdWRmcm9udC5TZWN1cml0eVBvbGljeVByb3RvY29sLlRMU19WMV8yXzIwMjEsXG4gICAgICBzc2xTdXBwb3J0TWV0aG9kOiBjbG91ZGZyb250LlNTTE1ldGhvZC5TTkksXG4gICAgICBodHRwVmVyc2lvbjogY2xvdWRmcm9udC5IdHRwVmVyc2lvbi5IVFRQMl9BTkRfMyxcbiAgICAgIC8vIHdlYkFjbElkOiBwcm9wcy53YWZBY2xJZCxcbiAgICAgIGxvZ0J1Y2tldDogcHJvcHMuYWNjZXNzTG9nQnVja2V0LFxuICAgICAgbG9nRmlsZVByZWZpeDogcHJvcHMuYWNjZXNzTG9nQnVja2V0ID8gYCR7cHJvcHMuZG9tYWluTmFtZX0vYCA6IHVuZGVmaW5lZCxcbiAgICAgIGRlZmF1bHRCZWhhdmlvcjoge1xuICAgICAgICBhbGxvd2VkTWV0aG9kczogY2xvdWRmcm9udC5BbGxvd2VkTWV0aG9kcy5BTExPV19HRVRfSEVBRF9PUFRJT05TLFxuICAgICAgICBjYWNoZWRNZXRob2RzOiBjbG91ZGZyb250LkNhY2hlZE1ldGhvZHMuQ0FDSEVfR0VUX0hFQURfT1BUSU9OUyxcbiAgICAgICAgY2FjaGVQb2xpY3k6IGNsb3VkZnJvbnQuQ2FjaGVQb2xpY3kuQ0FDSElOR19PUFRJTUlaRUQsXG4gICAgICAgIGNvbXByZXNzOiB0cnVlLFxuICAgICAgICB2aWV3ZXJQcm90b2NvbFBvbGljeTogY2xvdWRmcm9udC5WaWV3ZXJQcm90b2NvbFBvbGljeS5IVFRQU19PTkxZLFxuICAgICAgICBvcmlnaW46IG5ldyBvcmlnaW5zLlMzT3JpZ2luKHByb3BzLm9yaWdpbkJ1Y2tldCwge1xuICAgICAgICAgIG9yaWdpbkFjY2Vzc0lkZW50aXR5OiBwcm9wcy5vcmlnaW5BY2Nlc3NJZGVudGl0eSxcbiAgICAgICAgfSksXG4gICAgICAgIHJlc3BvbnNlSGVhZGVyc1BvbGljeTogbmV3IGNsb3VkZnJvbnQuUmVzcG9uc2VIZWFkZXJzUG9saWN5KHNjb3BlLCAnUmVzcG9uc2VIZWFkZXJzUG9saWN5Jywge1xuICAgICAgICAgIC8vcmVzcG9uc2VIZWFkZXJzUG9saWN5TmFtZTogLFxuICAgICAgICAgIGNvbW1lbnQ6ICdBIGRlZmF1bHQgcG9saWN5JyxcbiAgICAgICAgICBzZWN1cml0eUhlYWRlcnNCZWhhdmlvcjoge1xuICAgICAgICAgICAgLy9jb250ZW50U2VjdXJpdHlQb2xpY3k6IHsgY29udGVudFNlY3VyaXR5UG9saWN5OiAnZGVmYXVsdC1zcmMgaHR0cHM6OycsIG92ZXJyaWRlOiB0cnVlIH0sXG4gICAgICAgICAgICBjb250ZW50VHlwZU9wdGlvbnM6IHsgb3ZlcnJpZGU6IHRydWUgfSxcbiAgICAgICAgICAgIGZyYW1lT3B0aW9uczoge1xuICAgICAgICAgICAgICBmcmFtZU9wdGlvbjogY2xvdWRmcm9udC5IZWFkZXJzRnJhbWVPcHRpb24uU0FNRU9SSUdJTixcbiAgICAgICAgICAgICAgb3ZlcnJpZGU6IHRydWUsXG4gICAgICAgICAgICB9LFxuICAgICAgICAgICAgcmVmZXJyZXJQb2xpY3k6IHtcbiAgICAgICAgICAgICAgcmVmZXJyZXJQb2xpY3k6IGNsb3VkZnJvbnQuSGVhZGVyc1JlZmVycmVyUG9saWN5LlNUUklDVF9PUklHSU5fV0hFTl9DUk9TU19PUklHSU4sXG4gICAgICAgICAgICAgIG92ZXJyaWRlOiB0cnVlLFxuICAgICAgICAgICAgfSxcbiAgICAgICAgICAgIHN0cmljdFRyYW5zcG9ydFNlY3VyaXR5OiB7XG4gICAgICAgICAgICAgIGFjY2Vzc0NvbnRyb2xNYXhBZ2U6IGNkay5EdXJhdGlvbi5zZWNvbmRzKDMxNTM2MDAwKSwgLy8gMSB5ZWFyXG4gICAgICAgICAgICAgIHByZWxvYWQ6IHRydWUsXG4gICAgICAgICAgICAgIGluY2x1ZGVTdWJkb21haW5zOiB0cnVlLFxuICAgICAgICAgICAgICBvdmVycmlkZTogdHJ1ZSxcbiAgICAgICAgICAgIH0sXG4gICAgICAgICAgICB4c3NQcm90ZWN0aW9uOiB7XG4gICAgICAgICAgICAgIHByb3RlY3Rpb246IHRydWUsXG4gICAgICAgICAgICAgIG1vZGVCbG9jazogdHJ1ZSxcbiAgICAgICAgICAgICAgb3ZlcnJpZGU6IHRydWUsXG4gICAgICAgICAgICB9LFxuICAgICAgICAgIH0sXG4gICAgICAgICAgY3VzdG9tSGVhZGVyc0JlaGF2aW9yOiB7XG4gICAgICAgICAgICBjdXN0b21IZWFkZXJzOiBbXG4gICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICBoZWFkZXI6ICdDYWNoZS1Db250cm9sJyxcbiAgICAgICAgICAgICAgICB2YWx1ZTogJ25vLWNhY2hlLCBuby1zdG9yZSwgcHJpdmF0ZScsXG4gICAgICAgICAgICAgICAgb3ZlcnJpZGU6IHRydWUsXG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICBoZWFkZXI6ICdwcmFnbWEnLFxuICAgICAgICAgICAgICAgIHZhbHVlOiAnbm8tY2FjaGUnLFxuICAgICAgICAgICAgICAgIG92ZXJyaWRlOiB0cnVlLFxuICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgXSxcbiAgICAgICAgICB9LFxuICAgICAgICB9KSxcbiAgICAgIH0sXG4gICAgICBlcnJvclJlc3BvbnNlczogW1xuICAgICAgICB7XG4gICAgICAgICAgdHRsOiBjZGsuRHVyYXRpb24uc2Vjb25kcygzMDApLFxuICAgICAgICAgIGh0dHBTdGF0dXM6IDQwMyxcbiAgICAgICAgICByZXNwb25zZUh0dHBTdGF0dXM6IDIwMCxcbiAgICAgICAgICByZXNwb25zZVBhZ2VQYXRoOiAnL2luZGV4Lmh0bWwnLFxuICAgICAgICB9LFxuICAgICAgICB7XG4gICAgICAgICAgdHRsOiBjZGsuRHVyYXRpb24uc2Vjb25kcygzMDApLFxuICAgICAgICAgIGh0dHBTdGF0dXM6IDQwNCxcbiAgICAgICAgICByZXNwb25zZUh0dHBTdGF0dXM6IDIwMCxcbiAgICAgICAgICByZXNwb25zZVBhZ2VQYXRoOiAnL2luZGV4Lmh0bWwnLFxuICAgICAgICB9LFxuICAgICAgXSxcbiAgICAgIHByaWNlQ2xhc3M6IGNsb3VkZnJvbnQuUHJpY2VDbGFzcy5QUklDRV9DTEFTU19BTEwsXG4gICAgfSk7XG4gIH1cbn0iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9731121281464531%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.72.5'}", "'version'": "'0.7.7'"}*

```diff
@@ -21,15 +21,15 @@
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.86.1",
         "jsii-docgen": "^7.2.9",
         "jsii-pacmak": "^1.86.1",
         "jsii-rosetta": "1.x",
         "npm-check-updates": "^16",
-        "projen": "^0.72.4",
+        "projen": "^0.72.5",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.1",
         "typescript": "5.1.x"
     },
     "engines": {
         "node": ">= 16.0.0"
@@ -139,9 +139,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.7.6"
+    "version": "0.7.7"
 }
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.7.6
+Version: 0.7.7
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.6/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.6.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.7.jsii.tgz
```

