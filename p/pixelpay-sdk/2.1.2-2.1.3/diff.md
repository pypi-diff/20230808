# Comparing `tmp/pixelpay-sdk-2.1.2.tar.gz` & `tmp/pixelpay-sdk-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelpay-sdk-2.1.2.tar", last modified: Fri Jul 28 15:13:43 2023, max compression
+gzip compressed data, was "pixelpay-sdk-2.1.3.tar", last modified: Mon Aug  7 23:31:06 2023, max compression
```

## Comparing `pixelpay-sdk-2.1.2.tar` & `pixelpay-sdk-2.1.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.937703 pixelpay-sdk-2.1.2/
--rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/LICENSE.md
--rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-28 15:13:43.937517 pixelpay-sdk-2.1.2/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.1.2/README.md
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.914011 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/
--rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)     2079 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       31 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/requires.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/top_level.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/pyproject.toml
--rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-07-28 15:13:43.937744 pixelpay-sdk-2.1.2/setup.cfg
--rw-r--r--   0 javiercano   (501) staff       (20)     1398 2023-07-19 22:28:45.000000 pixelpay-sdk-2.1.2/setup.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.903339 pixelpay-sdk-2.1.2/src/
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.914238 pixelpay-sdk-2.1.2/src/pixelpay/
--rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-07-28 04:05:12.000000 pixelpay-sdk-2.1.2/src/pixelpay/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.917620 pixelpay-sdk-2.1.2/src/pixelpay/assets/
--rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/assets/countries.json
--rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.1.2/src/pixelpay/assets/formats.json
--rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/assets/states.json
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.920404 pixelpay-sdk-2.1.2/src/pixelpay/base/
--rw-r--r--   0 javiercano   (501) staff       (20)     3185 2023-07-19 22:25:29.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/Helpers.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1995 2023-07-28 03:39:52.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/RequestBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/Response.py
--rw-r--r--   0 javiercano   (501) staff       (20)    10006 2023-07-28 03:40:04.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/ServiceBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.921649 pixelpay-sdk-2.1.2/src/pixelpay/entities/
--rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/entities/CardResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/entities/TransactionResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/entities/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.923328 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/
--rw-r--r--   0 javiercano   (501) staff       (20)       53 2023-07-27 21:35:29.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/FailedEncryptionException.py
--rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/InvalidCredentialsException.py
--rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/InvalidTransactionTypeException.py
--rw-r--r--   0 javiercano   (501) staff       (20)      333 2023-07-27 21:35:45.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.926040 pixelpay-sdk-2.1.2/src/pixelpay/models/
--rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Billing.py
--rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Card.py
--rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Item.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Order.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1914 2023-07-27 22:07:03.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Settings.py
--rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.931716 pixelpay-sdk-2.1.2/src/pixelpay/requests/
--rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/AuthTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/CaptureTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3890 2023-07-28 03:40:47.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/CardTokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     5951 2023-07-28 03:40:39.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/PaymentTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/SaleTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/StatusTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/VoidTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.932612 pixelpay-sdk-2.1.2/src/pixelpay/resources/
--rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/resources/Environment.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.1.2/src/pixelpay/resources/Locations.py
--rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/resources/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.936478 pixelpay-sdk-2.1.2/src/pixelpay/responses/
--rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/ErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/FailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/InputErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/NetworkFailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/NoAccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/NotFoundResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/PayloadResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/PaymentDeclinedResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/PreconditionalResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/SuccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/TimeoutResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.937240 pixelpay-sdk-2.1.2/src/pixelpay/services/
--rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/services/Tokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/services/Transaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/services/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.133467 pixelpay-sdk-2.1.3/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/LICENSE.md
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-08-07 23:31:06.133252 pixelpay-sdk-2.1.3/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.1.3/README.md
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.097189 pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-08-07 23:31:06.000000 pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)     2079 2023-08-07 23:31:06.000000 pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-08-07 23:31:06.000000 pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       31 2023-08-07 23:31:06.000000 pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/requires.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-08-07 23:31:06.000000 pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/top_level.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/pyproject.toml
+-rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-08-07 23:31:06.133508 pixelpay-sdk-2.1.3/setup.cfg
+-rw-r--r--   0 javiercano   (501) staff       (20)     1398 2023-07-19 22:28:45.000000 pixelpay-sdk-2.1.3/setup.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.088707 pixelpay-sdk-2.1.3/src/
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.097456 pixelpay-sdk-2.1.3/src/pixelpay/
+-rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-08-07 22:40:40.000000 pixelpay-sdk-2.1.3/src/pixelpay/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.098683 pixelpay-sdk-2.1.3/src/pixelpay/assets/
+-rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/assets/countries.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.1.3/src/pixelpay/assets/formats.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/assets/states.json
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.101662 pixelpay-sdk-2.1.3/src/pixelpay/base/
+-rw-r--r--   0 javiercano   (501) staff       (20)     3335 2023-08-07 23:22:17.000000 pixelpay-sdk-2.1.3/src/pixelpay/base/Helpers.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     2061 2023-08-07 23:22:30.000000 pixelpay-sdk-2.1.3/src/pixelpay/base/RequestBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/base/Response.py
+-rw-r--r--   0 javiercano   (501) staff       (20)    10020 2023-08-07 22:56:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/base/ServiceBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/base/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.102580 pixelpay-sdk-2.1.3/src/pixelpay/entities/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/entities/CardResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/entities/TransactionResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/entities/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.104405 pixelpay-sdk-2.1.3/src/pixelpay/exceptions/
+-rw-r--r--   0 javiercano   (501) staff       (20)       53 2023-07-27 21:35:29.000000 pixelpay-sdk-2.1.3/src/pixelpay/exceptions/FailedEncryptionException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/exceptions/InvalidCredentialsException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/exceptions/InvalidTransactionTypeException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      333 2023-07-27 21:35:45.000000 pixelpay-sdk-2.1.3/src/pixelpay/exceptions/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.109432 pixelpay-sdk-2.1.3/src/pixelpay/models/
+-rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/models/Billing.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/models/Card.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/models/Item.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/models/Order.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1914 2023-07-27 22:07:03.000000 pixelpay-sdk-2.1.3/src/pixelpay/models/Settings.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/models/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.117815 pixelpay-sdk-2.1.3/src/pixelpay/requests/
+-rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/AuthTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/CaptureTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3931 2023-08-07 23:12:45.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/CardTokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     5913 2023-08-07 22:52:35.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/PaymentTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/SaleTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/StatusTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/VoidTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/requests/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.120707 pixelpay-sdk-2.1.3/src/pixelpay/resources/
+-rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/resources/Environment.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.1.3/src/pixelpay/resources/Locations.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/resources/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.130471 pixelpay-sdk-2.1.3/src/pixelpay/responses/
+-rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/ErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/FailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/InputErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/NetworkFailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/NoAccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/NotFoundResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/PayloadResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/PaymentDeclinedResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/PreconditionalResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/SuccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/TimeoutResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/responses/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-08-07 23:31:06.133017 pixelpay-sdk-2.1.3/src/pixelpay/services/
+-rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/services/Tokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/services/Transaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.3/src/pixelpay/services/__init__.py
```

### Comparing `pixelpay-sdk-2.1.2/LICENSE.md` & `pixelpay-sdk-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/PKG-INFO` & `pixelpay-sdk-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpay-sdk
-Version: 2.1.2
+Version: 2.1.3
 Summary: PixelPay SDK toolkit.
 Author: Javier Cano
 Author-email: javier@pixel.hn
 License: MIT
 Keywords: pixelpay pixel pay sdk
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/PKG-INFO` & `pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpay-sdk
-Version: 2.1.2
+Version: 2.1.3
 Summary: PixelPay SDK toolkit.
 Author: Javier Cano
 Author-email: javier@pixel.hn
 License: MIT
 Keywords: pixelpay pixel pay sdk
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/SOURCES.txt` & `pixelpay-sdk-2.1.3/pixelpay_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/setup.py` & `pixelpay-sdk-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/assets/countries.json` & `pixelpay-sdk-2.1.3/src/pixelpay/assets/countries.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/assets/formats.json` & `pixelpay-sdk-2.1.3/src/pixelpay/assets/formats.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/assets/states.json` & `pixelpay-sdk-2.1.3/src/pixelpay/assets/states.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/base/Helpers.py` & `pixelpay-sdk-2.1.3/src/pixelpay/base/Helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import hashlib
+from typing import List
 from nacl.public import PublicKey, PrivateKey, Box
 from nacl.encoding import Base64Encoder
 
 
 class _Object:
     pass
 
@@ -14,26 +15,27 @@
 
         Raises:
             ValueError: Utility class
         """
         raise ValueError("Utility class")
 
     @staticmethod
-    def objectToJson(value: object) -> str:
+    def objectToJson(value: object, ignore: List = []) -> str:
         """Serialize object to JSON string without empties
 
         Args:
             value (object): object to serialize
+            ignore (List): key values that will be excluded from final JSON
 
         Returns:
             str: JSON string
         """
         temp_object = _Object()
         for key, val in value.__dict__.items():
-            if val is not None and val != "":
+            if val is not None and val != "" and key not in ignore:
                 setattr(temp_object, key.lstrip("_"), val)
         return json.dumps(temp_object, default=lambda o: o.__dict__)
 
     @staticmethod
     def hash(algorithm: str, value: str) -> str:
         encoded_value = value.encode("utf-8")
         if algorithm == "MD5":
@@ -109,15 +111,15 @@
 
         Returns:
             str: encrypted value concatenated with base64 nonce
         """
         if not message:
             return None
 
-        if not public_key:
+        if message.find("|") != -1:
             return message
 
         merchant_public_key = PublicKey(public_key.encode(), encoder=Base64Encoder)
 
         box_before = Box(key_pair, merchant_public_key)
 
         box_bytes = box_before.encrypt(message.encode())
```

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/base/RequestBehaviour.py` & `pixelpay-sdk-2.1.3/src/pixelpay/base/RequestBehaviour.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import locale
+from nacl.public import PrivateKey
 from .Helpers import Helpers
 from .. import __version__
 
 
 class RequestBehaviour:
     def __init__(self):
         """Initialize request"""
@@ -22,15 +23,15 @@
 
         self.from_type: str = "sdk-python"
         """SDK identifier type"""
 
         self.sdk_version: str = __version__
         """SDK version"""
 
-        self._sdk_public_key: str = None
+        self._sdk_key_pair: PrivateKey = None
         """For internal use to prevent encrypting same request instance twice"""
 
     def isEncryptable(self) -> bool:
         """Check if current request needs encryption, must be overriden by inherited classes.
 
         Returns:
             bool: true if request contains parameters that must be encrypted
@@ -57,15 +58,15 @@
 
         # because "from" is a reserved keyword,
         # we temporarily change the attribute "from_type" to "from"
         if self.from_type:
             setattr(self, "from", self.from_type)
             delattr(self, "from_type")
 
-        json_output = Helpers.objectToJson(self)
+        json_output = Helpers.objectToJson(self, ignore=['_sdk_key_pair'])
 
         # restore the previous changes
         from_attr = getattr(self, "from")
         if from_attr:
             setattr(self, "from_type", from_attr)
             delattr(self, "from")
```

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/base/Response.py` & `pixelpay-sdk-2.1.3/src/pixelpay/base/Response.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/base/ServiceBehaviour.py` & `pixelpay-sdk-2.1.3/src/pixelpay/base/ServiceBehaviour.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
         Raises:
             FailedEncryptionException: When encryption process fails
         """
         tries = 0
         last_error: FailedEncryptionException = None
 
-        while not self.__sdk_public_key and tries < 3:
+        while not self.__sdk_public_key and tries < 3 or tries == 0:
             try:
                 self.__sdk_public_key = request.withEncryption(self._settings.public_key)
             except Exception as e:
                 last_error = e
             finally:
                 tries += 1
```

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/entities/CardResult.py` & `pixelpay-sdk-2.1.3/src/pixelpay/entities/CardResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/entities/TransactionResult.py` & `pixelpay-sdk-2.1.3/src/pixelpay/entities/TransactionResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/models/Billing.py` & `pixelpay-sdk-2.1.3/src/pixelpay/models/Billing.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/models/Card.py` & `pixelpay-sdk-2.1.3/src/pixelpay/models/Card.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/models/Item.py` & `pixelpay-sdk-2.1.3/src/pixelpay/models/Item.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/models/Order.py` & `pixelpay-sdk-2.1.3/src/pixelpay/models/Order.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/models/Settings.py` & `pixelpay-sdk-2.1.3/src/pixelpay/models/Settings.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/requests/CardTokenization.py` & `pixelpay-sdk-2.1.3/src/pixelpay/requests/CardTokenization.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,18 +53,22 @@
         """Associate and mapping Card model properties to transaction
 
         Args:
             card (Card): input Card
         """
         self.number = Helpers.cleanString(card.number)
         self.cvv2 = card.cvv2
-        self.expire_month = "{:02d}".format(card.expire_month)
-        self.expire_year = str(card.expire_year)
         self.cardholder = Helpers.trimValue(card.cardholder)
 
+        if card.expire_month != 0:
+            self.expire_month = "{:02d}".format(card.expire_month)
+
+        if card.expire_year != 0:
+            self.expire_year = str(card.expire_year)
+
     def setBilling(self, billing: Billing):
         self.address = Helpers.trimValue(billing.address)
         self.country = billing.country
         self.state = billing.state
         self.city = Helpers.trimValue(billing.city)
         self.zip = billing.zip
         self.phone = billing.phone
@@ -93,33 +97,30 @@
 
         Raises:
             FailedEncryptionException: When public key is empty or encryption fails
 
         Returns:
             str: SDK public key
         """
-        if self._sdk_public_key:
-            return self._sdk_public_key
-
         if not public_key:
             raise FailedEncryptionException("Could not process transaction without merchant public key.")
 
         try:
-            key_pair = Helpers.getKeyPair()
+            key_pair = Helpers.getKeyPair() if not self._sdk_key_pair else self._sdk_key_pair
 
             number = Helpers.encrypt(self.number, public_key, key_pair)
             cvv2 = Helpers.encrypt(self.cvv2, public_key, key_pair)
             expire_month = Helpers.encrypt(self.expire_month, public_key, key_pair)
             expire_year = Helpers.encrypt(self.expire_year, public_key, key_pair)
 
             sdk_public_key = key_pair.public_key.encode(encoder=Base64Encoder).decode()
 
             self.number = number
             self.cvv2 = cvv2
             self.expire_month = expire_month
             self.expire_year = expire_year
 
-            self._sdk_public_key = sdk_public_key
+            self._sdk_key_pair = key_pair
 
-            return self._sdk_public_key
+            return sdk_public_key
         except:
             raise FailedEncryptionException("Encryption process encountered an unexpected error.")
```

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/requests/PaymentTransaction.py` & `pixelpay-sdk-2.1.3/src/pixelpay/requests/PaymentTransaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,31 +159,28 @@
 
         Raises:
             FailedEncryptionException: When public key is empty or encryption fails
 
         Returns:
             str: SDK public key
         """
-        if self._sdk_public_key:
-            return self._sdk_public_key
-
         if not public_key:
             raise FailedEncryptionException("Could not process transaction without merchant public key.")
 
         try:
-            key_pair = Helpers.getKeyPair()
+            key_pair = Helpers.getKeyPair() if not self._sdk_key_pair else self._sdk_key_pair
 
             card_number = Helpers.encrypt(self.card_number, public_key, key_pair)
             card_cvv = Helpers.encrypt(self.card_cvv, public_key, key_pair)
             card_expire = Helpers.encrypt(self.card_expire, public_key, key_pair)
 
             sdk_public_key = key_pair.public_key.encode(encoder=Base64Encoder).decode()
 
             self.card_number = card_number
             self.card_cvv = card_cvv
             self.card_expire = card_expire
 
-            self._sdk_public_key = sdk_public_key
+            self._sdk_key_pair = key_pair
 
-            return self._sdk_public_key
+            return sdk_public_key
         except:
             raise FailedEncryptionException("Encryption process encountered an unexpected error.")
```

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/requests/SaleTransaction.py` & `pixelpay-sdk-2.1.3/src/pixelpay/requests/SaleTransaction.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/requests/__init__.py` & `pixelpay-sdk-2.1.3/src/pixelpay/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/resources/Locations.py` & `pixelpay-sdk-2.1.3/src/pixelpay/resources/Locations.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/responses/__init__.py` & `pixelpay-sdk-2.1.3/src/pixelpay/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/services/Tokenization.py` & `pixelpay-sdk-2.1.3/src/pixelpay/services/Tokenization.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.2/src/pixelpay/services/Transaction.py` & `pixelpay-sdk-2.1.3/src/pixelpay/services/Transaction.py`

 * *Files identical despite different names*

