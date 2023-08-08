# Comparing `tmp/cdk-lambda-recaptcha-authorizer-0.1.3.tar.gz` & `tmp/cdk-lambda-recaptcha-authorizer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-lambda-recaptcha-authorizer-0.1.3.tar", last modified: Mon Aug  7 11:08:31 2023, max compression
+gzip compressed data, was "cdk-lambda-recaptcha-authorizer-0.1.4.tar", last modified: Tue Aug  8 11:20:35 2023, max compression
```

## Comparing `cdk-lambda-recaptcha-authorizer-0.1.3.tar` & `cdk-lambda-recaptcha-authorizer-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/_jsii/cdk-lambda-recaptcha-authorizer@0.1.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:08:17.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:08:31.736701 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-08-07 11:08:31.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-07 11:08:31.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:08:31.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 11:08:31.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 11:08:31.000000 cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:35.428939 cdk-lambda-recaptcha-authorizer-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-08 11:20:35.428939 cdk-lambda-recaptcha-authorizer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 11:20:35.428939 cdk-lambda-recaptcha-authorizer-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:35.424939 cdk-lambda-recaptcha-authorizer-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:35.424939 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:35.428939 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/_jsii/cdk-lambda-recaptcha-authorizer@0.1.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:20:24.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:35.428939 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-08 11:20:35.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 11:20:35.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:20:35.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-08 11:20:35.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 11:20:35.000000 cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/top_level.txt
```

### Comparing `cdk-lambda-recaptcha-authorizer-0.1.3/LICENSE` & `cdk-lambda-recaptcha-authorizer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-lambda-recaptcha-authorizer-0.1.3/PKG-INFO` & `cdk-lambda-recaptcha-authorizer-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: cdk-lambda-recaptcha-authorizer
-Version: 0.1.3
-Summary: Custom construct for AWS CDK that provides an easy way to integrate reCAPTCHA-based authorization with Amazon API Gateway.
-Home-page: https://github.com/ilkerdagli/cdk-lambda-recaptcha-authorizer.git
-Author: Ilker Dagli<daglilker@gmail.com>
-License: MIT
-Project-URL: Source, https://github.com/ilkerdagli/cdk-lambda-recaptcha-authorizer.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ReCaptcha Authorizer for AWS CDK
 
 This is an AWS CDK construct that provides an easy way to add ReCaptcha-based authorization
 to your API Gateway endpoints. It uses Google's ReCaptcha API to verify user responses and
 secure your API resources.
 
 ## Installation
@@ -43,46 +19,109 @@
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import * as apigw from 'aws-cdk-lib/aws-apigateway';
 import * as lambda from 'aws-cdk-lib/aws-lambda';
 import { ReCaptchaAuthorizer } from 'cdk-lambda-recaptcha-authorizer';
 
-export class ExampleRecaptchaAuthorizerStack extends cdk.Stack {
+export class LraExampleStack extends cdk.Stack {
   constructor(scope: Construct, id: string, props?: cdk.StackProps) {
     super(scope, id, props);
 
+    const challangeResponseHeaderName = 'X-My-Header'
+
     const api = new apigw.RestApi(this, 'Api', {
       restApiName: 'API',
       description: 'API with reCAPTCHA authorizer',
+      defaultCorsPreflightOptions: {
+        allowHeaders: [
+          'Content-Type',
+          'X-Amz-Date',
+          challangeResponseHeaderName
+        ],
+        allowCredentials: true,
+        allowOrigins: ['*'],
+        allowMethods: ['OPTIONS', 'GET', 'POST', 'PUT', 'PATCH', 'DELETE'],
+      }
     });
 
-    // Create the ReCaptchaAuthorizer and provide your ReCaptcha secret key
     const reCaptchaAuthorizer = new ReCaptchaAuthorizer(this, 'ReCaptchaAuthorizer', {
-      reCaptchaSecretKey: 'YOUR_RECAPTCHA_SECRET_KEY',
-      reCaptchaVersion: 'v2', // Use 'v2' or 'v3'
-      // v3MinScoreRequired?: 0.5, // (Optional) Minimum score required for ReCaptcha v3
-      // v3Action?: 'your_custom_action', // (Optional) Specify a custom action for ReCaptcha v3
-      // challangeResponseHeaderName?: 'X-Recaptcha-Response', // (Optional) Custom header name for ReCaptcha token
-    });
+      reCaptchaSecretKey: 'YOUR-RECAPTCHA-SECRET-KEY',
+      reCaptchaVersion: 'v2',
+      challangeResponseHeaderName: challangeResponseHeaderName
+    })
+
+    const resource = api.root.addResource('submitForm');
 
-    // Create an API Gateway resource and associate the ReCaptchaAuthorizer with it
-    const resource = api.root.addResource('hello');
-    resource.addMethod('GET', new apigw.LambdaIntegration(new lambda.Function(this, 'Lambda', {
+    resource.addMethod('POST', new apigw.LambdaIntegration(new lambda.Function(this, 'Lambda', {
       runtime: lambda.Runtime.NODEJS_14_X,
       handler: 'index.handler',
       code: lambda.Code.fromInline('exports.handler = async () => { return { statusCode: 200, body: "Hello World!" }; };'),
     })), {
-      authorizer: reCaptchaAuthorizer.authorizer,
+
+      authorizer: reCaptchaAuthorizer,
       authorizationType: apigw.AuthorizationType.CUSTOM,
     });
   }
 }
 ```
 
+Here's an example form in html that sends recaptcha challange response in header:
+
+```html
+<!DOCTYPE html>
+<html>
+   <head>
+      <title>reCAPTCHA v2 Demo</title>
+      <script src="https://www.google.com/recaptcha/api.js" async defer></script>
+   </head>
+   <body>
+      <h1>reCAPTCHA v2 Demo Form</h1>
+      <form
+         id="demoForm"
+         method="POST"
+         >
+         <label for="name">Name:</label>
+         <input type="text" id="name" name="name" required />
+         <br />
+         <div class="g-recaptcha" data-sitekey="YOUR-RECAPTCHA-SITE-KEY"></div>
+         <button type="submit">Submit</button>
+      </form>
+      <script>
+         const form = document.getElementById("demoForm")
+
+         form.addEventListener("submit", async (event) => {
+           event.preventDefault()
+           const recaptchaResponse = grecaptcha.getResponse()
+
+           if (recaptchaResponse === "") {
+             alert("Please complete the reCAPTCHA verification.")
+             return
+           }
+
+           const headers = new Headers()
+           headers.append("X-My-Header", recaptchaResponse)
+
+           const response = await fetch("YOUR-API-GATEWAY-URL", {
+             method: "POST",
+             headers: headers,
+             body: new FormData(form),
+           })
+
+           if (response.ok) {
+             alert("Form submitted successfully!")
+           } else {
+             alert("Form submission failed. Please try again later.")
+           }
+         })
+      </script>
+   </body>
+</html>
+```
+
 ## Configuration
 
 The `ReCaptchaAuthorizer` accepts the following configuration options:
 
 * `reCaptchaSecretKey`: Your ReCaptcha secret key. It is required.
 * `reCaptchaVersion`: The ReCaptcha version to use. It can be either 'v2' or 'v3'.
 * `v3MinScoreRequired`: (Optional) The minimum score required for ReCaptcha v3 authorization. Default is 0.5.
```

### Comparing `cdk-lambda-recaptcha-authorizer-0.1.3/setup.py` & `cdk-lambda-recaptcha-authorizer-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-lambda-recaptcha-authorizer",
-    "version": "0.1.3",
+    "version": "0.1.4",
     "description": "Custom construct for AWS CDK that provides an easy way to integrate reCAPTCHA-based authorization with Amazon API Gateway.",
     "license": "MIT",
     "url": "https://github.com/ilkerdagli/cdk-lambda-recaptcha-authorizer.git",
     "long_description_content_type": "text/markdown",
     "author": "Ilker Dagli<daglilker@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_lambda_recaptcha_authorizer",
         "cdk_lambda_recaptcha_authorizer._jsii"
     ],
     "package_data": {
         "cdk_lambda_recaptcha_authorizer._jsii": [
-            "cdk-lambda-recaptcha-authorizer@0.1.3.jsii.tgz"
+            "cdk-lambda-recaptcha-authorizer@0.1.4.jsii.tgz"
         ],
         "cdk_lambda_recaptcha_authorizer": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer/__init__.py` & `cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,46 +20,109 @@
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import * as apigw from 'aws-cdk-lib/aws-apigateway';
 import * as lambda from 'aws-cdk-lib/aws-lambda';
 import { ReCaptchaAuthorizer } from 'cdk-lambda-recaptcha-authorizer';
 
-export class ExampleRecaptchaAuthorizerStack extends cdk.Stack {
+export class LraExampleStack extends cdk.Stack {
   constructor(scope: Construct, id: string, props?: cdk.StackProps) {
     super(scope, id, props);
 
+    const challangeResponseHeaderName = 'X-My-Header'
+
     const api = new apigw.RestApi(this, 'Api', {
       restApiName: 'API',
       description: 'API with reCAPTCHA authorizer',
+      defaultCorsPreflightOptions: {
+        allowHeaders: [
+          'Content-Type',
+          'X-Amz-Date',
+          challangeResponseHeaderName
+        ],
+        allowCredentials: true,
+        allowOrigins: ['*'],
+        allowMethods: ['OPTIONS', 'GET', 'POST', 'PUT', 'PATCH', 'DELETE'],
+      }
     });
 
-    // Create the ReCaptchaAuthorizer and provide your ReCaptcha secret key
     const reCaptchaAuthorizer = new ReCaptchaAuthorizer(this, 'ReCaptchaAuthorizer', {
-      reCaptchaSecretKey: 'YOUR_RECAPTCHA_SECRET_KEY',
-      reCaptchaVersion: 'v2', // Use 'v2' or 'v3'
-      // v3MinScoreRequired?: 0.5, // (Optional) Minimum score required for ReCaptcha v3
-      // v3Action?: 'your_custom_action', // (Optional) Specify a custom action for ReCaptcha v3
-      // challangeResponseHeaderName?: 'X-Recaptcha-Response', // (Optional) Custom header name for ReCaptcha token
-    });
+      reCaptchaSecretKey: 'YOUR-RECAPTCHA-SECRET-KEY',
+      reCaptchaVersion: 'v2',
+      challangeResponseHeaderName: challangeResponseHeaderName
+    })
 
-    // Create an API Gateway resource and associate the ReCaptchaAuthorizer with it
-    const resource = api.root.addResource('hello');
-    resource.addMethod('GET', new apigw.LambdaIntegration(new lambda.Function(this, 'Lambda', {
+    const resource = api.root.addResource('submitForm');
+
+    resource.addMethod('POST', new apigw.LambdaIntegration(new lambda.Function(this, 'Lambda', {
       runtime: lambda.Runtime.NODEJS_14_X,
       handler: 'index.handler',
       code: lambda.Code.fromInline('exports.handler = async () => { return { statusCode: 200, body: "Hello World!" }; };'),
     })), {
-      authorizer: reCaptchaAuthorizer.authorizer,
+
+      authorizer: reCaptchaAuthorizer,
       authorizationType: apigw.AuthorizationType.CUSTOM,
     });
   }
 }
 ```
 
+Here's an example form in html that sends recaptcha challange response in header:
+
+```html
+<!DOCTYPE html>
+<html>
+   <head>
+      <title>reCAPTCHA v2 Demo</title>
+      <script src="https://www.google.com/recaptcha/api.js" async defer></script>
+   </head>
+   <body>
+      <h1>reCAPTCHA v2 Demo Form</h1>
+      <form
+         id="demoForm"
+         method="POST"
+         >
+         <label for="name">Name:</label>
+         <input type="text" id="name" name="name" required />
+         <br />
+         <div class="g-recaptcha" data-sitekey="YOUR-RECAPTCHA-SITE-KEY"></div>
+         <button type="submit">Submit</button>
+      </form>
+      <script>
+         const form = document.getElementById("demoForm")
+
+         form.addEventListener("submit", async (event) => {
+           event.preventDefault()
+           const recaptchaResponse = grecaptcha.getResponse()
+
+           if (recaptchaResponse === "") {
+             alert("Please complete the reCAPTCHA verification.")
+             return
+           }
+
+           const headers = new Headers()
+           headers.append("X-My-Header", recaptchaResponse)
+
+           const response = await fetch("YOUR-API-GATEWAY-URL", {
+             method: "POST",
+             headers: headers,
+             body: new FormData(form),
+           })
+
+           if (response.ok) {
+             alert("Form submitted successfully!")
+           } else {
+             alert("Form submission failed. Please try again later.")
+           }
+         })
+      </script>
+   </body>
+</html>
+```
+
 ## Configuration
 
 The `ReCaptchaAuthorizer` accepts the following configuration options:
 
 * `reCaptchaSecretKey`: Your ReCaptcha secret key. It is required.
 * `reCaptchaVersion`: The ReCaptcha version to use. It can be either 'v2' or 'v3'.
 * `v3MinScoreRequired`: (Optional) The minimum score required for ReCaptcha v3 authorization. Default is 0.5.
@@ -120,248 +183,203 @@
 
 from ._jsii import *
 
 import aws_cdk.aws_apigateway as _aws_cdk_aws_apigateway_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
-@jsii.interface(jsii_type="cdk-lambda-recaptcha-authorizer.IReCaptchaAuthorizerProps")
-class IReCaptchaAuthorizerProps(typing_extensions.Protocol):
+@jsii.implements(_aws_cdk_aws_apigateway_ceddda9d.IAuthorizer)
+class ReCaptchaAuthorizer(
+    _aws_cdk_aws_apigateway_ceddda9d.Authorizer,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="cdk-lambda-recaptcha-authorizer.ReCaptchaAuthorizer",
+):
     '''
     :stability: experimental
     '''
 
-    @builtins.property
-    @jsii.member(jsii_name="reCaptchaSecretKey")
-    def re_captcha_secret_key(self) -> builtins.str:
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        re_captcha_secret_key: builtins.str,
+        re_captcha_version: builtins.str,
+        challange_response_header_name: typing.Optional[builtins.str] = None,
+        v3_action: typing.Optional[builtins.str] = None,
+        v3_min_score_required: typing.Optional[jsii.Number] = None,
+    ) -> None:
         '''
+        :param scope: -
+        :param id: -
+        :param re_captcha_secret_key: 
+        :param re_captcha_version: 
+        :param challange_response_header_name: 
+        :param v3_action: 
+        :param v3_min_score_required: 
+
         :stability: experimental
         '''
-        ...
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__77b92147e87efd304b41a314930a9f13bece7b0666b81bcfd1b4dd14d86a03a6)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = ReCaptchaAuthorizerProps(
+            re_captcha_secret_key=re_captcha_secret_key,
+            re_captcha_version=re_captcha_version,
+            challange_response_header_name=challange_response_header_name,
+            v3_action=v3_action,
+            v3_min_score_required=v3_min_score_required,
+        )
 
-    @re_captcha_secret_key.setter
-    def re_captcha_secret_key(self, value: builtins.str) -> None:
-        ...
+        jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
-    @jsii.member(jsii_name="reCaptchaVersion")
-    def re_captcha_version(self) -> builtins.str:
+    @jsii.member(jsii_name="authorizer")
+    def authorizer(self) -> _aws_cdk_aws_apigateway_ceddda9d.RequestAuthorizer:
         '''
         :stability: experimental
         '''
-        ...
-
-    @re_captcha_version.setter
-    def re_captcha_version(self, value: builtins.str) -> None:
-        ...
+        return typing.cast(_aws_cdk_aws_apigateway_ceddda9d.RequestAuthorizer, jsii.get(self, "authorizer"))
 
     @builtins.property
-    @jsii.member(jsii_name="challangeResponseHeaderName")
-    def challange_response_header_name(self) -> typing.Optional[builtins.str]:
-        '''
+    @jsii.member(jsii_name="authorizerId")
+    def authorizer_id(self) -> builtins.str:
+        '''(experimental) The authorizer ID.
+
         :stability: experimental
         '''
-        ...
-
-    @challange_response_header_name.setter
-    def challange_response_header_name(
+        return typing.cast(builtins.str, jsii.get(self, "authorizerId"))
+
+
+@jsii.data_type(
+    jsii_type="cdk-lambda-recaptcha-authorizer.ReCaptchaAuthorizerProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "re_captcha_secret_key": "reCaptchaSecretKey",
+        "re_captcha_version": "reCaptchaVersion",
+        "challange_response_header_name": "challangeResponseHeaderName",
+        "v3_action": "v3Action",
+        "v3_min_score_required": "v3MinScoreRequired",
+    },
+)
+class ReCaptchaAuthorizerProps:
+    def __init__(
         self,
-        value: typing.Optional[builtins.str],
+        *,
+        re_captcha_secret_key: builtins.str,
+        re_captcha_version: builtins.str,
+        challange_response_header_name: typing.Optional[builtins.str] = None,
+        v3_action: typing.Optional[builtins.str] = None,
+        v3_min_score_required: typing.Optional[jsii.Number] = None,
     ) -> None:
-        ...
-
-    @builtins.property
-    @jsii.member(jsii_name="v3Action")
-    def v3_action(self) -> typing.Optional[builtins.str]:
-        '''
-        :stability: experimental
         '''
-        ...
-
-    @v3_action.setter
-    def v3_action(self, value: typing.Optional[builtins.str]) -> None:
-        ...
+        :param re_captcha_secret_key: 
+        :param re_captcha_version: 
+        :param challange_response_header_name: 
+        :param v3_action: 
+        :param v3_min_score_required: 
 
-    @builtins.property
-    @jsii.member(jsii_name="v3MinScoreRequired")
-    def v3_min_score_required(self) -> typing.Optional[jsii.Number]:
-        '''
         :stability: experimental
         '''
-        ...
-
-    @v3_min_score_required.setter
-    def v3_min_score_required(self, value: typing.Optional[jsii.Number]) -> None:
-        ...
-
-
-class _IReCaptchaAuthorizerPropsProxy:
-    '''
-    :stability: experimental
-    '''
-
-    __jsii_type__: typing.ClassVar[str] = "cdk-lambda-recaptcha-authorizer.IReCaptchaAuthorizerProps"
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__03df3d2de02c9602312fd3c7395d364c04abfebd128fc9ee58d9c3363ffedbe9)
+            check_type(argname="argument re_captcha_secret_key", value=re_captcha_secret_key, expected_type=type_hints["re_captcha_secret_key"])
+            check_type(argname="argument re_captcha_version", value=re_captcha_version, expected_type=type_hints["re_captcha_version"])
+            check_type(argname="argument challange_response_header_name", value=challange_response_header_name, expected_type=type_hints["challange_response_header_name"])
+            check_type(argname="argument v3_action", value=v3_action, expected_type=type_hints["v3_action"])
+            check_type(argname="argument v3_min_score_required", value=v3_min_score_required, expected_type=type_hints["v3_min_score_required"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "re_captcha_secret_key": re_captcha_secret_key,
+            "re_captcha_version": re_captcha_version,
+        }
+        if challange_response_header_name is not None:
+            self._values["challange_response_header_name"] = challange_response_header_name
+        if v3_action is not None:
+            self._values["v3_action"] = v3_action
+        if v3_min_score_required is not None:
+            self._values["v3_min_score_required"] = v3_min_score_required
 
     @builtins.property
-    @jsii.member(jsii_name="reCaptchaSecretKey")
     def re_captcha_secret_key(self) -> builtins.str:
         '''
         :stability: experimental
         '''
-        return typing.cast(builtins.str, jsii.get(self, "reCaptchaSecretKey"))
-
-    @re_captcha_secret_key.setter
-    def re_captcha_secret_key(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7780121939ac4a770ef2be6a1333c356b8435b400e83aeb717f3f9e04b035c54)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "reCaptchaSecretKey", value)
+        result = self._values.get("re_captcha_secret_key")
+        assert result is not None, "Required property 're_captcha_secret_key' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
-    @jsii.member(jsii_name="reCaptchaVersion")
     def re_captcha_version(self) -> builtins.str:
         '''
         :stability: experimental
         '''
-        return typing.cast(builtins.str, jsii.get(self, "reCaptchaVersion"))
-
-    @re_captcha_version.setter
-    def re_captcha_version(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e234ae4bfc2d9f45c7f4ef16526e9dfe9aca5d024d55b9193f976eccb0e87ee5)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "reCaptchaVersion", value)
+        result = self._values.get("re_captcha_version")
+        assert result is not None, "Required property 're_captcha_version' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
-    @jsii.member(jsii_name="challangeResponseHeaderName")
     def challange_response_header_name(self) -> typing.Optional[builtins.str]:
         '''
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "challangeResponseHeaderName"))
-
-    @challange_response_header_name.setter
-    def challange_response_header_name(
-        self,
-        value: typing.Optional[builtins.str],
-    ) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d5c248acdb87a9d991387cadce721f9ae901c6c9c8c1cda4e078af98d191d687)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "challangeResponseHeaderName", value)
+        result = self._values.get("challange_response_header_name")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="v3Action")
     def v3_action(self) -> typing.Optional[builtins.str]:
         '''
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "v3Action"))
-
-    @v3_action.setter
-    def v3_action(self, value: typing.Optional[builtins.str]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ef0eca27c32f002bf6d024b5d2e433d4593b8f7f74f318e6bb1872c9dcc5563e)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "v3Action", value)
+        result = self._values.get("v3_action")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="v3MinScoreRequired")
     def v3_min_score_required(self) -> typing.Optional[jsii.Number]:
         '''
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "v3MinScoreRequired"))
-
-    @v3_min_score_required.setter
-    def v3_min_score_required(self, value: typing.Optional[jsii.Number]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9e6187176637344de7fafd24f02ddac3fe9230e98080ff0bb06861cf587fa34d)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "v3MinScoreRequired", value)
+        result = self._values.get("v3_min_score_required")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
-# Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
-typing.cast(typing.Any, IReCaptchaAuthorizerProps).__jsii_proxy_class__ = lambda : _IReCaptchaAuthorizerPropsProxy
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
 
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
 
-class ReCaptchaAuthorizer(
-    _constructs_77d1e7e8.Construct,
-    metaclass=jsii.JSIIMeta,
-    jsii_type="cdk-lambda-recaptcha-authorizer.ReCaptchaAuthorizer",
-):
-    '''
-    :stability: experimental
-    '''
-
-    def __init__(
-        self,
-        scope: _constructs_77d1e7e8.Construct,
-        id: builtins.str,
-        props: IReCaptchaAuthorizerProps,
-    ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param props: -
-
-        :stability: experimental
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__77b92147e87efd304b41a314930a9f13bece7b0666b81bcfd1b4dd14d86a03a6)
-            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
-        jsii.create(self.__class__, self, [scope, id, props])
-
-    @builtins.property
-    @jsii.member(jsii_name="authorizer")
-    def authorizer(self) -> _aws_cdk_aws_apigateway_ceddda9d.RequestAuthorizer:
-        '''
-        :stability: experimental
-        '''
-        return typing.cast(_aws_cdk_aws_apigateway_ceddda9d.RequestAuthorizer, jsii.get(self, "authorizer"))
+    def __repr__(self) -> str:
+        return "ReCaptchaAuthorizerProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
 
 
 __all__ = [
-    "IReCaptchaAuthorizerProps",
     "ReCaptchaAuthorizer",
+    "ReCaptchaAuthorizerProps",
 ]
 
 publication.publish()
 
-def _typecheckingstub__7780121939ac4a770ef2be6a1333c356b8435b400e83aeb717f3f9e04b035c54(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e234ae4bfc2d9f45c7f4ef16526e9dfe9aca5d024d55b9193f976eccb0e87ee5(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d5c248acdb87a9d991387cadce721f9ae901c6c9c8c1cda4e078af98d191d687(
-    value: typing.Optional[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__ef0eca27c32f002bf6d024b5d2e433d4593b8f7f74f318e6bb1872c9dcc5563e(
-    value: typing.Optional[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__9e6187176637344de7fafd24f02ddac3fe9230e98080ff0bb06861cf587fa34d(
-    value: typing.Optional[jsii.Number],
+def _typecheckingstub__77b92147e87efd304b41a314930a9f13bece7b0666b81bcfd1b4dd14d86a03a6(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    re_captcha_secret_key: builtins.str,
+    re_captcha_version: builtins.str,
+    challange_response_header_name: typing.Optional[builtins.str] = None,
+    v3_action: typing.Optional[builtins.str] = None,
+    v3_min_score_required: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__77b92147e87efd304b41a314930a9f13bece7b0666b81bcfd1b4dd14d86a03a6(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    props: IReCaptchaAuthorizerProps,
+def _typecheckingstub__03df3d2de02c9602312fd3c7395d364c04abfebd128fc9ee58d9c3363ffedbe9(
+    *,
+    re_captcha_secret_key: builtins.str,
+    re_captcha_version: builtins.str,
+    challange_response_header_name: typing.Optional[builtins.str] = None,
+    v3_action: typing.Optional[builtins.str] = None,
+    v3_min_score_required: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/PKG-INFO` & `cdk-lambda-recaptcha-authorizer-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-lambda-recaptcha-authorizer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Custom construct for AWS CDK that provides an easy way to integrate reCAPTCHA-based authorization with Amazon API Gateway.
 Home-page: https://github.com/ilkerdagli/cdk-lambda-recaptcha-authorizer.git
 Author: Ilker Dagli<daglilker@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/ilkerdagli/cdk-lambda-recaptcha-authorizer.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -43,46 +43,109 @@
 ```python
 import * as cdk from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import * as apigw from 'aws-cdk-lib/aws-apigateway';
 import * as lambda from 'aws-cdk-lib/aws-lambda';
 import { ReCaptchaAuthorizer } from 'cdk-lambda-recaptcha-authorizer';
 
-export class ExampleRecaptchaAuthorizerStack extends cdk.Stack {
+export class LraExampleStack extends cdk.Stack {
   constructor(scope: Construct, id: string, props?: cdk.StackProps) {
     super(scope, id, props);
 
+    const challangeResponseHeaderName = 'X-My-Header'
+
     const api = new apigw.RestApi(this, 'Api', {
       restApiName: 'API',
       description: 'API with reCAPTCHA authorizer',
+      defaultCorsPreflightOptions: {
+        allowHeaders: [
+          'Content-Type',
+          'X-Amz-Date',
+          challangeResponseHeaderName
+        ],
+        allowCredentials: true,
+        allowOrigins: ['*'],
+        allowMethods: ['OPTIONS', 'GET', 'POST', 'PUT', 'PATCH', 'DELETE'],
+      }
     });
 
-    // Create the ReCaptchaAuthorizer and provide your ReCaptcha secret key
     const reCaptchaAuthorizer = new ReCaptchaAuthorizer(this, 'ReCaptchaAuthorizer', {
-      reCaptchaSecretKey: 'YOUR_RECAPTCHA_SECRET_KEY',
-      reCaptchaVersion: 'v2', // Use 'v2' or 'v3'
-      // v3MinScoreRequired?: 0.5, // (Optional) Minimum score required for ReCaptcha v3
-      // v3Action?: 'your_custom_action', // (Optional) Specify a custom action for ReCaptcha v3
-      // challangeResponseHeaderName?: 'X-Recaptcha-Response', // (Optional) Custom header name for ReCaptcha token
-    });
+      reCaptchaSecretKey: 'YOUR-RECAPTCHA-SECRET-KEY',
+      reCaptchaVersion: 'v2',
+      challangeResponseHeaderName: challangeResponseHeaderName
+    })
 
-    // Create an API Gateway resource and associate the ReCaptchaAuthorizer with it
-    const resource = api.root.addResource('hello');
-    resource.addMethod('GET', new apigw.LambdaIntegration(new lambda.Function(this, 'Lambda', {
+    const resource = api.root.addResource('submitForm');
+
+    resource.addMethod('POST', new apigw.LambdaIntegration(new lambda.Function(this, 'Lambda', {
       runtime: lambda.Runtime.NODEJS_14_X,
       handler: 'index.handler',
       code: lambda.Code.fromInline('exports.handler = async () => { return { statusCode: 200, body: "Hello World!" }; };'),
     })), {
-      authorizer: reCaptchaAuthorizer.authorizer,
+
+      authorizer: reCaptchaAuthorizer,
       authorizationType: apigw.AuthorizationType.CUSTOM,
     });
   }
 }
 ```
 
+Here's an example form in html that sends recaptcha challange response in header:
+
+```html
+<!DOCTYPE html>
+<html>
+   <head>
+      <title>reCAPTCHA v2 Demo</title>
+      <script src="https://www.google.com/recaptcha/api.js" async defer></script>
+   </head>
+   <body>
+      <h1>reCAPTCHA v2 Demo Form</h1>
+      <form
+         id="demoForm"
+         method="POST"
+         >
+         <label for="name">Name:</label>
+         <input type="text" id="name" name="name" required />
+         <br />
+         <div class="g-recaptcha" data-sitekey="YOUR-RECAPTCHA-SITE-KEY"></div>
+         <button type="submit">Submit</button>
+      </form>
+      <script>
+         const form = document.getElementById("demoForm")
+
+         form.addEventListener("submit", async (event) => {
+           event.preventDefault()
+           const recaptchaResponse = grecaptcha.getResponse()
+
+           if (recaptchaResponse === "") {
+             alert("Please complete the reCAPTCHA verification.")
+             return
+           }
+
+           const headers = new Headers()
+           headers.append("X-My-Header", recaptchaResponse)
+
+           const response = await fetch("YOUR-API-GATEWAY-URL", {
+             method: "POST",
+             headers: headers,
+             body: new FormData(form),
+           })
+
+           if (response.ok) {
+             alert("Form submitted successfully!")
+           } else {
+             alert("Form submission failed. Please try again later.")
+           }
+         })
+      </script>
+   </body>
+</html>
+```
+
 ## Configuration
 
 The `ReCaptchaAuthorizer` accepts the following configuration options:
 
 * `reCaptchaSecretKey`: Your ReCaptcha secret key. It is required.
 * `reCaptchaVersion`: The ReCaptcha version to use. It can be either 'v2' or 'v3'.
 * `v3MinScoreRequired`: (Optional) The minimum score required for ReCaptcha v3 authorization. Default is 0.5.
```

### Comparing `cdk-lambda-recaptcha-authorizer-0.1.3/src/cdk_lambda_recaptcha_authorizer.egg-info/SOURCES.txt` & `cdk-lambda-recaptcha-authorizer-0.1.4/src/cdk_lambda_recaptcha_authorizer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_lambda_recaptcha_authorizer/py.typed
 src/cdk_lambda_recaptcha_authorizer.egg-info/PKG-INFO
 src/cdk_lambda_recaptcha_authorizer.egg-info/SOURCES.txt
 src/cdk_lambda_recaptcha_authorizer.egg-info/dependency_links.txt
 src/cdk_lambda_recaptcha_authorizer.egg-info/requires.txt
 src/cdk_lambda_recaptcha_authorizer.egg-info/top_level.txt
 src/cdk_lambda_recaptcha_authorizer/_jsii/__init__.py
-src/cdk_lambda_recaptcha_authorizer/_jsii/cdk-lambda-recaptcha-authorizer@0.1.3.jsii.tgz
+src/cdk_lambda_recaptcha_authorizer/_jsii/cdk-lambda-recaptcha-authorizer@0.1.4.jsii.tgz
```

