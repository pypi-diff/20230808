# Comparing `tmp/localstack-core-2.2.1.dev20230808025517.tar.gz` & `tmp/localstack-core-2.2.1.dev20230808030244.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.2.1.dev20230808025517.tar", last modified: Tue Aug  8 02:55:33 2023, max compression
+gzip compressed data, was "localstack-core-2.2.1.dev20230808030244.tar", last modified: Tue Aug  8 03:03:02 2023, max compression
```

## Comparing `localstack-core-2.2.1.dev20230808025517.tar` & `localstack-core-2.2.1.dev20230808030244.tar`

### file list

```diff
@@ -1,897 +1,906 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15463 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11767 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-08 02:55:17.000000 localstack-core-2.2.1.dev20230808025517/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89045 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.007736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   761978 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72158 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68029 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15408 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/scheduler/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.011736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10043 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10618 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49981 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14655 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.015736 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28990 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51487 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6236 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8744 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.019736 localstack-core-2.2.1.dev20230808025517/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.023736 localstack-core-2.2.1.dev20230808025517/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.023736 localstack-core-2.2.1.dev20230808025517/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.023736 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14992 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    85717 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.023736 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24649 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.023736 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.027736 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20045 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.027736 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   156015 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.027736 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3587 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.027736 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12539 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50605 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.031736 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33125 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20288 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      943 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2522 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6543 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2251 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5628 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21069 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2570 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8604 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27126 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3201 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2876 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4863 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1437 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3655 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13424 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6535 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4826 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10793 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5626 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41357 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26078 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.031736 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.031736 localstack-core-2.2.1.dev20230808025517/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.031736 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.031736 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4547 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6060 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.031736 localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24704 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6650 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.035736 localstack-core-2.2.1.dev20230808025517/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12066 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2556 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/cors.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68165 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15016 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17710 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    95851 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34001 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19181 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/scheduler/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/scheduler/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/scheduler/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.039736 localstack-core-2.2.1.dev20230808025517/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54706 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.043736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1531 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      744 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.047736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.055736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.055736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.055736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.055736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.059736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.059736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.059736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.063736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.067736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.067736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4331 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.067736 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6029 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10660 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.071735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.075735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2954 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1250 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1359 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3273 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6915 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.075735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1602 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1184 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7164 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.075735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1639 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.079735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.079735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6068 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5345 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5863 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5049 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9094 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5199 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.079735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.079735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3387 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1614 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.079735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.079735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.083735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1682 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.083735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5069 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1539 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1711 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      860 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32935 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8885 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2611 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14214 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.087735 localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7949 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.091735 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69100 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/marking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.091735 localstack-core-2.2.1.dev20230808025517/localstack/testing/scenario/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/scenario/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6860 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/scenario/provisioning.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.091735 localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.095735 localstack-core-2.2.1.dev20230808025517/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.095735 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.095735 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17941 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7674 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26833 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.095735 localstack-core-2.2.1.dev20230808025517/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48572 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33233 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4113 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 02:55:32.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40469 2023-08-08 02:55:32.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 02:55:32.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5400 2023-08-08 02:55:32.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 02:55:27.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5494 2023-08-08 02:55:27.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2894 2023-08-08 02:55:32.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-08-08 02:55:32.000000 localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3275 2023-08-08 02:55:33.099735 localstack-core-2.2.1.dev20230808025517/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-08-08 02:16:48.000000 localstack-core-2.2.1.dev20230808025517/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15463 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11767 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.943204 localstack-core-2.2.1.dev20230808030244/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.943204 localstack-core-2.2.1.dev20230808030244/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-08 03:02:44.000000 localstack-core-2.2.1.dev20230808030244/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89045 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   761978 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72158 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-08-08 02:26:09.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.947205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68029 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   135061 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15408 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/scheduler/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10043 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.951205 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10618 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49981 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14655 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31104 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28990 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51644 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.955205 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.959206 localstack-core-2.2.1.dev20230808030244/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6236 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.959206 localstack-core-2.2.1.dev20230808030244/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.959206 localstack-core-2.2.1.dev20230808030244/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8744 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.959206 localstack-core-2.2.1.dev20230808030244/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.959206 localstack-core-2.2.1.dev20230808030244/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.959206 localstack-core-2.2.1.dev20230808030244/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.963206 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14992 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    85717 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.963206 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24649 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.963206 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.963206 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20045 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.963206 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   156015 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.967206 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3587 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.967206 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12539 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50605 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33125 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20288 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      943 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2522 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6543 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2251 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5628 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21069 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2570 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8604 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27126 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3201 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2876 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4863 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1437 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3655 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13424 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6535 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4826 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10793 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5626 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41357 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26078 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4547 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6060 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.971207 localstack-core-2.2.1.dev20230808030244/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24704 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6650 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12249 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.975207 localstack-core-2.2.1.dev20230808030244/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3028 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/exceptions.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68165 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15016 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17710 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    95039 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34001 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23872 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22373 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49285 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/storage/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/storage/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/storage/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/v3/storage/ephemeral.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.979207 localstack-core-2.2.1.dev20230808030244/localstack/services/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/scheduler/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/scheduler/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/scheduler/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54706 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.983208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1531 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      744 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.987208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.991208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.991208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.991208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.991208 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:01.999209 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.007210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.007210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.007210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.007210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.007210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4331 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.007210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6029 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.011210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.011210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.011210 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10660 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2954 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1250 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1359 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3273 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6915 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1602 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1184 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7164 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.015211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1639 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.019211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6068 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5345 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5863 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5049 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9094 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5199 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3387 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1614 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1682 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5069 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1539 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1711 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      860 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32935 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.023211 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8885 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2611 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14214 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7949 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69100 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/marking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.031212 localstack-core-2.2.1.dev20230808030244/localstack/testing/scenario/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/scenario/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6860 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/scenario/provisioning.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.035212 localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.035212 localstack-core-2.2.1.dev20230808030244/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.039213 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.039213 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17941 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7674 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26833 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.039213 localstack-core-2.2.1.dev20230808030244/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48572 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33233 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4113 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 03:03:01.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40753 2023-08-08 03:03:01.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 03:03:01.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5444 2023-08-08 03:03:01.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 03:02:56.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5539 2023-08-08 03:02:56.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2894 2023-08-08 03:03:01.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-08-08 03:03:01.000000 localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3275 2023-08-08 03:03:02.043213 localstack-core-2.2.1.dev20230808030244/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-08-08 02:26:10.000000 localstack-core-2.2.1.dev20230808030244/setup.py
```

### Comparing `localstack-core-2.2.1.dev20230808025517/LICENSE.txt` & `localstack-core-2.2.1.dev20230808030244/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/Makefile` & `localstack-core-2.2.1.dev20230808030244/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/PKG-INFO` & `localstack-core-2.2.1.dev20230808030244/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230808025517
+Version: 2.2.1.dev20230808030244
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230808025517/README.md` & `localstack-core-2.2.1.dev20230808030244/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/bin/localstack` & `localstack-core-2.2.1.dev20230808030244/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/bin/localstack-supervisor` & `localstack-core-2.2.1.dev20230808030244/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/accounts.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/acm/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/config/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/core.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/es/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/events/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/iam/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/kms/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/logs/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/route53/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/s3/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/s3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,14 @@
 StringToSignBytes = str
 CanonicalRequest = str
 CanonicalRequestBytes = str
 X_Amz_Expires = int
 HttpMethod = str
 ResourceType = str
 MissingHeaderName = str
-Method = str
 
 
 class AnalyticsS3ExportFileFormat(str):
     CSV = "CSV"
 
 
 class ArchiveStatus(str):
@@ -608,14 +607,16 @@
 
 
 class NoSuchKey(ServiceException):
     code: str = "NoSuchKey"
     sender_fault: bool = False
     status_code: int = 404
     Key: Optional[ObjectKey]
+    DeleteMarker: Optional[DeleteMarker]
+    VersionId: Optional[ObjectVersionId]
 
 
 class NoSuchUpload(ServiceException):
     code: str = "NoSuchUpload"
     sender_fault: bool = False
     status_code: int = 404
     UploadId: Optional[MultipartUploadId]
@@ -643,14 +644,22 @@
 class InvalidBucketName(ServiceException):
     code: str = "InvalidBucketName"
     sender_fault: bool = False
     status_code: int = 400
     BucketName: Optional[BucketName]
 
 
+class NoSuchVersion(ServiceException):
+    code: str = "NoSuchVersion"
+    sender_fault: bool = False
+    status_code: int = 404
+    VersionId: Optional[ObjectVersionId]
+    Key: Optional[ObjectKey]
+
+
 class PreconditionFailed(ServiceException):
     code: str = "PreconditionFailed"
     sender_fault: bool = False
     status_code: int = 412
     Condition: Optional[IfCondition]
 
 
@@ -767,16 +776,19 @@
     StorageClassRequested: Optional[StorageClass]
 
 
 class MethodNotAllowed(ServiceException):
     code: str = "MethodNotAllowed"
     sender_fault: bool = False
     status_code: int = 405
-    Method: Optional[Method]
+    Method: Optional[HttpMethod]
     ResourceType: Optional[ResourceType]
+    DeleteMarker: Optional[DeleteMarker]
+    VersionId: Optional[ObjectVersionId]
+    Allow: Optional[HttpMethod]
 
 
 class CrossLocationLoggingProhibitted(ServiceException):
     code: str = "CrossLocationLoggingProhibitted"
     sender_fault: bool = False
     status_code: int = 403
     TargetBucketLocation: Optional[BucketRegion]
@@ -785,14 +797,21 @@
 class InvalidTargetBucketForLogging(ServiceException):
     code: str = "InvalidTargetBucketForLogging"
     sender_fault: bool = False
     status_code: int = 400
     TargetBucket: Optional[BucketName]
 
 
+class BucketNotEmpty(ServiceException):
+    code: str = "BucketNotEmpty"
+    sender_fault: bool = False
+    status_code: int = 409
+    BucketName: Optional[BucketName]
+
+
 AbortDate = datetime
 
 
 class AbortIncompleteMultipartUpload(TypedDict, total=False):
     DaysAfterInitiation: Optional[DaysAfterInitiation]
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/scheduler/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ses/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sns/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/sts/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/support/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/swf/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/app.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/chain.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/connect.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/forwarder.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/gateway.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/analytics.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/auth.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/codec.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/cors.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/fallback.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/internal.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/legacy.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/logging.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/proxy.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/region.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/routes.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/service.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/mocking.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/op_router.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/parser.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/serializer.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/service_router.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/protocol/validate.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/proxy.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/scaffold.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/asgi.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/edge.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/hypercorn.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/werkzeug.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/serving/wsgi.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/skeleton.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/spec-patches.json` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/spec-patches.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9661430180180182%*

 * *Differences: {"'s3/2006-03-01/service-2'": "{60: {'value': {'members': {'Method': {'shape': 'HttpMethod'}, "*

 * *                              "'DeleteMarker': OrderedDict([('shape', 'DeleteMarker'), "*

 * *                              "('location', 'header'), ('locationName', 'x-amz-delete-marker')]), "*

 * *                              "'VersionId': OrderedDict([('shape', 'ObjectVersionId'), "*

 * *                              "('location', 'header'), ('locationName', 'x-amz-version-id')]), "*

 * *                              "'Allow': O […]*

```diff
@@ -125,14 +125,52 @@
             "path": "/shapes/NoSuchKey/error",
             "value": {
                 "httpStatusCode": 404
             }
         },
         {
             "op": "add",
+            "path": "/shapes/NoSuchKey/members/DeleteMarker",
+            "value": {
+                "location": "header",
+                "locationName": "x-amz-delete-marker",
+                "shape": "DeleteMarker"
+            }
+        },
+        {
+            "op": "add",
+            "path": "/shapes/NoSuchKey/members/VersionId",
+            "value": {
+                "location": "header",
+                "locationName": "x-amz-version-id",
+                "shape": "ObjectVersionId"
+            }
+        },
+        {
+            "op": "add",
+            "path": "/shapes/NoSuchVersion",
+            "value": {
+                "documentation": "<p></p>",
+                "error": {
+                    "httpStatusCode": 404
+                },
+                "exception": true,
+                "members": {
+                    "Key": {
+                        "shape": "ObjectKey"
+                    },
+                    "VersionId": {
+                        "shape": "ObjectVersionId"
+                    }
+                },
+                "type": "structure"
+            }
+        },
+        {
+            "op": "add",
             "path": "/shapes/PreconditionFailed",
             "value": {
                 "documentation": "<p>At least one of the pre-conditions you specified did not hold</p>",
                 "error": {
                     "httpStatusCode": 412
                 },
                 "exception": true,
@@ -749,21 +787,14 @@
                 "location": "header",
                 "locationName": "x-amz-bucket-region",
                 "shape": "BucketRegion"
             }
         },
         {
             "op": "add",
-            "path": "/shapes/Method",
-            "value": {
-                "type": "string"
-            }
-        },
-        {
-            "op": "add",
             "path": "/shapes/ResourceType",
             "value": {
                 "type": "string"
             }
         },
         {
             "op": "add",
@@ -771,19 +802,34 @@
             "value": {
                 "documentation": "<p>The specified method is not allowed against this resource.</p>",
                 "error": {
                     "httpStatusCode": 405
                 },
                 "exception": true,
                 "members": {
+                    "Allow": {
+                        "location": "header",
+                        "locationName": "allow",
+                        "shape": "HttpMethod"
+                    },
+                    "DeleteMarker": {
+                        "location": "header",
+                        "locationName": "x-amz-delete-marker",
+                        "shape": "DeleteMarker"
+                    },
                     "Method": {
-                        "shape": "Method"
+                        "shape": "HttpMethod"
                     },
                     "ResourceType": {
                         "shape": "ResourceType"
+                    },
+                    "VersionId": {
+                        "location": "header",
+                        "locationName": "x-amz-version-id",
+                        "shape": "ObjectVersionId"
                     }
                 },
                 "type": "structure"
             }
         },
         {
             "op": "remove",
@@ -865,10 +911,27 @@
             "path": "/operations/PutBucketAnalyticsConfiguration/http/responseCode",
             "value": 204
         },
         {
             "op": "add",
             "path": "/operations/PutBucketIntelligentTieringConfiguration/http/responseCode",
             "value": 204
+        },
+        {
+            "op": "add",
+            "path": "/shapes/BucketNotEmpty",
+            "value": {
+                "documentation": "<p>The bucket you tried to delete is not empty</p>",
+                "error": {
+                    "httpStatusCode": 409
+                },
+                "exception": true,
+                "members": {
+                    "BucketName": {
+                        "shape": "BucketName"
+                    }
+                },
+                "type": "structure"
+            }
         }
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/spec.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/aws/trace.py` & `localstack-core-2.2.1.dev20230808030244/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/cli/localstack.py` & `localstack-core-2.2.1.dev20230808030244/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/cli/lpm.py` & `localstack-core-2.2.1.dev20230808030244/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/cli/plugin.py` & `localstack-core-2.2.1.dev20230808030244/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/cli/plugins.py` & `localstack-core-2.2.1.dev20230808030244/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/cli/profiles.py` & `localstack-core-2.2.1.dev20230808030244/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/config.py` & `localstack-core-2.2.1.dev20230808030244/localstack/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,14 +426,17 @@
 
 # whether legacy s3 is enabled
 LEGACY_S3_PROVIDER = os.environ.get("PROVIDER_OVERRIDE_S3", "") == "legacy"
 
 # whether the S3 streaming provider is enabled (beware, it breaks persistence for now)
 STREAM_S3_PROVIDER = os.environ.get("PROVIDER_OVERRIDE_S3", "") == "stream"
 
+# whether the S3 native provider is enabled (beware, it breaks persistence for now)
+NATIVE_S3_PROVIDER = os.environ.get("PROVIDER_OVERRIDE_S3", "") == "v3"
+
 # Whether to report internal failures as 500 or 501 errors.
 FAIL_FAST = is_env_true("FAIL_FAST")
 
 # whether to use the legacy single-region mode, defined via DEFAULT_REGION
 USE_SINGLE_REGION = is_env_true("USE_SINGLE_REGION")
 
 # whether to run in TF compatibility mode for TF integration tests
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/constants.py` & `localstack-core-2.2.1.dev20230808030244/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/deprecations.py` & `localstack-core-2.2.1.dev20230808030244/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/aws.py` & `localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/extensions/api/extension.py` & `localstack-core-2.2.1.dev20230808030244/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/adapters.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/asgi.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/dispatcher.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/hypercorn.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/proxy.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/request.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/resource.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/response.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/http/router.py` & `localstack-core-2.2.1.dev20230808030244/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/logging/format.py` & `localstack-core-2.2.1.dev20230808030244/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/logging/setup.py` & `localstack-core-2.2.1.dev20230808030244/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/packages/__init__.py` & `localstack-core-2.2.1.dev20230808030244/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/packages/api.py` & `localstack-core-2.2.1.dev20230808030244/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/packages/core.py` & `localstack-core-2.2.1.dev20230808030244/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/packages/debugpy.py` & `localstack-core-2.2.1.dev20230808030244/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/packages/ffmpeg.py` & `localstack-core-2.2.1.dev20230808030244/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/packages/terraform.py` & `localstack-core-2.2.1.dev20230808030244/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/plugins.py` & `localstack-core-2.2.1.dev20230808030244/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/runtime/analytics.py` & `localstack-core-2.2.1.dev20230808030244/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/runtime/hooks.py` & `localstack-core-2.2.1.dev20230808030244/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/runtime/init.py` & `localstack-core-2.2.1.dev20230808030244/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/runtime/main.py` & `localstack-core-2.2.1.dev20230808030244/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/runtime/shutdown.py` & `localstack-core-2.2.1.dev20230808030244/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/acm/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/context.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/helpers.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/integration.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/invocations.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/patches.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/router_asf.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/apigateway/templates.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/api_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/hooks.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/plugins.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/deploy.html` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/events.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/service_models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudformation/stores.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/cloudwatch/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/server.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodb/utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/exceptions.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ec2/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/edge.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/es/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/events/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/events/scheduler.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/mappers.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/firehose/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/generic_proxy.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/iam/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.2.1.dev20230808030244/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/infra.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/internal.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kinesis/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kms/local_kms_server.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kms/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kms/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kms/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/kms/utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/logs/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/logs/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/messages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/moto.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/motoserver.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/cluster.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/opensearch/versions.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/plugins.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/providers.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,14 +275,22 @@
 def s3_stream():
     from localstack.services.s3.provider_stream import S3ProviderStream
 
     provider = S3ProviderStream()
     return Service.for_provider(provider, dispatch_table_factory=MotoFallbackDispatcher)
 
 
+@aws_provider(api="s3", name="v3")
+def s3_v3():
+    from localstack.services.s3.v3.provider import S3Provider
+
+    provider = S3Provider()
+    return Service.for_provider(provider)
+
+
 @aws_provider()
 def s3control():
     from localstack.services.s3control.provider import S3ControlProvider
 
     provider = S3ControlProvider()
     return Service.for_provider(provider, dispatch_table_factory=MotoFallbackDispatcher)
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/redshift/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/route53/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/route53resolver/utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/codec.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/constants.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from localstack.aws.api.s3 import BucketCannedACL, ObjectCannedACL, Permission, StorageClass
 
 S3_VIRTUAL_HOST_FORWARDED_HEADER = "x-s3-vhost-forwarded-for"
 
+S3_UPLOAD_PART_MIN_SIZE = 5242880
+"""
+This is minimum size allowed by S3 when uploading more than one part for a Multipart Upload, except for the last part
+"""
+
 VALID_CANNED_ACLS_BUCKET = {
     # https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl
     # bucket-owner-read + bucket-owner-full-control are allowed, but ignored for buckets
     ObjectCannedACL.private,
     ObjectCannedACL.authenticated_read,
     ObjectCannedACL.aws_exec_read,
     ObjectCannedACL.bucket_owner_full_control,
@@ -36,14 +41,21 @@
     StorageClass.GLACIER_IR,
     StorageClass.REDUCED_REDUNDANCY,
     StorageClass.ONEZONE_IA,
     StorageClass.INTELLIGENT_TIERING,
     StorageClass.DEEP_ARCHIVE,
 ]
 
+# TODO validate those?
+ARCHIVES_STORAGE_CLASSES = [
+    StorageClass.GLACIER,
+    StorageClass.GLACIER_IR,
+    StorageClass.DEEP_ARCHIVE,
+]
+
 # response header overrides the client may request
 ALLOWED_HEADER_OVERRIDES = {
     "ResponseContentType": "ContentType",
     "ResponseContentLanguage": "ContentLanguage",
     "ResponseExpires": "Expires",
     "ResponseCacheControl": "CacheControl",
     "ResponseContentDisposition": "ContentDisposition",
@@ -51,14 +63,24 @@
 }
 
 # Whether to enable S3 bucket policy enforcement in moto - currently disabled, as some recent CDK versions
 # are creating bucket policies that enforce aws:SecureTransport, which makes the CDK deployment fail.
 # TODO: potentially look into making configurable
 ENABLE_MOTO_BUCKET_POLICY_ENFORCEMENT = False
 
+
+SYSTEM_METADATA_SETTABLE_HEADERS = [
+    "CacheControl",
+    "ContentDisposition",
+    "ContentEncoding",
+    "ContentLanguage",
+    "ContentMD5",
+    "ContentType",
+]
+
 # params are required in presigned url
 SIGNATURE_V2_PARAMS = ["Signature", "Expires", "AWSAccessKeyId"]
 
 SIGNATURE_V4_PARAMS = [
     "X-Amz-Algorithm",
     "X-Amz-Credential",
     "X-Amz-Date",
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/cors.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/multipart_content.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/s3_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/s3_starter.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/legacy/s3_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/legacy/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/notifications.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/presigned_url.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,21 @@
 )
 from localstack.services.edge import ROUTER
 from localstack.services.moto import call_moto
 from localstack.services.plugins import ServiceLifecycleHook
 from localstack.services.s3 import constants as s3_constants
 from localstack.services.s3.codec import AwsChunkedDecoder
 from localstack.services.s3.cors import S3CorsHandler, s3_cors_request_handler
+from localstack.services.s3.exceptions import (
+    InvalidRequest,
+    MalformedACLError,
+    MalformedXML,
+    NoSuchConfiguration,
+    UnexpectedContent,
+)
 from localstack.services.s3.models import S3Store, get_moto_s3_backend, s3_stores
 from localstack.services.s3.notifications import NotificationDispatcher, S3EventNotificationContext
 from localstack.services.s3.presigned_url import (
     s3_presigned_url_request_handler,
     s3_presigned_url_response_handler,
     validate_post_policy,
 )
@@ -193,41 +200,14 @@
 ] = "s3.localhost.localstack.cloud:4566,s3.localhost.localstack.cloud"
 
 MOTO_CANONICAL_USER_ID = "75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a"
 # max file size for S3 objects kept in memory (500 KB by default)
 S3_MAX_FILE_SIZE_BYTES = 512 * 1024
 
 
-class MalformedXML(CommonServiceException):
-    def __init__(self, message=None):
-        if not message:
-            message = "The XML you provided was not well-formed or did not validate against our published schema"
-        super().__init__("MalformedXML", status_code=400, message=message)
-
-
-class MalformedACLError(CommonServiceException):
-    def __init__(self, message=None):
-        super().__init__("MalformedACLError", status_code=400, message=message)
-
-
-class InvalidRequest(CommonServiceException):
-    def __init__(self, message=None):
-        super().__init__("InvalidRequest", status_code=400, message=message)
-
-
-class UnexpectedContent(CommonServiceException):
-    def __init__(self, message=None):
-        super().__init__("UnexpectedContent", status_code=400, message=message)
-
-
-class NoSuchConfiguration(CommonServiceException):
-    def __init__(self, message=None):
-        super().__init__("NoSuchConfiguration", status_code=404, message=message)
-
-
 def get_full_default_bucket_location(bucket_name):
     if config.HOSTNAME_EXTERNAL != config.LOCALHOST:
         host_definition = localstack_host(
             use_hostname_external=True, custom_port=config.get_edge_port_http()
         )
         return f"{config.get_protocol()}://{host_definition.host_and_port()}/{bucket_name}/"
     else:
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/provider_stream.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import datetime
 import hashlib
 import logging
 import re
 import zlib
-from typing import IO, Dict, Literal, Optional, Tuple, Union
+from dataclasses import dataclass
+from typing import IO, Any, Dict, Literal, Optional, Protocol, Tuple, Type, Union
 from urllib import parse as urlparser
 from zoneinfo import ZoneInfo
 
 import moto.s3.models as moto_s3_models
 from botocore.exceptions import ClientError
 from botocore.utils import InvalidArnException
 from moto.s3.exceptions import MissingBucket
 from moto.s3.models import FakeBucket, FakeDeleteMarker, FakeKey
 from moto.s3.utils import clean_key_name
 
-from localstack.aws.api import CommonServiceException, RequestContext, ServiceException
+from localstack import config
+from localstack.aws.api import CommonServiceException, RequestContext
 from localstack.aws.api.s3 import (
     BucketName,
     ChecksumAlgorithm,
     CopySource,
     InvalidArgument,
+    InvalidRange,
     LifecycleExpiration,
     LifecycleRule,
     LifecycleRules,
+    Metadata,
     MethodNotAllowed,
     NoSuchBucket,
     NoSuchKey,
     ObjectKey,
+    ObjectVersionId,
+    Owner,
 )
 from localstack.aws.connect import connect_to
 from localstack.services.s3.constants import (
     S3_CHUNK_SIZE,
     S3_VIRTUAL_HOST_FORWARDED_HEADER,
     SIGNATURE_V2_PARAMS,
     SIGNATURE_V4_PARAMS,
+    SYSTEM_METADATA_SETTABLE_HEADERS,
     VALID_CANNED_ACLS_BUCKET,
 )
+from localstack.services.s3.exceptions import InvalidRequest
 from localstack.utils.aws import arns
 from localstack.utils.aws.arns import parse_arn
 from localstack.utils.strings import checksum_crc32, checksum_crc32c, hash_sha1, hash_sha256
+from localstack.utils.urls import localstack_host
 
 LOG = logging.getLogger(__name__)
 
 checksum_keys = ["ChecksumSHA1", "ChecksumSHA256", "ChecksumCRC32", "ChecksumCRC32C"]
 
 BUCKET_NAME_REGEX = (
     r"(?=^.{3,63}$)(?!^(\d+\.)+\d+$)"
@@ -66,37 +75,58 @@
     r"[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}"
 )
 
 
 RFC1123 = "%a, %d %b %Y %H:%M:%S GMT"
 
 
-class InvalidRequest(ServiceException):
-    code: str = "InvalidRequest"
-    sender_fault: bool = False
-    status_code: int = 400
+def get_owner_for_account_id(account_id: str):
+    """
+    This method returns the S3 Owner from the account id. for now, this is hardcoded as it was in moto, but we can then
+    extend it to return different values depending on the account ID
+    See https://docs.aws.amazon.com/AmazonS3/latest/API/API_Owner.html
+    :param account_id: the owner account id
+    :return: the Owner object containing the DisplayName and owner ID
+    """
+    return Owner(
+        DisplayName="webfile",  # only in certain regions, see above
+        ID="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
+    )
 
 
 def extract_bucket_key_version_id_from_copy_source(
     copy_source: CopySource,
-) -> tuple[BucketName, ObjectKey, Optional[str]]:
+) -> tuple[BucketName, ObjectKey, Optional[ObjectVersionId]]:
     """
     Utility to parse bucket name, object key and optionally its versionId. It accepts the CopySource format:
     - <bucket-name/<object-key>?versionId=<version-id>, used for example in CopySource for CopyObject
     :param copy_source: the S3 CopySource to parse
     :return: parsed BucketName, ObjectKey and optionally VersionId
     """
     copy_source_parsed = urlparser.urlparse(copy_source)
     src_bucket, src_key = urlparser.unquote(copy_source_parsed.path).lstrip("/").split("/", 1)
     src_version_id = urlparser.parse_qs(copy_source_parsed.query).get("versionId", [None])[0]
 
     return src_bucket, src_key, src_version_id
 
 
-def get_s3_checksum(algorithm):
+class ChecksumHash(Protocol):
+    """
+    This Protocol allows proper typing for different kind of hash used by S3 (hashlib.shaX, zlib.crc32 from
+    S3CRC32Checksum, and botocore CrtCrc32cChecksum).
+    """
+
+    def digest(self) -> bytes:
+        ...
+
+    def update(self, value: bytes):
+        ...
+
+
+def get_s3_checksum(algorithm) -> ChecksumHash:
     match algorithm:
         case ChecksumAlgorithm.CRC32:
             return S3CRC32Checksum()
 
         case ChecksumAlgorithm.CRC32C:
             from botocore.httpchecksum import CrtCrc32cChecksum
 
@@ -110,14 +140,16 @@
 
         case _:
             # TODO: check proper error? for now validated client side, need to check server response
             raise InvalidRequest("The value specified in the x-amz-trailer header is not supported")
 
 
 class S3CRC32Checksum:
+    """Implements a unified way of using zlib.crc32 compatibl with hashlib.sha and botocore CrtCrc32cChecksum"""
+
     __slots__ = ["checksum"]
 
     def __init__(self):
         self.checksum = None
 
     def update(self, value: bytes):
         if self.checksum is None:
@@ -126,15 +158,77 @@
 
         self.checksum = zlib.crc32(value, self.checksum)
 
     def digest(self) -> bytes:
         return self.checksum.to_bytes(4, "big")
 
 
-def get_object_checksum_for_algorithm(checksum_algorithm: str, data: bytes):
+@dataclass
+class ParsedRange:
+    """
+    Dataclass representing a parsed Range header with the requested S3 object size
+    https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Range
+    """
+
+    content_range: str  # the original Range header
+    content_length: int  # the full requested object size
+    begin: int  # the start of range
+    end: int  # the end of the end
+
+
+def parse_range_header(range_header: str, object_size: int) -> ParsedRange:
+    """
+    Takes a Range header, and returns a dataclass containing the necessary information to return only a slice of an
+    S3 object
+    :param range_header: a Range header
+    :param object_size: the requested S3 object total size
+    :return: ParsedRange
+    """
+    last = object_size - 1
+    _, rspec = range_header.split("=")
+    # TODO: check with AWS
+    if "," in rspec:
+        raise NotImplementedError("Multiple range specifiers not supported")
+
+    begin, end = [int(i) if i else None for i in rspec.split("-")]
+    if begin is not None:  # byte range
+        end = last if end is None else min(end, last)
+    elif end is not None:  # suffix byte range
+        begin = object_size - min(end, object_size)
+        end = last
+    else:
+        # TODO, find exception here
+        raise Exception("TODO")
+    if begin < 0 or end > last or begin > min(end, last):
+        raise InvalidRange(
+            "",
+            ActualObjectSize=str(object_size),
+            RangeRequest=range_header,
+        )
+
+    return ParsedRange(
+        content_range=f"bytes {begin}-{end}/{object_size}",
+        content_length=end - begin + 1,
+        begin=begin,
+        end=end,
+    )
+
+
+def get_full_default_bucket_location(bucket_name: BucketName) -> str:
+    if config.HOSTNAME_EXTERNAL != config.LOCALHOST:
+        host_definition = localstack_host(
+            use_hostname_external=True, custom_port=config.get_edge_port_http()
+        )
+        return f"{config.get_protocol()}://{host_definition.host_and_port()}/{bucket_name}/"
+    else:
+        host_definition = localstack_host(use_localhost_cloud=True)
+        return f"{config.get_protocol()}://{bucket_name}.s3.{host_definition.host_and_port()}/"
+
+
+def get_object_checksum_for_algorithm(checksum_algorithm: str, data: bytes) -> str:
     match checksum_algorithm:
         case ChecksumAlgorithm.CRC32:
             return checksum_crc32(data)
 
         case ChecksumAlgorithm.CRC32C:
             return checksum_crc32c(data)
 
@@ -255,14 +349,28 @@
     return (
         True
         if ".s3" in host and ((match := _s3_virtual_host_regex.match(host)) and match.group(3))
         else False
     )
 
 
+def get_class_attrs_from_spec_class(spec_class: Type[str]) -> set[str]:
+    return {attr for attr in vars(spec_class) if not attr.startswith("__")}
+
+
+def get_system_metadata_from_request(request: dict) -> Metadata:
+    metadata: Metadata = {}
+
+    for system_metadata_field in SYSTEM_METADATA_SETTABLE_HEADERS:
+        if field_value := request.get(system_metadata_field):
+            metadata[system_metadata_field] = field_value
+
+    return metadata
+
+
 def forwarded_from_virtual_host_addressed_request(headers: dict[str, str]) -> bool:
     """
     Determines if the request was forwarded from a v-host addressing style into a path one
     """
     # we can assume that the host header we are receiving here is actually the header we originally received
     # from the client (because the edge service is forwarding the request in memory)
     match = re.match(S3_VIRTUAL_HOSTNAME_REGEX, headers.get(S3_VIRTUAL_HOST_FORWARDED_HEADER, ""))
@@ -383,43 +491,49 @@
     return ex
 
 
 def capitalize_header_name_from_snake_case(header_name: str) -> str:
     return "-".join([part.capitalize() for part in header_name.split("-")])
 
 
-def validate_kms_key_id(kms_key: str, bucket: FakeBucket) -> None:
+# TODO: replace Any by a replacement for S3Bucket, some kind of defined type?
+def validate_kms_key_id(kms_key: str, bucket: FakeBucket | Any) -> None:
     """
     Validate that the KMS key used to encrypt the object is valid
     :param kms_key: the KMS key id or ARN
     :param bucket: the targeted bucket
     :raise KMS.DisabledException if the key is disabled
     :raise KMS.NotFoundException if the key is not in the same region or does not exist
     :return: the key ARN if found and enabled
     """
+    if hasattr(bucket, "region_name"):
+        bucket_region = bucket.region_name
+    else:
+        bucket_region = bucket.bucket_region
+
     try:
         parsed_arn = parse_arn(kms_key)
         key_region = parsed_arn["region"]
         # the KMS key should be in the same region as the bucket, we can raise an exception without calling KMS
-        if key_region != bucket.region_name:
+        if key_region != bucket_region:
             raise CommonServiceException(
                 code="KMS.NotFoundException", message=f"Invalid arn {key_region}"
             )
 
     except InvalidArnException:
         # if it fails, the passed ID is a UUID with no region data
         key_id = kms_key
         # recreate the ARN manually with the bucket region and bucket owner
         # if the KMS key is cross-account, user should provide an ARN and not a KeyId
         kms_key = arns.kms_key_arn(
-            key_id=key_id, account_id=bucket.account_id, region_name=bucket.region_name
+            key_id=key_id, account_id=bucket.account_id, region_name=bucket_region
         )
 
     # the KMS key should be in the same region as the bucket, create the client in the bucket region
-    kms_client = connect_to(region_name=bucket.region_name).kms
+    kms_client = connect_to(region_name=bucket_region).kms
     try:
         key = kms_client.describe_key(KeyId=kms_key)
         if not key["KeyMetadata"]["Enabled"]:
             if key["KeyMetadata"]["KeyState"] == "PendingDeletion":
                 raise CommonServiceException(
                     code="KMS.KMSInvalidStateException",
                     message=f'{key["KeyMetadata"]["Arn"]} is pending deletion.',
@@ -440,24 +554,44 @@
     return src.strftime(RFC1123)
 
 
 def str_to_rfc_1123_datetime(value: str) -> datetime.datetime:
     return datetime.datetime.strptime(value, RFC1123).replace(tzinfo=ZoneInfo("GMT"))
 
 
+def iso_8601_datetime_without_milliseconds_s3(
+    value: datetime,
+) -> Optional[str]:
+    return value.strftime("%Y-%m-%dT%H:%M:%S.000Z") if value else None
+
+
+def add_expiration_days_to_datetime(user_datatime: datetime.datetime, exp_days: int) -> str:
+    """
+    This adds expiration days to a datetime, rounding to the next day at midnight UTC.
+    :param user_datatime: datetime object
+    :param exp_days: provided days
+    :return: return a datetime object, rounded to midnight, in string formatted to rfc_1123
+    """
+    rounded_datetime = user_datatime.replace(
+        hour=0, minute=0, second=0, microsecond=0
+    ) + datetime.timedelta(days=exp_days + 1)
+
+    return rfc_1123_datetime(rounded_datetime)
+
+
 def serialize_expiration_header(
     rule_id: str, lifecycle_exp: LifecycleExpiration, last_modified: datetime.datetime
 ):
-    if not (exp_date := lifecycle_exp.get("Date")):
-        exp_days = lifecycle_exp.get("Days")
+    if exp_days := lifecycle_exp.get("Days"):
         # AWS round to the next day at midnight UTC
-        exp_date = last_modified.replace(
-            hour=0, minute=0, second=0, microsecond=0
-        ) + datetime.timedelta(days=exp_days + 1)
-    return f'expiry-date="{rfc_1123_datetime(exp_date)}", rule-id="{rule_id}"'
+        exp_date = add_expiration_days_to_datetime(last_modified, exp_days)
+    else:
+        exp_date = rfc_1123_datetime(lifecycle_exp["Date"])
+
+    return f'expiry-date="{exp_date}", rule-id="{rule_id}"'
 
 
 def get_lifecycle_rule_from_object(
     lifecycle_conf_rules: LifecycleRules, moto_object: FakeKey, object_tags: dict[str, str]
 ) -> LifecycleRule:
     for rule in lifecycle_conf_rules:
         if not (expiration := rule.get("Expiration")) or "ExpiredObjectDeleteMarker" in expiration:
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/virtual_host.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/s3/website_hosting.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/secretsmanager/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ses/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sns/constants.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sns/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sns/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sns/publisher.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/constants.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/exceptions.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/query_api.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sqs/utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.2.1.dev20230808030244/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/program_state.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/program_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/packages.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/stores.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/sts/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/services/transcribe/provider.py` & `localstack-core-2.2.1.dev20230808030244/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/state/core.py` & `localstack-core-2.2.1.dev20230808030244/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/state/inspect.py` & `localstack-core-2.2.1.dev20230808030244/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/state/pickle.py` & `localstack-core-2.2.1.dev20230808030244/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/state/snapshot.py` & `localstack-core-2.2.1.dev20230808030244/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/asf_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/aws/util.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/filters.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/fixtures.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/marking.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/marking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/snapshot.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/pytest/util.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/scenario/provisioning.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/scenario/provisioning.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/prototype.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/report.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/transformer.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.2.1.dev20230808030244/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/cli.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/events.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/logger.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/metadata.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/publisher.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/analytics/usage.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/archives.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/asyncio.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/auth.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/arns.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/aws_models.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/aws_responses.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/aws_stack.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/client_types.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/queries.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/request_context.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/resources.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/aws/templating.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/bootstrap.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/collections.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/common.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/config_listener.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/container_networking.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/container_client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/coverage_docs.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/crypto.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/diagnose.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/docker_utils.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/files.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/functions.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/http.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/json.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/net.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/numbers.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/objects.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/patch.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/platform.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/run.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/scheduler.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/server/http2_server.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/server/proxy_server.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/serving.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/ssl.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/strings.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/sync.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/tagging.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/tail.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/testutil.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/threads.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/time.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/urls.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/venv.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack/utils/xml.py` & `localstack-core-2.2.1.dev20230808030244/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230808025517
+Version: 2.2.1.dev20230808030244
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -324,27 +324,34 @@
 localstack/services/route53resolver/models.py
 localstack/services/route53resolver/provider.py
 localstack/services/route53resolver/utils.py
 localstack/services/s3/__init__.py
 localstack/services/s3/codec.py
 localstack/services/s3/constants.py
 localstack/services/s3/cors.py
+localstack/services/s3/exceptions.py
 localstack/services/s3/models.py
 localstack/services/s3/notifications.py
 localstack/services/s3/presigned_url.py
 localstack/services/s3/provider.py
 localstack/services/s3/provider_stream.py
 localstack/services/s3/utils.py
 localstack/services/s3/virtual_host.py
 localstack/services/s3/website_hosting.py
 localstack/services/s3/legacy/__init__.py
 localstack/services/s3/legacy/multipart_content.py
 localstack/services/s3/legacy/s3_listener.py
 localstack/services/s3/legacy/s3_starter.py
 localstack/services/s3/legacy/s3_utils.py
+localstack/services/s3/v3/__init__.py
+localstack/services/s3/v3/models.py
+localstack/services/s3/v3/provider.py
+localstack/services/s3/v3/storage/__init__.py
+localstack/services/s3/v3/storage/core.py
+localstack/services/s3/v3/storage/ephemeral.py
 localstack/services/s3control/__init__.py
 localstack/services/s3control/provider.py
 localstack/services/scheduler/__init__.py
 localstack/services/scheduler/models.py
 localstack/services/scheduler/provider.py
 localstack/services/secretsmanager/__init__.py
 localstack/services/secretsmanager/provider.py
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 route53resolver:default = localstack.services.providers:route53resolver
 s3:asf = localstack.services.providers:s3_asf
 s3:default = localstack.services.providers:s3
 s3:legacy = localstack.services.providers:s3_legacy
 s3:stream = localstack.services.providers:s3_stream
 s3:v1 = localstack.services.providers:s3_v1
 s3:v2 = localstack.services.providers:s3_v2
+s3:v3 = localstack.services.providers:s3_v3
 s3control:default = localstack.services.providers:s3control
 scheduler:default = localstack.services.providers:scheduler
 secretsmanager:default = localstack.services.providers:secretsmanager
 ses:default = localstack.services.providers:ses
 sns:default = localstack.services.providers:sns
 sqs:default = localstack.services.providers:sqs
 ssm:default = localstack.services.providers:ssm
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/plux.json` & `localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/plux.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8543735224586289%*

 * *Differences: {"'localstack.aws.provider'": "{insert: [(32, 's3:v3=localstack.services.providers:s3_v3')]}",*

 * * "'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_hand […]*

```diff
@@ -28,14 +28,15 @@
         "route53resolver:default=localstack.services.providers:route53resolver",
         "s3:default=localstack.services.providers:s3",
         "s3:asf=localstack.services.providers:s3_asf",
         "s3:legacy=localstack.services.providers:s3_legacy",
         "s3:stream=localstack.services.providers:s3_stream",
         "s3:v1=localstack.services.providers:s3_v1",
         "s3:v2=localstack.services.providers:s3_v2",
+        "s3:v3=localstack.services.providers:s3_v3",
         "s3control:default=localstack.services.providers:s3control",
         "scheduler:default=localstack.services.providers:scheduler",
         "secretsmanager:default=localstack.services.providers:secretsmanager",
         "ses:default=localstack.services.providers:ses",
         "sns:default=localstack.services.providers:sns",
         "sqs:default=localstack.services.providers:sqs",
         "ssm:default=localstack.services.providers:ssm",
@@ -52,44 +53,44 @@
         "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
         "configure_edge_port=localstack.plugins:configure_edge_port",
         "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
-        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs"
+        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package"
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230808025517/localstack_core.egg-info/requires.txt` & `localstack-core-2.2.1.dev20230808030244/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/pyproject.toml` & `localstack-core-2.2.1.dev20230808030244/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808025517/setup.cfg` & `localstack-core-2.2.1.dev20230808030244/setup.cfg`

 * *Files identical despite different names*

